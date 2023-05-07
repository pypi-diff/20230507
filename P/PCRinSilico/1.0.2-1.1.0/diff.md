# Comparing `tmp/PCRinSilico-1.0.2.tar.gz` & `tmp/PCRinSilico-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PCRinSilico-1.0.2.tar", last modified: Sun May  7 07:35:44 2023, max compression
+gzip compressed data, was "PCRinSilico-1.1.0.tar", last modified: Sun May  7 09:46:33 2023, max compression
```

## Comparing `PCRinSilico-1.0.2.tar` & `PCRinSilico-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 07:35:44.806016 PCRinSilico-1.0.2/
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 07:35:44.804939 PCRinSilico-1.0.2/PCRinSilico/
--rw-r--r--   0 semiquant   (502) staff       (20)    10166 2023-05-07 07:34:07.000000 PCRinSilico-1.0.2/PCRinSilico/PCRinSilico.py
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 07:35:44.805669 PCRinSilico-1.0.2/PCRinSilico.egg-info/
--rw-r--r--   0 semiquant   (502) staff       (20)     3909 2023-05-07 07:35:44.000000 PCRinSilico-1.0.2/PCRinSilico.egg-info/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)      257 2023-05-07 07:35:44.000000 PCRinSilico-1.0.2/PCRinSilico.egg-info/SOURCES.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-07 07:35:44.000000 PCRinSilico-1.0.2/PCRinSilico.egg-info/dependency_links.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       61 2023-05-07 07:35:44.000000 PCRinSilico-1.0.2/PCRinSilico.egg-info/entry_points.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       17 2023-05-07 07:35:44.000000 PCRinSilico-1.0.2/PCRinSilico.egg-info/requires.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       12 2023-05-07 07:35:44.000000 PCRinSilico-1.0.2/PCRinSilico.egg-info/top_level.txt
--rw-r--r--   0 semiquant   (502) staff       (20)     3909 2023-05-07 07:35:44.805844 PCRinSilico-1.0.2/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)     3463 2023-05-07 07:09:38.000000 PCRinSilico-1.0.2/README.md
--rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-07 07:35:44.806070 PCRinSilico-1.0.2/setup.cfg
--rw-r--r--   0 semiquant   (502) staff       (20)     1955 2023-05-07 07:34:26.000000 PCRinSilico-1.0.2/setup.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 09:46:33.116729 PCRinSilico-1.1.0/
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 09:46:33.115724 PCRinSilico-1.1.0/PCRinSilico/
+-rw-r--r--   0 semiquant   (502) staff       (20)    10837 2023-05-07 09:44:05.000000 PCRinSilico-1.1.0/PCRinSilico/PCRinSilico.py
+-rw-r--r--   0 semiquant   (502) staff       (20)        0 2023-05-07 07:39:24.000000 PCRinSilico-1.1.0/PCRinSilico/__init__.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 09:46:33.116397 PCRinSilico-1.1.0/PCRinSilico.egg-info/
+-rw-r--r--   0 semiquant   (502) staff       (20)     4007 2023-05-07 09:46:32.000000 PCRinSilico-1.1.0/PCRinSilico.egg-info/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)      281 2023-05-07 09:46:33.000000 PCRinSilico-1.1.0/PCRinSilico.egg-info/SOURCES.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-07 09:46:32.000000 PCRinSilico-1.1.0/PCRinSilico.egg-info/dependency_links.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       61 2023-05-07 09:46:32.000000 PCRinSilico-1.1.0/PCRinSilico.egg-info/entry_points.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       17 2023-05-07 09:46:32.000000 PCRinSilico-1.1.0/PCRinSilico.egg-info/requires.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       12 2023-05-07 09:46:33.000000 PCRinSilico-1.1.0/PCRinSilico.egg-info/top_level.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)     4007 2023-05-07 09:46:33.116569 PCRinSilico-1.1.0/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)     3561 2023-05-07 09:43:48.000000 PCRinSilico-1.1.0/README.md
+-rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-07 09:46:33.116777 PCRinSilico-1.1.0/setup.cfg
+-rw-r--r--   0 semiquant   (502) staff       (20)     1955 2023-05-07 09:45:56.000000 PCRinSilico-1.1.0/setup.py
```

### Comparing `PCRinSilico-1.0.2/PCRinSilico/PCRinSilico.py` & `PCRinSilico-1.1.0/PCRinSilico/PCRinSilico.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 parser.add_argument('--annealing_temp', type=int, help='Annealing temperature (in Celsius)', default = 60.0)
 parser.add_argument('--salt_concentration', type=float, help='Salt concentration (in nM)', default = 50)
 parser.add_argument('--max_amplicon_len', type=float, help='maximum length of PCR products in nucleotides', default = 2000)
 parser.add_argument('--req_five', type=str, help="Require the 5' end of the primer to bind?", default = True)
 parser.add_argument('--primer_seq', type=str, help="Primer sequences, one per line", required = True)
 parser.add_argument('--ref_fasta_file', type=str, help="Reference fasta file", required = True)
 parser.add_argument('--out_file', type=str, help="Output file name", default = "in_silico_PCR")
