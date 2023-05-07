# Comparing `tmp/banksync-0.9.4.tar.gz` & `tmp/banksync-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/banksync-0.9.4.tar", last modified: Wed May 29 04:23:47 2019, max compression
+gzip compressed data, was "/System/Volumes/Data/Development/Python/banksync_Package/dist/.tmp-dlpqb55b/banksync-0.9.9.tar", last modified: Sun May  7 19:29:58 2023, max compression
```

## Comparing `banksync-0.9.4.tar` & `banksync-0.9.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 jason      (501) wheel        (0)        0 2019-05-29 04:23:47.000000 banksync-0.9.4/
--rw-r--r--   0 jason      (501) wheel        (0)     1504 2016-11-03 14:19:14.000000 banksync-0.9.4/LICENSE.txt
--rw-r--r--   0 jason      (501) wheel        (0)       31 2016-11-23 07:06:41.000000 banksync-0.9.4/MANIFEST.in
--rw-r--r--   0 jason      (501) wheel        (0)    17038 2019-05-29 04:23:47.000000 banksync-0.9.4/PKG-INFO
--rw-r--r--   0 jason      (501) wheel        (0)    13761 2016-12-26 17:21:24.000000 banksync-0.9.4/README.md
-drwxr-xr-x   0 jason      (501) wheel        (0)        0 2019-05-29 04:23:47.000000 banksync-0.9.4/banksync/
--rwxr-xr-x   0 jason      (501) wheel        (0)       30 2016-11-17 20:03:24.000000 banksync-0.9.4/banksync/__init__.py
--rwxr-xr-x   0 jason      (501) wheel        (0)    36540 2019-05-29 04:22:11.000000 banksync-0.9.4/banksync/banksync.py
--rwxr-xr-x   0 jason      (501) wheel        (0)    11288 2017-01-18 03:51:01.000000 banksync-0.9.4/banksync/banksync_common.py
-drwxr-xr-x   0 jason      (501) wheel        (0)        0 2019-05-29 04:23:47.000000 banksync-0.9.4/banksync.egg-info/
--rw-r--r--   0 jason      (501) wheel        (0)    17038 2019-05-29 04:23:46.000000 banksync-0.9.4/banksync.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) wheel        (0)      330 2019-05-29 04:23:46.000000 banksync-0.9.4/banksync.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) wheel        (0)        1 2019-05-29 04:23:46.000000 banksync-0.9.4/banksync.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) wheel        (0)       46 2016-12-01 17:22:32.000000 banksync-0.9.4/banksync.egg-info/pbr.json
--rw-r--r--   0 jason      (501) wheel        (0)       52 2019-05-29 04:23:46.000000 banksync-0.9.4/banksync.egg-info/requires.txt
--rw-r--r--   0 jason      (501) wheel        (0)        9 2019-05-29 04:23:46.000000 banksync-0.9.4/banksync.egg-info/top_level.txt
-drwxr-xr-x   0 jason      (501) wheel        (0)        0 2019-05-29 04:23:47.000000 banksync-0.9.4/bin/
--rwxr-xr-x   0 jason      (501) wheel        (0)      262 2019-05-29 04:12:21.000000 banksync-0.9.4/bin/bank
--rwxr-xr-x   0 jason      (501) wheel        (0)      262 2019-05-29 04:12:21.000000 banksync-0.9.4/bin/banksync
--rw-r--r--   0 jason      (501) wheel        (0)       79 2019-05-29 04:23:47.000000 banksync-0.9.4/setup.cfg
--rw-r--r--   0 jason      (501) wheel        (0)     1618 2019-05-29 04:23:27.000000 banksync-0.9.4/setup.py
+drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:29:58.000000 banksync-0.9.9/
+-rw-r--r--   0 jason      (501) wheel        (0)     1504 2016-11-03 14:19:14.000000 banksync-0.9.9/LICENSE.txt
+-rw-r--r--   0 jason      (501) wheel        (0)    15294 2023-05-07 19:29:58.000000 banksync-0.9.9/PKG-INFO
+-rw-r--r--   0 jason      (501) wheel        (0)    14406 2023-05-07 19:28:58.000000 banksync-0.9.9/README.md
+drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync/
+-rwxr-xr-x   0 jason      (501) wheel        (0)       30 2016-11-17 20:03:24.000000 banksync-0.9.9/banksync/__init__.py
+-rwxr-xr-x   0 jason      (501) wheel        (0)    41943 2023-05-07 19:28:58.000000 banksync-0.9.9/banksync/banksync.py
+-rwxr-xr-x   0 jason      (501) wheel        (0)    14890 2023-05-07 19:28:58.000000 banksync-0.9.9/banksync/banksync_common.py
+drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync.egg-info/
+-rw-r--r--   0 jason      (501) wheel        (0)    15294 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) wheel        (0)      326 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) wheel        (0)        1 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) wheel        (0)       52 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) wheel        (0)        9 2023-05-07 19:29:58.000000 banksync-0.9.9/banksync.egg-info/top_level.txt
+drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:29:58.000000 banksync-0.9.9/bin/
+-rwxr-xr-x   0 jason      (501) wheel        (0)      246 2021-02-27 05:41:33.000000 banksync-0.9.9/bin/bank
+-rwxr-xr-x   0 jason      (501) wheel        (0)      246 2021-02-27 05:41:33.000000 banksync-0.9.9/bin/banksync
+-rw-r--r--   0 jason      (501) wheel        (0)      103 2021-02-27 16:30:49.000000 banksync-0.9.9/pyproject.toml
+-rw-r--r--   0 jason      (501) wheel        (0)       79 2023-05-07 19:29:58.000000 banksync-0.9.9/setup.cfg
+-rw-r--r--   0 jason      (501) wheel        (0)     1879 2021-02-27 16:51:04.000000 banksync-0.9.9/setup.py
+drwxr-xr-x   0 jason      (501) wheel        (0)        0 2023-05-07 19:29:58.000000 banksync-0.9.9/tests/
+-rw-r--r--   0 jason      (501) wheel        (0)      546 2023-05-06 14:37:19.000000 banksync-0.9.9/tests/test_setup.py
```

### Comparing `banksync-0.9.4/LICENSE.txt` & `banksync-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `banksync-0.9.4/PKG-INFO` & `banksync-0.9.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,321 +1,340 @@
 Metadata-Version: 2.1
 Name: banksync
-Version: 0.9.4
+Version: 0.9.9
 Summary: A library for manipulating banks of git repositories
 Home-page: https://github.com/jasonfharris/banksync
+Download-URL: https://github.com/jasonfharris/banksync/tarball/0.9.9
 Author: Jason Harris
 Author-email: jason@jasonfharris.com
 License: MIT
-Download-URL: https://github.com/jasonfharris/banksync/tarball/0.9.4
-Description: ## Purpose
-        
-        The banksync command line tool allows the easy operation of git commands across a "bank" or "collection" or repositories. It allows synchronization to historic configurations across the bank of repos.
-        
-        ## Installation
-        
-        You can install `banksync` from PyPi with a simple:
-        
-        ```
-        pip install banksync
-        ```
-        
-        ## Quickstart
-        
-        A bank is a collection of repos. The collection of repos is specified in a *syncfile*. The syncfile typically lives in *syncrepo*. So let us demonstrate this with a trivial collection of repos. The overall project will be called `animals` and it will contain a repo `repoFish` and a repo `repoBirds`. The project can live anywhere but to make the description easy let us put the project in the users root directory.
-        
-        So make a directory `animals`:
-        
-            cd ~
-            mkdir animals
-            cd animals
-        
-        Now clone the demonstration syncrepo for the animals project using standard git:
-        
-            git clone https://github.com/testbank/animalsRepoSync.git
-        
-        This will clone the thin repo which records the syncfile over time. Ie it records the state of the repos in the bank at different times / stages. We now have the hierarchy:
-        
-            animals
-            └── animalsRepoSync
-                ├── bankconfig.ini
-                └── syncfile.wl
-        
-        Now we enter into this directory and we clone the repositories in the bank
-        
-            cd animalsRepoSync
-            bank clone
-        
-        The clone command will clone all of the repos specified in the syncfile and we will now have the following layout:
-        
-            animals
-            ├── animalsRepoSync
-            │   ├── bankconfig.ini
-            │   └── syncfile.wl
-            ├── repoBird
-            │   └── Bird.txt
-            └── repoFish
-                └── Fish.txt
-        
-        We can now issue commands across the repos in the bank. From the syncrepo we can execute:
-        
-            cd ~/animals/animalsRepoSync
-            bank git status
-        
-        Which will execute the status command in each of the repos in the bank. If we want to checkout a previous state across the repos in the project we can do this via (from the syncrepo):
-        
-            git checkout master~2
-            bank sync
-        
-        The last two commands just moved the syncrepo two revisions back, and then synchronized the repos in the bank to the sync file at this earlier time. To get all repos back to the master branch revisions you can simply execute:
-        
-            bank gitall checkout master
-        
-        Which will do a `git checkout master` on all the repos in the bank including the sync repo.
-        
-        ## Syncfile
-        
-        The syncfile specifies which repositories are part of the bank, and what state the repositories should be synchronized to. A typical simple sync file might be the following
-        
-            more ~/animals/animalsRepoSync/syncfile.wl
-        
-        Which yields:
-        
-        ```
-        <|
-            "repoFish" -> <|
-                "path" -> "repoFish",
-                "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
-                "UnixTimeStamp" -> "1480517200",
-                "date" -> "30 Nov 2016 - 15:46:40",
-                "author" -> "Jason Harris",
-                "revisionNumber" -> "3",
-                "message" -> "committing salmon",
-                "cloneURL" -> "https://github.com/testbank/repoFish.git"
-            |>,
-            "repoBird" -> <|
-                "path" -> "repoBird",
-                "sha" -> "6bf9d646b2aa224b64fb86cbddb4d7ab0f2e37d3",
-                "UnixTimeStamp" -> "1480517200",
-                "date" -> "30 Nov 2016 - 15:46:40",
-                "author" -> "Jason Harris",
-                "revisionNumber" -> "3",
-                "message" -> "committing eagle",
-                "cloneURL" -> "https://github.com/testbank/repoBird.git"
-            |>
-        |>
-        ```
-        
-        The syncfile should lie inside a git repo (the syncrepo). Whenever we want to record a configuration of the repos we simply alter the syncfile by transcribing the current state of the repos into the syncfile using `bank recordRepos` with the appropriate options. We then use `git commit` to record this new state / configuration in the syncrepo.
-        
-        So let us add some content to repoBird in our example and then commit this change.
-        
-            cd  ~/animals/repoBird
-            echo "toucan" >> Bird.txt
-            git commit -am "committing toucan"
-        
-        So now we can update the syncfile with the state of the current repos in the bank:
-        
-            cd ~/animals/animalsRepoSync/
-            bank recordRepos
-        
-        The contents of our syncfile will now be something like:
-        
-        ```
-        <|
-            "repoFish" -> <|
-                "path" -> "repoFish",
-                "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
-                "UnixTimeStamp" -> "1480517200",
-                "date" -> "30 Nov 2016 - 15:46:40",
-                "author" -> "Jason Harris",
-                "revisionNumber" -> "3",
-                "message" -> "committing salmon",
-                "cloneURL" -> "https://github.com/testbank/repoFish.git"
-            |>,
-            "repoBird" -> <|
-                "path" -> "repoBird",
-                "sha" -> "c8fb05947c5161e484104d99f427ec082fb4e85b",
-                "UnixTimeStamp" -> "1480519159",
-                "date" -> "30 Nov 2016 - 16:19:19",
-                "author" -> "Jason Harris",
-                "revisionNumber" -> "4",
-                "message" -> "committing toucan",
-                "cloneURL" -> "https://github.com/testbank/repoBird.git"
-            |>
-        |>
-        ```
-        
-        (Note the sha, timestamps, and other data about the state of the repo `repoBird` has changed.)
-        
-        So we could now record this new overall state of the repos in the bank via simply committing the file syncfile in the syncrepo.
-        
-            git commit -am "recording the latest state of the repos in animals."
-        
-        ## Locations
-        
-        How does the bank command know where to put the `repoBird` and `repoFish`? How does it know which syncfile to use, etc. Well in the syncrepo there is the file `bankconfig.ini`. This is a standard preferences file but in this example it has two important options: `cwd=..` and `syncfile=syncfile.wl`.
-        
-        The cwd (ChangeWorkingDirectory) option specifies that the repo commands should be executed one level up from our current working directory. So since we are currently at `~/animals/animalsRepoSync` that means that the repos paths will start from `~/animals/`
-        
-        The second option just tells us what the name of the syncfile is. We could have called it `earthanimals.wl` if we wanted to.
-        
-        ## Bank command line options
-        
-        The command line tool `bank` has several options which can be specified:
-        
-        #### --syncfile <path>
-        
-        The `syncfile` option specifies a syncfile. The syncfile contents specify which repos are part of the bank. The various keys which are recorded if present are:`path`, `sha`, `UnixTimeStamp`, `date`, `author`, `revisionNumber`, `message`, and `cloneURL`. Adding other keys at present will not effect or change the behavior of the bank tool so you can add other info as you see fit / want to each of the recorded states in the various repos.
-        
-        #### --cwd <path>
-        
-        The cwd option will change the working directory. Using this you can specify the relative path to get to the base of where the path for each of the repos in the bank are. For instance in the layout example of the animals project above, if we are in the directory `animals/animalsSyncRepo` then since the path in the syncfile for "Birds" is just `repoBird` then relative to `animals/animalsSyncRepo` we want the directory `../repoBird`. So we would use the option `--cwd ..`
-        
-        #### --dryrun
-        
-        If this option is specified then `banksync` will report what it *would* do but it doesn't actually do anything.
-        
-        #### --colorize <bool>
-        
-        You can specify if color is not to be used in output if for instance you want the logs to be parsed in jenkins or other devops tools. (The default is `True`, i.e. colorize the output of the bank command)
-        
-        #### --verbosity <num>
-        
-        You can specify how much information banksync reports. This integer should be between 0, 1, 2, 3, or 4. The higher the number the more verbose is the reporting. The default is 2.
-        
-        #### --matching <type>
-        
-        When attempting to sync the constituent repos to the versions specified in the syncfile, how do we determine what to set the versions to? We want some loose coupling in that for instance if someone runs filter branch on a project or they do some rebase very early on in the history then the shas will change on all the revisions in the repository. So instead of finding a commit via a sha we will have to fall back to looking for a matching timestamp for the revision. These are generally fairly unique in a project unless a lot of cherrypicking has gone on. If we don't find that exact timestamp then we could fall back to the closest matching revision to that timestamp. In this way at least we have some hope of getting close to the configuration at the time instead of just giving up. Ie we get to the exact configuration if it is available but if not get as close as we can. The value of the option can be:
-        
-        - **shaOnly**: if we can't find the exact same revision given by the sha in the syncfile than give up.
-        - **timestamps**: try matching by sha first but if that fails find the first revision with the same unix timestamp. (This is almost always preserved across repo manipulation)
-        - **closetimestamps**: try matching by sha first, if that fails try matching by timestamp. and if that fails find the revision with the closest timestamp and match to that.
-        
-        ## Config file
-        
-        Instead of specifying the `--syncfile` and`—cwd` in each command you can create a `bankconfig.ini` file alongside the syncfile. In the `bankconfig.ini` file you can specify the default syncfile and cwd to use if none is specified. Eg we could add the file `animals/animalsSyncRepo/bankconfig.ini` with the following contents:
-        
-        ```
-        [General]
-        cwd=..
-        syncFile=syncfile.wl
-        ```
-        
-        Then you could omit the options to the bank command and they would be taken from the bankconfig.ini file so the above example would become:
-        
-        ```
-        cd animals/animalsSyncRepo
-        bank recordRepos
-        git commit -am "recording the latest state of the repos in animals."
-        ```
-        
-        You can choose weather to include the `bankconfig.ini` in the syncrepo history or not. (We choose to in this example but other teams may leave this to the individual developers.)
-        
-        ## Commands
-        
-        The form of a bank command is `bank <cmd> <opts>` where `<cmd>` is one of `sync`, `recordRepos`, `createSyncfile`, `bisect`, `clone`,  `git` or `gitall` 
-        
-        #### bank sync <opts>
-        
-        `sync` will update / checkout the revisions specified in the syncfile for each of the repos specified in the bank.
-        
-        ```
-        bank sync --syncfile syncfile.wl
-        ```
-        
-        This would checkout / update the repos given in the syncfile `syncfile.wl` to the states given in the syncfile. It each repo it tries to checkout the version first by the given sha, and then it falls back to the given timestamp, and then it falls back to the closest timestamp. (This fallback behavior can be controlled by the `--matching` option.)
-        
-        ```
-        bank sync --syncfile syncfile.wl --cwd ../other/dir
-        ```
-        
-        This would checkout / update the repos given in the syncfile to the states given in the syncfile
-        (but the path to each repo in the bank will be prefixed by the value of the `--cwd` option `../other/dir`).
-        
-        #### bank recordRepos <opts>
-        
-        `recordRepos` is used to transcribe the current state of the repos into the syncfile. Eg:
-        
-        ```
-        bank recordRepos --syncfile syncfile.wl
-        ```
-        
-        This would alter the contents of the syncfile and change the revisions stored in the syncfile.wl to match the current revisions of the referenced repositories.
-        
-        #### bank createSyncfile <opts>
-        
-        `createSyncfile` is used to generate an initial syncfile. Eg:
-        
-        ```
-        bank createSyncfile --syncfile syncfile.wl repo1 repo2 ... repoN --cwd some/dir
-        ```
-        
-        This would generate or overwrite the syncfile.wl to contain sync points for the current states of `repo1`, `repo2`, ... `repoN`
-        
-        #### bank createSyncrepo <opts>
-        
-        `createSyncrepo` is used to generate the syncrepo directory, initialize a git repository there, create the syncfile and also create the bankconfig.ini file. Basically it creates all the working parts of a syncrepo. Eg:
-        
-        ```
-        bank createSyncrepo repo1 repo2 ... repoN
-        ```
-        
-        This would create the directory `syncrepo` and fill it with a `syncfile.json` and a `bankconfig.ini`. The syncfile would contain the latest states of the `repo1`, `repo2`, ... `repoN`. 
-        
-        ```
-        bank createSyncrepo --syncreponame controlrepo --syncfilename felipe.json repo1 repo2 ... repoN
-        ```
-        Would create and initialize a syncrepo called `controlrepo` and inside that a syncfile called `felipe.json`.
-        
-        #### bank bisect <opts>
-        
-        You can use `bank bisect` on the syncrepo to step through historic configurations looking for a configuration which produces some change. (Typically we are searching for a regression.) Eg if we have a configuration file in the syncrepo the following might be a typical bisect session:
-        
-            cd SomeSyncRepo
-            bank bisect start
-            bank bisect good 12e4f5
-            bank bisect bad master
-            <do build / test>
-            bank bisect good 78a6b9
-            <do build / test>
-            bank bisect bad ae726a
-            ...
-        
-        Basically we are git bisecting on the syncrepo, and after each bisect step we get a new configuration, then `bank sync` will be run to synchronize the repositories in the bank to their state at the time that iteration of the syncfile was recorded . So `bank bisect <arguments>` is basically equivalent to `git bisect <arguments>; bank sync`
-        
-        #### Dispatching git commands
-        
-        We can use `bank` to perform a git command on each repository in the bank. All git commands have the prefix 'git' along with the normal name of the git command. Eg
-        
-            bank git status --syncfile syncfile.wl
-        
-        Will perform a `git status` operation on each of the repositories in the bank and print the results to stdout.
-        
-        If you use `gitall` instead of `git` command, then the git command will also be run in the syncrepo.
-        
-            bank gitall status --syncfile syncfile.wl
-        
-        Will perform a `git status` operation on each of the repositories in the bank and print the results to stdout.
-        
-        ## Testing
-        
-        To run the test suite you need `py.test` installed on your machine. Then after downloading the source code you can simply execute:
-        
-        ```
-        cd banksync_Package
-        py.test
-        ```
-        
 Keywords: execute,shell,system,git,submodule
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+## Purpose
+
+`banksync` is a command line tool that simplifies the use of git commands across a "bank" or "collection" of repositories. It enables synchronization of historical configurations throughout the bank of repos.
+
+## Installation
+
+You can install `banksync` from PyPi with a simple:
+
+
+    pip install banksync
+
+## Quick Start
+
+A bank is a collection of repos defined in a *syncfile*. The syncfile typically resides in a *syncrepo*. In this example, we'll use a project called `animals` containing two repos: `repoFish` and `repoBirds`. The project can be placed anywhere, but for simplicity, we'll put it in the user's root directory.
+
+To quickly clone and populate the example collection of repos, use the following commands:
+
+    cd ~
+    bank clone https://github.com/testbank/animalsRepoSync.git animals
+
+This will git clone the thin syncrepo, which contains the syncfile, and then populate all constituent repos. The resulting structure will be:
+
+    animals
+    ├── repoBird
+    │   └── Bird.txt
+    ├── repoFish
+    │   └── Fish.txt
+    └── syncrepo
+        ├── bankconfig.ini
+        └── syncfile.json
+
+
+Let's walk quickly through what is happening
+
+### Step-by-step Walkthrough
+
+Let's break down the quick start process into steps.
+
+1. Create a directory `animals`:
+
+   ```
+   cd ~
+   sudo rm -r animals
+   mkdir animals
+   cd animals
+   ```
+
+2. Clone the demonstration syncrepo for the animals project using standard git:
+
+   ```
+   git clone https://github.com/testbank/animalsRepoSync.git
+   ```
+
+   This clones the thin repo, which records the syncfile over time. It tracks the state of the repos in the bank at different times or stages. The resulting hierarchy is:
+
+   ```
+   animals
+   └── animalsRepoSync
+       ├── bankconfig.ini
+       └── syncfile.json
+   ```
+
+3. Populate the repositories in the bank:
+
+   ```
+   cd animalsRepoSync
+   bank populate
+   ```
+
+   The `populate` command clones each of the repos specified in the syncfile, resulting in the following layout:
+
+   ```
+   animals
+   ├── animalsRepoSync
+   │   ├── bankconfig.ini
+   │   └── syncfile.json
+   ├── repoBird
+   │   └── Bird.txt
+   └── repoFish
+       └── Fish.txt
+   ```
+
+### issuing commands
+
+We can now issue commands across the repos in the bank. From the syncrepo we can execute:
+
+    cd ~/animals/animalsRepoSync
+    bank git status
+
+Which will execute the status command in each of the repos in the bank. If we want to checkout a previous state across the repos in the project we can do this via (from the syncrepo):
+
+    git checkout master~2
+    bank sync
+
+The last two commands just moved the syncrepo two revisions back, and then synchronized the repos in the bank to the sync file at this earlier time. To get all repos back to the master branch revisions you can simply execute:
+
+    bank gitall checkout master
+
+Which will do a `git checkout master` on all the repos in the bank including the sync repo.
+
+## Syncfile
+
+The syncfile specifies which repositories are part of the bank, and what state the repositories should be synchronized to. A typical simple sync file might be the following
+
+    more ~/animals/animalsRepoSync/syncfile.json
+
+Which yields:
+
+```
+<|
+    "repoFish" -> <|
+        "path" -> "repoFish",
+        "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
+        "UnixTimeStamp" -> "1480517200",
+        "date" -> "30 Nov 2016 - 15:46:40",
+        "author" -> "Jason Harris",
+        "revisionNumber" -> "3",
+        "message" -> "committing salmon",
+        "cloneURL" -> "https://github.com/testbank/repoFish.git"
+    |>,
+    "repoBird" -> <|
+        "path" -> "repoBird",
+        "sha" -> "6bf9d646b2aa224b64fb86cbddb4d7ab0f2e37d3",
+        "UnixTimeStamp" -> "1480517200",
+        "date" -> "30 Nov 2016 - 15:46:40",
+        "author" -> "Jason Harris",
+        "revisionNumber" -> "3",
+        "message" -> "committing eagle",
+        "cloneURL" -> "https://github.com/testbank/repoBird.git"
+    |>
+|>
+```
+
+The syncfile should lie inside a git repo (the syncrepo). Whenever we want to record a configuration of the repos we simply alter the syncfile by transcribing the current state of the repos into the syncfile using `bank record_repos` with the appropriate options. We then use `git commit` to record this new state / configuration in the syncrepo.
+
+So let us add some content to repoBird in our example and then commit this change.
+
+    cd  ~/animals/repoBird
+    echo "toucan" >> Bird.txt
+    git commit -am "committing toucan"
+
+So now we can update the syncfile with the state of the current repos in the bank:
+
+    cd ~/animals/animalsRepoSync/
+    bank record_repos
+
+The contents of our syncfile will now be something like:
+
+```
+<|
+    "repoFish" -> <|
+        "path" -> "repoFish",
+        "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
+        "UnixTimeStamp" -> "1480517200",
+        "date" -> "30 Nov 2016 - 15:46:40",
+        "author" -> "Jason Harris",
+        "revisionNumber" -> "3",
+        "message" -> "committing salmon",
+        "cloneURL" -> "https://github.com/testbank/repoFish.git"
+    |>,
+    "repoBird" -> <|
+        "path" -> "repoBird",
+        "sha" -> "c8fb05947c5161e484104d99f427ec082fb4e85b",
+        "UnixTimeStamp" -> "1480519159",
+        "date" -> "30 Nov 2016 - 16:19:19",
+        "author" -> "Jason Harris",
+        "revisionNumber" -> "4",
+        "message" -> "committing toucan",
+        "cloneURL" -> "https://github.com/testbank/repoBird.git"
+    |>
+|>
+```
+
+(Note the sha, timestamps, and other data about the state of the repo `repoBird` has changed.)
+
+So we could now record this new overall state of the repos in the bank via simply committing the file syncfile in the syncrepo.
+
+    git commit -am "recording the latest state of the repos in animals."
+
+## Locations
+
+How does the bank command know where to put the `repoBird` and `repoFish`? How does it know which syncfile to use, etc. Well in the syncrepo there is the file `bankconfig.ini`. This is a standard preferences file but in this example it has two important options: `cwd=..` and `syncfile=syncfile.json`.
+
+The cwd (ChangeWorkingDirectory) option specifies that the repo commands should be executed one level up from our current working directory. So since we are currently at `~/animals/animalsRepoSync` that means that the repos paths will start from `~/animals/`
+
+The second option just tells us what the name of the syncfile is. We could have called it `earthanimals.json` if we wanted to.
+
+## Bank command line options
+
+The command line tool `bank` has several options which can be specified:
+
+#### --syncfile <path>
+
+The `syncfile` option specifies a syncfile. The syncfile contents specify which repos are part of the bank. The various keys which are recorded if present are:`path`, `sha`, `UnixTimeStamp`, `date`, `author`, `revisionNumber`, `message`, and `cloneURL`. Adding other keys at present will not effect or change the behavior of the bank tool so you can add other info as you see fit / want to each of the recorded states in the various repos.
+
+#### --cwd <path>
+
+The cwd option will change the working directory. Using this you can specify the relative path to get to the base of where the path for each of the repos in the bank are. For instance in the layout example of the animals project above, if we are in the directory `animals/animalsSyncRepo` then since the path in the syncfile for "Birds" is just `repoBird` then relative to `animals/animalsSyncRepo` we want the directory `../repoBird`. So we would use the option `--cwd ..`
+
+#### --dryrun
+
+If this option is specified then `banksync` will report what it *would* do but it doesn't actually do anything.
+
+#### --colorize <bool>
+
+You can specify if color is not to be used in output if for instance you want the logs to be parsed in jenkins or other devops tools. (The default is `True`, i.e. colorize the output of the bank command)
+
+#### --verbosity <num>
+
+You can specify how much information banksync reports. This integer should be between 0, 1, 2, 3, or 4. The higher the number the more verbose is the reporting. The default is 2.
+
+#### --matching <type>
+
+When attempting to sync the constituent repos to the versions specified in the syncfile, how do we determine what to set the versions to? We want some loose coupling in that for instance if someone runs filter branch on a project or they do some rebase very early on in the history then the shas will change on all the revisions in the repository. So instead of finding a commit via a sha we will have to fall back to looking for a matching timestamp for the revision. These are generally fairly unique in a project unless a lot of cherrypicking has gone on. If we don't find that exact timestamp then we could fall back to the closest matching revision to that timestamp. In this way at least we have some hope of getting close to the configuration at the time instead of just giving up. Ie we get to the exact configuration if it is available but if not get as close as we can. The value of the option can be:
+
+- **shaOnly**: if we can't find the exact same revision given by the sha in the syncfile than give up.
+- **timestamps**: try matching by sha first but if that fails find the first revision with the same unix timestamp. (This is almost always preserved across repo manipulation)
+- **closetimestamps**: try matching by sha first, if that fails try matching by timestamp. and if that fails find the revision with the closest timestamp and match to that.
+
+## Config file
+
+Instead of specifying the `--syncfile` and`—cwd` in each command you can create a `bankconfig.ini` file alongside the syncfile. In the `bankconfig.ini` file you can specify the default syncfile and cwd to use if none is specified. Eg we could add the file `animals/animalsSyncRepo/bankconfig.ini` with the following contents:
+
+    [general]
+    cwd=..
+    syncFile=syncfile.json
+
+Then you could omit the options to the bank command and they would be taken from the bankconfig.ini file so the above example would become:
+
+    cd animals/animalsSyncRepo
+    bank record_repos
+    git commit -am "recording the latest state of the repos in animals."
+
+You can choose weather to include the `bankconfig.ini` in the syncrepo history or not. (We choose to in this example but other teams may leave this to the individual developers.)
+
+## Commands
+
+The form of a bank command is `bank <cmd> <opts>` where `<cmd>` is one of `sync`, `record_repos`, `create_syncfile`, `bisect`, `populate`,  `git` or `gitall` 
+
+#### bank sync <opts>
+
+`sync` will update / checkout the revisions specified in the syncfile for each of the repos specified in the bank.
+
+    bank sync --syncfile syncfile.json
+
+This would checkout / update the repos given in the syncfile `syncfile.json` to the states given in the syncfile. It each repo it tries to checkout the version first by the given sha, and then it falls back to the given timestamp, and then it falls back to the closest timestamp. (This fallback behavior can be controlled by the `--matching` option.)
+
+    bank sync --syncfile syncfile.json --cwd ../other/dir
+
+This would checkout / update the repos given in the syncfile to the states given in the syncfile
+(but the path to each repo in the bank will be prefixed by the value of the `--cwd` option `../other/dir`).
+
+#### bank record_repos <opts>
+
+`record_repos` is used to transcribe the current state of the repos into the syncfile. Eg:
+
+    bank record_repos --syncfile syncfile.json
+
+This would alter the contents of the syncfile and change the revisions stored in the syncfile.json to match the current revisions of the referenced repositories.
+
+#### bank create_syncfile <opts>
+
+`create_syncfile` is used to generate an initial syncfile. Eg:
+
+    bank create_syncfile --syncfile syncfile.json repo1 repo2 ... repoN --cwd some/dir
+
+This would generate or overwrite the syncfile.json to contain sync points for the current states of `repo1`, `repo2`, ... `repoN`
+
+#### bank create_syncrepo <opts>
+
+`create_syncrepo` is used to generate the syncrepo directory, initialize a git repository there, create the syncfile and also create the bankconfig.ini file. Basically it creates all the working parts of a syncrepo. Eg:
+
+    bank create_syncrepo repo1 repo2 ... repoN
+
+This would create the directory `syncrepo` and fill it with a `syncfile.json` and a `bankconfig.ini`. The syncfile would contain the latest states of the `repo1`, `repo2`, ... `repoN`. 
+
+    bank create_syncrepo --syncreponame controlrepo --syncfilename felipe.json repo1 repo2 ... repoN
+
+Would create and initialize a syncrepo called `controlrepo` and inside that a syncfile called `felipe.json`.
+
+#### bank bisect <opts>
+
+You can use `bank bisect` on the syncrepo to step through historic configurations looking for a configuration which produces some change. (Typically we are searching for a regression.) Eg if we have a configuration file in the syncrepo the following might be a typical bisect session:
+
+    cd SomeSyncRepo
+    bank bisect start
+    bank bisect good 12e4f5
+    bank bisect bad master
+    <do build / test>
+    bank bisect good 78a6b9
+    <do build / test>
+    bank bisect bad ae726a
+    ...
+
+Basically we are git bisecting on the syncrepo, and after each bisect step we get a new configuration, then `bank sync` will be run to synchronize the repositories in the bank to their state at the time that iteration of the syncfile was recorded . So `bank bisect <arguments>` is basically equivalent to `git bisect <arguments>; bank sync`
+
+#### Dispatching git commands
+
+We can use `bank` to perform a git command on each repository in the bank. All git commands have the prefix 'git' along with the normal name of the git command. Eg
+
+    bank git status --syncfile syncfile.json
+
+Will perform a `git status` operation on each of the repositories in the bank and print the results to stdout.
+
+If you use `gitall` instead of `git` command, then the git command will also be run in the syncrepo.
+
+    bank gitall status --syncfile syncfile.json
+
+Will perform a `git status` operation on each of the repositories in the bank and print the results to stdout.
+
+## Testing
+
+To run the test suite you need `py.test` installed on your machine. Then after downloading the source code you can simply execute:
+
+    cd banksync_Package
+    py.test
+
```

