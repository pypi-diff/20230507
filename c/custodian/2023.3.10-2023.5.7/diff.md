# Comparing `tmp/custodian-2023.3.10.tar.gz` & `tmp/custodian-2023.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodian-2023.3.10.tar", last modified: Fri Mar 10 22:13:47 2023, max compression
+gzip compressed data, was "custodian-2023.5.7.tar", last modified: Sun May  7 20:41:37 2023, max compression
```

## Comparing `custodian-2023.3.10.tar` & `custodian-2023.5.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:13:47.147518 custodian-2023.3.10/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-10 22:09:49.000000 custodian-2023.3.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-10 22:09:49.000000 custodian-2023.3.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-03-10 22:13:47.147518 custodian-2023.3.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-03-10 22:09:49.000000 custodian-2023.3.10/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:13:47.143518 custodian-2023.3.10/custodian/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:13:47.143518 custodian-2023.3.10/custodian/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/ansible/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/ansible/interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:13:47.143518 custodian-2023.3.10/custodian/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/cli/converge_geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4538 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/cli/converge_kpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/cli/cstdn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2337 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/cli/run_nwchem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12410 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/cli/run_vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:13:47.143518 custodian-2023.3.10/custodian/cp2k/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/cp2k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/cp2k/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/cp2k/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/cp2k/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/cp2k/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/cp2k/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    36593 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:13:47.147518 custodian-2023.3.10/custodian/feff/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/feff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/feff/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/feff/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/feff/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:13:47.147518 custodian-2023.3.10/custodian/lobster/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/lobster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/lobster/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/lobster/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:13:47.147518 custodian-2023.3.10/custodian/nwchem/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/nwchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/nwchem/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/nwchem/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:13:47.147518 custodian-2023.3.10/custodian/qchem/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/qchem/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/qchem/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/qchem/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:13:47.147518 custodian-2023.3.10/custodian/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/tests/test_custodian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:13:47.147518 custodian-2023.3.10/custodian/vasp/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75334 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/vasp/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/vasp/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    38518 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/vasp/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-03-10 22:09:49.000000 custodian-2023.3.10/custodian/vasp/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 22:13:47.143518 custodian-2023.3.10/custodian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-03-10 22:13:47.000000 custodian-2023.3.10/custodian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-10 22:13:47.000000 custodian-2023.3.10/custodian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 22:13:47.000000 custodian-2023.3.10/custodian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-10 22:13:47.000000 custodian-2023.3.10/custodian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-10 22:13:47.000000 custodian-2023.3.10/custodian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-10 22:13:47.000000 custodian-2023.3.10/custodian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-10 22:09:49.000000 custodian-2023.3.10/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-10 22:09:49.000000 custodian-2023.3.10/requirements-ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-10 22:09:49.000000 custodian-2023.3.10/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-10 22:13:47.147518 custodian-2023.3.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-10 22:09:49.000000 custodian-2023.3.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.788636 custodian-2023.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-07 20:37:45.000000 custodian-2023.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-07 20:37:45.000000 custodian-2023.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-07 20:41:37.788636 custodian-2023.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-07 20:37:45.000000 custodian-2023.5.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.780636 custodian-2023.5.7/custodian/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/ansible/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/ansible/interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/converge_geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4538 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/converge_kpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/cstdn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2337 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/run_nwchem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12410 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/run_vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/cp2k/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36593 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/feff/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/feff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/feff/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/feff/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/feff/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/lobster/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/lobster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/lobster/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/lobster/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/nwchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/nwchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/nwchem/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/nwchem/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/qchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/qchem/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/qchem/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/qchem/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.788636 custodian-2023.5.7/custodian/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/tests/test_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.788636 custodian-2023.5.7/custodian/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76156 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38518 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-07 20:37:45.000000 custodian-2023.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 20:37:45.000000 custodian-2023.5.7/requirements-ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-07 20:37:45.000000 custodian-2023.5.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-07 20:41:37.788636 custodian-2023.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-07 20:37:45.000000 custodian-2023.5.7/setup.py
```

### Comparing `custodian-2023.3.10/LICENSE` & `custodian-2023.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/PKG-INFO` & `custodian-2023.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custodian
-Version: 2023.3.10
+Version: 2023.5.7
 Summary: A simple JIT job management framework in Python.
 Home-page: https://github.com/materialsproject/custodian
 Author: Shyue Ping Ong, William Davidson Richards, Stephen Dacek, Xiaohui Qu, Matthew Horton, Samuel M. Blau
 Author-email: ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 License: MIT
 Keywords: jit,just-in-time,job,management,vasp
```

### Comparing `custodian-2023.3.10/README.rst` & `custodian-2023.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/ansible/actions.py` & `custodian-2023.5.7/custodian/ansible/actions.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/ansible/interpreter.py` & `custodian-2023.5.7/custodian/ansible/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/cli/converge_geometry.py` & `custodian-2023.5.7/custodian/cli/converge_geometry.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/cli/converge_kpoints.py` & `custodian-2023.5.7/custodian/cli/converge_kpoints.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/cli/cstdn.py` & `custodian-2023.5.7/custodian/cli/cstdn.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/cli/run_nwchem.py` & `custodian-2023.5.7/custodian/cli/run_nwchem.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/cli/run_vasp.py` & `custodian-2023.5.7/custodian/cli/run_vasp.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/cp2k/handlers.py` & `custodian-2023.5.7/custodian/cp2k/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/cp2k/interpreter.py` & `custodian-2023.5.7/custodian/cp2k/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/cp2k/jobs.py` & `custodian-2023.5.7/custodian/cp2k/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/cp2k/utils.py` & `custodian-2023.5.7/custodian/cp2k/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/cp2k/validators.py` & `custodian-2023.5.7/custodian/cp2k/validators.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/custodian.py` & `custodian-2023.5.7/custodian/custodian.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/feff/handlers.py` & `custodian-2023.5.7/custodian/feff/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/feff/interpreter.py` & `custodian-2023.5.7/custodian/feff/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/feff/jobs.py` & `custodian-2023.5.7/custodian/feff/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/lobster/handlers.py` & `custodian-2023.5.7/custodian/lobster/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/lobster/jobs.py` & `custodian-2023.5.7/custodian/lobster/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/nwchem/handlers.py` & `custodian-2023.5.7/custodian/nwchem/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/nwchem/jobs.py` & `custodian-2023.5.7/custodian/nwchem/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/qchem/handlers.py` & `custodian-2023.5.7/custodian/qchem/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/qchem/jobs.py` & `custodian-2023.5.7/custodian/qchem/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/qchem/utils.py` & `custodian-2023.5.7/custodian/qchem/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/tests/test_custodian.py` & `custodian-2023.5.7/custodian/tests/test_custodian.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/utils.py` & `custodian-2023.5.7/custodian/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/vasp/handlers.py` & `custodian-2023.5.7/custodian/vasp/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import shutil
 import time
 import warnings
 from collections import Counter
 from functools import reduce
 
 import numpy as np
