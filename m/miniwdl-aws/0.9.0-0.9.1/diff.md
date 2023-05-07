# Comparing `tmp/miniwdl-aws-0.9.0.tar.gz` & `tmp/miniwdl-aws-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniwdl-aws-0.9.0.tar", last modified: Sat Jan 28 10:21:46 2023, max compression
+gzip compressed data, was "miniwdl-aws-0.9.1.tar", last modified: Wed Feb  8 08:00:51 2023, max compression
```

## Comparing `miniwdl-aws-0.9.0.tar` & `miniwdl-aws-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 10:21:46.636555 miniwdl-aws-0.9.0/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1057 2021-07-21 10:10:47.000000 miniwdl-aws-0.9.0/LICENSE
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       35 2021-07-22 09:47:06.000000 miniwdl-aws-0.9.0/MANIFEST.in
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    12378 2023-01-28 10:21:46.636555 miniwdl-aws-0.9.0/PKG-INFO
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    12174 2023-01-28 09:03:21.000000 miniwdl-aws-0.9.0/README.md
--rw-rw-r--   0 mlin      (1000) mlin      (1000)        6 2023-01-28 10:21:45.000000 miniwdl-aws-0.9.0/RELEASE-VERSION
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 10:21:46.636555 miniwdl-aws-0.9.0/miniwdl_aws/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      188 2022-10-03 10:06:47.000000 miniwdl-aws-0.9.0/miniwdl_aws/__init__.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      170 2021-07-21 10:10:47.000000 miniwdl-aws-0.9.0/miniwdl_aws/__main__.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     7771 2022-12-17 05:51:09.000000 miniwdl-aws-0.9.0/miniwdl_aws/_util.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    25971 2023-01-28 09:52:34.000000 miniwdl-aws-0.9.0/miniwdl_aws/batch_job.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    11152 2022-12-18 00:19:12.000000 miniwdl-aws-0.9.0/miniwdl_aws/cli_run_s3upload.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    28239 2022-12-18 00:41:26.000000 miniwdl-aws-0.9.0/miniwdl_aws/cli_submit.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 10:21:46.636555 miniwdl-aws-0.9.0/miniwdl_aws.egg-info/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    12378 2023-01-28 10:21:46.000000 miniwdl-aws-0.9.0/miniwdl_aws.egg-info/PKG-INFO
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      442 2023-01-28 10:21:46.000000 miniwdl-aws-0.9.0/miniwdl_aws.egg-info/SOURCES.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)        1 2023-01-28 10:21:46.000000 miniwdl-aws-0.9.0/miniwdl_aws.egg-info/dependency_links.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      243 2023-01-28 10:21:46.000000 miniwdl-aws-0.9.0/miniwdl_aws.egg-info/entry_points.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       36 2023-01-28 10:21:46.000000 miniwdl-aws-0.9.0/miniwdl_aws.egg-info/requires.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       12 2023-01-28 10:21:46.000000 miniwdl-aws-0.9.0/miniwdl_aws.egg-info/top_level.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       38 2023-01-28 10:21:46.636555 miniwdl-aws-0.9.0/setup.cfg
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      928 2023-01-28 09:28:00.000000 miniwdl-aws-0.9.0/setup.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-01-28 10:21:46.636555 miniwdl-aws-0.9.0/test/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    13945 2022-12-27 11:38:37.000000 miniwdl-aws-0.9.0/test/test.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     3528 2021-07-21 10:16:22.000000 miniwdl-aws-0.9.0/version.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-08 08:00:51.050923 miniwdl-aws-0.9.1/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1057 2021-07-21 10:10:47.000000 miniwdl-aws-0.9.1/LICENSE
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       35 2021-07-22 09:47:06.000000 miniwdl-aws-0.9.1/MANIFEST.in
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    12378 2023-02-08 08:00:51.050923 miniwdl-aws-0.9.1/PKG-INFO
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    12174 2023-01-28 09:03:21.000000 miniwdl-aws-0.9.1/README.md
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)        6 2023-02-08 08:00:50.000000 miniwdl-aws-0.9.1/RELEASE-VERSION
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-08 08:00:51.050923 miniwdl-aws-0.9.1/miniwdl_aws/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      188 2022-10-03 10:06:47.000000 miniwdl-aws-0.9.1/miniwdl_aws/__init__.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      170 2021-07-21 10:10:47.000000 miniwdl-aws-0.9.1/miniwdl_aws/__main__.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     7771 2022-12-17 05:51:09.000000 miniwdl-aws-0.9.1/miniwdl_aws/_util.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    25979 2023-02-05 11:20:29.000000 miniwdl-aws-0.9.1/miniwdl_aws/batch_job.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    11151 2023-02-05 11:25:33.000000 miniwdl-aws-0.9.1/miniwdl_aws/cli_run_s3upload.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    28239 2022-12-18 00:41:26.000000 miniwdl-aws-0.9.1/miniwdl_aws/cli_submit.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-08 08:00:51.050923 miniwdl-aws-0.9.1/miniwdl_aws.egg-info/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    12378 2023-02-08 08:00:50.000000 miniwdl-aws-0.9.1/miniwdl_aws.egg-info/PKG-INFO
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      442 2023-02-08 08:00:51.000000 miniwdl-aws-0.9.1/miniwdl_aws.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)        1 2023-02-08 08:00:50.000000 miniwdl-aws-0.9.1/miniwdl_aws.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      243 2023-02-08 08:00:50.000000 miniwdl-aws-0.9.1/miniwdl_aws.egg-info/entry_points.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       36 2023-02-08 08:00:50.000000 miniwdl-aws-0.9.1/miniwdl_aws.egg-info/requires.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       12 2023-02-08 08:00:50.000000 miniwdl-aws-0.9.1/miniwdl_aws.egg-info/top_level.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       38 2023-02-08 08:00:51.050923 miniwdl-aws-0.9.1/setup.cfg
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      928 2023-01-28 09:28:00.000000 miniwdl-aws-0.9.1/setup.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-02-08 08:00:51.050923 miniwdl-aws-0.9.1/test/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    13945 2022-12-27 11:38:37.000000 miniwdl-aws-0.9.1/test/test.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     3528 2021-07-21 10:16:22.000000 miniwdl-aws-0.9.1/version.py
```

### Comparing `miniwdl-aws-0.9.0/LICENSE` & `miniwdl-aws-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `miniwdl-aws-0.9.0/PKG-INFO` & `miniwdl-aws-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniwdl-aws
-Version: 0.9.0
+Version: 0.9.1
 Summary: miniwdl AWS backend (Batch+EFS)
 Author: Wid L. Hacker
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # miniwdl AWS plugin
```

