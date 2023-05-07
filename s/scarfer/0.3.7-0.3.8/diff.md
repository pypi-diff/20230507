# Comparing `tmp/scarfer-0.3.7.tar.gz` & `tmp/scarfer-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scarfer-0.3.7.tar", last modified: Mon May  1 15:44:58 2023, max compression
+gzip compressed data, was "scarfer-0.3.8.tar", last modified: Sun May  7 14:35:05 2023, max compression
```

## Comparing `scarfer-0.3.7.tar` & `scarfer-0.3.8.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 hesa      (1001) hesa      (1001)        0 2023-05-01 15:44:58.022554 scarfer-0.3.7/
--rw-rw-r--   0 hesa      (1001) hesa      (1001)      268 2022-12-20 17:51:14.000000 scarfer-0.3.7/DESCRIPTION.md
-drwxrwxr-x   0 hesa      (1001) hesa      (1001)        0 2023-05-01 15:44:58.022554 scarfer-0.3.7/LICENSES/
--rw-rw-r--   0 hesa      (1001) hesa      (1001)    34670 2022-12-20 17:51:14.000000 scarfer-0.3.7/LICENSES/GPL-3.0-or-later.txt
--rw-rw-r--   0 hesa      (1001) hesa      (1001)      111 2023-05-01 15:01:55.000000 scarfer-0.3.7/MANIFEST.in
--rw-rw-r--   0 hesa      (1001) hesa      (1001)     1106 2023-05-01 15:44:58.022554 scarfer-0.3.7/PKG-INFO
--rw-rw-r--   0 hesa      (1001) hesa      (1001)     3007 2023-05-01 15:01:55.000000 scarfer-0.3.7/README.md
--rw-rw-r--   0 hesa      (1001) hesa      (1001)        1 2022-12-20 17:51:14.000000 scarfer-0.3.7/requirements-dev.txt
--rw-rw-r--   0 hesa      (1001) hesa      (1001)       37 2023-05-01 15:01:55.000000 scarfer-0.3.7/requirements.txt
-drwxrwxr-x   0 hesa      (1001) hesa      (1001)        0 2023-05-01 15:44:58.022554 scarfer-0.3.7/scarfer/
--rwxrwxr-x   0 hesa      (1001) hesa      (1001)    13211 2023-05-01 15:42:08.000000 scarfer-0.3.7/scarfer/__main__.py
--rw-rw-r--   0 hesa      (1001) hesa      (1001)     6761 2023-05-01 15:01:55.000000 scarfer-0.3.7/scarfer/analyzer.py
--rw-rw-r--   0 hesa      (1001) hesa      (1001)       51 2023-05-01 15:42:18.000000 scarfer-0.3.7/scarfer/config.py
--rw-rw-r--   0 hesa      (1001) hesa      (1001)      612 2023-05-01 15:01:55.000000 scarfer-0.3.7/scarfer/filter_utils.py
-drwxrwxr-x   0 hesa      (1001) hesa      (1001)        0 2023-05-01 15:44:58.022554 scarfer-0.3.7/scarfer/format/
--rw-rw-r--   0 hesa      (1001) hesa      (1001)        0 2022-12-20 17:51:14.000000 scarfer-0.3.7/scarfer/format/__init__.py
--rw-rw-r--   0 hesa      (1001) hesa      (1001)      672 2023-05-01 15:01:55.000000 scarfer-0.3.7/scarfer/format/factory.py
--rw-rw-r--   0 hesa      (1001) hesa      (1001)     1122 2023-05-01 15:01:55.000000 scarfer-0.3.7/scarfer/format/format_json.py
--rw-rw-r--   0 hesa      (1001) hesa      (1001)      968 2023-05-01 15:01:55.000000 scarfer-0.3.7/scarfer/format/format_markdown.py
--rw-rw-r--   0 hesa      (1001) hesa      (1001)     2572 2023-05-01 15:01:55.000000 scarfer-0.3.7/scarfer/format/format_text.py
--rw-rw-r--   0 hesa      (1001) hesa      (1001)      190 2022-12-20 17:51:14.000000 scarfer-0.3.7/scarfer/format/format_yaml.py
--rw-rw-r--   0 hesa      (1001) hesa      (1001)     1141 2023-05-01 15:01:55.000000 scarfer-0.3.7/scarfer/format/interface.py
--rw-rw-r--   0 hesa      (1001) hesa      (1001)     4438 2023-05-01 15:01:55.000000 scarfer-0.3.7/scarfer/scan_interface.py
-drwxrwxr-x   0 hesa      (1001) hesa      (1001)        0 2023-05-01 15:44:58.022554 scarfer-0.3.7/scarfer/var/
--rw-rw-r--   0 hesa      (1001) hesa      (1001)     3113 2023-05-01 15:01:55.000000 scarfer-0.3.7/scarfer/var/normalized-scan.json
-drwxrwxr-x   0 hesa      (1001) hesa      (1001)        0 2023-05-01 15:44:58.022554 scarfer-0.3.7/scarfer.egg-info/
--rw-rw-r--   0 hesa      (1001) hesa      (1001)     1106 2023-05-01 15:44:58.000000 scarfer-0.3.7/scarfer.egg-info/PKG-INFO
--rw-rw-r--   0 hesa      (1001) hesa      (1001)      647 2023-05-01 15:44:58.000000 scarfer-0.3.7/scarfer.egg-info/SOURCES.txt
--rw-rw-r--   0 hesa      (1001) hesa      (1001)        1 2023-05-01 15:44:58.000000 scarfer-0.3.7/scarfer.egg-info/dependency_links.txt
--rw-rw-r--   0 hesa      (1001) hesa      (1001)       50 2023-05-01 15:44:58.000000 scarfer-0.3.7/scarfer.egg-info/entry_points.txt
--rw-rw-r--   0 hesa      (1001) hesa      (1001)       44 2023-05-01 15:44:58.000000 scarfer-0.3.7/scarfer.egg-info/requires.txt
--rw-rw-r--   0 hesa      (1001) hesa      (1001)       23 2023-05-01 15:44:58.000000 scarfer-0.3.7/scarfer.egg-info/top_level.txt
--rw-rw-r--   0 hesa      (1001) hesa      (1001)       38 2023-05-01 15:44:58.022554 scarfer-0.3.7/setup.cfg
--rw-rw-r--   0 hesa      (1001) hesa      (1001)     1937 2023-05-01 15:01:55.000000 scarfer-0.3.7/setup.py
+drwxr-xr-x   0 hesa      (1000) hesa      (1000)        0 2023-05-07 14:35:05.296931 scarfer-0.3.8/
+-rw-r--r--   0 hesa      (1000) hesa      (1000)      268 2023-04-26 16:41:20.000000 scarfer-0.3.8/DESCRIPTION.md
+drwxr-xr-x   0 hesa      (1000) hesa      (1000)        0 2023-05-07 14:35:05.292931 scarfer-0.3.8/LICENSES/
+-rw-r--r--   0 hesa      (1000) hesa      (1000)    34670 2023-04-26 16:41:20.000000 scarfer-0.3.8/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 hesa      (1000) hesa      (1000)      111 2023-04-26 16:41:20.000000 scarfer-0.3.8/MANIFEST.in
+-rw-r--r--   0 hesa      (1000) hesa      (1000)     1126 2023-05-07 14:35:05.296931 scarfer-0.3.8/PKG-INFO
+-rw-r--r--   0 hesa      (1000) hesa      (1000)     3007 2023-05-01 14:57:15.000000 scarfer-0.3.8/README.md
+-rw-r--r--   0 hesa      (1000) hesa      (1000)        1 2023-04-26 16:41:20.000000 scarfer-0.3.8/requirements-dev.txt
+-rw-r--r--   0 hesa      (1000) hesa      (1000)       37 2023-04-26 16:41:20.000000 scarfer-0.3.8/requirements.txt
+drwxr-xr-x   0 hesa      (1000) hesa      (1000)        0 2023-05-07 14:35:05.292931 scarfer-0.3.8/scarfer/
+-rwxr-xr-x   0 hesa      (1000) hesa      (1000)    13731 2023-05-07 14:34:56.000000 scarfer-0.3.8/scarfer/__main__.py
+-rw-r--r--   0 hesa      (1000) hesa      (1000)     6761 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/analyzer.py
+-rw-r--r--   0 hesa      (1000) hesa      (1000)      237 2023-05-07 14:34:56.000000 scarfer-0.3.8/scarfer/config.py
+-rw-r--r--   0 hesa      (1000) hesa      (1000)      612 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/filter_utils.py
+drwxr-xr-x   0 hesa      (1000) hesa      (1000)        0 2023-05-07 14:35:05.292931 scarfer-0.3.8/scarfer/format/
+-rw-r--r--   0 hesa      (1000) hesa      (1000)        0 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/__init__.py
+-rw-r--r--   0 hesa      (1000) hesa      (1000)      672 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/factory.py
+-rw-r--r--   0 hesa      (1000) hesa      (1000)     1122 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/format_json.py
+-rw-r--r--   0 hesa      (1000) hesa      (1000)      968 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/format_markdown.py
+-rw-r--r--   0 hesa      (1000) hesa      (1000)     2572 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/format_text.py
+-rw-r--r--   0 hesa      (1000) hesa      (1000)      190 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/format_yaml.py
+-rw-r--r--   0 hesa      (1000) hesa      (1000)     1141 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/format/interface.py
+-rw-r--r--   0 hesa      (1000) hesa      (1000)     4438 2023-05-01 14:54:06.000000 scarfer-0.3.8/scarfer/scan_interface.py
+drwxr-xr-x   0 hesa      (1000) hesa      (1000)        0 2023-05-07 14:35:05.296931 scarfer-0.3.8/scarfer/var/
+-rw-r--r--   0 hesa      (1000) hesa      (1000)     2927 2023-05-07 14:34:56.000000 scarfer-0.3.8/scarfer/var/default-exclude-files.txt
+-rw-r--r--   0 hesa      (1000) hesa      (1000)     3113 2023-04-26 16:41:20.000000 scarfer-0.3.8/scarfer/var/normalized-scan.json
+drwxr-xr-x   0 hesa      (1000) hesa      (1000)        0 2023-05-07 14:35:05.292931 scarfer-0.3.8/scarfer.egg-info/
+-rw-r--r--   0 hesa      (1000) hesa      (1000)     1126 2023-05-07 14:35:05.000000 scarfer-0.3.8/scarfer.egg-info/PKG-INFO
+-rw-r--r--   0 hesa      (1000) hesa      (1000)      685 2023-05-07 14:35:05.000000 scarfer-0.3.8/scarfer.egg-info/SOURCES.txt
+-rw-r--r--   0 hesa      (1000) hesa      (1000)        1 2023-05-07 14:35:05.000000 scarfer-0.3.8/scarfer.egg-info/dependency_links.txt
+-rw-r--r--   0 hesa      (1000) hesa      (1000)       51 2023-05-07 14:35:05.000000 scarfer-0.3.8/scarfer.egg-info/entry_points.txt
+-rw-r--r--   0 hesa      (1000) hesa      (1000)       44 2023-05-07 14:35:05.000000 scarfer-0.3.8/scarfer.egg-info/requires.txt
+-rw-r--r--   0 hesa      (1000) hesa      (1000)       23 2023-05-07 14:35:05.000000 scarfer-0.3.8/scarfer.egg-info/top_level.txt
+-rw-r--r--   0 hesa      (1000) hesa      (1000)       38 2023-05-07 14:35:05.296931 scarfer-0.3.8/setup.cfg
+-rw-r--r--   0 hesa      (1000) hesa      (1000)     1937 2023-04-26 16:41:20.000000 scarfer-0.3.8/setup.py
```

### Comparing `scarfer-0.3.7/LICENSES/GPL-3.0-or-later.txt` & `scarfer-0.3.8/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.7/PKG-INFO` & `scarfer-0.3.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: scarfer
-Version: 0.3.7
+Version: 0.3.8
+Summary: UNKNOWN
 Home-page: https://github.com/hesa/scarfer
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
+License: UNKNOWN
+Description: Scarfer outputs compliance related information from a scan report.
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
@@ -18,10 +22,7 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSES/GPL-3.0-or-later.txt
-
-Scarfer outputs compliance related information from a scan report.
```

### Comparing `scarfer-0.3.7/README.md` & `scarfer-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.7/scarfer/__main__.py` & `scarfer-0.3.8/scarfer/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 from scarfer.scan_interface import ScanReportReader
 from scarfer.scan_interface import ScanReportException
 from scarfer.analyzer import Analyzer
 from scarfer.format.interface import Settings
 from scarfer.filter_utils import create_filters
 from scarfer.config import scarfer_version
 from scarfer.config import scarfer_name
