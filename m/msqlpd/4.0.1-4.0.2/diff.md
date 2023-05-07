# Comparing `tmp/msqlpd-4.0.1.tar.gz` & `tmp/msqlpd-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msqlpd-4.0.1.tar", last modified: Mon Feb  6 21:34:59 2023, max compression
+gzip compressed data, was "msqlpd-4.0.2.tar", last modified: Sun May  7 10:59:50 2023, max compression
```

## Comparing `msqlpd-4.0.1.tar` & `msqlpd-4.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-06 21:34:59.754188 msqlpd-4.0.1/
--rwxrwxrwx   0 root         (0) root         (0)     1071 2022-07-21 12:54:01.000000 msqlpd-4.0.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      278 2023-02-06 21:34:59.754049 msqlpd-4.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      107 2023-02-06 21:34:59.000000 msqlpd-4.0.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-06 21:34:59.752419 msqlpd-4.0.1/msqlpd/
--rwxrwxrwx   0 root         (0) root         (0)       36 2022-10-18 10:06:35.000000 msqlpd-4.0.1/msqlpd/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-06 21:34:59.753673 msqlpd-4.0.1/msqlpd/src/
--rwxrwxrwx   0 root         (0) root         (0)    13819 2022-11-16 15:33:41.000000 msqlpd-4.0.1/msqlpd/src/connection.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-06 21:34:59.753457 msqlpd-4.0.1/msqlpd.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      278 2023-02-06 21:34:59.000000 msqlpd-4.0.1/msqlpd.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      190 2023-02-06 21:34:59.000000 msqlpd-4.0.1/msqlpd.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-02-06 21:34:59.000000 msqlpd-4.0.1/msqlpd.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-02-06 21:34:59.000000 msqlpd-4.0.1/msqlpd.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-02-06 21:34:59.754236 msqlpd-4.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      409 2023-02-06 21:33:20.000000 msqlpd-4.0.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 10:59:50.036565 msqlpd-4.0.2/
+-rwxrwxrwx   0 root         (0) root         (0)     1071 2023-05-07 10:45:43.000000 msqlpd-4.0.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      278 2023-05-07 10:59:50.034992 msqlpd-4.0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      107 2023-05-07 10:59:48.000000 msqlpd-4.0.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 10:59:50.026114 msqlpd-4.0.2/msqlpd/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-05-07 10:45:43.000000 msqlpd-4.0.2/msqlpd/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 10:59:50.032804 msqlpd-4.0.2/msqlpd/src/
+-rwxrwxrwx   0 root         (0) root         (0)    13819 2023-05-07 10:45:43.000000 msqlpd-4.0.2/msqlpd/src/connection.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 10:59:50.032068 msqlpd-4.0.2/msqlpd.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      278 2023-05-07 10:59:49.000000 msqlpd-4.0.2/msqlpd.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      219 2023-05-07 10:59:49.000000 msqlpd-4.0.2/msqlpd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-07 10:59:49.000000 msqlpd-4.0.2/msqlpd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-07 10:59:49.000000 msqlpd-4.0.2/msqlpd.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-07 10:59:49.000000 msqlpd-4.0.2/msqlpd.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-07 10:59:50.036981 msqlpd-4.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      512 2023-05-07 10:49:24.000000 msqlpd-4.0.2/setup.py
```

### Comparing `msqlpd-4.0.1/LICENSE` & `msqlpd-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `msqlpd-4.0.1/msqlpd/src/connection.py` & `msqlpd-4.0.2/msqlpd/src/connection.py`

 * *Files identical despite different names*

