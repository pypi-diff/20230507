# Comparing `tmp/nonebot-plugin-mcversion-0.1.0.tar.gz` & `tmp/nonebot-plugin-mcversion-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcversion-0.1.0.tar", last modified: Sun May  7 12:02:16 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcversion-0.1.1.tar", last modified: Sun May  7 12:15:47 2023, max compression
```

## Comparing `nonebot-plugin-mcversion-0.1.0.tar` & `nonebot-plugin-mcversion-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-05-07 12:02:07.376232 nonebot-plugin-mcversion-0.1.0/LICENSE
--rw-r--r--   0        0        0     1077 2023-05-07 12:02:07.376232 nonebot-plugin-mcversion-0.1.0/README.md
--rw-r--r--   0        0        0     4114 2023-05-07 12:02:07.376232 nonebot-plugin-mcversion-0.1.0/nonebot_plugin_mcversion/__init__.py
--rw-r--r--   0        0        0      621 2023-05-07 12:02:07.376232 nonebot-plugin-mcversion-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-07 12:15:37.356691 nonebot-plugin-mcversion-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1931 2023-05-07 12:15:37.356691 nonebot-plugin-mcversion-0.1.1/README.md
+-rw-r--r--   0        0        0     4114 2023-05-07 12:15:37.356691 nonebot-plugin-mcversion-0.1.1/nonebot_plugin_mcversion/__init__.py
+-rw-r--r--   0        0        0      621 2023-05-07 12:15:37.356691 nonebot-plugin-mcversion-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.1.1/PKG-INFO
```

### Comparing `nonebot-plugin-mcversion-0.1.0/LICENSE` & `nonebot-plugin-mcversion-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.1.0/nonebot_plugin_mcversion/__init__.py` & `nonebot-plugin-mcversion-0.1.1/nonebot_plugin_mcversion/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.1.0/pyproject.toml` & `nonebot-plugin-mcversion-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-mcversion"
-version = "0.1.0"
+version = "0.1.1"
 description = "NoneBot2 plugin for CheckMCupdate"
 authors = [
     { name = "CN171-1", email = "3428166361@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
```

