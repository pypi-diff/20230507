# Comparing `tmp/wgd-2.0.0.tar.gz` & `tmp/wgd-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wgd-2.0.0.tar", last modified: Sat May  6 18:06:40 2023, max compression
+gzip compressed data, was "dist/wgd-2.0.1.tar", last modified: Sat May  6 22:08:22 2023, max compression
```

## Comparing `wgd-2.0.0.tar` & `wgd-2.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-06 18:06:40.061311 wgd-2.0.0/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.0/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)      196 2023-05-06 18:06:40.061311 wgd-2.0.0/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    26680 2023-05-06 17:53:01.000000 wgd-2.0.0/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)    48850 2023-05-06 17:49:05.000000 wgd-2.0.0/cli.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-06 18:06:40.062311 wgd-2.0.0/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1751 2023-05-06 17:34:56.000000 wgd-2.0.0/setup.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-06 18:06:40.043786 wgd-2.0.0/test/
--rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-05-06 17:05:44.000000 wgd-2.0.0/test/test_core.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-06 18:06:40.056311 wgd-2.0.0/wgd/
--rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.0/wgd/__init__.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.0/wgd/beast.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.0/wgd/cluster.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.0/wgd/codeml.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   134256 2023-05-06 17:43:55.000000 wgd-2.0.0/wgd/core.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.0/wgd/mcmctree.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.0/wgd/mix.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   103602 2023-05-05 17:52:04.000000 wgd-2.0.0/wgd/peak.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8513 2023-04-27 10:26:53.000000 wgd-2.0.0/wgd/syn.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    28648 2022-09-30 07:30:21.000000 wgd-2.0.0/wgd/utils.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    94414 2023-04-27 13:43:08.000000 wgd-2.0.0/wgd/viz.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-06 18:06:40.060311 wgd-2.0.0/wgd.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)      196 2023-05-06 18:06:39.000000 wgd-2.0.0/wgd.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      369 2023-05-06 18:06:39.000000 wgd-2.0.0/wgd.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-06 18:06:39.000000 wgd-2.0.0/wgd.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2023-05-06 18:06:39.000000 wgd-2.0.0/wgd.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      707 2023-05-06 18:06:39.000000 wgd-2.0.0/wgd.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-05-06 18:06:39.000000 wgd-2.0.0/wgd.egg-info/top_level.txt
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-06 22:08:22.375787 wgd-2.0.1/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.1/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    30069 2023-05-06 22:08:22.375787 wgd-2.0.1/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    26759 2023-05-06 21:15:09.000000 wgd-2.0.1/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    49022 2023-05-06 19:30:56.000000 wgd-2.0.1/cli.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-06 22:08:22.376806 wgd-2.0.1/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1918 2023-05-06 21:54:59.000000 wgd-2.0.1/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-06 22:08:22.362205 wgd-2.0.1/test/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-05-06 17:05:44.000000 wgd-2.0.1/test/test_core.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-06 22:08:22.370630 wgd-2.0.1/wgd/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.1/wgd/__init__.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.1/wgd/beast.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.1/wgd/cluster.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.1/wgd/codeml.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   134346 2023-05-06 19:28:28.000000 wgd-2.0.1/wgd/core.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.1/wgd/mcmctree.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.1/wgd/mix.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   103602 2023-05-05 17:52:04.000000 wgd-2.0.1/wgd/peak.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8513 2023-04-27 10:26:53.000000 wgd-2.0.1/wgd/syn.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    28648 2022-09-30 07:30:21.000000 wgd-2.0.1/wgd/utils.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    94414 2023-04-27 13:43:08.000000 wgd-2.0.1/wgd/viz.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-06 22:08:22.374787 wgd-2.0.1/wgd.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    30069 2023-05-06 22:08:22.000000 wgd-2.0.1/wgd.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      369 2023-05-06 22:08:22.000000 wgd-2.0.1/wgd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-06 22:08:22.000000 wgd-2.0.1/wgd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       51 2023-05-06 22:08:22.000000 wgd-2.0.1/wgd.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      754 2023-05-06 22:08:22.000000 wgd-2.0.1/wgd.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-05-06 22:08:22.000000 wgd-2.0.1/wgd.egg-info/top_level.txt
```

### Comparing `wgd-2.0.0/LICENSE` & `wgd-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wgd-2.0.0/README.md` & `wgd-2.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,21 @@
 
 Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
 
 The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
 
 ## Installation
 
