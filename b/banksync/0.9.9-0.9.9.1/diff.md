# Comparing `tmp/banksync-0.9.9.tar.gz` & `tmp/banksync-0.9.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/System/Volumes/Data/Development/Python/banksync_Package/dist/.tmp-dlpqb55b/banksync-0.9.9.tar", last modified: Sun May  7 19:29:58 2023, max compression
+gzip compressed data, was "/System/Volumes/Data/Development/Python/banksync_Package/dist/.tmp-49_1ugx0/banksync-0.9.9.1.tar", last modified: Sun May  7 19:33:03 2023, max compression
```

## Comparing `banksync-0.9.9.tar` & `banksync-0.9.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:29:58.000000 banksync-0.9.9/
--rw-r--r--   0 jason      (501) wheel        (0)     1504 2016-11-03 14:19:14.000000 banksync-0.9.9/LICENSE.txt
--rw-r--r--   0 jason      (501) wheel        (0)    15294 2023-05-07 19:29:58.000000 banksync-0.9.9/PKG-INFO
--rw-r--r--   0 jason      (501) wheel        (0)    14406 2023-05-07 19:28:58.000000 banksync-0.9.9/README.md
-drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync/
--rwxr-xr-x   0 jason      (501) wheel        (0)       30 2016-11-17 20:03:24.000000 banksync-0.9.9/banksync/__init__.py
--rwxr-xr-x   0 jason      (501) wheel        (0)    41943 2023-05-07 19:28:58.000000 banksync-0.9.9/banksync/banksync.py
--rwxr-xr-x   0 jason      (501) wheel        (0)    14890 2023-05-07 19:28:58.000000 banksync-0.9.9/banksync/banksync_common.py
-drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync.egg-info/
--rw-r--r--   0 jason      (501) wheel        (0)    15294 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) wheel        (0)      326 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) wheel        (0)        1 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) wheel        (0)       52 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync.egg-info/requires.txt
--rw-r--r--   0 jason      (501) wheel        (0)        9 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync.egg-info/top_level.txt
-drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:29:58.000000 banksync-0.9.9/bin/
--rwxr-xr-x   0 jason      (501) wheel        (0)      246 2021-02-27 05:41:33.000000 banksync-0.9.9/bin/bank
--rwxr-xr-x   0 jason      (501) wheel        (0)      246 2021-02-27 05:41:33.000000 banksync-0.9.9/bin/banksync
--rw-r--r--   0 jason      (501) wheel        (0)      103 2021-02-27 16:30:49.000000 banksync-0.9.9/pyproject.toml
--rw-r--r--   0 jason      (501) wheel        (0)       79 2023-05-07 19:29:58.000000 banksync-0.9.9/setup.cfg
--rw-r--r--   0 jason      (501) wheel        (0)     1879 2021-02-27 16:51:04.000000 banksync-0.9.9/setup.py
-drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:29:58.000000 banksync-0.9.9/tests/
--rw-r--r--   0 jason      (501) wheel        (0)      546 2023-05-06 14:37:19.000000 banksync-0.9.9/tests/test_setup.py
+drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:33:03.000000 banksync-0.9.9.1/
+-rw-r--r--   0 jason      (501) wheel        (0)     1504 2016-11-03 14:19:14.000000 banksync-0.9.9.1/LICENSE.txt
+-rw-r--r--   0 jason      (501) wheel        (0)    15250 2023-05-07 19:33:03.000000 banksync-0.9.9.1/PKG-INFO
+-rw-r--r--   0 jason      (501) wheel        (0)    14358 2023-05-07 19:32:13.000000 banksync-0.9.9.1/README.md
+drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:33:03.000000 banksync-0.9.9.1/banksync/
+-rwxr-xr-x   0 jason      (501) wheel        (0)       30 2016-11-17 20:03:24.000000 banksync-0.9.9.1/banksync/__init__.py
+-rwxr-xr-x   0 jason      (501) wheel        (0)    41945 2023-05-07 19:32:47.000000 banksync-0.9.9.1/banksync/banksync.py
+-rwxr-xr-x   0 jason      (501) wheel        (0)    14890 2023-05-07 19:28:58.000000 banksync-0.9.9.1/banksync/banksync_common.py
+drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:33:03.000000 banksync-0.9.9.1/banksync.egg-info/
+-rw-r--r--   0 jason      (501) wheel        (0)    15250 2023-05-07 19:33:03.000000 banksync-0.9.9.1/banksync.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) wheel        (0)      326 2023-05-07 19:33:03.000000 banksync-0.9.9.1/banksync.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) wheel        (0)        1 2023-05-07 19:33:03.000000 banksync-0.9.9.1/banksync.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) wheel        (0)       52 2023-05-07 19:33:03.000000 banksync-0.9.9.1/banksync.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) wheel        (0)        9 2023-05-07 19:33:03.000000 banksync-0.9.9.1/banksync.egg-info/top_level.txt
+drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:33:03.000000 banksync-0.9.9.1/bin/
+-rwxr-xr-x   0 jason      (501) wheel        (0)      246 2021-02-27 05:41:33.000000 banksync-0.9.9.1/bin/bank
+-rwxr-xr-x   0 jason      (501) wheel        (0)      246 2021-02-27 05:41:33.000000 banksync-0.9.9.1/bin/banksync
+-rw-r--r--   0 jason      (501) wheel        (0)      103 2021-02-27 16:30:49.000000 banksync-0.9.9.1/pyproject.toml
+-rw-r--r--   0 jason      (501) wheel        (0)       79 2023-05-07 19:33:03.000000 banksync-0.9.9.1/setup.cfg
+-rw-r--r--   0 jason      (501) wheel        (0)     1879 2021-02-27 16:51:04.000000 banksync-0.9.9.1/setup.py
+drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:33:03.000000 banksync-0.9.9.1/tests/
+-rw-r--r--   0 jason      (501) wheel        (0)      546 2023-05-06 14:37:19.000000 banksync-0.9.9.1/tests/test_setup.py
```

### Comparing `banksync-0.9.9/LICENSE.txt` & `banksync-0.9.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `banksync-0.9.9/PKG-INFO` & `banksync-0.9.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: banksync
-Version: 0.9.9
+Version: 0.9.9.1
 Summary: A library for manipulating banks of git repositories
 Home-page: https://github.com/jasonfharris/banksync
-Download-URL: https://github.com/jasonfharris/banksync/tarball/0.9.9
+Download-URL: https://github.com/jasonfharris/banksync/tarball/0.9.9.1
 Author: Jason Harris
 Author-email: jason@jasonfharris.com
 License: MIT
 Keywords: execute,shell,system,git,submodule
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
@@ -126,36 +126,36 @@
 The syncfile specifies which repositories are part of the bank, and what state the repositories should be synchronized to. A typical simple sync file might be the following
 
     more ~/animals/animalsRepoSync/syncfile.json
 
 Which yields:
 
 ```