-from monty.dev import deprecated
 from monty.os.path import zpath
 from monty.serialization import loadfn
 from pymatgen.core.structure import Structure
 from pymatgen.io.vasp.inputs import Incar, Kpoints, Poscar, VaspInput
 from pymatgen.io.vasp.outputs import Oszicar, Outcar, Vasprun
 from pymatgen.io.vasp.sets import MPScanRelaxSet
 from pymatgen.transformations.standard_transformations import SupercellTransformation
@@ -100,74 +99,67 @@
         "point_group": ["group operation missing"],
         "symprec_noise": ["determination of the symmetry of your systems shows a strong"],
         "dfpt_ncore": ["PEAD routines do not work for NCORE", "remove the tag NPAR from the INCAR file"],
         "bravais": ["Inconsistent Bravais lattice"],
         "nbands_not_sufficient": ["number of bands is not sufficient"],
         "hnform": ["HNFORM: k-point generating"],
         "coef": ["while reading plane"],
+        "set_core_wf": ["internal error in SET_CORE_WF"],
     }
 
     def __init__(
         self,
         output_filename="vasp.out",
-        natoms_large_cell=None,
         errors_subset_to_catch=None,
         vtst_fixes=False,
     ):
         """
         Initializes the handler with the output file to check.
 
         Args:
             output_filename (str): This is the file where the stdout for vasp
                 is being redirected. The error messages that are checked are
                 present in the stdout. Defaults to "vasp.out", which is the
                 default redirect used by :class:`custodian.vasp.jobs.VaspJob`.
-            natoms_large_cell (int): Number of atoms threshold to treat cell
-                as large. Affects the correction of certain errors. Defaults to
-                None (not used). Deprecated.
             errors_subset_to_detect (list): A subset of errors to catch. The
                 default is None, which means all supported errors are detected.
                 Use this to only catch only a subset of supported errors.
                 E.g., ["eddrrm", "zheev"] will only catch the eddrmm and zheev
                 errors, and not others. If you wish to only excluded one or
                 two of the errors, you can create this list by the following
                 lines:
             vtst_fixes (bool): Whether to consider VTST optimizers. Defaults to
-                False for compatibility purposes.
+                False for compatibility purposes, but if you have VTST, you
+                would likely benefit from setting this to True.
 
                 ```
                 subset = list(VaspErrorHandler.error_msgs.keys())
                 subset.pop("eddrrm")
 
                 handler = VaspErrorHandler(errors_subset_to_catch=subset)
                 ```
         """
         self.output_filename = output_filename
         self.errors = set()
         self.error_count = Counter()
-        # threshold of number of atoms to treat the cell as large.
-        self.natoms_large_cell = natoms_large_cell  # (deprecated)
-        if self.natoms_large_cell:
-            warnings.warn(
-                "natoms_large_cell is deprecated and currently does nothing.",
-                DeprecationWarning,
-            )
         self.errors_subset_to_catch = errors_subset_to_catch or list(VaspErrorHandler.error_msgs.keys())
         self.vtst_fixes = vtst_fixes
         self.logger = logging.getLogger(self.__class__.__name__)
 
     def check(self):
         """
         Check for error.
         """
         incar = Incar.from_file("INCAR")
         self.errors = set()
         error_msgs = set()
         with open(self.output_filename) as file:
             text = file.read()
+
+            # Check for errors
             for err in self.errors_subset_to_catch:
                 for msg in self.error_msgs[err]:
                     if text.find(msg) != -1:
                         # this checks if we want to run a charged
                         # computation (e.g., defects) if yes we don't
                         # want to kill it because there is a change in
                         # e-density (brmix error)
@@ -196,15 +188,16 @@
                         "action": {"_set": {"KSPACING": vi["INCAR"].get("KSPACING") * 0.8}},
                     }
                 )
             else:
                 actions.append({"dict": "INCAR", "action": {"_set": {"ISMEAR": 0, "SIGMA": 0.05}}})
 
         if "inv_rot_mat" in self.errors:
-            actions.append({"dict": "INCAR", "action": {"_set": {"SYMPREC": 1e-8}}})
+            if vi["INCAR"].get("SYMPREC", 1e-5) > 1e-8:
+                actions.append({"dict": "INCAR", "action": {"_set": {"SYMPREC": 1e-8}}})
 
         if "brmix" in self.errors:
             # If there is not a valid OUTCAR already, increment
             # error count to 1 to skip first fix
             if self.error_count["brmix"] == 0:
                 try:
                     assert Outcar(zpath(os.path.join(os.getcwd(), "OUTCAR"))).is_stopped is False
@@ -213,157 +206,166 @@
 
             if self.error_count["brmix"] == 0:
                 # Valid OUTCAR - simply rerun the job and increment
                 # error count for next time
                 actions.append({"dict": "INCAR", "action": {"_set": {"ISTART": 1}}})
                 self.error_count["brmix"] += 1
 
