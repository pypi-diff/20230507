# Comparing `tmp/wombatoo-0.0.3.tar.gz` & `tmp/wombatoo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Prashant\Desktop\wombatoo\dist\.tmp-lp21ilpl\wombatoo-0.0.3.tar", last modified: Sun May  7 09:06:48 2023, max compression
+gzip compressed data, was "C:\Users\Prashant\Desktop\wombatoo\dist\.tmp-u2sywo3k\wombatoo-0.0.4.tar", last modified: Sun May  7 09:40:34 2023, max compression
```

## Comparing `wombatoo-0.0.3.tar` & `wombatoo-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 09:06:48.000000 wombatoo-0.0.3/
--rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombatoo-0.0.3/LICENSE.md
--rw-rw-rw-   0        0        0      320 2023-05-07 09:06:48.000000 wombatoo-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombatoo-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-07 09:06:48.000000 wombatoo-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      887 2023-05-07 09:04:28.000000 wombatoo-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:06:48.000000 wombatoo-0.0.3/wombatoo.egg-info/
--rw-rw-rw-   0        0        0      320 2023-05-07 09:06:48.000000 wombatoo-0.0.3/wombatoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-05-07 09:06:48.000000 wombatoo-0.0.3/wombatoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 09:06:48.000000 wombatoo-0.0.3/wombatoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-07 09:06:48.000000 wombatoo-0.0.3/wombatoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 09:06:48.000000 wombatoo-0.0.3/wombatoo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 09:40:34.000000 wombatoo-0.0.4/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombatoo-0.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0      409 2023-05-07 09:40:34.000000 wombatoo-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombatoo-0.0.4/README.md
+-rw-rw-rw-   0        0        0      446 2023-05-07 09:39:33.000000 wombatoo-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 09:40:34.000000 wombatoo-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 09:40:34.000000 wombatoo-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 09:40:34.000000 wombatoo-0.0.4/src/wombatoo/
+-rw-rw-rw-   0        0        0        0 2023-05-01 07:27:57.000000 wombatoo-0.0.4/src/wombatoo/__init__.py
+-rw-rw-rw-   0        0        0     9597 2023-05-03 03:53:25.000000 wombatoo-0.0.4/src/wombatoo/wombatoo.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:40:34.000000 wombatoo-0.0.4/src/wombatoo.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-05-07 09:40:34.000000 wombatoo-0.0.4/src/wombatoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-07 09:40:34.000000 wombatoo-0.0.4/src/wombatoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 09:40:34.000000 wombatoo-0.0.4/src/wombatoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 09:40:34.000000 wombatoo-0.0.4/src/wombatoo.egg-info/top_level.txt
```

### Comparing `wombatoo-0.0.3/LICENSE.md` & `wombatoo-0.0.4/LICENSE.md`

 * *Files identical despite different names*

