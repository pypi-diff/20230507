# Comparing `tmp/getMultiPrimerSet-0.2a0.tar.gz` & `tmp/getMultiPrimerSet-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getMultiPrimerSet-0.2a0.tar", last modified: Sat May  6 23:05:39 2023, max compression
+gzip compressed data, was "getMultiPrimerSet-0.3.tar", last modified: Sun May  7 03:40:33 2023, max compression
```

## Comparing `getMultiPrimerSet-0.2a0.tar` & `getMultiPrimerSet-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-06 23:05:39.031075 getMultiPrimerSet-0.2a0/
--rw-r--r--   0 semiquant   (502) staff       (20)     2682 2023-05-06 23:05:39.030913 getMultiPrimerSet-0.2a0/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)     2474 2023-05-06 23:04:07.000000 getMultiPrimerSet-0.2a0/README.md
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-06 23:05:39.029937 getMultiPrimerSet-0.2a0/getMultiPrimerSet/
--rw-r--r--   0 semiquant   (502) staff       (20)    13597 2023-05-06 22:51:30.000000 getMultiPrimerSet-0.2a0/getMultiPrimerSet/getMultiPrimerSet.py
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-06 23:05:39.030719 getMultiPrimerSet-0.2a0/getMultiPrimerSet.egg-info/
--rw-r--r--   0 semiquant   (502) staff       (20)     2682 2023-05-06 23:05:38.000000 getMultiPrimerSet-0.2a0/getMultiPrimerSet.egg-info/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)      305 2023-05-06 23:05:39.000000 getMultiPrimerSet-0.2a0/getMultiPrimerSet.egg-info/SOURCES.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-06 23:05:38.000000 getMultiPrimerSet-0.2a0/getMultiPrimerSet.egg-info/dependency_links.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       79 2023-05-06 23:05:38.000000 getMultiPrimerSet-0.2a0/getMultiPrimerSet.egg-info/entry_points.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       34 2023-05-06 23:05:38.000000 getMultiPrimerSet-0.2a0/getMultiPrimerSet.egg-info/requires.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       18 2023-05-06 23:05:38.000000 getMultiPrimerSet-0.2a0/getMultiPrimerSet.egg-info/top_level.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-06 23:05:39.031123 getMultiPrimerSet-0.2a0/setup.cfg
--rw-r--r--   0 semiquant   (502) staff       (20)     3035 2023-05-06 23:05:12.000000 getMultiPrimerSet-0.2a0/setup.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 03:40:33.482335 getMultiPrimerSet-0.3/
+-rw-r--r--   0 semiquant   (502) staff       (20)     2680 2023-05-07 03:40:33.482171 getMultiPrimerSet-0.3/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)     2550 2023-05-07 03:39:39.000000 getMultiPrimerSet-0.3/README.md
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 03:40:33.481166 getMultiPrimerSet-0.3/getMultiPrimerSet/
+-rw-r--r--   0 semiquant   (502) staff       (20)    16869 2023-05-07 03:39:27.000000 getMultiPrimerSet-0.3/getMultiPrimerSet/getMultiPrimerSet.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 03:40:33.481986 getMultiPrimerSet-0.3/getMultiPrimerSet.egg-info/
+-rw-r--r--   0 semiquant   (502) staff       (20)     2680 2023-05-07 03:40:33.000000 getMultiPrimerSet-0.3/getMultiPrimerSet.egg-info/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)      305 2023-05-07 03:40:33.000000 getMultiPrimerSet-0.3/getMultiPrimerSet.egg-info/SOURCES.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-07 03:40:33.000000 getMultiPrimerSet-0.3/getMultiPrimerSet.egg-info/dependency_links.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       79 2023-05-07 03:40:33.000000 getMultiPrimerSet-0.3/getMultiPrimerSet.egg-info/entry_points.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       34 2023-05-07 03:40:33.000000 getMultiPrimerSet-0.3/getMultiPrimerSet.egg-info/requires.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       18 2023-05-07 03:40:33.000000 getMultiPrimerSet-0.3/getMultiPrimerSet.egg-info/top_level.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-07 03:40:33.482387 getMultiPrimerSet-0.3/setup.cfg
+-rw-r--r--   0 semiquant   (502) staff       (20)     3034 2023-05-07 03:40:07.000000 getMultiPrimerSet-0.3/setup.py
```

### Comparing `getMultiPrimerSet-0.2a0/PKG-INFO` & `getMultiPrimerSet-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getMultiPrimerSet
-Version: 0.2a0
+Version: 0.3
 Summary: A package for generating multiplex PCR primer sets
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `getMultiPrimerSet-0.2a0/README.md` & `getMultiPrimerSet-0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -44,8 +44,12 @@
     --primer_len 20 \
     --product_size_min 400 \
     --product_size_max 800 \
     --ret 10 \
     --Q5 \
     --background "" \
     --output "example"
-```
+```
+
+
+### TODO
+-   Add pre and post check for overlapping amplicons and correct
```

