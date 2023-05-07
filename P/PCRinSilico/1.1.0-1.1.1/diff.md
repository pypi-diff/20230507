# Comparing `tmp/PCRinSilico-1.1.0.tar.gz` & `tmp/PCRinSilico-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PCRinSilico-1.1.0.tar", last modified: Sun May  7 09:46:33 2023, max compression
+gzip compressed data, was "PCRinSilico-1.1.1.tar", last modified: Sun May  7 10:02:56 2023, max compression
```

## Comparing `PCRinSilico-1.1.0.tar` & `PCRinSilico-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 09:46:33.116729 PCRinSilico-1.1.0/
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 09:46:33.115724 PCRinSilico-1.1.0/PCRinSilico/
--rw-r--r--   0 semiquant   (502) staff       (20)    10837 2023-05-07 09:44:05.000000 PCRinSilico-1.1.0/PCRinSilico/PCRinSilico.py
--rw-r--r--   0 semiquant   (502) staff       (20)        0 2023-05-07 07:39:24.000000 PCRinSilico-1.1.0/PCRinSilico/__init__.py
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 09:46:33.116397 PCRinSilico-1.1.0/PCRinSilico.egg-info/
--rw-r--r--   0 semiquant   (502) staff       (20)     4007 2023-05-07 09:46:32.000000 PCRinSilico-1.1.0/PCRinSilico.egg-info/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)      281 2023-05-07 09:46:33.000000 PCRinSilico-1.1.0/PCRinSilico.egg-info/SOURCES.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-07 09:46:32.000000 PCRinSilico-1.1.0/PCRinSilico.egg-info/dependency_links.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       61 2023-05-07 09:46:32.000000 PCRinSilico-1.1.0/PCRinSilico.egg-info/entry_points.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       17 2023-05-07 09:46:32.000000 PCRinSilico-1.1.0/PCRinSilico.egg-info/requires.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       12 2023-05-07 09:46:33.000000 PCRinSilico-1.1.0/PCRinSilico.egg-info/top_level.txt
--rw-r--r--   0 semiquant   (502) staff       (20)     4007 2023-05-07 09:46:33.116569 PCRinSilico-1.1.0/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)     3561 2023-05-07 09:43:48.000000 PCRinSilico-1.1.0/README.md
--rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-07 09:46:33.116777 PCRinSilico-1.1.0/setup.cfg
--rw-r--r--   0 semiquant   (502) staff       (20)     1955 2023-05-07 09:45:56.000000 PCRinSilico-1.1.0/setup.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 10:02:56.474017 PCRinSilico-1.1.1/
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 10:02:56.473005 PCRinSilico-1.1.1/PCRinSilico/
+-rw-r--r--   0 semiquant   (502) staff       (20)    10845 2023-05-07 10:02:33.000000 PCRinSilico-1.1.1/PCRinSilico/PCRinSilico.py
+-rw-r--r--   0 semiquant   (502) staff       (20)        0 2023-05-07 07:39:24.000000 PCRinSilico-1.1.1/PCRinSilico/__init__.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 10:02:56.473680 PCRinSilico-1.1.1/PCRinSilico.egg-info/
+-rw-r--r--   0 semiquant   (502) staff       (20)     4007 2023-05-07 10:02:56.000000 PCRinSilico-1.1.1/PCRinSilico.egg-info/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)      281 2023-05-07 10:02:56.000000 PCRinSilico-1.1.1/PCRinSilico.egg-info/SOURCES.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-07 10:02:56.000000 PCRinSilico-1.1.1/PCRinSilico.egg-info/dependency_links.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       61 2023-05-07 10:02:56.000000 PCRinSilico-1.1.1/PCRinSilico.egg-info/entry_points.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       17 2023-05-07 10:02:56.000000 PCRinSilico-1.1.1/PCRinSilico.egg-info/requires.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       12 2023-05-07 10:02:56.000000 PCRinSilico-1.1.1/PCRinSilico.egg-info/top_level.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)     4007 2023-05-07 10:02:56.473858 PCRinSilico-1.1.1/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)     3561 2023-05-07 09:43:48.000000 PCRinSilico-1.1.1/README.md
+-rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-07 10:02:56.474065 PCRinSilico-1.1.1/setup.cfg
+-rw-r--r--   0 semiquant   (502) staff       (20)     1955 2023-05-07 10:02:45.000000 PCRinSilico-1.1.1/setup.py
```

### Comparing `PCRinSilico-1.1.0/PCRinSilico/PCRinSilico.py` & `PCRinSilico-1.1.1/PCRinSilico/PCRinSilico.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     dimers = []
     melting_temps = []
 
     # Loop through all possible pairs of sequences
     for seq1, seq2 in itertools.combinations(seq_records, 2):
         # Calculate the melting temperature of the dimer
         # dimer_tm = MeltingTemp.Tm_NN(str(seq1.seq + seq2.seq), nn_table=MeltingTemp.DNA_NN4, Na=salt_conc, saltcorr=7)