+parser.add_argument('--Q5', action='store_true', help='Whether to use Q5 approximation settings for Tm calculations.', default=True)
 
 # check if blastn is in the system path
 try:
     status = os.system('which blastn > /dev/null 2>&1')
     if status != 0:
         print('Error: BLAST is not installed.')
         exit(1)
@@ -38,14 +39,21 @@
 salt_conc = args.salt_concentration
 max_amplicon_len = args.max_amplicon_len
 req_five = args.req_five
 primer_seq = args.primer_seq
 ref_fasta_file = args.ref_fasta_file
 out_file = args.out_file
 
+def calc_tm(seq, seq2='', Q5=args.Q5):
+    if Q5:
+        tm = MeltingTemp.Tm_NN(seq, seq2, nn_table=MeltingTemp.DNA_NN4, dnac1=2500, dnac2=2500, Na=40, K=0, Tris=0, Mg=0.4, dNTPs=0, saltcorr=5.0)
+    else:
+        tm = MeltingTemp.Tm_NN(seq, seq2, Na=salt_conc, dnac1=250, dnac2=0, saltcorr=7, nn_table=MeltingTemp.DNA_NN4, selfcomp=False, check=True, shift=0.0)
+
+    return tm
 
 def find_binding_positions(primer_seq, ref_fasta_file, annealing_temp, req_five, salt_conc):
     # Run BLAST to search for primer sequence against reference FASTA
     blast_cmd = f"blastn -query {primer_seq} -subject {ref_fasta_file} -task blastn-short -outfmt '6 qseqid sseqid qstart qend sstart send qseq sseq mismatch length' > blast_output.txt"
     os.system(blast_cmd)
     
     blast_df = pd.DataFrame(columns=['Query ID', 'Subject ID', 'Query Start', 'Query End', 'Subject Start', 'Subject End', 'Query Sequence Match', 'Direction', 'Binding Position', 'Mismatches', 'Binding Length'])
@@ -55,15 +63,16 @@
             fields = line.strip().split('\t')
             qseqid, sseqid, qstart, qend, sstart, send, qseq, sseq, mismatch, length = fields
             direction = '+' if int(sstart) < int(send) else '-'
             binding_pos = sstart if direction == '+' else send
             # Check if primer binds at the specified annealing temperature
             if req_five and int(qstart) >= 2:
                 continue
-            tm = MeltingTemp.Tm_NN(Seq(sseq), Na=salt_conc, dnac1=250, dnac2=0, saltcorr=7, nn_table=MeltingTemp.DNA_NN4, selfcomp=False, check=True, shift=0.0)
+            # tm = MeltingTemp.Tm_NN(Seq(sseq), Na=salt_conc, dnac1=250, dnac2=0, saltcorr=7, nn_table=MeltingTemp.DNA_NN4, selfcomp=False, check=True, shift=0.0)
+            tm = calc_tm(Seq(sseq))
             if annealing_temp <= tm:
                 blast_df.loc[len(blast_df)] = [qseqid, sseqid, qstart, qend, sstart, send, sseq, direction, binding_pos, mismatch, length]
     return blast_df
 
 def find_compatible_pairs(blast_df, max_len):
     pairs = itertools.combinations(blast_df.index, 2)
     compatible_pairs = []
@@ -89,15 +98,16 @@
     # Create a list to hold the dimer pairs and melting temperatures
     dimers = []
     melting_temps = []
 
     # Loop through all possible pairs of sequences
     for seq1, seq2 in itertools.combinations(seq_records, 2):
         # Calculate the melting temperature of the dimer
-        dimer_tm = MeltingTemp.Tm_NN(str(seq1.seq + seq2.seq), nn_table=MeltingTemp.DNA_NN4, Na=salt_conc, saltcorr=7)
+        # dimer_tm = MeltingTemp.Tm_NN(str(seq1.seq + seq2.seq), nn_table=MeltingTemp.DNA_NN4, Na=salt_conc, saltcorr=7)
+        tm = calc_tm(str(seq1.seq + seq2.seq))
 
         # Check if the dimer's melting temperature is above the given temperature
         if dimer_tm > temp:
             # Add the dimer's names and melting temperature to the lists
             dimers.append((seq1.id, seq2.id))
             melting_temps.append(round(dimer_tm))
 
@@ -201,15 +211,16 @@
     amplicon_seq = str(pf_seq) + str(amplicon_seq) + str(pr_seq)
     amplicons.append({'Forward_primer':  row['qseq1'], 'Reverse_primer':  row['qseq2'], 'amplicon_seq': amplicon_seq})
 
 
 tm_data = []
 for pair in itertools.combinations(amplicons, 2):
     tm = MeltingTemp.Tm_NN(pair[0]['amplicon_seq'], pair[1]['amplicon_seq'], Na=salt_conc, saltcorr=7)
