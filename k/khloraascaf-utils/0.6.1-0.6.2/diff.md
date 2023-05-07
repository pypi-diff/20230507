# Comparing `tmp/khloraascaf_utils-0.6.1.tar.gz` & `tmp/khloraascaf_utils-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf_utils-0.6.1.tar", last modified: Wed May  3 16:26:01 2023, max compression
+gzip compressed data, was "khloraascaf_utils-0.6.2.tar", last modified: Sun May  7 15:30:44 2023, max compression
```

## Comparing `khloraascaf_utils-0.6.1.tar` & `khloraascaf_utils-0.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:26:01.715077 khloraascaf_utils-0.6.1/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-03 16:25:36.000000 khloraascaf_utils-0.6.1/LICENCE
--rw-r--r--   0 root         (0) root         (0)    43838 2023-05-03 16:26:01.714077 khloraascaf_utils-0.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-03 16:25:36.000000 khloraascaf_utils-0.6.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-03 16:25:36.000000 khloraascaf_utils-0.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 16:26:01.715077 khloraascaf_utils-0.6.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:26:01.706077 khloraascaf_utils-0.6.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:26:01.710077 khloraascaf_utils-0.6.1/src/khloraascaf_utils/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-03 16:25:36.000000 khloraascaf_utils-0.6.1/src/khloraascaf_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8224 2023-05-03 16:25:36.000000 khloraascaf_utils-0.6.1/src/khloraascaf_utils/artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7169 2023-05-03 16:25:36.000000 khloraascaf_utils-0.6.1/src/khloraascaf_utils/asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-05-03 16:25:36.000000 khloraascaf_utils-0.6.1/src/khloraascaf_utils/contigs_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    13756 2023-05-03 16:25:36.000000 khloraascaf_utils-0.6.1/src/khloraascaf_utils/to_networkx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:26:01.713077 khloraascaf_utils-0.6.1/src/khloraascaf_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    43838 2023-05-03 16:26:01.000000 khloraascaf_utils-0.6.1/src/khloraascaf_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-03 16:26:01.000000 khloraascaf_utils-0.6.1/src/khloraascaf_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 16:26:01.000000 khloraascaf_utils-0.6.1/src/khloraascaf_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-03 16:26:01.000000 khloraascaf_utils-0.6.1/src/khloraascaf_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-03 16:26:01.000000 khloraascaf_utils-0.6.1/src/khloraascaf_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:26:01.714077 khloraascaf_utils-0.6.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4111 2023-05-03 16:25:36.000000 khloraascaf_utils-0.6.1/tests/test_artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3590 2023-05-03 16:25:36.000000 khloraascaf_utils-0.6.1/tests/test_asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     1770 2023-05-03 16:25:36.000000 khloraascaf_utils-0.6.1/tests/test_contigs_attributes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:30:44.045683 khloraascaf_utils-0.6.2/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-07 15:30:17.000000 khloraascaf_utils-0.6.2/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-05-07 15:30:44.044683 khloraascaf_utils-0.6.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-07 15:30:17.000000 khloraascaf_utils-0.6.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-07 15:30:17.000000 khloraascaf_utils-0.6.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 15:30:44.045683 khloraascaf_utils-0.6.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:30:44.037682 khloraascaf_utils-0.6.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:30:44.041682 khloraascaf_utils-0.6.2/src/khloraascaf_utils/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-07 15:30:17.000000 khloraascaf_utils-0.6.2/src/khloraascaf_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8224 2023-05-07 15:30:17.000000 khloraascaf_utils-0.6.2/src/khloraascaf_utils/artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7285 2023-05-07 15:30:17.000000 khloraascaf_utils-0.6.2/src/khloraascaf_utils/asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-05-07 15:30:17.000000 khloraascaf_utils-0.6.2/src/khloraascaf_utils/contigs_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    13756 2023-05-07 15:30:17.000000 khloraascaf_utils-0.6.2/src/khloraascaf_utils/to_networkx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:30:44.043682 khloraascaf_utils-0.6.2/src/khloraascaf_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-05-07 15:30:44.000000 khloraascaf_utils-0.6.2/src/khloraascaf_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-07 15:30:44.000000 khloraascaf_utils-0.6.2/src/khloraascaf_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 15:30:44.000000 khloraascaf_utils-0.6.2/src/khloraascaf_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-07 15:30:44.000000 khloraascaf_utils-0.6.2/src/khloraascaf_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-07 15:30:44.000000 khloraascaf_utils-0.6.2/src/khloraascaf_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:30:44.044683 khloraascaf_utils-0.6.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4111 2023-05-07 15:30:17.000000 khloraascaf_utils-0.6.2/tests/test_artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-05-07 15:30:17.000000 khloraascaf_utils-0.6.2/tests/test_asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2023-05-07 15:30:17.000000 khloraascaf_utils-0.6.2/tests/test_contigs_attributes.py
```

### Comparing `khloraascaf_utils-0.6.1/LICENCE` & `khloraascaf_utils-0.6.2/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.6.1/PKG-INFO` & `khloraascaf_utils-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf_utils
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf_utils-0.6.1/README.md` & `khloraascaf_utils-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.6.1/pyproject.toml` & `khloraascaf_utils-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf_utils"
-version = "0.6.1"
+version = "0.6.2"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "Python utilities for khloraascaf python package."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -17,15 +17,15 @@
     "Operating System :: Unix",
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 license = { file = "LICENCE" }
 requires-python = ">=3.9"
 dependencies = [
-    "khloraascaf >=1.5.1, <1.6",
+    "khloraascaf >=1.6.0, <1.7",
     "networkx >=3.0, <3.1",
     "biopython >=1.81, <1.82",
 ]
 
 [project.urls]
 
 Homepage = "https://gitlab.com/khloraa_scaffolding/khloraascaf_utils"
