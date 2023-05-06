# Comparing `tmp/langchain_shell-0.1.0.tar.gz` & `tmp/langchain_shell-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_shell-0.1.0.tar", max compression
+gzip compressed data, was "langchain_shell-0.1.1.tar", max compression
```

## Comparing `langchain_shell-0.1.0.tar` & `langchain_shell-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-05-06 21:38:57.946649 langchain_shell-0.1.0/LICENSE
--rw-r--r--   0        0        0       48 2023-05-06 21:43:52.543889 langchain_shell-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-06 21:48:07.954438 langchain_shell-0.1.0/langchain_shell/__init__.py
--rw-r--r--   0        0        0       71 2023-05-06 21:48:59.649766 langchain_shell-0.1.0/langchain_shell/main.py
--rw-r--r--   0        0        0      388 2023-05-06 21:47:54.784783 langchain_shell-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 langchain_shell-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-06 21:38:57.946649 langchain_shell-0.1.1/LICENSE
+-rw-r--r--   0        0        0       48 2023-05-06 21:43:52.543889 langchain_shell-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 21:48:07.954438 langchain_shell-0.1.1/langchain_shell/__init__.py
+-rw-r--r--   0        0        0     1908 2023-05-06 23:36:20.809573 langchain_shell-0.1.1/langchain_shell/main.py
+-rw-r--r--   0        0        0      503 2023-05-06 23:37:57.960925 langchain_shell-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 langchain_shell-0.1.1/PKG-INFO
```

### Comparing `langchain_shell-0.1.0/LICENSE` & `langchain_shell-0.1.1/LICENSE`

 * *Files identical despite different names*

