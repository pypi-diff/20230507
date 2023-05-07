# Comparing `tmp/gsem-0.2.2.tar.gz` & `tmp/gsem-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsem-0.2.2.tar", max compression
+gzip compressed data, was "gsem-0.2.3.tar", max compression
```

## Comparing `gsem-0.2.2.tar` & `gsem-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1080 2021-03-02 15:43:46.775403 gsem-0.2.2/LICENSE
--rw-r--r--   0        0        0     2275 2021-03-06 18:06:15.705343 gsem-0.2.2/README.md
--rw-r--r--   0        0        0        0 2021-03-02 15:43:46.775403 gsem-0.2.2/gsem/__init__.py
--rw-r--r--   0        0        0     7367 2021-03-06 21:34:32.526484 gsem-0.2.2/gsem/cli.py
--rw-r--r--   0        0        0      300 2021-03-06 16:10:10.078537 gsem-0.2.2/gsem/config.py
--rw-r--r--   0        0        0     5722 2021-03-06 21:34:32.526484 gsem-0.2.2/gsem/extension.py
--rw-r--r--   0        0        0     1612 2021-03-06 16:10:10.078537 gsem-0.2.2/gsem/utils.py
--rw-r--r--   0        0        0      936 2021-03-06 21:35:50.136658 gsem-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3115 2021-03-06 21:37:18.720697 gsem-0.2.2/setup.py
--rw-r--r--   0        0        0     3042 2021-03-06 21:37:18.720968 gsem-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-07 08:40:42.949771 gsem-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2279 2023-05-07 08:40:42.949771 gsem-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 08:40:42.949771 gsem-0.2.3/gsem/__init__.py
+-rw-r--r--   0        0        0     7367 2023-05-07 08:40:42.949771 gsem-0.2.3/gsem/cli.py
+-rw-r--r--   0        0        0      300 2023-05-07 08:40:42.949771 gsem-0.2.3/gsem/config.py
+-rw-r--r--   0        0        0     5746 2023-05-07 08:40:42.949771 gsem-0.2.3/gsem/extension.py
+-rw-r--r--   0        0        0     1612 2023-05-07 08:40:42.949771 gsem-0.2.3/gsem/utils.py
+-rw-r--r--   0        0        0      932 2023-05-07 08:42:24.833432 gsem-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 gsem-0.2.3/PKG-INFO
```

### Comparing `gsem-0.2.2/LICENSE` & `gsem-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gsem-0.2.2/README.md` & `gsem-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ### Global installation
 Run `sudo pip install gsem`
 
 ### Updating the package
 
 Run `pip install -U --user gsem` for user installation or `sudo pip install -U gsem` for global installation.
 
-## DONE:
+## Features:
 * list installed
 * list enabled/disabled
 * list outdated
 * extension info
 * search
 * enable/disable
 * install/uninstall/reinstall
```

### Comparing `gsem-0.2.2/gsem/cli.py` & `gsem-0.2.3/gsem/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         if args.uuid not in manager.installed_uuids():
             print(f"'{args.uuid}' is not installed")
         else:
             print(f"Uninstalling '{args.uuid}'")
             manager.uninstall(args.uuid)
     elif args.cmd == "update":
         outdated = manager.outdated()
-        print(f"Extension updates avaliable ({len(outdated)})")
+        print(f"Extension updates available ({len(outdated)})")
         if outdated:
             lines = [f"{e.uuid} {e.version} -> {e.remote_version}" for e in outdated]
             print_nice_list(lines)
             prompt = input("Would you like to install these updates? (yes) ")
             if prompt.lower().strip().startswith("y"):
                 for e in outdated:
                     was_enabled = e.is_enabled
```

### Comparing `gsem-0.2.2/gsem/extension.py` & `gsem-0.2.3/gsem/extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,15 +123,16 @@
             for uuid in set(self.installed_uuids()).difference(enabled_uuids)
         ]
 
     def outdated(self) -> List[Extension]:
         # TODO: use https://extensions.gnome.org/update-info/?installed={%22arch-update@RaphaelRochet%22:{%22version%22:6}}&shell_version=3.18.3  # noqa
         return [e for e in self.installed() if e.is_outdated]
 
