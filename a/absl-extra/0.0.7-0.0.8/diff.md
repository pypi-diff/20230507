# Comparing `tmp/absl_extra-0.0.7.tar.gz` & `tmp/absl_extra-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.7.tar", last modified: Sun Apr 30 14:03:04 2023, max compression
+gzip compressed data, was "absl_extra-0.0.8.tar", last modified: Sat May  6 22:23:13 2023, max compression
```

## Comparing `absl_extra-0.0.7.tar` & `absl_extra-0.0.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1404 2023-04-30 14:02:55.689952 absl_extra-0.0.7/Readme.md
--rw-r--r--   0        0        0     5647 2023-04-30 14:02:55.689952 absl_extra-0.0.7/absl_extra.py
--rw-r--r--   0        0        0     6066 2023-04-30 14:02:55.689952 absl_extra-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2140 1970-01-01 00:00:00.000000 absl_extra-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1299 2023-05-06 22:23:04.204153 absl_extra-0.0.8/Readme.md
+-rw-r--r--   0        0        0     6326 2023-05-06 22:23:04.204153 absl_extra-0.0.8/absl_extra.py
+-rw-r--r--   0        0        0      689 2023-05-06 22:23:04.204153 absl_extra-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1987 1970-01-01 00:00:00.000000 absl_extra-0.0.8/PKG-INFO
```

### Comparing `absl_extra-0.0.7/Readme.md` & `absl_extra-0.0.8/Readme.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,37 +7,32 @@
   - I prefer receiving those in Slack, though (see example below).
 - Log parsed CLI flags from `absl.flags.FLAGS` and config values from `config_file:get_config()`
 - Inject `ml_collections.ConfigDict` from `config_file`, if kwarg provided.
 - Inject `pymongo.collection.Collection` if `mongo_config` kwarg provided.
 - `log_after` and `log_before` decorators, which proved extremely usefully for print-debugging.
 
 Minimal example
+
 ```python
 import os
-import functools
 from pymongo.collection import Collection
-from absl import flags, app
 from ml_collections import ConfigDict
-from absl_extra import hook_main, SlackNotifier, MongoConfig
+from absl import logging
+from absl_extra import register_task, SlackBaseNotifier, MongoConfig, run
 
 
-FLAGS = flags.FLAGS
-flags.DEFINE_integer("some_flag", default=4, help=None)
+@register_task
+def main(config: ConfigDict, db: Collection) -> None:
+    logging.info("Doing some heavy lifting...")
 
-@functools.partial(
-    hook_main,
-    app_name="some_name",
-    config_file="config.py",
-    mongo_config=MongoConfig(
-        uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
-    ),
-    notifier=SlackNotifier(
-        slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
-    ),
-)
-def main(cmd: str, config: ConfigDict, db: Collection) -> None:
-    # Do all the heavy lifting. 
-    pass
 
 if __name__ == "__main__":
-    app.run(main)
+    run(
+        config_file="config.py",
+        mongo_config=MongoConfig(
+            uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
+        ),
+        notifier=SlackBaseNotifier(
+            slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
+        ),
+    )
 ```
```

### Comparing `absl_extra-0.0.7/absl_extra.py` & `absl_extra-0.0.8/absl_extra.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 from __future__ import annotations
 
-import functools
+import inspect
 import json
+from functools import wraps, partial
 from importlib import util
 from typing import Callable, NamedTuple, TypeVar, Mapping
-from functools import wraps
+
 from absl import app, flags, logging
-import inspect
 
 T = TypeVar("T", bound=Callable, covariant=True)
+FLAGS = flags.FLAGS
 
+flags.DEFINE_string("task", default="main", help="Name of task to run.")
 
 if util.find_spec("pymongo"):
     from pymongo import MongoClient
 else:
     logging.warning("pymongo not installed.")
 
-
 if util.find_spec("ml_collections"):
     from ml_collections import config_flags
 else:
     logging.warning("ml_collections not installed")
 
 
 class MongoConfig(NamedTuple):
     uri: str
     db_name: str
     collection: str | None = None
 
 