-    tm_data.append({    "amplicon1_PF": pair[0]['Forward_primer'],
+    tm = calc_tm(seq=pair[0]['amplicon_seq'], seq2=pair[1]['amplicon_seq'])
+    tm_data.append({"amplicon1_PF": pair[0]['Forward_primer'],
     "amplicon1_PR": pair[0]['Reverse_primer'],
     "amplicon2_PF": pair[1]['Forward_primer'],
     "amplicon2_PR": pair[1]['Reverse_primer'], 
     'tm': str(tm)})
 
 tm_df = pd.DataFrame(tm_data)
 print("Writing output to " + out_file + '_amplicon_interactions.tsv')
```

### Comparing `PCRinSilico-1.0.2/PCRinSilico.egg-info/PKG-INFO` & `PCRinSilico-1.1.0/PCRinSilico.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PCRinSilico
-Version: 1.0.2
+Version: 1.1.0
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/inSilicoPCR
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Platform: UNKNOWN
@@ -43,18 +43,19 @@
 ```
 
 ### Options
 
 | Argument              | Description                                                  | Default      |
 |-----------------------|--------------------------------------------------------------|--------------|
 | `--annealing_temp`     | Annealing temperature (in Celsius).                           | 60.0         |
-| `--salt_concentration` | Salt concentration (in nM).                                   | 50           |
+| `--salt_concentration` | Salt concentration (in nM, Ignored if Q5 True).               | 50           |
 | `--max_amplicon_len`   | Maximum length of PCR products in nucleotides.                | 2000         |
 | `--req_five`           | Require the 5' end of the primer to bind?                      | True         |
 | `--out_file`           | Output file name.                                             | "in_silico_PCR" |
+| `--Q5`           | Use Q5 approximation settings for Tm calculations?                | "True" |
 
 
 ### Example
 
 ```
 PCRinSilico \
    --primer_seq ./example/primers.txt \
```

### Comparing `PCRinSilico-1.0.2/PKG-INFO` & `PCRinSilico-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PCRinSilico
-Version: 1.0.2
+Version: 1.1.0
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/inSilicoPCR
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Platform: UNKNOWN
@@ -43,18 +43,19 @@
 ```
 
 ### Options
 
 | Argument              | Description                                                  | Default      |
 |-----------------------|--------------------------------------------------------------|--------------|
 | `--annealing_temp`     | Annealing temperature (in Celsius).                           | 60.0         |
-| `--salt_concentration` | Salt concentration (in nM).                                   | 50           |
+| `--salt_concentration` | Salt concentration (in nM, Ignored if Q5 True).               | 50           |
 | `--max_amplicon_len`   | Maximum length of PCR products in nucleotides.                | 2000         |
 | `--req_five`           | Require the 5' end of the primer to bind?                      | True         |
 | `--out_file`           | Output file name.                                             | "in_silico_PCR" |
+| `--Q5`           | Use Q5 approximation settings for Tm calculations?                | "True" |
 
 
 ### Example
 
 ```
 PCRinSilico \
    --primer_seq ./example/primers.txt \
```

### Comparing `PCRinSilico-1.0.2/README.md` & `PCRinSilico-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 ```
 
 ### Options
 
 | Argument              | Description                                                  | Default      |
 |-----------------------|--------------------------------------------------------------|--------------|
 | `--annealing_temp`     | Annealing temperature (in Celsius).                           | 60.0         |
-| `--salt_concentration` | Salt concentration (in nM).                                   | 50           |
+| `--salt_concentration` | Salt concentration (in nM, Ignored if Q5 True).               | 50           |
 | `--max_amplicon_len`   | Maximum length of PCR products in nucleotides.                | 2000         |
 | `--req_five`           | Require the 5' end of the primer to bind?                      | True         |
 | `--out_file`           | Output file name.                                             | "in_silico_PCR" |
+| `--Q5`           | Use Q5 approximation settings for Tm calculations?                | "True" |
 
 
 ### Example
 
 ```
 PCRinSilico \
    --primer_seq ./example/primers.txt \
```

### Comparing `PCRinSilico-1.0.2/setup.py` & `PCRinSilico-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         os.system("wget https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/2.14.0/ncbi-blast-2.14.0+-x64-linux.tar.gz")
         os.system("tar -xzvf ncbi-blast-2.11.0+-x64-linux.tar.gz")
         os.system("export PATH=$PATH:%s" % os.path.abspath("$(pwd)/ncbi-blast-2.11.0+/bin"))
 
 
 setup(
     name='PCRinSilico',
-    version='1.0.2',
+    version='1.1.0',
     url='https://github.com/SemiQuant/inSilicoPCR',
     install_requires=dependencies,
     description='In silico PCR tool',
     long_description=long_description,
     # long_description='This script takes a text file with primer sequence (one per line) and a reference FASTA file as input and identifies primer pairs which amplify a DNA sequence of length less than or equal to a user-specified maximum, at a given Tm and salt concentration. The script outputs the sequences of the primers, th eportion of the primer that binds, the number of mismatches, as well as the start and end coordinates of the amplified sequence.',
     long_description_content_type='text/markdown',
     author='Jason D Limberis',
```