-To install `wgd` in a virtual environment, the following command lines could be used.
+The easiest way to install `wgd v2` is using PYPI
+
+```
+pip install wgd
+```
+
+To install `wgd v2` in a virtual environment, the following command lines could be used.
 
 ```
 git clone <wgd repo>
 cd wgd
 virtualenv -p=python3 ENV (or python3 -m venv ENV)
 source ENV/bin/activate
 pip install -r requirements.txt
```

### Comparing `wgd-2.0.0/cli.py` & `wgd-2.0.1/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,17 +109,17 @@
 
         wgd dmd ath.fasta vvi.fasta egr.fasta --focus ath.fasta (--anchorpoints anchorpoints.txt --cscore 0.7)
 
     """
     _dmd(**kwargs)
 
 def _dmd(sequences, outdir, tmpdir, cscore, inflation, eval, to_stop, cds, focus, anchorpoints, keepfasta, keepduplicates, globalmrbh, nthreads, orthoinfer, onlyortho, getnsog, tree_method, treeset, msogcut, geneassign, assign_method, seq2assign, fam2assign, concat, segments, listelements, collinearcoalescence, testsog, bins, buscosog, buscohmm, buscocutoff, genetable, normalizedpercent, nonormalization):
-    from wgd.core import SequenceData, read_MultiRBH_gene_families,mrbh,ortho_infer,genes2fams,endt,memory_reporter,segmentsaps,bsog
-    memory_reporter()
+    from wgd.core import SequenceData, read_MultiRBH_gene_families,mrbh,ortho_infer,genes2fams,endt,segmentsaps,bsog
     start = timer()
+    if tmpdir != None and not os.path.isdir(tmpdir): os.mkdir(tmpdir)
     s = [SequenceData(s, out_path=outdir, tmp_path=tmpdir, to_stop=to_stop, cds=cds, cscore=cscore, threads=nthreads, bins=bins, normalizedpercent=normalizedpercent, nonormalization=nonormalization) for s in sequences]
     for i in s: logging.info("tmpdir = {} for {}".format(i.tmp_path,i.prefix))
     if buscosog:
         logging.info("Constructing busco-guided families")
         bsog(s,buscohmm,outdir,eval,nthreads,buscocutoff)
         endt(tmpdir,start,s)
     if collinearcoalescence:
@@ -215,14 +215,15 @@
     """
     _focus(**kwargs)
 
 def _focus(families, sequences, outdir, tmpdir, nthreads, to_stop, cds, strip_gaps, aligner, tree_method, treeset, concatenation, coalescence, speciestree, dating, datingset, nsites, outgroup, partition, aamodel, ks, annotation, pairwise, eggnogdata, pfam, dmnb, hmm, evalue, exepath, fossil, rootheight, chainset, beastlgjar, beagle, protdating):
     from wgd.core import SequenceData, read_gene_families, get_gene_families, KsDistributionBuilder
     from wgd.core import mergeMultiRBH_seqs, read_MultiRBH_gene_families, get_MultipRBH_gene_families, Concat, _Codon2partition_, Coale, Run_MCMCTREE, Run_r8s, Reroot, eggnog, hmmer_pfam, interproscan, Run_BEAST, get_only_protaln, Run_MCMCTREE_concprot, Concat_prot
     start = timer()
+    if tmpdir != None and not os.path.isdir(tmpdir): os.mkdir(tmpdir)
     if dating=='r8s' and not speciestree is None and nsites is None:
         logging.error("Please provide nsites parameter for r8s dating")
         exit(0)
     if dating=='r8s' and speciestree is None and outgroup is None:
         logging.error("Please provide outgroup species for r8s dating")
         exit(0)
     if len(sequences) < 2:
@@ -442,14 +443,15 @@
 
 def _ksd(families, sequences, outdir, tmpdir, nthreads, to_stop, cds, pairwise,
         strip_gaps, tree_method,spair, speciestree, reweight, onlyrootout):
     from wgd.core import get_gene_families, SequenceData, KsDistributionBuilder
     from wgd.core import read_gene_families, merge_seqs
     from wgd.viz import default_plot, apply_filters,multi_sp_plot
     start = timer()
