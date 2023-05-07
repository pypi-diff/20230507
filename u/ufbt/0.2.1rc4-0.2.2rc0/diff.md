# Comparing `tmp/ufbt-0.2.1rc4.tar.gz` & `tmp/ufbt-0.2.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufbt-0.2.1rc4.tar", last modified: Sun Apr  9 23:26:44 2023, max compression
+gzip compressed data, was "ufbt-0.2.2rc0.tar", last modified: Sun May  7 15:17:13 2023, max compression
```

## Comparing `ufbt-0.2.1rc4.tar` & `ufbt-0.2.2rc0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:26:44.071512 ufbt-0.2.1rc4/
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-04-09 23:26:34.000000 ufbt-0.2.1rc4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-09 23:26:44.071512 ufbt-0.2.1rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-09 23:26:34.000000 ufbt-0.2.1rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-09 23:26:34.000000 ufbt-0.2.1rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 23:26:44.071512 ufbt-0.2.1rc4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:26:44.071512 ufbt-0.2.1rc4/ufbt/
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-09 23:26:34.000000 ufbt-0.2.1rc4/ufbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-09 23:26:34.000000 ufbt-0.2.1rc4/ufbt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26207 2023-04-09 23:26:34.000000 ufbt-0.2.1rc4/ufbt/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:26:44.071512 ufbt-0.2.1rc4/ufbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-09 23:26:44.000000 ufbt-0.2.1rc4/ufbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 23:26:44.000000 ufbt-0.2.1rc4/ufbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 23:26:44.000000 ufbt-0.2.1rc4/ufbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 23:26:44.000000 ufbt-0.2.1rc4/ufbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 23:26:44.000000 ufbt-0.2.1rc4/ufbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:17:13.476405 ufbt-0.2.2rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-05-07 15:16:55.000000 ufbt-0.2.2rc0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-07 15:17:13.472404 ufbt-0.2.2rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-07 15:16:55.000000 ufbt-0.2.2rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-07 15:16:55.000000 ufbt-0.2.2rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 15:17:13.476405 ufbt-0.2.2rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:17:13.472404 ufbt-0.2.2rc0/ufbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-07 15:16:55.000000 ufbt-0.2.2rc0/ufbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-07 15:16:55.000000 ufbt-0.2.2rc0/ufbt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26425 2023-05-07 15:16:55.000000 ufbt-0.2.2rc0/ufbt/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:17:13.472404 ufbt-0.2.2rc0/ufbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-07 15:17:13.000000 ufbt-0.2.2rc0/ufbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-07 15:17:13.000000 ufbt-0.2.2rc0/ufbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 15:17:13.000000 ufbt-0.2.2rc0/ufbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-07 15:17:13.000000 ufbt-0.2.2rc0/ufbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 15:17:13.000000 ufbt-0.2.2rc0/ufbt.egg-info/top_level.txt
```

### Comparing `ufbt-0.2.1rc4/LICENSE.md` & `ufbt-0.2.2rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc4/PKG-INFO` & `ufbt-0.2.2rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.1rc4
+Version: 0.2.2rc0
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
@@ -25,14 +25,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # uFBT - micro Flipper Build Tool
 
 uFBT is a cross-platform tool for building applications for [Flipper Zero](https://flipperzero.one/). It is a simplified version of [Flipper Build Tool (FBT)](https://github.com/flipperdevices/flipperzero-firmware/blob/dev/documentation/fbt.md).
 
+**uFBT has an [official GitHub Action](https://github.com/marketplace/actions/build-flipper-application-package-fap). With it, you can automate building and publishing your application using GitHub workflows.**
+
 uFBT enables basic development tasks for Flipper Zero, such as building and debugging applications, flashing firmware, creating VSCode development configurations. It uses prebuilt binaries and libraries, so you don't need to build [the whole firmware](https://github.com/flipperdevices/flipperzero-firmware) to compile and debug your application for Flipper.
 
 ## Installation
 
 - **Linux & macOS**: `python3 -m pip install --upgrade ufbt`
 - **Windows**: `py -m pip install --upgrade ufbt`
```

### Comparing `ufbt-0.2.1rc4/README.md` & `ufbt-0.2.2rc0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # uFBT - micro Flipper Build Tool
 
 uFBT is a cross-platform tool for building applications for [Flipper Zero](https://flipperzero.one/). It is a simplified version of [Flipper Build Tool (FBT)](https://github.com/flipperdevices/flipperzero-firmware/blob/dev/documentation/fbt.md).
 
+**uFBT has an [official GitHub Action](https://github.com/marketplace/actions/build-flipper-application-package-fap). With it, you can automate building and publishing your application using GitHub workflows.**
+
 uFBT enables basic development tasks for Flipper Zero, such as building and debugging applications, flashing firmware, creating VSCode development configurations. It uses prebuilt binaries and libraries, so you don't need to build [the whole firmware](https://github.com/flipperdevices/flipperzero-firmware) to compile and debug your application for Flipper.
 
 ## Installation
 
 - **Linux & macOS**: `python3 -m pip install --upgrade ufbt`
 - **Windows**: `py -m pip install --upgrade ufbt`
```

### Comparing `ufbt-0.2.1rc4/pyproject.toml` & `ufbt-0.2.2rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc4/ufbt/__init__.py` & `ufbt-0.2.2rc0/ufbt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,26 +57,33 @@
         print("Run `ufbt update -h` for more information on how to update.")
         return 1
 
     UFBT_APP_DIR = os.getcwd()
 
     if platform.system() == "Windows":
         commandline = (
-            'call "%UFBT_STATE_DIR%/current/scripts/toolchain/fbtenv.cmd" env & '
-            f'python -m SCons -Q --warn=target-not-built -C "%UFBT_STATE_DIR%/current/scripts/ufbt" "UFBT_APP_DIR={UFBT_APP_DIR}" '
+            r'call "%UFBT_STATE_DIR%/current/scripts/toolchain/fbtenv.cmd" env & '
+            'python -m SCons -Q --warn=target-not-built '
+            r'-C "%UFBT_STATE_DIR%/current/scripts/ufbt" '
+            f'"UFBT_APP_DIR={UFBT_APP_DIR}" '
             + " ".join(sys.argv[1:])
         )
 
     else:
         commandline = (
             '. "$UFBT_STATE_DIR/current/scripts/toolchain/fbtenv.sh" && '
-            f'python3 -m SCons -Q --warn=target-not-built -C "$UFBT_STATE_DIR/current/scripts/ufbt" "UFBT_APP_DIR={UFBT_APP_DIR}" '
+            'python3 -m SCons -Q --warn=target-not-built '
+            '-C "$UFBT_STATE_DIR/current/scripts/ufbt" '
+            f'"UFBT_APP_DIR={UFBT_APP_DIR}" '
             + " ".join(sys.argv[1:])
         )
 
     # print(commandline)
     retcode = os.system(commandline)
-    return 1 if retcode != 0 else 0
+    if platform.system() != "Windows":
+        # low byte is signal number, high byte is exit code
+        retcode = retcode >> 8
+    return retcode
 
 
 if __name__ == "__main__":
     sys.exit(ufbt_cli() or 0)
```

### Comparing `ufbt-0.2.1rc4/ufbt/__main__.py` & `ufbt-0.2.2rc0/ufbt/__main__.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc4/ufbt/bootstrap.py` & `ufbt-0.2.2rc0/ufbt/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,20 @@
 import logging
 import os
 import re
 import shutil
 import sys
 from dataclasses import dataclass, field
 from html.parser import HTMLParser
+from importlib.metadata import version
 from pathlib import Path, PurePosixPath
 from typing import ClassVar, Dict, Optional
 from urllib.parse import unquote, urlparse
 from urllib.request import Request, urlopen
 from zipfile import ZipFile
-from importlib.metadata import version
-
 
 ##############################################################################
 
 log = logging.getLogger(__name__)
 DEFAULT_UFBT_HOME = os.path.expanduser("~/.ufbt")
 
 
@@ -107,17 +106,15 @@
     # Reconstruction of loader-specific data from metadata dict
     @classmethod
     def metadata_to_init_kwargs(cls, metadata: dict) -> Dict[str, str]:
         raise NotImplementedError()
 
     # Conversion of argparse.Namespace to metadata dict
     @classmethod
-    def args_namespace_to_metadata(
-        cls, namespace: argparse.Namespace
-    ) -> Dict[str, str]:
+    def args_namespace_to_metadata(cls, args: argparse.Namespace) -> Dict[str, str]:
         raise NotImplementedError()
 
     @classmethod
     def add_args_to_mode_group(cls, mode_group):
         raise NotImplementedError()
 
 
@@ -195,20 +192,18 @@
             "branch": metadata["branch"],
             "branch_root_url": metadata.get(
                 "branch_root", BranchSdkLoader.UPDATE_SERVER_BRANCH_ROOT
             ),
         }
 
     @classmethod
-    def args_namespace_to_metadata(
-        cls, namespace: argparse.Namespace
-    ) -> Dict[str, str]:
+    def args_namespace_to_metadata(cls, args: argparse.Namespace) -> Dict[str, str]:
         return {
-            "branch": namespace.branch,
-            "branch_root": namespace.index_url,
+            "branch": args.branch,
+            "branch_root": args.index_url,
         }
 
     @classmethod
     def add_args_to_mode_group(cls, mode_group):
         mode_group.add_argument(
             "--branch",
             "-b",
@@ -262,15 +257,15 @@
         log.info(f"Using version: {versions[0]['version']}")
         log.debug(f"Changelog: {versions[0].get('changelog', 'None')}")
         return versions[0]
 
     @staticmethod
     def _get_file_info(version_data: dict, file_type: FileType, file_target: str):
         if not (files := version_data.get("files", [])):
-            raise ValueError(f"Empty files list")
+            raise ValueError("Empty files list")
 
         if not (
             file_info := next(
                 (
                     f
                     for f in files
                     if f["type"] == file_type.value and f["target"] == file_target
@@ -281,15 +276,15 @@
             raise ValueError(f"Invalid file type: {file_type}")
 
         return file_info
 
     def get_sdk_component(self, target: str) -> str:
         file_info = self._get_file_info(self.version_info, FileType.SDK_ZIP, target)
         if not (file_url := file_info.get("url", None)):
-            raise ValueError(f"Invalid file url")
+            raise ValueError("Invalid file url")
 
         return self._fetch_file(file_url)
 
     def get_metadata(self) -> Dict[str, str]:
         return {
             "mode": self.LOADER_MODE_KEY,
             "channel": self.channel.name.lower(),
@@ -303,20 +298,18 @@
             "channel": UpdateChannelSdkLoader.UpdateChannel[
                 metadata["channel"].upper()
             ],
             "json_index_url": metadata.get("json_index", None),
         }
 
     @classmethod
-    def args_namespace_to_metadata(
-        cls, namespace: argparse.Namespace
-    ) -> Dict[str, str]:
+    def args_namespace_to_metadata(cls, args: argparse.Namespace) -> Dict[str, str]:
         return {
-            "channel": namespace.channel,
-            "json_index": namespace.index_url,
+            "channel": args.channel,
+            "json_index": args.index_url,
         }
 
     @classmethod
     def add_args_to_mode_group(cls, mode_group):
         mode_group.add_argument(
             "--channel",
             "-c",
@@ -349,18 +342,18 @@
         }
 
     @classmethod
     def metadata_to_init_kwargs(cls, metadata: dict) -> Dict[str, str]:
         return {"url": metadata["url"]}
 
     @classmethod
-    def args_namespace_to_metadata(
-        cls, namespace: argparse.Namespace
-    ) -> Dict[str, str]:
-        return {"url": namespace.url}
+    def args_namespace_to_metadata(cls, args: argparse.Namespace) -> Dict[str, str]:
+        if args.url and not args.hw_target:
+            raise ValueError("HW target must be specified when using direct SDK URL")
+        return {"url": args.url}
 
     @classmethod
     def add_args_to_mode_group(cls, mode_group):
         mode_group.add_argument(
             "--url",
             "-u",
             type=str,
@@ -392,21 +385,25 @@
 
     @classmethod
     def metadata_to_init_kwargs(cls, metadata: dict) -> Dict[str, str]:
         return {"file_path": metadata["file_path"]}
 
     @classmethod
     def args_namespace_to_metadata(cls, args: argparse.Namespace) -> Dict[str, str]:
-        return {"file_path": args.local}
+        if args.local:
+            if not args.hw_target:
+                raise ValueError("HW target must be specified when using local SDK")
+            return {"file_path": str(Path(args.local).absolute())}
+        return {}
 
     @classmethod
     def add_args_to_mode_group(cls, mode_group):
         mode_group.add_argument(
-            f"--local",
-            f"-l",
+            "--local",
+            "-l",
             type=str,
             help="Path to local SDK zip file",
         )
 
 
 all_boostrap_loader_cls = (
     BranchSdkLoader,
@@ -522,15 +519,15 @@
         log.info(f"uFBT SDK dir: {sdk_target_dir}")
         if not task.force and os.path.exists(sdk_target_dir):
             # Read existing state
             with open(self.state_file, "r") as f:
                 ufbt_state = json.load(f)
             # Check if we need to update
             if ufbt_state.get("version") in sdk_loader.ALWAYS_UPDATE_VERSIONS:
-                log.info("Cannot determine SDK version, updating")
+                log.info("Cannot determine current SDK version, updating")
             elif (
                 ufbt_state.get("version") == sdk_loader.get_metadata().get("version")
                 and ufbt_state.get("hw_target") == task.hw_target
             ):
                 log.info("SDK is up-to-date")
                 return True
 
@@ -543,15 +540,15 @@
         shutil.rmtree(sdk_target_dir, ignore_errors=True)
 
         ufbt_state = {
             "hw_target": task.hw_target,
             **sdk_loader.get_metadata(),
         }
 
-        log.info(f"Deploying SDK")
+        log.info("Deploying SDK")
 
         with ZipFile(sdk_component_path, "r") as zip_file:
             zip_file.extractall(sdk_target_dir)
 
         with open(self.state_file, "w") as f:
             json.dump(ufbt_state, f, indent=4)
         log.info("SDK deployed.")
```

### Comparing `ufbt-0.2.1rc4/ufbt.egg-info/PKG-INFO` & `ufbt-0.2.2rc0/ufbt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.1rc4
+Version: 0.2.2rc0
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
@@ -25,14 +25,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # uFBT - micro Flipper Build Tool
 
 uFBT is a cross-platform tool for building applications for [Flipper Zero](https://flipperzero.one/). It is a simplified version of [Flipper Build Tool (FBT)](https://github.com/flipperdevices/flipperzero-firmware/blob/dev/documentation/fbt.md).
 
+**uFBT has an [official GitHub Action](https://github.com/marketplace/actions/build-flipper-application-package-fap). With it, you can automate building and publishing your application using GitHub workflows.**
+
 uFBT enables basic development tasks for Flipper Zero, such as building and debugging applications, flashing firmware, creating VSCode development configurations. It uses prebuilt binaries and libraries, so you don't need to build [the whole firmware](https://github.com/flipperdevices/flipperzero-firmware) to compile and debug your application for Flipper.
 
 ## Installation
 
 - **Linux & macOS**: `python3 -m pip install --upgrade ufbt`
 - **Windows**: `py -m pip install --upgrade ufbt`
```