+from scarfer.config import DEFAULT_FILE_EXCLUDE_FILE
 
 SCRIPT_DIR = os.path.dirname(os.path.realpath(__file__))
 
 PROGRAM_NAME = scarfer_name
+PROGRAM_VERSION = scarfer_version
 PROGRAM_DESCRIPTION = "Source code scan report file reporter reads scan reports and outputs selected information about filtered files"
 PROGRAM_URL = "https://github.com/hesa/scarfer"
 PROGRAM_EXAMPLES = "   Coming soon."
 BUG_URL = "https://github.com/hesa/scarfer/issues"
 PROGRAM_COPYRIGHT = "(c) 2021 Henrik Sandklef<hesa@sandklef.com>"
 PROGRAM_LICENSE = "GPL-3.0-or-later"
 PROGRAM_AUTHOR = "Henrik Sandklef"
@@ -38,15 +40,15 @@
 OUTPUT_FORMAT_YAML = "text"
 OUTPUT_FORMATS = [ OUTPUT_FORMAT_JSON, OUTPUT_FORMAT_TEXT, OUTPUT_FORMAT_YAML ]
 
 DATE_FMT = '%Y-%m-%d'
 
 def parse():
 
-    description = "NAME\n  " + PROGRAM_NAME + "\n\n"
+    description = f'NAME\n  {PROGRAM_NAME} ({PROGRAM_VERSION})\n\n'
     description = description + "DESCRIPTION\n  " + PROGRAM_DESCRIPTION + "\n\n"
     
     epilog = ""
     epilog = epilog + "EXAMPLES\n\n" + PROGRAM_EXAMPLES + "\n\n"
     epilog = epilog + "SUPPORTED SCAN REPORT FORMATS\n" + PROGRAM_SUPPORTED_FORMATS + "\n\n"
     epilog = epilog + "AUTHOR\n  " + PROGRAM_AUTHOR + "\n\n"
     epilog = epilog + "REPORTING BUGS\n  File a ticket at " + PROGRAM_URL + "\n\n"