-            elif self.error_count["brmix"] == 1:
+            elif self.error_count["brmix"] == 1 and vi["INCAR"].get("IMIX", 4) != 1:
                 # Use Kerker mixing w/default values for other parameters
                 actions.append({"dict": "INCAR", "action": {"_set": {"IMIX": 1}}})
                 self.error_count["brmix"] += 1
 
-            elif self.error_count["brmix"] == 2 and vi["KPOINTS"].style == Kpoints.supported_modes.Gamma:
+            elif (
+                self.error_count["brmix"] == 2
+                and vi["KPOINTS"] is not None
+                and vi["KPOINTS"].style == Kpoints.supported_modes.Gamma
+            ):
                 actions.append(
                     {
                         "dict": "KPOINTS",
                         "action": {"_set": {"generation_style": "Monkhorst"}},
                     }
                 )
-                actions.append({"dict": "INCAR", "action": {"_unset": {"IMIX": 1}}})
+                if "IMIX" in vi["INCAR"]:
+                    actions.append({"dict": "INCAR", "action": {"_unset": {"IMIX": 1}}})
                 self.error_count["brmix"] += 1
 
             elif self.error_count["brmix"] in [2, 3] and vi["KPOINTS"].style == Kpoints.supported_modes.Monkhorst:
                 actions.append(
                     {
                         "dict": "KPOINTS",
                         "action": {"_set": {"generation_style": "Gamma"}},
                     }
                 )
-                actions.append({"dict": "INCAR", "action": {"_unset": {"IMIX": 1}}})
+                if "IMIX" in vi["INCAR"]:
+                    actions.append({"dict": "INCAR", "action": {"_unset": {"IMIX": 1}}})
                 self.error_count["brmix"] += 1
 
-                if vi["KPOINTS"].num_kpts < 1:
-                    all_kpts_even = all(n % 2 == 0 for n in vi["KPOINTS"].kpts[0])
-                    if all_kpts_even:
-                        new_kpts = (tuple(n + 1 for n in vi["KPOINTS"].kpts[0]),)
-                        actions.append(
-                            {
-                                "dict": "KPOINTS",
-                                "action": {"_set": {"kpoints": new_kpts}},
-                            }
-                        )
+                if vi["KPOINTS"].num_kpts < 1 and all(n % 2 == 0 for n in vi["KPOINTS"].kpts[0]):
+                    new_kpts = (tuple(n + 1 for n in vi["KPOINTS"].kpts[0]),)
+                    actions.append(
+                        {
+                            "dict": "KPOINTS",
+                            "action": {"_set": {"kpoints": new_kpts}},
+                        }
+                    )
 
             else:
-                actions.append({"dict": "INCAR", "action": {"_set": {"ISYM": 0}}})
-                if vi["KPOINTS"] is not None:
-                    if vi["KPOINTS"].style == Kpoints.supported_modes.Monkhorst:
-                        actions.append(
-                            {
-                                "dict": "KPOINTS",
-                                "action": {"_set": {"generation_style": "Gamma"}},
-                            }
-                        )
+                if vi["INCAR"].get("ISYM", 2) > 0:
+                    actions.append({"dict": "INCAR", "action": {"_set": {"ISYM": 0}}})
+                if vi["KPOINTS"] is not None and vi["KPOINTS"].style == Kpoints.supported_modes.Monkhorst:
+                    actions.append(
+                        {
+                            "dict": "KPOINTS",
+                            "action": {"_set": {"generation_style": "Gamma"}},
+                        }
+                    )
+                if vi["KPOINTS"] is not None and vi["KPOINTS"].style == Kpoints.supported_modes.Monkhorst:
+                    actions.append(
+                        {
+                            "dict": "KPOINTS",
+                            "action": {"_set": {"generation_style": "Gamma"}},
+                        }
+                    )
 
                 # Based on VASP forum's recommendation, you should delete the
                 # CHGCAR and WAVECAR when dealing with this error.
+                # A.S.R.: Then why only delete them now?
                 if vi["INCAR"].get("ICHARG", 0) < 10:
                     actions.append(
                         {
                             "file": "CHGCAR",
                             "action": {"_file_delete": {"mode": "actual"}},
                         }
                     )
                     actions.append(
                         {
                             "file": "WAVECAR",
                             "action": {"_file_delete": {"mode": "actual"}},
                         }
                     )
+                self.error_count["brmix"] += 1
 
         if "zpotrf" in self.errors:
             # Usually caused by short bond distances. If on the first step,
             # volume needs to be increased. Otherwise, it was due to a step
             # being too big and POTIM should be decreased. If a static run
-            # try turning off symmetry.
+            # try turning off symmetry. This also happens if NCORE or NPAR
+            # is set to a large value for a small structure.
+
             try:
                 oszicar = Oszicar("OSZICAR")
                 nsteps = len(oszicar.ionic_steps)
             except Exception:
                 nsteps = 0
 
-            if nsteps >= 1:
-                potim = round(vi["INCAR"].get("POTIM", 0.5) / 2.0, 2)
-                actions.append({"dict": "INCAR", "action": {"_set": {"ISYM": 0, "POTIM": potim}}})
-            elif vi["INCAR"].get("NSW", 0) == 0 or vi["INCAR"].get("ISIF", 0) in range(3):
+            if vi["INCAR"].get("ISYM", 2) > 0:
                 actions.append({"dict": "INCAR", "action": {"_set": {"ISYM": 0}}})
-            else:
-                s = vi["POSCAR"].structure
-                s.apply_strain(0.2)
-                actions.append({"dict": "POSCAR", "action": {"_set": {"structure": s.as_dict()}}})
 