### Comparing `banksync-0.9.4/README.md` & `banksync-0.9.9/banksync.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,113 @@
+Metadata-Version: 2.1
+Name: banksync
+Version: 0.9.9
+Summary: A library for manipulating banks of git repositories
+Home-page: https://github.com/jasonfharris/banksync
+Download-URL: https://github.com/jasonfharris/banksync/tarball/0.9.9
+Author: Jason Harris
+Author-email: jason@jasonfharris.com
+License: MIT
+Keywords: execute,shell,system,git,submodule
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Version Control
+Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 ## Purpose
 
-The banksync command line tool allows the easy operation of git commands across a "bank" or "collection" or repositories. It allows synchronization to historic configurations across the bank of repos.
+`banksync` is a command line tool that simplifies the use of git commands across a "bank" or "collection" of repositories. It enables synchronization of historical configurations throughout the bank of repos.
 
 ## Installation
 
 You can install `banksync` from PyPi with a simple:
 
-```
-pip install banksync
-```
-
-## Quickstart
 
-A bank is a collection of repos. The collection of repos is specified in a *syncfile*. The syncfile typically lives in *syncrepo*. So let us demonstrate this with a trivial collection of repos. The overall project will be called `animals` and it will contain a repo `repoFish` and a repo `repoBirds`. The project can live anywhere but to make the description easy let us put the project in the users root directory.
+    pip install banksync
 