-        tm = calc_tm(str(seq1.seq + seq2.seq))
+        dimer_tm = calc_tm(str(seq1.seq + seq2.seq))
 
         # Check if the dimer's melting temperature is above the given temperature
         if dimer_tm > temp:
             # Add the dimer's names and melting temperature to the lists
             dimers.append((seq1.id, seq2.id))
             melting_temps.append(round(dimer_tm))
 
@@ -210,15 +210,15 @@
         pr_seq = Seq(row['qseq2'])
     amplicon_seq = str(pf_seq) + str(amplicon_seq) + str(pr_seq)
     amplicons.append({'Forward_primer':  row['qseq1'], 'Reverse_primer':  row['qseq2'], 'amplicon_seq': amplicon_seq})
 
 
 tm_data = []
 for pair in itertools.combinations(amplicons, 2):
-    tm = MeltingTemp.Tm_NN(pair[0]['amplicon_seq'], pair[1]['amplicon_seq'], Na=salt_conc, saltcorr=7)
+    # tm = MeltingTemp.Tm_NN(pair[0]['amplicon_seq'], pair[1]['amplicon_seq'], Na=salt_conc, saltcorr=7)
     tm = calc_tm(seq=pair[0]['amplicon_seq'], seq2=pair[1]['amplicon_seq'])
     tm_data.append({"amplicon1_PF": pair[0]['Forward_primer'],
     "amplicon1_PR": pair[0]['Reverse_primer'],
     "amplicon2_PF": pair[1]['Forward_primer'],
     "amplicon2_PR": pair[1]['Reverse_primer'], 
     'tm': str(tm)})
```

### Comparing `PCRinSilico-1.1.0/PCRinSilico.egg-info/PKG-INFO` & `PCRinSilico-1.1.1/PCRinSilico.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PCRinSilico
-Version: 1.1.0
+Version: 1.1.1
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/inSilicoPCR
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Platform: UNKNOWN
```

### Comparing `PCRinSilico-1.1.0/PKG-INFO` & `PCRinSilico-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PCRinSilico
-Version: 1.1.0
+Version: 1.1.1
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/inSilicoPCR
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Platform: UNKNOWN
```

### Comparing `PCRinSilico-1.1.0/README.md` & `PCRinSilico-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PCRinSilico-1.1.0/setup.py` & `PCRinSilico-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         os.system("wget https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/2.14.0/ncbi-blast-2.14.0+-x64-linux.tar.gz")
         os.system("tar -xzvf ncbi-blast-2.11.0+-x64-linux.tar.gz")
         os.system("export PATH=$PATH:%s" % os.path.abspath("$(pwd)/ncbi-blast-2.11.0+/bin"))
 
 
 setup(
     name='PCRinSilico',
-    version='1.1.0',
+    version='1.1.1',
     url='https://github.com/SemiQuant/inSilicoPCR',
     install_requires=dependencies,
     description='In silico PCR tool',
     long_description=long_description,
     # long_description='This script takes a text file with primer sequence (one per line) and a reference FASTA file as input and identifies primer pairs which amplify a DNA sequence of length less than or equal to a user-specified maximum, at a given Tm and salt concentration. The script outputs the sequences of the primers, th eportion of the primer that binds, the number of mismatches, as well as the start and end coordinates of the amplified sequence.',
     long_description_content_type='text/markdown',
     author='Jason D Limberis',
```