@@ -137,14 +139,18 @@
     parser.add_argument('-eff', '--exclude-file-file',
                             type=str,
                             action='append',
                             nargs="+",
                             help='filter out on file containing file filters',
                             default=[])
     
+    parser.add_argument('-dde', '--disable-default-excludes',
+                        action='store_true',
+                        help=f'Disable exclusion of files as specified in {DEFAULT_FILE_EXCLUDE_FILE}')
+
     parser.add_argument('-cml', '--curate-missing-license',
                         type=str,
                         dest='curate_missing_license',
                         action='append',
                         help='curate missing license for a file with',
                         default=[])
     
@@ -215,14 +221,16 @@
     for l in lists:
         for elem in l:
             new_list.append(elem)
     return new_list
 
 def _output_config(args):
     config = {
+        'tool_name': scarfer_name,
+        'tool_version': scarfer_version,
 #        "copyrights": args.copyrights,
 #        "cumulative": args.cumulative,
         "curate_missing_license": args.curate_missing_license,
         "curate_file_license": args.curate_file_license,
         "exclude_file": args.exclude_file,
         "exclude_file_file": args.exclude_file_file,
         "exclude_license": args.exclude_license,
@@ -297,15 +305,19 @@
     include_license = flatten_lists(args['include_license'])
     exclude_license = flatten_lists(args['exclude_license'])
     #exclude_file = flatten_lists(args['exclude_file)
     
     # Create filters
     include_files = _merge_file_filters(args['include_file'], args['include_file_file'])
     filters = create_filters(include_license, include_files)
-    
+
+    if args['disable_default_excludes']:
+        pass
+    else:
+        args['exclude_file_file'].append([DEFAULT_FILE_EXCLUDE_FILE])
     exclude_files = _merge_file_filters(args['exclude_file'], args['exclude_file_file'])
     exclude_filters = create_filters(exclude_license, exclude_files)
     
 #    print(f"include_files:   {include_files}")
 #    print(f"include_filters: {filters}")
 #    print(f"exclude_files:   {exclude_files}")
 #    print(f"exclude_filters: {exclude_filters}")
```

### Comparing `scarfer-0.3.7/scarfer/analyzer.py` & `scarfer-0.3.8/scarfer/analyzer.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.7/scarfer/filter_utils.py` & `scarfer-0.3.8/scarfer/filter_utils.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.7/scarfer/format/factory.py` & `scarfer-0.3.8/scarfer/format/factory.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.7/scarfer/format/format_json.py` & `scarfer-0.3.8/scarfer/format/format_json.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.7/scarfer/format/format_markdown.py` & `scarfer-0.3.8/scarfer/format/format_markdown.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.7/scarfer/format/format_text.py` & `scarfer-0.3.8/scarfer/format/format_text.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.7/scarfer/format/interface.py` & `scarfer-0.3.8/scarfer/format/interface.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.7/scarfer/scan_interface.py` & `scarfer-0.3.8/scarfer/scan_interface.py`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.7/scarfer/var/normalized-scan.json` & `scarfer-0.3.8/scarfer/var/normalized-scan.json`

 * *Files identical despite different names*

### Comparing `scarfer-0.3.7/scarfer.egg-info/PKG-INFO` & `scarfer-0.3.8/scarfer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: scarfer
-Version: 0.3.7
+Version: 0.3.8
+Summary: UNKNOWN
 Home-page: https://github.com/hesa/scarfer
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
+License: UNKNOWN
+Description: Scarfer outputs compliance related information from a scan report.
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
@@ -18,10 +22,7 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSES/GPL-3.0-or-later.txt
-
-Scarfer outputs compliance related information from a scan report.
```

### Comparing `scarfer-0.3.7/setup.py` & `scarfer-0.3.8/setup.py`

 * *Files identical despite different names*