-So make a directory `animals`:
+## Quick Start
 
-    cd ~
-    mkdir animals
-    cd animals
+A bank is a collection of repos defined in a *syncfile*. The syncfile typically resides in a *syncrepo*. In this example, we'll use a project called `animals` containing two repos: `repoFish` and `repoBirds`. The project can be placed anywhere, but for simplicity, we'll put it in the user's root directory.
 
-Now clone the demonstration syncrepo for the animals project using standard git:
+To quickly clone and populate the example collection of repos, use the following commands:
 
-    git clone https://github.com/testbank/animalsRepoSync.git
+    cd ~
+    bank clone https://github.com/testbank/animalsRepoSync.git animals
 
-This will clone the thin repo which records the syncfile over time. Ie it records the state of the repos in the bank at different times / stages. We now have the hierarchy:
+This will git clone the thin syncrepo, which contains the syncfile, and then populate all constituent repos. The resulting structure will be:
 
     animals
-    └── animalsRepoSync
+    ├── repoBird
+    │   └── Bird.txt
+    ├── repoFish
+    │   └── Fish.txt
+    └── syncrepo
         ├── bankconfig.ini
-        └── syncfile.wl
+        └── syncfile.json
 
-Now we enter into this directory and we clone the repositories in the bank
 
-    cd animalsRepoSync
-    bank clone
+Let's walk quickly through what is happening
 
-The clone command will clone all of the repos specified in the syncfile and we will now have the following layout:
+### Step-by-step Walkthrough
 
-    animals
-    ├── animalsRepoSync
-    │   ├── bankconfig.ini
-    │   └── syncfile.wl
-    ├── repoBird
-    │   └── Bird.txt
-    └── repoFish
-        └── Fish.txt
+Let's break down the quick start process into steps.
+
+1. Create a directory `animals`:
+
+   ```
+   cd ~
+   sudo rm -r animals
+   mkdir animals
+   cd animals
+   ```
+
+2. Clone the demonstration syncrepo for the animals project using standard git:
+
+   ```
+   git clone https://github.com/testbank/animalsRepoSync.git
+   ```
+
+   This clones the thin repo, which records the syncfile over time. It tracks the state of the repos in the bank at different times or stages. The resulting hierarchy is:
+
+   ```
+   animals
+   └── animalsRepoSync
+       ├── bankconfig.ini
+       └── syncfile.json
+   ```
+
+3. Populate the repositories in the bank:
+
+   ```
+   cd animalsRepoSync
+   bank populate
+   ```
+
+   The `populate` command clones each of the repos specified in the syncfile, resulting in the following layout:
+
+   ```
+   animals
+   ├── animalsRepoSync
+   │   ├── bankconfig.ini
+   │   └── syncfile.json
+   ├── repoBird
+   │   └── Bird.txt
+   └── repoFish
+       └── Fish.txt
+   ```
+
+### issuing commands
 
 We can now issue commands across the repos in the bank. From the syncrepo we can execute:
 
     cd ~/animals/animalsRepoSync
     bank git status
 
 Which will execute the status command in each of the repos in the bank. If we want to checkout a previous state across the repos in the project we can do this via (from the syncrepo):
@@ -63,15 +121,15 @@
 
 Which will do a `git checkout master` on all the repos in the bank including the sync repo.
 
 ## Syncfile
 
 The syncfile specifies which repositories are part of the bank, and what state the repositories should be synchronized to. A typical simple sync file might be the following
 
-    more ~/animals/animalsRepoSync/syncfile.wl
+    more ~/animals/animalsRepoSync/syncfile.json
 
 Which yields:
 
 ```
 <|
     "repoFish" -> <|
         "path" -> "repoFish",
@@ -92,26 +150,26 @@
         "revisionNumber" -> "3",
         "message" -> "committing eagle",
         "cloneURL" -> "https://github.com/testbank/repoBird.git"
     |>
 |>
 ```
 
-The syncfile should lie inside a git repo (the syncrepo). Whenever we want to record a configuration of the repos we simply alter the syncfile by transcribing the current state of the repos into the syncfile using `bank recordRepos` with the appropriate options. We then use `git commit` to record this new state / configuration in the syncrepo.
+The syncfile should lie inside a git repo (the syncrepo). Whenever we want to record a configuration of the repos we simply alter the syncfile by transcribing the current state of the repos into the syncfile using `bank record_repos` with the appropriate options. We then use `git commit` to record this new state / configuration in the syncrepo.
 
 So let us add some content to repoBird in our example and then commit this change.
 
     cd  ~/animals/repoBird
     echo "toucan" >> Bird.txt
     git commit -am "committing toucan"
 
 So now we can update the syncfile with the state of the current repos in the bank:
 
     cd ~/animals/animalsRepoSync/
-    bank recordRepos
+    bank record_repos
 
 The contents of our syncfile will now be something like:
 
 ```
 <|
     "repoFish" -> <|
         "path" -> "repoFish",
@@ -140,19 +198,19 @@
 
 So we could now record this new overall state of the repos in the bank via simply committing the file syncfile in the syncrepo.
 
     git commit -am "recording the latest state of the repos in animals."
 
 ## Locations
 
-How does the bank command know where to put the `repoBird` and `repoFish`? How does it know which syncfile to use, etc. Well in the syncrepo there is the file `bankconfig.ini`. This is a standard preferences file but in this example it has two important options: `cwd=..` and `syncfile=syncfile.wl`.
+How does the bank command know where to put the `repoBird` and `repoFish`? How does it know which syncfile to use, etc. Well in the syncrepo there is the file `bankconfig.ini`. This is a standard preferences file but in this example it has two important options: `cwd=..` and `syncfile=syncfile.json`.
 
 The cwd (ChangeWorkingDirectory) option specifies that the repo commands should be executed one level up from our current working directory. So since we are currently at `~/animals/animalsRepoSync` that means that the repos paths will start from `~/animals/`
 
-The second option just tells us what the name of the syncfile is. We could have called it `earthanimals.wl` if we wanted to.
+The second option just tells us what the name of the syncfile is. We could have called it `earthanimals.json` if we wanted to.
 
 ## Bank command line options
 
 The command line tool `bank` has several options which can be specified:
 
 #### --syncfile <path>
 
@@ -182,84 +240,69 @@
 - **timestamps**: try matching by sha first but if that fails find the first revision with the same unix timestamp. (This is almost always preserved across repo manipulation)
 - **closetimestamps**: try matching by sha first, if that fails try matching by timestamp. and if that fails find the revision with the closest timestamp and match to that.
 
 ## Config file
 
 Instead of specifying the `--syncfile` and`—cwd` in each command you can create a `bankconfig.ini` file alongside the syncfile. In the `bankconfig.ini` file you can specify the default syncfile and cwd to use if none is specified. Eg we could add the file `animals/animalsSyncRepo/bankconfig.ini` with the following contents:
 
-```
-[General]
-cwd=..
-syncFile=syncfile.wl
-```
+    [general]
+    cwd=..
+    syncFile=syncfile.json
 
 Then you could omit the options to the bank command and they would be taken from the bankconfig.ini file so the above example would become:
 
-```
-cd animals/animalsSyncRepo
-bank recordRepos
-git commit -am "recording the latest state of the repos in animals."
-```
+    cd animals/animalsSyncRepo
+    bank record_repos
+    git commit -am "recording the latest state of the repos in animals."
 
 You can choose weather to include the `bankconfig.ini` in the syncrepo history or not. (We choose to in this example but other teams may leave this to the individual developers.)
 
 ## Commands
 
-The form of a bank command is `bank <cmd> <opts>` where `<cmd>` is one of `sync`, `recordRepos`, `createSyncfile`, `bisect`, `clone`,  `git` or `gitall` 
+The form of a bank command is `bank <cmd> <opts>` where `<cmd>` is one of `sync`, `record_repos`, `create_syncfile`, `bisect`, `populate`,  `git` or `gitall` 
 
 #### bank sync <opts>
 
 `sync` will update / checkout the revisions specified in the syncfile for each of the repos specified in the bank.
 
-```
-bank sync --syncfile syncfile.wl
-```
+    bank sync --syncfile syncfile.json
 
-This would checkout / update the repos given in the syncfile `syncfile.wl` to the states given in the syncfile. It each repo it tries to checkout the version first by the given sha, and then it falls back to the given timestamp, and then it falls back to the closest timestamp. (This fallback behavior can be controlled by the `--matching` option.)
+This would checkout / update the repos given in the syncfile `syncfile.json` to the states given in the syncfile. It each repo it tries to checkout the version first by the given sha, and then it falls back to the given timestamp, and then it falls back to the closest timestamp. (This fallback behavior can be controlled by the `--matching` option.)
 
-```
-bank sync --syncfile syncfile.wl --cwd ../other/dir
-```
+    bank sync --syncfile syncfile.json --cwd ../other/dir
 
 This would checkout / update the repos given in the syncfile to the states given in the syncfile
 (but the path to each repo in the bank will be prefixed by the value of the `--cwd` option `../other/dir`).
 
-#### bank recordRepos <opts>
+#### bank record_repos <opts>
 
-`recordRepos` is used to transcribe the current state of the repos into the syncfile. Eg:
+`record_repos` is used to transcribe the current state of the repos into the syncfile. Eg:
 
-```
-bank recordRepos --syncfile syncfile.wl
-```
+    bank record_repos --syncfile syncfile.json
 
-This would alter the contents of the syncfile and change the revisions stored in the syncfile.wl to match the current revisions of the referenced repositories.
+This would alter the contents of the syncfile and change the revisions stored in the syncfile.json to match the current revisions of the referenced repositories.
 
-#### bank createSyncfile <opts>
+#### bank create_syncfile <opts>
 
-`createSyncfile` is used to generate an initial syncfile. Eg:
+`create_syncfile` is used to generate an initial syncfile. Eg:
 
-```
-bank createSyncfile --syncfile syncfile.wl repo1 repo2 ... repoN --cwd some/dir
-```
+    bank create_syncfile --syncfile syncfile.json repo1 repo2 ... repoN --cwd some/dir
 
-This would generate or overwrite the syncfile.wl to contain sync points for the current states of `repo1`, `repo2`, ... `repoN`
+This would generate or overwrite the syncfile.json to contain sync points for the current states of `repo1`, `repo2`, ... `repoN`
 
-#### bank createSyncrepo <opts>
+#### bank create_syncrepo <opts>
 
-`createSyncrepo` is used to generate the syncrepo directory, initialize a git repository there, create the syncfile and also create the bankconfig.ini file. Basically it creates all the working parts of a syncrepo. Eg:
+`create_syncrepo` is used to generate the syncrepo directory, initialize a git repository there, create the syncfile and also create the bankconfig.ini file. Basically it creates all the working parts of a syncrepo. Eg:
 
-```
-bank createSyncrepo repo1 repo2 ... repoN
-```
+    bank create_syncrepo repo1 repo2 ... repoN
 
 This would create the directory `syncrepo` and fill it with a `syncfile.json` and a `bankconfig.ini`. The syncfile would contain the latest states of the `repo1`, `repo2`, ... `repoN`. 
 
-```
-bank createSyncrepo --syncreponame controlrepo --syncfilename felipe.json repo1 repo2 ... repoN
-```
+    bank create_syncrepo --syncreponame controlrepo --syncfilename felipe.json repo1 repo2 ... repoN
+
 Would create and initialize a syncrepo called `controlrepo` and inside that a syncfile called `felipe.json`.
 
 #### bank bisect <opts>
 
 You can use `bank bisect` on the syncrepo to step through historic configurations looking for a configuration which produces some change. (Typically we are searching for a regression.) Eg if we have a configuration file in the syncrepo the following might be a typical bisect session:
 
     cd SomeSyncRepo
@@ -274,25 +317,24 @@
 
 Basically we are git bisecting on the syncrepo, and after each bisect step we get a new configuration, then `bank sync` will be run to synchronize the repositories in the bank to their state at the time that iteration of the syncfile was recorded . So `bank bisect <arguments>` is basically equivalent to `git bisect <arguments>; bank sync`
 
 #### Dispatching git commands
 
 We can use `bank` to perform a git command on each repository in the bank. All git commands have the prefix 'git' along with the normal name of the git command. Eg
 
-    bank git status --syncfile syncfile.wl
+    bank git status --syncfile syncfile.json
 
 Will perform a `git status` operation on each of the repositories in the bank and print the results to stdout.
 
 If you use `gitall` instead of `git` command, then the git command will also be run in the syncrepo.
 
-    bank gitall status --syncfile syncfile.wl
+    bank gitall status --syncfile syncfile.json
 
 Will perform a `git status` operation on each of the repositories in the bank and print the results to stdout.
 
 ## Testing
 
 To run the test suite you need `py.test` installed on your machine. Then after downloading the source code you can simply execute:
 
-```
-cd banksync_Package
-py.test
-```
+    cd banksync_Package
+    py.test
+
```