-<|
-    "repoFish" -> <|
-        "path" -> "repoFish",
-        "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
-        "UnixTimeStamp" -> "1480517200",
-        "date" -> "30 Nov 2016 - 15:46:40",
-        "author" -> "Jason Harris",
-        "revisionNumber" -> "3",
-        "message" -> "committing salmon",
-        "cloneURL" -> "https://github.com/testbank/repoFish.git"
-    |>,
-    "repoBird" -> <|
-        "path" -> "repoBird",
-        "sha" -> "6bf9d646b2aa224b64fb86cbddb4d7ab0f2e37d3",
-        "UnixTimeStamp" -> "1480517200",
-        "date" -> "30 Nov 2016 - 15:46:40",
-        "author" -> "Jason Harris",
-        "revisionNumber" -> "3",
-        "message" -> "committing eagle",
-        "cloneURL" -> "https://github.com/testbank/repoBird.git"
-    |>
-|>
+{
+    "repoFish" : {
+        "path" : "repoFish",
+        "sha" : "a27368bec17373938b1dcf73638945b89b60a9d0",
+        "UnixTimeStamp" : "1480517200",
+        "date" : "30 Nov 2016 - 15:46:40",
+        "author" : "Jason Harris",
+        "revisionNumber" : "3",
+        "message" : "committing salmon",
+        "cloneURL" : "https://github.com/testbank/repoFish.git"
+    },
+    "repoBird" : {
+        "path" : "repoBird",
+        "sha" : "6bf9d646b2aa224b64fb86cbddb4d7ab0f2e37d3",
+        "UnixTimeStamp" : "1480517200",
+        "date" : "30 Nov 2016 - 15:46:40",
+        "author" : "Jason Harris",
+        "revisionNumber" : "3",
+        "message" : "committing eagle",
+        "cloneURL" : "https://github.com/testbank/repoBird.git"
+    }
+}
 ```
 
 The syncfile should lie inside a git repo (the syncrepo). Whenever we want to record a configuration of the repos we simply alter the syncfile by transcribing the current state of the repos into the syncfile using `bank record_repos` with the appropriate options. We then use `git commit` to record this new state / configuration in the syncrepo.
 
 So let us add some content to repoBird in our example and then commit this change.
 
     cd  ~/animals/repoBird
@@ -166,36 +166,36 @@
 
     cd ~/animals/animalsRepoSync/
     bank record_repos
 
 The contents of our syncfile will now be something like:
 
 ```
