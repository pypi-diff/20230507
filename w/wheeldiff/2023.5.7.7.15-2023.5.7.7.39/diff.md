# Comparing `tmp/wheeldiff-2023.5.7.7.15.tar.gz` & `tmp/wheeldiff-2023.5.7.7.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheeldiff-2023.5.7.7.15.tar", last modified: Sun May  7 07:15:23 2023, max compression
+gzip compressed data, was "wheeldiff-2023.5.7.7.39.tar", last modified: Sun May  7 07:39:48 2023, max compression
```

## Comparing `wheeldiff-2023.5.7.7.15.tar` & `wheeldiff-2023.5.7.7.39.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:15:23.529129 wheeldiff-2023.5.7.7.15/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    46110 2023-05-07 07:15:23.529129 wheeldiff-2023.5.7.7.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 07:15:23.529129 wheeldiff-2023.5.7.7.15/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:15:23.521129 wheeldiff-2023.5.7.7.15/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:15:23.525129 wheeldiff-2023.5.7.7.15/src/wheeldiff/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:15:23.529129 wheeldiff-2023.5.7.7.15/src/wheeldiff/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff/_impl/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:15:23.525129 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46110 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:15:23.529129 wheeldiff-2023.5.7.7.15/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:39:48.251313 wheeldiff-2023.5.7.7.39/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    46110 2023-05-07 07:39:48.251313 wheeldiff-2023.5.7.7.39/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 07:39:48.251313 wheeldiff-2023.5.7.7.39/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:39:48.243313 wheeldiff-2023.5.7.7.39/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:39:48.247313 wheeldiff-2023.5.7.7.39/src/wheeldiff/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 07:39:47.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:39:48.251313 wheeldiff-2023.5.7.7.39/src/wheeldiff/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff/_impl/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:39:48.251313 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46110 2023-05-07 07:39:48.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 07:39:48.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 07:39:48.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 07:39:48.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:39:48.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 07:39:48.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:39:48.251313 wheeldiff-2023.5.7.7.39/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/tests/test_import.py
```

### Comparing `wheeldiff-2023.5.7.7.15/LICENSE` & `wheeldiff-2023.5.7.7.39/LICENSE`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7.7.15/PKG-INFO` & `wheeldiff-2023.5.7.7.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheeldiff
-Version: 2023.5.7.7.15
+Version: 2023.5.7.7.39
 Summary: Diff two Python wheels
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -699,15 +699,15 @@
 
 <!--TOC-->
 
 ## Overview
 
 `wheeldiff` is a command-line tool to show differences between two Python wheels.
 
-`wheeldiff` exits with an exit code of 1 if any differences were found, or 0 if no
+`wheeldiff` exits with an exit code of 2 if any differences were found, or 0 if no
 differences were found.
 
 Some types of difference can be ignored via the following options:
 
 - `--ignore version`: ignore differences in version number
 - `--ignore record`: ignore differences in dist-info `RECORD` file (checksums of wheel
   content)
@@ -752,15 +752,15 @@
 -rpmdyn-2023.5.7.dist-info/top_level.txt,sha256=juyQtSPbaEJ3AiMzwEI5aX67FyfxqrpJ-mVuZQayvIU,7
 -rpmdyn-2023.5.7.dist-info/RECORD,,
 +rpmdyn-2023.5.7.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
 +rpmdyn-2023.5.7.3.dist-info/METADATA,sha256=PHfp8XarCfrc6-wYaUfF_m5pgZp4CoDKSeFcyEn4Yqs,43845
 +rpmdyn-2023.5.7.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
 +rpmdyn-2023.5.7.3.dist-info/top_level.txt,sha256=juyQtSPbaEJ3AiMzwEI5aX67FyfxqrpJ-mVuZQayvIU,7
 +rpmdyn-2023.5.7.3.dist-info/RECORD,,
-1
+2
 ```
 
 Suppressing version number differences:
 
 ```
 $ wheeldiff rpmdyn-2023.5.7-py3-none-any.whl rpmdyn-2023.5.7.3-py3-none-any.whl --ignore version; echo $?
 --- rpmdyn-2023.5.7-py3-none-any.whl/rpmdyn-$VERSION/rpmdyn-$VERSION.dist-info/RECORD
@@ -777,15 +777,15 @@
  rpmdyn/rpmdyn.pth,sha256=wXLoNTnlvRUqLcf1828EUQvWW7oeVpjvk8nnKz50dvk,24
  rpmdyn-$VERSION.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
 -rpmdyn-$VERSION.dist-info/METADATA,sha256=VMv3OH7xsu_iJc_4aLpS7U8QpuEvMo2z0T860eUBCCM,43843
 +rpmdyn-$VERSION.dist-info/METADATA,sha256=PHfp8XarCfrc6-wYaUfF_m5pgZp4CoDKSeFcyEn4Yqs,43845
  rpmdyn-$VERSION.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
  rpmdyn-$VERSION.dist-info/top_level.txt,sha256=juyQtSPbaEJ3AiMzwEI5aX67FyfxqrpJ-mVuZQayvIU,7
  rpmdyn-$VERSION.dist-info/RECORD,,
-1
+2
 ```
 
 Suppressing version and RECORD differences; in this case, there are no remaining
 differences, so no output is generated and the exit code is 0.
 
 ```
 $ wheeldiff rpmdyn-2023.5.7-py3-none-any.whl rpmdyn-2023.5.7.3-py3-none-any.whl --ignore version,record; echo $?
```