+    if tmpdir != None and not os.path.isdir(tmpdir): os.mkdir(tmpdir)
     if len(sequences) == 0: 
         logging.error("Please provide at least one sequence file")
         exit(0)
     if len(sequences) == 2:
         tree_method = "cluster"  # for RBH others don't make sense (and crash)
     seqs = [SequenceData(s, tmp_path=tmpdir, out_path=outdir,
             to_stop=to_stop, cds=cds, threads=nthreads) for s in sequences]
```

### Comparing `wgd-2.0.0/setup.py` & `wgd-2.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,66 +5,71 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='wgd',
-    version='2.0.0',
+    version='2.0.1',
     packages=['wgd'],
     url='http://github.com/heche-psb/wgd',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='wgd',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     py_modules=['cli'],
     include_package_data=True,
     install_requires=[
        'attrs==20.3.0',
        'biopython==1.76',
        'click==7.1.2',
        'colorama==0.4.4',
        'commonmark==0.9.1',
        'cycler==0.10.0',
-       'fastcluster==1.1.25',
+       'fastcluster==1.1.28',
        'humanfriendly==8.2',
        'importlib-metadata==3.1.0',
        'iniconfig==1.1.1',
        'Jinja2==2.11.2',
        'joblib==0.11',
        'KDEpy==1.1.0',
        'kiwisolver==1.2.0',
        'MarkupSafe==1.1.1',
        'matplotlib==3.2.2',
        'numpy>=1.19.0',
+       'numexpr>=2.7.3',
        'packaging==20.4',
-       'pandas>=1.1.0',
-       'Pillow==7.1.2',
+       'pandas<=1.4.4',
+       'Pillow<=8.4.0',
        'pluggy==0.13.1',
        'plumbum==1.6.9',
        'progressbar2==3.51.4',
        'psutil==5.7.0',
        'py==1.9.0',
        'Pygments==2.7.2',
+       'pyqtwebengine<5.13',
+       'pyqt5<5.13',
        'pyparsing==2.4.7',
        'pytest==6.1.2',
-       'python-dateutil==2.8.1',
+       'python-dateutil>=2.8.2',
        'python-utils==2.4.0',
        'pytz==2020.1',
        'PyYAML==5.3.1',
-       'rich==9.3.0',
+       'rich==12.5.1',
        'scikit-learn==0.23.1',
        'scikit-learn-extra==0.2.0',
-       'scipy>=1.5.0',
+       'scipy<=1.5.4',
        'seaborn==0.10.1',
        'six==1.15.0',
        'threadpoolctl==2.1.0',
        'toml==0.10.2',
        'tornado==6.0.4',
-       'typing-extensions==3.7.4.3',
+       'typing-extensions>=3.10.0.0',
        'zipp==3.4.0'
     ],
     entry_points='''
         [console_scripts]
         wgd=cli:cli
     ''',
 )
```

### Comparing `wgd-2.0.0/test/test_core.py` & `wgd-2.0.1/test/test_core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.0/wgd/__init__.py` & `wgd-2.0.1/wgd/__init__.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.0/wgd/beast.py` & `wgd-2.0.1/wgd/beast.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.0/wgd/cluster.py` & `wgd-2.0.1/wgd/cluster.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.0/wgd/codeml.py` & `wgd-2.0.1/wgd/codeml.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.0/wgd/core.py` & `wgd-2.0.1/wgd/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 from concurrent.futures import ProcessPoolExecutor
 from wgd.codeml import Codeml
 from wgd.cluster import cluster_ks #fastcluster is not compatible with some versions of numpy which causes problems for python3.8 and higher
 from wgd.mcmctree import mcmctree
 from wgd.beast import beast
 from timeit import default_timer as timer
 import copy
-import psutil
+#import psutil
 from scipy.cluster.hierarchy import dendrogram, linkage
 from scipy import stats
 from sklearn.cluster import AgglomerativeClustering
 import matplotlib.pyplot as plt
 # Reconsider the renaming, more a pain than helpful?
 
 # helper functions