-class Notifier:
+class BaseNotifier:
     def notify_job_started(self, name: str):
         logging.info(f"Job {name} started.")
 
     def notify_job_finished(self, name: str):
         logging.info(f"Job {name} finished.")
 
     def notify_job_failed(self, name: str, exception: Exception):
         logging.fatal(f"Job {name} failed", exc_info=exception)
 
 
 if util.find_spec("slack_sdk"):
     import slack_sdk
 
-    class SlackNotifier(Notifier):
+    class SlackBaseNotifier(BaseNotifier):
         def __init__(self, slack_token: str, channel_id: str):
             self.slack_token = slack_token
             self.channel_id = channel_id
 
         def notify_job_started(self, name: str):
             slack_client = slack_sdk.WebClient(token=self.slack_token)
             slack_client.chat_postMessage(
@@ -97,87 +98,111 @@
             )
 
 else:
     logging.warning("slack_sdk not installed.")
 
 
 class ExceptionHandlerImpl(app.ExceptionHandler):
-    def __init__(self, name: str, notifier: Notifier):
+    def __init__(self, name: str, notifier: BaseNotifier):
         self.name = name
         self.notifier = notifier
 
     def handle(self, exception: Exception):
         self.notifier.notify_job_failed(self.name, exception)
 
 
-def hook_main(
-    main: Callable,
-    *,
-    app_name: str = "absl_app",
-    notifier: Notifier | None = None,
-    config_file: str | None = None,
-    mongo_config: MongoConfig | Mapping[str, ...] | None = None,
-) -> Callable:
-    main_kwargs = {}
+def log_before(func: T, logger=logging.debug) -> T:
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        func_args = inspect.signature(func).bind(*args, **kwargs).arguments
+        func_args_str = ", ".join(map("{0[0]} = {0[1]!r}".format, func_args.items()))
+        logger(
+            f"Entered {func.__module__}.{func.__qualname__} with args ( {func_args_str} )"
+        )
+        return func(*args, **kwargs)
 
-    if notifier is None:
-        notifier = Notifier()
-    if util.find_spec("ml_collections") and config_file is not None:
-        config = config_flags.DEFINE_config_file("config")
-        main_kwargs["config"] = config.value
-    else:
-        config = None
+    return wrapper
+
+
+def log_after(func: T, logger=logging.debug) -> T:
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        retval = func(*args, **kwargs)
+        logger("Exited " + func.__name__ + "() with value: " + repr(retval))
+        return retval
+
+    return wrapper
+
+
+TASKS = {}
 
-    if util.find_spec("pymongo") and mongo_config is not None:
-        if isinstance(mongo_config, Mapping):
-            mongo_config = MongoConfig(**mongo_config)
-        db = MongoClient(mongo_config.uri).get_database(mongo_config.db_name)
-        if mongo_config.collection is not None:
-            db = db.get_collection(mongo_config.collection)
-        main_kwargs["db"] = db
 
-    def init_callback():
+def register_task(fn: Callable, name: str | Callable[[], str] = "main"):
+    if isinstance(name, Callable):
+        name = name()
+    if name in TASKS:
+        raise RuntimeError(f"Can't register 2 tasks with same name: {name}")
+    TASKS[name] = fn
+
+
+def hook_task(
+    task: Callable, task_name: str, notifier: BaseNotifier, config_file: str | None
+) -> Callable:
+    @wraps(task)
+    def wrapper(*, db=None):
         logging.info("-" * 50)
         logging.info(
             f"Flags: {json.dumps(flags.FLAGS.flag_values_dict(), sort_keys=True, indent=4)}"
         )
+        if util.find_spec("ml_collections") and config_file is not None:
+            config = config_flags.DEFINE_config_file(config_file)
+        else:
+            config = None
+
         if config is not None:
             logging.info(
                 f"Config: {json.dumps(config.value, sort_keys=True, indent=4)}"
             )
         logging.info("-" * 50)
+        notifier.notify_job_started(task_name)
 
-        notifier.notify_job_started(app_name)
-
-    app.install_exception_handler(ExceptionHandlerImpl(app_name, notifier))
-    app.call_after_init(init_callback)
+        kwargs = {}
+        if db is not None:
+            kwargs["db"] = db
+        if config is not None:
+            kwargs["config"] = config
 
-    @wraps(main)
-    def wrapper(*args, **kwargs):
-        ret_val = main(*args, **kwargs)
-        notifier.notify_job_finished(app_name)
+        ret_val = task(**kwargs)
+        notifier.notify_job_finished(task_name)
         return ret_val
 