-<|
-    "repoFish" -> <|
-        "path" -> "repoFish",
-        "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
-        "UnixTimeStamp" -> "1480517200",
-        "date" -> "30 Nov 2016 - 15:46:40",
-        "author" -> "Jason Harris",
-        "revisionNumber" -> "3",
-        "message" -> "committing salmon",
-        "cloneURL" -> "https://github.com/testbank/repoFish.git"
-    |>,
-    "repoBird" -> <|
-        "path" -> "repoBird",
-        "sha" -> "c8fb05947c5161e484104d99f427ec082fb4e85b",
-        "UnixTimeStamp" -> "1480519159",
-        "date" -> "30 Nov 2016 - 16:19:19",
-        "author" -> "Jason Harris",
-        "revisionNumber" -> "4",
-        "message" -> "committing toucan",
-        "cloneURL" -> "https://github.com/testbank/repoBird.git"
-    |>
-|>
+{
+    "repoFish" : {
+        "path" : "repoFish",
+        "sha" : "a27368bec17373938b1dcf73638945b89b60a9d0",
+        "UnixTimeStamp" : "1480517200",
+        "date" : "30 Nov 2016 - 15:46:40",
+        "author" : "Jason Harris",
+        "revisionNumber" : "3",
+        "message" : "committing salmon",
+        "cloneURL" : "https://github.com/testbank/repoFish.git"
+    },
+    "repoBird" : {
+        "path" : "repoBird",
+        "sha" : "c8fb05947c5161e484104d99f427ec082fb4e85b",
+        "UnixTimeStamp" : "1480519159",
+        "date" : "30 Nov 2016 - 16:19:19",
+        "author" : "Jason Harris",
+        "revisionNumber" : "4",
+        "message" : "committing toucan",
+        "cloneURL" : "https://github.com/testbank/repoBird.git"
+    }
+}
 ```
 
 (Note the sha, timestamps, and other data about the state of the repo `repoBird` has changed.)
 
 So we could now record this new overall state of the repos in the bank via simply committing the file syncfile in the syncrepo.
 
     git commit -am "recording the latest state of the repos in animals."
```

### Comparing `banksync-0.9.9/README.md` & `banksync-0.9.9.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -103,36 +103,36 @@
 The syncfile specifies which repositories are part of the bank, and what state the repositories should be synchronized to. A typical simple sync file might be the following
 
     more ~/animals/animalsRepoSync/syncfile.json
 
 Which yields:
 
 ```
-<|
-    "repoFish" -> <|
-        "path" -> "repoFish",
-        "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
-        "UnixTimeStamp" -> "1480517200",
-        "date" -> "30 Nov 2016 - 15:46:40",
-        "author" -> "Jason Harris",
-        "revisionNumber" -> "3",
-        "message" -> "committing salmon",
-        "cloneURL" -> "https://github.com/testbank/repoFish.git"
-    |>,
-    "repoBird" -> <|
-        "path" -> "repoBird",
-        "sha" -> "6bf9d646b2aa224b64fb86cbddb4d7ab0f2e37d3",
-        "UnixTimeStamp" -> "1480517200",
-        "date" -> "30 Nov 2016 - 15:46:40",
-        "author" -> "Jason Harris",
-        "revisionNumber" -> "3",
-        "message" -> "committing eagle",
-        "cloneURL" -> "https://github.com/testbank/repoBird.git"
-    |>
-|>
+{
+    "repoFish" : {
+        "path" : "repoFish",
+        "sha" : "a27368bec17373938b1dcf73638945b89b60a9d0",
+        "UnixTimeStamp" : "1480517200",
+        "date" : "30 Nov 2016 - 15:46:40",
+        "author" : "Jason Harris",
+        "revisionNumber" : "3",
+        "message" : "committing salmon",
+        "cloneURL" : "https://github.com/testbank/repoFish.git"
+    },
+    "repoBird" : {
+        "path" : "repoBird",
+        "sha" : "6bf9d646b2aa224b64fb86cbddb4d7ab0f2e37d3",
+        "UnixTimeStamp" : "1480517200",
+        "date" : "30 Nov 2016 - 15:46:40",
+        "author" : "Jason Harris",
+        "revisionNumber" : "3",
+        "message" : "committing eagle",
+        "cloneURL" : "https://github.com/testbank/repoBird.git"
+    }
+}
 ```
 
 The syncfile should lie inside a git repo (the syncrepo). Whenever we want to record a configuration of the repos we simply alter the syncfile by transcribing the current state of the repos into the syncfile using `bank record_repos` with the appropriate options. We then use `git commit` to record this new state / configuration in the syncrepo.
 
 So let us add some content to repoBird in our example and then commit this change.
 
     cd  ~/animals/repoBird