-def memory_reporter():
-    d = psutil.virtual_memory()
-    logging.info("Available memory for processes : {}GB ".format(d[1]/1e9))
-    logging.info("Memory usage in percent : {}% ".format(d[2]))
-    logging.info("The memory used : {}GB ".format(d[3]/1e9))
-    logging.info("The memory not used but readily available : {}GB ".format(d[4]/1e9))
+#def memory_reporter():
+#    d = psutil.virtual_memory()
+#    logging.info("Available memory for processes : {}GB ".format(d[1]/1e9))
+#    logging.info("Memory usage in percent : {}% ".format(d[2]))
+#    logging.info("The memory used : {}GB ".format(d[3]/1e9))
+#    logging.info("The memory not used but readily available : {}GB ".format(d[4]/1e9))
 
 def _write_fasta(fname, seq_dict):
     with open(fname, "w") as f:
         for k, v in seq_dict.items():
             f.write(">{}\n{}\n".format(k, v.seq))
     return fname
 
@@ -236,14 +236,16 @@
     class that bundles sequence manipulation methods.
     """
     def __init__(self, cds_fasta,
             tmp_path=None, out_path="wgd_dmd",
             to_stop=True, cds=True, cscore=None,threads = 4, bins = 100, normalizedpercent = 5, nonormalization=False):
         if tmp_path == None:
             tmp_path = "wgdtmp_" + str(uuid.uuid4())
+        else:
+            tmp_path = tmp_path + "/"+ "wgdtmp_" + str(uuid.uuid4())
         self.np = normalizedpercent
         self.tmp_path  = _mkdir(tmp_path)
         self.out_path  = _mkdir(out_path)
         self.cds_fasta = cds_fasta
         self.prefix    = os.path.basename(self.cds_fasta)
         self.pro_fasta = os.path.join(tmp_path, self.prefix + ".tfa")
         self.pro_db    = os.path.join(tmp_path, self.prefix + ".db")
```

### Comparing `wgd-2.0.0/wgd/mcmctree.py` & `wgd-2.0.1/wgd/mcmctree.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.0/wgd/mix.py` & `wgd-2.0.1/wgd/mix.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.0/wgd/peak.py` & `wgd-2.0.1/wgd/peak.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.0/wgd/syn.py` & `wgd-2.0.1/wgd/syn.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.0/wgd/utils.py` & `wgd-2.0.1/wgd/utils.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.0/wgd/viz.py` & `wgd-2.0.1/wgd/viz.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.0/wgd.egg-info/requires.txt` & `wgd-2.0.1/wgd.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 attrs==20.3.0
 biopython==1.76
 click==7.1.2
 colorama==0.4.4
 commonmark==0.9.1
 cycler==0.10.0
-fastcluster==1.1.25
+fastcluster==1.1.28
 humanfriendly==8.2
 importlib-metadata==3.1.0
 iniconfig==1.1.1
 Jinja2==2.11.2
 joblib==0.11
 KDEpy==1.1.0
 kiwisolver==1.2.0
 MarkupSafe==1.1.1
 matplotlib==3.2.2
 numpy>=1.19.0
+numexpr>=2.7.3
 packaging==20.4
-pandas>=1.1.0
-Pillow==7.1.2
+pandas<=1.4.4
+Pillow<=8.4.0
 pluggy==0.13.1
 plumbum==1.6.9
 progressbar2==3.51.4
 psutil==5.7.0
 py==1.9.0
 Pygments==2.7.2
+pyqtwebengine<5.13
+pyqt5<5.13
 pyparsing==2.4.7
 pytest==6.1.2
-python-dateutil==2.8.1
+python-dateutil>=2.8.2
 python-utils==2.4.0
 pytz==2020.1
 PyYAML==5.3.1
-rich==9.3.0
+rich==12.5.1
 scikit-learn==0.23.1
 scikit-learn-extra==0.2.0
-scipy>=1.5.0
+scipy<=1.5.4
 seaborn==0.10.1
 six==1.15.0
 threadpoolctl==2.1.0
 toml==0.10.2
 tornado==6.0.4
-typing-extensions==3.7.4.3
+typing-extensions>=3.10.0.0
 zipp==3.4.0
```

