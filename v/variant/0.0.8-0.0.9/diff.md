# Comparing `tmp/variant-0.0.8.tar.gz` & `tmp/variant-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variant-0.0.8.tar", max compression
+gzip compressed data, was "variant-0.0.9.tar", max compression
```

## Comparing `variant-0.0.8.tar` & `variant-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2963 2021-11-24 22:58:16.765344 variant-0.0.8/README.md
--rw-r--r--   0        0        0      451 2021-11-24 23:41:52.777194 variant-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       22 2021-11-24 05:00:56.582691 variant-0.0.8/variant/__init__.py
--rwxr-xr-x   0        0        0     6644 2021-11-24 23:41:42.829788 variant-0.0.8/variant/effect.py
--rw-r--r--   0        0        0     3713 2021-11-24 23:42:17.011472 variant-0.0.8/setup.py
--rw-r--r--   0        0        0     3521 2021-11-24 23:42:17.011733 variant-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3286 2021-11-25 02:34:02.880549 variant-0.0.9/README.md
+-rw-r--r--   0        0        0      575 2021-11-25 02:40:09.737917 variant-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2021-11-24 05:00:56.582691 variant-0.0.9/variant/__init__.py
+-rwxr-xr-x   0        0        0     6644 2021-11-25 02:33:29.101142 variant-0.0.9/variant/effect.py
+-rw-r--r--   0        0        0     4077 2021-11-25 02:41:38.497736 variant-0.0.9/setup.py
+-rw-r--r--   0        0        0     4011 2021-11-25 02:41:38.498001 variant-0.0.9/PKG-INFO
```

### Comparing `variant-0.0.8/README.md` & `variant-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Python pakcage for genomic variant analysis
 