-    def search(self, term: str, shell_version: str = "all") -> List[Extension]:
+    @staticmethod
+    def search(term: str, shell_version: str = "all") -> List[Extension]:
         query = {
             "shell_version": shell_version,
             "search": term,
         }
         response = get_json_response(API_SEARCH, query)
         found = []
         for remote_meta in response["extensions"]:
@@ -163,15 +164,16 @@
         enabled_uuids.remove(uuid)
         Gio.Settings("org.gnome.shell").set_value(
             "enabled-extensions",
             GLib.Variant("as", list(enabled_uuids)),
         )
         return True
 
-    def install(self, uuid: str) -> Extension:
+    @staticmethod
+    def install(uuid: str) -> Extension:
         ext = Extension(uuid)
         download_url = API_ROOT + ext.remote_meta["download_url"]
         dest_dir = os.path.join(EXTENSION_DIR, uuid)
         download_and_extract_zip(download_url, dest_dir)
         return ext
 
     def uninstall(self, uuid: str) -> None:
```

### Comparing `gsem-0.2.2/gsem/utils.py` & `gsem-0.2.3/gsem/utils.py`

 * *Files identical despite different names*

### Comparing `gsem-0.2.2/pyproject.toml` & `gsem-0.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "gsem"
-version = "0.2.2"
+version = "0.2.3"
 description = "Command line extension manager for Gnome-Shell"
 authors = ["Andrii Kohut <kogut.andriy@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/andriykohut/gsem"
 repository = "https://github.com/andriykohut/gsem"
 
 keywords = ["gnome-shell", "gnome", "cli", "command-line-tool", "gnome-shell-extension"]
 classifiers = ["Topic :: Desktop Environment :: Gnome"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-PyGObject = "^3.38.0"
+python = ">=3.7"
+PyGObject = ">=3.0"
 
 [tool.poetry.dev-dependencies]
-black = "^20.8b1"
-flake8 = "^3.8.4"
-mypy = "^0.812"
-pre-commit = "^2.10.1"
-isort = "^5.7.0"
+black = "^23.3"
+flake8 = "^5.0.4"
+mypy = "^1.2"
+pre-commit = "^2.21.0"
+isort = "^5.11.5"
 
 [tool.poetry.scripts]
 gsem = "gsem.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gsem-0.2.2/setup.py` & `gsem-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,102 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gsem
+Version: 0.2.3
+Summary: Command line extension manager for Gnome-Shell
+Home-page: https://github.com/andriykohut/gsem
+License: MIT
+Keywords: gnome-shell,gnome,cli,command-line-tool,gnome-shell-extension
+Author: Andrii Kohut
+Author-email: kogut.andriy@gmail.com
+Requires-Python: >=3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Desktop Environment :: Gnome
+Requires-Dist: PyGObject (>=3.0)
+Project-URL: Repository, https://github.com/andriykohut/gsem
+Description-Content-Type: text/markdown
+
+# gsem
+
+[![PyPI version](https://badge.fury.io/py/gsem.svg)](https://pypi.org/project/gsem/)
+
+*gsem* - Command line extension manager for Gnome-Shell
+
+```
+usage: gsem [-h]
+            {ls,enabled,disabled,outdated,info,install,reinstall,uninstall,update,search,enable,disable}
+            ...
+
+Gnome-Shell extension manager
+
+positional arguments:
+  {ls,enabled,disabled,outdated,info,install,reinstall,uninstall,update,search,enable,disable}
+    ls                  list installed extensions
+    enabled             list enabled extensions
+    disabled            list disabled extensions
+    outdated            list outdated extensions
+    info                show extension information
+    install             install extension
+    reinstall           reinstall extension
+    uninstall           uninstall extension
+    update              update extensions
+    search              search extensions
+    enable              enable extension
+    disable             disable extension
+
+optional arguments:
+  -h, --help            show this help message and exit
+```
+
+## Installation
+
+### User installation (recommended)
+Run `pip install --user gsem`
+
+Make sure you have `"$HOME/.local/bin"` in your `$PATH`.
+
+### Global installation
+Run `sudo pip install gsem`
+
+### Updating the package
+
+Run `pip install -U --user gsem` for user installation or `sudo pip install -U gsem` for global installation.
+
+## Features:
+* list installed
+* list enabled/disabled
+* list outdated
+* extension info
+* search
+* enable/disable
+* install/uninstall/reinstall
+* update
+
+## Contributing
+
+Development on latest python version is preferred, as of now it's 3.9.
+To start you'll need the following setup:
+
+Example uses pyenv to install latest python and manage virtualenv. Run the following commands from the root of the repository.
+
+```sh
+pyenv install 3.9.2           # install latest python version
+pyenv virtualenv 3.9.2 gsem   # create gsem virtual environment
+pyenv activate gsem           # activate the venv
+pyenv local gsem              # set local python version for the repo
+poetry install                # install all dependencies inside the virtual environment
+pre-commit install            # install pre-commit hooks
+```
+
+Run all the linters:
+```sh
+pre-commit run -a
+```
 
-packages = \
-['gsem']
+## TODO:
+* pin
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyGObject>=3.38.0,<4.0.0']
-
-entry_points = \
-{'console_scripts': ['gsem = gsem.cli:main']}
-
-setup_kwargs = {
-    'name': 'gsem',
-    'version': '0.2.2',
-    'description': 'Command line extension manager for Gnome-Shell',
-    'long_description': '# gsem\n\n[![PyPI version](https://badge.fury.io/py/gsem.svg)](https://pypi.org/project/gsem/)\n\n*gsem* - Command line extension manager for Gnome-Shell\n\n```\nusage: gsem [-h]\n            {ls,enabled,disabled,outdated,info,install,reinstall,uninstall,update,search,enable,disable}\n            ...\n\nGnome-Shell extension manager\n\npositional arguments:\n  {ls,enabled,disabled,outdated,info,install,reinstall,uninstall,update,search,enable,disable}\n    ls                  list installed extensions\n    enabled             list enabled extensions\n    disabled            list disabled extensions\n    outdated            list outdated extensions\n    info                show extension information\n    install             install extension\n    reinstall           reinstall extension\n    uninstall           uninstall extension\n    update              update extensions\n    search              search extensions\n    enable              enable extension\n    disable             disable extension\n\noptional arguments:\n  -h, --help            show this help message and exit\n```\n\n## Installation\n\n### User installation (recommended)\nRun `pip install --user gsem`\n\nMake sure you have `"$HOME/.local/bin"` in your `$PATH`.\n\n### Global installation\nRun `sudo pip install gsem`\n\n### Updating the package\n\nRun `pip install -U --user gsem` for user installation or `sudo pip install -U gsem` for global installation.\n\n## DONE:\n* list installed\n* list enabled/disabled\n* list outdated\n* extension info\n* search\n* enable/disable\n* install/uninstall/reinstall\n* update\n\n## Contributing\n\nDevelopment on latest python version is preferred, as of now it\'s 3.9.\nTo start you\'ll need the following setup:\n\nExample uses pyenv to install latest python and manage virtualenv. Run the following commands from the root of the repository.\n\n```sh\npyenv install 3.9.2           # install latest python version\npyenv virtualenv 3.9.2 gsem   # create gsem virtual environment\npyenv activate gsem           # activate the venv\npyenv local gsem              # set local python version for the repo\npoetry install                # install all dependencies inside the virtual environment\npre-commit install            # install pre-commit hooks\n```\n\nRun all the linters:\n```sh\npre-commit run -a\n```\n\n## TODO:\n* pin\n',
-    'author': 'Andrii Kohut',
-    'author_email': 'kogut.andriy@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/andriykohut/gsem',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