```

### Comparing `khloraascaf_utils-0.6.1/src/khloraascaf_utils/artificial_data.py` & `khloraascaf_utils-0.6.2/src/khloraascaf_utils/artificial_data.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.6.1/src/khloraascaf_utils/asm_graph_to_fasta.py` & `khloraascaf_utils-0.6.2/src/khloraascaf_utils/asm_graph_to_fasta.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,29 +36,30 @@
         """The Initialiser."""
         #
         # Canonical couple of oriented contig for each link id (forward)
         #
         self.__orc_link_to_id: dict[tuple[OrCT, OrCT], IdLT] = {}
         #
         # Sequence for each forward link identifier
-        #
+        # OPTIMIZE stop keeping in hard memory: index method?
         self.__link_sequences: dict[IdLT, Seq.Seq] = {}
 
         for link_id, c_id, c_or, d_id, d_or in read_contig_links_file(
                 contig_links_file):
             self.__orc_link_to_id[(c_id, c_or), (d_id, d_or)] = link_id
             self.__link_sequences[link_id] = Seq.Seq('')
 
         for record in SeqIO.parse(link_sequences_file, 'fasta'):
             if record.id not in self.__link_sequences:
                 raise KeyError(record.id)
             self.__link_sequences[record.id] = record.seq
         #
         # Sequence for each forward region
         #
+        # OPTIMIZE stop keeping in hard memory: index method?
         self.__region_sequences: list[Seq.Seq] = []
         #
         # For each region (forward) gives its oriented contig extremities
         #
         self.__region_orc_extrem: list[tuple[OrCT, OrCT]] = []
 
         self.__build_region_sequences(asm_graph, contig_sequences_file)
@@ -96,15 +97,17 @@
         -------
         Seq.Seq
             Nucletotide sequence
         """
         region_path_iter = iter(region_path)
         u_ind, u_or = next(region_path_iter)
         begin_ind, begin_or = u_ind, u_or
+
         path_sequence: Seq.Seq = self.region_sequence(u_ind, u_or)
+
         for v_ind, v_or in region_path_iter:
             # Add link sequence
             u_ext: OrCT = (
                 self.__region_orc_extrem[u_ind][1] if u_or == FORWARD_INT
                 else rev_oriented_contig(self.__region_orc_extrem[u_ind][0])
             )
             v_ext: OrCT = (
```

### Comparing `khloraascaf_utils-0.6.1/src/khloraascaf_utils/contigs_attributes.py` & `khloraascaf_utils-0.6.2/src/khloraascaf_utils/contigs_attributes.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.6.1/src/khloraascaf_utils/to_networkx.py` & `khloraascaf_utils-0.6.2/src/khloraascaf_utils/to_networkx.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.6.1/src/khloraascaf_utils.egg-info/PKG-INFO` & `khloraascaf_utils-0.6.2/src/khloraascaf_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf-utils
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf_utils-0.6.1/src/khloraascaf_utils.egg-info/SOURCES.txt` & `khloraascaf_utils-0.6.2/src/khloraascaf_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.6.1/tests/test_artificial_data.py` & `khloraascaf_utils-0.6.2/tests/test_artificial_data.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.6.1/tests/test_asm_graph_to_fasta.py` & `khloraascaf_utils-0.6.2/tests/test_asm_graph_to_fasta.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.6.1/tests/test_contigs_attributes.py` & `khloraascaf_utils-0.6.2/tests/test_contigs_attributes.py`

 * *Files identical despite different names*