### Comparing `miniwdl-aws-0.9.0/README.md` & `miniwdl-aws-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `miniwdl-aws-0.9.0/miniwdl_aws/_util.py` & `miniwdl-aws-0.9.1/miniwdl_aws/_util.py`

 * *Files identical despite different names*

### Comparing `miniwdl-aws-0.9.0/miniwdl_aws/batch_job.py` & `miniwdl-aws-0.9.1/miniwdl_aws/batch_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
             resource_requirements += [{"type": "GPU", "value": "1"}]
 
         container_properties = {
             "image": image_tag,
             "command": ["/bin/bash", "-ec", "\n".join(commands)],
             "environment": [
                 {"name": ev_name, "value": ev_value}
-                for ev_name, ev_value in self.runtime_values.get("env", dict())
+                for ev_name, ev_value in self.runtime_values.get("env", dict()).items()
             ],
             "resourceRequirements": resource_requirements,
             "privileged": self.runtime_values.get("privileged", False),
             "mountPoints": [{"containerPath": self._fs_mount, "sourceVolume": "file_io_root"}],
         }
 
         if self.cfg["task_runtime"].get_bool("as_user"):
```

### Comparing `miniwdl-aws-0.9.0/miniwdl_aws/cli_run_s3upload.py` & `miniwdl-aws-0.9.1/miniwdl_aws/cli_run_s3upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,14 @@
                 f"[miniwdl_run_s3upload] deleted {run_dir}",
                 file=sys.stderr,
             )
         return miniwdl.returncode
 
     # recursively rewrite outputs JSON
     def rewrite(v):
-
         if v and isinstance(v, str) and v[0] == "/" and os.path.exists(v):
             # miniwdl writes File/Directory outputs with absolute paths
             return rebase_output_path(v, run_dir, s3_upload_folder)
         if isinstance(v, list):
             return [rewrite(u) for u in v]
         if isinstance(v, dict):
             return dict((k, rewrite(u)) for (k, u) in v.items())
```

### Comparing `miniwdl-aws-0.9.0/miniwdl_aws/cli_submit.py` & `miniwdl-aws-0.9.1/miniwdl_aws/cli_submit.py`

 * *Files identical despite different names*

### Comparing `miniwdl-aws-0.9.0/miniwdl_aws.egg-info/PKG-INFO` & `miniwdl-aws-0.9.1/miniwdl_aws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniwdl-aws
-Version: 0.9.0
+Version: 0.9.1
 Summary: miniwdl AWS backend (Batch+EFS)
 Author: Wid L. Hacker
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # miniwdl AWS plugin
```

### Comparing `miniwdl-aws-0.9.0/setup.py` & `miniwdl-aws-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `miniwdl-aws-0.9.0/test/test.py` & `miniwdl-aws-0.9.1/test/test.py`

 * *Files identical despite different names*

### Comparing `miniwdl-aws-0.9.0/version.py` & `miniwdl-aws-0.9.1/version.py`

 * *Files identical despite different names*