### Comparing `getMultiPrimerSet-0.2a0/getMultiPrimerSet/getMultiPrimerSet.py` & `getMultiPrimerSet-0.3/getMultiPrimerSet/getMultiPrimerSet.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 import primer3
 import pandas as pd
 import itertools
 import argparse
 import numpy as np
 import concurrent.futures
 import sys
+import random
 
 parser = argparse.ArgumentParser(description='PCR primer design')
 
 # Define input arguments
 parser.add_argument('--region_file', type=str, help='The path to the primer design region file. Two columns, start position and end position (1-based). tsv or xlxs', required=True)
 parser.add_argument('--input_file', type=str, help='The path to the input FASTA file.', required=True)
 parser.add_argument('--target_tm', type=float, help='The desired melting temperature (Tm) for the primers.', default=65)
 parser.add_argument('--primer_len', type=int, help='The desired length of the primers.', default=20)
 parser.add_argument('--product_size_min', type=int, help='The desired min size for the PCR product. Default is 400.', default=400)
 parser.add_argument('--product_size_max', type=int, help='The desired max size for the PCR product. Default is 800.', default=800)
 parser.add_argument('--ret', type=int, help='The maximum number of primer pairs to return.', default=100)
 parser.add_argument('--Q5', action='store_true', help='Whether to use Q5 settings for primer3.', default=True)
 parser.add_argument('--background', type=str, help='The path to the mispriming library FASTA file.', default='')
 parser.add_argument('--output', type=str, help='Output name.', default='MultiPlexPrimerSet')
-parser.add_argument('--cpus', type=int, help='CPUs', default=8)
-parser.add_argument('--eval', type=int, help='The maximum number of primer sets to evaluate. (this will be an upperlimit and may not be reched due to a complication in the code)', default=10000)
+# parser.add_argument('--cpus', type=int, help='number of threads (even though it says cpus)', default=1000)
+parser.add_argument('--eval', type=int, help='The maximum number of primer sets to evaluate.', default=10000)
 args = parser.parse_args()
 
 product_size_range = (args.product_size_min, args.product_size_max)
 
 def design_primers(input_file, region_start, region_end, target_tm=65, primer_len=20, product_size_range=(400, 800), name='', ret=100, Q5=True, background=''):
     """
     This function takes a FASTA file, start and end positions of a target region, and desired melting temperature
@@ -49,38 +50,47 @@
 
     Returns:
     list: A list of dicts containing information about the primer pairs.
     """
 
     # Parse the input FASTA file and extract the target region sequence.
     print("Picking initial primers for " + name)
-    record = SeqIO.read(input_file, "fasta")
-    target_seq = record.seq[region_start-1:region_end]
+    if region_start - 10000 > 0:
+        target_seq = input_file.seq[region_start-10000:region_end+10000]
+        seq_target = (10000-1, region_end-region_start)
+    else:
+        target_seq = input_file.seq[0:end]
+        seq_target = (region_start-1, region_end-region_start)
+    
+    # target_seq = input_file.seq
+    # seq_target = (region_start-1, region_end-region_start+2)
 
     # Set up the primer3 input parameters.
     input_params = {
     'SEQUENCE_ID': record.id,
     'SEQUENCE_TEMPLATE': str(target_seq),
+    'SEQUENCE_TARGET': seq_target,
     'PRIMER_OPT_SIZE': primer_len,
     'PRIMER_MIN_SIZE' : primer_len - 10,
     'PRIMER_MAX_SIZE' : primer_len + 20,
     'PRIMER_PICK_INTERNAL_OLIGO': 0,
-    'PRIMER_PRODUCT_SIZE_RANGE': f"{product_size_range[0]}-{product_size_range[1]}",
     }