### Comparing `wheeldiff-2023.5.7.7.15/README.md` & `wheeldiff-2023.5.7.7.39/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 <!--TOC-->
 
 ## Overview
 
 `wheeldiff` is a command-line tool to show differences between two Python wheels.
 
-`wheeldiff` exits with an exit code of 1 if any differences were found, or 0 if no
+`wheeldiff` exits with an exit code of 2 if any differences were found, or 0 if no
 differences were found.
 
 Some types of difference can be ignored via the following options:
 
 - `--ignore version`: ignore differences in version number
 - `--ignore record`: ignore differences in dist-info `RECORD` file (checksums of wheel
   content)
@@ -66,15 +66,15 @@
 -rpmdyn-2023.5.7.dist-info/top_level.txt,sha256=juyQtSPbaEJ3AiMzwEI5aX67FyfxqrpJ-mVuZQayvIU,7
 -rpmdyn-2023.5.7.dist-info/RECORD,,
 +rpmdyn-2023.5.7.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
 +rpmdyn-2023.5.7.3.dist-info/METADATA,sha256=PHfp8XarCfrc6-wYaUfF_m5pgZp4CoDKSeFcyEn4Yqs,43845
 +rpmdyn-2023.5.7.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
 +rpmdyn-2023.5.7.3.dist-info/top_level.txt,sha256=juyQtSPbaEJ3AiMzwEI5aX67FyfxqrpJ-mVuZQayvIU,7
 +rpmdyn-2023.5.7.3.dist-info/RECORD,,
-1
+2
 ```
 
 Suppressing version number differences:
 
 ```
 $ wheeldiff rpmdyn-2023.5.7-py3-none-any.whl rpmdyn-2023.5.7.3-py3-none-any.whl --ignore version; echo $?
 --- rpmdyn-2023.5.7-py3-none-any.whl/rpmdyn-$VERSION/rpmdyn-$VERSION.dist-info/RECORD
@@ -91,15 +91,15 @@
  rpmdyn/rpmdyn.pth,sha256=wXLoNTnlvRUqLcf1828EUQvWW7oeVpjvk8nnKz50dvk,24
  rpmdyn-$VERSION.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
 -rpmdyn-$VERSION.dist-info/METADATA,sha256=VMv3OH7xsu_iJc_4aLpS7U8QpuEvMo2z0T860eUBCCM,43843
 +rpmdyn-$VERSION.dist-info/METADATA,sha256=PHfp8XarCfrc6-wYaUfF_m5pgZp4CoDKSeFcyEn4Yqs,43845
  rpmdyn-$VERSION.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
  rpmdyn-$VERSION.dist-info/top_level.txt,sha256=juyQtSPbaEJ3AiMzwEI5aX67FyfxqrpJ-mVuZQayvIU,7
  rpmdyn-$VERSION.dist-info/RECORD,,
-1
+2
 ```
 
 Suppressing version and RECORD differences; in this case, there are no remaining
 differences, so no output is generated and the exit code is 0.
 
 ```
 $ wheeldiff rpmdyn-2023.5.7-py3-none-any.whl rpmdyn-2023.5.7.3-py3-none-any.whl --ignore version,record; echo $?
```

### Comparing `wheeldiff-2023.5.7.7.15/pyproject.toml` & `wheeldiff-2023.5.7.7.39/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7.7.15/src/wheeldiff/_impl/cmd.py` & `wheeldiff-2023.5.7.7.39/src/wheeldiff/_impl/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             LOG.debug("Renaming: %s => %s", entry.path, path)
             shutil.move(entry.path, path)
 
         if entry.is_dir():
             normalize(str(path), version, version_in_content)
         elif is_text(path) and version_in_content:
             content = path.read_text()