### Comparing `banksync-0.9.4/banksync/banksync.py` & `banksync-0.9.9/banksync/banksync.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 #!/usr/bin/env python
 # PYTHON_ARGCOMPLETE_OK
 
 import os.path
-import string
 import sys
-import time
-import re
 import argparse
 import argcomplete
 import json
 from collections import OrderedDict
 from sysexecute import *
 from .banksync_common import *
 
-
+__version__ = "0.9.9"
 
 # --------------------------------------------------------------------------------------------------------------------------
 # Defines
 # --------------------------------------------------------------------------------------------------------------------------
 
 tryOrder = ["sha", "UnixTimeStamp"]
 defaultSyncPointBranchName = "syncPoint"
@@ -25,31 +22,31 @@
 
 
 # --------------------------------------------------------------------------------------------------------------------------
 # Command and Option setup
 # --------------------------------------------------------------------------------------------------------------------------
 
 defaultOptions = {
-    'General' : {
+    'general' : {
         'cwd' : '.',
-        'syncfile' : 'syncfile.wl',
+        'syncfile' : 'syncfile.json',
         'verbosity' : 2,
         'colorize' : 'yes',
         'seperator' : ' '
     },
     'sync' : {
         'matching' : 'closetimestamp'
     },
-    'createSyncrepo' : {
+    'create_syncrepo' : {
         'syncfilename' : 'syncfile.json',
         'syncreponame' : 'syncrepo'
     }
 }
 
-sync_commands = ['sync', 'recordRepos', 'createSyncfile', 'createSyncrepo', 'bisect', 'clone', 'git', 'gitall']
+sync_commands = ['sync', 'record_repos', 'create_syncfile', 'create_syncrepo', 'bisect', 'clone', 'populate', 'git', 'gitall']
 approved_git_commands = ['reset', 'log', 'status', 'branch', 'checkout', 'commit', 'tag', 'diff', 'fetch',
                          'push', 'pull', 'prune', 'gc', 'fsck', 'ls-files', 'ls-remote', 'ls-tree']
                          
 bisectSubCommands = ['start', 'bad', 'new', 'good', 'old', 'terms', 'skip', 'reset', 'visualize', 'replay', 'log', 'run']
 
 # This list was culled from `git help -a`
 allGitCommands = [
@@ -117,106 +114,129 @@
 
 #  CMD: sync ----------
 
 syncCmdHelp = 'checkout / update the repos given in the syncfile to the states given in the syncfile'
 syncCmdDescription = syncCmdHelp
 syncCmdEpilog = wrapParagraphs('''Example usage:
 
-  bank sync --syncfile syncfile.wl
+  bank sync --syncfile syncfile.json
 
-This would checkout / update the repos given in the syncfile.wl to the states given
-in the syncfile.wl.
+This would checkout / update the repos given in the syncfile.json to the states given
+in the syncfile.json.
 
-  bank sync --syncfile syncfile.wl --cwd ../other/dir
+  bank sync --syncfile syncfile.json --cwd ../other/dir
 
-This would checkout / update the repos given in the syncfile.wl to the states given
-in the syncfile.wl (but the path to the repos are prefixed by the value of cwd).
+This would checkout / update the repos given in the syncfile.json to the states given
+in the syncfile.json (but the path to the repos are prefixed by the value of cwd).
 
   bank sync
 
 Use the syncfile specified in the file bankconfig.ini and list the results of the sync
 on each repo in the bank.
 ''')
 
 
-#  CMD: recordRepos ----------
+#  CMD: record_repos ----------
 
-recordReposCmdHelp = 'alter the contents of the syncfile so that it matches the current revisions of the referenced repositories.'
-recordReposCmdDescription = recordReposCmdHelp
-recordReposCmdEpilog = wrapParagraphs('''Example usage:
+record_reposCmdHelp = 'alter the contents of the syncfile so that it matches the current revisions of the referenced repositories.'
+record_reposCmdDescription = record_reposCmdHelp
+record_reposCmdEpilog = wrapParagraphs('''Example usage:
 
-  bank recordRepos --syncfile syncfile.wl
+  bank record_repos --syncfile syncfile.json
 
-This would alter the contents of syncfile.wl so that it matches the current revisions of the referenced repositories.
+This would alter the contents of syncfile.json so that it matches the current revisions of the referenced repositories.
 ''')
 
 
-#  CMD: createSyncfile ----------
+#  CMD: create_syncfile ----------
 
-createSyncfileCmdHelp = 'create or overwrite the syncfile to contain the current sync states for the passed in repos.'
-createSyncfileCmdDescription = createSyncfileCmdHelp
-createSyncfileCmdEpilog = wrapParagraphs('''Example usage:
+create_syncfileCmdHelp = 'create or overwrite the syncfile to contain the current sync states for the passed in repos.'
+create_syncfileCmdDescription = create_syncfileCmdHelp
+create_syncfileCmdEpilog = wrapParagraphs('''Example usage:
 
-  bank createSyncfile --syncfile syncfile.wl --cwd .. repo1 repo2 ... repoN
+  bank create_syncfile --syncfile syncfile.json --cwd .. repo1 repo2 ... repoN
 
-This would create or overwrite the syncfile.wl to record the current states of repo1 repo2 ... repoN which are located
+This would create or overwrite the syncfile.json to record the current states of repo1 repo2 ... repoN which are located
 one directory level up.
 ''')
 
 
-#  CMD: createSyncrepo ----------
+#  CMD: create_syncrepo ----------
 
-createSyncrepoCmdHelp = 'create or overwrite the syncrepo to contain the current sync states for the passed in repos.'
-createSyncrepoCmdDescription = createSyncrepoCmdHelp
-createSyncrepoCmdEpilog = wrapParagraphs('''Example usage:
+create_syncrepoCmdHelp = 'create or overwrite the syncrepo to contain the current sync states for the passed in repos.'
+create_syncrepoCmdDescription = create_syncrepoCmdHelp
+create_syncrepoCmdEpilog = wrapParagraphs('''Example usage:
 
-  bank createSyncrepo repo1 repo2 ... repoN
+  bank create_syncrepo repo1 repo2 ... repoN
 
 This would create and initilize a git repository called syncrepo and inside there it would create the syncfile.json
 to record the current states of the repo1 repo2 ... repoN which are located at this level. It would also create the
 bankconfig.ini inside this repo.
 
-  bank createSyncrepo --syncrepo <syncreponame> repo1 repo2 ... repoN --cwd some/dir
+  bank create_syncrepo --syncrepo <syncreponame> repo1 repo2 ... repoN --cwd some/dir
 
 This would create the syncrepo as the above command, but the repo would be called syncreponame.
 ''')
 
 #  CMD: clone ----------
 
 cloneCmdHelp = 'clone the repos specified in the syncfile'
 cloneCmdDescription = cloneCmdHelp
 cloneCmdEpilog = wrapParagraphs('''Example usage:
 
-  bank clone --syncfile syncfile.wl
+  bank clone https://github.com/myProject/syncrepo.git myProject
 
-This would perform a git clone for each of the repositories specified in the syncfile
+This would create the folder myProject and clone the syncrepo into myProject, and then populate each of the constituent repositories specified in the syncfile.
 ''')
 
 
+#  CMD: populate ----------
+
+populateCmdHelp = 'populate the repos specified in the syncfile'
+populateCmdDescription = populateCmdHelp
+populateCmdEpilog = wrapParagraphs('''Example usage:
+
+  bank populate --syncfile syncfile.json
+
+This would perform a git clone for each of the repositories specified in the syncfile.
+''')
+
+
+#  CMD: status ----------
+
+statusCmdHelp = 'reports the status of the repos specified in the syncfile'
+statusCmdDescription = statusCmdHelp
+statusCmdEpilog = wrapParagraphs('''Example usage:
+
+  bank status --syncfile syncfile.json
+
+This would report the status of each of the repositories specified in the syncfile.
+''')
+
 #  CMD: bisect ----------
 
 bisectCmdHelp = 'bisect the syncrepo and sync all repos in the bank to the new state of the syncfile'
-bisectCmdDescription = cloneCmdHelp
+bisectCmdDescription = bisectCmdHelp
 bisectCmdEpilog = wrapParagraphs('''Example usage:
 
-  bank bisect --syncfile syncfile.wl reset
+  bank bisect --syncfile syncfile.json reset
 
 This would pass the reset to the bisection of the sync-repo.
 ''')
 
 
 #  CMD: git ----------
 
 gitCmdHelp = 'perform the given git command in each repo in the bank'
 gitCmdDescription = gitCmdHelp
 gitCmdEpilog = wrapParagraphs('''Example usage:
 
-  bank git status --syncfile syncfile.wl 
+  bank git status --syncfile syncfile.json 
 
-Perform git status and list the results on each of the repositories specified in the syncfile.wl
+Perform git status and list the results on each of the repositories specified in the syncfile.json
 
   bank git tag release_1.7.0.1
 
 Use the syncfile specified in the file bankconfig.ini and apply the command `git tag release_1.7.0.1` to each of the
 repos in the bank.
 ''')
 
@@ -231,17 +251,17 @@
 {approved_git_commands}. (Actually any git command can be used but so far only those common git
 commands have been "approved" as making sense in the setting of banksync. Some other git commands definitely do not make
 sense such as `git rebase --interactive` since the bank command is not interactive. Command completion on the command
 line only works for the common commands.
 
 Example usage:
 
-  bank gitall status --syncfile syncfile.wl 
+  bank gitall status --syncfile syncfile.json 
 
-Perform git status and list the results on each of the repositories specified in the syncfile.wl
+Perform git status and list the results on each of the repositories specified in the syncfile.json
 and in addition to the actual repo containing the sync file (the syncrepo)
 
   bank gitall tag release_1.7.0.1
 
 Use the syncfile specified in the file bankconfig.ini and apply the command `git tag release_1.7.0.1` to each of the
 repos in the bank and in addition to the actual repo containing the sync file (the syncrepo).
 ''')
@@ -250,309 +270,337 @@
 
     pathOps_parser = argparse.ArgumentParser(add_help=False)                                 
     pathOps_parser.add_argument("--syncfile", metavar="SYNCFILE", help="the path to the syncfile", default='auto')
     pathOps_parser.add_argument("--cwd", metavar="CWD", help="prefix / change the working directory for the repos in the sync file", default='auto')
 
     commonOpts_parser = argparse.ArgumentParser(add_help=False)                                 
     commonOpts_parser.add_argument("--verbosity", metavar="NUM", help="Specify the level of reported feedback / detail. Acceptable values: 1 (minimal feedback), 2 (some feedback) , 3 (detailed feedback), or 4 (full feedback)", type=int, default=autoNum)
-    commonOpts_parser.add_argument('--colorize', metavar='BOOL', help=stringWithVars("Colorize the output: {colorizeOptionValues}"), choices=colorizeOptionValues, default='auto')
+    commonOpts_parser.add_argument('--colorize', metavar='BOOL', help=f"Colorize the output: {colorizeOptionValues}", choices=colorizeOptionValues, default='auto')
     commonOpts_parser.add_argument('--dryrun', dest='dryrun', action='store_true', help="Print what would happen instead of performing the command")
     commonOpts_parser.set_defaults(dryrun=False)
 
     parser = argparse.ArgumentParser(description=mainDescription, epilog=mainEpilog, formatter_class=argparse.RawDescriptionHelpFormatter, prog='bank')
     parser.add_argument('--version', dest='version', action='store_true', help="Show the version number of the banksync tool and exit")
     parser.set_defaults(version=False)
 
-    subparsers = parser.add_subparsers(title='commands', dest='subparser_name', metavar = '')
+    subparsers = parser.add_subparsers(title='commands', dest='command', metavar = '')
     def addSubparser(name, parent_parsers=[pathOps_parser, commonOpts_parser]):
         return subparsers.add_parser(name, help=eval(name+'CmdHelp'), description=eval(name+'CmdDescription'), epilog=eval(name+'CmdEpilog'), parents = parent_parsers, formatter_class=argparse.RawDescriptionHelpFormatter)
         
     parser_syncCmd = addSubparser('sync')
-    parser_syncCmd.add_argument("--matching", metavar="MATCH", help=stringWithVars('specify how we can recognize a revision "match": {matchingOptionValues}'), choices=matchingOptionValues, default='auto')
+    parser_syncCmd.add_argument("--matching", metavar="MATCH", help=f'specify how we can recognize a revision "match": {matchingOptionValues}', choices=matchingOptionValues, default='auto')
+
+    parser_record_reposCmd = addSubparser('record_repos')
+
+    parser_create_syncfileCmd = addSubparser('create_syncfile')
+    parser_create_syncfileCmd.add_argument("repos", metavar="reponame", help='the repos to be included in the bank', nargs="+")
 
-    parser_recordReposCmd = addSubparser('recordRepos')
+    parser_create_syncrepoCmd = addSubparser('create_syncrepo', [commonOpts_parser])
+    parser_create_syncrepoCmd.add_argument("repos", metavar="reponame", help='the repos to be included in the bank', nargs="+")
+    parser_create_syncrepoCmd.add_argument("--syncfilename", metavar="NAME", help='specify the name and extension of the syncfile', default='auto')
+    parser_create_syncrepoCmd.add_argument("--syncreponame", metavar="NAME", help='specify the name of the syncrepo', default='auto')
 
-    parser_createSyncfileCmd = addSubparser('createSyncfile')
-    parser_createSyncfileCmd.add_argument("repos", metavar="reponame", help='the repos to be included in the bank', nargs="+")
+    parser_cloneCmd = addSubparser('clone', [commonOpts_parser])
+    parser_cloneCmd.add_argument("url", metavar="URL", help='the URL of the sync repo')
+    parser_cloneCmd.add_argument("name", metavar="NAME", help='the optional name for the repo', default=None, nargs='?')
 
-    parser_createSyncrepoCmd = addSubparser('createSyncrepo', [commonOpts_parser])
-    parser_createSyncrepoCmd.add_argument("repos", metavar="reponame", help='the repos to be included in the bank', nargs="+")
-    parser_createSyncrepoCmd.add_argument("--syncfilename", metavar="NAME", help='specify the name and extension of the syncfile', default='auto')
-    parser_createSyncrepoCmd.add_argument("--syncreponame", metavar="NAME", help='specify the name of the syncrepo', default='auto')
+    parser_populateCmd = addSubparser('populate')
 
-    parser_cloneCmd = addSubparser('clone')
+    parser_statusCmd = addSubparser('status')
 
     parser_bisectCmd = addSubparser('bisect')
-    parser_bisectCmd.add_argument("bisectcmd", metavar="BISECTCMD", nargs='?', help=stringWithVars("the bisect subcommand one of {bisectSubCommands}."), choices=bisectSubCommands, default='log')
+    parser_bisectCmd.add_argument("bisectcmd", metavar="BISECTCMD", nargs='?', help=f"the bisect subcommand one of {bisectSubCommands}.", choices=bisectSubCommands, default='log')
 
     parser_gitCmd = addSubparser('git')
-    parser_gitCmd.add_argument("gitcmd", metavar="GITCMD", nargs='?', help=stringWithVars("perform one of {approved_git_commands} on all the repos in the bank."), choices=allGitCommands, default='status')
+    parser_gitCmd.add_argument("gitcmd", metavar="GITCMD", nargs='?', help=f"perform one of {approved_git_commands} on all the repos in the bank.", choices=allGitCommands, default='status')
 
     parser_gitallCmd = addSubparser('gitall')
-    parser_gitallCmd.add_argument("gitcmd", metavar="GITCMD", nargs='?', help=stringWithVars("perform one of {approved_git_commands} on all the repos in the bank including the syncrepo."), choices=allGitCommands, default='status')
+    parser_gitallCmd.add_argument("gitcmd", metavar="GITCMD", nargs='?', help=f"perform one of {approved_git_commands} on all the repos in the bank including the syncrepo.", choices=allGitCommands, default='status')
 
     argcomplete.autocomplete(parser)
 
     def printVersionAndExit():
-        printWithVars1("banksync {__version__}. Author: Jason F Harris.\nhttps://github.com/jasonfharris/banksync")
+        printWithVars1(f"banksync {__version__}. Author: Jason F Harris.\nhttps://github.com/jasonfharris/banksync")
         sys.exit(0)
 
     if len(sys.argv)==1:
         parser.print_help()
         sys.exit(1)
 
     if len(sys.argv)==2 and sys.argv[1] == '--version':
         printVersionAndExit()
 
-    args, remainingArgs = parser.parse_known_args()
-    command = args.subparser_name
+    args, remaining_args = parser.parse_known_args()
+    command = args.command
 
     if (not command in commands) and (not command in allGitCommands):
-        printWithVars1("unknown command: {command}", 'red')
+        printWithVars1(f"unknown command: {command}", 'red')
         sys.exit(1)
 
-    remainingArgs = [correctlyQuoteArg(arg) for arg in remainingArgs]
+    remaining_args = [correctlyQuoteArg(arg) for arg in remaining_args]
     if args.version:
         printVersionAndExit()
     
-    return args, remainingArgs
+    return args, remaining_args
+
+
+
+# --------------------------------------------------------------------------------------------------------------------------
+# internal utilities
+# --------------------------------------------------------------------------------------------------------------------------
 
 
+def _green(text):
+    return colored(text, 'green')
+def _red(text):
+    return colored(text, 'red')
+def _yellow(text):
+    return colored(text, 'yellow')
 
+# def _green(text):
+#     if not colorize:
+#         return colored(text, 'green')
+# def _red(text):
+#     if not colorize:
+#         return colored(text, 'red')
+# def _yellow(text):
+#     if not colorize:
+#         return colored(text, 'yellow')
 
 
 # --------------------------------------------------------------------------------------------------------------------------
 # command "sync"
 # --------------------------------------------------------------------------------------------------------------------------
 
 def commandSync():
-    matching = resolvedOpts['sync']['matching']
+    matching = _config['sync.matching']
     checkForSyncRepo(syncFilePath)
     syncDict = loadSyncFileAsDict(syncFilePath)
     allFound = True
 
     for repoName in syncDict:
         repoInfo = syncDict[repoName]
         absRepoPath = getAbsRepoPath(repoInfo["path"], cwd)
         repoString = paddedRepoName(repoName, list(syncDict.keys()))
-        greenRepoString  = colored(repoString, 'green')
-        redRepoString    = colored(repoString, 'red')
-        yellowRepoString = colored(repoString, 'yellow')
         if not checkForRepo(repoString, absRepoPath):
             allFound = False
             continue
     
         found = False
         for method in tryOrder:
             if found:
                 break
 
             if (method == "sha") and ("sha" in repoInfo):
                 hash = repoInfo["sha"]
                 shortHash = hash[0:12]
                 if dryrun:
-                    printWithVars2("{repoString}: would try and check out revision by {method}: {shortHash}", dryrun=False)
+                    printWithVars2(f"{repoString}: would try and check out revision by {method}: {shortHash}", dryrun=False)
                     break
+                
+                print(f"\r>> checking out {hash}...", end='', flush=True)
                 res = gitCommand("git checkout -B {defaultSyncPointBranchName} {hash}", 3, cwd=absRepoPath, verbosity=verbosity)
                 if res["code"] == 0:
-                    revNum = getRevNumber(hash, absRepoPath)
-                    printWithVars2("{greenRepoString}: successfully checked out revision by {method}: {shortHash} (revision number {revNum})")
+                    revNum = getRevNumber(absRepoPath)
+                    printWithVars2(f"\r{_green(repoString)}: successfully checked out revision by {method}: {shortHash} (revision number {revNum})")
                     found = True
                     break
-                printWithVars3("{repoString}: failed to check out revision by {method}: {hash}")
+                printWithVars3(f"\r{repoString}: failed to check out revision by {method}: {hash}")
 
             if (method == "UnixTimeStamp") and ("UnixTimeStamp" in repoInfo):
                 if (matching == 'timestamp') or (matching == 'closetimestamp'):
                     ts = repoInfo["UnixTimeStamp"]
-                    date = dateFromTimeStamp(ts)
+                    date = dateFromTimestamp(ts)
                     if dryrun:
-                        printWithVars2("{repoString}: would try and check out revision by {method}: {ts} ({date})", dryrun=False)
+                        printWithVars2(f"{repoString}: would try and check out revision by {method}: {ts} ({date})", dryrun=False)
                         break
+                    
                     res = gitCommand("git log --all --format=format:'\"%at\" : \"%H\",'", 4, cwd=absRepoPath, raiseOnFailure=True, verbosity=verbosity, permitShowingStdOut=False, permitShowingStdErr=False)
                     shaHash = 0
                     if res["code"] == 0:
                         timestampsToShas = json.loads('{'+res["stdout"][0:-1]+'}')
                         if (ts in timestampsToShas):
                             if (matching == 'timestamp') or (matching == 'closetimestamp'):
                                 hash = timestampsToShas[ts]
                                 branch=defaultSyncPointBranchName
-                                res = gitCommand("git checkout -B {branch} {hash}", 3, cwd=absRepoPath, verbosity=verbosity)
+                                print(f"\r>> checking out {ts} ({date})...", end='', flush=True)
+                                res = gitCommand(f"git checkout -B {branch} {hash}", 3, cwd=absRepoPath, verbosity=verbosity)
                                 if res["code"] == 0:
-                                    revNum = getRevNumber(hash, absRepoPath)
-                                    printWithVars2("{greenRepoString}: successfully checked out revision by {method}: {ts} ({date}) {hash} (revision number {revNum})")
+                                    revNum = getRevNumber(absRepoPath)
+                                    printWithVars2(f"{_green(repoString)}: successfully checked out revision by {method}: {ts} ({date}) {hash} (revision number {revNum})")
                                     found = True
                                     break
                         else:
                             if matching == 'closetimestamp':
                                 closestTimestamp = min(timestampsToShas, key=lambda x:abs(int(x)-int(ts)))
-                                closestDate = dateFromTimeStamp(closestTimestamp)
+                                closestDate = dateFromTimestamp(closestTimestamp)
                                 hash = timestampsToShas[closestTimestamp]
                                 branch=defaultSyncPointBranchName
+                                print(f"\r>> checking out close {ts} ({date})...", end='', flush=True)
                                 res = gitCommand("git checkout -B {branch} {hash}", 3, cwd=absRepoPath, verbosity=verbosity)
                                 if res["code"] == 0:
-                                    revNum = getRevNumber(hash, absRepoPath)
-                                    printWithVars2("{yellowRepoString}: warning checking out revision by closest timestamp.", "red")
-                                    printWithVars2("       requested {method}: {ts} ({date})")
-                                    printWithVars2("       used      {method}: {closestTimestamp} ({closestDate}) {hash} (revision number {revNum})")
+                                    revNum = getRevNumber(absRepoPath)
+                                    printWithVars2(f"\r{_yellow(repoString)}: warning checking out revision by closest timestamp.", "red")
+                                    printWithVars2(f"       requested {method}: {ts} ({date})")
+                                    printWithVars2(f"       used      {method}: {closestTimestamp} ({closestDate}) {hash} (revision number {revNum})")
                                     found = True
                                     break
 
-                    printWithVars3("{repoString}: failed to check out revision by {method}: {ts} {date}")
+                    printWithVars3(f"\r{repoString}: failed to check out revision by {method}: {ts} {date}")
 
         if not found and not dryrun:
             allFound = False
-            printWithVars2("{redRepoString}: failed to check out specified revision by any method.")
+            printWithVars2(f"{_red(repoString)}: failed to check out specified revision by any method.")
     if dryrun:
         pass
     elif allFound:
         print(colored("success! all repos checked out to the specified sync state.", 'green'))
     else:
         print(colored("failure! not all repos checked out to the specified sync state.", 'red'))
         sys.exit(1)
 
 
 
 # --------------------------------------------------------------------------------------------------------------------------
-# command "recordRepos"
+# command "record_repos"
 # --------------------------------------------------------------------------------------------------------------------------
 
 def commandRecordRepos():
     checkForSyncRepo(syncFilePath)
     syncDict = loadSyncFileAsDict(syncFilePath)
     newSyncDict = OrderedDict(syncDict)
     anyFailures = False
     for repoName in syncDict:
         repoInfo = syncDict[repoName]
         absRepoPath = getAbsRepoPath(repoInfo["path"], cwd)
         repoString = paddedRepoName(repoName, list(syncDict.keys()))
-        greenRepoString = colored(repoString, 'green')
-        redRepoString   = colored(repoString, 'red')
         if not checkForRepo(repoString, absRepoPath):
             anyFailures = True
             continue
         (worked, newRepoInfo) = dictFromCurrentRepoState(repoInfo["path"], cwd=cwd, verbosity=verbosity, dryrun=False)
         if worked:
             shortHash = newRepoInfo["sha"][0:12]
             date = newRepoInfo["date"]
-            printWithVars2("{greenRepoString}: recording bank sync state of {shortHash}, {date}.")
+            printWithVars2(f"{_green(repoString)}: recording bank sync state of {shortHash}, {date}.")
         else:
-            printWithVars2("{redRepoString}: failure! not able to get the status of {repoName} at {absRepoPath}", 'red')
+            printWithVars2(f"{_red(repoString)}: failure! not able to get the status of {repoName} at {absRepoPath}", 'red')
             anyFailures = True
         newSyncDict[repoName] = newRepoInfo
     
     if dryrun:
         sys.exit(0)
     
     writeDictToSyncFile(syncFilePath, newSyncDict)
 
     if anyFailures:
-        printWithVars1("failure! not all constituent repos had their state recorded.", 'red')
+        printWithVars1(f"failure! not all constituent repos had their state recorded.", 'red')
         sys.exit(1)
     else:
-        printWithVars1("success! all constituent repos had their state recorded.", 'green')
+        printWithVars1(f"success! all constituent repos had their state recorded.", 'green')
 
 
 
 # --------------------------------------------------------------------------------------------------------------------------
-# command "createSyncfile"
+# command "create_syncfile"
 # --------------------------------------------------------------------------------------------------------------------------
 
-def commandCreateSyncfile(repoNames):
+def commandCreateSyncfile():
+    repoNames = _config['args.repos']
     checkForSyncRepoDir(syncRepoPath, existing = False)
     newSyncDict = OrderedDict()
     anyFailures = False
     for repo in repoNames:
         absRepoPath = getAbsRepoPath(repo, cwd)
         repoName = os.path.basename(absRepoPath)
         repoString = paddedRepoName(repoName, repoNames)
-        greenRepoString = colored(repoString, 'green')
         if not checkForRepo(repoName, absRepoPath):
             anyFailures = True
             continue
         (worked, newRepoInfo) = dictFromCurrentRepoState(repo, cwd=cwd, verbosity=verbosity, dryrun=False)
         if worked:
             shortHash = newRepoInfo["sha"][0:12]
             date = newRepoInfo["date"]
-            printWithVars2("{greenRepoString}: recording repository state of {shortHash}, {date}.")
+            printWithVars2(f"{_green(repoString)}: recording repository state of {shortHash}, {date}.")
         else:
-            printWithVars2("failure! not able to get the status of {repoName} at {absRepoPath}", 'red')
+            printWithVars2(f"failure! not able to get the status of {repoName} at {absRepoPath}", 'red')
             anyFailures = True
         newSyncDict[repoName] = newRepoInfo
 
     if dryrun:
         sys.exit(0)
 
     writeDictToSyncFile(syncFilePath, newSyncDict)
 
     if anyFailures:
-        printWithVars1("failure! not all constituent repos had their state recorded.", 'red')
+        printWithVars1(f"failure! not all constituent repos had their state recorded.", 'red')
         sys.exit(1)
     else:
-        printWithVars1("success! all constituent repos had their state recorded.", 'green')
+        printWithVars1(f"success! all constituent repos had their state recorded.", 'green')
 
 
 
 # --------------------------------------------------------------------------------------------------------------------------
-# command "createSyncrepo"
+# command "create_syncrepo"
 # --------------------------------------------------------------------------------------------------------------------------
 
-def commandCreateSyncrepo(repoNames):
+def commandCreateSyncrepo():
     global syncFilePath
-    syncfilename = resolvedOpts['createSyncrepo']['syncfilename']
-    syncreponame = resolvedOpts['createSyncrepo']['syncreponame']
+    global syncRepoPath
+    syncfilename = _config['create_syncrepo.syncfilename']
+    syncreponame = _config['create_syncrepo.syncreponame']
     syncRepoPath = os.path.abspath(syncreponame)
     syncFilePath = os.path.join(syncRepoPath, syncfilename)
     configFilePath = os.path.join(syncRepoPath, 'bankconfig.ini')
 
     if os.path.isdir(syncRepoPath):
-        printWithVars1("failure! The directory {syncRepoPath} already exists.", 'red')
+        printWithVars1(f"failure! The directory {syncRepoPath} already exists.", 'red')
         sys.exit(1)
 
     if dryrun:
-        printWithVars1("The directory {syncRepoPath} would be created and a git repository would be initilized there. The file {configFilePath} and {syncFilePath} would be created and filled.")
+        printWithVars1(f"The directory {syncRepoPath} would be created and a git repository would be initilized there. The file {configFilePath} and {syncFilePath} would be created and filled.")
         sys.exit(0)
 
     os.makedirs(syncRepoPath)
     with open(configFilePath, 'w') as f:
-        f.write(stringWithVars("[General]\ncwd=..\nsyncFile={syncfilename}"))
+        f.write(f"[general]\ncwd=..\nsyncFile={syncfilename}")
     execute2("git init", cwd=syncRepoPath)
 
-    commandCreateSyncfile(repoNames)
+    commandCreateSyncfile()
 
 
 
 # --------------------------------------------------------------------------------------------------------------------------
 # command "bisect"
 # --------------------------------------------------------------------------------------------------------------------------
 
-def commandBisect(command):
+def commandBisect():
+    command = _config['args.bisectcmd']
+    remainingArgs = _config['remaining_args']
     checkForSyncRepo(syncFilePath)
     syncDict = loadSyncFileAsDict(syncFilePath)
     currentRev = getCurrentRevHash(syncRepoPath)
     anyFailures = False
 
     if dryrun:
-        printWithVars2("would try exectue the given bisect command on the current sync repo and sync the bank repos to the new state.")
+        printWithVars2(f"would try exectue the given bisect command on the current sync repo and sync the bank repos to the new state.")
         sys.exit(0)
 
     if command == 'start':
         restoreDict = OrderedDict()
         for repoName in syncDict:
             repoInfo = syncDict[repoName]
             absRepoPath = getAbsRepoPath(repoInfo["path"], cwd)
             repoString = paddedRepoName(repoName, list(syncDict.keys()))
-            greenRepoString = colored(repoString, 'green')
-            redRepoString   = colored(repoString, 'red')
             try:
                 rev = getCurrentBranchOrHash(absRepoPath)
                 restoreDict[absRepoPath] = rev
-                printWithVars2("{greenRepoString}: recording repository state of '{rev}' before starting bisect")
+                printWithVars2(f"{_green(repoString)}: recording repository state of '{rev}' before starting bisect")
             except:
                 anyFailures = True
-                printWithVars2("{redRepoString}: error recoding original branch in {absRepoPath}")
+                printWithVars2(f"{_red(repoString)}: error recoding original branch in {absRepoPath}")
                 continue
         writeBisectRestoreToJson(syncRepoPath, restoreDict)
         if anyFailures:
             print(colored("failure! not all repo states recorded before bisect.", 'red'))
 
     bisectCmd = "git bisect " + command + " " + " ".join(remainingArgs)
     res = gitCommand(bisectCmd, 2, cwd=syncRepoPath, verbosity=verbosity);
@@ -562,93 +610,185 @@
 
     if command == 'reset':
         restoreDict = loadBisectRestoreFromJson(syncRepoPath)
         for repoName in syncDict:
             repoInfo = syncDict[repoName]
             absRepoPath = getAbsRepoPath(repoInfo["path"], cwd)
             repoString = paddedRepoName(repoName, list(syncDict.keys()))
-            greenRepoString = colored(repoString, 'green')
-            redRepoString   = colored(repoString, 'red')
             try:
                 rev = restoreDict[absRepoPath] if (absRepoPath in restoreDict) else None
                 if not rev:
                     raise Exception("Restore changesete not found")
                 res = gitCommand("git checkout {rev}", 3, cwd=absRepoPath, verbosity=verbosity)
-                printWithVars2("{greenRepoString}: restoring repository state to '{rev}' after finishing bisect")
+                printWithVars2(f"{_green(repoString)}: restoring repository state to '{rev}' after finishing bisect")
             except:
                 anyFailures = True
-                printWithVars2("{redRepoString}: error restoring original branch in {absRepoPath}")
+                printWithVars2(f"{_red(repoString)}: error restoring original branch in {absRepoPath}")
                 continue
         if anyFailures:
             print(colored("failure! not all repo states restored after bisect.", 'red'))
         removeBisectRestoreFile(syncRepoPath)
 
 
 
 # --------------------------------------------------------------------------------------------------------------------------
 # command "clone"
 # --------------------------------------------------------------------------------------------------------------------------
 
 def commandClone():
+    global syncFilePath, syncRepoPath, cwd
+    cloneURL = _config['args.url']
+    if not isValidGitUrl(cloneURL):
+        print(colored("failure! {cloneURL} appears not to be a URL that works with git clone.", 'red'))
+        sys.exit(1)
+    destName = _config['args.name']
+    destName = destName if (destName is not None) else getRepoNameFromUrl(cloneURL)
+    absDestNamePath = getAbsRepoPath(destName, cwd)
+
+    execute3("mkdir -p {absDestNamePath}")
+    opts = {'captureStdOutStdErr':False, 'verbosity':verbosity, 'cwd': os.path.dirname(absDestNamePath)}
+    print(f"\r>> cloning {cloneURL}...", end='', flush=True)
+    res = gitCommand("git clone {cloneURL} {destName}", 3, **opts)
+    if res['code'] != 0:
+        anyFailures = True
+        printWithVars2(f"\r{_red(cloneURL)}: error cloning repo to {absDestNamePath}: {res['stderr']}")
+        sys.exit(1)
+
+    printWithVars2(f"\r{_green(cloneURL)}: cloned repo to {absDestNamePath}")
+
+    syncRepoPath = os.path.join(absDestNamePath, 'syncrepo')
+
+    # If we have just cloned a sync repo (the typical case) then move the contents into the sync repo directory
+    if getSyncFileInDir(absDestNamePath):
+        moveDirectory(absDestNamePath, syncRepoPath)
+
+    syncFilePath = getSyncFileInDir(syncRepoPath)
+    if not syncFilePath:
+            anyFailures = True
+            printWithVars2(f"{_red('failure!') }: no syncfile found at {absDestNamePath} or {syncRepoPath}")
+            sys.exit(1)
+    
+    cwd = absDestNamePath
+    commandPopulate()
+
+
+
+# --------------------------------------------------------------------------------------------------------------------------
+# command "populate"
+# --------------------------------------------------------------------------------------------------------------------------
+
+def commandPopulate():
     checkForSyncRepo(syncFilePath)
     syncDict = loadSyncFileAsDict(syncFilePath)
     anyFailures = False
 
     opts = {'captureStdOutStdErr':False, 'verbosity':verbosity}
     for repoName in syncDict:
         repoInfo = syncDict[repoName]
         absRepoPath = getAbsRepoPath(repoInfo["path"], cwd)
         repoString = paddedRepoName(repoName, list(syncDict.keys()))
-        greenRepoString = colored(repoString, 'green')
-        redRepoString   = colored(repoString, 'red')
         if not "cloneURL" in repoInfo:
             anyFailures = True
-            printWithVars2("{repoString}: there is no cloneURL for this repo", "red")
+            printWithVars2(f"{repoString}: there is no cloneURL for this repo", "red")
             continue   
         cloneURL = repoInfo["cloneURL"]
         name = os.path.basename(absRepoPath)
         dir  = os.path.dirname(absRepoPath)
         if dryrun:
-            printWithVars2("{repoString}: would clone {cloneURL} to {absRepoPath}.", dryrun=False)
+            printWithVars2(f"{repoString}: would clone {cloneURL} to {absRepoPath}.", dryrun=False)
             continue
 
         opts['cwd'] = dir
         execute3("mkdir -p {dir}")
+        print(f"\r>> cloning {name}...", end='', flush=True)
         res = gitCommand("git clone {cloneURL} {name}", 3, **opts)
         if res['code'] == 0:
-            printWithVars2("{greenRepoString}: cloned repo to {absRepoPath}")
+            printWithVars2(f"\r{_green(repoString)}: cloned repo to {absRepoPath}")
         else:
             anyFailures = True
-            printWithVars2("{redRepoString}: error cloning repo to {absRepoPath}")
+            printWithVars2(f"\r{_red(repoString)}: error cloning repo to {absRepoPath}")
 
     if dryrun:
         sys.exit(0)
     if anyFailures:
-        print(colored("failure! not all repos cloned.", 'red'))
+        print(colored("failure! not all repos populated.", 'red'))
         sys.exit(1)
 
-    print(colored("success! all repos cloned.", 'green'))
+    print(colored("success! all repos populated.", 'green'))
     commandSync()
 
 
+# --------------------------------------------------------------------------------------------------------------------------
+# command "status"
+# --------------------------------------------------------------------------------------------------------------------------
+
+def commandStatus():
+    checkForSyncRepo(syncFilePath)
+    syncDict = loadSyncFileAsDict(syncFilePath)
+    anyFailures = False
+
+    for repoName in syncDict:
+        repoInfo = syncDict[repoName]
+        absRepoPath = getAbsRepoPath(repoInfo["path"], cwd)
+        repoString = paddedRepoName(repoName, list(syncDict.keys()))
+        if dryrun:
+            printWithVars2(f"{repoString} : would give the status of the repo at {absRepoPath}.", dryrun=False)
+            continue
+
+        if not checkForRepo(repoString, absRepoPath):
+            allFound = False
+            anyFailures = True
+            continue
+
+        modifiedCount = getModifiedCount(absRepoPath)
+        stagedCount = getStagedCount(absRepoPath)
+        branchName = getBranchName(absRepoPath)
+        
+        # This is actually dimmed not grey since grey appears like black text for me
+        def greyText(txt):
+            return '\033[2m'+txt+"\033[00m"
+
+        description = f"{greyText('branch')}: {colored(branchName,'blue')}".strip()
+        description = description.strip()
+        
+        if modifiedCount > 0:
+            description = f"{description}, {greyText('modified')}: {modifiedCount}".strip()
+        if stagedCount > 0:
+            description = f"{description}, {greyText('staged')}: {stagedCount}".strip()
+        print(f"{_green(repoString)} : {description}")
+
+    if dryrun:
+        sys.exit(0)
+    if anyFailures:
+        print(colored("failure! not all repos reported the status correctly.", 'red'))
+        sys.exit(1)
+
+    print(colored("success! all repos status reported.", 'green'))
+
+
+
 
 # --------------------------------------------------------------------------------------------------------------------------
 # a git command
 # --------------------------------------------------------------------------------------------------------------------------
 
-def distributeGitCommand(command, includeSyncRepo=False, *remainingArgs):
+def distributeGitCommand():
+
+    command = _config['args.gitcmd']
+    includeSyncRepo = (_config['args.command'] == 'gitall')
+    remainingArgs = _config['remaining_args']
+
     if not command in approved_git_commands:
-        yellowWarning = colored("warning", 'yellow')
-        printWithVars1("{yellowWarning}: the git command `{command}` might not make sense being applied non-interactively to each repo in the bank. Use at your own discretion.")
+        printWithVars1(f"{_yellow('warning')}: the git command `{command}` might not make sense being applied non-interactively to each repo in the bank. Use at your own discretion.")
     if not command in allGitCommands:
-        printWithVars1("failure! unknown git command `{command}`", 'red')
+        printWithVars1(f"failure! unknown git command `{command}`", 'red')
 
     gitCmd = "git " + command + " " + " ".join(remainingArgs)
     gitCmd = gitCmd.strip()
-    gitRepoSeperatorString = (resolvedOpts['General']['seperator']*40)[0:40]
+    gitRepoSeperatorString = (_config['general.seperator']*40)[0:40]
     checkForSyncRepoDir(syncRepoPath)
     syncDict = loadSyncFileAsDict(syncFilePath)
     anyFailures = False
     opts = {'captureStdOutStdErr':False, 'verbosity':verbosity}
     printWithVars2(gitRepoSeperatorString, dryrun=False)
     for repoName in syncDict:
         repoInfo = syncDict[repoName]
@@ -661,105 +801,110 @@
         printWithVars2(gitRepoSeperatorString, dryrun=False)
     if includeSyncRepo:
         opts['cwd'] = syncRepoPath
         gitCommand(gitCmd, 2, **opts);
         printWithVars2(gitRepoSeperatorString, dryrun=False)
 
     if anyFailures:
-        printWithVars1("failure! not all constituent repos present.", 'red')
+        printWithVars1(f"failure! not all constituent repos present.", 'red')
         sys.exit(1)
     else:
-        printWithVars1("all constituent repos issued git command '{gitCmd}'", 'green')
+        printWithVars1(f"all constituent repos issued git command '{gitCmd}'", 'green')
 
 
 
 # --------------------------------------------------------------------------------------------------------------------------
 # dispatch command
 # --------------------------------------------------------------------------------------------------------------------------
 
-def dispatchCommand(command):
-    if command == "sync":
-        commandSync()
-    if command == "clone":
-        commandClone()
-    if command == "recordRepos":
-        commandRecordRepos()
-    if command == "createSyncfile":
-        commandCreateSyncfile(args.repos)
-    if command == "createSyncrepo":
-        commandCreateSyncrepo(args.repos)
-    if command == "bisect":
-        commandBisect(args.bisectcmd)
-    if command == "git":
-        distributeGitCommand(args.gitcmd, False, *remainingArgs)
-    if command == "gitall":
-        distributeGitCommand(args.gitcmd, True, *remainingArgs)
+def dispatchCommand():
+    command_map = {
+        "sync": commandSync,
+        "clone": commandClone,
+        "populate": commandPopulate,
+        "status": commandStatus,
+        "record_repos": commandRecordRepos,
+        "create_syncfile": commandCreateSyncfile,
+        "create_syncrepo": commandCreateSyncrepo,
+        "bisect": commandBisect,
+        "git": distributeGitCommand,
+        "gitall": distributeGitCommand,
+    }
 
+    command = _config['args.command']
+    if command in command_map:
+        command_map[command]()
+    else:
+        printWithVars1(f"failure! unkown command {command}.", 'red')
+        sys.exit(1)
 
 
 # --------------------------------------------------------------------------------------------------------------------------
 # Extract and clean the argument parameters
 # --------------------------------------------------------------------------------------------------------------------------
 
 def getResolvedOptions(args):
     
-    bankOptions = dict(defaultOptions)
+    bankOptions = flattenDict(dict(defaultOptions))
     if os.path.isfile('~/.bankconfigrc'):
-        newOptions = getOptionDictFromIniFile('~/.bankconfigrc')
+        newOptions = flattenDict(getOptionDictFromIniFile('~/.bankconfigrc'))
         bankOptions = mergeOptionDicts(bankOptions, newOptions)
 
     # Get the config file path
     if getattr(args, 'cwd', 'auto') != 'auto':
         configFile = os.path.abspath(os.path.join(args.cwd, 'bankconfig.ini'))
     else:
         configFile = os.path.abspath('bankconfig.ini')    
     if os.path.isfile(configFile):
-        newOptions = getOptionDictFromIniFile(configFile)
+        newOptions = flattenDict(getOptionDictFromIniFile(configFile))
         bankOptions = mergeOptionDicts(bankOptions, newOptions)
 
     passedInOptions = {
-        'General' : {
+        'general' : {
             'cwd' : getattr(args, 'cwd', 'auto'),
             'syncfile' : getattr(args, 'syncfile', 'auto'),
             'verbosity' : getattr(args, 'verbosity', autoNum),
             'colorize' :  getattr(args, 'colorize', 'auto'),
             'seperator' : getattr(args, 'seperator', 'auto'),
         },
         'sync' : {
             'matching' : getattr(args, 'matching', 'auto')
         },
-        'createSyncrepo' : {
+        'create_syncrepo' : {
             'syncfilename' : getattr(args, 'syncfilename', 'auto'),
             'syncreponame' : getattr(args, 'syncreponame', 'auto')
         }
     }
     
-    bankOptions = mergeOptionDicts(bankOptions, passedInOptions)
+    bankOptions = mergeOptionDicts(bankOptions, flattenDict(passedInOptions))
     
     # normalize non-string options
-    bankOptions['General']['verbosity'] = int(bankOptions['General']['verbosity'])
-    bankOptions['General']['colorize'] = True if (bankOptions['General']['colorize'].lower() in ['yes','true']) else False
+    bankOptions['general.verbosity'] = int(bankOptions['general.verbosity'])
+    bankOptions['general.colorize'] = True if (bankOptions['general.colorize'].lower() in ['yes','true']) else False
 
     return bankOptions
 
 
 def main():
-    global args, remainingArgs, syncFilePath, syncRepoPath, cwd, verbosity, dryrun, resolvedOpts
-    args, remainingArgs = parseArguments()
+    global syncFilePath, syncRepoPath, cwd, verbosity, dryrun, _config
+    args, remaining_args = parseArguments()
 
-    command = args.subparser_name
-    resolvedOpts = getResolvedOptions(args)
-    cwd = resolvedOpts['General']['cwd']
-    verbosity = resolvedOpts['General']['verbosity']
-    colorize = resolvedOpts['General']['colorize']
-    syncFilePath = resolvedOpts['General']['syncfile']
+    _config = getResolvedOptions(args)
+    _config['args'] = vars(args)
+    _config['remaining_args'] = remaining_args
+    _config = flattenDict(_config)
+
+    cwd = _config['general.cwd']
+    verbosity = _config['general.verbosity']
+    colorize = _config['general.colorize']
+    syncFilePath = _config['general.syncfile']
     syncRepoPath = os.path.dirname(os.path.abspath(syncFilePath))
-    dryrun = args.dryrun
+    dryrun = _config['args.dryrun']
     set_execute_defaults('verbosity', verbosity)
     set_execute_defaults('dryrun', dryrun)
     set_execute_defaults('colorize', colorize)
     
-    dispatchCommand(command)
+    dispatchCommand()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `banksync-0.9.4/banksync.egg-info/PKG-INFO` & `banksync-0.9.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,321 +1,317 @@
-Metadata-Version: 2.1
-Name: banksync
-Version: 0.9.4
-Summary: A library for manipulating banks of git repositories
-Home-page: https://github.com/jasonfharris/banksync
-Author: Jason Harris
-Author-email: jason@jasonfharris.com
-License: MIT
-Download-URL: https://github.com/jasonfharris/banksync/tarball/0.9.4
-Description: ## Purpose
-        
-        The banksync command line tool allows the easy operation of git commands across a "bank" or "collection" or repositories. It allows synchronization to historic configurations across the bank of repos.
-        
-        ## Installation
-        
-        You can install `banksync` from PyPi with a simple:
-        
-        ```
-        pip install banksync
-        ```
-        
-        ## Quickstart
-        
-        A bank is a collection of repos. The collection of repos is specified in a *syncfile*. The syncfile typically lives in *syncrepo*. So let us demonstrate this with a trivial collection of repos. The overall project will be called `animals` and it will contain a repo `repoFish` and a repo `repoBirds`. The project can live anywhere but to make the description easy let us put the project in the users root directory.
-        
-        So make a directory `animals`:
-        
-            cd ~
-            mkdir animals
-            cd animals
-        
-        Now clone the demonstration syncrepo for the animals project using standard git:
-        
-            git clone https://github.com/testbank/animalsRepoSync.git
-        
-        This will clone the thin repo which records the syncfile over time. Ie it records the state of the repos in the bank at different times / stages. We now have the hierarchy:
-        
-            animals
-            └── animalsRepoSync
-                ├── bankconfig.ini
-                └── syncfile.wl
-        
-        Now we enter into this directory and we clone the repositories in the bank
-        
-            cd animalsRepoSync
-            bank clone
-        
-        The clone command will clone all of the repos specified in the syncfile and we will now have the following layout:
-        
-            animals
-            ├── animalsRepoSync
-            │   ├── bankconfig.ini
-            │   └── syncfile.wl
-            ├── repoBird
-            │   └── Bird.txt
-            └── repoFish
-                └── Fish.txt
-        
-        We can now issue commands across the repos in the bank. From the syncrepo we can execute:
-        
-            cd ~/animals/animalsRepoSync
-            bank git status
-        
-        Which will execute the status command in each of the repos in the bank. If we want to checkout a previous state across the repos in the project we can do this via (from the syncrepo):
-        
-            git checkout master~2
-            bank sync
-        
-        The last two commands just moved the syncrepo two revisions back, and then synchronized the repos in the bank to the sync file at this earlier time. To get all repos back to the master branch revisions you can simply execute:
-        
-            bank gitall checkout master
-        
-        Which will do a `git checkout master` on all the repos in the bank including the sync repo.
-        
-        ## Syncfile
-        
-        The syncfile specifies which repositories are part of the bank, and what state the repositories should be synchronized to. A typical simple sync file might be the following
-        
-            more ~/animals/animalsRepoSync/syncfile.wl
-        
-        Which yields:
-        
-        ```
-        <|
-            "repoFish" -> <|
-                "path" -> "repoFish",
-                "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
-                "UnixTimeStamp" -> "1480517200",
-                "date" -> "30 Nov 2016 - 15:46:40",
-                "author" -> "Jason Harris",
-                "revisionNumber" -> "3",
-                "message" -> "committing salmon",
-                "cloneURL" -> "https://github.com/testbank/repoFish.git"
-            |>,
-            "repoBird" -> <|
-                "path" -> "repoBird",
-                "sha" -> "6bf9d646b2aa224b64fb86cbddb4d7ab0f2e37d3",
-                "UnixTimeStamp" -> "1480517200",
-                "date" -> "30 Nov 2016 - 15:46:40",
-                "author" -> "Jason Harris",
-                "revisionNumber" -> "3",
-                "message" -> "committing eagle",
-                "cloneURL" -> "https://github.com/testbank/repoBird.git"
-            |>
-        |>
-        ```
-        
-        The syncfile should lie inside a git repo (the syncrepo). Whenever we want to record a configuration of the repos we simply alter the syncfile by transcribing the current state of the repos into the syncfile using `bank recordRepos` with the appropriate options. We then use `git commit` to record this new state / configuration in the syncrepo.
-        
-        So let us add some content to repoBird in our example and then commit this change.
-        
-            cd  ~/animals/repoBird
-            echo "toucan" >> Bird.txt
-            git commit -am "committing toucan"
-        
-        So now we can update the syncfile with the state of the current repos in the bank:
-        
-            cd ~/animals/animalsRepoSync/
-            bank recordRepos
-        
-        The contents of our syncfile will now be something like:
-        
-        ```
-        <|
-            "repoFish" -> <|
-                "path" -> "repoFish",
-                "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
-                "UnixTimeStamp" -> "1480517200",
-                "date" -> "30 Nov 2016 - 15:46:40",
-                "author" -> "Jason Harris",
-                "revisionNumber" -> "3",
-                "message" -> "committing salmon",
-                "cloneURL" -> "https://github.com/testbank/repoFish.git"
-            |>,
-            "repoBird" -> <|
-                "path" -> "repoBird",
-                "sha" -> "c8fb05947c5161e484104d99f427ec082fb4e85b",
-                "UnixTimeStamp" -> "1480519159",
-                "date" -> "30 Nov 2016 - 16:19:19",
-                "author" -> "Jason Harris",
-                "revisionNumber" -> "4",
-                "message" -> "committing toucan",
-                "cloneURL" -> "https://github.com/testbank/repoBird.git"
-            |>
-        |>
-        ```
-        
-        (Note the sha, timestamps, and other data about the state of the repo `repoBird` has changed.)
-        
-        So we could now record this new overall state of the repos in the bank via simply committing the file syncfile in the syncrepo.
-        
-            git commit -am "recording the latest state of the repos in animals."
-        
-        ## Locations
-        
-        How does the bank command know where to put the `repoBird` and `repoFish`? How does it know which syncfile to use, etc. Well in the syncrepo there is the file `bankconfig.ini`. This is a standard preferences file but in this example it has two important options: `cwd=..` and `syncfile=syncfile.wl`.
-        
-        The cwd (ChangeWorkingDirectory) option specifies that the repo commands should be executed one level up from our current working directory. So since we are currently at `~/animals/animalsRepoSync` that means that the repos paths will start from `~/animals/`
-        
-        The second option just tells us what the name of the syncfile is. We could have called it `earthanimals.wl` if we wanted to.
-        
-        ## Bank command line options
-        
-        The command line tool `bank` has several options which can be specified:
-        
-        #### --syncfile <path>
-        
-        The `syncfile` option specifies a syncfile. The syncfile contents specify which repos are part of the bank. The various keys which are recorded if present are:`path`, `sha`, `UnixTimeStamp`, `date`, `author`, `revisionNumber`, `message`, and `cloneURL`. Adding other keys at present will not effect or change the behavior of the bank tool so you can add other info as you see fit / want to each of the recorded states in the various repos.
-        
-        #### --cwd <path>
-        
-        The cwd option will change the working directory. Using this you can specify the relative path to get to the base of where the path for each of the repos in the bank are. For instance in the layout example of the animals project above, if we are in the directory `animals/animalsSyncRepo` then since the path in the syncfile for "Birds" is just `repoBird` then relative to `animals/animalsSyncRepo` we want the directory `../repoBird`. So we would use the option `--cwd ..`
-        
-        #### --dryrun
-        
-        If this option is specified then `banksync` will report what it *would* do but it doesn't actually do anything.
-        
-        #### --colorize <bool>
-        
-        You can specify if color is not to be used in output if for instance you want the logs to be parsed in jenkins or other devops tools. (The default is `True`, i.e. colorize the output of the bank command)
-        
-        #### --verbosity <num>
-        
-        You can specify how much information banksync reports. This integer should be between 0, 1, 2, 3, or 4. The higher the number the more verbose is the reporting. The default is 2.
-        
-        #### --matching <type>
-        
-        When attempting to sync the constituent repos to the versions specified in the syncfile, how do we determine what to set the versions to? We want some loose coupling in that for instance if someone runs filter branch on a project or they do some rebase very early on in the history then the shas will change on all the revisions in the repository. So instead of finding a commit via a sha we will have to fall back to looking for a matching timestamp for the revision. These are generally fairly unique in a project unless a lot of cherrypicking has gone on. If we don't find that exact timestamp then we could fall back to the closest matching revision to that timestamp. In this way at least we have some hope of getting close to the configuration at the time instead of just giving up. Ie we get to the exact configuration if it is available but if not get as close as we can. The value of the option can be:
-        
-        - **shaOnly**: if we can't find the exact same revision given by the sha in the syncfile than give up.
-        - **timestamps**: try matching by sha first but if that fails find the first revision with the same unix timestamp. (This is almost always preserved across repo manipulation)
-        - **closetimestamps**: try matching by sha first, if that fails try matching by timestamp. and if that fails find the revision with the closest timestamp and match to that.
-        
-        ## Config file
-        
-        Instead of specifying the `--syncfile` and`—cwd` in each command you can create a `bankconfig.ini` file alongside the syncfile. In the `bankconfig.ini` file you can specify the default syncfile and cwd to use if none is specified. Eg we could add the file `animals/animalsSyncRepo/bankconfig.ini` with the following contents:
-        
-        ```
-        [General]
-        cwd=..
-        syncFile=syncfile.wl
-        ```
-        
-        Then you could omit the options to the bank command and they would be taken from the bankconfig.ini file so the above example would become:
-        
-        ```
-        cd animals/animalsSyncRepo
-        bank recordRepos
-        git commit -am "recording the latest state of the repos in animals."
-        ```
-        
-        You can choose weather to include the `bankconfig.ini` in the syncrepo history or not. (We choose to in this example but other teams may leave this to the individual developers.)
-        
-        ## Commands
-        
-        The form of a bank command is `bank <cmd> <opts>` where `<cmd>` is one of `sync`, `recordRepos`, `createSyncfile`, `bisect`, `clone`,  `git` or `gitall` 
-        
-        #### bank sync <opts>
-        
-        `sync` will update / checkout the revisions specified in the syncfile for each of the repos specified in the bank.
-        
-        ```
-        bank sync --syncfile syncfile.wl
-        ```
-        
-        This would checkout / update the repos given in the syncfile `syncfile.wl` to the states given in the syncfile. It each repo it tries to checkout the version first by the given sha, and then it falls back to the given timestamp, and then it falls back to the closest timestamp. (This fallback behavior can be controlled by the `--matching` option.)
-        
-        ```
-        bank sync --syncfile syncfile.wl --cwd ../other/dir
-        ```
-        
-        This would checkout / update the repos given in the syncfile to the states given in the syncfile
-        (but the path to each repo in the bank will be prefixed by the value of the `--cwd` option `../other/dir`).
-        
-        #### bank recordRepos <opts>
-        
-        `recordRepos` is used to transcribe the current state of the repos into the syncfile. Eg:
-        
-        ```
-        bank recordRepos --syncfile syncfile.wl
-        ```
-        
-        This would alter the contents of the syncfile and change the revisions stored in the syncfile.wl to match the current revisions of the referenced repositories.
-        
-        #### bank createSyncfile <opts>
-        
-        `createSyncfile` is used to generate an initial syncfile. Eg:
-        
-        ```
-        bank createSyncfile --syncfile syncfile.wl repo1 repo2 ... repoN --cwd some/dir
-        ```
-        
-        This would generate or overwrite the syncfile.wl to contain sync points for the current states of `repo1`, `repo2`, ... `repoN`
-        
-        #### bank createSyncrepo <opts>
-        
-        `createSyncrepo` is used to generate the syncrepo directory, initialize a git repository there, create the syncfile and also create the bankconfig.ini file. Basically it creates all the working parts of a syncrepo. Eg:
-        
-        ```
-        bank createSyncrepo repo1 repo2 ... repoN
-        ```
-        
-        This would create the directory `syncrepo` and fill it with a `syncfile.json` and a `bankconfig.ini`. The syncfile would contain the latest states of the `repo1`, `repo2`, ... `repoN`. 
-        
-        ```
-        bank createSyncrepo --syncreponame controlrepo --syncfilename felipe.json repo1 repo2 ... repoN
-        ```
-        Would create and initialize a syncrepo called `controlrepo` and inside that a syncfile called `felipe.json`.
-        
-        #### bank bisect <opts>
-        
-        You can use `bank bisect` on the syncrepo to step through historic configurations looking for a configuration which produces some change. (Typically we are searching for a regression.) Eg if we have a configuration file in the syncrepo the following might be a typical bisect session:
-        
-            cd SomeSyncRepo
-            bank bisect start
-            bank bisect good 12e4f5
-            bank bisect bad master
-            <do build / test>
-            bank bisect good 78a6b9
-            <do build / test>
-            bank bisect bad ae726a
-            ...
-        
-        Basically we are git bisecting on the syncrepo, and after each bisect step we get a new configuration, then `bank sync` will be run to synchronize the repositories in the bank to their state at the time that iteration of the syncfile was recorded . So `bank bisect <arguments>` is basically equivalent to `git bisect <arguments>; bank sync`
-        
-        #### Dispatching git commands
-        
-        We can use `bank` to perform a git command on each repository in the bank. All git commands have the prefix 'git' along with the normal name of the git command. Eg
-        
-            bank git status --syncfile syncfile.wl
-        
-        Will perform a `git status` operation on each of the repositories in the bank and print the results to stdout.
-        
-        If you use `gitall` instead of `git` command, then the git command will also be run in the syncrepo.
-        
-            bank gitall status --syncfile syncfile.wl
-        
-        Will perform a `git status` operation on each of the repositories in the bank and print the results to stdout.
-        
-        ## Testing
-        
-        To run the test suite you need `py.test` installed on your machine. Then after downloading the source code you can simply execute:
-        
-        ```
-        cd banksync_Package
-        py.test
-        ```
-        
-Keywords: execute,shell,system,git,submodule
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Version Control
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
+## Purpose
+
+`banksync` is a command line tool that simplifies the use of git commands across a "bank" or "collection" of repositories. It enables synchronization of historical configurations throughout the bank of repos.
+
+## Installation
+
+You can install `banksync` from PyPi with a simple:
+
+
+    pip install banksync
+
+## Quick Start
+
+A bank is a collection of repos defined in a *syncfile*. The syncfile typically resides in a *syncrepo*. In this example, we'll use a project called `animals` containing two repos: `repoFish` and `repoBirds`. The project can be placed anywhere, but for simplicity, we'll put it in the user's root directory.
+
+To quickly clone and populate the example collection of repos, use the following commands:
+
+    cd ~
+    bank clone https://github.com/testbank/animalsRepoSync.git animals
+
+This will git clone the thin syncrepo, which contains the syncfile, and then populate all constituent repos. The resulting structure will be:
+
+    animals
+    ├── repoBird
+    │   └── Bird.txt
+    ├── repoFish
+    │   └── Fish.txt
+    └── syncrepo
+        ├── bankconfig.ini
+        └── syncfile.json
+
+
+Let's walk quickly through what is happening
+
+### Step-by-step Walkthrough
+
+Let's break down the quick start process into steps.
+
+1. Create a directory `animals`:
+
+   ```
+   cd ~
+   sudo rm -r animals
+   mkdir animals
+   cd animals
+   ```
+
+2. Clone the demonstration syncrepo for the animals project using standard git:
+
+   ```
+   git clone https://github.com/testbank/animalsRepoSync.git
+   ```
+
+   This clones the thin repo, which records the syncfile over time. It tracks the state of the repos in the bank at different times or stages. The resulting hierarchy is:
+
+   ```
+   animals
+   └── animalsRepoSync
+       ├── bankconfig.ini
+       └── syncfile.json
+   ```
+
+3. Populate the repositories in the bank:
+
+   ```
+   cd animalsRepoSync
+   bank populate
+   ```
+
+   The `populate` command clones each of the repos specified in the syncfile, resulting in the following layout:
+
+   ```
+   animals
+   ├── animalsRepoSync
+   │   ├── bankconfig.ini
+   │   └── syncfile.json
+   ├── repoBird
+   │   └── Bird.txt
+   └── repoFish
+       └── Fish.txt
+   ```
+
+### issuing commands
+
+We can now issue commands across the repos in the bank. From the syncrepo we can execute:
+
+    cd ~/animals/animalsRepoSync
+    bank git status
+
+Which will execute the status command in each of the repos in the bank. If we want to checkout a previous state across the repos in the project we can do this via (from the syncrepo):
+
+    git checkout master~2
+    bank sync
+
+The last two commands just moved the syncrepo two revisions back, and then synchronized the repos in the bank to the sync file at this earlier time. To get all repos back to the master branch revisions you can simply execute:
+
+    bank gitall checkout master
+
+Which will do a `git checkout master` on all the repos in the bank including the sync repo.
+
+## Syncfile
+
+The syncfile specifies which repositories are part of the bank, and what state the repositories should be synchronized to. A typical simple sync file might be the following
+
+    more ~/animals/animalsRepoSync/syncfile.json
+
+Which yields:
+
+```
+<|
+    "repoFish" -> <|
+        "path" -> "repoFish",
+        "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
+        "UnixTimeStamp" -> "1480517200",
+        "date" -> "30 Nov 2016 - 15:46:40",
+        "author" -> "Jason Harris",
+        "revisionNumber" -> "3",
+        "message" -> "committing salmon",
+        "cloneURL" -> "https://github.com/testbank/repoFish.git"
+    |>,
+    "repoBird" -> <|
+        "path" -> "repoBird",
+        "sha" -> "6bf9d646b2aa224b64fb86cbddb4d7ab0f2e37d3",
+        "UnixTimeStamp" -> "1480517200",
+        "date" -> "30 Nov 2016 - 15:46:40",
+        "author" -> "Jason Harris",
+        "revisionNumber" -> "3",
+        "message" -> "committing eagle",
+        "cloneURL" -> "https://github.com/testbank/repoBird.git"
+    |>
+|>
+```
+
+The syncfile should lie inside a git repo (the syncrepo). Whenever we want to record a configuration of the repos we simply alter the syncfile by transcribing the current state of the repos into the syncfile using `bank record_repos` with the appropriate options. We then use `git commit` to record this new state / configuration in the syncrepo.
+
+So let us add some content to repoBird in our example and then commit this change.
+
+    cd  ~/animals/repoBird
+    echo "toucan" >> Bird.txt
+    git commit -am "committing toucan"
+
+So now we can update the syncfile with the state of the current repos in the bank:
+
+    cd ~/animals/animalsRepoSync/
+    bank record_repos
+
+The contents of our syncfile will now be something like:
+
+```
+<|
+    "repoFish" -> <|
+        "path" -> "repoFish",
+        "sha" -> "a27368bec17373938b1dcf73638945b89b60a9d0",
+        "UnixTimeStamp" -> "1480517200",
+        "date" -> "30 Nov 2016 - 15:46:40",
+        "author" -> "Jason Harris",
+        "revisionNumber" -> "3",
+        "message" -> "committing salmon",
+        "cloneURL" -> "https://github.com/testbank/repoFish.git"
+    |>,
+    "repoBird" -> <|
+        "path" -> "repoBird",
+        "sha" -> "c8fb05947c5161e484104d99f427ec082fb4e85b",
+        "UnixTimeStamp" -> "1480519159",
+        "date" -> "30 Nov 2016 - 16:19:19",
+        "author" -> "Jason Harris",
+        "revisionNumber" -> "4",
+        "message" -> "committing toucan",
+        "cloneURL" -> "https://github.com/testbank/repoBird.git"
+    |>
+|>
+```
+
+(Note the sha, timestamps, and other data about the state of the repo `repoBird` has changed.)
+
+So we could now record this new overall state of the repos in the bank via simply committing the file syncfile in the syncrepo.
+
+    git commit -am "recording the latest state of the repos in animals."
+
+## Locations
+
+How does the bank command know where to put the `repoBird` and `repoFish`? How does it know which syncfile to use, etc. Well in the syncrepo there is the file `bankconfig.ini`. This is a standard preferences file but in this example it has two important options: `cwd=..` and `syncfile=syncfile.json`.
+
+The cwd (ChangeWorkingDirectory) option specifies that the repo commands should be executed one level up from our current working directory. So since we are currently at `~/animals/animalsRepoSync` that means that the repos paths will start from `~/animals/`
+
+The second option just tells us what the name of the syncfile is. We could have called it `earthanimals.json` if we wanted to.
+
+## Bank command line options
+
+The command line tool `bank` has several options which can be specified:
+
+#### --syncfile <path>
+
+The `syncfile` option specifies a syncfile. The syncfile contents specify which repos are part of the bank. The various keys which are recorded if present are:`path`, `sha`, `UnixTimeStamp`, `date`, `author`, `revisionNumber`, `message`, and `cloneURL`. Adding other keys at present will not effect or change the behavior of the bank tool so you can add other info as you see fit / want to each of the recorded states in the various repos.
+
+#### --cwd <path>
+
+The cwd option will change the working directory. Using this you can specify the relative path to get to the base of where the path for each of the repos in the bank are. For instance in the layout example of the animals project above, if we are in the directory `animals/animalsSyncRepo` then since the path in the syncfile for "Birds" is just `repoBird` then relative to `animals/animalsSyncRepo` we want the directory `../repoBird`. So we would use the option `--cwd ..`
+
+#### --dryrun
+
+If this option is specified then `banksync` will report what it *would* do but it doesn't actually do anything.
+
+#### --colorize <bool>
+
+You can specify if color is not to be used in output if for instance you want the logs to be parsed in jenkins or other devops tools. (The default is `True`, i.e. colorize the output of the bank command)
+
+#### --verbosity <num>
+
+You can specify how much information banksync reports. This integer should be between 0, 1, 2, 3, or 4. The higher the number the more verbose is the reporting. The default is 2.
+
+#### --matching <type>
+
+When attempting to sync the constituent repos to the versions specified in the syncfile, how do we determine what to set the versions to? We want some loose coupling in that for instance if someone runs filter branch on a project or they do some rebase very early on in the history then the shas will change on all the revisions in the repository. So instead of finding a commit via a sha we will have to fall back to looking for a matching timestamp for the revision. These are generally fairly unique in a project unless a lot of cherrypicking has gone on. If we don't find that exact timestamp then we could fall back to the closest matching revision to that timestamp. In this way at least we have some hope of getting close to the configuration at the time instead of just giving up. Ie we get to the exact configuration if it is available but if not get as close as we can. The value of the option can be:
+
+- **shaOnly**: if we can't find the exact same revision given by the sha in the syncfile than give up.
+- **timestamps**: try matching by sha first but if that fails find the first revision with the same unix timestamp. (This is almost always preserved across repo manipulation)
+- **closetimestamps**: try matching by sha first, if that fails try matching by timestamp. and if that fails find the revision with the closest timestamp and match to that.
+
+## Config file
+
+Instead of specifying the `--syncfile` and`—cwd` in each command you can create a `bankconfig.ini` file alongside the syncfile. In the `bankconfig.ini` file you can specify the default syncfile and cwd to use if none is specified. Eg we could add the file `animals/animalsSyncRepo/bankconfig.ini` with the following contents:
+
+    [general]
+    cwd=..
+    syncFile=syncfile.json
+
+Then you could omit the options to the bank command and they would be taken from the bankconfig.ini file so the above example would become:
+
+    cd animals/animalsSyncRepo
+    bank record_repos
+    git commit -am "recording the latest state of the repos in animals."
+
+You can choose weather to include the `bankconfig.ini` in the syncrepo history or not. (We choose to in this example but other teams may leave this to the individual developers.)
+
+## Commands
+
+The form of a bank command is `bank <cmd> <opts>` where `<cmd>` is one of `sync`, `record_repos`, `create_syncfile`, `bisect`, `populate`,  `git` or `gitall` 
+
+#### bank sync <opts>
+
+`sync` will update / checkout the revisions specified in the syncfile for each of the repos specified in the bank.
+
+    bank sync --syncfile syncfile.json
+
+This would checkout / update the repos given in the syncfile `syncfile.json` to the states given in the syncfile. It each repo it tries to checkout the version first by the given sha, and then it falls back to the given timestamp, and then it falls back to the closest timestamp. (This fallback behavior can be controlled by the `--matching` option.)
+
+    bank sync --syncfile syncfile.json --cwd ../other/dir
+
+This would checkout / update the repos given in the syncfile to the states given in the syncfile
+(but the path to each repo in the bank will be prefixed by the value of the `--cwd` option `../other/dir`).
+
+#### bank record_repos <opts>
+
+`record_repos` is used to transcribe the current state of the repos into the syncfile. Eg:
+
+    bank record_repos --syncfile syncfile.json
+
+This would alter the contents of the syncfile and change the revisions stored in the syncfile.json to match the current revisions of the referenced repositories.
+
+#### bank create_syncfile <opts>
+
+`create_syncfile` is used to generate an initial syncfile. Eg:
+
+    bank create_syncfile --syncfile syncfile.json repo1 repo2 ... repoN --cwd some/dir
+
+This would generate or overwrite the syncfile.json to contain sync points for the current states of `repo1`, `repo2`, ... `repoN`
+
+#### bank create_syncrepo <opts>
+
+`create_syncrepo` is used to generate the syncrepo directory, initialize a git repository there, create the syncfile and also create the bankconfig.ini file. Basically it creates all the working parts of a syncrepo. Eg:
+
+    bank create_syncrepo repo1 repo2 ... repoN
+
+This would create the directory `syncrepo` and fill it with a `syncfile.json` and a `bankconfig.ini`. The syncfile would contain the latest states of the `repo1`, `repo2`, ... `repoN`. 
+
+    bank create_syncrepo --syncreponame controlrepo --syncfilename felipe.json repo1 repo2 ... repoN
+
+Would create and initialize a syncrepo called `controlrepo` and inside that a syncfile called `felipe.json`.
+
+#### bank bisect <opts>
+
+You can use `bank bisect` on the syncrepo to step through historic configurations looking for a configuration which produces some change. (Typically we are searching for a regression.) Eg if we have a configuration file in the syncrepo the following might be a typical bisect session:
+
+    cd SomeSyncRepo
+    bank bisect start
+    bank bisect good 12e4f5
+    bank bisect bad master
+    <do build / test>
+    bank bisect good 78a6b9
+    <do build / test>
+    bank bisect bad ae726a
+    ...
+
+Basically we are git bisecting on the syncrepo, and after each bisect step we get a new configuration, then `bank sync` will be run to synchronize the repositories in the bank to their state at the time that iteration of the syncfile was recorded . So `bank bisect <arguments>` is basically equivalent to `git bisect <arguments>; bank sync`
+
+#### Dispatching git commands
+
+We can use `bank` to perform a git command on each repository in the bank. All git commands have the prefix 'git' along with the normal name of the git command. Eg
+
+    bank git status --syncfile syncfile.json
+
+Will perform a `git status` operation on each of the repositories in the bank and print the results to stdout.
+
+If you use `gitall` instead of `git` command, then the git command will also be run in the syncrepo.
+
+    bank gitall status --syncfile syncfile.json
+
+Will perform a `git status` operation on each of the repositories in the bank and print the results to stdout.
+
+## Testing
+
+To run the test suite you need `py.test` installed on your machine. Then after downloading the source code you can simply execute:
+
+    cd banksync_Package
+    py.test
+
```

### Comparing `banksync-0.9.4/setup.py` & `banksync-0.9.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-from setuptools import setup
+import setuptools
 
 with open('README.md') as f:
     long_description = f.read()
 
-version = '0.9.4'
+# Read the version number from banksync.py so we only need to specify it in a single place
+version = "unknown"
+with open('banksync/banksync.py') as f:
+    for line in f:
+        if line.startswith('__version__'):
+            _, _, version = line.replace("\"", '').replace("'", '').split()
+            break
 
-setup(
+setuptools.setup(
     name = 'banksync',
-    packages = ['banksync'], # this must be the same as the name above
+    packages = setuptools.find_packages(),
     version = version,
     description = 'A library for manipulating banks of git repositories',
     long_description = long_description,
     long_description_content_type='text/markdown',  # This is important!
     author = 'Jason Harris',
     author_email = 'jason@jasonfharris.com',
     license='MIT',
```