+
     if background != '':
         input_params.update({'PRIMER_MISPRIMING_LIBRARY': background,})
 
     global_args = {
     'PRIMER_MIN_GC': 40,
     'PRIMER_MAX_GC': 80,
     'PRIMER_NUM_RETURN': ret,
     'PRIMER_EXPLAIN_FLAG': 1,
     'PRIMER_MIN_TM': target_tm-4,
     'PRIMER_OPT_TM': target_tm,
     'PRIMER_MAX_TM': target_tm+4,
+    'PRIMER_PRODUCT_SIZE_RANGE': product_size_range,
     }
         
     if Q5:
         global_args.update({
         'PRIMER_SALT_DIVALENT': 2,
         'PRIMER_SALT_MONOVALENT': 80,
         'PRIMER_DNA_CONC': 5800,
@@ -89,15 +99,15 @@
         })
 
     # Run primer3 to design the primers.
     primers = primer3.bindings.designPrimers(input_params, global_args)
     try:
         # Check if any primer pairs were returned.
         if 'PRIMER_PAIR_NUM_RETURNED' not in primers or primers['PRIMER_PAIR_NUM_RETURNED'] == 0:
-            print("No primers found!")
+            # print("No primers found for: " + name)
             return []
         else:
             # Extract information about the primer pairs.
             primer_pairs = []
             for i in range(primers['PRIMER_PAIR_NUM_RETURNED']):
                 forward_seq = primers[f'PRIMER_LEFT_{i}_SEQUENCE']
                 reverse_seq = primers[f'PRIMER_RIGHT_{i}_SEQUENCE']
@@ -117,26 +127,51 @@
                     })
     except Exception as e:
         print("An error occurred:", e)
 
     return primer_pairs
 
 
+def is_valid_combination(combination, names):
+    if set(entry['name'] for entry in combination) == names:
+        return combination
+    return []
+
+def evaluate_combination(comb):
+    # Create a list of primer pairs
+    primer_pairs = [(p1, p2) for p1, p2 in itertools.combinations(comb, 2)]
+    # Extract the primer sequences from the primer pairs
+    primer_pairs_sequences = [(p1['Forward Primer'], p2['Reverse Primer']) for p1, p2 in primer_pairs]
+    # Calculate heterodimer formation energy
+    heterodimer_scores = []
+    for p in primer_pairs_sequences:
+        heterodimer_scores.append(primer3.calcHeterodimer(p[0], p[1], temp_c=args.target_tm).dg) #gibbs free energy
+        
+    score = {'size': product_size_range,
+             'tmp': tm_range,
+             'mean': np.mean(heterodimer_scores),
+             'range': abs(np.min(heterodimer_scores)) - abs(np.max(heterodimer_scores))
+            }
+    
+    return score, comb
+
 # Read the file into a pandas DataFrame
 file_path = args.region_file  # or 'file.xlsx'
 if file_path.endswith('.tsv'):
     df = pd.read_csv(file_path, sep='\t')
 else:
     df = pd.read_excel(file_path)
 
 seen_names = set()
 modified_names = {}
 
 primers_all = []
 
+record = SeqIO.read(args.input_file, "fasta")
+
 # Iterate over each row
 for index, row in df.iterrows():
     # Access the "start" and "end" values using the column names
     # name=str(row['name'])
     start = int(row['start'])
     end = int(row['end'])
     name = 'Target ' + str(start) + "-" + str(end)
@@ -152,21 +187,22 @@
             modified_name = modified_names[name]
         else:
             modified_name = name + '_' + str(random.randint(1, 100))
             modified_names[name] = modified_name
         # Update name in row
         df.at[index, 'name'] = modified_name
         seen_names.add(modified_name)