-            new_content = version_re.sub(content, "\1$VERSION\2")
+            new_content = version_re.sub(r"\1$VERSION\2", content)
             if content != new_content:
                 LOG.debug("Rewrote version in %s", path)
                 path.write_text(new_content)
 
 
 class UnpackedWheel:
     def __init__(self, filename: str, normalize_version_in_content: bool):
@@ -191,15 +191,15 @@
                     elif record.diff_type == DiffType.RIGHT_ONLY:
                         print(f"Only in {self.wheel2}: {record.path}")
                     elif record.diff_type == DiffType.BINARY_DIFFERS:
                         print(f"Binary file differs: {record.path}")
                     elif record.diff_type == DiffType.TEXT_DIFFERS:
                         self.print_unified_diff(unpacked1, unpacked2, record.path)
 
-        sys.exit(0 if not accum else 1)
+        sys.exit(0 if not accum else 2)
 
 
 def entry_point():
     p = argparse.ArgumentParser(description="Show differences between wheels")
     p.add_argument("wheel1")
     p.add_argument("wheel2")
```

### Comparing `wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/PKG-INFO` & `wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheeldiff
-Version: 2023.5.7.7.15
+Version: 2023.5.7.7.39
 Summary: Diff two Python wheels
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -699,15 +699,15 @@
 
 <!--TOC-->
 
 ## Overview
 
 `wheeldiff` is a command-line tool to show differences between two Python wheels.
 
-`wheeldiff` exits with an exit code of 1 if any differences were found, or 0 if no
+`wheeldiff` exits with an exit code of 2 if any differences were found, or 0 if no
 differences were found.
 
 Some types of difference can be ignored via the following options:
 
 - `--ignore version`: ignore differences in version number
 - `--ignore record`: ignore differences in dist-info `RECORD` file (checksums of wheel
   content)
@@ -752,15 +752,15 @@
 -rpmdyn-2023.5.7.dist-info/top_level.txt,sha256=juyQtSPbaEJ3AiMzwEI5aX67FyfxqrpJ-mVuZQayvIU,7
 -rpmdyn-2023.5.7.dist-info/RECORD,,
 +rpmdyn-2023.5.7.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
 +rpmdyn-2023.5.7.3.dist-info/METADATA,sha256=PHfp8XarCfrc6-wYaUfF_m5pgZp4CoDKSeFcyEn4Yqs,43845
 +rpmdyn-2023.5.7.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
 +rpmdyn-2023.5.7.3.dist-info/top_level.txt,sha256=juyQtSPbaEJ3AiMzwEI5aX67FyfxqrpJ-mVuZQayvIU,7
 +rpmdyn-2023.5.7.3.dist-info/RECORD,,
-1
+2
 ```
 
 Suppressing version number differences:
 
 ```
 $ wheeldiff rpmdyn-2023.5.7-py3-none-any.whl rpmdyn-2023.5.7.3-py3-none-any.whl --ignore version; echo $?
 --- rpmdyn-2023.5.7-py3-none-any.whl/rpmdyn-$VERSION/rpmdyn-$VERSION.dist-info/RECORD
@@ -777,15 +777,15 @@
  rpmdyn/rpmdyn.pth,sha256=wXLoNTnlvRUqLcf1828EUQvWW7oeVpjvk8nnKz50dvk,24
  rpmdyn-$VERSION.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
 -rpmdyn-$VERSION.dist-info/METADATA,sha256=VMv3OH7xsu_iJc_4aLpS7U8QpuEvMo2z0T860eUBCCM,43843
 +rpmdyn-$VERSION.dist-info/METADATA,sha256=PHfp8XarCfrc6-wYaUfF_m5pgZp4CoDKSeFcyEn4Yqs,43845
  rpmdyn-$VERSION.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
  rpmdyn-$VERSION.dist-info/top_level.txt,sha256=juyQtSPbaEJ3AiMzwEI5aX67FyfxqrpJ-mVuZQayvIU,7
  rpmdyn-$VERSION.dist-info/RECORD,,
-1
+2
 ```
 
 Suppressing version and RECORD differences; in this case, there are no remaining
 differences, so no output is generated and the exit code is 0.
 
 ```
 $ wheeldiff rpmdyn-2023.5.7-py3-none-any.whl rpmdyn-2023.5.7.3-py3-none-any.whl --ignore version,record; echo $?
```

