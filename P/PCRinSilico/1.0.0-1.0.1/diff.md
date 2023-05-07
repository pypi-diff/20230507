# Comparing `tmp/PCRinSilico-1.0.0.tar.gz` & `tmp/PCRinSilico-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PCRinSilico-1.0.0.tar", last modified: Sun May  7 07:00:42 2023, max compression
+gzip compressed data, was "PCRinSilico-1.0.1.tar", last modified: Sun May  7 07:16:00 2023, max compression
```

## Comparing `PCRinSilico-1.0.0.tar` & `PCRinSilico-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 07:00:42.187438 PCRinSilico-1.0.0/
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 07:00:42.186363 PCRinSilico-1.0.0/PCRinSilico/
--rw-r--r--   0 semiquant   (502) staff       (20)    10153 2023-05-05 22:30:45.000000 PCRinSilico-1.0.0/PCRinSilico/inSilicoPCR.py
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 07:00:42.187100 PCRinSilico-1.0.0/PCRinSilico.egg-info/
--rw-r--r--   0 semiquant   (502) staff       (20)     3898 2023-05-07 07:00:41.000000 PCRinSilico-1.0.0/PCRinSilico.egg-info/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)      257 2023-05-07 07:00:42.000000 PCRinSilico-1.0.0/PCRinSilico.egg-info/SOURCES.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-07 07:00:41.000000 PCRinSilico-1.0.0/PCRinSilico.egg-info/dependency_links.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       61 2023-05-07 07:00:41.000000 PCRinSilico-1.0.0/PCRinSilico.egg-info/entry_points.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       17 2023-05-07 07:00:42.000000 PCRinSilico-1.0.0/PCRinSilico.egg-info/requires.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       12 2023-05-07 07:00:42.000000 PCRinSilico-1.0.0/PCRinSilico.egg-info/top_level.txt
--rw-r--r--   0 semiquant   (502) staff       (20)     3898 2023-05-07 07:00:42.187288 PCRinSilico-1.0.0/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)     3452 2023-05-07 06:59:51.000000 PCRinSilico-1.0.0/README.md
--rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-07 07:00:42.187488 PCRinSilico-1.0.0/setup.cfg
--rw-r--r--   0 semiquant   (502) staff       (20)     1955 2023-05-07 06:59:44.000000 PCRinSilico-1.0.0/setup.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 07:16:00.606500 PCRinSilico-1.0.1/
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 07:16:00.605298 PCRinSilico-1.0.1/PCRinSilico/
+-rw-r--r--   0 semiquant   (502) staff       (20)    10153 2023-05-07 07:09:44.000000 PCRinSilico-1.0.1/PCRinSilico/PCRinSilico.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 07:16:00.606107 PCRinSilico-1.0.1/PCRinSilico.egg-info/
+-rw-r--r--   0 semiquant   (502) staff       (20)     3909 2023-05-07 07:16:00.000000 PCRinSilico-1.0.1/PCRinSilico.egg-info/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)      257 2023-05-07 07:16:00.000000 PCRinSilico-1.0.1/PCRinSilico.egg-info/SOURCES.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-07 07:16:00.000000 PCRinSilico-1.0.1/PCRinSilico.egg-info/dependency_links.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       61 2023-05-07 07:16:00.000000 PCRinSilico-1.0.1/PCRinSilico.egg-info/entry_points.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       17 2023-05-07 07:16:00.000000 PCRinSilico-1.0.1/PCRinSilico.egg-info/requires.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       12 2023-05-07 07:16:00.000000 PCRinSilico-1.0.1/PCRinSilico.egg-info/top_level.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)     3909 2023-05-07 07:16:00.606336 PCRinSilico-1.0.1/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)     3463 2023-05-07 07:09:38.000000 PCRinSilico-1.0.1/README.md
+-rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-07 07:16:00.606549 PCRinSilico-1.0.1/setup.cfg
+-rw-r--r--   0 semiquant   (502) staff       (20)     1955 2023-05-07 07:10:04.000000 PCRinSilico-1.0.1/setup.py
```

### Comparing `PCRinSilico-1.0.0/PCRinSilico/inSilicoPCR.py` & `PCRinSilico-1.0.1/PCRinSilico/PCRinSilico.py`

 * *Files identical despite different names*

### Comparing `PCRinSilico-1.0.0/PCRinSilico.egg-info/PKG-INFO` & `PCRinSilico-1.0.1/PCRinSilico.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PCRinSilico
-Version: 1.0.0
+Version: 1.0.1
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/inSilicoPCR
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Platform: UNKNOWN
@@ -27,21 +27,21 @@
 -   [Biopython](https://biopython.org/)
 -   [pandas](https://pandas.pydata.org/)
 -   [BLAST+](https://www.ncbi.nlm.nih.gov/books/NBK569861/)
 
 These may be installed by running
 
 ```
-pip install 
+pip install PCRinSilico
 ```
 
 ### Usage
 
 ```
-inSilicoPCR [options]
+PCRinSilico [options]
    --primer_seq [path to primer sequence file, one primer per line]
    --ref_fasta_file [path to reference FASTA file]
 ```
 
 ### Options
 
 | Argument              | Description                                                  | Default      |
@@ -52,15 +52,15 @@
 | `--req_five`           | Require the 5' end of the primer to bind?                      | True         |
 | `--out_file`           | Output file name.                                             | "in_silico_PCR" |
 
 
 ### Example
 
 ```
-inSilicoPCR \
+PCRinSilico \
    --primer_seq ./example/primers.txt \
    --ref_fasta_file  ./example/ref.fasta
 ```
 
 #### in_silico_PCR.tsv
 | qseq1   | qseq2_input          | qstart1 | qend1 | direction1 | mismatch2 | qseq2 | qseq1_input   | qstart2 | qend2 | direction2 | mismatch1 | binding_pos_diff | reference | ref_region |
 |---------|----------------------|---------|-------|------------|-----------|-------|---------------|---------|-------|------------|-----------|------------------|-----------|------------|
```

### Comparing `PCRinSilico-1.0.0/PKG-INFO` & `PCRinSilico-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PCRinSilico
-Version: 1.0.0
+Version: 1.0.1
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/inSilicoPCR
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Platform: UNKNOWN
@@ -27,21 +27,21 @@
 -   [Biopython](https://biopython.org/)
 -   [pandas](https://pandas.pydata.org/)
 -   [BLAST+](https://www.ncbi.nlm.nih.gov/books/NBK569861/)
 
 These may be installed by running
 
 ```
-pip install 
+pip install PCRinSilico
 ```
 
 ### Usage
 
 ```
-inSilicoPCR [options]
+PCRinSilico [options]
    --primer_seq [path to primer sequence file, one primer per line]
    --ref_fasta_file [path to reference FASTA file]
 ```
 
 ### Options
 
 | Argument              | Description                                                  | Default      |
@@ -52,15 +52,15 @@
 | `--req_five`           | Require the 5' end of the primer to bind?                      | True         |
 | `--out_file`           | Output file name.                                             | "in_silico_PCR" |
 
 
 ### Example
 
 ```
-inSilicoPCR \
+PCRinSilico \
    --primer_seq ./example/primers.txt \
    --ref_fasta_file  ./example/ref.fasta
 ```
 
 #### in_silico_PCR.tsv
 | qseq1   | qseq2_input          | qstart1 | qend1 | direction1 | mismatch2 | qseq2 | qseq1_input   | qstart2 | qend2 | direction2 | mismatch1 | binding_pos_diff | reference | ref_region |
 |---------|----------------------|---------|-------|------------|-----------|-------|---------------|---------|-------|------------|-----------|------------------|-----------|------------|
```

### Comparing `PCRinSilico-1.0.0/README.md` & `PCRinSilico-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 -   [Biopython](https://biopython.org/)
 -   [pandas](https://pandas.pydata.org/)
 -   [BLAST+](https://www.ncbi.nlm.nih.gov/books/NBK569861/)
 
 These may be installed by running
 
 ```
-pip install 
+pip install PCRinSilico
 ```
 
 ### Usage
 
 ```
-inSilicoPCR [options]
+PCRinSilico [options]
    --primer_seq [path to primer sequence file, one primer per line]
    --ref_fasta_file [path to reference FASTA file]
 ```
 
 ### Options
 
 | Argument              | Description                                                  | Default      |
@@ -37,15 +37,15 @@
 | `--req_five`           | Require the 5' end of the primer to bind?                      | True         |
 | `--out_file`           | Output file name.                                             | "in_silico_PCR" |
 
 
 ### Example
 
 ```
-inSilicoPCR \
+PCRinSilico \
    --primer_seq ./example/primers.txt \
    --ref_fasta_file  ./example/ref.fasta
 ```
 
 #### in_silico_PCR.tsv
 | qseq1   | qseq2_input          | qstart1 | qend1 | direction1 | mismatch2 | qseq2 | qseq1_input   | qstart2 | qend2 | direction2 | mismatch1 | binding_pos_diff | reference | ref_region |
 |---------|----------------------|---------|-------|------------|-----------|-------|---------------|---------|-------|------------|-----------|------------------|-----------|------------|
```

### Comparing `PCRinSilico-1.0.0/setup.py` & `PCRinSilico-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         os.system("wget https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/2.14.0/ncbi-blast-2.14.0+-x64-linux.tar.gz")
         os.system("tar -xzvf ncbi-blast-2.11.0+-x64-linux.tar.gz")
         os.system("export PATH=$PATH:%s" % os.path.abspath("$(pwd)/ncbi-blast-2.11.0+/bin"))
 
 
 setup(
     name='PCRinSilico',
-    version='1.0.0',
+    version='1.0.1',
     url='https://github.com/SemiQuant/inSilicoPCR',
     install_requires=dependencies,
     description='In silico PCR tool',
     long_description=long_description,
     # long_description='This script takes a text file with primer sequence (one per line) and a reference FASTA file as input and identifies primer pairs which amplify a DNA sequence of length less than or equal to a user-specified maximum, at a given Tm and salt concentration. The script outputs the sequences of the primers, th eportion of the primer that binds, the number of mismatches, as well as the start and end coordinates of the amplified sequence.',
     long_description_content_type='text/markdown',
     author='Jason D Limberis',
```