+        name = modified_name
     else:
         seen_names.add(name)
 
     # Call the design_primers function to design primers for the target region.
     primer_tmp = []
     primer_tmp = design_primers(
-        input_file=args.input_file,
+        input_file=record,
         region_start=start,
         region_end=end,
         target_tm=args.target_tm,
         primer_len=args.primer_len,
         product_size_range=product_size_range,
         name=name,
         ret=args.ret,
@@ -188,123 +224,169 @@
 flat_list = []
 for sublist in primers_all:
     for item in sublist:
         flat_list.append(item)
 
 primers_all = flat_list
 
-names = set(d['name'] for d in primers_all)
-
+names = set([primer['name'] for primer in primers_all])  # get unique names
+if len(names) <= 1:
+    print("not enough targets! " + ' '.join(map(str, names)))
+    exit(1)
+else:
+    print("Finding best primer set for the following targets: " + ', '.join(map(str, names)))
+    best_score = {'mean': float('inf'), 'range': float('inf'), 'tmp': float('inf'), 'size': float('inf')}
+    best_comb = None
+    valid_combinations = []
+    pos = 0
+    name_primers_dict = {}
+    for name in names:
+        name_primers_dict[name] = [primer for primer in primers_all if primer['name'] == name]  # group primers by name
+
+    # This nees to be fixed
+    combinations = []
+    for i in range(args.eval):
+        combination = []
+        for name in names:
+            name_primers = name_primers_dict[name]  # get primers for the current name
+            combination.append(random.choice(name_primers))
+        combinations.append(combination)
 
-def calculate_score(comb, target_tm=target_tm):
+    print("Picking best set from: ", len(combinations), " combinations")
     # tm and size
     product_sizes = [d['Product Size'] for d in primers_all]
     tm_values = [d['Forward tm'] for d in primers_all] + [d['Reverse tm'] for d in primers_all]
-    product_size_range = max(product_sizes) - min(product_sizes)
+    # product_size_range = max(product_sizes) - min(product_sizes)
     tm_range = max(tm_values) - min(tm_values)
-
-    # Create a list of primer pairs
-    primer_pairs = [(p1, p2) for p1, p2 in itertools.combinations(comb, 2)]
-    # Extract the primer sequences from the primer pairs
-    primer_pairs_sequences = [(p1['Forward Primer'], p2['Reverse Primer']) for p1, p2 in primer_pairs]
-    # Calculate heterodimer formation energy
-    heterodimer_scores = []
-    for p in primer_pairs_sequences:
-        heterodimer_scores.append(primer3.calcHeterodimer(p[0], p[1], temp_c = target_tm).dg) #gibbs free energy
-
-    score = {'size': product_size_range,
-            'tmp': tm_range,
-            'mean': np.mean(heterodimer_scores),
-            'range': abs(np.min(heterodimer_scores)) - abs(np.max(heterodimer_scores))
-            }
-
-    return score, comb
-
-
-if len(names) <= 1:
-    print("not enough targets! " + ' '.join(str(x) for x in names))
-    exit(1)
-else:
-    print("Finding best primer set for the following targets: " + ', '.join(str(x) for x in names))
-    # generate all possible combinations of the entries, this takes forever, so gen 4*args.eval and hope its enough
-    combinations = itertools.islice(itertools.combinations(primers_all, len(names)), 4 * args.eval)
-
-    # filter out combinations that don't include each unique name
-    valid_combinations = [c for c in combinations if set(entry['name'] for entry in c) == names]
-
-    # select only args.eval valid combinations
-    valid_combinations = itertools.islice(valid_combinations, args.eval)
-
-    best_score = {'mean': float('inf'), 'range': float('inf'), 'tmp': float('inf'), 'size': float('inf')}
+    best_score = {'mean': float('inf'), 'range': float('inf'), 'tmp': float('inf')}
     best_comb = None
 
-    num_valid_combinations = len(valid_combinations)
-    print("From a total of " + str(num_valid_combinations) + " combinations")
-    with concurrent.futures.ThreadPoolExecutor(max_workers=args.cpus) as executor:
-        # Submit each combination to the thread pool
-        future_scores = {executor.submit(calculate_score, comb): comb for comb in valid_combinations}
-        for i, future in enumerate(concurrent.futures.as_completed(future_scores)):
+    with concurrent.futures.ThreadPoolExecutor() as executor:
+        futures = [executor.submit(evaluate_combination, comb) for comb in combinations]
+
+        for future in concurrent.futures.as_completed(futures):
             score, comb = future.result()
-            # Update best_score and best_comb if score is better
             if best_score['mean'] > score['mean']:
                 if best_score['range'] * 0.9 > score['range']:
                     best_score = score
                     best_comb = comb
                 elif best_score['tmp'] > 4 or score['tmp'] > 4 and best_score['tmp'] > score['tmp']:
                     best_score = score
                     best_comb = comb
-            # Print progress
-            progress = (i + 1) / num_valid_combinations * 100
-            sys.stdout.write('\rProgress: %.2f%%' % progress)
-            sys.stdout.flush()
 
-    with pd.ExcelWriter(args.MultiPlexPrimerSet + '.xlsx') as writer:
-        best_comb.to_excel(writer, sheet_name='PrimerSet', index=False)
+    print("")
+    print("writing file: " + args.output + '.xlsx')
+    # convert best_comb tuple to DataFrame object
+    best_comb = pd.DataFrame(list(best_comb))
+    best_comb.to_excel(args.output + '.xlsx', sheet_name='PrimerSet', index=False)
+
+
+
 
+
+###############
+## GRAVEYARD ##
+    # with concurrent.futures.ThreadPoolExecutor(max_workers=args.cpus) as executor:
+    #     future_scores = {executor.submit(calculate_score, comb): comb for comb in combinations}
+    #     for i, future in enumerate(concurrent.futures.as_completed(future_scores)):
+    #         score, comb = future.result()
+    #         if best_score['mean'] > score['mean'] and (best_score['range'] * 0.9 > score['range'] or (best_score['tmp'] > 4 or score['tmp'] > 4 and best_score['tmp'] > score['tmp'])):
+    #             best_score = score
+    #             best_comb = comb
+    #         progress = (i + 1) / len(combinations) * 100
+    #         sys.stdout.write('\rProgress: %.2f%%' % progress)
+    #         sys.stdout.flush()
+    
+
+
+
+# multithread
+# names = set(d['name'] for d in primers_all)
+# if len(names) <= 1:
+#     print("not enough targets! " + ' '.join(map(str, names)))
+#     exit(1)
+# else:
+#     print("Finding best primer set for the following targets: " + ', '.join(map(str, names)))
+#     best_score = {'mean': float('inf'), 'range': float('inf'), 'tmp': float('inf'), 'size': float('inf')}
+#     best_comb = None
+#     valid_combinations = []
+#     pos = 0
+
+#     with concurrent.futures.ThreadPoolExecutor(max_workers=args.cpus) as executor:
+#         while len(valid_combinations) < args.eval:
+#             combinations = itertools.islice(itertools.combinations(primers_all, len(names)), pos+1, pos+1000)
+#             pos += 1000
+#             futures = [executor.submit(is_valid_combination, c, names) for c in combinations]
+#             for future in concurrent.futures.as_completed(futures):
+#                 if future.result():
+#                     valid_combinations.append(future.result())
+#                 if len(valid_combinations) >= args.eval:
+#                     break
+
+#     print("Picking best set from: ", len(valid_combinations), " combinations")
+
+#     with concurrent.futures.ThreadPoolExecutor(max_workers=args.cpus) as executor:
+#         future_scores = {executor.submit(calculate_score, comb): comb for comb in valid_combinations}
+#         for i, future in enumerate(concurrent.futures.as_completed(future_scores)):
+#             score, comb = future.result()
+#             if best_score['mean'] > score['mean'] and (best_score['range'] * 0.9 > score['range'] or (best_score['tmp'] > 4 or score['tmp'] > 4 and best_score['tmp'] > score['tmp'])):
+#                 best_score = score
+#                 best_comb = comb
+#             progress = (i + 1) / len(valid_combinations) * 100
+#             sys.stdout.write('\rProgress: %.2f%%' % progress)
+#             sys.stdout.flush()
+#     print("")
+#     print("writing file: " + args.output + '.xlsx')
+#     # convert best_comb tuple to DataFrame object
+#     best_comb = pd.DataFrame(list(best_comb))
+#     best_comb.to_excel(args.output + '.xlsx', sheet_name='PrimerSet', index=False)
+
+
+# single thread
 # if len(names) <= 1:
 #     print("not enough targets! " + ' '.join(str(x) for x in names))
 #     exit(1)
 # else:
 #     print("Finding best primer set for the following targets: " + ' '.join(str(x) for x in names))
 #     # generate all possible combinations
 #     combinations = itertools.chain.from_iterable(itertools.combinations(primers_all, r) for r in range(len(primers_all) + 1))
 
 #     # filter out combinations that don't include each unique name
 #     valid_combinations = [c for c in combinations if set(d['name'] for d in c) == names]
 
 #     # Iterate over valid combinations
-#     for comb in valid_combinations:
-#         # tm and size
-#         product_sizes = [d['Product Size'] for d in primers_all]
-#         tm_values = [d['Forward tm'] for d in primers_all] + [d['Reverse tm'] for d in primers_all]
-#         product_size_range = max(product_sizes) - min(product_sizes)
-#         tm_range = max(tm_values) - min(tm_values)
+    # for comb in valid_combinations:
+    #     # tm and size
+    #     product_sizes = [d['Product Size'] for d in primers_all]
+    #     tm_values = [d['Forward tm'] for d in primers_all] + [d['Reverse tm'] for d in primers_all]
+    #     product_size_range = max(product_sizes) - min(product_sizes)
+    #     tm_range = max(tm_values) - min(tm_values)
         
-#         # Create a list of primer pairs
-#         primer_pairs = [(p1, p2) for p1, p2 in itertools.combinations(comb, 2)]
-#         # Extract the primer sequences from the primer pairs
-#         primer_pairs_sequences = [(p1['Forward Primer'], p2['Reverse Primer']) for p1, p2 in primer_pairs]
-#         # Calculate heterodimer formation energy
-#         heterodimer_scores = []
-#         for p in primer_pairs_sequences:
-#             heterodimer_scores.append(primer3.calcHeterodimer(p[0], p[1], temp_c = target_tm).dg) #gibbs free energy
+    #     # Create a list of primer pairs
+    #     primer_pairs = [(p1, p2) for p1, p2 in itertools.combinations(comb, 2)]
+    #     # Extract the primer sequences from the primer pairs
+    #     primer_pairs_sequences = [(p1['Forward Primer'], p2['Reverse Primer']) for p1, p2 in primer_pairs]
+    #     # Calculate heterodimer formation energy
+    #     heterodimer_scores = []
+    #     for p in primer_pairs_sequences:
+    #         heterodimer_scores.append(primer3.calcHeterodimer(p[0], p[1], temp_c = target_tm).dg) #gibbs free energy
         
-#         score = {'size': product_size_range,
-#               'tmp': tm_range,
-#               'mean': np.mean(heterodimer_scores),
-#               'range': abs(np.min(heterodimer_scores)) - abs(np.max(heterodimer_scores))
-#                  }
-
-#         if best_score['mean'] > score['mean']:
-#             if best_score['range'] * 0.9 > score['range']:
-#                 best_score = score
-#                 best_comb = comb
-#             elif best_score['tmp'] > 4 or score['tmp'] > 4 and best_score['tmp'] > score['tmp']:
-#                 best_score = score
-#                 best_comb = comb
+    #     score = {'size': product_size_range,
+    #           'tmp': tm_range,
+    #           'mean': np.mean(heterodimer_scores),
+    #           'range': abs(np.min(heterodimer_scores)) - abs(np.max(heterodimer_scores))
+    #              }
+
+    #     if best_score['mean'] > score['mean']:
+    #         if best_score['range'] * 0.9 > score['range']:
+    #             best_score = score
+    #             best_comb = comb
+    #         elif best_score['tmp'] > 4 or score['tmp'] > 4 and best_score['tmp'] > score['tmp']:
+    #             best_score = score
+    #             best_comb = comb
 
 #     best_comb = pd.DataFrame(best_comb)
 #     # df.to_csv('my_dataframe.tsv', sep='\t', index=False)
 #     # Write the DataFrame to an Excel file
     # with pd.ExcelWriter(args.MultiPlexPrimerSet + '.xlsx') as writer:
     #     best_comb.to_excel(writer, sheet_name='PrimerSet', index=False)
```

### Comparing `getMultiPrimerSet-0.2a0/getMultiPrimerSet.egg-info/PKG-INFO` & `getMultiPrimerSet-0.3/getMultiPrimerSet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getMultiPrimerSet
-Version: 0.2a0
+Version: 0.3
 Summary: A package for generating multiplex PCR primer sets
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `getMultiPrimerSet-0.2a0/setup.py` & `getMultiPrimerSet-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='getMultiPrimerSet',
-    version='0.2a',
+    version='0.3',
     description='A package for generating multiplex PCR primer sets',
     author='Jason D Limberis',
     author_email='Jason.Limberis@ucsf.edu',
     long_description='''
 This program designs PCR primers for a multiplex of given target regions of a DNA sequence in a FASTA file.
 
 The script takes several arguments:
```

