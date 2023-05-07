# Comparing `tmp/ebi_eva_common_pyutils-0.5.3.dev6.tar.gz` & `tmp/ebi_eva_common_pyutils-0.5.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebi_eva_common_pyutils-0.5.3.dev6.tar", last modified: Tue Apr 25 07:20:58 2023, max compression
+gzip compressed data, was "ebi_eva_common_pyutils-0.5.3.dev7.tar", last modified: Fri Apr 28 16:50:33 2023, max compression
```

## Comparing `ebi_eva_common_pyutils-0.5.3.dev6.tar` & `ebi_eva_common_pyutils-0.5.3.dev7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 07:20:58.553067 ebi_eva_common_pyutils-0.5.3.dev6/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1492 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/CHANGELOG.md
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    11357 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/LICENSE
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       28 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/MANIFEST.in
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      545 2023-04-25 07:20:58.553067 ebi_eva_common_pyutils-0.5.3.dev6/PKG-INFO
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1434 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/README.md
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 07:20:58.549067 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4984 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/archive_directory.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 07:20:58.553067 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/assembly/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       66 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/assembly/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1562 2023-04-25 06:44:42.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/assembly/assembly.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2151 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/command_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1192 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/common_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2242 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/config.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     7838 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/config_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 07:20:58.553067 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/contig_alias/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/contig_alias/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3056 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/contig_alias/contig_alias.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1452 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/ena_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1375 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/file_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4990 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/logger.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    14950 2023-04-25 06:14:55.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/metadata_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3589 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/mongo_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 07:20:58.553067 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/mongodb/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       72 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/mongodb/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     9676 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/mongodb/mongo_database.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4009 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/ncbi_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2285 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/network_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 07:20:58.553067 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/nextflow/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      120 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/nextflow/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    10114 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4398 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/pg_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 07:20:58.553067 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/reference/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      134 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/reference/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    12162 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/reference/assembly.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3911 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/reference/sequence.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     9540 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/spring_properties.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 07:20:58.553067 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/taxonomy/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/taxonomy/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2259 2023-04-23 09:52:55.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/taxonomy/taxonomy.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 07:20:58.553067 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/variation/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/variation/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3515 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/variation/assembly_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     5230 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/variation/contig_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 07:20:58.553067 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils.egg-info/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      545 2023-04-25 07:20:58.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1702 2023-04-25 07:20:58.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        1 2023-04-25 07:20:58.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       81 2023-04-25 07:20:58.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils.egg-info/requires.txt
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       23 2023-04-25 07:20:58.000000 ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils.egg-info/top_level.txt
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      225 2023-04-25 07:20:58.557067 ebi_eva_common_pyutils-0.5.3.dev6/setup.cfg
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      912 2023-04-25 07:17:48.000000 ebi_eva_common_pyutils-0.5.3.dev6/setup.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.663999 ebi_eva_common_pyutils-0.5.3.dev7/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1492 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/CHANGELOG.md
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    11357 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/LICENSE
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       28 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/MANIFEST.in
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      517 2023-04-28 16:50:33.663999 ebi_eva_common_pyutils-0.5.3.dev7/PKG-INFO
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1434 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/README.md
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.659999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4984 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/archive_directory.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.659999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/assembly/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       66 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/assembly/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1570 2023-04-28 09:52:41.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/assembly/assembly.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2151 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/command_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1192 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/common_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2242 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/config.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     8356 2023-04-28 16:29:30.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/config_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.659999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/contig_alias/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/contig_alias/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3056 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/contig_alias/contig_alias.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1452 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/ena_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1375 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/file_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4990 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/logger.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    14953 2023-04-28 09:52:41.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/metadata_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3589 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/mongo_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.659999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/mongodb/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       72 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/mongodb/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     9676 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/mongodb/mongo_database.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4859 2023-04-28 16:47:03.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/ncbi_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2285 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/network_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.659999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/nextflow/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      120 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/nextflow/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    10114 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4398 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/pg_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.663999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/reference/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      134 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/reference/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    12162 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/reference/assembly.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3911 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/reference/sequence.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    14310 2023-04-28 16:32:46.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/spring_properties.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.663999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/taxonomy/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/taxonomy/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2259 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/taxonomy/taxonomy.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.663999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/variation/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/variation/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3515 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/variation/assembly_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     5230 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/variation/contig_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.659999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      517 2023-04-28 16:50:33.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1699 2023-04-28 16:50:33.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        1 2023-04-28 16:50:33.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       81 2023-04-28 16:50:33.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/requires.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       23 2023-04-28 16:50:33.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      225 2023-04-28 16:50:33.663999 ebi_eva_common_pyutils-0.5.3.dev7/setup.cfg
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      912 2023-04-28 11:34:28.000000 ebi_eva_common_pyutils-0.5.3.dev7/setup.py
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/CHANGELOG.md` & `ebi_eva_common_pyutils-0.5.3.dev7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/LICENSE` & `ebi_eva_common_pyutils-0.5.3.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/PKG-INFO` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 Metadata-Version: 2.1
-Name: ebi_eva_common_pyutils
-Version: 0.5.3.dev6
+Name: ebi-eva-common-pyutils
+Version: 0.5.3.dev7
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/README.md` & `ebi_eva_common_pyutils-0.5.3.dev7/README.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/archive_directory.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/archive_directory.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/assembly/assembly.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/assembly/assembly.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,9 +25,9 @@
     logger.info(f'Query Ensembl for species name using taxonomy {tax_id}')
     scientific_name_api_param = get_scientific_name_from_ensembl(tax_id).lower().replace(' ', '_')
     ENSEMBL_REST_API_URL = "http://rest.ensembl.org/info/assembly/{0}?content-type=application/json".format(
         scientific_name_api_param)
     response = json_request(ENSEMBL_REST_API_URL)
     assembly_accession_attribute = 'assembly_accession'
     if assembly_accession_attribute in response:
-        return str(response.get('assembly_accession'))
+        return str(response.get(assembly_accession_attribute))
     return None
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/command_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/common_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/common_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/config.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/config.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/config_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/config_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,26 @@
     properties = get_properties_from_xml_file(profile_name, settings_xml_file)
     pg_url = properties['eva.accession.jdbc.url']
     pg_user = properties['eva.accession.user']
     pg_pass = properties['eva.accession.password']
     return pg_url, pg_user, pg_pass
 
 
+def get_variant_load_job_tracker_creds_for_profile(profile_name: str, settings_xml_file: str):
+    """
+    Gets host, username, and password for variant load job tracker database.
+    Useful for filling properties files.
+    """
+    properties = get_properties_from_xml_file(profile_name, settings_xml_file)
+    variant_url = properties['eva.variant.jdbc.url']
+    variant_user = properties['eva.variant.user']
+    variant_pass = properties['eva.variant.password']
+    return variant_url, variant_user, variant_pass
+
+
 def get_contig_alias_db_creds_for_profile(profile_name: str, settings_xml_file: str):
     """
     Gets url, username, and password for contig alias database.
 
     """
     properties = get_properties_from_xml_file(profile_name, settings_xml_file)
     contig_alias_url = properties['contig-alias.url']
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/contig_alias/contig_alias.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/contig_alias/contig_alias.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/ena_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/ena_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/file_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/logger.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/logger.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/metadata_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/metadata_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,30 +259,30 @@
 
 
 def add_to_supported_assemblies(metadata_connection_handle, source_of_assembly: str, target_assembly: str,
                                 taxonomy_id: int):
     today = datetime.date.today().strftime('%Y-%m-%d')
     # First check if the current assembly is already target - if so don't do anything
     current_query = (
-        f"SELECT assembly_id FROM evapro.supported_assembly_tracker "
+        f"SELECT assembly_id FROM {SUPPORTED_ASSEMBLY_TRACKER_TABLE} "
         f"WHERE taxonomy_id={taxonomy_id} AND current=true;"
     )
     results = get_all_results_for_query(metadata_connection_handle, current_query)
     if len(results) > 0 and results[0][0] == target_assembly:
         logger.warning(f'Current assembly for taxonomy {taxonomy_id} is already {target_assembly}!')
         return
 
     # Deprecate the last current assembly
     update_query = (
-        f"UPDATE evapro.supported_assembly_tracker "
+        f"UPDATE {SUPPORTED_ASSEMBLY_TRACKER_TABLE} "
         f"SET current=false, end_date='{today}' "
         f"WHERE taxonomy_id={taxonomy_id} AND current=true;"
     )
     execute_query(metadata_connection_handle, update_query)
 
     # Then insert the new assembly
     insert_query = (
-        f"INSERT INTO evapro.supported_assembly_tracker "
+        f"INSERT INTO {SUPPORTED_ASSEMBLY_TRACKER_TABLE} "
         f"(taxonomy_id, source, assembly_id, current, start_date) "
         f"VALUES({taxonomy_id}, '{source_of_assembly}', '{target_assembly}', true, '{today}');"
     )
     execute_query(metadata_connection_handle, insert_query)
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/mongo_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/mongo_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/mongodb/mongo_database.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/mongodb/mongo_database.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/ncbi_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/ncbi_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -90,7 +90,26 @@
     if match:
         rank = match.group(1)
     if rank not in ['species', 'subspecies']:
         logger.warning('Taxonomy id %s does not point to a species', taxid)
     match = re.search('<ScientificName>(.+?)</ScientificName>', r.text, re.MULTILINE)
     if match:
         return match.group(1)
+
+
+def get_species_name_from_ncbi(assembly_acc):
+    # We first need to search for the species associated with the assembly
+    assembly_dicts = get_ncbi_assembly_dicts_from_term(assembly_acc)
+    taxids = set([assembly_dict.get('taxid')
+        for assembly_dict in assembly_dicts
+        if assembly_dict.get('assemblyaccession') == assembly_acc or
+           assembly_dict.get('synonym', {}).get('genbank') == assembly_acc])
+
+    # This is a search so could retrieve multiple results
+    if len(taxids) != 1:
+        raise ValueError(f'Multiple species found for {assembly_acc}. '
+                         f'Cannot resolve single species for assembly {assembly_acc} in NCBI.')
+
+    taxonomy_id = taxids.pop()
+
+    scientific_name = retrieve_species_scientific_name_from_tax_id_ncbi(taxonomy_id)
+    return scientific_name.replace(' ', '_').lower()
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/network_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/network_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/pg_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/pg_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/reference/assembly.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/reference/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/reference/sequence.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/reference/sequence.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/spring_properties.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/spring_properties.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from collections import defaultdict
 
-from ebi_eva_common_pyutils.config_utils import get_primary_mongo_creds_for_profile, get_accession_pg_creds_for_profile, \
-    get_count_service_creds_for_profile, get_properties_from_xml_file
+from ebi_eva_common_pyutils.config_utils import get_primary_mongo_creds_for_profile, \
+    get_accession_pg_creds_for_profile, \
+    get_count_service_creds_for_profile, get_properties_from_xml_file, get_variant_load_job_tracker_creds_for_profile
 
 
 class SpringPropertiesGenerator:
     """
     Class to generate Spring properties for various Spring Batch pipelines.
     These methods can be used to generate complete properties files entirely in Python; alternatively, certain
     properties can be left unfilled and supplied as command-line arguments (e.g. by a NextFlow process).
@@ -48,141 +49,236 @@
         if param is None:
             return None
         elif not param:
             return ''
         else:
             return string.format(param)
 
-    def _common_properties(self, *, assembly_accession, read_preference='primary', chunk_size=100):
-        """Properties common to all Spring pipelines"""
+    def _mongo_properties(self):
         mongo_host, mongo_user, mongo_pass = get_primary_mongo_creds_for_profile(
             self.maven_profile, self.private_settings_file)
-        pg_url, pg_user, pg_pass = get_accession_pg_creds_for_profile(self.maven_profile, self.private_settings_file)
-        accession_db = get_properties_from_xml_file(
-            self.maven_profile, self.private_settings_file)['eva.accession.mongo.database']
         return {
-            'spring.datasource.driver-class-name': 'org.postgresql.Driver',
-            'spring.datasource.url': pg_url,
-            'spring.datasource.username': pg_user,
-            'spring.datasource.password': pg_pass,
-            'spring.datasource.tomcat.max-active': 3,
-            'spring.jpa.generate-ddl': 'true',
             'spring.data.mongodb.host': mongo_host,
             'spring.data.mongodb.port': 27017,
-            'spring.data.mongodb.database': accession_db,
             'spring.data.mongodb.username': mongo_user,
             'spring.data.mongodb.password': mongo_pass,
             'spring.data.mongodb.authentication-database': 'admin',
+        }
+
+    def _variant_load_job_tracker_properties(self):
+        variant_url, variant_user, variant_pass = get_variant_load_job_tracker_creds_for_profile(self.maven_profile,
+                                                                                                 self.private_settings_file)
+        return {
+            'job.repository.url': variant_url,
+            'job.repository.username': variant_user,
+            'job.repository.password': variant_pass,
+        }
+
+    def _count_stats_properties(self):
+        counts_url, counts_username, counts_password = get_count_service_creds_for_profile(
+            self.maven_profile, self.private_settings_file)
+        return {
+            'eva.count-stats.url': counts_url,
+            'eva.count-stats.username': counts_username,
+            'eva.count-stats.password': counts_password
+        }
+
+    def _common_properties(self, *, read_preference='primary', chunk_size=100):
+        """Properties common to all Spring pipelines"""
+        props = {
+            'spring.datasource.driver-class-name': 'org.postgresql.Driver',
+            'spring.datasource.tomcat.max-active': 3,
+            'spring.jpa.generate-ddl': 'true',
+
             'mongodb.read-preference': read_preference,
+
             'spring.main.web-application-type': 'none',
             'spring.main.allow-bean-definition-overriding': 'true',
-            'spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation': 'true',
+            'spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation': True,
+            'spring.jpa.properties.hibernate.temp.use_jdbc_metadata_defaults': False,
+            'spring.jpa.database-platform': 'org.hibernate.dialect.PostgreSQL9Dialect',
             'parameters.chunkSize': chunk_size,
+        }
+        merge = {**self._mongo_properties(), **self._count_stats_properties(), **props}
+        return merge
+
+    def _common_accessioning_properties(self, assembly_accession, read_preference, chunk_size):
+        pg_url, pg_user, pg_pass = get_accession_pg_creds_for_profile(self.maven_profile,
+                                                                               self.private_settings_file)
+        accession_db = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.accession.mongo.database']
+        props = {
+            'spring.datasource.url': pg_url,
+            'spring.datasource.username': pg_user,
+            'spring.datasource.password': pg_pass,
+            'spring.data.mongodb.database': accession_db,
             'parameters.assemblyAccession': assembly_accession,
         }
 
-    def _accessioning_properties(self, *, instance=''):
-        """Properties common to accessioning and clustering pipelines."""
-        counts_url, counts_username, counts_password = get_count_service_creds_for_profile(
-            self.maven_profile, self.private_settings_file)
+        merge = {**self._common_properties(read_preference=read_preference, chunk_size=chunk_size), **props}
+        return merge
 
-        return {
+    def _common_accessioning_clustering_properties(self, *, instance='', assembly_accession, read_preference, chunk_size):
+        """Properties common to accessioning and clustering pipelines."""
+        props = {
             'accessioning.instanceId': self._format_str('instance-{0}', instance),
             'accessioning.submitted.categoryId': 'ss',
             'accessioning.clustered.categoryId': 'rs',
             'accessioning.monotonic.ss.blockSize': 100000,
             'accessioning.monotonic.ss.blockStartValue': 5000000000,
             'accessioning.monotonic.ss.nextBlockInterval': 1000000000,
             'accessioning.monotonic.rs.blockSize': 100000,
             'accessioning.monotonic.rs.blockStartValue': 3000000000,
             'accessioning.monotonic.rs.nextBlockInterval': 1000000000,
-            'eva.count-stats.url': counts_url,
-            'eva.count-stats.username': counts_username,
-            'eva.count-stats.password': counts_password
         }
+        merge = {**self._common_accessioning_properties(assembly_accession, read_preference, chunk_size), **props}
+        return merge
 
-    def get_accessioning_properties(self, *, instance=None, target_assembly=None,  fasta=None, assembly_report=None,
+    def get_accessioning_properties(self, *, instance=None, target_assembly=None, fasta=None, assembly_report=None,
                                     project_accession=None, aggregation='BASIC', taxonomy_accession=None,
                                     vcf_file='', output_vcf='', chunk_size=100):
         """Properties for accessioning pipeline."""
         return self._format(
-            self._common_properties(assembly_accession=target_assembly, read_preference='secondaryPreferred',
-                                    chunk_size=chunk_size),
-            self._accessioning_properties(instance=instance),
+            self._common_accessioning_clustering_properties(instance=instance, assembly_accession=target_assembly,
+                                                            read_preference='secondaryPreferred', chunk_size=chunk_size),
             {
                 'spring.batch.job.names': 'CREATE_SUBSNP_ACCESSION_JOB',
                 'parameters.assemblyReportUrl': self._format_str('file:{0}', assembly_report),
                 'parameters.contigNaming': 'NO_REPLACEMENT',
                 'parameters.fasta': fasta,
                 'parameters.forceRestart': 'false',
                 'parameters.projectAccession': project_accession,
                 'parameters.taxonomyAccession': taxonomy_accession,
                 'parameters.vcfAggregation': aggregation,
                 'parameters.vcf': vcf_file,
                 'parameters.outputVcf': output_vcf
             },
         )
 
+    def get_clustering_properties(self, *, instance=None, read_preference='primary',
+                                  job_name=None, source_assembly='', target_assembly='', rs_report_path='', projects='',
+                                  project_accession='', vcf=''):
+        """Properties common to all clustering pipelines, though not all are always used."""
+        return self._format(
+            self._common_accessioning_clustering_properties(instance=instance, assembly_accession=target_assembly,
+                                                            read_preference=read_preference, chunk_size=100,
+                                                            ),
+            {
+                'spring.batch.job.names': job_name,
+                'parameters.remappedFrom': source_assembly,
+                'parameters.projects': projects,
+                'parameters.projectAccession': project_accession,
+                'parameters.vcf': vcf,
+                'parameters.rsReportPath': rs_report_path
+            }
+        )
+
     def get_remapping_extraction_properties(self, *, taxonomy=None, source_assembly=None, fasta=None,
                                             assembly_report=None,
                                             projects='', output_folder=None):
         """Properties for remapping extraction pipeline."""
         return self._format(
-            self._common_properties(assembly_accession=source_assembly, read_preference='secondaryPreferred',
-                                    chunk_size=1000),
+            self._common_accessioning_properties(assembly_accession=source_assembly,
+                                                 read_preference='secondaryPreferred',
+                                                 chunk_size=1000),
             {
                 'spring.batch.job.names': 'EXPORT_SUBMITTED_VARIANTS_JOB',
                 'parameters.taxonomy': taxonomy,
                 'parameters.fasta': fasta,
                 'parameters.assemblyReportUrl': self._format_str('file:{0}', assembly_report),
                 'parameters.projects': projects,
                 'parameters.outputFolder': output_folder
             })
 
     def get_remapping_ingestion_properties(self, *, source_assembly=None, target_assembly=None, vcf=None, load_to=None,
                                            remapping_version=1.0):
         """Properties for remapping ingestion pipeline."""
         return self._format(
-            self._common_properties(assembly_accession=target_assembly, read_preference='secondaryPreferred',
-                                    chunk_size=1000),
+            self._common_accessioning_properties(assembly_accession=target_assembly,
+                                                 read_preference='secondaryPreferred',
+                                                 chunk_size=1000),
             {
                 'spring.batch.job.names': 'INGEST_REMAPPED_VARIANTS_FROM_VCF_JOB',
                 'parameters.vcf': vcf,
                 'parameters.remappedFrom': source_assembly,
                 'parameters.loadTo': load_to,
                 'parameters.remappingVersion': remapping_version,
             }
         )
 
-    def get_clustering_properties(self, *, instance=None, read_preference='primary',
-                                  job_name=None, source_assembly='', target_assembly='', rs_report_path='', projects='',
-                                  project_accession='', vcf=''):
-        """Properties common to all clustering pipelines, though not all are always used."""
-        return self._format(
-            self._common_properties(assembly_accession=target_assembly, read_preference=read_preference,
-                                    chunk_size=100),
-            self._accessioning_properties(instance=instance),
-            {
-                'spring.batch.job.names': job_name,
-                'parameters.remappedFrom': source_assembly,
-                'parameters.projects': projects,
-                'parameters.projectAccession': project_accession,
-                'parameters.vcf': vcf,
-                'parameters.rsReportPath': rs_report_path
-            }
-        )
-
     def get_release_properties(self, *, job_name=None, assembly_accession=None, fasta=None, assembly_report=None,
                                contig_naming=None, output_folder=None, accessioned_vcf=None):
 
         return self._format(
-            self._common_properties(assembly_accession=assembly_accession, read_preference='secondaryPreferred',
-                                    chunk_size=1000),
+            self._common_accessioning_properties(assembly_accession=assembly_accession,
+                                                 read_preference='secondaryPreferred',
+                                                 chunk_size=1000),
             {
                 'spring.batch.job.names': job_name,
                 'parameters.contigNaming': contig_naming,
                 'parameters.fasta': fasta,
                 'parameters.assemblyReportUrl': self._format_str('file:{0}', assembly_report),
                 'parameters.outputFolder': output_folder,
                 'parameters.accessionedVcf': accessioned_vcf,
                 'logging.level.uk.ac.ebi.eva.accession.release': 'INFO'
             })
+
+    def _common_eva_pipeline_properties(self, opencga_path, read_preference='secondaryPreferred'):
+        variants_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.variants']
+        props = {
+            'spring.profiles.active': 'production,mongo',
+            'spring.profiles.include': 'variant-writer-mongo,variant-annotation-mongo',
+
+            'spring.data.mongodb.authentication-mechanism': 'SCRAM-SHA-1',
+            'job.repository.driverClassName': 'org.postgresql.Driver',
+
+            'db.collections.variants.name': variants_collection,
+
+            'app.opencga.path': opencga_path,
+            'config.restartability.allow': 'false',
+            'config.db.read-preference': read_preference,
+
+            'logging.level.embl.ebi.variation.eva': 'DEBUG',
+            'logging.level.org.opencb.opencga': 'DEBUG',
+            'logging.level.org.springframework': 'INFO',
+        }
+
+        merge = {**self._common_properties(read_preference=read_preference, chunk_size=100), **props}
+        return merge
+
+    def get_accession_import_properties(self, opencga_path, read_preference='secondaryPreferred'):
+        return self._format(self._common_eva_pipeline_properties(opencga_path, read_preference))
+
+    def get_variant_load_properties(self, project_accession, study_name, output_dir, annotation_dir, stats_dir,
+                                    vep_cache_path, opencga_path, read_preference='secondaryPreferred'):
+        files_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.files']
+        annotation_metadata_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.annotation-metadata']
+        annotation_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.annotations']
+        return self._format(
+            self._common_eva_pipeline_properties(opencga_path, read_preference),
+            self._variant_load_job_tracker_properties(),
+            {
+                'db.collections.files.name': files_collection,
+                'db.collections.annotation-metadata.name': annotation_metadata_collection,
+                'db.collections.annotations.name': annotation_collection,
+
+                'annotation.overwrite': False,
+                'app.vep.cache.path': vep_cache_path,
+                'app.vep.num-forks': 4,
+                'app.vep.timeout': 500,
+                'config.chunk.size': 200,
+
+                'input.study.id': project_accession,
+                'input.study.name': study_name,
+                'input.study.type': 'COLLECTION',
+
+                'output.dir': str(output_dir),
+                'output.dir.annotation': str(annotation_dir),
+                'output.dir.statistics': str(stats_dir),
+
+                'statistics.skip': False
+            },
+        )
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/taxonomy/taxonomy.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/taxonomy/taxonomy.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/variation/assembly_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/variation/assembly_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils/variation/contig_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/variation/contig_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/ebi_eva_common_pyutils.egg-info/SOURCES.txt` & `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-/data/sundarvenkata_work/EVA3208/eva-common-pyutils/ebi_eva_common_pyutils/archive_directory.py
+/home/nkumar2/PycharmProjects/eva-common-pyutils/ebi_eva_common_pyutils/archive_directory.py
 ebi_eva_common_pyutils/__init__.py
 ebi_eva_common_pyutils/archive_directory.py
 ebi_eva_common_pyutils/command_utils.py
 ebi_eva_common_pyutils/common_utils.py
 ebi_eva_common_pyutils/config.py
 ebi_eva_common_pyutils/config_utils.py
 ebi_eva_common_pyutils/ena_utils.py
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev6/setup.py` & `ebi_eva_common_pyutils-0.5.3.dev7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages
 
 setup(
     name='ebi_eva_common_pyutils',
     scripts=[os.path.join(os.path.dirname(__file__), 'ebi_eva_common_pyutils', 'archive_directory.py')],
     packages=find_packages(),
-    version='0.5.3.dev6',
+    version='0.5.3-dev7',
     license='Apache',
     description='EBI EVA - Common Python Utilities',
     url='https://github.com/EBIVariation/eva-common-pyutils',
     keywords=['EBI', 'EVA', 'PYTHON', 'UTILITIES'],
     install_requires=['psycopg2-binary', 'requests', 'pymongo', 'lxml', 'pyyaml', 'cached-property', 'retry',
                       'networkx<=2.5'],
     classifiers=[
```