-            # Based on VASP forum's recommendation, you should delete the
-            # CHGCAR and WAVECAR when dealing with this error.
-            if vi["INCAR"].get("ICHARG", 0) < 10:
-                actions.append({"file": "CHGCAR", "action": {"_file_delete": {"mode": "actual"}}})
-                actions.append({"file": "WAVECAR", "action": {"_file_delete": {"mode": "actual"}}})
-
-            # A.S.R.: This can also happen if NCORE or NPAR is set to an unusually large value.
-            # We should add logic for this at some point.
+            # The natoms of 5 was chosen somewhat arbitrarily. Could be worth revisiting to fine-tune.
+            if len(vi["POSCAR"].structure) < 5 and (vi["INCAR"].get("NCORE", 1) > 1 or vi["INCAR"].get("NPAR", 1) > 1):
+                actions.append({"dict": "INCAR", "action": {"_set": {"NCORE": 1}}})
+                if vi["INCAR"].get("NPAR", 1) > 1:
+                    actions.append({"dict": "INCAR", "action": {"_unset": {"NPAR": 1}}})
+            elif vi["INCAR"].get("NSW", 0) > 0:
+                if nsteps == 0:
+                    s = vi["POSCAR"].structure
+                    s.apply_strain(0.2)
+                    actions.append({"dict": "POSCAR", "action": {"_set": {"structure": s.as_dict()}}})
+                else:
+                    potim = round(vi["INCAR"].get("POTIM", 0.5) / 2.0, 2)
+                    actions.append({"dict": "INCAR", "action": {"_set": {"POTIM": potim}}})
 
         if self.errors.intersection(["subspacematrix"]):
-            if self.error_count["subspacematrix"] == 0:
+            if self.error_count["subspacematrix"] == 0 and vi["INCAR"].get("LREAL", False) is not False:
                 actions.append({"dict": "INCAR", "action": {"_set": {"LREAL": False}}})
-            elif self.error_count["subspacematrix"] == 1:
+            elif self.error_count["subspacematrix"] == 1 and vi["INCAR"].get("PREC", "Normal") != "Accurate":
                 actions.append({"dict": "INCAR", "action": {"_set": {"PREC": "Accurate"}}})
             self.error_count["subspacematrix"] += 1
 
         if self.errors.intersection(["rspher", "real_optlay", "nicht_konv"]):
             if vi["INCAR"].get("LREAL", False) is not False:
                 actions.append({"dict": "INCAR", "action": {"_set": {"LREAL": False}}})
 
         if self.errors.intersection(["tetirr", "incorrect_shift"]):
-            if vi["KPOINTS"] is not None:
-                if vi["KPOINTS"].style == Kpoints.supported_modes.Monkhorst:
-                    actions.append(
-                        {
-                            "dict": "KPOINTS",
-                            "action": {"_set": {"generation_style": "Gamma"}},
-                        }
-                    )
+            if vi["KPOINTS"] is not None and vi["KPOINTS"].style == Kpoints.supported_modes.Monkhorst:
+                actions.append(
+                    {
+                        "dict": "KPOINTS",
+                        "action": {"_set": {"generation_style": "Gamma"}},
+                    }
+                )
 
         if "rot_matrix" in self.errors:
-            if vi["KPOINTS"] is not None:
-                if vi["KPOINTS"].style == Kpoints.supported_modes.Monkhorst:
-                    actions.append(
-                        {
-                            "dict": "KPOINTS",
-                            "action": {"_set": {"generation_style": "Gamma"}},
-                        }
-                    )
-            else:
+            if vi["KPOINTS"] is not None and vi["KPOINTS"].style == Kpoints.supported_modes.Monkhorst:
+                actions.append(
+                    {
+                        "dict": "KPOINTS",
+                        "action": {"_set": {"generation_style": "Gamma"}},
+                    }
+                )
+            elif vi["INCAR"].get("ISYM", 2) > 0:
                 actions.append({"dict": "INCAR", "action": {"_set": {"ISYM": 0}}})
 
-        if "amin" in self.errors:
-            actions.append({"dict": "INCAR", "action": {"_set": {"AMIN": "0.01"}}})
-
         if "triple_product" in self.errors:
             s = vi["POSCAR"].structure
             trans = SupercellTransformation(((1, 0, 0), (0, 0, 1), (0, 1, 0)))
             new_s = trans.apply_transformation(s)
             actions.append(
                 {
                     "dict": "POSCAR",
                     "action": {"_set": {"structure": new_s.as_dict()}},
                     "transformation": trans.as_dict(),
                 }
             )
 
         if "pricel" in self.errors:
-            actions.append({"dict": "INCAR", "action": {"_set": {"SYMPREC": 1e-8, "ISYM": 0}}})
+            if vi["INCAR"].get("SYMPREC", 1e-5) > 1e-8:
+                actions.append({"dict": "INCAR", "action": {"_set": {"SYMPREC": 1e-8, "ISYM": 0}}})
 
         if "coef" in self.errors:
             actions.append({"file": "WAVECAR", "action": {"_file_delete": {"mode": "actual"}}})
 
         if "brions" in self.errors:
             # Copy CONTCAR to POSCAR so we do not lose our progress.
             actions.append({"file": "CONTCAR", "action": {"_file_copy": {"dest": "POSCAR"}}})
@@ -429,31 +431,38 @@
                 # first place without switching IBRION to 1.
                 if self.error_count["zbrent"] == 1:
                     actions.append({"dict": "INCAR", "action": {"_set": {"IBRION": 1}}})
 
             self.error_count["zbrent"] += 1
 
         if "too_few_bands" in self.errors:
+            nbands = None
             if "NBANDS" in vi["INCAR"]:
                 nbands = vi["INCAR"]["NBANDS"]
             else:
                 with open("OUTCAR") as f:
                     for line in f:
-                        if "NBANDS" in line:
+                        # Have to take the last NBANDS line since sometimes VASP
+                        # updates it automatically even if the user specifies it.
+                        # The last one is marked by NBANDS= (no space).
+                        if "NBANDS=" in line:
                             try:
                                 d = line.split("=")
                                 nbands = int(d[-1].strip())
                                 break
                             except (IndexError, ValueError):
                                 pass
-            new_nbands = max(int(1.1 * nbands), nbands + 1)  # This handles the case when nbands is too low (< 8).
-            actions.append({"dict": "INCAR", "action": {"_set": {"NBANDS": new_nbands}}})
+            if nbands:
+                new_nbands = max(int(1.1 * nbands), nbands + 1)  # This handles the case when nbands is too low (< 8).
+                actions.append({"dict": "INCAR", "action": {"_set": {"NBANDS": new_nbands}}})
 
         if "pssyevx" in self.errors:
-            actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "Normal"}}})
+            if vi["INCAR"].get("ALGO", "Normal").lower() != "normal":
+                actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "Normal"}}})
+
         if "eddrmm" in self.errors:
             # RMM algorithm is not stable for this calculation
             # Copy CONTCAR to POSCAR if CONTCAR has already been populated.
             try:
                 is_contcar = Poscar.from_file("CONTCAR")
             except Exception:
                 is_contcar = False
@@ -493,32 +502,14 @@
             try:
                 nelect = Outcar("OUTCAR").nelect
             except Exception:
                 nelect = 1  # dummy value
             if nelect < nprocs:
                 actions.append({"dict": "INCAR", "action": {"_set": {"NCORE": vi["INCAR"].get("NCORE", 1) * 2}}})
 
-        if "algo_tet" in self.errors:
-            # ALGO=All/Damped / IALGO=5X often fails with ISMEAR < 0. There are two options VASP
-            # suggests: 1) Use ISMEAR = 0 (and a small sigma) to get the SCF to converge.
-            # 2) Use ALGO = Damped but only *after* an ISMEAR = 0 run where the wavefunction
-            # has been stored and read in for the subsequent run.
-            #
-            # For simplicity, we go with Option 1 here, but if the user wants high-quality
-            # DOS then they should consider running a subsequent job with ISMEAR = -5 and
-            # ALGO = Damped, provided the wavefunction has been stored.
-            if vi["INCAR"].get("ISMEAR", 1) < 0:
-                actions.append({"dict": "INCAR", "action": {"_set": {"ISMEAR": 0, "SIGMA": 0.05}}})
-                if vi["INCAR"].get("NEDOS") or vi["INCAR"].get("EMIN") or vi["INCAR"].get("EMAX"):
-                    warnings.warn(
-                        "This looks like a DOS run. You may want to follow-up this job with ALGO = Damped"
-                        " and ISMEAR = -5, using the wavefunction from the current job.",
-                        UserWarning,
-                    )
-
         if "grad_not_orth" in self.errors:
             # Often coincides with algo_tet, in which the algo_tet error handler will also resolve grad_not_orth.
             # When not present alongside algo_tet, the grad_not_orth error is due to how VASP is compiled.
             # Depending on the optimization flag and choice of compiler, the ALGO = All and Damped algorithms
             # may not work. The only fix is either to change ALGO or to recompile VASP. Since meta-GGAs/hybrids
             # are often used with ALGO = All (and hybrids are incompatible with ALGO = VeryFast/Fast and slow with
             # ALGO = Normal), we do not adjust ALGO in these cases.
@@ -526,34 +517,38 @@
                 if vi["INCAR"].get("ALGO", "Normal").lower() in ["all", "damped"]:
                     actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "Fast"}}})
                 elif 53 <= vi["INCAR"].get("IALGO", 38) <= 58:
                     actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "Fast"}, "_unset": {"IALGO": 38}}})
             if "algo_tet" not in self.errors:
                 warnings.warn(
                     "EDWAV error reported by VASP without a simultaneous algo_tet error. You may wish to consider "
-                    "recompiling VASP with the -O1 optimization if you used -O2 and this error keeps cropping up."
+                    "recompiling VASP with the -O1 optimization if you used -O2 and this error keeps cropping up.",
+                    UserWarning,
                 )
 
         if "zheev" in self.errors:
             # Copy CONTCAR to POSCAR if CONTCAR has already been populated.
             try:
                 is_contcar = Poscar.from_file("CONTCAR")
             except Exception:
                 is_contcar = False
             if is_contcar:
                 actions.append({"file": "CONTCAR", "action": {"_file_copy": {"dest": "POSCAR"}}})
             if vi["INCAR"].get("ALGO", "Normal").lower() != "exact":
                 actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "Exact"}}})
+
         if "elf_kpar" in self.errors:
-            actions.append({"dict": "INCAR", "action": {"_set": {"KPAR": 1}}})
+            if vi["INCAR"].get("KPAR", 1) != 1:
+                actions.append({"dict": "INCAR", "action": {"_set": {"KPAR": 1}}})
 
         if "rhosyg" in self.errors:
-            if vi["INCAR"].get("SYMPREC", 1e-4) == 1e-4:
+            if vi["INCAR"].get("SYMPREC", 1e-5) < 1e-4:
+                actions.append({"dict": "INCAR", "action": {"_set": {"SYMPREC": 1e-4}}})
+            else:
                 actions.append({"dict": "INCAR", "action": {"_set": {"ISYM": 0}}})
-            actions.append({"dict": "INCAR", "action": {"_set": {"SYMPREC": 1e-4}}})
 
         if "posmap" in self.errors:
             # VASP advises to decrease or increase SYMPREC by an order of magnitude
             # the default SYMPREC value is 1e-5
             if self.error_count["posmap"] == 0:
                 # first, reduce by 10x
                 orig_symprec = vi["INCAR"].get("SYMPREC", 1e-5)
@@ -561,21 +556,23 @@
             elif self.error_count["posmap"] == 1:
                 # next, increase by 100x (10x the original)
                 orig_symprec = vi["INCAR"].get("SYMPREC", 1e-6)
                 actions.append({"dict": "INCAR", "action": {"_set": {"SYMPREC": orig_symprec * 100}}})
             self.error_count["posmap"] += 1
 
         if "point_group" in self.errors:
-            actions.append({"dict": "INCAR", "action": {"_set": {"ISYM": 0}}})
+            if vi["INCAR"].get("ISYM", 2) > 0:
+                actions.append({"dict": "INCAR", "action": {"_set": {"ISYM": 0}}})
 
         if "symprec_noise" in self.errors:
-            if (vi["INCAR"].get("ISYM", 2) > 0) and (vi["INCAR"].get("SYMPREC", 1e-5) > 1e-6):
-                actions.append({"dict": "INCAR", "action": {"_set": {"SYMPREC": 1e-6}}})
-            else:
-                actions.append({"dict": "INCAR", "action": {"_set": {"ISYM": 0}}})
+            if vi["INCAR"].get("ISYM", 2) > 0:
+                if vi["INCAR"].get("SYMPREC", 1e-5) > 1e-6:
+                    actions.append({"dict": "INCAR", "action": {"_set": {"SYMPREC": 1e-6}}})
+                else:
+                    actions.append({"dict": "INCAR", "action": {"_set": {"ISYM": 0}}})
 
         if "dfpt_ncore" in self.errors:
             # note that when using "_unset" action, the value is ignored
             if "NCORE" in vi["INCAR"]:
                 actions.append({"dict": "INCAR", "action": {"_unset": {"NCORE": 0}}})
             if "NPAR" in vi["INCAR"]:
                 actions.append({"dict": "INCAR", "action": {"_unset": {"NPAR": 0}}})
@@ -593,16 +590,24 @@
         if "nbands_not_sufficient" in self.errors:
             # There is something very wrong about the value of NBANDS. We don't make
             # any updates to NBANDS though because it's likely the user screwed something
             # up pretty badly during setup. For instance, this has happened to me if
             # MAGMOM = 2*nan or something similar.
 
             # Unfixable error. Just return None for actions.
+            warnings.warn("Double-check your INCAR. Something is potentially wrong.", UserWarning)
             return {"errors": ["nbands_not_sufficient"], "actions": None}
 
+        if "set_core_wf" in self.errors:
+            # Unfixable error where the solution is to update the POTCARs
+            warnings.warn(
+                "We suggest using a new version of the POTCAR files to resolve the SET_CORE_WF error.", UserWarning
+            )
+            return {"errors": ["set_core_wf"], "actions": None}
+
         if "hnform" in self.errors:
             # The only solution is to change your k-point grid or disable symmetry
             # For internal calculation compatibility's sake, we do the latter
             if vi["INCAR"].get("ISYM", 2) > 0:
                 actions.append({"dict": "INCAR", "action": {"_set": {"ISYM": 0}}})
 
         VaspModder(vi=vi).apply_actions(actions)
@@ -653,17 +658,16 @@
         Perform corrections.
         """
         backup(VASP_BACKUP_FILES | {self.output_filename})
         actions = []
         vi = VaspInput.from_directory(".")
 
         if "lrf_comm" in self.errors:
-            if Outcar(zpath(os.path.join(os.getcwd(), "OUTCAR"))).is_stopped is False:
-                if not vi["INCAR"].get("LPEAD"):
-                    actions.append({"dict": "INCAR", "action": {"_set": {"LPEAD": True}}})
+            if Outcar(zpath(os.path.join(os.getcwd(), "OUTCAR"))).is_stopped is False and not vi["INCAR"].get("LPEAD"):
+                actions.append({"dict": "INCAR", "action": {"_set": {"LPEAD": True}}})
 
         VaspModder(vi=vi).apply_actions(actions)
         return {"errors": list(self.errors), "actions": actions}
 
 
 class StdErrHandler(ErrorHandler):
     """
@@ -894,19 +898,16 @@
 
         incar = vi["INCAR"]
         outcar = Outcar("OUTCAR")
 
         # Move CONTCAR to POSCAR
         actions.append({"file": "CONTCAR", "action": {"_file_copy": {"dest": "POSCAR"}}})
 
-        # First try adding ADDGRID
-        if not incar.get("ADDGRID", False):
-            actions.append({"dict": "INCAR", "action": {"_set": {"ADDGRID": True}}})
-        # Otherwise set PREC to High so ENAUG can be used to control Augmentation Grid Size
-        elif incar.get("PREC", "Accurate").lower() != "high":
+        # Set PREC to High so ENAUG can be used to control Augmentation Grid Size
+        if incar.get("PREC", "Accurate").lower() != "high":
             actions.append({"dict": "INCAR", "action": {"_set": {"PREC": "High"}}})
             actions.append(
                 {
                     "dict": "INCAR",
                     "action": {"_set": {"ENAUG": incar.get("ENCUT", 520) * 2}},
                 }
             )
@@ -1030,34 +1031,59 @@
         """
         Perform corrections.
         """
         v = Vasprun(self.output_filename)
         algo = v.incar.get("ALGO", "Normal").lower()
         actions = []
         if not v.converged_electronic:
-            # Ladder from VeryFast to Fast to Normal to All
-            # (except for meta-GGAs and hybrids).
-            # These progressively switch to more stable but more
-            # expensive algorithms.
-            if v.incar.get("METAGGA", "--") != "--":
-                # If meta-GGA, go straight to Algo = All. Algo = All is recommended in the VASP
-                # manual and some meta-GGAs explicitly say to set Algo = All for proper convergence.
-                # I am using "--" as the check for METAGGA here because this is the default in the
-                # vasprun.xml file
-                if algo != "all":
-                    actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "All"}}})
-            elif v.incar.get("LHFCALC", False):
-                # If a hybrid is used, do not set Algo = Fast or VeryFast. Hybrid calculations do not
-                # support these algorithms, but no warning is printed.
+            # NOTE: This is the algo_tet handler response.
+            if (
+                v.incar.get("ALGO", "Normal").lower() in ["all", "damped"] or (50 <= v.incar.get("IALGO", 38) <= 59)
+            ) and v.incar.get("ISMEAR", 1) < 0:
+                # ALGO=All/Damped / IALGO=5X often fails with ISMEAR < 0. There are two options VASP
+                # suggests: 1) Use ISMEAR = 0 (and a small sigma) to get the SCF to converge.
+                # 2) Use ALGO = Damped but only *after* an ISMEAR = 0 run where the wavefunction
+                # has been stored and read in for the subsequent run.
+                #
+                # For simplicity, we go with Option 1 here, but if the user wants high-quality
+                # DOS then they should consider running a subsequent job with ISMEAR = -5 and
+                # ALGO = Damped, provided the wavefunction has been stored.
+                actions.append({"dict": "INCAR", "action": {"_set": {"ISMEAR": 0, "SIGMA": 0.05}}})
+                if v.incar.get("NEDOS") or v.incar.get("EMIN") or v.incar.get("EMAX"):
+                    warnings.warn(
+                        "This looks like a DOS run. You may want to follow-up this job with ALGO = Damped"
+                        " and ISMEAR = -5, using the wavefunction from the current job.",
+                        UserWarning,
+                    )
+            # NOTE: This is the amin error handler
+            # Sometimes an AMIN warning can appear with large unit cell dimensions, so we'll address it now
+            if np.max(v.final_structure.lattice.abc) > 50.0 and v.incar.get("AMIN", 0.1) > 0.01:
+                actions.append({"dict": "INCAR", "action": {"_set": {"AMIN": 0.01}}})
+
+            # If meta-GGA, go straight to Algo = All. Algo = All is recommended in the VASP
+            # manual and some meta-GGAs explicitly say to set Algo = All for proper convergence.
+            # I am using "--" as the check for METAGGA here because this is the default in the
+            # vasprun.xml file
+            if v.incar.get("METAGGA", "--") != "--" and algo != "all":
+                actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "All"}}})
+
+            # If a hybrid is used, do not set Algo = Fast or VeryFast. Hybrid calculations do not
+            # support these algorithms, but no warning is printed.
+            if v.incar.get("LHFCALC", False):
                 if algo != "all":
                     actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "All"}}})
                 # See the VASP manual section on LHFCALC for more information.
                 elif algo != "damped":
                     actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "Damped", "TIME": 0.5}}})
-            else:
+
+            # Ladder from VeryFast to Fast to Normal to All
+            # (except for meta-GGAs and hybrids).
+            # These progressively switch to more stable but more
+            # expensive algorithms.
+            if len(actions) == 0:
                 if algo == "veryfast":
                     actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "Fast"}}})
                 elif algo == "fast":
                     actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "Normal"}}})
                 elif algo == "normal":
                     actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "All"}}})
                 else:
@@ -1253,73 +1279,14 @@
                 }
             )
 
         VaspModder(vi=vi).apply_actions(actions)
         return {"errors": ["LargeSigma"], "actions": actions}
 
 
-@deprecated(
-    message="This handler is no longer supported and its use is no "
-    "longer recommended. It will be removed in v2020.x."
-)
-class MaxForceErrorHandler(ErrorHandler):
-    """
-    Checks that the desired force convergence has been achieved. Otherwise
-    restarts the run with smaller EDIFFG. (This is necessary since energy
-    and force convergence criteria cannot be set simultaneously)
-    """
-
-    is_monitor = False
-
-    def __init__(self, output_filename="vasprun.xml", max_force_threshold=0.25):
-        """
-        Args:
-            input_filename (str): name of the vasp INCAR file
-            output_filename (str): name to look for the vasprun
-            max_force_threshold (float): Threshold for max force for
-                restarting the run. (typically should be set to the value
-                that the creator looks for)
-        """
-        self.output_filename = output_filename
-        self.max_force_threshold = max_force_threshold
-
-    def check(self):
-        """
-        Check for error.
-        """
-        try:
-            v = Vasprun(self.output_filename)
-            forces = np.array(v.ionic_steps[-1]["forces"])
-            sdyn = v.final_structure.site_properties.get("selective_dynamics")
-            if sdyn:
-                forces[np.logical_not(sdyn)] = 0
-            max_force = max(np.linalg.norm(forces, axis=1))
-            if max_force > self.max_force_threshold and v.converged is True:
-                return True
-        except Exception:
-            pass
-        return False
-
-    def correct(self):
-        """
-        Perform corrections.
-        """
-        backup(VASP_BACKUP_FILES | {self.output_filename})
-        vi = VaspInput.from_directory(".")
-        ediff = vi["INCAR"].get("EDIFF", 1e-4)
-        ediffg = vi["INCAR"].get("EDIFFG", ediff * 10)
-        actions = [
-            {"file": "CONTCAR", "action": {"_file_copy": {"dest": "POSCAR"}}},
-            {"dict": "INCAR", "action": {"_set": {"EDIFFG": ediffg * 0.5}}},
-        ]
-        VaspModder(vi=vi).apply_actions(actions)
-
-        return {"errors": ["MaxForce"], "actions": actions}
-
-
 class PotimErrorHandler(ErrorHandler):
     """
     Check if a run has excessively large positive energy changes.
     This is typically caused by too large a POTIM. Runs typically
     end up crashing with some other error (e.g. BRMIX) as the geometry
     gets progressively worse.
     """