@@ -143,36 +143,36 @@
 
     cd ~/animals/animalsRepoSync/
     bank record_repos
 
 The contents of our syncfile will now be something like:
 
 ```
-<|
-    "repoFish" -> <|
-        "path" -> "repoFish",
-        "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
-        "UnixTimeStamp" -> "1480517200",
-        "date" -> "30 Nov 2016 - 15:46:40",
-        "author" -> "Jason Harris",
-        "revisionNumber" -> "3",
-        "message" -> "committing salmon",
-        "cloneURL" -> "https://github.com/testbank/repoFish.git"
-    |>,
-    "repoBird" -> <|
-        "path" -> "repoBird",
-        "sha" -> "c8fb05947c5161e484104d99f427ec082fb4e85b",
-        "UnixTimeStamp" -> "1480519159",
-        "date" -> "30 Nov 2016 - 16:19:19",
-        "author" -> "Jason Harris",
-        "revisionNumber" -> "4",
-        "message" -> "committing toucan",
-        "cloneURL" -> "https://github.com/testbank/repoBird.git"
-    |>
-|>
+{
+    "repoFish" : {
+        "path" : "repoFish",
+        "sha" : "a27368bec17373938b1dcf73638945b89b60a9d0",
+        "UnixTimeStamp" : "1480517200",
+        "date" : "30 Nov 2016 - 15:46:40",
+        "author" : "Jason Harris",
+        "revisionNumber" : "3",
+        "message" : "committing salmon",
+        "cloneURL" : "https://github.com/testbank/repoFish.git"
+    },
+    "repoBird" : {
+        "path" : "repoBird",
+        "sha" : "c8fb05947c5161e484104d99f427ec082fb4e85b",
+        "UnixTimeStamp" : "1480519159",
+        "date" : "30 Nov 2016 - 16:19:19",
+        "author" : "Jason Harris",
+        "revisionNumber" : "4",
+        "message" : "committing toucan",
+        "cloneURL" : "https://github.com/testbank/repoBird.git"
+    }
+}
 ```
 
 (Note the sha, timestamps, and other data about the state of the repo `repoBird` has changed.)
 
 So we could now record this new overall state of the repos in the bank via simply committing the file syncfile in the syncrepo.
 
     git commit -am "recording the latest state of the repos in animals."
```

### Comparing `banksync-0.9.9/banksync/banksync.py` & `banksync-0.9.9.1/banksync/banksync.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import argparse
 import argcomplete
 import json
 from collections import OrderedDict
 from sysexecute import *
 from .banksync_common import *
 
-__version__ = "0.9.9"
+__version__ = "0.9.9.1"
 
 # --------------------------------------------------------------------------------------------------------------------------
 # Defines
 # --------------------------------------------------------------------------------------------------------------------------
 
 tryOrder = ["sha", "UnixTimeStamp"]
 defaultSyncPointBranchName = "syncPoint"
```

### Comparing `banksync-0.9.9/banksync/banksync_common.py` & `banksync-0.9.9.1/banksync/banksync_common.py`

 * *Files identical despite different names*

### Comparing `banksync-0.9.9/banksync.egg-info/PKG-INFO` & `banksync-0.9.9.1/banksync.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: banksync
-Version: 0.9.9
+Version: 0.9.9.1
 Summary: A library for manipulating banks of git repositories
 Home-page: https://github.com/jasonfharris/banksync
