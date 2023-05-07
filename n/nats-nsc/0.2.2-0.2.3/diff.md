# Comparing `tmp/nats_nsc-0.2.2.tar.gz` & `tmp/nats_nsc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats_nsc-0.2.2.tar", last modified: Sat May  6 20:34:16 2023, max compression
+gzip compressed data, was "nats_nsc-0.2.3.tar", last modified: Sun May  7 19:32:17 2023, max compression
```

## Comparing `nats_nsc-0.2.2.tar` & `nats_nsc-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1071 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/LICENSE
--rw-r--r--   0        0        0      191 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/README.md
--rw-r--r--   0        0        0      730 2023-05-06 20:34:16.227260 nats_nsc-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4489 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/src/nats_nsc/__init__.py
--rw-r--r--   0        0        0     1826 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/src/nats_nsc/common.py
--rw-r--r--   0        0        0     2085 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/src/nats_nsc/nk.py
--rw-r--r--   0        0        0     6008 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/src/nats_nsc/nsc_utils.py
--rw-r--r--   0        0        0       68 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/tests/nsc_workdir/.gitignore
--rw-r--r--   0        0        0       71 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/tests/nsc_workdir/keys/DO_NOT_USE
--rw-r--r--   0        0        0       75 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/tests/nsc_workdir/nats-nsc-testing/.nsc
--rw-r--r--   0        0        0     1582 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt
--rw-r--r--   0        0        0      646 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt
--rw-r--r--   0        0        0      745 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      562 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      668 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      175 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/tests/nsc_workdir/nsc.json
--rw-r--r--   0        0        0      891 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/tests/test_nk.py
--rw-r--r--   0        0        0     1412 2023-05-06 20:33:55.598945 nats_nsc-0.2.2/tests/test_setup.py
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 nats_nsc-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/LICENSE
+-rw-r--r--   0        0        0      191 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/README.md
+-rw-r--r--   0        0        0      730 2023-05-07 19:32:17.558712 nats_nsc-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4489 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/src/nats_nsc/__init__.py
+-rw-r--r--   0        0        0     1826 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/src/nats_nsc/common.py
+-rw-r--r--   0        0        0     2085 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/src/nats_nsc/nk.py
+-rw-r--r--   0        0        0     5995 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/src/nats_nsc/nsc_utils.py
+-rw-r--r--   0        0        0       68 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/.gitignore
+-rw-r--r--   0        0        0       71 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/keys/DO_NOT_USE
+-rw-r--r--   0        0        0       75 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/.nsc
+-rw-r--r--   0        0        0     1582 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt
+-rw-r--r--   0        0        0      646 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt
+-rw-r--r--   0        0        0      745 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      562 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      668 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      175 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/nsc_workdir/nsc.json
+-rw-r--r--   0        0        0      891 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/test_nk.py
+-rw-r--r--   0        0        0     1412 2023-05-07 19:31:57.602651 nats_nsc-0.2.3/tests/test_setup.py
+-rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 nats_nsc-0.2.3/PKG-INFO
```

### Comparing `nats_nsc-0.2.2/LICENSE` & `nats_nsc-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.2/pyproject.toml` & `nats_nsc-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [tool.pytest.ini_options]
 pythonpath = [
     "src/",
 ]
 
 [project]
 name = "nats-nsc"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python wrapper for nsc, nats credential manager"
 authors = [
     { name = "Mikołaj Nowak", email = "12396461+m3nowak@users.noreply.github.com" },
 ]
 dependencies = [
     "pyJWT~=2.6.0",
     "aiofiles~=23.1.0",
```

### Comparing `nats_nsc-0.2.2/src/nats_nsc/__init__.py` & `nats_nsc-0.2.3/src/nats_nsc/__init__.py`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.2/src/nats_nsc/common.py` & `nats_nsc-0.2.3/src/nats_nsc/common.py`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.2/src/nats_nsc/nk.py` & `nats_nsc-0.2.3/src/nats_nsc/nk.py`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.2/src/nats_nsc/nsc_utils.py` & `nats_nsc-0.2.3/src/nats_nsc/nsc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     if allow_pub_response is not None:
         args.append(f'--allow-pub-response={allow_pub_response}')
     if allow_pub is not None:
         args += ['--allow-pub', shlex.quote(','.join(allow_pub))]
     if allow_pubsub is not None:
         args += ['--allow-pubsub', shlex.quote(','.join(allow_pubsub))]
     if allow_sub is not None:
-        args += ['--allow-sub', shlex.quote(','.join(allow_sub))]
+        args += ['--allow-sub', ','.join(allow_sub)]
     if bearer:
         args += ['--bearer']
     if deny_pub is not None:
         args += ['--deny-pub', shlex.quote(','.join(deny_pub))]
     if deny_pubsub is not None:
         args += ['--deny-pubsub', shlex.quote(','.join(deny_pubsub))]
     if deny_sub is not None:
```

### Comparing `nats_nsc-0.2.2/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt` & `nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.2/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt` & `nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.2/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt` & `nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.2/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt` & `nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.2/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt` & `nats_nsc-0.2.3/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.2/tests/test_nk.py` & `nats_nsc-0.2.3/tests/test_nk.py`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.2/tests/test_setup.py` & `nats_nsc-0.2.3/tests/test_setup.py`

 * *Files identical despite different names*