@@ -1470,55 +1437,78 @@
         """
         vi = VaspInput.from_directory(".")
         algo = vi["INCAR"].get("ALGO", "Normal").lower()
         amix = vi["INCAR"].get("AMIX", 0.4)
         bmix = vi["INCAR"].get("BMIX", 1.0)
         amin = vi["INCAR"].get("AMIN", 0.1)
         actions = []
+
+        # NOTE: This is the algo_tet handler response.
+        if (
+            vi["INCAR"].get("ALGO", "Normal").lower() in ["all", "damped"] or (50 <= vi["INCAR"].get("IALGO", 38) <= 59)
+        ) and vi["INCAR"].get("ISMEAR", 1) < 0:
+            # ALGO=All/Damped / IALGO=5X often fails with ISMEAR < 0. There are two options VASP
+            # suggests: 1) Use ISMEAR = 0 (and a small sigma) to get the SCF to converge.
+            # 2) Use ALGO = Damped but only *after* an ISMEAR = 0 run where the wavefunction
+            # has been stored and read in for the subsequent run.
+            #
+            # For simplicity, we go with Option 1 here, but if the user wants high-quality
+            # DOS then they should consider running a subsequent job with ISMEAR = -5 and
+            # ALGO = Damped, provided the wavefunction has been stored.
+            actions.append({"dict": "INCAR", "action": {"_set": {"ISMEAR": 0, "SIGMA": 0.05}}})
+            if vi["INCAR"].get("NEDOS") or vi["INCAR"].get("EMIN") or vi["INCAR"].get("EMAX"):
+                warnings.warn(
+                    "This looks like a DOS run. You may want to follow-up this job with ALGO = Damped"
+                    " and ISMEAR = -5, using the wavefunction from the current job.",
+                    UserWarning,
+                )
+
+        # NOTE: This is the amin error handler
+        # Sometimes an AMIN warning can appear with large unit cell dimensions, so we'll address it now
+        if np.max(Structure.from_file("CONTCAR").structure.lattice.abc) > 50.0 and amin > 0.01:
+            actions.append({"dict": "INCAR", "action": {"_set": {"AMIN": 0.01}}})
+
+        # If a hybrid is used, do not set Algo = Fast or VeryFast. Hybrid calculations do not
+        # support these algorithms, but no warning is printed.
+        # If meta-GGA, go straight to Algo = All. Algo = All is recommended in the VASP
+        # manual and some meta-GGAs explicitly say to set Algo = All for proper convergence.
+        # I am using "none" here because METAGGA is a string variable and this is the default
+        if (
+            vi["INCAR"].get("LHFCALC", False) or vi["INCAR"].get("METAGGA", "none").lower() != "none"
+        ) and algo != "all":
+            actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "All"}}})
+
         # Ladder from VeryFast to Fast to Normal to All
         # (except for meta-GGAs and hybrids).
         # These progressively switch to more stable but more
         # expensive algorithms.
-        if vi["INCAR"].get("METAGGA", "none").lower() != "none":
-            # If meta-GGA, go straight to Algo = All. Algo = All is recommended in the VASP
-            # manual and some meta-GGAs explicitly say to set Algo = All for proper convergence.
-            # I am using "none" here because METAGGA is a string variable and this is the default
-            if algo != "all":
-                actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "All"}}})
-        elif vi["INCAR"].get("LHFCALC", False):
-            # If a hybrid is used, do not set Algo = Fast or VeryFast. Hybrid calculations do not
-            # support these algorithms, but no warning is printed.
-            if algo != "all":
-                actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "All"}}})
-            # uncomment the line below for a backup option
-            # elif algo != "damped":
-            #     actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "Damped", "Time": 0.5}}})
-        else:
+        if len(actions) == 0:
             if algo == "veryfast":
                 actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "Fast"}}})
             elif algo == "fast":
                 actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "Normal"}}})
             elif algo == "normal":
                 actions.append({"dict": "INCAR", "action": {"_set": {"ALGO": "All"}}})
-            elif amix > 0.1 and bmix > 0.01:
-                # Try linear mixing
-                actions.append(
-                    {
-                        "dict": "INCAR",
-                        "action": {"_set": {"ALGO": "Normal", "AMIX": 0.1, "BMIX": 0.01, "ICHARG": 2}},
-                    }
-                )
-            elif bmix < 3.0 and amin > 0.01:
-                # Try increasing bmix
-                actions.append(
-                    {
-                        "dict": "INCAR",
-                        "action": {"_set": {"Algo": "Normal", "AMIN": 0.01, "BMIX": 3.0, "ICHARG": 2}},
-                    }
-                )
+            elif algo == "all":
+                if amix > 0.1 and bmix > 0.01:
+                    # Try linear mixing
+                    actions.append(
+                        {
+                            "dict": "INCAR",
+                            "action": {"_set": {"ALGO": "Normal", "AMIX": 0.1, "BMIX": 0.01, "ICHARG": 2}},
+                        }
+                    )
+                elif bmix < 3.0 and amin > 0.01:
+                    # Try increasing bmix
+                    actions.append(
+                        {
+                            "dict": "INCAR",
+                            "action": {"_set": {"Algo": "Normal", "AMIN": 0.01, "BMIX": 3.0, "ICHARG": 2}},
+                        }
+                    )
 
         if actions:
             backup(VASP_BACKUP_FILES)
             VaspModder(vi=vi).apply_actions(actions)
             return {"errors": ["Non-converging job"], "actions": actions}
         # Unfixable error. Just return None for actions.
         return {"errors": ["Non-converging job"], "actions": None}
```

### Comparing `custodian-2023.3.10/custodian/vasp/interpreter.py` & `custodian-2023.5.7/custodian/vasp/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/vasp/jobs.py` & `custodian-2023.5.7/custodian/vasp/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian/vasp/validators.py` & `custodian-2023.5.7/custodian/vasp/validators.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/custodian.egg-info/PKG-INFO` & `custodian-2023.5.7/custodian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custodian
-Version: 2023.3.10
+Version: 2023.5.7
 Summary: A simple JIT job management framework in Python.
 Home-page: https://github.com/materialsproject/custodian
 Author: Shyue Ping Ong, William Davidson Richards, Stephen Dacek, Xiaohui Qu, Matthew Horton, Samuel M. Blau
 Author-email: ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 License: MIT
 Keywords: jit,just-in-time,job,management,vasp
```

### Comparing `custodian-2023.3.10/custodian.egg-info/SOURCES.txt` & `custodian-2023.5.7/custodian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/setup.cfg` & `custodian-2023.5.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `custodian-2023.3.10/setup.py` & `custodian-2023.5.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_desc = f.read()
     ind = long_desc.find("\n")
     long_desc = long_desc[ind + 1 :]
 
 setup(
     name="custodian",
     packages=find_packages(),
-    version="2023.3.10",
+    version="2023.5.7",
     install_requires=["monty>=2.0.6", "ruamel.yaml>=0.15.6", "sentry-sdk>=0.8.0"],
     extras_require={"vasp, nwchem, qchem": ["pymatgen>=2019.8.23"]},
     package_data={},
     author="Shyue Ping Ong, William Davidson Richards, Stephen Dacek, Xiaohui Qu, Matthew Horton, Samuel M. Blau",
     author_email="ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     url="https://github.com/materialsproject/custodian",
```