-Download-URL: https://github.com/jasonfharris/banksync/tarball/0.9.9
+Download-URL: https://github.com/jasonfharris/banksync/tarball/0.9.9.1
 Author: Jason Harris
 Author-email: jason@jasonfharris.com
 License: MIT
 Keywords: execute,shell,system,git,submodule
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
@@ -126,36 +126,36 @@
 The syncfile specifies which repositories are part of the bank, and what state the repositories should be synchronized to. A typical simple sync file might be the following
 
     more ~/animals/animalsRepoSync/syncfile.json
 
 Which yields:
 
 ```
-<|
-    "repoFish" -> <|
-        "path" -> "repoFish",
-        "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
-        "UnixTimeStamp" -> "1480517200",
-        "date" -> "30 Nov 2016 - 15:46:40",
-        "author" -> "Jason Harris",
-        "revisionNumber" -> "3",
-        "message" -> "committing salmon",
-        "cloneURL" -> "https://github.com/testbank/repoFish.git"
-    |>,
-    "repoBird" -> <|
-        "path" -> "repoBird",
-        "sha" -> "6bf9d646b2aa224b64fb86cbddb4d7ab0f2e37d3",
-        "UnixTimeStamp" -> "1480517200",
-        "date" -> "30 Nov 2016 - 15:46:40",
-        "author" -> "Jason Harris",
-        "revisionNumber" -> "3",
-        "message" -> "committing eagle",
-        "cloneURL" -> "https://github.com/testbank/repoBird.git"
-    |>
-|>
+{
+    "repoFish" : {
+        "path" : "repoFish",
+        "sha" : "a27368bec17373938b1dcf73638945b89b60a9d0",
+        "UnixTimeStamp" : "1480517200",
+        "date" : "30 Nov 2016 - 15:46:40",
+        "author" : "Jason Harris",
+        "revisionNumber" : "3",
+        "message" : "committing salmon",
+        "cloneURL" : "https://github.com/testbank/repoFish.git"
+    },
+    "repoBird" : {
+        "path" : "repoBird",
+        "sha" : "6bf9d646b2aa224b64fb86cbddb4d7ab0f2e37d3",
+        "UnixTimeStamp" : "1480517200",
+        "date" : "30 Nov 2016 - 15:46:40",
+        "author" : "Jason Harris",
+        "revisionNumber" : "3",
+        "message" : "committing eagle",
+        "cloneURL" : "https://github.com/testbank/repoBird.git"
+    }
+}
 ```
 
 The syncfile should lie inside a git repo (the syncrepo). Whenever we want to record a configuration of the repos we simply alter the syncfile by transcribing the current state of the repos into the syncfile using `bank record_repos` with the appropriate options. We then use `git commit` to record this new state / configuration in the syncrepo.
 
 So let us add some content to repoBird in our example and then commit this change.
 
     cd  ~/animals/repoBird
@@ -166,36 +166,36 @@
 
     cd ~/animals/animalsRepoSync/
     bank record_repos
 
 The contents of our syncfile will now be something like:
 
 ```
-<|
-    "repoFish" -> <|
-        "path" -> "repoFish",
-        "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
-        "UnixTimeStamp" -> "1480517200",
-        "date" -> "30 Nov 2016 - 15:46:40",
-        "author" -> "Jason Harris",
-        "revisionNumber" -> "3",
-        "message" -> "committing salmon",
-        "cloneURL" -> "https://github.com/testbank/repoFish.git"
-    |>,
-    "repoBird" -> <|
-        "path" -> "repoBird",
-        "sha" -> "c8fb05947c5161e484104d99f427ec082fb4e85b",
-        "UnixTimeStamp" -> "1480519159",
-        "date" -> "30 Nov 2016 - 16:19:19",
-        "author" -> "Jason Harris",
-        "revisionNumber" -> "4",
-        "message" -> "committing toucan",
-        "cloneURL" -> "https://github.com/testbank/repoBird.git"
-    |>
-|>
+{
+    "repoFish" : {
+        "path" : "repoFish",
+        "sha" : "a27368bec17373938b1dcf73638945b89b60a9d0",
+        "UnixTimeStamp" : "1480517200",
+        "date" : "30 Nov 2016 - 15:46:40",
+        "author" : "Jason Harris",
+        "revisionNumber" : "3",
+        "message" : "committing salmon",
+        "cloneURL" : "https://github.com/testbank/repoFish.git"
+    },
+    "repoBird" : {
+        "path" : "repoBird",
+        "sha" : "c8fb05947c5161e484104d99f427ec082fb4e85b",
+        "UnixTimeStamp" : "1480519159",
+        "date" : "30 Nov 2016 - 16:19:19",
+        "author" : "Jason Harris",
+        "revisionNumber" : "4",
+        "message" : "committing toucan",
+        "cloneURL" : "https://github.com/testbank/repoBird.git"
+    }
+}
 ```
 
 (Note the sha, timestamps, and other data about the state of the repo `repoBird` has changed.)
 
 So we could now record this new overall state of the repos in the bank via simply committing the file syncfile in the syncrepo.
 
     git commit -am "recording the latest state of the repos in animals."
```

### Comparing `banksync-0.9.9/setup.py` & `banksync-0.9.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `banksync-0.9.9/tests/test_setup.py` & `banksync-0.9.9.1/tests/test_setup.py`

 * *Files identical despite different names*