-
 [![Pypi Releases](https://img.shields.io/pypi/v/variant.svg)](https://pypi.python.org/pypi/variant)
 [![Downloads](https://pepy.tech/badge/variant)](https://pepy.tech/project/variant)
 
 ## `variant-effect` command can infer the effect of a mutation
 
-The input file has 5 columns: `chromosome`, `position`, `strand`, `reference allele`, `alternative allele`.
+- `-i/--input` to sepecify the input file. The input file has 5 columns: `chromosome`, `position`, `strand`, `reference allele`, `alternative allele`.
 
-- No header is required.
-- The 3rd column (strand) is not used by default, just for compatibility with RNA mode.
-- By default, the base of reference and alternative allele are based on DNA information
-- For RNA mode (through `--rna` argument), the base of reference and alternative allele is reverse complement if the strand is negative(-).
+  - No header is required.
+  - The 3rd column (strand) is not used by default, just for compatibility with RNA mode.
+  - By default, the base of reference and alternative allele are based on DNA information
+  - For RNA mode (through `--rna` argument), the base of reference and alternative allele is reverse complement if the strand is negative(-).
+
+- `-o/--output` to specify the output file, leave empty for stdout.
+- `-r/--reference` to specify reference name, can be human / mouse / dog / cat / chicken ...
+- `--rna` to run in RNA mode
+- `--all` output all effects of the variant.
 
-eg:
+> demo:
 
 Store the following table in sites.tsv.
 
 ```
 chr3    10301112        -       G       T
 chr7    94669540        +       G       N
 chr2    215361150       -       A       T
@@ -26,22 +30,26 @@
 chr2    84906537        +       C       T
 chr14   23645352        +       G       T
 chr20   37241351        +       G       T
 chrX    153651037       +       G       T
 chr17   81844010        -       A       T
 ```
 
-By command: `variant-effect -i sites.tsv -r human --rna`, the output will be:
+Run command `variant-effect -i sites.tsv -r human --rna` to get the following output.
 
 ```
 #chrom  pos     strand  ref     alt     mut_type        gene_name       transcript_id   transcript_pos  transcript_motif        coding_pos      codon_ref       aa_pos  aa_ref
 chr3    10301112        -       C       A       Silent  SEC13   ENST00000397117 1441    TTGATCATCTGCCTTAACGTG   849     CTG     284     L
 chr7    94669540        +       G       N       ThreePrimeUTR   PEG10   ENST00000612941 6240    TTTTACCCCTGTCAGTAGCCC   None    None    None    None
 chr2    215361150       -       T       A       ThreePrimeUTR   FN1     ENST00000323926 8012    GGCCCGCAATACTGTAGGAAC   None    None    None    None
 chr15   72199549        -       C       A       ThreePrimeUTR   PKM     ENST00000319622 2197    GCTGTAACGTGGCACTGGTAG   None    None    None    None
 chr17   81843580        -       G       A       ThreePrimeUTR   P4HB    ENST00000681020 3061    AGAAGCTTGTCCCCCGTGTGG   None    None    None    None
 chr2    84906537        +       C       T       ThreePrimeUTR   TMSB10  ENST00000233143 327     CCTGGGCACTCCGCGCCGATG   None    None    None    None
 chr14   23645352        +       G       T       ThreePrimeUTR   DHRS2   ENST00000344777 1391    CTGCCATTCTGCCAGACTAGC   None    None    None    None
 chr20   37241351        +       G       T       ThreePrimeUTR   RPN2    ENST00000237530 1959    AAAACTGAATGTCAAGAAAAG   None    None    None    None
 chrX    153651037       +       G       T       ThreePrimeUTR   DUSP9   ENST00000342782 2145    CTGCTACTTTGGGGGGTGGGG   None    None    None    None
 chr17   81844010        -       T       A       ThreePrimeUTR   P4HB    ENST00000681020 2631    GAACTGTAATACGCAAAGCCA   None    None    None    None
 ```
+
+TODO:
+
+- support GRCh37
```

### Comparing `variant-0.0.8/variant/effect.py` & `variant-0.0.9/variant/effect.py`

 * *Files identical despite different names*

### Comparing `variant-0.0.8/setup.py` & `variant-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 ['pyensembl>=1.9.4,<2.0.0', 'varcode']
 
 entry_points = \
 {'console_scripts': ['variant-effect = variant.effect:run']}
 
 setup_kwargs = {
     'name': 'variant',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': '',
-    'long_description': '# Python pakcage for genomic variant analysis\n\n\n[![Pypi Releases](https://img.shields.io/pypi/v/variant.svg)](https://pypi.python.org/pypi/variant)\n[![Downloads](https://pepy.tech/badge/variant)](https://pepy.tech/project/variant)\n\n## `variant-effect` command can infer the effect of a mutation\n\nThe input file has 5 columns: `chromosome`, `position`, `strand`, `reference allele`, `alternative allele`.\n\n- No header is required.\n- The 3rd column (strand) is not used by default, just for compatibility with RNA mode.\n- By default, the base of reference and alternative allele are based on DNA information\n- For RNA mode (through `--rna` argument), the base of reference and alternative allele is reverse complement if the strand is negative(-).\n\neg:\n\nStore the following table in sites.tsv.\n\n```\nchr3    10301112        -       G       T\nchr7    94669540        +       G       N\nchr2    215361150       -       A       T\nchr15   72199549        -       G       T\nchr17   81843580        -       C       T\nchr2    84906537        +       C       T\nchr14   23645352        +       G       T\nchr20   37241351        +       G       T\nchrX    153651037       +       G       T\nchr17   81844010        -       A       T\n```\n\nBy command: `variant-effect -i sites.tsv -r human --rna`, the output will be:\n\n```\n#chrom  pos     strand  ref     alt     mut_type        gene_name       transcript_id   transcript_pos  transcript_motif        coding_pos      codon_ref       aa_pos  aa_ref\nchr3    10301112        -       C       A       Silent  SEC13   ENST00000397117 1441    TTGATCATCTGCCTTAACGTG   849     CTG     284     L\nchr7    94669540        +       G       N       ThreePrimeUTR   PEG10   ENST00000612941 6240    TTTTACCCCTGTCAGTAGCCC   None    None    None    None\nchr2    215361150       -       T       A       ThreePrimeUTR   FN1     ENST00000323926 8012    GGCCCGCAATACTGTAGGAAC   None    None    None    None\nchr15   72199549        -       C       A       ThreePrimeUTR   PKM     ENST00000319622 2197    GCTGTAACGTGGCACTGGTAG   None    None    None    None\nchr17   81843580        -       G       A       ThreePrimeUTR   P4HB    ENST00000681020 3061    AGAAGCTTGTCCCCCGTGTGG   None    None    None    None\nchr2    84906537        +       C       T       ThreePrimeUTR   TMSB10  ENST00000233143 327     CCTGGGCACTCCGCGCCGATG   None    None    None    None\nchr14   23645352        +       G       T       ThreePrimeUTR   DHRS2   ENST00000344777 1391    CTGCCATTCTGCCAGACTAGC   None    None    None    None\nchr20   37241351        +       G       T       ThreePrimeUTR   RPN2    ENST00000237530 1959    AAAACTGAATGTCAAGAAAAG   None    None    None    None\nchrX    153651037       +       G       T       ThreePrimeUTR   DUSP9   ENST00000342782 2145    CTGCTACTTTGGGGGGTGGGG   None    None    None    None\nchr17   81844010        -       T       A       ThreePrimeUTR   P4HB    ENST00000681020 2631    GAACTGTAATACGCAAAGCCA   None    None    None    None\n```\n',
+    'long_description': '# Python pakcage for genomic variant analysis\n\n[![Pypi Releases](https://img.shields.io/pypi/v/variant.svg)](https://pypi.python.org/pypi/variant)\n[![Downloads](https://pepy.tech/badge/variant)](https://pepy.tech/project/variant)\n\n## `variant-effect` command can infer the effect of a mutation\n\n- `-i/--input` to sepecify the input file. The input file has 5 columns: `chromosome`, `position`, `strand`, `reference allele`, `alternative allele`.\n\n  - No header is required.\n  - The 3rd column (strand) is not used by default, just for compatibility with RNA mode.\n  - By default, the base of reference and alternative allele are based on DNA information\n  - For RNA mode (through `--rna` argument), the base of reference and alternative allele is reverse complement if the strand is negative(-).\n\n- `-o/--output` to specify the output file, leave empty for stdout.\n- `-r/--reference` to specify reference name, can be human / mouse / dog / cat / chicken ...\n- `--rna` to run in RNA mode\n- `--all` output all effects of the variant.\n\n> demo:\n\nStore the following table in sites.tsv.\n\n```\nchr3    10301112        -       G       T\nchr7    94669540        +       G       N\nchr2    215361150       -       A       T\nchr15   72199549        -       G       T\nchr17   81843580        -       C       T\nchr2    84906537        +       C       T\nchr14   23645352        +       G       T\nchr20   37241351        +       G       T\nchrX    153651037       +       G       T\nchr17   81844010        -       A       T\n```\n\nRun command `variant-effect -i sites.tsv -r human --rna` to get the following output.\n\n```\n#chrom  pos     strand  ref     alt     mut_type        gene_name       transcript_id   transcript_pos  transcript_motif        coding_pos      codon_ref       aa_pos  aa_ref\nchr3    10301112        -       C       A       Silent  SEC13   ENST00000397117 1441    TTGATCATCTGCCTTAACGTG   849     CTG     284     L\nchr7    94669540        +       G       N       ThreePrimeUTR   PEG10   ENST00000612941 6240    TTTTACCCCTGTCAGTAGCCC   None    None    None    None\nchr2    215361150       -       T       A       ThreePrimeUTR   FN1     ENST00000323926 8012    GGCCCGCAATACTGTAGGAAC   None    None    None    None\nchr15   72199549        -       C       A       ThreePrimeUTR   PKM     ENST00000319622 2197    GCTGTAACGTGGCACTGGTAG   None    None    None    None\nchr17   81843580        -       G       A       ThreePrimeUTR   P4HB    ENST00000681020 3061    AGAAGCTTGTCCCCCGTGTGG   None    None    None    None\nchr2    84906537        +       C       T       ThreePrimeUTR   TMSB10  ENST00000233143 327     CCTGGGCACTCCGCGCCGATG   None    None    None    None\nchr14   23645352        +       G       T       ThreePrimeUTR   DHRS2   ENST00000344777 1391    CTGCCATTCTGCCAGACTAGC   None    None    None    None\nchr20   37241351        +       G       T       ThreePrimeUTR   RPN2    ENST00000237530 1959    AAAACTGAATGTCAAGAAAAG   None    None    None    None\nchrX    153651037       +       G       T       ThreePrimeUTR   DUSP9   ENST00000342782 2145    CTGCTACTTTGGGGGGTGGGG   None    None    None    None\nchr17   81844010        -       T       A       ThreePrimeUTR   P4HB    ENST00000681020 2631    GAACTGTAATACGCAAAGCCA   None    None    None    None\n```\n\nTODO:\n\n- support GRCh37\n',
     'author': 'Chang Ye',
     'author_email': 'yech1990@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
-    'url': None,
+    'url': 'https://github.com/yech1990/variant',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.6,<4.0',
 }
```

### Comparing `variant-0.0.8/PKG-INFO` & `variant-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 Metadata-Version: 2.1
 Name: variant
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
+Home-page: https://github.com/yech1990/variant
 License: MIT
+Keywords: bioinformatics,variant,mutation,RNA modification
 Author: Chang Ye
 Author-email: yech1990@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: pyensembl (>=1.9.4,<2.0.0)
 Requires-Dist: varcode
+Project-URL: Repository, https://github.com/yech1990/variant
 Description-Content-Type: text/markdown
 
 # Python pakcage for genomic variant analysis
 
-
 [![Pypi Releases](https://img.shields.io/pypi/v/variant.svg)](https://pypi.python.org/pypi/variant)
 [![Downloads](https://pepy.tech/badge/variant)](https://pepy.tech/project/variant)
 
 ## `variant-effect` command can infer the effect of a mutation
 
-The input file has 5 columns: `chromosome`, `position`, `strand`, `reference allele`, `alternative allele`.
+- `-i/--input` to sepecify the input file. The input file has 5 columns: `chromosome`, `position`, `strand`, `reference allele`, `alternative allele`.
 
-- No header is required.
-- The 3rd column (strand) is not used by default, just for compatibility with RNA mode.
-- By default, the base of reference and alternative allele are based on DNA information
-- For RNA mode (through `--rna` argument), the base of reference and alternative allele is reverse complement if the strand is negative(-).
+  - No header is required.
+  - The 3rd column (strand) is not used by default, just for compatibility with RNA mode.
+  - By default, the base of reference and alternative allele are based on DNA information
+  - For RNA mode (through `--rna` argument), the base of reference and alternative allele is reverse complement if the strand is negative(-).
+
+- `-o/--output` to specify the output file, leave empty for stdout.
+- `-r/--reference` to specify reference name, can be human / mouse / dog / cat / chicken ...
+- `--rna` to run in RNA mode
+- `--all` output all effects of the variant.
 
-eg:
+> demo:
 
 Store the following table in sites.tsv.
 
 ```
 chr3    10301112        -       G       T
 chr7    94669540        +       G       N
 chr2    215361150       -       A       T
@@ -44,15 +51,15 @@
 chr2    84906537        +       C       T
 chr14   23645352        +       G       T
 chr20   37241351        +       G       T
 chrX    153651037       +       G       T
 chr17   81844010        -       A       T
 ```
 
-By command: `variant-effect -i sites.tsv -r human --rna`, the output will be:
+Run command `variant-effect -i sites.tsv -r human --rna` to get the following output.
 
 ```
 #chrom  pos     strand  ref     alt     mut_type        gene_name       transcript_id   transcript_pos  transcript_motif        coding_pos      codon_ref       aa_pos  aa_ref
 chr3    10301112        -       C       A       Silent  SEC13   ENST00000397117 1441    TTGATCATCTGCCTTAACGTG   849     CTG     284     L
 chr7    94669540        +       G       N       ThreePrimeUTR   PEG10   ENST00000612941 6240    TTTTACCCCTGTCAGTAGCCC   None    None    None    None
 chr2    215361150       -       T       A       ThreePrimeUTR   FN1     ENST00000323926 8012    GGCCCGCAATACTGTAGGAAC   None    None    None    None
 chr15   72199549        -       C       A       ThreePrimeUTR   PKM     ENST00000319622 2197    GCTGTAACGTGGCACTGGTAG   None    None    None    None
@@ -60,7 +67,11 @@
 chr2    84906537        +       C       T       ThreePrimeUTR   TMSB10  ENST00000233143 327     CCTGGGCACTCCGCGCCGATG   None    None    None    None
 chr14   23645352        +       G       T       ThreePrimeUTR   DHRS2   ENST00000344777 1391    CTGCCATTCTGCCAGACTAGC   None    None    None    None
 chr20   37241351        +       G       T       ThreePrimeUTR   RPN2    ENST00000237530 1959    AAAACTGAATGTCAAGAAAAG   None    None    None    None
 chrX    153651037       +       G       T       ThreePrimeUTR   DUSP9   ENST00000342782 2145    CTGCTACTTTGGGGGGTGGGG   None    None    None    None
 chr17   81844010        -       T       A       ThreePrimeUTR   P4HB    ENST00000681020 2631    GAACTGTAATACGCAAAGCCA   None    None    None    None
 ```
 
+TODO:
+
+- support GRCh37
+
```