-    return functools.partial(wrapper, **main_kwargs)
+    return wrapper
 
 
-def log_before(func: T, logger=logging.debug) -> T:
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        func_args = inspect.signature(func).bind(*args, **kwargs).arguments
-        func_args_str = ", ".join(map("{0[0]} = {0[1]!r}".format, func_args.items()))
-        logger(
-            f"Entered {func.__module__}.{func.__qualname__} with args ( {func_args_str} )"
-        )
-        return func(*args, **kwargs)
+def pseudo_main(cmd, **kwargs):
+    TASKS[FLAGS.task](**kwargs)
 
-    return wrapper
 
+def run(
+    app_name: str | Callable[[], str] = "app",
+    notifier: BaseNotifier | None = None,
+    config_file: str | None = None,
+    mongo_config: MongoConfig | Mapping[str, ...] | None = None,
+):
+    if notifier is None:
+        notifier = BaseNotifier()
 
-def log_after(func: T, logger=logging.debug) -> T:
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        retval = func(*args, **kwargs)
-        logger("Exited " + func.__name__ + "() with value: " + repr(retval))
-        return retval
+    if util.find_spec("pymongo") and mongo_config is not None:
+        if isinstance(mongo_config, Mapping):
+            mongo_config = MongoConfig(**mongo_config)
+        db = MongoClient(mongo_config.uri).get_database(mongo_config.db_name)
+        if mongo_config.collection is not None:
+            db = db.get_collection(mongo_config.collection)
+    else:
+        db = None
 
-    return wrapper
+    app.install_exception_handler(ExceptionHandlerImpl(app_name, notifier))
+    global TASKS
+    TASKS = {
+        k: hook_task(v, k, notifier, config_file=config_file) for k, v in TASKS.items()
+    }
+    app.run(partial(pseudo_main, db=db))
```

### Comparing `absl_extra-0.0.7/PKG-INFO` & `absl_extra-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.7
+Version: 0.0.8
 Summary: A wrapper to run and monitor absl app.
-Keywords: 
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: absl_py
 Requires-Dist: black ; extra == "dev"
-Requires-Dist: mypy ; extra == "dev"
 Requires-Dist: ml_collections ; extra == "ml_collections"
 Requires-Dist: pymongo ; extra == "mongo"
 Requires-Dist: slack_sdk ; extra == "slack"
 Project-URL: Homepage, https://github.com/aaarrti/absl_extra
 Provides-Extra: dev
 Provides-Extra: ml_collections
 Provides-Extra: mongo
@@ -29,38 +27,33 @@
   - I prefer receiving those in Slack, though (see example below).
 - Log parsed CLI flags from `absl.flags.FLAGS` and config values from `config_file:get_config()`
 - Inject `ml_collections.ConfigDict` from `config_file`, if kwarg provided.
 - Inject `pymongo.collection.Collection` if `mongo_config` kwarg provided.
 - `log_after` and `log_before` decorators, which proved extremely usefully for print-debugging.
 
 Minimal example
+
 ```python
 import os
-import functools
 from pymongo.collection import Collection
-from absl import flags, app
 from ml_collections import ConfigDict
-from absl_extra import hook_main, SlackNotifier, MongoConfig
+from absl import logging
+from absl_extra import register_task, SlackBaseNotifier, MongoConfig, run
 
 
-FLAGS = flags.FLAGS
-flags.DEFINE_integer("some_flag", default=4, help=None)
+@register_task
+def main(config: ConfigDict, db: Collection) -> None:
+    logging.info("Doing some heavy lifting...")
 
-@functools.partial(
-    hook_main,
-    app_name="some_name",
-    config_file="config.py",
-    mongo_config=MongoConfig(
-        uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
-    ),
-    notifier=SlackNotifier(
-        slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
-    ),
-)
-def main(cmd: str, config: ConfigDict, db: Collection) -> None:
-    # Do all the heavy lifting. 
-    pass
 
 if __name__ == "__main__":
-    app.run(main)
+    run(
+        config_file="config.py",
+        mongo_config=MongoConfig(
+            uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
+        ),
+        notifier=SlackBaseNotifier(
+            slack_token=os.environ["SLACK_BOT_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
+        ),
+    )
 ```
```

