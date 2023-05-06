# Comparing `tmp/luna-0.12.2.tar.gz` & `tmp/luna-0.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/luna-0.12.2.tar", last modified: Wed Oct 12 17:56:30 2022, max compression
+gzip compressed data, was "dist/luna-0.13.0.tar", last modified: Sat May  6 21:57:40 2023, max compression
```

## Comparing `luna-0.12.2.tar` & `luna-0.13.0.tar`

### file list

```diff
@@ -1,126 +1,149 @@
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:30.000000 luna-0.12.2/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1203 2022-04-11 17:24:17.000000 luna-0.12.2/LICENSE
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      142 2022-10-12 11:34:30.000000 luna-0.12.2/MANIFEST.in
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5677 2022-10-12 17:56:30.000000 luna-0.12.2/PKG-INFO
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4292 2022-10-06 13:43:51.000000 luna-0.12.2/README.rst
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:29.000000 luna-0.12.2/luna/
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:29.000000 luna-0.12.2/luna/MyBio/
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:30.000000 luna-0.12.2/luna/MyBio/PDB/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4087 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/AbstractPropertyMap.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11839 2022-07-01 19:27:47.000000 luna-0.12.2/luna/MyBio/PDB/Atom.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5593 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/Chain.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    19116 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/DSSP.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2695 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/Dice.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11663 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/Entity.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    13625 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/FTMapParser.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9923 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/FragmentMapper.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11628 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/HSExposure.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2306 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/MMCIF2Dict.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    18386 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/MMCIFParser.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2571 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/Model.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7538 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/NACCESS.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5146 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/NeighborSearch.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      556 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/PDBExceptions.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14196 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/PDBIO.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    20725 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/PDBList.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    22895 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/PDBParser.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3339 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/PSEA.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14359 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/Polypeptide.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    10467 2022-09-22 19:25:28.000000 luna-0.12.2/luna/MyBio/PDB/Residue.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    23405 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/ResidueDepth.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2949 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/Selection.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1917 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/Structure.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3573 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/StructureAlignment.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14154 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/StructureBuilder.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2265 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/Superimposer.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9473 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/Vector.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2101 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     8731 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/PDB/parse_pdb_header.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2746 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/extractor.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3537 2022-07-01 19:31:33.000000 luna-0.12.2/luna/MyBio/selector.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    28509 2022-10-12 11:34:30.000000 luna-0.12.2/luna/MyBio/util.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      954 2022-04-11 17:24:17.000000 luna-0.12.2/luna/MyBio/version_control.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)       83 2022-04-11 17:24:17.000000 luna-0.12.2/luna/__init__.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:30.000000 luna-0.12.2/luna/align/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:17.000000 luna-0.12.2/luna/align/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     8853 2022-04-11 17:24:17.000000 luna-0.12.2/luna/align/tmalign.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:30.000000 luna-0.12.2/luna/analysis/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:17.000000 luna-0.12.2/luna/analysis/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6027 2022-04-11 17:24:17.000000 luna-0.12.2/luna/analysis/residues.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2971 2022-04-11 17:24:17.000000 luna-0.12.2/luna/analysis/summary.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:30.000000 luna-0.12.2/luna/config/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-05 18:25:54.000000 luna-0.12.2/luna/config/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1008 2022-10-05 18:25:54.000000 luna-0.12.2/luna/config/default.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    20109 2022-10-06 13:43:23.000000 luna-0.12.2/luna/config/params.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:30.000000 luna-0.12.2/luna/data/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6803 2022-04-11 17:24:17.000000 luna-0.12.2/luna/data/BaseFeatures.fdef
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6982 2022-04-11 17:24:17.000000 luna-0.12.2/luna/data/BaseFeatures_DIP2_NoMicrospecies.fdef
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    32050 2022-10-10 17:32:08.000000 luna-0.12.2/luna/data/LUNA.fdef
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1669 2022-04-11 17:24:17.000000 luna-0.12.2/luna/data/MinimalFeatures.fdef
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)  4170251 2022-04-11 17:24:18.000000 luna-0.12.2/luna/data/ligand_expo.tsv
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9049 2022-07-13 19:01:51.000000 luna-0.12.2/luna/data/precomputed_residue_atom_features.json
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:30.000000 luna-0.12.2/luna/interaction/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.12.2/luna/interaction/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2434 2022-10-05 18:25:54.000000 luna-0.12.2/luna/interaction/bind.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)   136894 2022-10-06 13:43:23.000000 luna-0.12.2/luna/interaction/calc.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7018 2022-10-05 18:25:54.000000 luna-0.12.2/luna/interaction/config.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2526 2022-10-06 13:43:23.000000 luna-0.12.2/luna/interaction/config.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    12587 2022-10-12 11:34:30.000000 luna-0.12.2/luna/interaction/contact.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      308 2022-10-05 18:25:54.000000 luna-0.12.2/luna/interaction/filter.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    26953 2022-10-12 17:50:10.000000 luna-0.12.2/luna/interaction/filter.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:30.000000 luna-0.12.2/luna/interaction/fp/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.12.2/luna/interaction/fp/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    40108 2022-10-11 20:10:42.000000 luna-0.12.2/luna/interaction/fp/fingerprint.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    48644 2022-10-06 13:43:23.000000 luna-0.12.2/luna/interaction/fp/shell.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      453 2022-10-12 11:34:30.000000 luna-0.12.2/luna/interaction/fp/type.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6689 2022-10-12 11:34:30.000000 luna-0.12.2/luna/interaction/fp/view.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    19173 2022-04-11 17:24:18.000000 luna-0.12.2/luna/interaction/type.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9862 2022-10-06 12:19:22.000000 luna-0.12.2/luna/interaction/view.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:30.000000 luna-0.12.2/luna/mol/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.12.2/luna/mol/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9999 2022-10-12 11:34:30.000000 luna-0.12.2/luna/mol/atom.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5417 2022-04-11 17:24:18.000000 luna-0.12.2/luna/mol/charge_model.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4554 2022-04-11 17:24:18.000000 luna-0.12.2/luna/mol/clustering.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7116 2022-04-11 17:24:18.000000 luna-0.12.2/luna/mol/depiction.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    49597 2022-10-06 13:43:23.000000 luna-0.12.2/luna/mol/entry.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9729 2022-10-12 11:34:30.000000 luna-0.12.2/luna/mol/features.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    12676 2022-10-05 18:25:54.000000 luna-0.12.2/luna/mol/fingerprint.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    48376 2022-10-12 11:34:30.000000 luna-0.12.2/luna/mol/groups.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    80570 2022-10-11 20:10:42.000000 luna-0.12.2/luna/mol/standardiser.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4133 2022-04-11 17:24:18.000000 luna-0.12.2/luna/mol/templates.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    10593 2022-10-12 11:34:30.000000 luna-0.12.2/luna/mol/validator.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    64201 2022-10-11 20:10:42.000000 luna-0.12.2/luna/projects.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    19494 2022-10-05 18:25:54.000000 luna-0.12.2/luna/run.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:30.000000 luna-0.12.2/luna/util/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6256 2022-10-05 18:25:54.000000 luna-0.12.2/luna/util/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1895 2022-10-12 17:31:41.000000 luna-0.12.2/luna/util/config.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9235 2022-10-12 11:34:26.000000 luna-0.12.2/luna/util/default_values.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1434 2022-07-01 19:27:54.000000 luna-0.12.2/luna/util/exceptions.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    10794 2022-10-05 18:25:54.000000 luna-0.12.2/luna/util/file.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9632 2022-10-06 13:43:23.000000 luna-0.12.2/luna/util/jobs.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      433 2022-10-05 18:25:54.000000 luna-0.12.2/luna/util/logging.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3661 2022-10-05 18:25:54.000000 luna-0.12.2/luna/util/logging.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      183 2022-04-11 17:24:18.000000 luna-0.12.2/luna/util/logging_ini.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2728 2022-04-11 17:24:18.000000 luna-0.12.2/luna/util/math.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3226 2022-04-11 17:24:18.000000 luna-0.12.2/luna/util/multiprocessing_logging.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7843 2022-10-05 18:25:54.000000 luna-0.12.2/luna/util/progress_tracker.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6386 2022-04-11 17:24:18.000000 luna-0.12.2/luna/util/stringcase.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      762 2022-10-12 17:56:11.000000 luna-0.12.2/luna/version.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:30.000000 luna-0.12.2/luna/wrappers/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.12.2/luna/wrappers/__init__.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    32914 2022-10-12 11:34:30.000000 luna-0.12.2/luna/wrappers/base.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2123 2022-10-06 13:43:51.000000 luna-0.12.2/luna/wrappers/cgo_arrow.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1628 2022-04-11 17:24:18.000000 luna-0.12.2/luna/wrappers/cif.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5663 2022-10-11 20:17:06.000000 luna-0.12.2/luna/wrappers/obabel.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    35709 2022-10-06 13:43:51.000000 luna-0.12.2/luna/wrappers/pymol.py
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)    12594 2022-04-11 17:24:18.000000 luna-0.12.2/luna/wrappers/rdkit.py
-drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-12 17:56:29.000000 luna-0.12.2/luna.egg-info/
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5677 2022-10-12 17:56:29.000000 luna-0.12.2/luna.egg-info/PKG-INFO
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2792 2022-10-12 17:56:29.000000 luna-0.12.2/luna.egg-info/SOURCES.txt
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        1 2022-10-12 17:56:29.000000 luna-0.12.2/luna.egg-info/dependency_links.txt
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)       43 2022-10-12 17:56:29.000000 luna-0.12.2/luna.egg-info/entry_points.txt
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)      127 2022-10-12 17:56:29.000000 luna-0.12.2/luna.egg-info/requires.txt
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)        5 2022-10-12 17:56:29.000000 luna-0.12.2/luna.egg-info/top_level.txt
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)       38 2022-10-12 17:56:30.000000 luna-0.12.2/setup.cfg
--rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3071 2022-04-11 17:24:18.000000 luna-0.12.2/setup.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1203 2022-04-11 17:24:17.000000 luna-0.13.0/LICENSE
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      142 2023-05-06 18:48:23.000000 luna-0.13.0/MANIFEST.in
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6032 2023-05-06 21:57:40.000000 luna-0.13.0/PKG-INFO
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4647 2023-05-06 18:48:23.000000 luna-0.13.0/README.rst
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/MyBio/
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/MyBio/PDB/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4087 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/AbstractPropertyMap.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    12801 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/PDB/Atom.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5593 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Chain.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    19116 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/DSSP.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2695 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Dice.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11663 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Entity.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    13625 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/FTMapParser.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9923 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/FragmentMapper.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11628 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/HSExposure.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2306 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/MMCIF2Dict.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    18386 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/MMCIFParser.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2614 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/PDB/Model.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7538 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/NACCESS.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5146 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/NeighborSearch.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      556 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/PDBExceptions.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14988 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/PDB/PDBIO.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    20725 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/PDBList.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    22906 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/PDB/PDBParser.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3339 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/PSEA.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14359 2023-04-21 12:53:04.000000 luna-0.13.0/luna/MyBio/PDB/Polypeptide.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    10871 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/PDB/Residue.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    23405 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/ResidueDepth.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2949 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Selection.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1917 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Structure.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3573 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/StructureAlignment.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14154 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/StructureBuilder.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2265 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Superimposer.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9473 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/Vector.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2101 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     8731 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/PDB/parse_pdb_header.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2917 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/extractor.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9607 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/neighbors.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3608 2023-05-06 17:09:37.000000 luna-0.13.0/luna/MyBio/selector.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    19698 2023-05-06 20:52:29.000000 luna-0.13.0/luna/MyBio/util.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      954 2022-04-11 17:24:17.000000 luna-0.13.0/luna/MyBio/version_control.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)       83 2022-04-11 17:24:17.000000 luna-0.13.0/luna/__init__.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/align/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:17.000000 luna-0.13.0/luna/align/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9316 2023-05-06 17:09:37.000000 luna-0.13.0/luna/align/tmalign.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/analysis/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:17.000000 luna-0.13.0/luna/analysis/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6778 2023-05-06 17:09:37.000000 luna-0.13.0/luna/analysis/residues.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3165 2023-05-06 17:09:37.000000 luna-0.13.0/luna/analysis/summary.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/config/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-10-05 18:25:54.000000 luna-0.13.0/luna/config/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1008 2022-10-05 18:25:54.000000 luna-0.13.0/luna/config/default.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    20345 2023-05-06 18:48:23.000000 luna-0.13.0/luna/config/params.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/data/
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/data/.ipynb_checkpoints/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1702 2023-04-28 13:49:04.000000 luna-0.13.0/luna/data/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6803 2022-04-11 17:24:17.000000 luna-0.13.0/luna/data/BaseFeatures.fdef
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6982 2023-04-10 15:02:48.000000 luna-0.13.0/luna/data/BaseFeatures_DIP2_NoMicrospecies.fdef
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    33752 2023-05-06 17:09:37.000000 luna-0.13.0/luna/data/LUNA.fdef
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1669 2022-04-11 17:24:17.000000 luna-0.13.0/luna/data/MinimalFeatures.fdef
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)  4170251 2022-04-11 17:24:18.000000 luna-0.13.0/luna/data/ligand_expo.tsv
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9049 2022-07-13 19:01:51.000000 luna-0.13.0/luna/data/precomputed_residue_atom_features.json
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)   102236 2023-05-06 17:09:37.000000 luna-0.13.0/luna/data/precomputed_residue_data.json
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/docking/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 19:59:06.000000 luna-0.13.0/luna/docking/__init__.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/docking/dock6/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4184 2023-05-06 21:26:36.000000 luna-0.13.0/luna/docking/dock6/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4705 2023-05-06 19:59:06.000000 luna-0.13.0/luna/docking/dock6/default.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11148 2023-05-06 19:59:06.000000 luna-0.13.0/luna/docking/dock6/ligands.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1623 2023-05-06 19:59:06.000000 luna-0.13.0/luna/docking/dock6/params.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/interaction/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.13.0/luna/interaction/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2434 2022-10-05 18:25:54.000000 luna-0.13.0/luna/interaction/bind.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)   157331 2023-05-06 18:48:23.000000 luna-0.13.0/luna/interaction/calc.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7066 2023-05-06 17:09:37.000000 luna-0.13.0/luna/interaction/config.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2951 2023-05-06 18:48:23.000000 luna-0.13.0/luna/interaction/config.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14309 2023-05-06 17:09:37.000000 luna-0.13.0/luna/interaction/contact.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1721 2023-05-06 17:09:37.000000 luna-0.13.0/luna/interaction/cov.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      308 2022-10-05 18:25:54.000000 luna-0.13.0/luna/interaction/filter.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    27574 2023-05-06 18:48:23.000000 luna-0.13.0/luna/interaction/filter.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/interaction/fp/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.13.0/luna/interaction/fp/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    42211 2023-05-06 18:48:23.000000 luna-0.13.0/luna/interaction/fp/fingerprint.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    52388 2023-05-06 19:42:57.000000 luna-0.13.0/luna/interaction/fp/shell.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      542 2023-05-06 17:09:37.000000 luna-0.13.0/luna/interaction/fp/type.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6724 2023-05-06 18:48:23.000000 luna-0.13.0/luna/interaction/fp/view.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    20615 2023-05-06 17:09:37.000000 luna-0.13.0/luna/interaction/type.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11615 2023-05-06 18:48:23.000000 luna-0.13.0/luna/interaction/view.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/mol/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.13.0/luna/mol/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    10165 2023-05-06 18:48:23.000000 luna-0.13.0/luna/mol/atom.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     5464 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/charge_model.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4678 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/clustering.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7793 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/depiction.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    56156 2023-05-06 18:48:23.000000 luna-0.13.0/luna/mol/entry.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9823 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/features.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    13252 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/fingerprint.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    56203 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/groups.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1149 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/precomp_data.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    55074 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/standardiser.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4744 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/templates.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    22804 2023-05-06 17:09:37.000000 luna-0.13.0/luna/mol/validator.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    64690 2023-05-06 17:09:37.000000 luna-0.13.0/luna/projects.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    19360 2023-05-06 18:48:23.000000 luna-0.13.0/luna/run.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/util/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6256 2022-10-05 18:25:54.000000 luna-0.13.0/luna/util/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2185 2023-05-06 18:48:23.000000 luna-0.13.0/luna/util/config.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     9496 2023-05-06 20:09:15.000000 luna-0.13.0/luna/util/default_values.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1580 2023-05-06 19:59:06.000000 luna-0.13.0/luna/util/exceptions.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    11071 2023-05-06 17:09:37.000000 luna-0.13.0/luna/util/file.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    10054 2023-05-06 17:09:37.000000 luna-0.13.0/luna/util/jobs.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      433 2022-10-05 18:25:54.000000 luna-0.13.0/luna/util/logging.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3590 2023-05-06 17:09:37.000000 luna-0.13.0/luna/util/logging.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      183 2022-04-11 17:24:18.000000 luna-0.13.0/luna/util/logging_ini.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2728 2022-04-11 17:24:18.000000 luna-0.13.0/luna/util/math.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3294 2023-05-06 17:09:37.000000 luna-0.13.0/luna/util/multiprocessing_logging.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     8153 2023-05-06 17:09:37.000000 luna-0.13.0/luna/util/progress_tracker.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6386 2022-04-11 17:24:18.000000 luna-0.13.0/luna/util/stringcase.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      762 2023-05-06 18:09:52.000000 luna-0.13.0/luna/version.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/wrappers/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2022-04-11 17:24:18.000000 luna-0.13.0/luna/wrappers/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     4003 2023-05-06 19:59:06.000000 luna-0.13.0/luna/wrappers/antechamber.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    36639 2023-05-06 20:48:45.000000 luna-0.13.0/luna/wrappers/base.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2123 2022-10-06 13:43:51.000000 luna-0.13.0/luna/wrappers/cgo_arrow.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/wrappers/chemaxon/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 19:59:06.000000 luna-0.13.0/luna/wrappers/chemaxon/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6300 2023-05-06 21:03:44.000000 luna-0.13.0/luna/wrappers/chemaxon/conformer.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     2727 2023-05-06 20:05:05.000000 luna-0.13.0/luna/wrappers/chemaxon/stereoisomers.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     8454 2023-05-06 20:04:50.000000 luna-0.13.0/luna/wrappers/chemaxon/tautomers.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      281 2023-05-06 19:59:06.000000 luna-0.13.0/luna/wrappers/chemaxon/util.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna/wrappers/chimera/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1558 2023-05-06 19:59:06.000000 luna-0.13.0/luna/wrappers/chimera/__init__.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1395 2023-05-06 19:59:06.000000 luna-0.13.0/luna/wrappers/chimera/add_charges.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     1628 2022-04-11 17:24:18.000000 luna-0.13.0/luna/wrappers/cif.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     7313 2023-05-06 20:44:51.000000 luna-0.13.0/luna/wrappers/obabel.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    37884 2023-05-06 17:09:37.000000 luna-0.13.0/luna/wrappers/pymol.py
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)    14407 2023-05-06 17:09:37.000000 luna-0.13.0/luna/wrappers/rdkit.py
+drwxrwxrwx   0 afassio   (1000) afassio   (1000)        0 2023-05-06 21:57:40.000000 luna-0.13.0/luna.egg-info/
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     6032 2023-05-06 21:57:39.000000 luna-0.13.0/luna.egg-info/PKG-INFO
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3384 2023-05-06 21:57:39.000000 luna-0.13.0/luna.egg-info/SOURCES.txt
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        1 2023-05-06 21:57:39.000000 luna-0.13.0/luna.egg-info/dependency_links.txt
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)       43 2023-05-06 21:57:39.000000 luna-0.13.0/luna.egg-info/entry_points.txt
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)      127 2023-05-06 21:57:39.000000 luna-0.13.0/luna.egg-info/requires.txt
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)        5 2023-05-06 21:57:39.000000 luna-0.13.0/luna.egg-info/top_level.txt
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)       38 2023-05-06 21:57:40.000000 luna-0.13.0/setup.cfg
+-rwxrwxrwx   0 afassio   (1000) afassio   (1000)     3071 2022-04-11 17:24:18.000000 luna-0.13.0/setup.py
```

### Comparing `luna-0.12.2/LICENSE` & `luna-0.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/PKG-INFO` & `luna-0.13.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: luna
-Version: 0.12.2
+Version: 0.13.0
 Summary: LUNA: drug discovery toolkit
 Home-page: https://github.com/keiserlab/LUNA
-Download-URL: https://github.com/keiserlab/LUNA/tarball/v0.12.2
+Download-URL: https://github.com/keiserlab/LUNA/tarball/v0.13.0
 Author: Alexandre Fassio
 Author-email: afassio@keiserlab.org
 License: MIT
 Project-URL: Bug Reports, https://github.com/keiserlab/LUNA/issues
 Project-URL: Source, https://github.com/keiserlab/LUNA/
 Keywords: luna eifp fifp hifp ifp interaction fingerprint protein-ligand molecule docking
 Platform: UNKNOWN
@@ -42,17 +42,31 @@
 
 Documentation is hosted by ReadTheDocs_, and development occurs on GitHub_.
 
 
 Installation and Usage
 ----------------------
 
-For installation and usage instructions, see the `documentation <http://luna-toolkit.readthedocs.io>`_.
+The latest stable release (and required dependencies) can be installed as follows:
 
-See the LUNA `paper repository`_ for an application of LUNA and all code used for the LUNA paper [1]_.
+1. Download LUNA’s `environment.yml <https://github.com/keiserlab/LUNA/blob/master/luna-env.yml>`_ file.
+
+2. Create the Conda environment using the downloaded file:
+
+    conda env create -f <LUNA-ENV-FILE>
+
+3. After creating the Conda environment, activate it:
+
+    conda activate luna-env
+
+4. Finally, install LUNA from Pip:
+
+    pip install luna
+
+For additional installation options and usage instructions, refer to the `documentation <http://luna-toolkit.readthedocs.io>`_.
 
 
 License
 -------
 
 LUNA is available under the |license|.
```

### Comparing `luna-0.12.2/README.rst` & `luna-0.13.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -9,17 +9,31 @@
 
 Documentation is hosted by ReadTheDocs_, and development occurs on GitHub_.
 
 
 Installation and Usage
 ----------------------
 
-For installation and usage instructions, see the `documentation <http://luna-toolkit.readthedocs.io>`_.
+The latest stable release (and required dependencies) can be installed as follows:
 
-See the LUNA `paper repository`_ for an application of LUNA and all code used for the LUNA paper [1]_.
+1. Download LUNA’s `environment.yml <https://github.com/keiserlab/LUNA/blob/master/luna-env.yml>`_ file.
+
+2. Create the Conda environment using the downloaded file:
+
+    conda env create -f <LUNA-ENV-FILE>
+
+3. After creating the Conda environment, activate it:
+
+    conda activate luna-env
+
+4. Finally, install LUNA from Pip:
+
+    pip install luna
+
+For additional installation options and usage instructions, refer to the `documentation <http://luna-toolkit.readthedocs.io>`_.
 
 
 License
 -------
 
 LUNA is available under the |license|.
```

### Comparing `luna-0.12.2/luna/MyBio/PDB/AbstractPropertyMap.py` & `luna-0.13.0/luna/MyBio/PDB/AbstractPropertyMap.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/Atom.py` & `luna-0.13.0/luna/MyBio/PDB/Atom.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,29 @@
         self.serial_number = serial_number
         # Dictionary that keeps additional properties
         self.xtra = {}
         assert not element or element == element.upper(), element
         self.element = self._assign_element(element)
         self.mass = self._assign_atom_mass()
 
+        self.metal_coordination = set()
+
+    @property
+    def full_name(self):
+        full_name = "%s/%s/%s" % self.get_full_id()[0:3]
+        res_name = "%s/%d%s" % (self.parent.resname,
+                                self.parent.id[1],
+                                self.parent.id[2].strip())
+        atom_name = "%s" % self.name
+        if self.altloc != " ":
+            atom_name += "-%s" % self.altloc
+        full_name += "/%s/%s" % (res_name, atom_name)
+
+        return full_name
+
     def _assign_element(self, element):
         """Tries to guess element from atom name if not recognised."""
         if not element or element.capitalize() not in IUPACData.atom_weights:
             # Inorganic elements have their name shifted left by one position
             #  (is a convention in PDB, but not part of the standard).
             # isdigit() check on last two characters to avoid mis-assignment of
             # hydrogens atoms (GLN HE21 for example)
@@ -147,15 +162,25 @@
         """
         diff = self.coord - other.coord
         return numpy.sqrt(numpy.dot(diff, diff))
 
     # MODBY: Alexandre Fassio.
     # __lt__ method overwritten.
     def __lt__(self, a2):
-        return self.id < a2.id
+
+        # I have substituted the residue id for its index in order 
+        # to keep the same order as in the PDB.
+        full_id1 = (self.get_full_id()[0:3] + 
+                    (self.parent.idx, ) +
+                    self.get_full_id()[4:])
+        full_id2 = (a2.get_full_id()[0:3] +
+                    (a2.parent.idx, ) +
+                    a2.get_full_id()[4:])
+
+        return full_id1 < full_id2
 
     # set methods
 
     def set_serial_number(self, n):
         self.serial_number = n
 
     def set_bfactor(self, bfactor):
@@ -288,14 +313,17 @@
     def get_altloc(self):
         """Return alternative location specifier."""
         return self.altloc
 
     def get_level(self):
         return self.level
 
+    def has_metal_coordination(self):
+        return len(self.metal_coordination) > 0
+
     def transform(self, rot, tran):
         """Apply rotation and translation to the atomic coordinates.
 
         Example:
 
             >>> rotation=rotmat(pi, Vector(1, 0, 0))
             >>> translation=array((0, 0, 1), 'f')
```

### Comparing `luna-0.12.2/luna/MyBio/PDB/Chain.py` & `luna-0.13.0/luna/MyBio/PDB/Chain.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/DSSP.py` & `luna-0.13.0/luna/MyBio/PDB/DSSP.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/Dice.py` & `luna-0.13.0/luna/MyBio/PDB/Dice.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/Entity.py` & `luna-0.13.0/luna/MyBio/PDB/Entity.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/FTMapParser.py` & `luna-0.13.0/luna/MyBio/PDB/FTMapParser.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/FragmentMapper.py` & `luna-0.13.0/luna/MyBio/PDB/FragmentMapper.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/HSExposure.py` & `luna-0.13.0/luna/MyBio/PDB/HSExposure.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/MMCIF2Dict.py` & `luna-0.13.0/luna/MyBio/PDB/MMCIF2Dict.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/MMCIFParser.py` & `luna-0.13.0/luna/MyBio/PDB/MMCIFParser.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/Model.py` & `luna-0.13.0/luna/MyBio/PDB/Model.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,11 +89,12 @@
             yield c
 
     def get_residues(self):
         for c in self.get_chains():
             for r in c:
                 yield r
 
+    # MODBY: Alexandre
     def get_atoms(self):
         for r in self.get_residues():
-            for a in r:
+            for a in r.get_unpacked_list():
                 yield a
```

### Comparing `luna-0.12.2/luna/MyBio/PDB/NACCESS.py` & `luna-0.13.0/luna/MyBio/PDB/NACCESS.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/NeighborSearch.py` & `luna-0.13.0/luna/MyBio/PDB/NeighborSearch.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/PDBExceptions.py` & `luna-0.13.0/luna/MyBio/PDB/PDBExceptions.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/PDBIO.py` & `luna-0.13.0/luna/MyBio/PDB/PDBIO.py`

 * *Files 10% similar despite different names*

```diff
@@ -188,16 +188,43 @@
             structure = sb.structure
 
         # MODBY: Alexandre Fassio
         # Set the copied CONECTs to the new Structure object.
         structure.conects = conects
         self.structure = structure
 
+    def _get_list(self, entity, sort=False):
+        # S -> M
+        # M -> C
+        if entity.get_level() in ["S", "M"]:
+            the_list = entity.get_list()
+
+            # Sort Models/Chains by id.
+            if sort:
+                return sorted(the_list, key=lambda x: x.id)
+
+        # C -> R
+        elif entity.get_level() == "C":
+            the_list = entity.get_unpacked_list()
+
+            # Sort residues by index, i.e., by their order in a PDB chain.
+            if sort:
+                return sorted(the_list, key=lambda x: x.idx)
+
+        # R -> A
+        #
+        #   Always keep atoms order as in PDB.
+        #
+        elif entity.get_level() == "R":
+            the_list = entity.get_unpacked_list()
+
+        return the_list
+
     def save(self, file, select=Select(), write_conects=False,
-             write_end=True, preserve_atom_numbering=False):
+             write_end=True, preserve_atom_numbering=False, sort=False):
         """
         @param select: selects which entities will be written.
         @type select: object
 
         Typically select is a subclass of L{Select}, it should
         have the following methods:
 
@@ -226,40 +253,41 @@
         serial_number_mapping = {}
 
         # multiple models?
         if len(self.structure) > 1 or self.use_model_flag:
             model_flag = 1
         else:
             model_flag = 0
-        for model in self.structure.get_list():
+
+        for model in self._get_list(self.structure, sort):
             if not select.accept_model(model):
                 continue
             # necessary for ENDMDL
             # do not write ENDMDL if no residues were written
             # for this model
             model_residues_written = 0
             if not preserve_atom_numbering:
                 atom_number = 1
             if model_flag:
                 fp.write("MODEL      %s\n" % model.serial_num)
-            for chain in model.get_list():
+            for chain in self._get_list(model, sort):
                 if not select.accept_chain(chain):
                     continue
                 chain_id = chain.get_id()
                 # necessary for TER
                 # do not write TER if no residues were written
                 # for this chain
                 chain_residues_written = 0
-                for residue in chain.get_unpacked_list():
+                for residue in self._get_list(chain, sort):
                     if not select.accept_residue(residue):
                         continue
                     hetfield, resseq, icode = residue.get_id()
                     resname = residue.get_resname()
                     segid = residue.get_segid()
-                    for atom in residue.get_unpacked_list():
+                    for atom in self._get_list(residue, sort):
                         if select.accept_atom(atom):
                             chain_residues_written = 1
                             model_residues_written = 1
 
                             if preserve_atom_numbering:
                                 atom_number = atom.get_serial_number()
 
@@ -294,15 +322,14 @@
             if model_flag and model_residues_written:
                 fp.write("ENDMDL\n")
 
         # MODBY: Alexandre Fassio
         # Print CONECT records
         if write_conects:
             conects = self.structure.conects
-
             for serial_number in sorted(conects):
                 # Substitutes the old serial number by the new serial number
                 new_serial_number = serial_number_mapping.get(serial_number, None)
 
                 if new_serial_number not in valid_serial_numbers:
                     continue
```

### Comparing `luna-0.12.2/luna/MyBio/PDB/PDBList.py` & `luna-0.13.0/luna/MyBio/PDB/PDBList.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/PDBParser.py` & `luna-0.13.0/luna/MyBio/PDB/PDBParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 from luna.MyBio.PDB.parse_pdb_header import _parse_pdb_header_list
 
 
 # MODBY: Alexandre Fassio
 # Possible labels for water molecules.
 # Ref: http://prody.csb.pitt.edu/manual/reference/atomic/flags.html.
 # DOD: deutered water.
-WATER_NAMES = ['HOH', 'DOD', 'WAT', 'H2O', 'OH2']
+WATER_NAMES = ['HOH', 'DOD', 'WAT', 'H2O', 'OH', 'OH2', "O"]
 
 # MODBY: Alexandre Fassio
 # Replace empty chains for a default value.
 DEFAULT_CHAIN_ID = "z"
 
 
 # If PDB spec says "COLUMNS 18-20" this means line[17:20]
```

### Comparing `luna-0.12.2/luna/MyBio/PDB/PSEA.py` & `luna-0.13.0/luna/MyBio/PDB/PSEA.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/Polypeptide.py` & `luna-0.13.0/luna/MyBio/PDB/Polypeptide.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/Residue.py` & `luna-0.13.0/luna/MyBio/PDB/Residue.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,14 +138,22 @@
     @property
     def full_name(self):
         full_name = "%s/%s/%s" % self.get_full_id()[0:3]
         res_name = "%s/%d%s" % (self.resname, self.id[1], self.id[2].strip())
         full_name += "/%s" % res_name
         return full_name
 
+    @property
+    def metal_coordination(self):
+        metal_coordination = {}
+        for a in self.get_atoms():
+            if a.has_metal_coordination():
+                metal_coordination[a] = a.metal_coordination
+        return metal_coordination
+
     def add(self, atom):
         """Add an Atom object.
 
         Checks for adding duplicate atoms, and raises a
         PDBConstructionException if so.
         """
         atom_id = atom.get_id()
@@ -168,37 +176,42 @@
     # MODBY: Alexandre Fassio
     # Check if a residue is a water.
     def is_water(self):
         """Return 1 if the residue is a water molecule."""
         return self.get_id()[0] == "W"
 
     # MODBY: Alexandre Fassio
+    # Check if a compound is a metal.
+    def is_metal(self):
+        """Return True if the residue is a metal."""
+        return (self.get_id()[0].startswith("H_")
+                and self.resname in METALS)
+
+    # MODBY: Alexandre Fassio
     # Check if a compound is a hetero group.
     def is_hetatm(self):
         """Return True if the residue is an hetero group."""
-        return self.get_id()[0].startswith("H_")
-
-    def is_metal(self):
-        """Return True if the residue is a metal."""
-        return self.is_hetatm() and self.resname in METALS
+        return (self.get_id()[0].startswith("H_")
+                and not self.is_metal())
 
     # MODBY: Alexandre Fassio
     # Check if a residue is an amino acid.
     def is_residue(self):
         """Return True if the residue is an amino acid."""
         return self.get_id()[0] == " " and is_aa(self.resname)
 
     # MODBY: Alexandre Fassio
     # Check if a residue is a nucleotide.
     def is_nucleotide(self):
         """Return True if the residue is a nucleic acid."""
         return self.get_id()[0] == " " and not self.is_residue()
 
     # MODBY: Alexandre Fassio
-    # Check if a residue is a target, i.e., if it will be used for any calculations.
+    # Check if a residue is a target, i.e., if it will be
+    # used for any calculations.
     def is_target(self):
         return self._is_target
 
     # MODBY: Alexandre Fassio
     # Get the compound class.
     def get_class(self):
         if self.is_water():
@@ -246,15 +259,14 @@
 
     # MODBY: Alexandre Fassio
     # Define if the residue is a target or not.
     def set_as_target(self, is_target=True):
         self._is_target = is_target
 
     def as_json(self):
-
         if self.is_water():
             comp_repr = "sphere"
         elif self.is_hetatm():
             if len(self.child_list) == 1 or len([atm for atm in self.child_list if atm.element != "H"]) == 1:
                 comp_repr = "sphere"
             else:
                 comp_repr = "stick"
```

### Comparing `luna-0.12.2/luna/MyBio/PDB/ResidueDepth.py` & `luna-0.13.0/luna/MyBio/PDB/ResidueDepth.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/Selection.py` & `luna-0.13.0/luna/MyBio/PDB/Selection.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/Structure.py` & `luna-0.13.0/luna/MyBio/PDB/Structure.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/StructureAlignment.py` & `luna-0.13.0/luna/MyBio/PDB/StructureAlignment.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/StructureBuilder.py` & `luna-0.13.0/luna/MyBio/PDB/StructureBuilder.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/Superimposer.py` & `luna-0.13.0/luna/MyBio/PDB/Superimposer.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/Vector.py` & `luna-0.13.0/luna/MyBio/PDB/Vector.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/__init__.py` & `luna-0.13.0/luna/MyBio/PDB/__init__.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/PDB/parse_pdb_header.py` & `luna-0.13.0/luna/MyBio/PDB/parse_pdb_header.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/MyBio/extractor.py` & `luna-0.13.0/luna/MyBio/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,32 @@
 
 
 class Extractor():
     """Extract chains or residues from ``entity``.
 
     Parameters
     ----------
-    entity : :class:`~luna.MyBio.PDB.Entity.Model` or :class:`~luna.MyBio.PDB.Entity.Chain`
-        A model or chain object from where chains and residues will be extracted, respectively.
+    entity : :class:`~luna.MyBio.PDB.Entity.Model` or \
+                :class:`~luna.MyBio.PDB.Entity.Chain`
+        A model or chain object from where chains and residues
+        will be extracted, respectively.
     """
 
     def __init__(self, entity):
         self.entity = entity
 
     @property
     def entity(self):
         return self._entity
 
     @entity.setter
     def entity(self, entity):
         if not isinstance(entity, (Model, Chain)):
-            raise TypeError("Only objects of type %s or %s are accepted." % (Model.__module__, Chain.__module__))
+            raise TypeError("Only objects of type %s or %s are accepted." %
+                            (Model.__module__, Chain.__module__))
         self._entity = entity
 
     def extract_chains(self, chains, output_file):
         """Extract chains from ``entity`` and save it to ``output_file``.
 
         Parameters
         ----------
@@ -47,15 +50,17 @@
             for chain in chains:
                 if chain in self.entity.child_dict:
                     chain_sel.add(self.entity[chain])
                 else:
                     logger.warning("Chain %s does not exist." % chain)
 
             if len(chain_sel) > 0:
-                save_to_file(self.entity, output_file, ChainSelector(chain_sel))
+                save_to_file(self.entity,
+                             output_file,
+                             ChainSelector(chain_sel))
             else:
                 logger.warning("No valid chain to extract.")
 
     def extract_residues(self, residues, output_file):
         """Extract residues from ``entity`` and save it to ``output_file``.
 
         Parameters
@@ -72,10 +77,12 @@
             for res in residues:
                 if res in self.entity.child_dict:
                     res_sel.add(self.entity[res])
                 else:
                     logger.warning("Residue %s does not exist." % str(res))
 
             if len(res_sel) > 0:
-                save_to_file(self.entity, output_file, ResidueSelector(res_sel))
+                save_to_file(self.entity, 
+                             output_file,
+                             ResidueSelector(res_sel))
             else:
                 logger.warning("No valid residue to extract.")
```

### Comparing `luna-0.12.2/luna/MyBio/selector.py` & `luna-0.13.0/luna/MyBio/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,25 @@
 
     Parameters
     ----------
     keep_hydrog : bool
         If True (default), keeps all hydrogens. Otherwise, filter them out.
         Hydrogens are atoms whose element is either "H" or "D" (deuterium).
     keep_altloc : bool
-        If True (default), keeps all atoms. Otherwise, keeps only atoms whose alternate location is in the list ``altloc``.
+        If True (default), keeps all atoms. Otherwise, keeps only atoms whose
+        alternate location is in the list ``altloc``.
     altloc : iterable
-        List of valid alternate location identifiers. The default valid values are "A" and "1".
+        List of valid alternate location identifiers. 
+        The default valid values are "A" and "1".
     """
 
-    def __init__(self, keep_hydrog=True, keep_altloc=True, altloc=DEFAULT_ALTLOC):
+    def __init__(self, 
+                 keep_hydrog=True, 
+                 keep_altloc=True, 
+                 altloc=DEFAULT_ALTLOC):
         self.keep_hydrog = keep_hydrog
         self.keep_altloc = keep_altloc
         self.altloc = altloc
 
     def accept_atom(self, atom):
         """Decide if the atom is valid or not."""
```

### Comparing `luna-0.12.2/luna/MyBio/version_control.py` & `luna-0.13.0/luna/MyBio/version_control.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/align/tmalign.py` & `luna-0.13.0/luna/align/tmalign.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 
 def align_structures(pdb_to_align, ref_pdb, output_path=None, tmalign=None):
     """Align two PDB files with TM-align.
 
     .. warning::
 
         TM-align performs pair-wise structural alignments.
-        Therefore, if your PDB file contains multiple structures, it is recommended
-        you extract the chains first and align them separately, otherwise the alignment
-        may not produce the expected results.
+        Therefore, if your PDB file contains multiple structures, it is
+        recommended you extract the chains first and align them separately,
+        otherwise the alignment may not produce the expected results.
 
         To extract chains you can use :class:`~luna.MyBio.extractor.Extractor`.
 
     Parameters
     ----------
     pdb_to_align : str
         The PDB structure that will be aligned to ``ref_pdb``.
@@ -74,37 +74,43 @@
     Examples
     --------
 
     >>> from luna.util.default_values import LUNA_PATH
     >>> from luna.align.tmalign import align_structures
     >>> pdb1 = "{LUNA_PATH}/tutorial/inputs/3QQF.pdb"
     >>> pdb2 = "{LUNA_PATH}/tutorial/inputs/3QQK.pdb"
-    >>> alignment = align_structures(pdb1, pdb2, "./", tmalign="/media/data/Workspace/Softwares/TMalignc/TMalign")
+    >>> alignment = align_structures(pdb1, pdb2, "./", \
+tmalign="/media/data/Workspace/Softwares/TMalignc/TMalign")
     >>> print(alignment.score)
     0.98582
     """
 
     tmalign = tmalign or TMALIGN
 
-    logger.info("TM-align will try to align the files %s and %s." % (pdb_to_align, ref_pdb))
+    logger.info("TM-align will try to align the files %s and %s."
+                % (pdb_to_align, ref_pdb))
 
     output = _run_tmalign(pdb_to_align, ref_pdb, output_path, tmalign)
 
     seq_pair, tm_score = get_seq_records(output, pdb_to_align, ref_pdb)
 
-    alignment = TMAlignment(tm_score, records=seq_pair, alphabet=generic_protein)
+    alignment = TMAlignment(tm_score,
+                            records=seq_pair,
+                            alphabet=generic_protein)
 
-    logger.info("TM-align finished successfully. %s." % alignment[0].description)
+    logger.info("TM-align finished successfully. %s."
+                % alignment[0].description)
 
     return alignment
 
 
 def _run_tmalign(file1, file2, output_path, tmalign):
 
-    logger.debug("It will try to execute the command: '%s %s %s'." % (tmalign, file1, file2))
+    logger.debug("It will try to execute the command: '%s %s %s'."
+                 % (tmalign, file1, file2))
 
     for fname in (file1, file2):
         if not os.path.isfile(fname):
             logging.error("Missing file: %s", fname)
             raise FileNotFoundError("Missing file: %s", fname)
 
     try:
@@ -119,21 +125,23 @@
         else:
             args = [tmalign, file1, file2]
 
         output = subprocess.check_output(args)
     except subprocess.CalledProcessError as e:
         logger.exception(e)
 
-        raise RuntimeError("TMalign failed for PDB files: %s and %s" % (file1, file2))
+        raise RuntimeError("TMalign failed for PDB files: %s and %s"
+                           % (file1, file2))
 
     return output.decode()
 
 
 def get_seq_records(tm_output, aligned_pdb_id, ref_pdb_id):
-    """Create a pair of :class:`Bio.SeqRecord.SeqRecord` from a TM-align output.
+    """Create a pair of :class:`Bio.SeqRecord.SeqRecord` from a
+    TM-align output.
 
     Parameters
     ----------
     tm_output : str
         The output produced by TM-align.
     aligned_pdb_id : str
         An identifier for the aligned PDB file.
@@ -165,61 +173,75 @@
     last_lines = lines[-7:]
 
     assert last_lines[0].startswith('(":"')  # (":" denotes the residues pairs
     assert last_lines[-1].startswith('Total running time is')
 
     aligned_seq, ref_seq = last_lines[1].strip(), last_lines[3].strip()
 
-    return (SeqRecord(Seq(aligned_seq), id=aligned_pdb_id, description="TM-score=%f" % tm_score),
-            SeqRecord(Seq(ref_seq), id=ref_pdb_id, description="TM-score=%f" % tm_score)), tm_score
+    return (SeqRecord(Seq(aligned_seq),
+                      id=aligned_pdb_id,
+                      description="TM-score=%f" % tm_score),
+            SeqRecord(Seq(ref_seq),
+                      id=ref_pdb_id,
+                      description="TM-score=%f" % tm_score)), tm_score
 
 
-def extract_chain_from_sup(sup_file, extract_chain, output_file, new_chain_id=None, QUIET=True):
+def extract_chain_from_sup(sup_file,
+                           extract_chain,
+                           output_file,
+                           new_chain_id=None,
+                           QUIET=True):
     """ Extract a chain from the superposition file generated by TM-align.
 
         .. warning::
             TM-align modifies the id of the original chains, so it is highly
             recommended to rename it to match the original chain id.
             To do so, use the parameter ``new_chain_id``.
 
         Parameters
         ----------
         sup_file: str
             A superposition file generated by TM-align.
         extract_chain: {'A', 'B'}
-            Target chain id to be extracted. TM-align performs pair-wise structural alignment,
-            so the output file will always contain two chains 'A' and 'B',
-            where 'A' and 'B' are the aligned and reference structures, respectively.
+            Target chain id to be extracted. TM-align performs pair-wise
+            structural alignment, so the output file will always contain
+            two chains 'A' and 'B', where 'A' and 'B' are the aligned and
+            reference structures, respectively.
         output_file: str
             Save the extracted chain to this file.
         new_chain_id: str, optional
             The new chain id of the extracted chain.
-            If not provided, the chain ids will be maintained as it is in the TM-align output.
+            If not provided, the chain ids will be maintained as it is in the
+            TM-align output.
         QUIET: bool
-            If True (the default), mute warning messages generated by Biopython.
+            If True (the default), mute warning messages generated by
+            Biopython.
     """
     if QUIET:
         try:
             warnings.filterwarnings("ignore")
-            logger.debug("Quiet mode activated. From now on, no warning will be printed.")
+            logger.debug("Quiet mode activated. From now on, no warning will "
+                         "be printed.")
         except Exception:
             logger.warning("Quiet mode could not be activated.")
 
     if extract_chain not in ["A", "B"]:
         raise ValueError("Valid values for 'extract_chain' are 'A' and 'B'.")
 
     try:
         logger.debug("Trying to parse the file '%s'." % sup_file)
 
         structure = parse_from_file("SUP", sup_file)
 
         model = structure[0]
         if (len(model.child_list) != 2):
-            raise InvalidSuperpositionFileError("This structure has %d chains. The file generated "
-                                                "by TM-align must have 2 chains." % len(model.child_list))
+            error_msg = ("This structure has %d chains. The file generated "
+                         "by TM-align must have 2 chains."
+                         % len(model.child_list))
+            raise InvalidSuperpositionFileError(error_msg)
 
         chain_to_remove = 'B' if extract_chain == "A" else "A"
         model.detach_child(chain_to_remove)
 
         if new_chain_id is not None and extract_chain != new_chain_id:
             model[extract_chain].id = new_chain_id
             logger.debug("Modifications completed.")
@@ -229,18 +251,20 @@
         logger.debug("File '%s' created successfully." % output_file)
     except Exception as e:
         logger.exception(e)
         raise
 
 
 def remove_sup_files(path):
-    """ Remove all superposition files created by TM-align at a defined directory ``path``."""
+    """ Remove all superposition files created by TM-align at a defined
+    directory ``path``."""
     try:
         if (is_directory_valid(path)):
-            targets = ['*.sup', '*.sup_atm', '*.sup_all', '*.sup_all_atm', '*.sup_all_atm_lig']
+            targets = ['*.sup', '*.sup_atm', '*.sup_all',
+                       '*.sup_all_atm', '*.sup_all_atm_lig']
 
             for target in targets:
                 files = glob.glob('%s/%s' % (path, target))
                 for file in files:
                     try:
                         remove(file)
                     except Exception as e:
```

### Comparing `luna-0.12.2/luna/analysis/residues.py` & `luna-0.13.0/luna/analysis/residues.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,35 +8,38 @@
 
 
 def generate_residue_matrix(interactions_mngrs, by_interaction=True):
     """Generate a matrix to count interactions per residue.
 
     Parameters
     ----------
-    interactions_mngrs : iterable of :class:`~luna.interaction.calc.InteractionsManager`
-        A sequence of :class:`~luna.interaction.calc.InteractionsManager` objects
-        from where interactions will be recovered.
+    interactions_mngrs : iterable of \
+            :class:`~luna.interaction.calc.InteractionsManager`
+        A sequence of :class:`~luna.interaction.calc.InteractionsManager`
+        objects from where interactions will be recovered.
     by_interaction : bool
-        If True (the default), count the number of each interaction type per residue.
-        Otherwise, count the overall number of interactions per residue.
+        If True (the default), count the number of each interaction type
+        per residue. Otherwise, count the overall number of interactions
+        per residue.
 
     Returns
     -------
      : :class:`pandas.DataFrame`
     """
 
     data_by_entry = defaultdict(lambda: defaultdict(int))
     residues = set()
 
     for inter_mngr in interactions_mngrs:
         entry = inter_mngr.entry
 
         for inter in inter_mngr:
             # Continue if no target is in the interaction.
-            if not inter.src_grp.has_target() and not inter.trgt_grp.has_target():
+            if (not inter.src_grp.has_target()
+                    and not inter.trgt_grp.has_target()):
                 continue
             # Ignore interactions involving the same compounds.
             if inter.src_grp.compounds == inter.trgt_grp.compounds:
                 continue
 
             if inter.src_grp.has_hetatm():
                 comp1 = sorted(inter.src_grp.compounds)
@@ -45,18 +48,26 @@
                 comp1 = sorted(inter.trgt_grp.compounds)
                 comp2 = sorted(inter.src_grp.compounds)
             else:
                 comp1 = sorted(inter.src_grp.compounds)
                 comp2 = sorted(inter.trgt_grp.compounds)
                 comp1, comp2 = sorted([comp1, comp2])
 
-            comp1 = ";".join(["%s/%s/%d%s" % (r.parent.id, r.resname, r.id[1], r.id[2].strip()) for r in comp1])
-            comp2 = ";".join(["%s/%s/%d%s" % (r.parent.id, r.resname, r.id[1], r.id[2].strip()) for r in comp2])
+            comp1 = ";".join(["%s/%s/%d%s" % (r.parent.id,
+                                              r.resname,
+                                              r.id[1],
+                                              r.id[2].strip()) for r in comp1])
+            comp2 = ";".join(["%s/%s/%d%s" % (r.parent.id,
+                                              r.resname,
+                                              r.id[1],
+                                              r.id[2].strip()) for r in comp2])
+
+            entry_id = (entry.mol_id if isinstance(entry, MolFileEntry)
+                        else entry.to_string())
 
-            entry_id = entry.mol_id if isinstance(entry, MolFileEntry) else entry.to_string()
             if by_interaction:
                 key = (entry_id, inter.type)
             else:
                 key = entry_id
 
             data_by_entry[key][comp2] += 1
 
@@ -83,39 +94,54 @@
 
                 heatmap_data["residues"].append(res)
                 heatmap_data["frequency"].append(data_by_entry[key][res])
 
     df = pd.DataFrame.from_dict(heatmap_data)
 
     if by_interaction:
-        return pd.pivot_table(df, index=['entry', 'interaction'], columns='residues', values='frequency', fill_value=0)
+        return pd.pivot_table(df,
+                              index=['entry', 'interaction'],
+                              columns='residues',
+                              values='frequency',
+                              fill_value=0)
     else:
-        return pd.pivot_table(df, index='entry', columns='residues', values='frequency', fill_value=0)
+        return pd.pivot_table(df,
+                              index='entry',
+                              columns='residues',
+                              values='frequency',
+                              fill_value=0)
 
 
-def heatmap(data_df, figsize=None, cmap="Blues", heatmap_kw=None, gridspec_kw=None):
+def heatmap(data_df,
+            figsize=None,
+            cmap="Blues",
+            heatmap_kw=None,
+            gridspec_kw=None):
     """ Plot a residue matrix as a color-encoded matrix.
 
     Parameters
     ----------
     data_df : :class:`pandas.DataFrame`
-        A residue matrix produced with :func:`~luna.analysis.residues.generate_residue_matrix`.
+        A residue matrix produced
+        with :func:`~luna.analysis.residues.generate_residue_matrix`.
     figsize : tuple, optional
         Size (width, height) of a figure in inches.
     cmap : str, iterable of str
-        The mapping from data values to color space. The default value is 'Blues'.
+        The mapping from data values to color space.
+        The default value is 'Blues'.
     heatmap_kw : dict, optional
         Keyword arguments for :func:`seaborn.heatmap`.
     gridspec_kw : dict, optional
         Keyword arguments for :class:`matplotlib.gridspec.GridSpec`.
         Used only if the residue matrix (``data_df``) contains interactions.
 
     Returns
     -------
-     : :class:`matplotlib.axes.Axes` or :class:`numpy.ndarray` of :class:`matplotlib.axes.Axes`
+     : :class:`matplotlib.axes.Axes` or :class:`numpy.ndarray` \
+            of :class:`matplotlib.axes.Axes`
 
     """
     data_df = data_df.reset_index()
 
     heatmap_kw = heatmap_kw or {}
     gridspec_kw = gridspec_kw or {}
 
@@ -126,34 +152,37 @@
     else:
         max_value = data_df[data_df.columns[1:]].max().max()
 
     if not interactions:
         data_df.set_index('entry', inplace=True)
 
         fig = plt.figure(figsize=figsize)
-        ax = sns.heatmap(data_df, cmap=cmap, vmax=max_value, vmin=0, **heatmap_kw)
+        ax = sns.heatmap(data_df, cmap=cmap,
+                         vmax=max_value, vmin=0, **heatmap_kw)
         ax.set_xlabel("")
         ax.set_ylabel("")
         return ax
     else:
         ncols = 3
         if "ncols" in gridspec_kw:
             ncols = gridspec_kw["ncols"]
             del gridspec_kw["ncols"]
         nrows = math.ceil(len(interactions) / ncols)
 
-        fig, axs = plt.subplots(nrows, ncols, figsize=figsize, gridspec_kw=gridspec_kw)
+        fig, axs = plt.subplots(nrows, ncols, 
+                                figsize=figsize, gridspec_kw=gridspec_kw)
 
         row, col = 0, 0
         for i, interaction in enumerate(interactions):
             df = data_df[data_df["interaction"] == interaction].copy()
             df.drop(columns="interaction", inplace=True)
             df.set_index('entry', inplace=True)
 
-            g = sns.heatmap(df, cmap=cmap, vmax=max_value, vmin=0, ax=axs[row][col], **heatmap_kw)
+            g = sns.heatmap(df, cmap=cmap, vmax=max_value, vmin=0,
+                            ax=axs[row][col], **heatmap_kw)
 
             g.set_title(interaction)
             g.set_xlabel("")
             g.set_ylabel("")
 
             col += 1
             if col == ncols:
```

### Comparing `luna-0.12.2/luna/analysis/summary.py` & `luna-0.13.0/luna/analysis/summary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 from collections import defaultdict
 import logging
 
 
 logger = logging.getLogger()
 
 
-def count_interaction_types(interactions, must_have_target=True, compounds=None, key_map={}):
+def count_interaction_types(interactions,
+                            must_have_target=True,
+                            compounds=None,
+                            key_map={}):
     """Count the number of each type of interaction in ``interactions``.
 
     Parameters
     ----------
     interactions : iterable
-            An iterable object containing a sequence of interactions (``InteractionType``).
+            An iterable object containing a sequence of interactions
+            (``InteractionType``).
     must_have_target : bool
-            If True, count only interactions involving the target ligand. The default value is True.
+            If True, count only interactions involving the target ligand.
+            The default value is True.
     compounds: iterable, optional
             Only count interactions involving the compounds in ``compounds``.
-            The default value is None, which implies that all compounds will be considered.
+            The default value is None, which implies that all compounds will
+            be considered.
     key_map: dictionary, optional
-            A dictionary to control which interactions to count and how to aggregate them.
-            The keys are the interaction types to be considered and the values are the final interaction type,
-            which can be used to aggregate interactions. If a value is None, the interaction will be ignored.
+            A dictionary to control which interactions to count and how to
+            aggregate them. The keys are the interaction types to be
+            considered and the values are the final interaction type, which
+            can be used to aggregate interactions. If a value is None, the
+            interaction will be ignored.
 
-            For example, to aggregate all covalent interactions, ``key_map`` could be defined as follows:
+            For example, to aggregate all covalent interactions, ``key_map``
+            could be defined as follows:
 
                .. code-block:: python
 
                     key_map = {"Single bond": "Covalent bond",
                                "Double bond": "Covalent bond",
                                "Triple bond": "Covalent bond",
                                "Aromatic bond": "Covalent bond"}
 
-            Now, if Ionic interactions should be ignored, ``key_map`` could be defined as follows:
+            Now, if Ionic interactions should be ignored, ``key_map`` could
+            be defined as follows:
 
                 .. code-block:: python
 
                     key_map = {"Ionic": None}
 
     Returns
     -------
@@ -53,15 +63,16 @@
             is_valid = True
         else:
             if must_have_target:
                 if i.src_grp.has_target() or i.trgt_grp.has_target():
                     is_valid = True
 
             if compounds:
-                if len(i.src_grp.compounds & compounds) > 0 or len(i.trgt_grp.compounds & compounds):
+                if (len(i.src_grp.compounds & compounds) > 0
+                        or len(i.trgt_grp.compounds & compounds)):
                     is_valid = True
 
         if is_valid:
             pair_key1 = (i.type, i.src_grp, i.trgt_grp)
             pair_key2 = (i.type, i.trgt_grp, i.src_grp)
 
             if pair_key1 in seen_pairs or pair_key2 in seen_pairs:
```

### Comparing `luna-0.12.2/luna/config/default.cfg` & `luna-0.13.0/luna/config/default.cfg`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/config/params.py` & `luna-0.13.0/luna/config/params.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,35 @@
 
 from luna.util.config import Config
 from luna.mol.entry import *
 from luna.interaction.calc import InteractionCalculator
 from luna.interaction.config import InteractionConfig
 from luna.interaction.filter import InteractionFilter, BindingModeFilter
 from luna.interaction.fp.type import IFPType
-from luna.util.default_values import ACCEPTED_MOL_OBJ_TYPES
 from luna.util.logging import VERBOSITY_LEVEL
 from luna.util.exceptions import IllegalArgumentError
 
 
 class ProjectParams(dict):
 
+    """Define LUNA project parameters.
+
+    Parameters
+    ----------
+    params : dict
+        Set LUNA parameters from ``params``.
+
+    fill_defaults : bool
+        If True, initialize `ProjectParams` with default LUNA values.
+
+        .. note::
+            Any parameter provided in ``params`` will overwrite the
+            default values.
+    """
+
     def __init__(self, params=None, fill_defaults=False):
 
         params_to_parse = {}
 
         # Loads in default LUNA values.
         if fill_defaults:
             luna_path = path.abspath(path.join(path.realpath(__file__),
@@ -42,14 +56,20 @@
         if params:
             params_to_parse.update(params)
 
         self._validate(params_to_parse)
 
     @classmethod
     def from_project_obj(cls, proj_obj):
+        """Initialize a `ProjectParams` from a `~luna.projects.Project` object.
+
+        Returns
+        -------
+         : `ProjectParams`
+        """
         params = {"add_h": proj_obj.add_h,
                   "amend_mol": proj_obj.amend_mol,
                   "append_mode": proj_obj.append_mode,
                   "feat_cfg": proj_obj.atom_prop_file,
                   "binding_mode_filter": proj_obj.binding_mode_filter,
                   "ifp": proj_obj.calc_ifp,
                   "mfp": proj_obj.calc_mfp,
@@ -61,100 +81,34 @@
                   "ifp_output": proj_obj.ifp_output,
                   "ifp_radius_step": proj_obj.ifp_radius_step,
                   "ifp_sim_matrix_output": proj_obj.ifp_sim_matrix_output,
                   "ifp_type": proj_obj.ifp_type,
                   "inter_calc": proj_obj.inter_calc,
                   "logging_enabled": proj_obj.logging_enabled,
                   "mfp_output": proj_obj.mfp_output,
-                  "mol_obj_type": proj_obj.mol_obj_type,
                   "nproc": proj_obj.nproc,
                   "pse": proj_obj.out_pse,
                   "overwrite_path": proj_obj.overwrite_path,
                   "pdb_path": proj_obj.pdb_path,
                   "ph": proj_obj.ph,
                   "pse_path": proj_obj.pse_path,
                   "use_cache": proj_obj.use_cache,
                   "verbosity": proj_obj.verbosity,
                   "working_path": proj_obj.working_path}
 
         return cls(params)
 
-    def _get_entry_params(self, config_file):
-        sep = ":"
-        entries = []
-        for e in self["entries"]:
-            if isinstance(e, MolEntry):
-                entries.append(e.to_string(sep))
-
-            elif isinstance(e, MolFileEntry):
-                fields = [str(e.pdb_id), str(e.mol_id), str(e.mol_file),
-                          str(e.is_multimol_file)]
-                entries.append(",".join(fields))
-
-        path = Path(config_file).parent.resolve()
-        filename = Path(config_file).stem
-
-        entry_file = f"{path}/{filename}.entries.txt"
-        with open(entry_file, "w") as OUT:
-            for e in entries:
-                OUT.write(f"{e}\n")
-
-        return {"entries": entry_file,
-                "pdb_id": None,
-                "mol_file": None,
-                "entries_sep": ":",
-                "fields_sep": ","}
-
-    def _get_inter_params(self, config_file):
-        path = Path(config_file).parent.resolve()
-        filename = Path(config_file).stem
-
-        ic = self["inter_calc"]
-
-        inter_config = ic.inter_config
-        inter_cfg_file = None
-        if isinstance(inter_config, InteractionConfig):
-            inter_cfg_file = f"{path}/{filename}.inter.txt"
-            inter_config.save_config_file(inter_cfg_file)
-
-        inter_filter = ic.inter_filter
-        filter_cfg_file = None
-        if isinstance(inter_filter, InteractionFilter):
-            filter_cfg_file = f"{path}/{filename}.filter.txt"
-            inter_filter.save_config_file(filter_cfg_file)
-
-        inter_filter = ic.inter_filter
-
-        return {"inter_cfg": inter_cfg_file,
-                "filter_cfg": filter_cfg_file,
-                "add_non_cov": ic.add_non_cov,
-                "add_cov": ic.add_cov,
-                "add_proximal": ic.add_proximal,
-                "add_atom_atom": ic.add_atom_atom,
-                "add_dependent_inter": ic.add_dependent_inter,
-                "add_h2o_pairs_with_no_target":
-                    ic.add_h2o_pairs_with_no_target,
-                "strict_donor_rules": ic.strict_donor_rules,
-                "strict_weak_donor_rules": ic.strict_weak_donor_rules,
-                "lazy_comps_list": ",".join(ic.lazy_comps_list)}
-
-    def _get_binding_filter_params(self, config_file):
-        path = Path(config_file).parent.resolve()
-        filename = Path(config_file).stem
-
-        bmf = self["binding_mode_filter"]
-        bmf_cfg_file = None
-        if isinstance(bmf, BindingModeFilter):
-            bmf_cfg_file = f"{path}/{filename}.bind.txt"
-            bmf.save_config_file(bmf_cfg_file)
-
-        return {"bind_cfg": bmf_cfg_file}
-
     def save_config_file(self, config_file):
+        """Save the project parameters into a configuration file.
 
+        Parameters
+        ----------
+        config_file : str
+            The output configuration file.
+        """
         with open(config_file, "w") as OUT:
             OUT.write("[entries]\n")
             for k, v in self._get_entry_params(config_file).items():
                 OUT.write(f"{k} = {v}\n")
             OUT.write("\n")
 
             OUT.write("[paths]\n")
@@ -210,22 +164,92 @@
             OUT.write("pse_path = %s\n" % self["pse_path"])
             OUT.write("\n")
 
             verbosity = [k for k, v in VERBOSITY_LEVEL.items()
                          if v == self["verbosity"]].pop()
 
             OUT.write("[general]\n")
-            OUT.write("mol_obj_type = %s\n" % self["mol_obj_type"])
             OUT.write("append_mode = %s\n" % self["append_mode"])
             OUT.write("use_cache = %s\n" % self["use_cache"])
             OUT.write("verbosity = %s\n" % verbosity)
             OUT.write("logging_enabled = %s\n" % self["logging_enabled"])
             OUT.write("nproc = %s\n" % self["nproc"])
             OUT.write("\n")
 
+    def _get_entry_params(self, config_file):
+        sep = ":"
+        entries = []
+        for e in self["entries"]:
+            if isinstance(e, MolEntry):
+                entries.append(e.to_string(sep))
+
+            elif isinstance(e, MolFileEntry):
+                fields = [str(e.pdb_id), str(e.mol_id), str(e.mol_file),
+                          str(e.is_multimol_file)]
+                entries.append(",".join(fields))
+
+        path = Path(config_file).parent.resolve()
+        filename = Path(config_file).stem
+
+        entry_file = f"{path}/{filename}.entries.txt"
+        with open(entry_file, "w") as OUT:
+            for e in entries:
+                OUT.write(f"{e}\n")
+
+        return {"entries": entry_file,
+                "pdb_id": None,
+                "mol_file": None,
+                "entries_sep": ":",
+                "fields_sep": ","}
+
+    def _get_inter_params(self, config_file):
+        path = Path(config_file).parent.resolve()
+        filename = Path(config_file).stem
+
+        ic = self["inter_calc"]
+
+        inter_config = ic.inter_config
+        inter_cfg_file = None
+        if isinstance(inter_config, InteractionConfig):
+            inter_cfg_file = f"{path}/{filename}.inter.txt"
+            inter_config.save_config_file(inter_cfg_file)
+
+        inter_filter = ic.inter_filter
+        filter_cfg_file = None
+        if isinstance(inter_filter, InteractionFilter):
+            filter_cfg_file = f"{path}/{filename}.filter.txt"
+            inter_filter.save_config_file(filter_cfg_file)
+
+        inter_filter = ic.inter_filter
+
+        return {"inter_cfg": inter_cfg_file,
+                "filter_cfg": filter_cfg_file,
+                "add_non_cov": ic.add_non_cov,
+                "add_cov": ic.add_cov,
+                "add_proximal": ic.add_proximal,
+                "add_atom_atom": ic.add_atom_atom,
+                "add_dependent_inter": ic.add_dependent_inter,
+                "add_h2o_pairs_with_no_target":
+                    ic.add_h2o_pairs_with_no_target,
+                "strict_donor_rules": ic.strict_donor_rules,
+                "strict_weak_donor_rules": ic.strict_weak_donor_rules,
+                "lazy_comps_list": ",".join(ic.lazy_comps_list)}
+
+    def _get_binding_filter_params(self, config_file):
+        path = Path(config_file).parent.resolve()
+        filename = Path(config_file).stem
+
+        bmf = self["binding_mode_filter"]
+        bmf_cfg_file = None
+        if isinstance(bmf, BindingModeFilter):
+            bmf_cfg_file = f"{path}/{filename}.bind.txt"
+            bmf.save_config_file(bmf_cfg_file)
+
+        return {"bind_cfg": bmf_cfg_file}
+
     def _get_value(self, params, param_name, dtype,
                    fallback=None, is_none_valid=True):
 
         value = params.get(param_name, fallback)
 
         try:
             value = ast.literal_eval(value)
@@ -252,20 +276,25 @@
     def _parse_entries_params(self, params):
         try:
             entries_file = self._get_value(params, "entries", str)
 
             pdb_id = self._get_value(params, "pdb_id", str)
             mol_file = self._get_value(params, "mol_file", str)
             entries_sep = self._get_value(params, "entries_sep", str)
-            fields_sep = self._get_value(params, "fields_sep", str,)
+            fields_sep = self._get_value(params, "fields_sep", str)
+
+            mol_obj_type = params["mol_obj_type"]
 
             entries = None
             if entries_file:
                 entries = list(Entry.from_file(entries_file, pdb_id, mol_file,
-                                               entries_sep, fields_sep))
+                                               entries_sep, fields_sep,
+                                               mol_obj_type=mol_obj_type))
+        except IllegalArgumentError:
+            raise
         except Exception:
             entries = self._get_value(params, "entries", list)
 
         return {"entries": entries}
 
     def _parse_paths_params(self, params):
         working_path = self._get_value(params, "working_path", str)
@@ -447,22 +476,14 @@
     def _parse_pse_params(self, params):
         out_pse = self._get_value(params, "pse", bool)
         pse_path = self._get_value(params, "pse_path", str)
 
         return {"out_pse": out_pse, "pse_path": pse_path}
 
     def _parse_general_params(self, params):
-        mol_obj_type = self._get_value(params, "mol_obj_type", str)
-
-        if (mol_obj_type is not None
-                and mol_obj_type not in ACCEPTED_MOL_OBJ_TYPES):
-            raise KeyError("Invalid choise '%s' for property 'mol_obj_type'. "
-                           "Choose from: %s."
-                           % (mol_obj_type,
-                              ", ".join(ACCEPTED_MOL_OBJ_TYPES)))
 
         append_mode = self._get_value(params, "append_mode", bool)
 
         use_cache = self._get_value(params, "use_cache", bool)
 
         verbosity = self._get_value(params, "verbosity", int)
 
@@ -482,15 +503,14 @@
                     raise IllegalArgumentError(msg)
 
         logging_enabled = self._get_value(params, "logging_enabled", bool)
 
         nproc = self._get_value(params, "nproc", int)
 
         return {
-            "mol_obj_type": mol_obj_type,
             "append_mode": append_mode,
             "use_cache": use_cache,
             "verbosity": verbosity,
             "logging_enabled": logging_enabled,
             "nproc": nproc,
         }
```

### Comparing `luna-0.12.2/luna/data/BaseFeatures.fdef` & `luna-0.13.0/luna/data/BaseFeatures.fdef`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/data/BaseFeatures_DIP2_NoMicrospecies.fdef` & `luna-0.13.0/luna/data/BaseFeatures_DIP2_NoMicrospecies.fdef`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/data/LUNA.fdef` & `luna-0.13.0/luna/data/LUNA.fdef`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 # Good AC, Oprea TI. Optimization of CAMD techniques 3. Virtual screening enrichment studies: a help or hindrance in tool selection? Journal of Computer-Aided Molecular Design. 2008;22:169–78.
 # Ballatore C, Huryn DM, Smith AB. Carboxylic Acid (Bio)Isosteres in Drug Design. ChemMedChem. 2013;8:385–95.
 #
 # 1st constraint: acyl sulfonamide
 # 2nd constraint: barbiturates/thiazolidinediones/rhodanine...
 #
 # OBS: I removed general sulfonamide constraint ("$([NH,NH0-1](S(=O)(=O))c)") from this atom definition.
-#      I did it because the sulfonamides are weakly acid (pKa=~10) and depend on appropriate substituents to lower the pKa.
+#      That's because sulfonamides are weakly acid (pKa=~10) and depend on appropriate substituents to lower the pKa.
 #      Then, I prefer to let their N to be donor atoms, i.e., the N will not be considered always deprotonated.
 #      REF: Ballatore C, Huryn DM, Smith AB. Carboxylic Acid (Bio)Isosteres in Drug Design. ChemMedChem. 2013;8:385–95
 #
 AtomType AcidicN  [$([NH,NH0-1](S(=O)(=O))(C(=O))),$([NH1,NH0-1;R](C(=O))(C(=[O,S])))]
 
 #
 # Adapted from RDKit (Marcus Kossner)
@@ -79,15 +79,27 @@
 EndFeature
 
 #
 # Capture: Tetrazoles
 # Adapted from RDKit (Marcus Kossner)
 #
 AtomType TetrazoleN [nR1r5;$(n:n:n:n:c),$(n:n:n:c:n)]
-DefineFeature TautomerRingDonorN [$(n[n;H1]),$(nc[n;H1]);!{TetrazoleN}]
+
+#
+# Capture: tautomeric nitrogens as in imidazole.
+#
+#   => Aromatic rings containing a tertiary N are not tautomeric.
+#
+#   => R1 forces all atoms to belong to the same ring, avoiding cases where a C connecting two rings (R2)
+#           is captured by the rule 'ncn' and makes the N to be incorrectly perceived as a Donor.
+#
+#       . E.g: 2-aminopurin-6-one (Nc1nc(=O)c2ncnc2[nH]1)
+#       
+#
+DefineFeature TautomerRingDonorN [$([n;R1][n;H1;R1]),$([n;R1][c;R1][n;H1;R1]);!$([n;H0;X3]);!{TetrazoleN}]
   Family Donor
   Weights 1.0
 EndFeature
 
 #
 # Capture: tautomeric Guanidine
 # N[CH0X3](=N)N
@@ -99,23 +111,28 @@
 #EndFeature
 
 #
 # Capture: Hydroxyl from acid groups containing S, O and P (sulfonic and sulfunic acids, carboxylic acids, etc).
 # This constraint also cover thioketones, i.e., compounds with a double bonded S, instead of a double bonded O.
 #
 AtomType AcidicHydroxyl [$([O][C,S,P](=[O,S]))]
+
 DefineFeature DonorAtom [N!H0v3,N!H0+v4,nH+0&!{TetrazoleN},OH2v2,OH+0,SH+0;!{AcidicN};!{AcidicHydroxyl}]
   Family Donor
   Weights 1.0
 EndFeature
 
+
+#
+# Capture: Carbonic acid or carbonate
+AtomType CarbonateO [$([O;H1,H0&-1]C(=[O,S])-[O;H1,H0&-1]),$([O,S]=C(-[O;H1,H0&-1])-[O;H1,H0&-1])]
 #
 # Capture: Ketene acetal oxygen
 #
-DefineFeature KeteneAcetalO [$([O;H1,H0&-1]-[#6;X3]-,:[#8])]
+DefineFeature KeteneAcetalO [$([O;H1,H0&-1]-[#6;X3]-,:[#8]);!{CarbonateO}]
   Family Donor
   Weights 1.0
 EndFeature
 
 
 ########################################################################################
 #                                                                                      #
@@ -168,21 +185,37 @@
 #                                                                                      #
 #                Acceptors for:                                                        #
 #                                - Hydrogen   bond                                     #
 #                                - Halogen    bond                                     #
 #                                - Chalcogen  bond                                     #
 #                                                                                      #
 ########################################################################################
-#
+
 #
 # Joule JA, Mills K. Heterocyclic chemistry. 5th ed. Hoboken, N.J: Wiley; 2009.
 # Li S, Hong M. Protonation, Tautomerization, and Rotameric Structure of Histidine: A Comprehensive Study by Magic-Angle-Spinning Solid-State NMR. Journal of the American Chemical Society. 2011;133:1534–44.
 # Sudmeier JL, Bradshaw EM, Haddad KEC, Day RM, Thalhauser CJ, Bullock PA, et al. Identification of Histidine Tautomers in Proteins by 2D 1 H/ 13 C δ2 One-Bond Correlated NMR. Journal of the American Chemical Society. 2003;125:8430–1.
 #
-DefineFeature TautomerRingAcceptorN [$([n;H1]n),$([n;H1]cn);!{TetrazoleN}]
+#   => Aromatic rings containing a tertiary N are not tautomeric.
+#
+#   => R1 forces all atoms to belong to the same ring, avoiding cases where a C connecting two rings (R2)
+#           is captured by the rule 'ncn' and makes the N to be incorrectly perceived as an Acceptor.
+#
+DefineFeature TautomerRingAcceptorN [$([n;H1;R1][n;R1]),$([n;H1;R1][c;R1][n;R1]);!$([nH,n-1][c;R1][n;H0;X3;R1]);!{TetrazoleN}]
+  Family Acceptor
+  Weights 1.0
+EndFeature
+
+#
+# Capture: uracil-like aromatic rings.
+#
+#   . E.g: 1-methyluracil (CN1C=CC(=O)NC1=O)
+#
+AtomType UracilLikeN [$([nH,n-1;R1]1[c;R1](=O)[n;H0;X3;R1][c;R1][c;R1][c;R1]1(=O))]
+DefineFeature UracilLikeN [{UracilLikeN}]
   Family Acceptor
   Weights 1.0
 EndFeature
 
 #
 # Adapted from RDKit (Marcus Kossner)
 # Aromatic N with a double bond and no hydrogen. In this case, the N already contributes to the ring resonance, so the two valence electrons are free to "accept" a hydrogen atom.
@@ -339,14 +372,22 @@
 ########################################################################################
 #                                                                                      #
 #                                 Negative ionizable                                   #
 #                                                                                      #
 ########################################################################################
 #
 #
+# Capture: Carbonic acid and carbonate.
+# It also captures thiocarboxylic acids
+#
+DefineFeature CarbonateGroup C(=[O,S])(-[O;H1,H0&-1])-[O;H1,H0&-1]
+    Family NegativelyIonizable
+    Weights 1.0,1.0,1.0,1.0
+EndFeature
+
 # Capture: Carboxylic acid and Carboxylate
 # It also captures thiocarboxylic acids
 #
 DefineFeature CarboxGroup C(=[O,S])-[O;H1,H0&-1]
     Family NegativelyIonizable
     Weights 1.0,1.0,1.0
 EndFeature
@@ -382,19 +423,29 @@
 EndFeature
 
 # Capture: Diformamide-like
 #
 # Generic constraint for barbiturates/thiazolidinediones...
 #
 # Good AC, Oprea TI. Optimization of CAMD techniques 3. Virtual screening enrichment studies: a help or hindrance in tool selection? Journal of Computer-Aided Molecular Design. 2008;22:169–78.
-DefineFeature Diformamide [NH1,NH0-1;R](C(=O))(C(=O))
+DefineFeature Diformamide [NH1,NH0-1;R](C(=O))C(=O)
     Family NegativelyIonizable
     Weights 1.0,1.0,1.0,1.0,1.0
 EndFeature
 
+#
+# Capture: uracil-like aromatic rings.
+#
+#   . E.g: 1-methyluracil (CN1C=CC(=O)NC1=O)
+#
+DefineFeature UracilAromaticRing [nH,n-1;R1]1[c;R1](=O)[n;H0;X3;R1][c;R1][c;R1][c;R1]1(=O)
+  Family NegativelyIonizable
+  Weights 1.0,1.0,1.0,1.0,1.0,1.0,1.0,1.0
+EndFeature
+
 
 ########################################################################################
 #                          Hydroxamic acids - RC(=O)N(R’)OH                            #
 
 # Hydroxamic acids bind metals
 # Bertrand S, Hélesbeux J-J, Larcher G, Duval O. Hydroxamate, a key pharmacophore exhibiting a wide range of biological activities. Mini Rev Med Chem. 2013;13:1311–26.
 # Zuccotto F. Pharmacophore Features Distributions in Different Classes of Compounds. J Chem Inf Comput Sci. 2003;43:1542–52.
@@ -733,15 +784,17 @@
 #                                                                                      #
 ########################################################################################
 #
 #
 # For amide-pi interactions
 # Amide–π interactions between formamide and benzene (Imai et al, 2009).
 #
-DefineFeature AmideGroup [NX3][CX3](=[OX1])
+# It also captures deprotonated amide Ns.
+#
+DefineFeature AmideGroup [NX3,NX2-1][CX3](=[OX1])
   Family Amide
   Weights 1.0,1.0,1.0
 EndFeature
 
 
 ########################################################################################
 #                                                                                      #
```

### Comparing `luna-0.12.2/luna/data/MinimalFeatures.fdef` & `luna-0.13.0/luna/data/MinimalFeatures.fdef`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/data/ligand_expo.tsv` & `luna-0.13.0/luna/data/ligand_expo.tsv`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/data/precomputed_residue_atom_features.json` & `luna-0.13.0/luna/data/precomputed_residue_atom_features.json`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/interaction/bind.cfg` & `luna-0.13.0/luna/interaction/bind.cfg`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/interaction/calc.py` & `luna-0.13.0/luna/interaction/calc.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,25 +28,28 @@
     BondType.SINGLE: "Single bond",
     BondType.DOUBLE: "Double bond",
     BondType.TRIPLE: "Triple bond",
     BondType.AROMATIC: "Aromatic bond"
 }
 
 WATER_NAMES = ['HOH', 'DOD', 'WAT', 'H2O', 'OH2']
-DEFAULT_SOLVENTS = WATER_NAMES + ["NH3", "NH4"]
+DEFAULT_LAZY_LIST = WATER_NAMES + ["NH3", "NH4", "CMO", "SCN"]
 
 
 class InteractionsManager:
 
-    """Store and manage :class:`~luna.interaction.type.InteractionType` objects.
+    """Store and manage :class:`~luna.interaction.type.InteractionType`
+    objects.
 
     Parameters
     ----------
-    interactions : iterable of :class:`~luna.interaction.type.InteractionType`, optional
-        An initial sequence of :class:`~luna.interaction.type.InteractionType` objects.
+    interactions : iterable of \
+                :class:`~luna.interaction.type.InteractionType`, optional
+        An initial sequence of :class:`~luna.interaction.type.InteractionType`
+        objects.
     entry : :class:`~luna.mol.entry.Entry`, optional
         The chain or compound used as reference to calculate interactions.
 
     """
 
     def __init__(self, interactions=None, entry=None):
         if interactions is None:
@@ -55,16 +58,18 @@
         self.entry = entry
         self._interactions = list(interactions)
 
         self.version = __version__
 
     @property
     def interactions(self):
-        """ list of :class:`~luna.interaction.type.InteractionType`, read-only: The list of interactions.\
-        Additional interactions should be added using the method :py:meth:`add_interactions`."""
+        """ list of :class:`~luna.interaction.type.InteractionType`, \
+            read-only: The list of interactions.\
+        Additional interactions should be added using the method
+        :py:meth:`add_interactions`."""
         return self._interactions
 
     @property
     def size(self):
         """int, read-only: The number of interactions."""
         return len(self._interactions)
 
@@ -84,41 +89,44 @@
     def count_interations(self, must_have_target=False):
         """Count the number of each type of interaction in ``interactions``.
 
         Parameters
         ----------
         must_have_target : bool
                 If True, count only interactions involving the target ligand.
-                The default value is False, which implies all interactions will be considered.
+                The default value is False, which implies all interactions
+                will be considered.
 
         Returns
         -------
          : dict
         """
-        return count_interaction_types(self.interactions, must_have_target=must_have_target)
+        return count_interaction_types(self.interactions,
+                                       must_have_target=must_have_target)
 
     def add_interactions(self, interactions):
-        """Add one or more :class:`~luna.interaction.type.InteractionType` objects to
-         ``interactions``."""
+        """Add one or more :class:`~luna.interaction.type.InteractionType`
+        objects to ``interactions``."""
 
         self._interactions = list(set(self.interactions + list(interactions)))
 
     def remove_interactions(self, interactions):
-        """Remove one or more :class:`~luna.interaction.type.InteractionType` objects from \
-        ``interactions``.
+        """Remove one or more :class:`~luna.interaction.type.InteractionType`
+        objects from ``interactions``.
 
         Any recursive references to the removed objects will also be cleared.
         """
         self._interactions = list(set(self.interactions) - set(interactions))
 
         for inter in interactions:
             inter.clear_refs()
 
     def filter_by_types(self, types):
-        """Filter :class:`~luna.interaction.type.InteractionType` objects by their types.
+        """Filter :class:`~luna.interaction.type.InteractionType` objects by
+        their types.
 
         Parameters
         ----------
         types : iterable of str
             A sequence of interaction types.
 
         Yields
@@ -132,17 +140,19 @@
     def filter_out_by_binding_mode(self, binding_modes_filter):
         """Filter out interactions based on binding modes.
 
         **Note:** this method modifies ``interactions``.
 
         Parameters
         ----------
-        binding_modes_filter : :class:`~luna.interaction.filter.BindingModeFilter`
-            A :class:`~luna.interaction.filter.BindingModeFilter` object that defines binding mode conditions
-            to decide which interactions are valid.
+        binding_modes_filter : \
+                :class:`~luna.interaction.filter.BindingModeFilter`
+            A :class:`~luna.interaction.filter.BindingModeFilter` object that
+            defines binding mode conditions to decide which interactions
+            are valid.
 
         Returns
         -------
          : set of :class:`~luna.interaction.type.InteractionType`
             The interactions that were filtered out.
         """
         inters_to_remove = set()
@@ -160,63 +170,70 @@
         Parameters
         ----------
         output_file : str
             The output CSV file.
         """
         interactions_set = set()
         for inter in self.interactions:
-            grp1 = ";".join(sorted(["/".join(a.full_atom_name.split("/")) for a in inter.src_grp.atoms]))
-            grp2 = ";".join(sorted(["/".join(a.full_atom_name.split("/")) for a in inter.trgt_grp.atoms]))
+            grp1 = ";".join(sorted(["/".join(a.full_atom_name.split("/"))
+                                    for a in inter.src_grp.atoms]))
+            grp2 = ";".join(sorted(["/".join(a.full_atom_name.split("/"))
+                                    for a in inter.trgt_grp.atoms]))
 
             grp1, grp2 = sorted([grp1, grp2])
             interactions_set.add((grp1, grp2, inter.type))
 
         with open(output_file, "w") as OUT:
             OUT.write("atom_group1,atom_group2,interaction\n")
             # Sort lines before writing to always keep the same order.
-            OUT.write("\n".join([",".join(k) for k in sorted(interactions_set)]))
+            OUT.write("\n".join([",".join(k)
+                                 for k in sorted(interactions_set)]))
 
     def to_json(self, output_file=None, indent=None):
         """Write interactions to a_initial_shell_data JSON file.
 
         Parameters
         ----------
         output_file : str
             The output JSON file.
         indent : int or str, optional
             Indent level for pretty-printed JSON files.
             An indent level of 0, negative, or '' only insert newlines.
             Positive integers indent that many spaces per level.
-            If a string is provided (e.g., '\\\\t'), it will be used to indent each level.
-            The default value is None, which selects the most compact representation.
+            If a string is provided (e.g., '\\\\t'), it will be used to indent
+            each level. The default value is None, which selects the most
+            compact representation.
         """
         with open(output_file, 'w') as OUT:
             inter_objs = [inter.as_json() for inter in self.interactions]
             json.dump(inter_objs, OUT, indent=indent)
 
     def save(self, output_file, compressed=True):
-        """Write the pickled representation of the `InteractionsManager` object to the file ``output_file``.
+        """Write the pickled representation of the `InteractionsManager` object
+        to the file ``output_file``.
 
         Parameters
         ----------
         output_file : str
             The output file.
         compressed : bool, optional
-            If True (the default), compress the pickled representation as a gzip file (.gz).
+            If True (the default), compress the pickled representation as a
+            gzip file (.gz).
 
         Raises
         -------
         FileNotCreated
             If the file could not be created.
         """
         pickle_data(self, output_file, compressed)
 
     @staticmethod
     def load(input_file):
-        """Load the pickled representation of an `InteractionsManager` object saved at the file ``input_file``.
+        """Load the pickled representation of an `InteractionsManager` object
+        saved at the file ``input_file``.
 
         Returns
         ----------
          : `InteractionsManager`
             The reconstituted `InteractionsManager` object.
 
         Raises
@@ -238,192 +255,221 @@
 
 class InteractionCalculator:
 
     """Calculate interactions.
 
     .. note::
         This class provides default LUNA methods to calculate interactions.
-        However, one can provide their own methods without modifying this class.
-        In the **Examples** section, we will show how to define custom functions.
+        However, one can provide their own methods without modifying this
+        class. In the **Examples** section, we will show how to define
+        custom functions.
 
     .. note::
-        In case you want to disable specific parameters (e.g., angles) used during
-        the calculation of interactions, you do not need to define a custom
-        function for it. You could just delete the parameter from the configuration
-        and LUNA will automatically recognize that a given parameter is not
-        necessary anymore.
+        In case you want to disable specific parameters (e.g., angles) used
+        during the calculation of interactions, you do not need to define a
+        custom function for it. You could just delete the parameter from the
+        configuration and LUNA will automatically recognize that a given
+        parameter is not necessary anymore.
 
-        Check **Examples 3** to see how to do it and how to implement this automatic
-        behavior on your custom functions.
+        Check **Examples 3** to see how to do it and how to implement this
+        automatic behavior on your custom functions.
 
 
     Parameters
     ----------
     inter_config : :class:`~luna.interaction.config.InteractionConfig`
-        An :class:`~luna.interaction.config.InteractionConfig` object with all parameters and cutoffs necessary
-        to compute interactions defined in ``inter_funcs``.
-        If not provided, the default LUNA configuration will be used instead \
+        An :class:`~luna.interaction.config.InteractionConfig` object with
+        all parameters and cutoffs necessary to compute interactions defined
+        in ``inter_funcs``. If not provided, the default LUNA configuration
+        will be used instead \
         (:class:`~luna.interaction.config.DefaultInteractionConfig`).
-    inter_filter : :class:`~luna.interaction.filter.InteractionFilter`, optional
-        An :class:`~luna.interaction.filter.InteractionFilter` object to filter out interactions on-the-fly.
-        The default value is None, which implies no interaction will be filtered out.
+    inter_filter : :class:`~luna.interaction.filter.InteractionFilter`, \
+            optional
+        An :class:`~luna.interaction.filter.InteractionFilter` object to filter
+        out interactions on-the-fly. The default value is None, which implies
+        no interaction will be filtered out.
     inter_funcs : dict of {tuple : iterable of callable}
         A dict to define custom functions to calculate interactions,
-        where keys are tuples of feature names (e.g. ``("Hydrophobic", "Hydrophobic")``) and
-        values are lists of references to custom functions (see Examples for more details).
+        where keys are tuples of feature names \
+        (e.g. ``("Hydrophobic", "Hydrophobic")``) and values are lists of
+        references to custom functions (see Examples for more details).
         If not provided, the default LUNA methods will be used instead.
     add_non_cov : bool
          If True (the default), compute non-covalent interactions.
-         If you are providing custom functions to compute non-covalent interactions and
-         want to make them controllable by this flag, make sure to verify the state of
-         ``add_non_cov`` at the beginning of the function and return an empty list in case it is False.
+         If you are providing custom functions to compute non-covalent
+         interactions and want to make them controllable by this flag, make
+         sure to verify the state of ``add_non_cov`` at the beginning of the
+         function and return an empty list in case it is False.
     add_cov : bool
         If True (the default), compute covalent interactions.
-        If you are providing custom functions to compute covalent interactions and
-        want to make them controllable by this flag, make sure to verify the state of
-        ``add_cov`` at the beginning of the function and return an empty list in case it is False.
+        If you are providing custom functions to compute covalent interactions
+        and want to make them controllable by this flag, make sure to verify
+        the state of ``add_cov`` at the beginning of the function and return
+        an empty list in case it is False.
     add_proximal : bool
-        If True, compute proximal interactions, which are only distance-based contacts between atoms
-        or atom groups that, therefore, only imply proximity. The default value is False.
-        If you are providing custom functions to compute proximal interactions and
-        want to make them controllable by this flag, make sure to verify the state of
-        ``add_proximal`` at the beginning of the function and return an empty list in case it is False.
+        If True, compute proximal interactions, which are only distance-based
+        contacts between atoms or atom groups that, therefore, only imply
+        proximity. The default value is False. If you are providing custom
+        functions to compute proximal interactions and want to make them
+        controllable by this flag, make sure to verify the state of
+        ``add_proximal`` at the beginning of the function and return an empty
+        list in case it is False.
     add_atom_atom : bool
         If True (the default), compute atom-atom interactions,
-        which, as the name suggests, are interactions that only involve atoms no matter their features.
-        If you are providing custom functions to compute atom-atom interactions and want to make them
-        controllable by this flag, make sure to verify the state of ``add_atom_atom`` at the beginning
-        of the function and return an empty list in case it is False.
+        which, as the name suggests, are interactions that only involve atoms
+        no matter their features. If you are providing custom functions to
+        compute atom-atom interactions and want to make them controllable by
+        this flag, make sure to verify the state of ``add_atom_atom`` at the
+        beginning of the function and return an empty list in case it is False.
 
         .. note::
-            In LUNA, we consider the following interactions as atom-atom: `Van der Waals`,
-            `Van der Waals clash`, and `Atom overlap`. We opted to separate `Van der Waals` from
-            other non-covalent interactions because LUNA may generate an unnecessary number of additional
-            interactions that are usually already represented by other non-covalent interactions as
-            weak hydrogen bonds, hydrophobic, or dipole-dipole interactions.
-            Thus, to give users a fine-grain control over which interactions to calculate,
-            we provided this additional flag to turn off the calculation of Van der Waals interactions.
+            In LUNA, we consider the following interactions as atom-atom:
+            `Van der Waals`, `Van der Waals clash`, and `Atom overlap`.
+            We opted to separate `Van der Waals` from other non-covalent
+            interactions because LUNA may generate an unnecessary number of
+            additional interactions that are usually already represented by
+            other non-covalent interactions as weak hydrogen bonds,
+            hydrophobic, or dipole-dipole interactions. Thus, to give users
+            a fine-grain control over which interactions to calculate, we
+            provided this additional flag to turn off the calculation of
+            Van der Waals interactions.
     add_dependent_inter : bool
         If True, compute interactions that depend on other interactions.
-        Currently, only water-bridged hydrogen bonds and salt bridges have a dependency on
-        other interactions. The first, depends on two or more hydrogen bonds, while the second depends on
-        an ionic and a hydrogen bond. The default value is False, which implies no dependent interaction
-        will be computed.
+        Currently, only water-bridged hydrogen bonds and salt bridges have a
+        dependency on other interactions. The first, depends on two or more
+        hydrogen bonds, while the second depends on an ionic and a hydrogen
+        bond. The default value is False, which implies no dependent
+        interaction will be computed.
     add_h2o_pairs_with_no_target : bool
-        If True, keep interactions of water with atoms and atom groups that do not belong to the target
-        of LUNA's analysis, which are chains or molecules defined as an :class:`~luna.mol.entry.Entry` instance.
-        For example, if the target is a ligand and ``add_h2o_pairs_with_no_target`` is False,
-        then water-water and water-residue hydrogen bonds will be removed because the ligand is not
+        If True, keep interactions of water with atoms and atom groups that
+        do not belong to the target of LUNA's analysis, which are chains or
+        molecules defined as an :class:`~luna.mol.entry.Entry` instance.
+        For example, if the target is a ligand and
+        ``add_h2o_pairs_with_no_target`` is False, then water-water and
+        water-residue hydrogen bonds will be removed because the ligand is not
         participating in the interactions. The default value is False.
     strict_donor_rules : bool
-        If True (the default), hydrogen bonds will only be considered for donor atoms with explicit
-        hydrogens bound to them. In that case, angles and distances will be evaluated.
-        However, if the molecule containing the donor atom is in ``lazy_comps_list``, then angles and hydrogens
-        will be ignored and LUNA will proceed with the determination of hydrogen bonds based only on
-        donor-acceptor distances.
-        Another exception occurs for solvent molecules in which the donor atom is only bound to hydrogens atoms
-        (e.g., water, ammonia, and hydrogen sulfide).
-        In that case, hydrogens can be positioned in many different ways by Open Babel, which may cause LUNA to
-        detect different hydrogen bonds at each run.
-        So, to circumvent this problem, by default, LUNA always ignores the explicit hydrogen position
-        for donor atoms that only contain hydrogens bound to it.
+        If True (the default), hydrogen bonds will only be considered for donor
+        atoms with explicit hydrogens bound to them. In that case, angles and
+        distances will be evaluated. However, if the molecule containing the
+        donor atom is in ``lazy_comps_list``, then angles and hydrogens will be
+        ignored and LUNA will proceed with the determination of hydrogen bonds
+        based only on donor-acceptor distances. Another exception occurs for
+        solvent molecules in which the donor atom is only bound to hydrogens
+        atoms (e.g., water, ammonia, and hydrogen sulfide). In that case,
+        hydrogens can be positioned in many different ways by Open Babel, which
+        may cause LUNA to detect different hydrogen bonds at each run.
+        So, to circumvent this problem, by default, LUNA always ignores the
+        explicit hydrogen position for donor atoms that only contain hydrogens
+        bound to it.
     strict_weak_donor_rules : bool
-        If True (the default), weak hydrogen bonds will only be considered for donor atoms with explicit
-        hydrogens bound to them. In that case, angles and distances will be evaluated.
+        If True (the default), weak hydrogen bonds will only be considered for
+        donor atoms with explicit hydrogens bound to them. In that case, angles
+        and distances will be evaluated.
         The same exceptions described for ``strict_donor_rules`` apply here.
     lazy_comps_list : iterable
-         A sequence of molecule names to ignore explicit hydrogen position during the calculation of hydrogen bonds and weak hydrogen bonds.
-         The default list is ['HOH', 'DOD', 'WAT', 'H2O', 'OH2', 'NH3', 'NH4'], which only contains water, ammonia, and ammonium ion,
-         including water name variations used by different programs.
+         A sequence of molecule names to ignore explicit hydrogen position
+         during the calculation of hydrogen bonds and weak hydrogen bonds.
+         The default list is
+         ['HOH', 'DOD', 'WAT', 'H2O', 'OH2', 'NH3', 'NH4'], which only contains
+         water, ammonia, and ammonium ion, including water name variations
+         used by different programs.
 
 
     Examples
     --------
 
     **Example 1) How to define custom interactions:**
 
-    In this example, we will define a custom function to calculate hydrogen bonds.
+    In this example, we will define a custom function to calculate
+    hydrogen bonds.
 
     First, let's start importing the classes and the function we will use.
 
     >>> from luna.interaction.type import InteractionType
     >>> from luna.interaction.calc import InteractionCalculator
     >>> from luna.util.math import euclidean_distance
 
-    Now, we define the custom function, which simply calculates hydrogen bonds based
-    on donor-acceptor distances. If it is less than 3.5, then a new
-    :class:`~luna.interaction.type.InteractionType` object is created with type `Hydrogen bond`.
+    Now, we define the custom function, which simply calculates hydrogen bonds
+    based on donor-acceptor distances. If it is less than 3.5, then a new
+    :class:`~luna.interaction.type.InteractionType` object is created with type
+    `Hydrogen bond`.
 
     .. code-block::
 
         def custom_hbond_function(self, params):
             if not self.add_non_cov:
                 return []
 
             group1, group2, feat1, feat2 = params
             interactions = []
 
             cc_dist = euclidean_distance(group1.centroid, group2.centroid)
             if cc_dist <= 3.5:
                 params = {"dist_hbond_inter": cc_dist}
-                inter = InteractionType(group1, group2, "Hydrogen bond", params=params)
+                inter = InteractionType(group1, group2, "Hydrogen bond", \
+params=params)
                 interactions.append(inter)
             return interactions
 
     .. note::
-        Observe that the function checks if ``add_non_cov`` has been turned off and if
-        so returns an empty list. That's a recommended strategy because it allows one to
-        turn off all non-covalent interactions with a single flag.
-
-        Also, observe that `InteractionCalculator` always expects functions to return a list at the end.
-        That means multiple interactions may be detected for a single pair of
-        :class:`~luna.mol.groups.AtomGroup` objects.
-        For example, a donor atom containing 2 hydrogens could, in theory, form two
-        different hydrogen bonds with an acceptor atom.
+        Observe that the function checks if ``add_non_cov`` has been turned off
+        and if so returns an empty list. That's a recommended strategy because
+        it allows one to turn off all non-covalent interactions with a single
+        flag.
+
+        Also, observe that `InteractionCalculator` always expects functions to
+        return a list at the end. That means multiple interactions may be
+        detected for a single pair of :class:`~luna.mol.groups.AtomGroup`
+        objects. For example, a donor atom containing 2 hydrogens could,
+        in theory, form two different hydrogen bonds with an acceptor atom.
 
 
-    Now, we have two options to set the custom function to an `InteractionCalculator` object:
+    Now, we have two options to set the custom function to an
+    `InteractionCalculator` object:
 
         1) Define a new dict with the custom functions:
 
         >>> custom_funcs = {("Donor", "Acceptor"): [custom_hbond_function]}
         >>> ic = InteractionCalculator(inter_funcs=custom_funcs)
 
         2) Overwrite the default dict in InteractionCalculator:
 
         >>> ic = InteractionCalculator()
         >>> ic.funcs[("Donor", "Acceptor")] = [custom_hbond_function]
 
     **Example 2)** How to modify parameters to calculate interactions:
 
     If you just want to modify specific values from the default configuration,
-    you can create a new :class:`~luna.interaction.config.DefaultInteractionConfig`,
+    you can create a new
+    :class:`~luna.interaction.config.DefaultInteractionConfig`,
     alter parameters, and pass it to `InteractionCalculator`.
 
     >>> from luna.interaction.calc import InteractionCalculator
     >>> from luna.interaction.config import DefaultInteractionConfig
     >>> custom_config = DefaultInteractionConfig()
     >>> custom_config.config["min_dha_ang_hb_inter"] = 120
     >>> ic = InteractionCalculator(inter_config=custom_config)
 
-    Alternatively, you can initiate a new `InteractionCalculator` without providing an
-    :class:`~luna.interaction.config.InteractionConfig` object, which will cause
-    `InteractionCalculator` to initiate the default configuration.
-    Then, you can modify it directly as we did before.
+    Alternatively, you can initiate a new `InteractionCalculator` without
+    providing an :class:`~luna.interaction.config.InteractionConfig` object,
+    which will cause `InteractionCalculator` to initiate the default
+    configuration. Then, you can modify it directly as we did before.
 
     >>> from luna.interaction.calc import InteractionCalculator
     >>> ic = InteractionCalculator()
     >>> print(ic.inter_config["min_dha_ang_hb_inter"])
     90
     >>> ic.inter_config["min_dha_ang_hb_inter"] = 120
     >>> print(ic.inter_config["min_dha_ang_hb_inter"])
     120
 
-    Finally, if you want to define a custom configuration that will be used in your custom functions,
-    you first need to define the parameters as a dict and then initiate a new
+    Finally, if you want to define a custom configuration that will be
+    used in your custom functions, you first need to define the
+    parameters as a dict and then initiate a new
     :class:`~luna.interaction.config.InteractionConfig`. See below:
 
     >>> from luna.interaction.config import InteractionConfig
     >>> config = {"param1": 2.5, "param2": 90}
     >>> custom_config = InteractionConfig(config)
     >>> ic = InteractionCalculator(inter_config=custom_config)
     >>> print(ic.inter_config["param1"])
@@ -431,41 +477,44 @@
     >>> print(ic.inter_config["param2"])
     90
 
     **Example 3)** How to disable specific parameters and how to enable
     automatic recognition of disabled parameters in custom functions:
 
     To automatically disable, for instance, verification of angles during the
-    calculation of interactions using LUNA's default functions, we just need to remove
-    the parameters related to angles from ``inter_config``. Let's see an example where
-    we disable angles from hydrogen bonds:
+    calculation of interactions using LUNA's default functions, we just need
+    to remove the parameters related to angles from ``inter_config``.
+    Let's see an example where we disable angles from hydrogen bonds:
 
     >>> ic = InteractionCalculator()
     >>> del ic.inter_config["min_dha_ang_hb_inter"]
     >>> del ic.inter_config["min_har_ang_hb_inter"]
     >>> del ic.inter_config["min_dar_ang_hb_inter"]
 
-    This simple behavior is possible thanks to the function `is_within_boundary`,
-    which always returns True if the parameter does not exist in ``inter_config``.
-    Thus, you can take advantage of this system when implementing custom functions
-    so others will also have the possibility to turn off specific parameters without
-    modifying the code directly. Let's see that in practice.
+    This simple behavior is possible thanks to the function
+    `is_within_boundary`, which always returns True if the parameter does not
+    exist in ``inter_config``. Thus, you can take advantage of this system when
+    implementing custom functions so others will also have the possibility to
+    turn off specific parameters without modifying the code directly.
+    Let's see that in practice.
 
     First, let's start importing the classes and the function we will use.
 
     >>> from luna.interaction.config import InteractionConfig
     >>> from luna.interaction.type import InteractionType
     >>> from luna.interaction.calc import InteractionCalculator
     >>> from luna.util.math import euclidean_distance
     >>> from operator import le
 
-    Now, we define a custom function that calculates hydrogen bonds based on donor-acceptor distances only.
-    Observe at line #9 that instead of checking the cutoff directly, we call `is_within_boundary`
-    with the value, parameter, and a comparison function (``le``: less than or equal), which will
-    make it possible to modify or even disable the parameter automatically.
+    Now, we define a custom function that calculates hydrogen bonds based on
+    donor-acceptor distances only. Observe at line #9 that instead of checking
+    the cutoff directly, we call `is_within_boundary` with the value,
+    parameter, and a comparison function (``le``: less than or equal), which
+    will make it possible to modify or even disable the parameter
+    automatically.
 
     .. code-block::
         :linenos:
         :emphasize-lines: 9
 
         def custom_hbond_function(self, params):
             if not self.add_non_cov:
@@ -473,23 +522,26 @@
 
             group1, group2, feat1, feat2 = params
             interactions = []
 
             cc_dist = euclidean_distance(group1.centroid, group2.centroid)
             if self.is_within_boundary(cc_dist, "max_hb_dist", le):
                 params = {"dist_hbond_inter": cc_dist}
-                inter = InteractionType(group1, group2, "Hydrogen bond", params=params)
+                inter = InteractionType(group1, group2, "Hydrogen bond", \
+params=params)
                 interactions.append(inter)
             return interactions
 
-    Finally, we are ready to provide the function and custom parameters to `InteractionCalculator`.
+    Finally, we are ready to provide the function and custom parameters
+    to `InteractionCalculator`.
 
     >>> custom_config = InteractionConfig({"max_hb_dist": 3})
     >>> custom_funcs = {("Donor", "Acceptor"): [custom_hbond_function]}
-    >>> ic = InteractionCalculator(inter_funcs=custom_funcs, inter_config=custom_config)
+    >>> ic = InteractionCalculator(inter_funcs=custom_funcs, \
+inter_config=custom_config)
 
     By doing so, we can now alter the new parameter or turn it off.
 
     >>> ic.inter_config["max_hb_dist"] = 3.5
     >>> del ic.inter_config["max_hb_dist"]
 
     """
@@ -497,15 +549,15 @@
     def __init__(self, inter_config=DefaultInteractionConfig(),
                  inter_filter=None, inter_funcs=None, add_non_cov=True,
                  add_cov=True, add_proximal=False, add_atom_atom=True,
                  add_dependent_inter=False,
                  add_h2o_pairs_with_no_target=False,
                  strict_donor_rules=True,
                  strict_weak_donor_rules=True,
-                 lazy_comps_list=DEFAULT_SOLVENTS):
+                 lazy_comps_list=DEFAULT_LAZY_LIST):
 
         if (inter_config is not None
                 and isinstance(inter_config, InteractionConfig) is False):
             msg = ("The informed interaction configuration "
                    "must be an instance of '%s'." % InteractionConfig)
             raise IllegalArgumentError(msg)
 
@@ -537,44 +589,50 @@
         return self._inter_funcs
 
     @funcs.setter
     def funcs(self, funcs):
         self._inter_funcs = funcs
 
     def calc_interactions(self, trgt_atm_grps, nb_atm_grps=None):
-        """Calculate interactions established by atoms and atoms groups in ``trgt_atm_grps``
-        using methods available in ``funcs``.
+        """Calculate interactions established by atoms and atoms groups in
+        ``trgt_atm_grps`` using methods available in ``funcs``.
 
-        The functions in ``funcs`` are chosen based on the features of each atom or atom group.
-        For example, consider that a pair of :class:`~luna.mol.groups.AtomGroup` objects have both the
-        features 'Hydrophobic'. Then, `calc_interactions` will call any
-        interaction function defined for the tuple ``("Hydrophobic", "Hydrophobic")`` in ``funcs``.
-        Consider now a pair of :class:`~luna.mol.groups.AtomGroup` objects whose features are
-        'Donor' and 'Hydrophobic'. Once again, `calc_interactions` will evaluate if there is any
-        function defined for the tuple ``("Donor", "Hydrophobic")`` (the order does not matter).
+        The functions in ``funcs`` are chosen based on the features of each
+        atom or atom group. For example, consider that a pair of
+        :class:`~luna.mol.groups.AtomGroup` objects have both the features
+        'Hydrophobic'. Then, `calc_interactions` will call any interaction
+        function defined for the tuple ``("Hydrophobic", "Hydrophobic")`` in
+        ``funcs``. Consider now a pair of :class:`~luna.mol.groups.AtomGroup`
+        objects whose features are 'Donor' and 'Hydrophobic'. Once again,
+        `calc_interactions` will evaluate if there is any function defined for
+        the tuple ``("Donor", "Hydrophobic")`` (the order does not matter).
         If there is none, nothing is done and the pair is skipped.
 
         Parameters
         ----------
         trgt_atm_grps : iterable of :class:`~luna.mol.groups.AtomGroup`
-            Compute interactions involving these :class:`~luna.mol.groups.AtomGroup` objects.
+            Compute interactions involving these
+            :class:`~luna.mol.groups.AtomGroup` objects.
         nb_atm_grps : iterable of :class:`~luna.mol.groups.AtomGroup`
-            If defined, only compute interactions between :class:`~luna.mol.groups.AtomGroup` objects from ``trgt_atm_grps``
-            with :class:`~luna.mol.groups.AtomGroup` objects from ``nb_atm_grps``.
-            If not provided, set ``nb_atm_grps`` to be the same as ``trgt_atm_grps``,
-            which implies that interactions will be calculated using only pairs of :class:`~luna.mol.groups.AtomGroup` objects
-            from ``trgt_atm_grps``.
+            If defined, only compute interactions between
+            :class:`~luna.mol.groups.AtomGroup` objects from ``trgt_atm_grps``
+            with :class:`~luna.mol.groups.AtomGroup` objects from
+            ``nb_atm_grps``. If not provided, set ``nb_atm_grps`` to be the
+            same as ``trgt_atm_grps``, which implies that interactions will be
+            calculated using only pairs of :class:`~luna.mol.groups.AtomGroup`
+            objects from ``trgt_atm_grps``.
         """
 
         # TODO: Water-bridged interaction with weak hydrogen bond
-        # TODO: threshold for including slightly out of limit interactions. For example, a hydrogen bond not included for 0.01A.
+        # TODO: threshold for including slightly out of limit interactions.
+        #       For example, a hydrogen bond not included for 0.01A.
         #           Distances: 0.2 and Angles: 5
 
-        # If nb_atm_grps was not informed, it uses the trgt_atm_grps as the neighbors.
-        # In this case, the interactions will be target x target.
+        # If nb_atm_grps was not informed, it uses the trgt_atm_grps as the
+        # neighbors. In this case, the interactions will be target x target.
         nb_comp_grps = nb_atm_grps or trgt_atm_grps
 
         # Define the scope of the neighborhood search.
         ss = AtomGroupNeighborhood(nb_comp_grps, 10)
 
         computed_pairs = set()
         all_interactions = []
@@ -582,63 +640,86 @@
         bsite_param = "bsite_cutoff"
         bsite_cutoff = self.inter_config.get(bsite_param,
                                              BOUNDARY_CONFIG[bsite_param])
 
         for trgt_atm_grp in trgt_atm_grps:
             for nb_atm_grp in ss.search(trgt_atm_grp.centroid, bsite_cutoff):
 
-                # It will always ignore interactions involving the same atom groups.
-                # Loops in the graph is not permitted and does not make any sense.
+                # It will always ignore interactions involving the same atom
+                # groups. Loops in the graph is not permitted and does not make
+                # any sense.
                 if trgt_atm_grp == nb_atm_grp:
                     continue
 
                 # If the pair has already been calculated.
-                if (trgt_atm_grp, nb_atm_grp) in computed_pairs or (nb_atm_grp, trgt_atm_grp) in computed_pairs:
+                if ((trgt_atm_grp, nb_atm_grp) in computed_pairs
+                        or (nb_atm_grp, trgt_atm_grp) in computed_pairs):
                     continue
 
                 # If no filter was informed, it will accept everything.
-                if self.inter_filter is not None and not self.inter_filter.is_valid_pair(trgt_atm_grp, nb_atm_grp):
+                if (self.inter_filter is not None
+                        and not self.inter_filter.is_valid_pair(trgt_atm_grp,
+                                                                nb_atm_grp)):
                     continue
 
                 computed_pairs.add((trgt_atm_grp, nb_atm_grp))
 
-                feat_pairs = list(product(trgt_atm_grp.features, nb_atm_grp.features))
-                feat_pairs = filter(lambda x: self.is_feature_pair_valid(*x), feat_pairs)
-
-                # If the groups belongs to the same molecule (intramolecule interaction).
-                is_intramol_inter = self._is_intramol_inter(trgt_atm_grp, nb_atm_grp)
+                feat_pairs = list(product(trgt_atm_grp.features,
+                                          nb_atm_grp.features))
+                feat_pairs = filter(lambda x: self.is_feature_pair_valid(*x),
+                                    feat_pairs)
+
+                # If the groups belongs to the same molecule
+                # (intramolecule interaction).
+                is_intramol_inter = \
+                    self._is_intramol_inter(trgt_atm_grp, nb_atm_grp)
                 shortest_path_length = None
 
                 for pair in feat_pairs:
-                    # It will ignore interactions for atoms in the same molecule that are separated from each other by only N bonds.
-                    # Covalent bonds keep atoms very tightly, producing distances lower than their sum of Van der Waals radius.
-                    # As a consequence the algorithm will find a lot of false interactions.
+                    # It will ignore interactions for atoms in the same
+                    # molecule that are separated from each other by only
+                    # N bonds. Covalent bonds keep atoms very tightly,
+                    # producing distances lower than their sum of Van der Waals
+                    # radius. As a consequence the algorithm will find a lot of
+                    # false interactions.
                     #
-                    # But, it will never skip pairs of Atom features because they are used to calculate covalent interactions.
-                    if pair[0].name != "Atom" and pair[1].name != "Atom" and is_intramol_inter:
-                        # Compute the shortest path only once. The reason not to precompute it outside the For is to avoid computing
-                        # the algorithm for groups containing only Atom features.
+                    # But, it will never skip pairs of Atom features because
+                    # they are used to calculate covalent interactions.
+                    if (pair[0].name != "Atom" and pair[1].name != "Atom"
+                            and is_intramol_inter):
+                        # Compute the shortest path only once. The reason not
+                        # to precompute it outside the For is to avoid
+                        # computing the algorithm for groups containing only
+                        # Atom features.
                         if shortest_path_length is None:
-                            # By providing a cutoff, it will force the algorithm to return paths only for groups connected by
-                            # less than or equal N paths. So, if two groups return INF, it means they are a valid combination as they
+                            # By providing a cutoff, it will force the
+                            # algorithm to return paths only for groups
+                            # connected by less than or equal N paths.
+                            # So, if two groups return INF, it means
+                            # they are a valid combination as they
                             # match the minimum bond separation.
                             cutoff = self.inter_config.get("min_bond_separation", 0)
                             shortest_path_length = trgt_atm_grp.get_shortest_path_length(nb_atm_grp, cutoff)
 
-                        # If get_shortest_path_length() returns any value that is not infinite (INF), it means these two groups
-                        # contain a path with at less than or equal to the cutoff 'min_bond_separation'. Therefore, ignore them.
+                        # If get_shortest_path_length() returns any value that
+                        # is not infinite (INF), it means these two groups
+                        # contain a path with at less than or equal to the
+                        # cutoff 'min_bond_separation'.
+                        # Therefore, ignore them.
                         if shortest_path_length != float('inf'):
                             continue
 
                     calc_inter_params = (trgt_atm_grp, nb_atm_grp) + pair
-                    interactions = self._resolve_interactions(*calc_inter_params)
+                    interactions = \
+                        self._resolve_interactions(*calc_inter_params)
                     all_interactions.extend(interactions)
 
         if self.add_dependent_inter:
-            dependent_interactions = self.find_dependent_interactions(all_interactions)
+            dependent_interactions = \
+                self.find_dependent_interactions(all_interactions)
             all_interactions.extend(dependent_interactions)
 
         # Get only unique interactions.
         all_interactions = set(all_interactions)
 
         # Remove potential inconsistences. For example: a hydrogen bond and
         # an unfavorable interation between the same atoms.
@@ -663,18 +744,20 @@
         for func in funcs:
             result = func(self, (group1, group2, feat1, feat2)) or []
             interactions.extend(result)
 
         return interactions
 
     def find_dependent_interactions(self, interactions):
-        """ Compute interactions that depend on other interactions. Currently, only water-bridged
-        hydrogen bonds and salt bridges have a dependency on other interactions. The first, depends
-        on two or more hydrogen bonds, while the second depends on an ionic and a hydrogen bond.
-        The default value is False, which implies no dependent interaction will be computed.
+        """ Compute interactions that depend on other interactions.
+        Currently, only water-bridged hydrogen bonds and salt bridges have a
+        dependency on other interactions. The first, depends on two or more
+        hydrogen bonds, while the second depends on an ionic and a hydrogen
+        bond. The default value is False, which implies no dependent
+        interaction will be computed.
 
         Parameters
         ----------
         interactions : :class:`~luna.interaction.type.InteractionType`
             Use these interactions to compute dependent interactions.
         """
         hbond_set = set()
@@ -737,84 +820,104 @@
 
             condA = (ionic.src_grp.has_atom(hbond.src_grp.atoms[0])
                      and ionic.trgt_grp.has_atom(hbond.trgt_grp.atoms[0]))
 
             condB = (ionic.src_grp.has_atom(hbond.trgt_grp.atoms[0])
                      and ionic.trgt_grp.has_atom(hbond.src_grp.atoms[0]))
 
-            # If an acceptor atom belongs to a negative group, and the donor to a positive group
-            # (and vice-versa), it means that the interaction occurs between the same meioties.
-            # However, just one condition should occur. For example, it is not possible that an acceptor
-            # atom belongs to a negative and positive group at the same time.
+            # If an acceptor atom belongs to a negative group, and the donor
+            # to a positive group (and vice-versa), it means that the
+            # interaction occurs between the same meioties. However, just one
+            # condition should occur. For example, it is not possible that an
+            # acceptor atom belongs to a negative and positive group at the
+            # same time.
             if condA ^ condB:
                 key1 = (ionic.src_grp, ionic.trgt_grp)
                 key2 = (ionic.trgt_grp, ionic.src_grp)
 
                 if key1 in sb_groups or key2 in sb_groups:
                     continue
 
                 if isinstance(self.inter_filter, InteractionFilter):
-                    if not self.inter_filter.is_valid_pair(ionic.src_grp, ionic.trgt_grp):
+                    if not self.inter_filter.is_valid_pair(ionic.src_grp,
+                                                           ionic.trgt_grp):
                         continue
 
                 sb_groups.add(key1)
                 params = {"depends_on": [hbond, ionic]}
 
-                inter = InteractionType(ionic.src_grp, ionic.trgt_grp, "Salt bridge", params=params)
+                inter = InteractionType(ionic.src_grp,
+                                        ionic.trgt_grp,
+                                        "Salt bridge",
+                                        params=params)
                 dependent_interactions.add(inter)
 
         return dependent_interactions
 
     def remove_inconsistencies(self, interactions):
         """Remove conflicts between interactions in ``interactions``.
 
         .. note::
-            By default, LUNA defines conflicts as any unfavorable dipole interaction involving an
-            atom establishing a hydrogen bond. Due to the strength of a hydrogen bond, atoms may
-            approximate more to each other, which sometimes may cause unfavorable interactions
-            involving dipoles to be detected. To avoid such conflicts, LUNA removes the
-            unfavorable interactions.
-
-            Also, it may occur that unfavorable dipole interactions are detected for
-            amide-aromatic stackings, in which the aromatic ring contains heteroatoms.
-            To avoid such conflicts, LUNA also removes those unfavorable interactions.
+            By default, LUNA defines conflicts as any unfavorable dipole
+            interaction involving an atom establishing a hydrogen bond.
+            Due to the strength of a hydrogen bond, atoms may approximate more
+            to each other, which sometimes may cause unfavorable interactions
+            involving dipoles to be detected. To avoid such conflicts, LUNA
+            removes the unfavorable interactions.
+
+            Also, it may occur that unfavorable dipole interactions are
+            detected for amide-aromatic stackings, in which the aromatic
+            ring contains heteroatoms. To avoid such conflicts, LUNA also
+            removes those unfavorable interactions.
 
         Parameters
         ----------
         interactions : :class:`~luna.interaction.type.InteractionType`
         """
         amide_inconsistences = defaultdict(list)
         hbond_inconsistences = defaultdict(list)
         for inter in interactions:
             if inter.type == "Unfavorable nucleophile-nucleophile":
                 # A nucleophile may have only 1 atom (water oxygen).
                 atm1 = inter.src_grp.atoms[0]
-                # If a nucleophile has 2 atoms, it will select the partially negative atom based on the electronegativity.
+                # If a nucleophile has 2 atoms, it will select the partially
+                # negative atom based on the electronegativity.
                 if len(inter.src_grp.atoms) == 2:
-                    atm1 = inter.src_grp.atoms[0] if (inter.src_grp.atoms[0].electronegativity
-                                                      > inter.src_grp.atoms[1].electronegativity) else inter.src_grp.atoms[1]
+                    atm1 = (inter.src_grp.atoms[0]
+                            if (inter.src_grp.atoms[0].electronegativity
+                                > inter.src_grp.atoms[1].electronegativity)
+                            else inter.src_grp.atoms[1])
 
                 # A nucleophile may have only 1 atom (water oxygen).
                 atm2 = inter.trgt_grp.atoms[0]
-                # If a nucleophile has 2 atoms, it will select the partially negative atom based on the electronegativity.
+                # If a nucleophile has 2 atoms, it will select the partially
+                # negative atom based on the electronegativity.
                 if len(inter.trgt_grp.atoms) == 2:
-                    atm2 = inter.trgt_grp.atoms[0] if (inter.trgt_grp.atoms[0].electronegativity
-                                                       > inter.trgt_grp.atoms[1].electronegativity) else inter.trgt_grp.atoms[1]
+                    atm2 = (inter.trgt_grp.atoms[0]
+                            if (inter.trgt_grp.atoms[0].electronegativity
+                                > inter.trgt_grp.atoms[1].electronegativity)
+                            else inter.trgt_grp.atoms[1])
                 key = (atm1, atm2)
                 if (atm2, atm1) in hbond_inconsistences:
                     key = (atm2, atm1)
                 hbond_inconsistences[key].append(inter)
             elif inter.type == "Unfavorable anion-nucleophile":
-                nucl_grp = inter.src_grp if any([f.name == "Nucleophile" for f in inter.src_grp.features]) else inter.trgt_grp
+                nucl_grp = (inter.src_grp
+                            if any([f.name == "Nucleophile"
+                                    for f in inter.src_grp.features])
+                            else inter.trgt_grp)
                 # A nucleophile may have only 1 atom (water oxygen).
                 nucl_atm = nucl_grp.atoms[0]
-                # If a nucleophile has 2 atoms, it will select the partially negative atom based on the electronegativity.
+                # If a nucleophile has 2 atoms, it will select the partially
+                # negative atom based on the electronegativity.
                 if len(nucl_grp.atoms) == 2:
-                    nucl_atm = nucl_grp.atoms[0] if (nucl_grp.atoms[0].electronegativity
-                                                     > nucl_grp.atoms[1].electronegativity) else nucl_grp.atoms[1]
+                    nucl_atm = (nucl_grp.atoms[0]
+                                if (nucl_grp.atoms[0].electronegativity
+                                    > nucl_grp.atoms[1].electronegativity)
+                                else nucl_grp.atoms[1])
                 anion_grp = inter.get_partner(nucl_grp)
                 for anion_atm in anion_grp.atoms:
                     key = (nucl_atm, anion_atm)
                     if (anion_atm, nucl_atm) in hbond_inconsistences:
                         key = (anion_atm, nucl_atm)
                     hbond_inconsistences[key].append(inter)
             elif inter.type == "Hydrogen bond":
@@ -822,48 +925,62 @@
                 atm1, atm2 = (inter.src_grp.atoms[0], inter.trgt_grp.atoms[0])
 
                 key = (atm1, atm2)
                 if (atm2, atm1) in hbond_inconsistences:
                     key = (atm2, atm1)
                 hbond_inconsistences[key].append(inter)
             elif inter.type == "Amide-aromatic stacking":
-                amide_grp = inter.src_grp if any([f.name == "Amide" for f in inter.src_grp.features]) else inter.trgt_grp
+                amide_grp = (inter.src_grp
+                             if any([f.name == "Amide"
+                                     for f in inter.src_grp.features])
+                             else inter.trgt_grp)
                 arom_grp = inter.get_partner(amide_grp)
                 for amide_atm in amide_grp.atoms:
                     amide_inconsistences[(amide_atm, arom_grp)].append(inter)
             elif inter.type == "Unfavorable cation-electrophile":
-                elect_grp = inter.src_grp if any([f.name == "Nucleophile" for f in inter.src_grp.features]) else inter.trgt_grp
+                elect_grp = (inter.src_grp
+                             if any([f.name == "Nucleophile"
+                                     for f in inter.src_grp.features])
+                             else inter.trgt_grp)
                 # A nucleophile may have only 1 atom (water oxygen).
                 elect_atm = elect_grp.atoms[0]
-                # If a nucleophile has 2 atoms, it will select the partially negative atom based on the electronegativity.
+                # If a nucleophile has 2 atoms, it will select the partially
+                # negative atom based on the electronegativity.
                 if len(elect_grp.atoms) == 2:
-                    elect_atm = elect_grp.atoms[0] if (elect_grp.atoms[0].electronegativity
-                                                       > elect_grp.atoms[1].electronegativity) else elect_grp.atoms[1]
+                    elect_atm = (elect_grp.atoms[0]
+                                 if (elect_grp.atoms[0].electronegativity
+                                     > elect_grp.atoms[1].electronegativity)
+                                 else elect_grp.atoms[1])
 
                 cation_grp = inter.get_partner(elect_grp)
                 amide_inconsistences[(elect_atm, cation_grp)].append(inter)
 
         inconsistencies = set()
         for (atm1, atm2), inters in hbond_inconsistences.items():
-            if len(inters) > 1 and any([i.type == "Hydrogen bond" for i in inters]):
-                inconsistencies.update([i for i in inters if i.type != "Hydrogen bond"])
+            if (len(inters) > 1
+                    and any([i.type == "Hydrogen bond" for i in inters])):
+                inconsistencies.update([i for i in inters
+                                        if i.type != "Hydrogen bond"])
 
         for (amide_atm, arom_grp), inters in amide_inconsistences.items():
             if len(inters) > 1:
-                inconsistencies.update([i for i in inters if i.type != "Amide-aromatic stacking"])
+                inter_name = "Amide-aromatic stacking"
+                inconsistencies.update([i for i in inters
+                                        if i.type != inter_name])
 
         interactions -= inconsistencies
 
         # Clear the references of each interaction from the AtomGroup objects.
         for inter in inconsistencies:
             inter.clear_refs()
 
     def remove_h2o_pairs_with_no_target(self, interactions):
-        """Remove interactions of water with atoms and atom groups that do not belong to the target
-        of LUNA's analysis, which are chains or molecules defined as an :class:`~luna.mol.entry.Entry` instance.
+        """Remove interactions of water with atoms and atom groups that do not
+        belong to the target of LUNA's analysis, which are chains or molecules
+        defined as an :class:`~luna.mol.entry.Entry` instance.
 
         Parameters
         ----------
         interactions : :class:`~luna.interaction.type.InteractionType`
         """
         valid_h2o_set = set()
         h2o_interactions = set()
@@ -897,99 +1014,99 @@
         interactions -= inters_to_remove
 
         # Clear the references of each interaction from the AtomGroup objects.
         for inter in inters_to_remove:
             inter.clear_refs()
 
     def _default_functions(self):
-        return {
-                    # Hydrophobic interaction
-                    ("Hydrophobic", "Hydrophobic"): [self.calc_hydrop],
-                    ("Hydrophobe", "Hydrophobe"): [self.calc_hydrop],
-
-                    # Hydrogen bond
-                    ("Donor", "Acceptor"): [self.calc_hbond],
-
-                    # Weak hydrogen bond
-                    ("WeakDonor", "Acceptor"): [self.calc_weak_hbond],
-                    ("WeakDonor", "WeakAcceptor"): [self.calc_weak_hbond],
-                    ("Donor", "Aromatic"): [self.calc_hbond_pi],
-                    ("WeakDonor", "Aromatic"): [self.calc_hbond_pi],
-
-                    # Halogen bond
-                    ("HalogenDonor", "Acceptor"): [self.calc_xbond],
-                    ("HalogenDonor", "Aromatic"): [self.calc_xbond_pi],
-
-                    # Chalcogen bond
-                    ("ChalcogenDonor", "Acceptor"): [self.calc_chalc_bond],
-                    ("ChalcogenDonor", "Aromatic"): [self.calc_chalc_bond_pi],
-
-                    # Stackings
-                    ("Aromatic", "Aromatic"): [self.calc_pi_pi],
-                    ("Amide", "Aromatic"): [self.calc_amide_pi],
-                    ("Positive", "Aromatic"): [self.calc_cation_pi],
-                    ("PosIonizable", "Aromatic"): [self.calc_cation_pi],
-                    ("PositivelyIonizable", "Aromatic"): [self.calc_cation_pi],
-
-                    # Ionic interaction
-                    ("NegativelyIonizable",
-                     "PositivelyIonizable"): [self.calc_ionic],
-                    ("NegIonizable", "PosIonizable"): [self.calc_ionic],
-                    ("Negative", "Positive"): [self.calc_ionic],
-
-                    # Repulsive interaction
-                    ("NegativelyIonizable",
-                     "NegativelyIonizable"): [self.calc_repulsive],
-                    ("PositivelyIonizable",
-                     "PositivelyIonizable"): [self.calc_repulsive],
-                    ("NegIonizable", "NegIonizable"): [self.calc_repulsive],
-                    ("PosIonizable", "PosIonizable"): [self.calc_repulsive],
-                    ("Negative", "Negative"): [self.calc_repulsive],
-                    ("Positive", "Positive"): [self.calc_repulsive],
-
-                    # Favorable multipolar interactions.
-                    ("Nucleophile", "Electrophile"): [self.calc_multipolar],
-
-                    # Unfavorable multipolar interactions.
-                    ("Nucleophile", "Nucleophile"): [self.calc_multipolar],
-                    ("Electrophile", "Electrophile"): [self.calc_multipolar],
-
-                    # Favorable ion-dipole interactions
-                    ("Nucleophile",
-                     "PositivelyIonizable"): [self.calc_ion_multipole],
-                    ("Nucleophile",
-                     "PosIonizable"): [self.calc_ion_multipole],
-                    ("Nucleophile",
-                     "Positive"): [self.calc_ion_multipole],
-                    ("Electrophile",
-                     "NegativelyIonizable"): [self.calc_ion_multipole],
-                    ("Electrophile",
-                     "NegIonizable"): [self.calc_ion_multipole],
-                    ("Electrophile",
-                     "Negative"): [self.calc_ion_multipole],
-
-                    # Unfavorable ion-dipole interactions
-                    ("Nucleophile",
-                     "NegativelyIonizable"): [self.calc_ion_multipole],
-                    ("Nucleophile",
-                     "NegIonizable"): [self.calc_ion_multipole],
-                    ("Nucleophile",
-                     "Negative"): [self.calc_ion_multipole],
-                    ("Electrophile",
-                     "PositivelyIonizable"): [self.calc_ion_multipole],
-                    ("Electrophile",
-                     "PosIonizable"): [self.calc_ion_multipole],
-                    ("Electrophile",
-                     "Positive"): [self.calc_ion_multipole],
-
-                    # Proximal, covalent, vdw, clash
-                    ("Atom", "Atom"): [self.calc_atom_atom, self.calc_proximal]
-            }
+        #         Hydrophobic interaction
+        return {("Hydrophobic", "Hydrophobic"): [self.calc_hydrop],
+                ("Hydrophobe", "Hydrophobe"): [self.calc_hydrop],
+
+                # Hydrogen bond
+                ("Donor", "Acceptor"): [self.calc_hbond],
+
+                # Weak hydrogen bond
+                ("WeakDonor", "Acceptor"): [self.calc_weak_hbond],
+                ("WeakDonor", "WeakAcceptor"): [self.calc_weak_hbond],
+                ("Donor", "Aromatic"): [self.calc_hbond_pi],
+                ("WeakDonor", "Aromatic"): [self.calc_hbond_pi],
+
+                # Halogen bond
+                ("HalogenDonor", "Acceptor"): [self.calc_xbond],
+                ("HalogenDonor", "Aromatic"): [self.calc_xbond_pi],
+
+                # Chalcogen bond
+                ("ChalcogenDonor", "Acceptor"): [self.calc_chalc_bond],
+                ("ChalcogenDonor", "Aromatic"): [self.calc_chalc_bond_pi],
+
+                # Stackings
+                ("Aromatic", "Aromatic"): [self.calc_pi_pi],
+                ("Amide", "Aromatic"): [self.calc_amide_pi],
+                ("Positive", "Aromatic"): [self.calc_cation_pi],
+                ("PosIonizable", "Aromatic"): [self.calc_cation_pi],
+                ("PositivelyIonizable", "Aromatic"): [self.calc_cation_pi],
+
+                # Ionic interaction
+                ("NegativelyIonizable",
+                 "PositivelyIonizable"): [self.calc_ionic],
+                ("NegIonizable", "PosIonizable"): [self.calc_ionic],
+                ("Negative", "Positive"): [self.calc_ionic],
+
+                # Repulsive interaction
+                ("NegativelyIonizable",
+                 "NegativelyIonizable"): [self.calc_repulsive],
+                ("PositivelyIonizable",
+                 "PositivelyIonizable"): [self.calc_repulsive],
+                ("NegIonizable", "NegIonizable"): [self.calc_repulsive],
+                ("PosIonizable", "PosIonizable"): [self.calc_repulsive],
+                ("Negative", "Negative"): [self.calc_repulsive],
+                ("Positive", "Positive"): [self.calc_repulsive],
+
+                # Favorable multipolar interactions.
+                ("Nucleophile", "Electrophile"): [self.calc_multipolar],
+
+                # Unfavorable multipolar interactions.
+                ("Nucleophile", "Nucleophile"): [self.calc_multipolar],
+                ("Electrophile", "Electrophile"): [self.calc_multipolar],
+
+                # Favorable ion-dipole interactions
+                ("Nucleophile",
+                 "PositivelyIonizable"): [self.calc_ion_multipole],
+                ("Nucleophile",
+                 "PosIonizable"): [self.calc_ion_multipole],
+                ("Nucleophile",
+                 "Positive"): [self.calc_ion_multipole],
+                ("Electrophile",
+                 "NegativelyIonizable"): [self.calc_ion_multipole],
+                ("Electrophile",
+                 "NegIonizable"): [self.calc_ion_multipole],
+                ("Electrophile",
+                 "Negative"): [self.calc_ion_multipole],
+
+                # Unfavorable ion-dipole interactions
+                ("Nucleophile",
+                 "NegativelyIonizable"): [self.calc_ion_multipole],
+                ("Nucleophile",
+                 "NegIonizable"): [self.calc_ion_multipole],
+                ("Nucleophile",
+                 "Negative"): [self.calc_ion_multipole],
+                ("Electrophile",
+                 "PositivelyIonizable"): [self.calc_ion_multipole],
+                ("Electrophile",
+                 "PosIonizable"): [self.calc_ion_multipole],
+                ("Electrophile",
+                 "Positive"): [self.calc_ion_multipole],
+
+                ("Atom", "Metal"): [self.calc_metal_coord],
+
+                # Proximal, covalent, vdw, clash
+                ("Atom", "Atom"): [self.calc_atom_atom, self.calc_proximal]}
 
-        # TODO: Incluir:
+        # TODO: Include:
 
         # Anion - pi system
 
         # disulfide bond
 
         # Weak donor - weak acceptor
 
@@ -1007,32 +1124,37 @@
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
 
         group1, group2, feat1, feat2 = params
         interactions = []
 
         cc_dist = im.euclidean_distance(group1.centroid, group2.centroid)
 
         if (self.is_within_boundary(cc_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(cc_dist, "max_dist_cation_pi_inter", le)):
+                and self.is_within_boundary(cc_dist,
+                                            "max_dist_cation_pi_inter",
+                                            le)):
             params = {"dist_cation_pi_inter": cc_dist}
             inter = InteractionType(group1, group2, "Cation-pi", params=params)
 
             interactions.append(inter)
         return interactions
 
     @staticmethod
@@ -1041,95 +1163,126 @@
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
 
         ring1, ring2, feat1, feat2 = params
         interactions = []
 
         cc_dist = im.euclidean_distance(ring1.centroid, ring2.centroid)
 
         if (self.is_within_boundary(cc_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(cc_dist, "max_cc_dist_pi_pi_inter", le)):
+                and self.is_within_boundary(cc_dist, "max_cc_dist_pi_pi_inter",
+                                            le)):
 
             dihedral_angle = im.to_quad1(im.angle(ring1.normal, ring2.normal))
 
             min_disp_angle = float("Inf")
             for r1, r2 in [(ring1, ring2), (ring2, ring1)]:
                 cc_vect = r2.centroid - r1.centroid
                 disp_angle = im.to_quad1(im.angle(r1.normal, cc_vect))
 
                 if disp_angle < min_disp_angle:
                     ring1, ring2 = r1, r2
                     min_disp_angle = disp_angle
 
-            criteria = ["min_dihed_ang_slope_pi_pi_inter", "max_dihed_ang_slope_pi_pi_inter", "min_disp_ang_offset_pi_pi_inter",
+            criteria = ["min_dihed_ang_slope_pi_pi_inter",
+                        "max_dihed_ang_slope_pi_pi_inter",
+                        "min_disp_ang_offset_pi_pi_inter",
                         "max_disp_ang_offset_pi_pi_inter"]
 
-            # If the angle criterion were not defined, a specific Pi-stacking definition is not possible as it depends on
-            # angle criterion. Therefore, a more general classification is used instead, i.e., all interactions will be Pi-stacking.
+            # If the angle criterion were not defined, a specific Pi-stacking
+            # definition is not possible as it depends on angle criterion.
+            # Therefore, a more general classification is used instead, i.e.,
+            # all interactions will be Pi-stacking.
             if any([c not in self.inter_config for c in criteria]):
                 inter_type = "Pi-stacking"
-            elif self.is_within_boundary(min_disp_angle, "min_disp_ang_offset_pi_pi_inter", le):
-                if self.is_within_boundary(dihedral_angle, "min_dihed_ang_slope_pi_pi_inter", le):
+            elif self.is_within_boundary(min_disp_angle,
+                                         "min_disp_ang_offset_pi_pi_inter",
+                                         le):
+                if self.is_within_boundary(dihedral_angle,
+                                           "min_dihed_ang_slope_pi_pi_inter",
+                                           le):
                     inter_type = "Face-to-face pi-stacking"
-                elif self.is_within_boundary(dihedral_angle, "max_dihed_ang_slope_pi_pi_inter", ge):
+                elif self.is_within_boundary(dihedral_angle,
+                                             "max_dihed_ang_slope_pi_pi_inter",
+                                             ge):
                     inter_type = "Face-to-edge pi-stacking"
                 else:
                     inter_type = "Face-to-slope pi-stacking"
-            elif self.is_within_boundary(min_disp_angle, "max_disp_ang_offset_pi_pi_inter", ge):
-                if self.is_within_boundary(dihedral_angle, "min_dihed_ang_slope_pi_pi_inter", le):
+            elif self.is_within_boundary(min_disp_angle,
+                                         "max_disp_ang_offset_pi_pi_inter",
+                                         ge):
+                if self.is_within_boundary(dihedral_angle,
+                                           "min_dihed_ang_slope_pi_pi_inter",
+                                           le):
                     inter_type = "Edge-to-edge pi-stacking"
-                elif self.is_within_boundary(dihedral_angle, "max_dihed_ang_slope_pi_pi_inter", ge):
+                elif self.is_within_boundary(dihedral_angle,
+                                             "max_dihed_ang_slope_pi_pi_inter",
+                                             ge):
                     inter_type = "Edge-to-face pi-stacking"
                 else:
                     inter_type = "Edge-to-slope pi-stacking"
             else:
-                if self.is_within_boundary(dihedral_angle, "min_dihed_ang_slope_pi_pi_inter", le):
+                if self.is_within_boundary(dihedral_angle,
+                                           "min_dihed_ang_slope_pi_pi_inter",
+                                           le):
                     inter_type = "Displaced face-to-face pi-stacking"
-                elif self.is_within_boundary(dihedral_angle, "max_dihed_ang_slope_pi_pi_inter", ge):
+                elif self.is_within_boundary(dihedral_angle,
+                                             "max_dihed_ang_slope_pi_pi_inter",
+                                             ge):
                     inter_type = "Displaced face-to-edge pi-stacking"
                 else:
                     inter_type = "Displaced face-to-slope pi-stacking"
 
             params = {"cc_dist_pi_pi_inter": cc_dist,
                       "dihed_ang_pi_pi_inter": dihedral_angle,
                       "disp_ang_pi_pi_inter": min_disp_angle}
 
-            inter = InteractionType(ring1, ring2, inter_type, directional=True, params=params)
+            inter = InteractionType(ring1,
+                                    ring2,
+                                    inter_type,
+                                    directional=True,
+                                    params=params)
             interactions.append(inter)
 
         return interactions
 
     @staticmethod
     def calc_amide_pi(self, params):
         """Default method to calculate amide-pi stackings.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
@@ -1140,76 +1293,96 @@
         if feat1.name == "Aromatic" and feat2.name == "Amide":
             ring_grp = group1
             amide_grp = group2
         elif feat2.name == "Aromatic" and feat1.name == "Amide":
             ring_grp = group2
             amide_grp = group1
         else:
-            logger.warning("Amide-aromatic interactions require an aromatic and an amide group. However, the informed "
-                           "groups have the features %s and %s." % (group1.feature_names, group2.feature_names))
+            logger.warning("Amide-aromatic interactions require an aromatic "
+                           "and an amide group. However, the informed groups "
+                           "have the features %s and %s."
+                           % (group1.feature_names, group2.feature_names))
             return []
 
         # Distance between the amide and ring centroids.
         cc_dist = im.euclidean_distance(ring_grp.centroid, amide_grp.centroid)
 
         if (self.is_within_boundary(cc_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(cc_dist, "max_cc_dist_amide_pi_inter", le)):
+                and self.is_within_boundary(cc_dist,
+                                            "max_cc_dist_amide_pi_inter", le)):
 
-            dihedral_angle = im.to_quad1(im.angle(ring_grp.normal, amide_grp.normal))
+            dihedral_angle = im.to_quad1(im.angle(ring_grp.normal,
+                                                  amide_grp.normal))
             cc_vect = amide_grp.centroid - ring_grp.centroid
             disp_angle = im.to_quad1(im.angle(ring_grp.normal, cc_vect))
 
-            if (self.is_within_boundary(dihedral_angle, "max_dihed_ang_amide_pi_inter", le)
-                    and self.is_within_boundary(disp_angle, "max_disp_ang_pi_pi_inter", le)):
+            if (self.is_within_boundary(dihedral_angle,
+                                        "max_dihed_ang_amide_pi_inter", le)
+                    and self.is_within_boundary(disp_angle,
+                                                "max_disp_ang_pi_pi_inter",
+                                                le)):
 
                 params = {"cc_dist_amide_pi_inter": cc_dist,
                           "dihed_ang_amide_pi_inter": dihedral_angle,
                           "disp_ang_amide_pi_inter": disp_angle}
 
-                inter = InteractionType(group1, group2, "Amide-aromatic stacking", params=params)
+                inter = InteractionType(group1,
+                                        group2,
+                                        "Amide-aromatic stacking",
+                                        params=params)
                 interactions.append(inter)
         return interactions
 
     @staticmethod
     def calc_hydrop(self, params):
         """Default method to calculate hydrophobic interactons.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
 
         group1, group2, feat1, feat2 = params
         interactions = []
 
         if ((feat1.name != "Hydrophobic" and feat1.name != "Hydrophobe")
-                or (feat2.name != "Hydrophobic" and feat2.name != "Hydrophobe")):
-            logger.warning("Hydrophobic interactions require hydrophobic atoms or hydrophobes (group of hydrophobic atoms). "
-                           "However, the informed groups have the features %s and %s." % (group1.feature_names, group2.feature_names))
+                or (feat2.name != "Hydrophobic"
+                    and feat2.name != "Hydrophobe")):
+            logger.warning("Hydrophobic interactions require hydrophobic "
+                           "atoms or hydrophobes (group of hydrophobic "
+                           "atoms). However, the informed groups have the "
+                           "features %s and %s."
+                           % (group1.feature_names, group2.feature_names))
             return []
 
-        # Check if the interaction involves the same compound. For these cases, we ignore hydrophobic interactions.
+        # Check if the interaction involves the same compound.
+        # For these cases, we ignore hydrophobic interactions.
         if self._is_intramol_inter(group1, group2):
             return []
 
-        # Verify if the groups contain the required number of atoms to form a valid surface.
+        # Verify if the groups contain the required number of atoms to
+        # form a valid surface.
         if (not self.is_within_boundary(len(group1.atoms), "min_surf_size", ge)
-                or not self.is_within_boundary(len(group2.atoms), "min_surf_size", ge)):
+                or not self.is_within_boundary(len(group2.atoms),
+                                               "min_surf_size", ge)):
             return []
 
         interacting_atms_in_surf1 = set()
         interacting_atms_in_surf2 = set()
         min_cc_dist = float('Inf')
         for atm1, atm2 in product(group1.atoms, group2.atoms):
             cc_dist = atm1 - atm2
@@ -1217,41 +1390,50 @@
             if self.is_within_boundary(cc_dist, "max_dist_hydrop_inter", le):
                 interacting_atms_in_surf1.add(atm1)
                 interacting_atms_in_surf2.add(atm2)
 
                 if cc_dist < min_cc_dist:
                     min_cc_dist = cc_dist
 
-        # Verify if the number of interacting atoms attends the required number of interating atoms per surface.
+        # Verify if the number of interacting atoms attends the required number
+        # of interating atoms per surface.
         if (not self.is_within_boundary(len(interacting_atms_in_surf1), "min_inter_atom_in_surf", ge)
                 or not self.is_within_boundary(len(interacting_atms_in_surf2), "min_inter_atom_in_surf", ge)):
             return []
 
         if (self.is_within_boundary(min_cc_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(min_cc_dist, "max_dist_hydrop_inter", le)):
+                and self.is_within_boundary(min_cc_dist,
+                                            "max_dist_hydrop_inter", le)):
 
             params = {"dist_hydrop_inter": min_cc_dist}
-            inter = InteractionType(group1, group2, "Hydrophobic", params=params)
+            inter = InteractionType(group1,
+                                    group2,
+                                    "Hydrophobic",
+                                    params=params)
             interactions.append(inter)
 
         return interactions
 
     @staticmethod
     def calc_ion_multipole(self, params):
-        """Default method to calculate favorable and unfavorable ion-dipole interactions.
+        """Default method to calculate favorable and unfavorable ion-dipole
+        interactions.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
@@ -1284,286 +1466,427 @@
         elif feat1.name == "Electrophile" and feat2.name in CATIONS:
             dipole_grp, dipole_type = group1, "Electrophile"
             ion_grp, ion_type = group2, "Cation"
         elif feat1.name in CATIONS and feat2.name == "Electrophile":
             dipole_grp, dipole_type = group2, "Electrophile"
             ion_grp, ion_type = group1, "Cation"
         else:
-            logger.warning("Ion-dipole interactions require a dipole and an ion group. However, the informed groups "
-                           "have the features %s and %s." % (group1.feature_names, group2.feature_names))
+            logger.warning("Ion-dipole interactions require a dipole and an "
+                           "ion group. However, the informed groups have the "
+                           "features %s and %s."
+                           % (group1.feature_names, group2.feature_names))
             return []
 
         # A nucleophile may have only 1 atom (water oxygen).
         part_charged_atm = dipole_grp.atoms[0]
-        # If a nucleophile has 2 atoms, it will select the partially negative atom based on the electronegativity.
+        # If a nucleophile has 2 atoms, it will select the partially negative
+        # atom based on the electronegativity.
         if len(dipole_grp.atoms) == 2 and dipole_type == "Nucleophile":
-            part_charged_atm = dipole_grp.atoms[0] if (dipole_grp.atoms[0].electronegativity
-                                                       > dipole_grp.atoms[1].electronegativity) else dipole_grp.atoms[1]
+            part_charged_atm = \
+                (dipole_grp.atoms[0]
+                 if (dipole_grp.atoms[0].electronegativity
+                     > dipole_grp.atoms[1].electronegativity)
+                 else dipole_grp.atoms[1])
 
-        # If an electrophile has two atoms. It will select the partially negative atom based on the electronegativity.
+        # If an electrophile has two atoms. It will select the partially
+        # negative atom based on the electronegativity.
         elif len(dipole_grp.atoms) == 2 and dipole_type == "Electrophile":
-            part_charged_atm = dipole_grp.atoms[0] if (dipole_grp.atoms[0].electronegativity
-                                                       < dipole_grp.atoms[1].electronegativity) else dipole_grp.atoms[1]
+            part_charged_atm = \
+                (dipole_grp.atoms[0]
+                 if (dipole_grp.atoms[0].electronegativity
+                     < dipole_grp.atoms[1].electronegativity)
+                 else dipole_grp.atoms[1])
 
         # Distance between the ion and the dipole.
-        id_dist = im.euclidean_distance(part_charged_atm.coord, ion_grp.centroid)
+        id_dist = im.euclidean_distance(part_charged_atm.coord,
+                                        ion_grp.centroid)
 
         if (self.is_within_boundary(id_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(id_dist, "max_id_dist_ion_multipole_inter", le)):
+                and self.is_within_boundary(id_dist,
+                                            "max_id_dist_ion_multipole_inter",
+                                            le)):
 
             idy_angle = -1
             if len(dipole_grp.atoms) == 2:
-                # Model: I ... D-Y, where I is the ion, D the dipole atom of interest (the electrophile or nucleophile),
+                # Model: I ... D-Y, where I is the ion, D the dipole atom of
+                # interest (the electrophile or nucleophile),
                 # and Y is its counterpart.
                 y_atm = dipole_grp.atoms[1] if dipole_grp.atoms[0] == part_charged_atm else dipole_grp.atoms[0]
                 di_vect = ion_grp.centroid - part_charged_atm.coord
                 dy_vect = y_atm.coord - part_charged_atm.coord
                 idy_angle = im.angle(di_vect, dy_vect)
 
-            # Dipoles containing only one atom are allowed to pass without checking the angle IDY.
+            # Dipoles containing only one atom are allowed to pass without
+            # checking the angle IDY.
             if len(dipole_grp.atoms) == 1 or self.is_within_boundary(idy_angle, "min_idy_ang_ion_multipole_inter", ge):
 
-                dipole_nb_coords = [nbi.coord for nbi in part_charged_atm.neighbors_info if nbi.atomic_num != 1]
+                dipole_nb_coords = [nbi.coord
+                                    for nbi in part_charged_atm.neighbors_info
+                                    if nbi.atomic_num != 1]
                 params = {}
                 if len(dipole_nb_coords) > 1:
-                    dipole_normal = im.calc_normal(dipole_nb_coords + [part_charged_atm.coord])
+                    dipole_normal \
+                        = im.calc_normal(dipole_nb_coords
+                                         + [part_charged_atm.coord])
                     disp_angle = im.to_quad1(im.angle(dipole_normal, di_vect))
 
-                    if self.is_within_boundary(disp_angle, "max_disp_ang_ion_multipole_inter", le):
+                    prop_name = "max_disp_ang_ion_multipole_inter"
+                    if self.is_within_boundary(disp_angle, prop_name, le):
                         params = {"id_dist_ion_multipole_inter": id_dist,
                                   "idy_ang_ion_multipole_inter": idy_angle,
                                   "disp_ang_ion_multipole_inter": disp_angle}
                 else:
                     params = {"id_dist_ion_multipole_inter": id_dist,
                               "idy_ang_ion_multipole_inter": idy_angle,
                               "disp_ang_ion_multipole_inter": -1}
 
                 if params:
                     if dipole_type == "Nucleophile" and ion_type == "Cation":
-                        inter = InteractionType(dipole_grp, ion_grp, "Cation-nucleophile", params=params)
+                        inter = InteractionType(dipole_grp, ion_grp,
+                                                "Cation-nucleophile",
+                                                params=params)
                         interactions.append(inter)
                     elif dipole_type == "Nucleophile" and ion_type == "Anion":
-                        inter = InteractionType(dipole_grp, ion_grp, "Unfavorable anion-nucleophile", params=params)
+                        inter_name = "Unfavorable anion-nucleophile"
+                        inter = InteractionType(dipole_grp, ion_grp,
+                                                inter_name, params=params)
                         interactions.append(inter)
                     elif dipole_type == "Electrophile" and ion_type == "Anion":
-                        inter = InteractionType(ion_grp, dipole_grp, "Anion-electrophile", params=params)
+                        inter = InteractionType(ion_grp, dipole_grp,
+                                                "Anion-electrophile",
+                                                params=params)
                         interactions.append(inter)
-                    elif dipole_type == "Electrophile" and ion_type == "Cation":
-                        inter = InteractionType(ion_grp, dipole_grp, "Unfavorable cation-electrophile", params=params)
+                    elif (dipole_type == "Electrophile"
+                            and ion_type == "Cation"):
+                        inter_name = "Unfavorable cation-electrophile"
+                        inter = InteractionType(ion_grp, dipole_grp,
+                                                inter_name, params=params)
                         interactions.append(inter)
         return interactions
 
     @staticmethod
     def calc_multipolar(self, params):
-        """Default method to calculate favorable and unfavorable dipole-dipole interactions.
+        """Default method to calculate favorable and unfavorable dipole-dipole
+        interactions.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
 
         group1, group2, feat1, feat2 = params
         interactions = []
 
-        if len(group1.atoms) != 1 and len(group1.atoms) != 2 and len(group2.atoms) != 1 and len(group2.atoms) != 2:
-            logger.warning("A dipole group should have 1 (for cases when the atom has only hydrogens bonded to it) or 2 atoms. "
-                           "However, the informed groups '%s' and '%s' have %d and %d atoms, respectively."
-                           % (group1, group2, len(group1.atoms), len(group2.atoms)))
+        if (len(group1.atoms) != 1 and len(group1.atoms) != 2
+                and len(group2.atoms) != 1 and len(group2.atoms) != 2):
+            logger.warning("A dipole group should have 1 (for cases when the "
+                           "atom has only hydrogens bonded to it) or 2 atoms. "
+                           "However, the informed groups '%s' and '%s' have "
+                           "%d and %d atoms, respectively."
+                           % (group1, group2,
+                              len(group1.atoms), len(group2.atoms)))
             return []
 
-        # The reference dipole will always be the second one, i.e., one of its atom will be the center in the angle NEY.
+        # The reference dipole will always be the second one, i.e., one of its
+        # atom will be the center in the angle NEY.
         #
-        # Favorable interactions: in these cases, the Dipole 1 will always be the nucleophile and the Dipole 2 the
-        # electrophile in order to represent the nucleophile atack, i.e., the angles calculated using the dipole 2 as reference
-        # represents how the nucleophile aproximate the electrophile.
+        # Favorable interactions: in these cases, the Dipole 1 will always be
+        # the nucleophile and the Dipole 2 the electrophile in order to
+        # represent the nucleophile atack, i.e., the angles calculated using
+        # the dipole 2 as reference represents how the nucleophile aproximate
+        # the electrophile.
         if feat1.name == "Nucleophile" and feat2.name == "Electrophile":
             dipole_grp1, dipole_type1 = group1, feat1.name
             dipole_grp2, dipole_type2 = group2, feat2.name
         elif feat2.name == "Nucleophile" and feat1.name == "Electrophile":
             dipole_grp1, dipole_type1 = group2, feat2.name
             dipole_grp2, dipole_type2 = group1, feat1.name
-        # Unfavorable interactions: in these cases, the reference dipole will depend on the number of atoms in the dipoles.
-        # With dipoles containing 1 atom, it takes a generous approach by ignoring angles and accepting everything.
-        # With dipoles containing two atoms, it requires that at least one of the angles fits the rules to be accepted.
-        elif feat1.name == feat2.name and (feat1.name == "Nucleophile" or feat1.name == "Electrophile"):
-            # If only one group contains 1 atom, use it as the dipole 2 because it is used as the reference to calculate
-            # the NEY angle. Since we take a generous approach, with one atom no angle will be calculated and the interaction
-            # will be accepted.
+        # Unfavorable interactions: in these cases, the reference dipole will
+        # depend on the number of atoms in the dipoles. With dipoles containing
+        # 1 atom, it takes a generous approach by ignoring angles and accepting
+        # everything.
+        #
+        # With dipoles containing two atoms, it requires that at least one of
+        # the angles fits the rules to be accepted.
+        elif (feat1.name == feat2.name
+                and (feat1.name == "Nucleophile"
+                     or feat1.name == "Electrophile")):
+            # If only one group contains 1 atom, use it as the dipole 2 because
+            # it is used as the reference to calculate the NEY angle. Since we
+            # take a generous approach, with one atom no angle will be
+            # calculated and the interaction will be accepted.
             if len(group1.atoms) == 1 and len(group2.atoms) == 2:
                 dipole_grp1, dipole_type1 = group2, feat2.name
                 dipole_grp2, dipole_type2 = group1, feat1.name
-            # All the other number combinations ([2,1], [1,1], [2, 2]) come here.
+            # All the other number combinations ([2,1], [1,1], [2, 2]) come
+            # here.
             else:
                 dipole_grp1, dipole_type1 = group1, feat1.name
                 dipole_grp2, dipole_type2 = group2, feat2.name
         else:
-            logger.warning("Multipolar interactions require a nucleophile and an electrophile group. "
-                           "However, the informed groups have the features %s and %s." % (group1.feature_names, group2.feature_names))
+            logger.warning("Multipolar interactions require a nucleophile and "
+                           "an electrophile group. However, the informed "
+                           "groups have the features %s and %s."
+                           % (group1.feature_names, group2.feature_names))
             return []
 
-        # Ignore dipoles containing at least one common atom, which can happen to covalently bound dipoles.
-        # An example of it is the C-S-C substructure that contains two dipoles.
+        # Ignore dipoles containing at least one common atom, which can happen
+        # to covalently bound dipoles. An example of it is the C-S-C
+        # substructure that contains two dipoles.
         if any(atm in group2.atoms for atm in group1.atoms):
             return []
 
         # Atom 1 => Dipole 1
         #
         # A nucleophile may have only 1 atom (water oxygen).
         dipole_atm1 = dipole_grp1.atoms[0]
-        # If it has 2 atoms, it will select the nucleophilic atom based on the electronegativity.
+        # If it has 2 atoms, it will select the nucleophilic atom based on the
+        # electronegativity.
         if len(dipole_grp1.atoms) == 2 and dipole_type1 == "Nucleophile":
-            dipole_atm1 = dipole_grp1.atoms[0] if (dipole_grp1.atoms[0].electronegativity
-                                                   > dipole_grp1.atoms[1].electronegativity) else dipole_grp1.atoms[1]
-        # Or, it will select the nucleophilic atom based on the electronegativity.
+            dipole_atm1 = (dipole_grp1.atoms[0]
+                           if (dipole_grp1.atoms[0].electronegativity
+                               > dipole_grp1.atoms[1].electronegativity)
+                           else dipole_grp1.atoms[1])
+        # Or, it will select the nucleophilic atom based on the
+        # electronegativity.
         elif len(dipole_grp1.atoms) == 2 and dipole_type1 == "Electrophile":
-            dipole_atm1 = dipole_grp1.atoms[0] if (dipole_grp1.atoms[0].electronegativity
-                                                   < dipole_grp1.atoms[1].electronegativity) else dipole_grp1.atoms[1]
+            dipole_atm1 = (dipole_grp1.atoms[0]
+                           if (dipole_grp1.atoms[0].electronegativity
+                               < dipole_grp1.atoms[1].electronegativity)
+                           else dipole_grp1.atoms[1])
 
         # Atom 2 => Dipole 2
         #
-        # An electrophile may have only 1 atom. E.g.: NH4, although by default we consider it as an ion.
+        # An electrophile may have only 1 atom. E.g.: NH4, although by default
+        # we consider it as an ion.
         dipole_atm2 = dipole_grp2.atoms[0]
-        # If it has 2 atoms, it will select the nucleophilic atom based on the electronegativity.
+        # If it has 2 atoms, it will select the nucleophilic atom based on the
+        # electronegativity.
         if len(dipole_grp2.atoms) == 2 and dipole_type2 == "Nucleophile":
-            dipole_atm2 = dipole_grp2.atoms[0] if (dipole_grp2.atoms[0].electronegativity
-                                                   > dipole_grp2.atoms[1].electronegativity) else dipole_grp2.atoms[1]
-        # Or, it will select the nucleophilic atom based on the electronegativity.
+            dipole_atm2 = (dipole_grp2.atoms[0]
+                           if (dipole_grp2.atoms[0].electronegativity
+                               > dipole_grp2.atoms[1].electronegativity)
+                           else dipole_grp2.atoms[1])
+        # Or, it will select the nucleophilic atom based on the
+        # electronegativity.
         elif len(dipole_grp2.atoms) == 2 and dipole_type2 == "Electrophile":
-            dipole_atm2 = dipole_grp2.atoms[0] if (dipole_grp2.atoms[0].electronegativity
-                                                   < dipole_grp2.atoms[1].electronegativity) else dipole_grp2.atoms[1]
+            dipole_atm2 = (dipole_grp2.atoms[0]
+                           if (dipole_grp2.atoms[0].electronegativity
+                               < dipole_grp2.atoms[1].electronegativity)
+                           else dipole_grp2.atoms[1])
 
         # Model for favorable interactions: A-N ... E-Y
         # Model for unfavorable interactions: A-N ... N-A, Y-E ... E-Y.
         #
-        # Although there are two different models for unfavorable interactions, the method for them are equal to the
-        # favorable interaction. So, from now on, we will deal with them as if it was the first model.
+        # Although there are two different models for unfavorable interactions,
+        # the method for them are equal to the favorable interaction.
+        # So, from now on, we will deal with them as if it was the first model.
         #
         # Distance between the nucleophile and electrophile.
         ne_dist = im.euclidean_distance(dipole_atm1.coord, dipole_atm2.coord)
 
         if (self.is_within_boundary(ne_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(ne_dist, "max_ne_dist_multipolar_inter", le)):
+                and self.is_within_boundary(ne_dist,
+                                            "max_ne_dist_multipolar_inter",
+                                            le)):
 
-            # No angle can be calculated if the electrophile (dipole 2) has only one atom.
+            # No angle can be calculated if the electrophile (dipole 2) has
+            # only one atom.
             if len(dipole_grp2.atoms) == 1:
                 params = {"ne_dist_multipolar_inter": ne_dist,
                           "ney_ang_multipolar_inter": -1,
                           "disp_ang_multipolar_inter": -1,
                           "an_ey_ang_multipolar_inter": -1}
 
                 inter_type = ("Multipolar" if not dipole_type1 == dipole_type2
-                              else "Unfavorable %s-%s" % (dipole_type1.lower(), dipole_type2.lower()))
-                inter = InteractionType(dipole_grp1, dipole_grp2, inter_type, directional=True, params=params)
+                              else "Unfavorable %s-%s"
+                              % (dipole_type1.lower(), dipole_type2.lower()))
+                inter = InteractionType(dipole_grp1, dipole_grp2, inter_type,
+                                        directional=True, params=params)
                 interactions.append(inter)
 
             else:
                 dipole1 = (dipole_grp1, dipole_atm1, dipole_type1)
                 dipole2 = (dipole_grp2, dipole_atm2, dipole_type2)
 
                 combinations = [(dipole1, dipole2)]
-                # For unfavorable interactions, it is necessary to evaluate each combination of dipoles. So, it can
-                # produce two interactions.
+                # For unfavorable interactions, it is necessary to evaluate
+                # each combination of dipoles. So, it can produce two
+                # interactions.
                 if feat1.name == feat2.name:
                     combinations = [(dipole1, dipole2), (dipole2, dipole1)]
 
                 for d1, d2 in combinations:
                     dipole_grp1, dipole_atm1, dipole_type1 = d1
                     dipole_grp2, dipole_atm2, dipole_type2 = d2
 
                     # Model: A-N ... E-Y
-                    y_atm = dipole_grp2.atoms[1] if dipole_grp2.atoms[0] == dipole_atm2 else dipole_grp2.atoms[0]
+                    y_atm = (dipole_grp2.atoms[1]
+                             if dipole_grp2.atoms[0] == dipole_atm2
+                             else dipole_grp2.atoms[0])
                     en_vect = dipole_atm1.coord - dipole_atm2.coord
                     ey_vect = y_atm.coord - dipole_atm2.coord
                     ney_angle = im.angle(en_vect, ey_vect)
 
-                    if (self.is_within_boundary(ney_angle, "min_ney_ang_multipolar_inter", ge)
-                            and self.is_within_boundary(ney_angle, "max_ney_ang_multipolar_inter", le)):
-
-                        elect_nb_coords = [nbi.coord for nbi in dipole_atm2.neighbors_info if nbi.atomic_num != 1]
-                        elect_normal = im.calc_normal(elect_nb_coords + [dipole_atm2.coord])
-                        disp_angle = im.to_quad1(im.angle(elect_normal, en_vect))
-
-                        if self.is_within_boundary(disp_angle, "max_disp_ang_multipolar_inter", le):
-
-                            # If the nucleophile has two atoms, then we will be able to calculate the angle between the vectors AN and EY.
-                            # This angle is necessary to define the orientation of the dipole.
+                    prop_name1 = "min_ney_ang_multipolar_inter"
+                    prop_name2 = "max_ney_ang_multipolar_inter"
+                    if (self.is_within_boundary(ney_angle, prop_name1, ge)
+                            and self.is_within_boundary(ney_angle,
+                                                        prop_name2, le)):
+
+                        elect_nb_coords = \
+                            [nbi.coord
+                             for nbi in dipole_atm2.neighbors_info
+                             if nbi.atomic_num != 1]
+                        elect_normal = \
+                            im.calc_normal(elect_nb_coords
+                                           + [dipole_atm2.coord])
+                        disp_angle = im.to_quad1(im.angle(elect_normal,
+                                                          en_vect))
+
+                        prop_name = "max_disp_ang_multipolar_inter"
+                        if self.is_within_boundary(disp_angle, prop_name, le):
+
+                            # If the nucleophile has two atoms, then we will be
+                            # able to calculate the angle between the vectors AN
+                            # and EY. This angle is necessary to define the
+                            # orientation of the dipole.
                             if len(dipole_grp1.atoms) == 2:
                                 # Model: A-N ... E-Y
-                                a_atm = dipole_grp1.atoms[1] if dipole_grp1.atoms[0] == dipole_atm1 else dipole_grp1.atoms[0]
+                                a_atm = (dipole_grp1.atoms[1]
+                                         if dipole_grp1.atoms[0] == dipole_atm1
+                                         else dipole_grp1.atoms[0])
                                 an_vect = dipole_atm1.coord - a_atm.coord
                                 # Angle between vectors AN and EY
                                 an_ey_vect_angle = im.angle(an_vect, ey_vect)
 
-                                params = {"ne_dist_multipolar_inter": ne_dist,
-                                          "ney_ang_multipolar_inter": ney_angle,
-                                          "disp_ang_multipolar_inter": disp_angle,
-                                          "an_ey_ang_multipolar_inter": an_ey_vect_angle}
+                                params = \
+                                    {"ne_dist_multipolar_inter": ne_dist,
+                                     "ney_ang_multipolar_inter": ney_angle,
+                                     "disp_ang_multipolar_inter": disp_angle,
+                                     "an_ey_ang_multipolar_inter": an_ey_vect_angle}
 
                                 if not dipole_type1 == dipole_type2:
-                                    if self.is_within_boundary(an_ey_vect_angle, "max_an_ey_ang_para_multipolar_inter", le):
-                                        inter = InteractionType(dipole_grp1, dipole_grp2, "Parallel multipolar",
-                                                                directional=True, params=params)
+                                    if self.is_within_boundary(an_ey_vect_angle,
+                                                               "max_an_ey_ang_para_multipolar_inter",
+                                                               le):
+                                        inter_name = "Parallel multipolar"
+                                        inter = \
+                                            InteractionType(dipole_grp1,
+                                                            dipole_grp2,
+                                                            inter_name,
+                                                            directional=True,
+                                                            params=params)
                                         interactions.append(inter)
-                                    elif self.is_within_boundary(an_ey_vect_angle, "min_an_ey_ang_antipara_multipolar_inter", ge):
-                                        inter = InteractionType(dipole_grp1, dipole_grp2, "Antiparallel multipolar",
-                                                                directional=True, params=params)
+
+                                    elif self.is_within_boundary(an_ey_vect_angle,
+                                                                 "min_an_ey_ang_antipara_multipolar_inter",
+                                                                 ge):
+                                        inter_name = "Antiparallel multipolar"
+                                        inter = \
+                                            InteractionType(dipole_grp1,
+                                                            dipole_grp2,
+                                                            inter_name,
+                                                            directional=True,
+                                                            params=params)
                                         interactions.append(inter)
-                                    elif (self.is_within_boundary(an_ey_vect_angle, "min_an_ey_ang_ortho_multipolar_inter", ge)
-                                            and self.is_within_boundary(an_ey_vect_angle, "max_an_ey_ang_ortho_multipolar_inter", le)):
-                                        inter = InteractionType(dipole_grp1, dipole_grp2, "Orthogonal multipolar",
-                                                                directional=True, params=params)
+
+                                    elif (self.is_within_boundary(an_ey_vect_angle,
+                                                                  "min_an_ey_ang_ortho_multipolar_inter",
+                                                                  ge)
+                                            and self.is_within_boundary(an_ey_vect_angle,
+                                                                        "max_an_ey_ang_ortho_multipolar_inter",
+                                                                        le)):
+                                        inter_name = "Orthogonal multipolar"
+                                        inter = \
+                                            InteractionType(dipole_grp1,
+                                                            dipole_grp2,
+                                                            inter_name,
+                                                            directional=True,
+                                                            params=params)
                                         interactions.append(inter)
+
                                     else:
-                                        inter = InteractionType(dipole_grp1, dipole_grp2, "Tilted multipolar",
-                                                                directional=True, params=params)
+                                        inter_name = "Tilted multipolar"
+                                        inter = \
+                                            InteractionType(dipole_grp1,
+                                                            dipole_grp2,
+                                                            inter_name,
+                                                            directional=True,
+                                                            params=params)
                                         interactions.append(inter)
+
                                 else:
-                                    inter_type = "Unfavorable %s-%s" % (dipole_type1.lower(), dipole_type2.lower())
-                                    inter = InteractionType(dipole_grp1, dipole_grp2, inter_type, directional=True, params=params)
+                                    inter_type = ("Unfavorable %s-%s"
+                                                  % (dipole_type1.lower(),
+                                                     dipole_type2.lower()))
+                                    inter = InteractionType(dipole_grp1,
+                                                            dipole_grp2,
+                                                            inter_type,
+                                                            directional=True,
+                                                            params=params)
                                     interactions.append(inter)
 
-                            # Otherwise, ignore the angle AN and EY and add a general interaction (Multipolar) without a specific
-                            # definition of the orientation. It will happen only with Water molecules.
+                            # Otherwise, ignore the angle AN and EY and add a
+                            # general interaction (Multipolar) without a
+                            # specific definition of the orientation. It will
+                            # happen only with Water molecules.
                             else:
-                                params = {"ne_dist_multipolar_inter": ne_dist,
-                                          "ney_ang_multipolar_inter": ney_angle,
-                                          "disp_ang_multipolar_inter": disp_angle,
-                                          "an_ey_ang_multipolar_inter": -1}
-                                inter_type = ("Multipolar" if not dipole_type1 == dipole_type2
-                                              else "Unfavorable %s-%s" % (dipole_type1.lower(), dipole_type2.lower()))
-                                inter = InteractionType(dipole_grp1, dipole_grp2, inter_type, directional=True, params=params)
+                                params = \
+                                    {"ne_dist_multipolar_inter": ne_dist,
+                                     "ney_ang_multipolar_inter": ney_angle,
+                                     "disp_ang_multipolar_inter": disp_angle,
+                                     "an_ey_ang_multipolar_inter": -1}
+                                inter_type = \
+                                    ("Multipolar"
+                                     if (not dipole_type1 == dipole_type2)
+                                     else "Unfavorable %s-%s"
+                                     % (dipole_type1.lower(),
+                                        dipole_type2.lower()))
+                                inter = InteractionType(dipole_grp1,
+                                                        dipole_grp2,
+                                                        inter_type,
+                                                        directional=True,
+                                                        params=params)
                                 interactions.append(inter)
 
         return interactions
 
     @staticmethod
     def calc_xbond_pi(self, params):
-        """Default method to calculate halogen bonds between halogens and aromatic rings.
+        """Default method to calculate halogen bonds between halogens and
+        aromatic rings.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
@@ -1582,69 +1905,87 @@
         donor_atm = donor_grp.atoms[0]
 
         # Interaction model: C-X ---- A
         # Defining the XA distance, in which A is the ring center
         xa_dist = im.euclidean_distance(donor_grp.centroid, ring_grp.centroid)
 
         if (self.is_within_boundary(xa_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(xa_dist, "max_xc_dist_xbond_inter", le)):
+                and self.is_within_boundary(xa_dist,
+                                            "max_xc_dist_xbond_inter", le)):
 
             ax_vect = donor_grp.centroid - ring_grp.centroid
             disp_angle = im.to_quad1(im.angle(ring_grp.normal, ax_vect))
 
-            if (self.is_within_boundary(disp_angle, "max_disp_ang_xbond_inter", le)):
+            if (self.is_within_boundary(disp_angle,
+                                        "max_disp_ang_xbond_inter", le)):
                 # Interaction model: C-X ---- A
                 # XA vector is always the same
                 xa_vect = ring_grp.centroid - donor_grp.centroid
 
                 # Defining angle CXA, in which A is the ring center
-                # It may happen that X is covalently bound to more than one group.
-                # In such cases the halogen may also form more than one halogen bond.
+                # It may happen that X is covalently bound to more than one
+                # group. In such cases the halogen may also form more than
+                # one halogen bond.
+                #
                 # Ref: Cavallo, G. et al. The Halogen Bond. (2016).
-                carbon_coords = [nbi.coord for nbi in donor_atm.neighbors_info if nbi.atomic_num == 6]
+                #
+                carbon_coords = [nbi.coord
+                                 for nbi in donor_atm.neighbors_info
+                                 if nbi.atomic_num == 6]
                 for c_coord in carbon_coords:
                     xc_vect = c_coord - donor_grp.centroid
                     cxa_angle = im.angle(xc_vect, xa_vect)
 
-                    if (self.is_within_boundary(cxa_angle, "min_cxa_ang_xbond_inter", ge)):
+                    if (self.is_within_boundary(cxa_angle,
+                                                "min_cxa_ang_xbond_inter",
+                                                ge)):
                         params = {"xc_dist_xbond_inter": xa_dist,
                                   "disp_ang_xbond_inter": disp_angle,
                                   "cxa_ang_xbond_inter": cxa_angle}
 
-                        inter = InteractionType(donor_grp, ring_grp, "Halogen-pi", directional=True, params=params)
+                        inter = InteractionType(donor_grp,
+                                                ring_grp,
+                                                "Halogen-pi",
+                                                directional=True,
+                                                params=params)
                         interactions.append(inter)
         return interactions
 
     @staticmethod
     def calc_xbond(self, params):
         """Default method to calculate halogen bonds.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
 
         group1, group2, feat1, feat2 = params
         interactions = []
 
         if len(group1.atoms) != 1 or len(group2.atoms) != 1:
-            logger.warning("One or more invalid atom groups were informed: %s and %s. In halogen bonds, halogen donor "
-                           "and acceptor groups should always contain only one atom." % (group1, group2))
+            logger.warning("One or more invalid atom groups were informed: "
+                           "%s and %s. In halogen bonds, halogen donor "
+                           "and acceptor groups should always contain only "
+                           "one atom." % (group1, group2))
             return []
 
         if (feat1.name == "Acceptor" and feat2.name == "HalogenDonor"):
             donor_grp = group2
             acceptor_grp = group1
         else:
             donor_grp = group1
@@ -1652,91 +1993,116 @@
 
         # There are always just one donor/acceptor atom.
         donor_atm = donor_grp.atoms[0]
         acceptor_atm = acceptor_grp.atoms[0]
 
         # Interaction model: C-X ---- A-R
         # Distance XA.
-        xa_dist = im.euclidean_distance(donor_grp.centroid, acceptor_grp.centroid)
+        xa_dist = im.euclidean_distance(donor_grp.centroid,
+                                        acceptor_grp.centroid)
 
         if (self.is_within_boundary(xa_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(xa_dist, "max_xa_dist_xbond_inter", le)):
+                and self.is_within_boundary(xa_dist,
+                                            "max_xa_dist_xbond_inter", le)):
 
             # Interaction model: C-X ---- A-R
             # XA vector is always the same
             xa_vect = acceptor_grp.centroid - donor_grp.centroid
 
             # Defining the angle CXA
             # It may happen that X is covalently bound to more than one group.
-            # In such cases the halogen may also form more than one halogen bond.
-            # Ref: Cavallo, G. et al. The Halogen Bond. (2016).
-            carbon_coords = [nbi.coord for nbi in donor_atm.neighbors_info if nbi.atomic_num == 6]
+            # In such cases the halogen may also form more than one
+            # halogen bond. Ref: Cavallo, G. et al. The Halogen Bond. (2016).
+            carbon_coords = [nbi.coord
+                             for nbi in donor_atm.neighbors_info
+                             if nbi.atomic_num == 6]
 
             # Interaction model: C-X ---- A-R.
             # R coordinates, in which R is a heavy atom.
-            r_coords = [nbi.coord for nbi in acceptor_atm.neighbors_info if nbi.atomic_num != 1]
+            r_coords = [nbi.coord
+                        for nbi in acceptor_atm.neighbors_info
+                        if nbi.atomic_num != 1]
 
             for c_coord in carbon_coords:
                 xc_vect = c_coord - donor_grp.centroid
                 cxa_angle = im.angle(xc_vect, xa_vect)
 
-                if self.is_within_boundary(cxa_angle, "min_cxa_ang_xbond_inter", ge):
+                if self.is_within_boundary(cxa_angle,
+                                           "min_cxa_ang_xbond_inter", ge):
 
-                    # If no heavy atom is bonded to the acceptor, it means that only hydrogens may be bound to it. Then, we do not
-                    # calculate the angles because hydrogens are too dynamic, i.e., the acceptor could be ionized or not at a
-                    # specific moment in time and its hydrogens may be positioned in different ways.
+                    # If no heavy atom is bonded to the acceptor, it means that
+                    # only hydrogens may be bound to it. Then, we do not
+                    # calculate the angles because hydrogens are too dynamic,
+                    # i.e., the acceptor could be ionized or not at a specific
+                    # moment in time and its hydrogens may be positioned in
+                    # different ways.
                     if len(r_coords) == 0:
                         params = {"xa_dist_xbond_inter": xa_dist,
                                   "cxa_ang_xbond_inter": cxa_angle,
                                   "xar_ang_xbond_inter": -1}
 
-                        inter = InteractionType(donor_grp, acceptor_grp, "Halogen bond", directional=True, params=params)
+                        inter = InteractionType(donor_grp,
+                                                acceptor_grp,
+                                                "Halogen bond",
+                                                directional=True,
+                                                params=params)
                         interactions.append(inter)
                     else:
                         # AX vector is always the same.
                         # Obs: the donor_grp is the Halogen (X).
                         ax_vect = donor_grp.centroid - acceptor_grp.centroid
 
                         lowest_xar_angle = None
                         for r_coord in r_coords:
                             ar_vect = r_coord - acceptor_grp.centroid
                             xar_angle = im.angle(ax_vect, ar_vect)
 
                             # Update the XAR angle with the lowest value.
-                            if lowest_xar_angle is None or xar_angle < lowest_xar_angle:
+                            if (lowest_xar_angle is None
+                                    or xar_angle < lowest_xar_angle):
                                 lowest_xar_angle = xar_angle
 
-                        # The angle will be None when any R (heavy atom) atom was found.
-                        # In this case, the criteria must always fail.
+                        # The angle will be None when any R (heavy atom) atom
+                        # was found. In this case, the criteria must always
+                        # fail.
                         if lowest_xar_angle is None:
                             lowest_xar_angle = -1
 
-                        if self.is_within_boundary(lowest_xar_angle, "min_xar_ang_xbond_inter", ge):
+                        prop_name = "min_xar_ang_xbond_inter"
+                        if self.is_within_boundary(lowest_xar_angle,
+                                                   prop_name, ge):
                             params = {"xa_dist_xbond_inter": xa_dist,
                                       "cxa_ang_xbond_inter": cxa_angle,
                                       "xar_ang_xbond_inter": lowest_xar_angle}
 
-                            inter = InteractionType(donor_grp, acceptor_grp, "Halogen bond", directional=True, params=params)
+                            inter = InteractionType(donor_grp,
+                                                    acceptor_grp,
+                                                    "Halogen bond",
+                                                    directional=True,
+                                                    params=params)
                             interactions.append(inter)
 
         return interactions
 
     @staticmethod
     def calc_chalc_bond(self, params):
         """Default method to calculate chalcogen bonds.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f`
+            and :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
@@ -1763,100 +2129,126 @@
         acceptor_atm = acceptor_grp.atoms[0]
 
         # Interaction model: R-Y --- A-N
         # Distance YA.
         ya_dist = im.euclidean_distance(donor_grp.centroid,
                                         acceptor_grp.centroid)
 
+        prop_name = "max_ya_dist_ybond_inter"
         if (self.is_within_boundary(ya_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(ya_dist, "max_ya_dist_ybond_inter", le)):
+                and self.is_within_boundary(ya_dist, prop_name, le)):
 
             # Interaction model: R-Y --- A-N
             # YA vector is always the same
             ya_vect = acceptor_grp.centroid - donor_grp.centroid
 
             # Defining the angle RYA
-            r_atms = [nbi for nbi in donor_atm.neighbors_info if nbi.atomic_num != 1]
-            r_elems = sorted([nbi.atomic_num for nbi in donor_atm.neighbors_info if nbi.atomic_num != 1])
+            r_atms = [nbi for nbi in donor_atm.neighbors_info
+                      if nbi.atomic_num != 1]
+            r_elems = sorted([nbi.atomic_num
+                              for nbi in donor_atm.neighbors_info
+                              if nbi.atomic_num != 1])
 
             # Isothiazoles have only one sigma-hole located on the oposite
             # site of the N. Therefore, we should only evaluate this
             # sigma-hole by ignoring the angle formed with the carbon.
             # Ref: https://doi.org/10.1021/jm501853m.
             ignore_carbon = False
             if len(r_elems) == 2 and r_elems[0] == 6 and r_elems[1] == 7:
                 ignore_carbon = True
 
             # Interaction model: R-Y --- A-N.
             # N coordinates, in which N is a heavy atom.
-            n_coords = [nbi.coord for nbi in acceptor_atm.neighbors_info if nbi.atomic_num != 1]
+            n_coords = [nbi.coord
+                        for nbi in acceptor_atm.neighbors_info
+                        if nbi.atomic_num != 1]
 
             for r_atm in r_atms:
                 # Isothiazoles have only one sigma-hole located on the oposite
                 # site of the N. So, we must ignore the Carbon.
                 # Ref: https://doi.org/10.1021/jm501853m.
                 if r_atm.atomic_num == 6 and ignore_carbon is True:
                     continue
 
                 yr_vect = r_atm.coord - donor_grp.centroid
                 rya_angle = im.angle(yr_vect, ya_vect)
 
-                if (self.is_within_boundary(rya_angle, "min_rya_ang_ybond_inter", ge)):
+                if (self.is_within_boundary(rya_angle,
+                                            "min_rya_ang_ybond_inter", ge)):
 
-                    # If no heavy atom is bonded to the acceptor, it means that only hydrogens may be bound to it. Then, we do not
-                    # calculate the angles because hydrogens are too dynamic, i.e., the acceptor could be ionized or not at a
-                    # specific moment in time and its hydrogens may be positioned in different ways.
+                    # If no heavy atom is bonded to the acceptor, it means that
+                    # only hydrogens may be bound to it. Then, we do not
+                    # calculate the angles because hydrogens are too dynamic,
+                    # i.e., the acceptor could be ionized or not at a specific
+                    # moment in time and its hydrogens may be positioned in
+                    # different ways.
                     if len(n_coords) == 0:
                         params = {"ya_dist_ybond_inter": ya_dist,
                                   "rya_ang_ybond_inter": rya_angle,
                                   "yan_ang_ybond_inter": -1}
 
-                        inter = InteractionType(donor_grp, acceptor_grp, "Chalcogen bond", directional=True, params=params)
+                        inter = InteractionType(donor_grp,
+                                                acceptor_grp,
+                                                "Chalcogen bond",
+                                                directional=True,
+                                                params=params)
                         interactions.append(inter)
                     else:
                         # AY vector is always the same.
                         # Obs: the donor_grp is the Chalcogen (Y).
                         ay_vect = donor_grp.centroid - acceptor_grp.centroid
 
                         lowest_yan_angle = None
                         for n_coord in n_coords:
                             an_vect = n_coord - acceptor_grp.centroid
                             yan_angle = im.angle(ay_vect, an_vect)
 
                             # Update the XAR angle with the lowest value.
-                            if lowest_yan_angle is None or yan_angle < lowest_yan_angle:
+                            if (lowest_yan_angle is None
+                                    or yan_angle < lowest_yan_angle):
                                 lowest_yan_angle = yan_angle
 
-                        # The angle will be None when any R (heavy atom) atom was found.
-                        # In this case, the criteria must always fail.
+                        # The angle will be None when any R (heavy atom)
+                        # atom was found. In this case, the criteria must
+                        # always fail.
                         if lowest_yan_angle is None:
                             lowest_yan_angle = -1
 
-                        if self.is_within_boundary(lowest_yan_angle, "min_yan_ang_ybond_inter", ge):
+                        prop_name = "min_yan_ang_ybond_inter"
+                        if self.is_within_boundary(lowest_yan_angle,
+                                                   prop_name, ge):
                             params = {"ya_dist_ybond_inter": ya_dist,
                                       "rya_ang_ybond_inter": rya_angle,
                                       "yan_ang_ybond_inter": lowest_yan_angle}
 
-                            inter = InteractionType(donor_grp, acceptor_grp, "Chalcogen bond", directional=True, params=params)
+                            inter = InteractionType(donor_grp,
+                                                    acceptor_grp,
+                                                    "Chalcogen bond",
+                                                    directional=True,
+                                                    params=params)
                             interactions.append(inter)
         return interactions
 
     @staticmethod
     def calc_chalc_bond_pi(self, params):
-        """Default method to calculate chalcogen bonds between chalcogens and aromatic rings.
+        """Default method to calculate chalcogen bonds between chalcogens and
+        aromatic rings.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
@@ -1875,561 +2267,747 @@
         donor_atm = donor_grp.atoms[0]
 
         # Interaction model: R-Y --- A, where A is the ring center
         # Defining the YA distance.
         ya_dist = im.euclidean_distance(donor_grp.centroid, ring_grp.centroid)
 
         if (self.is_within_boundary(ya_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(ya_dist, "max_yc_dist_ybond_inter", le)):
+                and self.is_within_boundary(ya_dist,
+                                            "max_yc_dist_ybond_inter", le)):
 
             ay_vect = donor_grp.centroid - ring_grp.centroid
             disp_angle = im.to_quad1(im.angle(ring_grp.normal, ay_vect))
 
-            if (self.is_within_boundary(disp_angle, "max_disp_ang_ybond_inter", le)):
+            if (self.is_within_boundary(disp_angle,
+                                        "max_disp_ang_ybond_inter", le)):
                 # Interaction model: R-Y ---- A, where A is the ring center
                 # YA vector is always the same
                 ya_vect = ring_grp.centroid - donor_grp.centroid
 
                 # Defining the angle RYA, where A is the ring center
-                r_atms = [nbi for nbi in donor_atm.neighbors_info if nbi.atomic_num != 1]
-                r_elems = sorted([nbi.atomic_num for nbi in donor_atm.neighbors_info if nbi.atomic_num != 1])
+                r_atms = [nbi for nbi in donor_atm.neighbors_info
+                          if nbi.atomic_num != 1]
+                r_elems = sorted([nbi.atomic_num
+                                  for nbi in donor_atm.neighbors_info
+                                  if nbi.atomic_num != 1])
 
-                # Isothiazoles have only one sigma-hole located on the oposite site of the N.
-                # Therefore, we should only evaluate this sigma-hole by ignoring the angle formed with the carbon.
+                # Isothiazoles have only one sigma-hole located on the oposite
+                # site of the N. Therefore, we should only evaluate this
+                # sigma-hole by ignoring the angle formed with the carbon.
                 # Beno et al (2015). DOI: https://doi.org/10.1021/jm501853m.
                 ignore_carbon = False
                 if len(r_elems) == 2 and r_elems[0] == 6 and r_elems[1] == 7:
                     ignore_carbon = True
 
                 for r_atm in r_atms:
-                    # Isothiazoles have only one sigma-hole located on the oposite site of the N.
-                    # So, we must ignore the Carbon. Beno et al (2015). DOI: https://doi.org/10.1021/jm501853m.
+                    # Isothiazoles have only one sigma-hole located on the
+                    # oposite site of the N. So, we must ignore the Carbon.
+                    # Beno et al (2015).
+                    #   DOI: https://doi.org/10.1021/jm501853m.
                     if r_atm.atomic_num == 6 and ignore_carbon is True:
                         continue
 
                     yr_vect = r_atm.coord - donor_grp.centroid
                     rya_angle = im.angle(yr_vect, ya_vect)
 
-                    if (self.is_within_boundary(rya_angle, "min_rya_ang_ybond_inter", ge)):
+                    if self.is_within_boundary(rya_angle,
+                                               "min_rya_ang_ybond_inter",
+                                               ge):
                         params = {"yc_dist_ybond_inter": ya_dist,
                                   "disp_ang_ybond_inter": disp_angle,
                                   "rya_ang_ybond_inter": rya_angle}
 
-                        inter = InteractionType(donor_grp, ring_grp, "Chalcogen-pi", directional=True, params=params)
+                        inter = InteractionType(donor_grp,
+                                                ring_grp,
+                                                "Chalcogen-pi",
+                                                directional=True,
+                                                params=params)
                         interactions.append(inter)
+
         return interactions
 
     @staticmethod
     def calc_hbond(self, params):
         """Default method to calculate hydrogen bonds.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f`
+            and :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
 
         group1, group2, feat1, feat2 = params
         interactions = []
 
         if len(group1.atoms) != 1 or len(group2.atoms) != 1:
-            logger.warning("One or more invalid atom groups were informed: %s and %s. In hydrogen bonds, donor and acceptor "
-                           "groups should always contain only one atom." % (group1, group2))
+            logger.warning("One or more invalid atom groups were informed: "
+                           "%s and %s. In hydrogen bonds, donor and acceptor "
+                           "groups should always contain only one atom."
+                           % (group1, group2))
             return []
 
         if (feat1.name == "Acceptor" and feat2.name == "Donor"):
             donor_grp = group2
             acceptor_grp = group1
         else:
             donor_grp = group1
             acceptor_grp = group2
 
         donor_atm = donor_grp.atoms[0]
         acceptor_atm = acceptor_grp.atoms[0]
 
         # Interaction model: D-H ---- A-R.
         # DA distance
-        da_dist = im.euclidean_distance(donor_grp.centroid, acceptor_grp.centroid)
+        da_dist = im.euclidean_distance(donor_grp.centroid,
+                                        acceptor_grp.centroid)
 
         if (self.is_within_boundary(da_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(da_dist, "max_da_dist_hb_inter", le)):
+                and self.is_within_boundary(da_dist,
+                                            "max_da_dist_hb_inter", le)):
 
             # Interaction model: D-H ---- A-R.
             # Recover only hydrogen coordinates bonded to the donor.
-            hydrog_coords = [nbi.coord for nbi in donor_atm.neighbors_info if nbi.atomic_num == 1]
+            hydrog_coords = [nbi.coord
+                             for nbi in donor_atm.neighbors_info
+                             if nbi.atomic_num == 1]
 
             # Interaction model: D-H ---- A-R.
             # R coordinates, in which R is a heavy atom.
-            r_coords = [nbi.coord for nbi in acceptor_atm.neighbors_info if nbi.atomic_num != 1]
+            r_coords = [nbi.coord for nbi in acceptor_atm.neighbors_info
+                        if nbi.atomic_num != 1]
 
-            # Firstly, it checks if it is not necessary to apply a strict hbond rule, i.e.,
-            # hydrogens must exist and all geometrical criteria should be evaluated.
-            # Then it checks if no hydrogen is bonded to the donor, or if the donor has hydrogens
-            # and only hydrogens as neighbours (water, solvents, ammonia, SH2). In the latter case, the
-            # hydrogens can be positioned in many different ways, and each run of a tool like OpenBabel
-            # would vary the hydrogen bond list when one applies this algorithm.
+            # Firstly, it checks if it is not necessary to apply a strict
+            # hbond rule, i.e., hydrogens must exist and all geometrical
+            # criteria should be evaluated. Then it checks if no hydrogen is
+            # bonded to the donor, or if the donor has hydrogens and only
+            # hydrogens as neighbours (water, solvents, ammonia, SH2).
+            # In the latter case, the hydrogens can be positioned in many
+            # different ways, and each run of a tool like OpenBabel would vary
+            # the hydrogen bond list when one applies this algorithm.
             #
-            # If the user has also defined a list of lazy compounds, we can skip the application of strict rules on
-            # them as well. By default, the list contains only Water molecules.
+            # If the user has also defined a list of lazy compounds, we can
+            # skip the application of strict rules on them as well.
+            # By default, the list contains only Water molecules.
             if ((self.strict_donor_rules is False and (len(hydrog_coords) == 0
                                                        or len(hydrog_coords) == len(donor_atm.neighbors_info)))
                     or (donor_atm.parent.resname in self.lazy_comps_list)):
 
-                # When the position of the hydrogen cannot be defined, it assumes the hydrogen to be located 1A
-                # away from the donor in a line formed by the donor and the acceptor.
+                # When the position of the hydrogen cannot be defined, it
+                # assumes the hydrogen to be located 1A away from the donor
+                # in a line formed by the donor and the acceptor.
                 ha_dist = da_dist - 1
-                if self.is_within_boundary(ha_dist, "max_ha_dist_hb_inter", le):
+                if self.is_within_boundary(ha_dist, "max_ha_dist_hb_inter",
+                                           le):
 
-                    # If no heavy atom is bonded to the acceptor, it means that only hydrogens may be bound to it. Then, we do not
-                    # calculate the angles because hydrogens are too dynamic, i.e., the acceptor could be ionized or not at a
-                    # specific moment in time and its hydrogens may be positioned in different ways.
+                    # If no heavy atom is bonded to the acceptor, it means that
+                    # only hydrogens may be bound to it. Then, we do not
+                    # calculate the angles because hydrogens are too dynamic,
+                    # i.e., the acceptor could be ionized or not at a specific
+                    # moment in time and its hydrogens may be positioned in
+                    # different ways.
                     if len(r_coords) == 0:
                         params = {"da_dist_hb_inter": da_dist,
                                   "ha_dist_hb_inter": -1,
                                   "dha_ang_hb_inter": -1,
                                   "har_ang_hb_inter": -1,
                                   "dar_ang_hb_inter": -1}
 
-                        inter = InteractionType(donor_grp, acceptor_grp, "Hydrogen bond", directional=True, params=params)
+                        inter = InteractionType(donor_grp,
+                                                acceptor_grp,
+                                                "Hydrogen bond",
+                                                directional=True,
+                                                params=params)
                         interactions.append(inter)
                     else:
                         # AD vector is always the same.
                         ad_vect = donor_grp.centroid - acceptor_grp.centroid
 
                         lowest_dar_angle = None
                         for r_coord in r_coords:
                             ar_vect = r_coord - acceptor_grp.centroid
                             dar_angle = im.angle(ad_vect, ar_vect)
 
                             # Update the DAR angle with the lowest value.
-                            if lowest_dar_angle is None or dar_angle < lowest_dar_angle:
+                            if (lowest_dar_angle is None
+                                    or dar_angle < lowest_dar_angle):
                                 lowest_dar_angle = dar_angle
 
-                        # The angle will be None when any R (heavy atom) atom was found.
-                        # In this case, the criteria must always fail.
+                        # The angle will be None when any R (heavy atom) atom
+                        # was found. In this case, the criteria must always
+                        # fail.
                         if lowest_dar_angle is None:
                             lowest_dar_angle = -1
 
-                        if self.is_within_boundary(lowest_dar_angle, "min_dar_ang_hb_inter", ge):
+                        if self.is_within_boundary(lowest_dar_angle,
+                                                   "min_dar_ang_hb_inter",
+                                                   ge):
                             params = {"da_dist_hb_inter": da_dist,
                                       "ha_dist_hb_inter": -1,
                                       "dha_ang_hb_inter": -1,
                                       "har_ang_hb_inter": -1,
                                       "dar_ang_hb_inter": lowest_dar_angle}
 
-                            inter = InteractionType(donor_grp, acceptor_grp, "Hydrogen bond", directional=True, params=params)
+                            inter = InteractionType(donor_grp,
+                                                    acceptor_grp,
+                                                    "Hydrogen bond",
+                                                    directional=True,
+                                                    params=params)
                             interactions.append(inter)
             else:
-                # It may happen that D is covalently bound to more than one hydrogen atom.
-                # In this case, it is necessary to check the distances and angles for each atom.
-                # It will produce a hydrogen bond for each valid hydrogen.
+                # It may happen that D is covalently bound to more than one
+                # hydrogen atom. In this case, it is necessary to check the
+                # distances and angles for each atom. It will produce a
+                # hydrogen bond for each valid hydrogen.
                 for h_coord in hydrog_coords:
-                    ha_dist = im.euclidean_distance(h_coord, acceptor_grp.centroid)
+                    ha_dist = \
+                        im.euclidean_distance(h_coord, acceptor_grp.centroid)
 
                     hd_vect = donor_grp.centroid - h_coord
                     ha_vect = acceptor_grp.centroid - h_coord
                     dha_angle = im.angle(hd_vect, ha_vect)
 
-                    if (self.is_within_boundary(ha_dist, "max_ha_dist_hb_inter", le)
-                            and self.is_within_boundary(dha_angle, "min_dha_ang_hb_inter", ge)):
-
-                        # If no heavy atom is bonded to the acceptor, it means that only hydrogens may be bound to it. Then, we do not
-                        # calculate the angles because hydrogens are too dynamic, i.e., the acceptor could be ionized or not at a
-                        # specific moment in time and its hydrogens may be positioned in different ways.
+                    if (self.is_within_boundary(ha_dist,
+                                                "max_ha_dist_hb_inter", le)
+                            and self.is_within_boundary(dha_angle,
+                                                        "min_dha_ang_hb_inter",
+                                                        ge)):
+
+                        # If no heavy atom is bonded to the acceptor, it means
+                        # that only hydrogens may be bound to it. Then, we do
+                        # not calculate the angles because hydrogens are too
+                        # dynamic, i.e., the acceptor could be ionized or not
+                        # at a specific moment in time and its hydrogens may be
+                        # positioned in different ways.
                         if len(r_coords) == 0:
                             params = {"da_dist_hb_inter": da_dist,
                                       "ha_dist_hb_inter": ha_dist,
                                       "dha_ang_hb_inter": dha_angle,
                                       "har_ang_hb_inter": -1,
                                       "dar_ang_hb_inter": -1}
 
-                            inter = InteractionType(donor_grp, acceptor_grp, "Hydrogen bond", directional=True, params=params)
+                            inter = InteractionType(donor_grp,
+                                                    acceptor_grp,
+                                                    "Hydrogen bond",
+                                                    directional=True,
+                                                    params=params)
                             interactions.append(inter)
                         else:
                             # Interaction model: D-H ---- A-R
                             # AH vector is always the same.
                             ah_vect = h_coord - acceptor_grp.centroid
                             # AD vector is always the same.
-                            ad_vect = donor_grp.centroid - acceptor_grp.centroid
+                            ad_vect = \
+                                donor_grp.centroid - acceptor_grp.centroid
 
                             # Interaction model: D-H ---- A-R
-                            # Check the angles formed at the acceptor. When A is covalently bonded to more than one R atom,
-                            # it is necessary to evaluate all possible angles D-A-R and H-A-R. In this case, all angles should
-                            # satisfy the angle criterion. To do so, we could analyze only the lowest D-A-R and H-A-R angles.
-                            # It guarantees that all angles will satisfy the criteria. OBS: it may happen that each one of the
+                            # Check the angles formed at the acceptor. When
+                            # A is covalently bonded to more than one R atom,
+                            # it is necessary to evaluate all possible angles
+                            # D-A-R and H-A-R. In this case, all angles should
+                            # satisfy the angle criterion. To do so, we could
+                            # analyze only the lowest D-A-R and H-A-R angles.
+                            # It guarantees that all angles will satisfy the
+                            # criteria. OBS: it may happen that each one of the
                             # angles would belong to a different R atom.
                             lowest_har_angle = None
                             lowest_dar_angle = None
                             for r_coord in r_coords:
                                 ar_vect = r_coord - acceptor_grp.centroid
                                 har_angle = im.angle(ah_vect, ar_vect)
                                 dar_angle = im.angle(ad_vect, ar_vect)
 
                                 # Update the HAR angle with the lowest value.
-                                if lowest_har_angle is None or har_angle < lowest_har_angle:
+                                if (lowest_har_angle is None
+                                        or har_angle < lowest_har_angle):
                                     lowest_har_angle = har_angle
                                 # Update the DAR angle with the lowest value.
-                                if lowest_dar_angle is None or dar_angle < lowest_dar_angle:
+                                if (lowest_dar_angle is None
+                                        or dar_angle < lowest_dar_angle):
                                     lowest_dar_angle = dar_angle
 
-                            # The angles will be None when any R (heavy atom) atom was found.
-                            # In this case, the criteria must always fail.
-                            if lowest_har_angle is None or lowest_dar_angle is None:
+                            # The angles will be None when any R (heavy atom)
+                            # atom was found. In this case, the criteria must
+                            # always fail.
+                            if (lowest_har_angle is None
+                                    or lowest_dar_angle is None):
                                 lowest_har_angle = -1
                                 lowest_dar_angle = -1
 
-                            if (self.is_within_boundary(lowest_har_angle, "min_har_ang_hb_inter", ge)
-                                    and self.is_within_boundary(lowest_dar_angle, "min_dar_ang_hb_inter", ge)):
+                            prop_name1 = "min_har_ang_hb_inter"
+                            prop_name2 = "min_dar_ang_hb_inter"
+                            if (self.is_within_boundary(lowest_har_angle,
+                                                        prop_name1, ge)
+                                    and self.is_within_boundary(lowest_dar_angle,
+                                                                prop_name2, ge)):
 
-                                # Only the lowest D-A-R and H-A-R angles are provided.
+                                # Only the lowest D-A-R and H-A-R angles
+                                # are provided.
                                 params = {"da_dist_hb_inter": da_dist,
                                           "ha_dist_hb_inter": ha_dist,
                                           "dha_ang_hb_inter": dha_angle,
                                           "har_ang_hb_inter": lowest_har_angle,
                                           "dar_ang_hb_inter": lowest_dar_angle}
 
-                                inter = InteractionType(donor_grp, acceptor_grp, "Hydrogen bond", directional=True, params=params)
+                                inter = InteractionType(donor_grp,
+                                                        acceptor_grp,
+                                                        "Hydrogen bond",
+                                                        directional=True,
+                                                        params=params)
                                 interactions.append(inter)
 
         return interactions
 
     @staticmethod
     def calc_weak_hbond(self, params):
         """Default method to calculate weak hydrogen bonds.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
 
         group1, group2, feat1, feat2 = params
         interactions = []
 
         if len(group1.atoms) != 1 or len(group2.atoms) != 1:
-            logger.warning("One or more invalid atom groups were informed: %s and %s. In weak hydrogen bonds, weak donor and "
-                           "(weak) acceptor groups should always contain only one atom." % (group1, group2))
+            logger.warning("One or more invalid atom groups were informed: "
+                           "%s and %s. In weak hydrogen bonds, weak donor and "
+                           "(weak) acceptor groups should always contain only "
+                           "one atom." % (group1, group2))
             return []
 
-        if (feat1.name == "Acceptor" or feat1.name == "WeakAcceptor") and feat2.name == "WeakDonor":
+        if ((feat1.name == "Acceptor" or feat1.name == "WeakAcceptor")
+                and feat2.name == "WeakDonor"):
             donor_grp = group2
             acceptor_grp = group1
-        elif feat1.name == "WeakDonor" and (feat2.name == "Acceptor" or feat2.name == "WeakAcceptor"):
+        elif (feat1.name == "WeakDonor" and (feat2.name == "Acceptor"
+                                             or feat2.name == "WeakAcceptor")):
             donor_grp = group1
             acceptor_grp = group2
+
         else:
-            logger.warning("Weak hydrogen bond requires a weak donor and an (weak) acceptor groups. "
-                           "However, the informed groups have the features %s and %s." % (group1.feature_names, group2.feature_names))
+            logger.warning("Weak hydrogen bond requires a weak donor and an "
+                           "(weak) acceptor groups. However, the informed "
+                           "groups have the features %s and %s."
+                           % (group1.feature_names, group2.feature_names))
             return []
 
         donor_atm = donor_grp.atoms[0]
         acceptor_atm = acceptor_grp.atoms[0]
 
-        da_dist = im.euclidean_distance(donor_grp.centroid, acceptor_grp.centroid)
+        da_dist = im.euclidean_distance(donor_grp.centroid,
+                                        acceptor_grp.centroid)
         if (self.is_within_boundary(da_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(da_dist, "max_da_dist_whb_inter", le)):
+                and self.is_within_boundary(da_dist,
+                                            "max_da_dist_whb_inter", le)):
 
             # Interaction model: D-H ---- A-R.
             # Recover only hydrogen coordinates bonded to the donor.
-            hydrog_coords = [nbi.coord for nbi in donor_atm.neighbors_info if nbi.atomic_num == 1]
+            hydrog_coords = [nbi.coord
+                             for nbi in donor_atm.neighbors_info
+                             if nbi.atomic_num == 1]
 
             # Interaction model: D-H ---- A-R.
             # R coordinates, in which R is a heavy atom.
-            r_coords = [nbi.coord for nbi in acceptor_atm.neighbors_info if nbi.atomic_num != 1]
-
-            # Firstly, it checks if it is not necessary to apply a strict rule, i.e.,
-            # hydrogens must exist and all geometrical criteria should be evaluated.
-            # Then it checks if no hydrogen is bonded to the donor, or if the donor has hydrogens
-            # and only hydrogens as neighbours.
+            r_coords = [nbi.coord
+                        for nbi in acceptor_atm.neighbors_info
+                        if nbi.atomic_num != 1]
+
+            # Firstly, it checks if it is not necessary to apply a strict rule,
+            # i.e., hydrogens must exist and all geometrical criteria should be
+            # evaluated. Then it checks if no hydrogen is bonded to the donor,
+            # or if the donor has hydrogens and only hydrogens as neighbours.
             #
-            # If the user has also defined a list of lazy compounds, we can skip the application of strict rules on
-            # them as well. By default, the list contains only water, ammonia, and ammonium ion.
+            # If the user has also defined a list of lazy compounds, we can
+            # skip the application of strict rules on them as well. By default,
+            # the list contains only water, ammonia, and ammonium ion.
             if ((self.strict_weak_donor_rules is False and (len(hydrog_coords) == 0
                                                             or len(hydrog_coords) == len(donor_atm.neighbors_info)))
                     or (donor_atm.parent.resname in self.lazy_comps_list)):
 
-                # When the position of the hydrogen cannot be defined, it assumes the hydrogen to be located 1A
-                # away from the donor in a line formed by the donor and the acceptor.
+                # When the position of the hydrogen cannot be defined,
+                # it assumes the hydrogen to be located 1A away from the donor
+                # in a line formed by the donor and the acceptor.
                 ha_dist = da_dist - 1
-                if self.is_within_boundary(ha_dist, "max_ha_dist_whb_inter", le):
+                if self.is_within_boundary(ha_dist,
+                                           "max_ha_dist_whb_inter", le):
 
-                    # If no heavy atom is bonded to the acceptor, it means that only hydrogens may be bound to it. Then, we do not
-                    # calculate the angles because hydrogens are too dynamic, i.e., the acceptor could be ionized or not at a
-                    # specific moment in time and its hydrogens may be positioned in different ways.
+                    # If no heavy atom is bonded to the acceptor, it means that
+                    # only hydrogens may be bound to it. Then, we do not
+                    # calculate the angles because hydrogens are too dynamic,
+                    # i.e., the acceptor could be ionized or not at a specific
+                    # moment in time and its hydrogens may be positioned in
+                    # different ways.
                     if len(r_coords) == 0:
                         params = {"da_dist_whb_inter": da_dist,
                                   "ha_dist_whb_inter": -1,
                                   "dha_ang_whb_inter": -1,
                                   "har_ang_whb_inter": -1,
                                   "dar_ang_whb_inter": -1}
 
-                        inter = InteractionType(donor_grp, acceptor_grp, "Weak hydrogen bond", directional=True, params=params)
+                        inter = InteractionType(donor_grp,
+                                                acceptor_grp,
+                                                "Weak hydrogen bond",
+                                                directional=True,
+                                                params=params)
                         interactions.append(inter)
                     else:
                         # AD vector is always the same.
                         ad_vect = donor_grp.centroid - acceptor_grp.centroid
 
                         lowest_dar_angle = None
                         for r_coord in r_coords:
                             ar_vect = r_coord - acceptor_grp.centroid
                             dar_angle = im.angle(ad_vect, ar_vect)
 
                             # Update the DAR angle with the lowest value.
-                            if lowest_dar_angle is None or dar_angle < lowest_dar_angle:
+                            if (lowest_dar_angle is None
+                                    or dar_angle < lowest_dar_angle):
                                 lowest_dar_angle = dar_angle
 
-                        # The angle will be None when any R (heavy atom) atom was found.
-                        # In this case, the criteria must always fail.
+                        # The angle will be None when any R (heavy atom) atom
+                        # was found. In this case, the criteria must always
+                        # fail.
                         if lowest_dar_angle is None:
                             lowest_dar_angle = -1
 
-                        if self.is_within_boundary(lowest_dar_angle, "min_dar_ang_whb_inter", ge):
+                        if self.is_within_boundary(lowest_dar_angle,
+                                                   "min_dar_ang_whb_inter",
+                                                   ge):
                             params = {"da_dist_whb_inter": da_dist,
                                       "ha_dist_whb_inter": -1,
                                       "dha_ang_whb_inter": -1,
                                       "har_ang_whb_inter": -1,
                                       "dar_ang_whb_inter": lowest_dar_angle}
 
-                            inter = InteractionType(donor_grp, acceptor_grp, "Weak hydrogen bond", directional=True, params=params)
+                            inter = InteractionType(donor_grp,
+                                                    acceptor_grp,
+                                                    "Weak hydrogen bond",
+                                                    directional=True,
+                                                    params=params)
                             interactions.append(inter)
             else:
-                # It may happen that D is covalently bound to more than one hydrogen atom.
-                # In such cases, it's necessary to check the distances and angles for each atom.
+                # It may happen that D is covalently bound to more than one
+                # hydrogen atom. In such cases, it's necessary to check the
+                # distances and angles for each atom.
                 for h_coord in hydrog_coords:
-                    ha_dist = im.euclidean_distance(h_coord, acceptor_grp.centroid)
+                    ha_dist = im.euclidean_distance(h_coord,
+                                                    acceptor_grp.centroid)
 
                     hd_vect = donor_grp.centroid - h_coord
                     ha_vect = acceptor_grp.centroid - h_coord
                     dha_angle = im.angle(hd_vect, ha_vect)
 
-                    if (self.is_within_boundary(ha_dist, "max_ha_dist_whb_inter", le)
-                            and self.is_within_boundary(dha_angle, "min_dha_ang_whb_inter", ge)):
-
-                        # If no heavy atom is bonded to the acceptor, it means that only hydrogens may be bound to it. Then, we do not
-                        # calculate the angles because hydrogens are too dynamic, i.e., the acceptor could be ionized or not at a
-                        # specific moment in time and its hydrogens may be positioned in different ways.
+                    prop_name1 = "max_ha_dist_whb_inter"
+                    prop_name2 = "min_dha_ang_whb_inter"
+                    if (self.is_within_boundary(ha_dist, prop_name1, le)
+                            and self.is_within_boundary(dha_angle,
+                                                        prop_name2, ge)):
+
+                        # If no heavy atom is bonded to the acceptor, it means
+                        # that only hydrogens may be bound to it. Then, we do
+                        # not calculate the angles because hydrogens are too
+                        # dynamic, i.e., the acceptor could be ionized or not
+                        # at a specific moment in time and its hydrogens may
+                        # be positioned in different ways.
                         if len(r_coords) == 0:
                             params = {"da_dist_whb_inter": da_dist,
                                       "ha_dist_whb_inter": ha_dist,
                                       "dha_ang_whb_inter": dha_angle,
                                       "har_ang_whb_inter": -1,
                                       "dar_ang_whb_inter": -1}
 
-                            inter = InteractionType(donor_grp, acceptor_grp, "Weak hydrogen bond", directional=True, params=params)
+                            inter = InteractionType(donor_grp,
+                                                    acceptor_grp,
+                                                    "Weak hydrogen bond",
+                                                    directional=True,
+                                                    params=params)
                             interactions.append(inter)
                         else:
                             # Interaction model: D-H ---- A-R
                             # AH vector is always the same.
                             ah_vect = h_coord - acceptor_grp.centroid
                             # AD vector is always the same.
-                            ad_vect = donor_grp.centroid - acceptor_grp.centroid
+                            ad_vect = (donor_grp.centroid
+                                       - acceptor_grp.centroid)
 
                             # Interaction model: D-H ---- A-R
                             # Check the angles formed at the acceptor.
-                            # When A is covalently bonded to more than one R atom, it is necessary to
-                            # evaluate all possible angles D-A-R and H-A-R. In this case, all angles should
-                            # satisfy the angle criterion. To do so, we could analyze only the lowest D-A-R and
-                            # H-A-R angles. It guarantees that all angles will satisfy the criteria.
-                            # OBS: it may happen that each one of the angles would belong to a different R atom.
+                            # When A is covalently bonded to more than one R
+                            # atom, it is necessary to evaluate all possible
+                            # angles D-A-R and H-A-R. In this case, all angles
+                            # should satisfy the angle criterion. To do so, we
+                            # could analyze only the lowest D-A-R and H-A-R
+                            # angles. It guarantees that all angles will
+                            # satisfy the criteria.
+                            #
+                            # OBS: it may happen that each one of the angles
+                            # would belong to a different R atom.
                             lowest_har_angle = None
                             lowest_dar_angle = None
                             for r_coord in r_coords:
                                 ar_vect = r_coord - acceptor_grp.centroid
                                 har_angle = im.angle(ah_vect, ar_vect)
                                 dar_angle = im.angle(ad_vect, ar_vect)
 
                                 # Update the HAR angle with the lowest value.
-                                if lowest_har_angle is None or har_angle < lowest_har_angle:
+                                if (lowest_har_angle is None
+                                        or har_angle < lowest_har_angle):
                                     lowest_har_angle = har_angle
                                 # Update the DAR angle with the lowest value.
-                                if lowest_dar_angle is None or dar_angle < lowest_dar_angle:
+                                if (lowest_dar_angle is None
+                                        or dar_angle < lowest_dar_angle):
                                     lowest_dar_angle = dar_angle
 
-                            # The angles will be None when any R (heavy atom) atom was found.
-                            # In this case, the criteria must always fail.
-                            if lowest_har_angle is None or lowest_dar_angle is None:
+                            # The angles will be None when any R (heavy atom)
+                            # atom was found. In this case, the criteria must
+                            # always fail.
+                            if (lowest_har_angle is None
+                                    or lowest_dar_angle is None):
                                 lowest_har_angle = -1
                                 lowest_dar_angle = -1
 
-                            if (self.is_within_boundary(lowest_har_angle, "min_har_ang_whb_inter", ge)
-                                    and self.is_within_boundary(lowest_dar_angle, "min_dar_ang_whb_inter", ge)):
+                            prop_name1 = "min_har_ang_whb_inter"
+                            prop_name2 = "min_dar_ang_whb_inter"
+                            if (self.is_within_boundary(lowest_har_angle,
+                                                        prop_name1, ge)
+                                    and self.is_within_boundary(lowest_dar_angle,
+                                                                prop_name2, ge)):
 
-                                # Only the lowest D-A-R and H-A-R angles are provided.
+                                # Only the lowest D-A-R and H-A-R angles are
+                                # provided.
                                 params = {"da_dist_whb_inter": da_dist,
                                           "ha_dist_whb_inter": ha_dist,
                                           "dha_ang_whb_inter": dha_angle,
                                           "har_ang_whb_inter": lowest_har_angle,
                                           "dar_ang_whb_inter": lowest_dar_angle}
 
-                                inter = InteractionType(donor_grp, acceptor_grp, "Weak hydrogen bond", directional=True, params=params)
+                                inter = InteractionType(donor_grp,
+                                                        acceptor_grp,
+                                                        "Weak hydrogen bond",
+                                                        directional=True,
+                                                        params=params)
                                 interactions.append(inter)
 
         return interactions
 
     @staticmethod
     def calc_hbond_pi(self, params):
-        """Default method to calculate hydrogen bonds between (weak) donors and aromatic rings.
+        """Default method to calculate hydrogen bonds between (weak) donors
+        and aromatic rings.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
 
         group1, group2, feat1, feat2 = params
         interactions = []
 
-        if (feat1.name == "Aromatic" and (feat2.name == "Donor" or feat2.name == "WeakDonor")):
+        if (feat1.name == "Aromatic"
+                and (feat2.name == "Donor" or feat2.name == "WeakDonor")):
             ring_grp = group1
             donor_grp = group2
-        elif (feat2.name == "Aromatic" and (feat1.name == "Donor" or feat1.name == "WeakDonor")):
+        elif (feat2.name == "Aromatic"
+                and (feat1.name == "Donor" or feat1.name == "WeakDonor")):
             ring_grp = group2
             donor_grp = group1
+
         else:
-            logger.warning("Hydrogen bond involving pi-systems requires an aromatic and donor (weak donor) groups. However, "
-                           "the informed groups have the features %s and %s." % (group1.feature_names, group2.feature_names))
+            logger.warning("Hydrogen bond involving pi-systems requires an "
+                           "aromatic and donor (weak donor) groups. However, "
+                           "the informed groups have the features %s and %s."
+                           % (group1.feature_names, group2.feature_names))
             return []
 
         if len(donor_grp.atoms) != 1:
-            logger.warning("Invalid (weak) donor group was informed: %s. In hydrogen bonds involving pi-systems, (weak) donor "
-                           "groups should always contain only one atom." % donor_grp)
+            logger.warning("Invalid (weak) donor group was informed: %s. "
+                           "In hydrogen bonds involving pi-systems, (weak) "
+                           "donor groups should always contain only one "
+                           "atom." % donor_grp)
             return []
 
         # There are always just one donor/acceptor atom.
         donor_atm = donor_grp.atoms[0]
 
         # Interaction model: D-H ---- A, in which A is the ring center.
         da_dist = im.euclidean_distance(donor_grp.centroid, ring_grp.centroid)
         if (self.is_within_boundary(da_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(da_dist, "max_dc_dist_whb_inter", le)):
+                and self.is_within_boundary(da_dist,
+                                            "max_dc_dist_whb_inter", le)):
 
             # Interaction model: D-H ---- A, in which A is the ring center.
             # Recover only hydrogen coordinates bonded to the donor.
-            hydrog_coords = [nbi.coord for nbi in donor_atm.neighbors_info if nbi.atomic_num == 1]
-
-            # Firstly, it checks if it is not necessary to apply a strict hbond rule, i.e.,
-            # hydrogens must exist and all geometrical criteria should be evaluated.
-            # Then it checks if no hydrogen is bonded to the donor, or if the donor has hydrogens
-            # and only hydrogens as neighbours (water, solvents, ammonia, SH2). In the latter case, the
-            # hydrogens can be positioned in many different set of ways, and each run of a tool like
-            # OpenBabel would vary the hydrogen bond list when one applies this algorithm.
+            hydrog_coords = [nbi.coord
+                             for nbi in donor_atm.neighbors_info
+                             if nbi.atomic_num == 1]
+
+            # Firstly, it checks if it is not necessary to apply a strict
+            # hbond rule, i.e., hydrogens must exist and all geometrical
+            # criteria should be evaluated. Then it checks if no hydrogen
+            # is bonded to the donor, or if the donor has hydrogens and
+            # only hydrogens as neighbours (water, solvents, ammonia, SH2).
+            # In the latter case, the hydrogens can be positioned in many
+            # different set of ways, and each run of a tool like OpenBabel
+            # would vary the hydrogen bond list when one applies this
+            # algorithm.
             #
-            # If the user has also defined a list of lazy compounds, we can skip the application of strict rules on
-            # them as well. By default, the list contains only water, ammonia, and ammonium ion.
-            if ((self.strict_weak_donor_rules is False and (len(hydrog_coords) == 0
-                                                            or len(hydrog_coords) == len(donor_atm.neighbors_info)))
+            # If the user has also defined a list of lazy compounds, we can
+            # skip the application of strict rules on them as well.
+            # By default, the list contains only water, ammonia, and
+            # ammonium ion.
+            if ((self.strict_weak_donor_rules is False
+                    and (len(hydrog_coords) == 0
+                         or len(hydrog_coords) == len(donor_atm.neighbors_info)))
                     or (donor_atm.parent.resname in self.lazy_comps_list)):
 
-                # When the position of the hydrogen cannot be defined, it assumes the hydrogen to be located 1A
-                # away from the donor in a line formed by the donor and the acceptor.
+                # When the position of the hydrogen cannot be defined, it
+                # assumes the hydrogen to be located 1A away from the donor
+                # in a line formed by the donor and the acceptor.
                 ha_dist = da_dist - 1
-                if self.is_within_boundary(ha_dist, "max_hc_dist_whb_inter", le):
+                if self.is_within_boundary(ha_dist,
+                                           "max_hc_dist_whb_inter", le):
 
-                    # Interaction model: D-H ---- A, in which A is the ring center.
-                    # Calculate the displacement angle formed between the ring normal and the vector Donor-Centroid.
+                    # Interaction model: D-H ---- A, in which A is the ring
+                    # center. Calculate the displacement angle formed between
+                    # the ring normal and the vector Donor-Centroid.
                     ad_vect = donor_grp.centroid - ring_grp.centroid
-                    disp_angle = im.to_quad1(im.angle(ring_grp.normal, ad_vect))
+                    disp_angle = im.to_quad1(im.angle(ring_grp.normal,
+                                                      ad_vect))
 
-                    if (self.is_within_boundary(disp_angle, "max_disp_ang_whb_inter", le)):
+                    if (self.is_within_boundary(disp_angle,
+                                                "max_disp_ang_whb_inter", le)):
                         params = {"dc_dist_whb_inter": da_dist,
                                   "hc_dist_whb_inter": -1,
                                   "dhc_ang_whb_inter": -1,
                                   "disp_ang_whb_inter": disp_angle}
 
-                        inter = InteractionType(donor_grp, ring_grp, "Weak hydrogen bond", directional=True, params=params)
+                        inter = InteractionType(donor_grp,
+                                                ring_grp,
+                                                "Weak hydrogen bond",
+                                                directional=True,
+                                                params=params)
                         interactions.append(inter)
             else:
-                # It may happen that D is covalently bound to more than one hydrogen atom.
-                # In this case, it is necessary to check the distances and angles for each atom.
-                # It will produce a hydrogen bond for each valid hydrogen.
+                # It may happen that D is covalently bound to more than one
+                # hydrogen atom. In this case, it is necessary to check the
+                # distances and angles for each atom. It will produce a
+                # hydrogen bond for each valid hydrogen.
                 for h_coord in hydrog_coords:
                     ha_dist = im.euclidean_distance(h_coord, ring_grp.centroid)
 
                     hd_vect = donor_grp.centroid - h_coord
                     ha_vect = ring_grp.centroid - h_coord
                     dha_angle = im.angle(hd_vect, ha_vect)
 
-                    if (self.is_within_boundary(ha_dist, "max_hc_dist_whb_inter", le)
-                            and self.is_within_boundary(dha_angle, "min_dhc_ang_whb_inter", ge)):
-
-                        # Interaction model: D-H ---- A, in which A is the ring center.
-                        # Calculate the displacement angle formed between the ring normal and the vector Donor-Centroid.
+                    prop_name1 = "max_hc_dist_whb_inter"
+                    prop_name2 = "min_dhc_ang_whb_inter"
+                    if (self.is_within_boundary(ha_dist, prop_name1, le)
+                            and self.is_within_boundary(dha_angle,
+                                                        prop_name2, ge)):
+
+                        # Interaction model: D-H ---- A, in which A is the ring
+                        # center. Calculate the displacement angle formed
+                        # between the ring normal and the vector
+                        # Donor-Centroid.
                         ad_vect = donor_grp.centroid - ring_grp.centroid
-                        disp_angle = im.to_quad1(im.angle(ring_grp.normal, ad_vect))
+                        disp_angle = im.to_quad1(im.angle(ring_grp.normal,
+                                                          ad_vect))
 
-                        if (self.is_within_boundary(disp_angle, "max_disp_ang_whb_inter", le)):
+                        if (self.is_within_boundary(disp_angle,
+                                                    "max_disp_ang_whb_inter",
+                                                    le)):
                             params = {"dc_dist_whb_inter": da_dist,
                                       "hc_dist_whb_inter": ha_dist,
                                       "dhc_ang_whb_inter": dha_angle,
                                       "disp_ang_whb_inter": disp_angle}
 
-                            inter = InteractionType(donor_grp, ring_grp, "Weak hydrogen bond", directional=True, params=params)
+                            inter = InteractionType(donor_grp,
+                                                    ring_grp,
+                                                    "Weak hydrogen bond",
+                                                    directional=True,
+                                                    params=params)
                             interactions.append(inter)
         return interactions
 
     @staticmethod
     def calc_ionic(self, params):
         """Default method to calculate attractive ionic interactions.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
 
         group1, group2, feat1, feat2 = params
         interactions = []
 
         cc_dist = im.euclidean_distance(group1.centroid, group2.centroid)
         if (self.is_within_boundary(cc_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(cc_dist, "max_dist_attract_inter", le)):
+                and self.is_within_boundary(cc_dist,
+                                            "max_dist_attract_inter", le)):
 
             params = {"dist_attract_inter": cc_dist}
             inter = InteractionType(group1, group2, "Ionic", params=params)
 
             interactions.append(inter)
         return interactions
 
@@ -2439,31 +3017,35 @@
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_non_cov:
             return []
 
         group1, group2, feat1, feat2 = params
         interactions = []
 
         cc_dist = im.euclidean_distance(group1.centroid, group2.centroid)
         if (self.is_within_boundary(cc_dist, "bsite_cutoff", le)
-                and self.is_within_boundary(cc_dist, "max_dist_repuls_inter", le)):
+                and self.is_within_boundary(cc_dist,
+                                            "max_dist_repuls_inter", le)):
 
             params = {"dist_repuls_inter": cc_dist}
             inter = InteractionType(group1, group2, "Repulsive", params=params)
 
             interactions.append(inter)
         return interactions
 
@@ -2473,17 +3055,20 @@
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         if not self.add_proximal:
             return []
@@ -2498,134 +3083,219 @@
             params = {"dist_proximal": cc_dist}
             inter = InteractionType(group1, group2, "Proximal", params=params)
             interactions.append(inter)
 
         return interactions
 
     @staticmethod
+    def calc_metal_coord(self, params):
+        # Ignore covalent bonds.
+        if not self.add_cov:
+            return []
+
+        group1, group2, feat1, feat2 = params
+        interactions = []
+
+        if feat1.name == "Atom" and feat2.name == "Metal":
+            other_grp = group1
+            metal_grp = group2
+        elif feat1.name == "Metal" and feat2.name == "Atom":
+            other_grp = group2
+            metal_grp = group1
+        else:
+            logger.warning("Metal complexes require an "
+                           "other and a metal group. However, "
+                           "the informed groups have the features %s and %s."
+                           % (group1.feature_names, group2.feature_names))
+            return []
+
+        if other_grp.atoms[0].element not in ["O", "N", "S"]:
+            return []
+
+        # Interaction model: M ---- A.
+        # MA distance
+        ma_dist = im.euclidean_distance(metal_grp.centroid,
+                                        other_grp.centroid)
+
+        if self.is_within_boundary(ma_dist, "max_ma_dist_metal_coord", le):
+            params = {"ma_dist_metal_coord": ma_dist}
+            inter = InteractionType(other_grp,
+                                    metal_grp,
+                                    "Metal coordination",
+                                    directional=True,
+                                    params=params)
+            interactions.append(inter)
+
+        return interactions
+
+    @staticmethod
     def calc_atom_atom(self, params):
-        """Default method to calculate atom-atom interactions, which include covalent bonds, Van der Waals,
-        Van der Waals clash, and atom overlap.
+        """Default method to calculate atom-atom interactions, which include
+        covalent bonds, Van der Waals, Van der Waals clash, and atom overlap.
 
-        Note that covalent bonds are controlled by the flag ``add_cov``, while the other three interactions
-        are controlled by the flag ``add_atom_atom``.
+        Note that covalent bonds are controlled by the flag ``add_cov``, while
+        the other three interactions are controlled by the flag
+        ``add_atom_atom``.
 
         .. note::
-            We opted to separate `Van der Waals` from other non-covalent interactions because LUNA may
-            generate an unnecessary number of additional interactions that are usually already represented
-            by other non-covalent interactions as weak hydrogen bonds, hydrophobic, or dipole-dipole
-            interactions. Thus, to give users a fine-grain control over which interactions to calculate,
-            we provided this additional flag to turn off the calculation of Van der Waals interactions.
+            We opted to separate `Van der Waals` from other non-covalent
+            interactions because LUNA may generate an unnecessary number of
+            additional interactions that are usually already represented by
+            other non-covalent interactions as weak hydrogen bonds,
+            hydrophobic, or dipole-dipole interactions. Thus, to give users a
+            fine-grain control over which interactions to calculate, we
+            provided this additional flag to turn off the calculation of
+            Van der Waals interactions.
 
         Parameters
         ----------
         params : tuple of (:class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.groups.AtomGroup`,\
                            :class:`~luna.mol.features.ChemicalFeature`,\
                            :class:`~luna.mol.features.ChemicalFeature`)
-            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`, :math:`B_f`), where
-            :math:`A` and :math:`B` are two :class:`~luna.mol.groups.AtomGroup` objects, and
-            :math:`A_f` and :math:`B_f` are their features (:class:`~luna.mol.features.ChemicalFeature` objects), respectively.
+            The tuple follows the order (:math:`A`, :math:`B`, :math:`A_f`,
+            :math:`B_f`), where :math:`A` and :math:`B` are two
+            :class:`~luna.mol.groups.AtomGroup` objects, and :math:`A_f` and
+            :math:`B_f` are their features
+            (:class:`~luna.mol.features.ChemicalFeature` objects),
+            respectively.
 
         Returns
         -------
          : list
         """
         group1, group2, feat1, feat2 = params
         interactions = []
 
         atm1 = group1.atoms[0]
         atm2 = group2.atoms[0]
 
         cc_dist = im.euclidean_distance(group1.centroid, group2.centroid)
         params = {"dist_atom_atom": cc_dist}
 
-        # It checks if the two atoms are neighbors, i.e., if they are covalently bonded.
-        # The covalent bonds are detected by OpenBabel, which besides other evaluations,
-        # states that two atoms are covalently bonded if:
+        # It checks if the two atoms are neighbors, i.e., if they are
+        # covalently bonded. The covalent bonds are detected by OpenBabel,
+        # which besides other evaluations, states that two atoms are
+        # covalently bonded if:
         #       0.4 <= d(a1, a2) <= cov_rad(a1) + cov_rad(a2) + 0.45
         if atm1.is_neighbor(atm2):
             # Ignore covalent bonds.
             if not self.add_cov:
                 return []
 
             bond_type = atm1.get_neighbor_info(atm2).bond_type
 
             if bond_type in COV_BONDS_MAPPING:
                 bond_name = COV_BONDS_MAPPING[bond_type]
             else:
                 bond_name = "Other bond"
-                logger.warning("An unexpected bond (%s) was found between the atoms %s and %s. "
-                               "Therefore, a general bond name (%s) will be used instead." % (bond_type, atm1, atm2, bond_name))
+                logger.warning("An unexpected bond (%s) was found between the "
+                               "atoms %s and %s. Therefore, a general bond "
+                               "name (%s) will be used instead."
+                               % (bond_type, atm1, atm2, bond_name))
 
             inter = InteractionType(group1, group2, bond_name, params=params)
             interactions.append(inter)
         else:
             if not self.add_atom_atom:
                 return []
 
             cov1 = ob.GetCovalentRad(ob.GetAtomicNum(atm1.element))
             cov2 = ob.GetCovalentRad(ob.GetAtomicNum(atm2.element))
 
             if cc_dist <= cov1 + cov2:
-                inter = InteractionType(group1, group2, "Atom overlap", params=params)
+                inter = InteractionType(group1,
+                                        group2,
+                                        "Atom overlap",
+                                        params=params)
                 interactions.append(inter)
             else:
                 rdw1 = ob.GetVdwRad(ob.GetAtomicNum(atm1.element))
                 rdw2 = ob.GetVdwRad(ob.GetAtomicNum(atm2.element))
 
                 # r1 + r2 - d < 0 => no clash
                 # r1 + r2 - d = 0 => in the limit, i.e., spheres are touching.
                 # r1 + r2 - d > 0 => clash.
-                if (rdw1 + rdw2 - cc_dist) >= self.inter_config.get("vdw_clash_tolerance", 0):
-                    # Ignore Van der Waals and clashes for atoms separated from each other by only N bonds.
-                    # Covalent bonds keep atoms very tightly, producing distances lower than their sum of Van der Waals radius.
-                    # As a consequence the algorithm will find a lot of false clashes and Van der Waals interactions.
-                    #
-                    # It is better to keep this function inside the IFs to avoid the Dijkstra processing for pairs of atoms
-                    # that wouldn't enter inside the IF.
-                    shortest_path_length = group1.get_shortest_path_length(group2, self.inter_config.get("min_bond_separation", 0))
+                if ((rdw1 + rdw2 - cc_dist)
+                        >= self.inter_config.get("vdw_clash_tolerance", 0)):
 
-                    # If get_shortest_path_length() returns any value that is not infinite (INF), it means these two groups
-                    # contain a path with at less than or equal to the cutoff 'min_bond_separation'. Therefore, ignore them.
+                    # Ignore Van der Waals and clashes for atoms separated from
+                    # each other by only N bonds. Covalent bonds keep atoms
+                    # very tightly, producing distances lower than their sum of
+                    # Van der Waals radius. As a consequence the algorithm will
+                    # find a lot of false clashes and Van der Waals
+                    # interactions.
+                    #
+                    # It is better to keep this function inside the IFs to
+                    # avoid the Dijkstra processing for pairs of atoms that
+                    # wouldn't enter inside the IF.
+                    min_bond_sep = \
+                        self.inter_config.get("min_bond_separation", 0)
+                    shortest_path_length = \
+                        group1.get_shortest_path_length(group2, min_bond_sep)
+
+                    # If get_shortest_path_length() returns any value that is
+                    # not infinite (INF), it means these two groups contain a
+                    # path with at less than or equal to the cutoff
+                    # 'min_bond_separation'. Therefore, ignore them.
                     if shortest_path_length != float('inf'):
                         return []
 
-                    inter = InteractionType(group1, group2, "Van der Waals clash", params=params)
+                    inter = InteractionType(group1,
+                                            group2,
+                                            "Van der Waals clash",
+                                            params=params)
                     interactions.append(inter)
 
-                elif cc_dist <= rdw1 + rdw2 + self.inter_config.get("vdw_tolerance", 0):
-                    # Ignore Van der Waals and clashes for atoms separated from each other by only N bonds.
-                    # Covalent bonds keep atoms very tightly, producing distances lower than their sum of Van der Waals radius.
-                    # As a consequence the algorithm will find a lot of false clashes and Van der Waals interactions.
+                elif (cc_dist
+                        <= (rdw1 + rdw2
+                            + self.inter_config.get("vdw_tolerance", 0))):
+
+                    # Ignore Van der Waals and clashes for atoms separated from
+                    # each other by only N bonds. Covalent bonds keep atoms
+                    # very tightly, producing distances lower than their sum of
+                    # Van der Waals radius. As a consequence the algorithm will
+                    # find a lot of false clashes and Van der Waals
+                    # interactions.
                     #
-                    # It is better to keep this function inside the IFs to avoid the Dijkstra processing for pairs of atoms
-                    # that wouldn't enter inside the IF.
-                    shortest_path_length = group1.get_shortest_path_length(group2, self.inter_config.get("min_bond_separation", 0))
-
-                    # If get_shortest_path_length() returns any value that is not infinite (INF), it means these two groups
-                    # contain a path with at less than or equal to the cutoff 'min_bond_separation'. Therefore, ignore them.
+                    # It is better to keep this function inside the IFs to
+                    # avoid the Dijkstra processing for pairs of atoms that
+                    # wouldn't enter inside the IF.
+                    min_bond_sep = \
+                        self.inter_config.get("min_bond_separation", 0)
+                    shortest_path_length = \
+                        group1.get_shortest_path_length(group2, min_bond_sep)
+
+                    # If get_shortest_path_length() returns any value that is
+                    # not infinite (INF), it means these two groups contain a
+                    # path with at less than or equal to the cutoff
+                    # 'min_bond_separation'. Therefore, ignore them.
                     if shortest_path_length != float('inf'):
                         return []
 
-                    inter = InteractionType(group1, group2, "Van der Waals", params=params)
+                    inter = InteractionType(group1,
+                                            group2,
+                                            "Van der Waals",
+                                            params=params)
                     interactions.append(inter)
 
         return interactions
 
     def _is_intramol_inter(self, grp1, grp2):
         comps1 = grp1.compounds
         comps2 = grp2.compounds
         return len(comps1) == 1 and len(comps2) == 1 and comps1 == comps2
 
     def is_within_boundary(self, value, key, func):
-        """Check if a value is within the boundary defined for a given parameter.
+        """Check if a value is within the boundary defined for a given
+        parameter.
 
         .. note::
-            It will always return True if the parameter does not exist in ``inter_config``.
+            It will always return True if the parameter does not exist in
+            ``inter_config``.
 
         Parameters
         ----------
         value : any
             The value to be evaluated.
         key :
             A parameter defined in ``inter_config``.
@@ -2645,21 +3315,22 @@
         if key not in self.inter_config:
             return True
         return func(value, self.inter_config[key])
 
     def is_feature_pair_valid(self, feat1, feat2):
         """Check if the provided pair of features is valid or not.
 
-        It will be valid if the pair exists in ``funcs``, i.e., there is one or more
-        functions to calculate interactions defined for that given pair of features.
-
-        It also return False if non-covalent interactions is turned off (``add_non_cov = False``)
-        and at least one of the features is not `Atom`.
-        This is useful to save processing time as it skips pairs that have functions to
-        calculate non-covalent interactions right away.
+        It will be valid if the pair exists in ``funcs``, i.e., there is one or
+        more functions to calculate interactions defined for that given pair of
+        features.
+
+        It also return False if non-covalent interactions is turned off
+        (``add_non_cov = False``) and at least one of the features is not
+        `Atom`. This is useful to save processing time as it skips pairs that
+        have functions to calculate non-covalent interactions right away.
 
         Parameters
         ----------
         feat1, feat2: :class:`~luna.mol.features.ChemicalFeature`
 
         Returns
         -------
@@ -2699,15 +3370,17 @@
             return funcs[(feat1, feat2)]
         elif (feat2, feat1) in funcs:
             return funcs[(feat2, feat1)]
         else:
             return None
 
     def set_functions_to_pair(self, pair, funcs):
-        """Set functions to calculate interaction for the given pair of features.
+        """Set functions to calculate interaction for the given pair of
+        features.
 
         Parameters
         ----------
-        pair: tuple of (:class:`~luna.mol.features.ChemicalFeature`, :class:`~luna.mol.features.ChemicalFeature`)
+        pair: tuple of (:class:`~luna.mol.features.ChemicalFeature`, \
+                    :class:`~luna.mol.features.ChemicalFeature`)
         funcs : iterable of callable
         """
         self.funcs[pair] = funcs
```

### Comparing `luna-0.12.2/luna/interaction/config.cfg` & `luna-0.13.0/luna/interaction/config.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -230,14 +230,18 @@
 vdw_clash_tolerance = 0.6
 
 ; Ref: Chimera (https://www.cgl.ucsf.edu/chimerax/docs/user/commands/clashes.html).
 ;
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 
 
+[Metal complex]
+max_ma_dist_metal_coord = 2.8
+
+
 
 [Bond separation]
 min_bond_separation = 3
 min_bond_separation_for_clash = 4
 
 ; Ref: Chimera (https://www.cgl.ucsf.edu/chimerax/docs/user/commands/clashes.html).
 ;
```

### Comparing `luna-0.12.2/luna/interaction/config.py` & `luna-0.13.0/luna/interaction/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,25 @@
     @property
     def params(self):
         """list: The list of parameters."""
         return sorted(self.keys())
 
     @classmethod
     def from_config_file(cls, config_file):
+        """Initialize from a configuration file.
+
+        Parameters
+        ----------
+        config_file : str
+            The configuration file pathname.
+
+        Returns
+        -------
+         : `InteractionConfig`
+        """
         if not path.exists(config_file):
             raise OSError("File '%s' does not exist." % config_file)
 
         config = {}
         params = Config(config_file)
         names_map = {}
 
@@ -52,14 +63,21 @@
                            for prop in params_dict}
             names_map.update({k: section for k in params_dict})
             config.update(params_dict)
 
         return cls(config, names_map)
 
     def save_config_file(self, config_file):
+        """Save the interaction parameters into a configuration file.
+
+        Parameters
+        ----------
+        config_file : str
+            The output configuration file.
+        """
         args_by_section = defaultdict(list)
         for k, v in self.items():
             section = self.names_map.get(k, "Other")
             args_by_section[section].append((k, v))
 
         with open(config_file, "w") as OUT:
             for section in sorted(args_by_section):
```

### Comparing `luna-0.12.2/luna/interaction/contact.py` & `luna-0.13.0/luna/interaction/contact.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,164 +1,200 @@
 from itertools import product
 
-from luna.util.default_values import COV_SEARCH_RADIUS, BOUNDARY_CONFIG
+from luna.util.default_values import (COV_SEARCH_RADIUS, BOUNDARY_CONFIG)
 from luna.util.exceptions import EntityLevelError, IllegalArgumentError
-from luna.MyBio.util import ENTITY_LEVEL_NAME, is_covalently_bound
+from luna.interaction.cov import is_covalently_bound
+from luna.MyBio.util import ENTITY_LEVEL_NAME
 from luna.MyBio.PDB.NeighborSearch import NeighborSearch
 from luna.MyBio.PDB import Selection
 from luna.MyBio.PDB.Residue import Residue
 
 import logging
 
 logger = logging.getLogger()
 
 
-def get_all_contacts(entity, radius=BOUNDARY_CONFIG["bsite_cutoff"],
+def get_all_contacts(entity,
+                     radius=BOUNDARY_CONFIG["bsite_cutoff"],
                      level='A'):
     """Recover all residue-residue or atom-atom contacts in ``entity``.
 
     Parameters
     ----------
     entity : :class:`~luna.MyBio.PDB.Entity.Entity`
         The PDB object from where atoms and residues will be recovered.
     radius : float
-        The cutoff distance (in Å) for defining contacts. The default value is 6.2.
+        The cutoff distance (in Å) for defining contacts.
+        The default value is 6.2.
     level : {'R', 'A'}
         Return residues ('R') or atoms ('A') in contact with ``source``.
 
     Returns
     -------
-     : list of tuple of (:class:`~luna.MyBio.PDB.Residue.Residue` or :class:`~luna.MyBio.PDB.Atom.Atom`, \
-      :class:`~luna.MyBio.PDB.Residue.Residue` or :class:`~luna.MyBio.PDB.Atom.Atom`)
+     : list of tuple of (:class:`~luna.MyBio.PDB.Residue.Residue` or \
+                :class:`~luna.MyBio.PDB.Atom.Atom`, \
+                :class:`~luna.MyBio.PDB.Residue.Residue` or \
+                :class:`~luna.MyBio.PDB.Atom.Atom`)
         Each tuple contains either a pair of residues or atoms in contact.
 
     Raises
     ------
     EntityLevelError
         If ``level`` is neither 'R' nor 'A'.
 
     Examples
     --------
 
-    In this example, we will identify all residue-residue contacts within 2.5 Å in the PDB 3QQK.
-    So, let's first parse the PDB file.
+    In this example, we will identify all residue-residue contacts
+    within 2.5 Å in the PDB 3QQK. So, let's first parse the PDB file.
 
     >>> from luna.util.default_values import LUNA_PATH
     >>> from luna.MyBio.PDB.PDBParser import PDBParser
     >>> pdb_parser = PDBParser(PERMISSIVE=True, QUIET=True)
-    >>> structure = pdb_parser.get_structure("Protein", f"{LUNA_PATH}/tutorial/inputs/3QQK.pdb")
+    >>> structure = pdb_parser.get_structure("Protein", \
+f"{LUNA_PATH}/tutorial/inputs/3QQK.pdb")
 
-    Then, to recover all residue-residue contacts within 2.5 Å use :meth:`get_all_contacts`
-    with ``level`` set to 'R' and radius set to 2.5.
+    Then, to recover all residue-residue contacts within 2.5 Å use
+    :meth:`get_all_contacts` with ``level`` set to 'R' and radius set to 2.5.
 
     >>> from luna.interaction.contact import get_all_contacts
     >>> contacts = get_all_contacts(structure, radius=2.5, level="R")
     >>> print(len(contacts))
     314
 
     """
     try:
         if level == 'S' or level == 'M' or level == 'C':
-            raise EntityLevelError("Maximum entity level to be chosen is: R (residues) or A (atoms)")
+            raise EntityLevelError("Maximum entity level to be chosen "
+                                   "is: R (residues) or A (atoms)")
 
         if level not in ENTITY_LEVEL_NAME:
-            raise EntityLevelError("The defined level '%s' does not exist" % level)
+            raise EntityLevelError("The defined level '%s' does not exist"
+                                   % level)
 
-        logger.debug("Trying to select all contacts in the PDB file %s." % entity.get_parent_by_level('S').id)
+        logger.debug("Trying to select all contacts in the PDB file %s."
+                     % entity.get_parent_by_level('S').id)
 
         all_atoms = list(entity.get_atoms())
         ns = NeighborSearch(all_atoms)
         pairs = ns.search_all(radius, level)
 
-        logger.debug("Number of nearby %s(s) found: %d." % (ENTITY_LEVEL_NAME[level].lower(), len(pairs)))
+        logger.debug("Number of nearby %s(s) found: %d."
+                     % (ENTITY_LEVEL_NAME[level].lower(), len(pairs)))
 
         return pairs
     except Exception as e:
         logger.exception(e)
         raise
 
 
-def get_contacts_with(entity, source, target=None,
-                      radius=BOUNDARY_CONFIG["bsite_cutoff"], level='A'):
+def get_contacts_with(source,
+                      target=None,
+                      entity=None,
+                      radius=BOUNDARY_CONFIG["bsite_cutoff"],
+                      level='A'):
     """Recover atoms or residues in contact with ``source``.
 
     Parameters
     ----------
-    entity : :class:`~luna.MyBio.PDB.Entity.Entity`
-        The PDB object from where atoms and residues will be recovered.
     source : :class:`~luna.MyBio.PDB.Entity.Entity`
-        The reference, which can be any :class:`~luna.MyBio.PDB.Entity.Entity` instance (structure, model, chain, residue, or atom).
+        The reference, which can be any :class:`~luna.MyBio.PDB.Entity.Entity`
+        instance (structure, model, chain, residue, or atom).
     target : :class:`~luna.MyBio.PDB.Entity.Entity`, optional
         If provided, only contacts with the ``target`` will be considered.
+    entity : :class:`~luna.MyBio.PDB.Entity.Entity`
+        The PDB object from where atoms will be recovered.
+        If not provided (the default), the model object that contains
+        ``source`` will be used instead.
     radius : float
-        The cutoff distance (in Å) for defining contacts. The default value is 6.2.
+        The cutoff distance (in Å) for defining contacts.
+        The default value is 6.2.
     level : {'R', 'A'}
         Return residues ('R') or atoms ('A') in contact with ``source``.
 
     Returns
     -------
-     : set of tuple of (:class:`~luna.MyBio.PDB.Residue.Residue` or :class:`~luna.MyBio.PDB.Atom.Atom`, \
-    :class:`~luna.MyBio.PDB.Residue.Residue` or :class:`~luna.MyBio.PDB.Atom.Atom`)
+     : set of tuple of (:class:`~luna.MyBio.PDB.Residue.Residue` or \
+            :class:`~luna.MyBio.PDB.Atom.Atom`, \
+            :class:`~luna.MyBio.PDB.Residue.Residue` or \
+            :class:`~luna.MyBio.PDB.Atom.Atom`)
         Each tuple contains two items:\
             the first corresponds to a residue/atom from the ``source``,\
-            and the second corresponds to a residue/atom in contact with ``source``.
+            and the second corresponds to a residue/atom in contact
+            with ``source``.
 
     Raises
     ------
     EntityLevelError
         If ``level`` is neither 'R' nor 'A'.
 
     Examples
     --------
 
-    **Example 1)** In this example, we will identify residue-residue contacts between a ligand and nearby residues.
+    **Example 1)** In this example, we will identify residue-residue contacts
+    between a ligand and nearby residues.
 
     First, let's parse a PDB file to work with.
 
     >>> from luna.util.default_values import LUNA_PATH
     >>> from luna.MyBio.PDB.PDBParser import PDBParser
     >>> pdb_parser = PDBParser(PERMISSIVE=True, QUIET=True)
-    >>> structure = pdb_parser.get_structure("Protein", f"{LUNA_PATH}/tutorial/inputs/3QQK.pdb")
+    >>> structure = pdb_parser.get_structure("Protein", \
+f"{LUNA_PATH}/tutorial/inputs/3QQK.pdb")
 
     Now, we define the target ligand.
 
     >>> ligand = structure[0]["A"][('H_X02', 497, ' ')]
 
-    Then, to recover contacts between this ligand and nearby residues we use :meth:`get_contacts_with`
-    with ``level`` set to 'R'.
+    Then, to recover contacts between this ligand and nearby residues we use
+    :meth:`get_contacts_with` with ``level`` set to 'R'.
 
     >>> from luna.interaction.contact import get_contacts_with
-    >>> contacts = sorted(get_contacts_with(structure, ligand, radius=3, level="R"))
+    >>> contacts = sorted(get_contacts_with(ligand,
+    ...                                     entity=structure,
+    ...                                     radius=3,
+    ...                                     level="R"))
     >>> for pair in contacts:
     ...     print(pair)
-    (<Residue X02 het=H_X02 resseq=497 icode= >, <Residue GLU het=  resseq=81 icode= >)
-    (<Residue X02 het=H_X02 resseq=497 icode= >, <Residue LEU het=  resseq=83 icode= >)
-    (<Residue X02 het=H_X02 resseq=497 icode= >, <Residue X02 het=H_X02 resseq=497 icode= >)
-    (<Residue X02 het=H_X02 resseq=497 icode= >, <Residue HOH het=W resseq=321 icode= >)
+    (<Residue X02 het=H_X02 resseq=497 icode= >, \
+<Residue GLU het=  resseq=81 icode= >)
+    (<Residue X02 het=H_X02 resseq=497 icode= >, \
+<Residue LEU het=  resseq=83 icode= >)
+    (<Residue X02 het=H_X02 resseq=497 icode= >, \
+<Residue X02 het=H_X02 resseq=497 icode= >)
+    (<Residue X02 het=H_X02 resseq=497 icode= >, \
+<Residue HOH het=W resseq=321 icode= >)
 
 
-    **Example 2)** In this example, we will identify atom-atom contacts between a ligand and a given residue.
+    **Example 2)** In this example, we will identify atom-atom contacts
+    between a ligand and a given residue.
 
     First, let's parse a PDB file to work with.
 
     >>> from luna.util.default_values import LUNA_PATH
     >>> from luna.MyBio.PDB.PDBParser import PDBParser
     >>> pdb_parser = PDBParser(PERMISSIVE=True, QUIET=True)
-    >>> structure = pdb_parser.get_structure("Protein", f"{LUNA_PATH}/tutorial/inputs/3QQK.pdb")
+    >>> structure = pdb_parser.get_structure("Protein", \
+f"{LUNA_PATH}/tutorial/inputs/3QQK.pdb")
 
     Now, we define the target ligand and residue.
 
     >>> ligand = structure[0]["A"][('H_X02', 497, ' ')]
     >>> residue = structure[0]["A"][(' ', 81, ' ')]
 
-    Then, to recover contacts between these compounds we use :meth:`get_contacts_with`.
-    As we need atom-wise contacts, set ``level`` to 'A'.
+    Then, to recover contacts between these compounds we use
+    :meth:`get_contacts_with`. As we need atom-wise contacts, set ``level``
+    to 'A'.
 
     >>> from luna.interaction.contact import get_contacts_with
-    >>> contacts = sorted(get_contacts_with(structure, ligand, target=residue, radius=4, level="A"))
+    >>> contacts = sorted(get_contacts_with(ligand,
+    ...                   target=residue,
+    ...                   entity=structure,
+    ...                   radius=4,
+    ...                   level="A"))
     >>> for pair in contacts:
     ...     print(pair)
     (<Atom C7>, <Atom O>)
     (<Atom N10>, <Atom C>)
     (<Atom N10>, <Atom O>)
     """
     try:
@@ -166,20 +202,28 @@
             raise EntityLevelError("Maximum entity level to be chosen is: "
                                    "R (residues) or A (atoms)")
 
         if level not in ENTITY_LEVEL_NAME:
             raise EntityLevelError("The defined level '%s' does not exist"
                                    % level)
 
+        entity = entity or source.get_parent_by_level("M")
+
         source_atoms = Selection.unfold_entities([source], 'A')
+
         target_atoms = []
         if target is None:
             target_atoms = list(entity.get_atoms())
         else:
-            target_atoms = Selection.unfold_entities(target, 'A')
+            if target.level == "A":
+                target_atoms = [target]
+            else:
+                target_residues = Selection.unfold_entities(target, 'R')
+                target_atoms = [a for r in target_residues
+                                for a in r.get_unpacked_list()]
 
         ns = NeighborSearch(target_atoms)
         entities = set()
         for atom in source_atoms:
             entity = atom.get_parent_by_level(level)
             nb_entities = ns.search(atom.coord, radius, level)
             pairs = set(product([entity], nb_entities))
@@ -189,132 +233,160 @@
                      % (ENTITY_LEVEL_NAME[level].lower(), len(entities)))
         return entities
     except Exception as e:
         logger.exception(e)
         raise
 
 
-def get_cov_contacts_with(entity, source, target=None):
-    """Recover potential covalent bonds with ``source``.
-
-    Covalent bonds between two nearby atoms A and B are determined as in Open Babel:
-
-    .. math:: 0.4 <= \overrightarrow{\|AB\|} <= A_{cov} + B_{cov} + 0.45
-
-    Where :math:`\overrightarrow{\|AB\|}` is the distance between atoms A and B,
-    and :math:`A_{cov}` and :math:`B_{cov}` are the covalent radius of atoms A and B, respectively.
+def get_proximal_compounds(source, radius=COV_SEARCH_RADIUS):
+    """Recover proximal compounds to ``source``.
 
     Parameters
     ----------
-    entity : :class:`~luna.MyBio.PDB.Entity.Entity`
-        The PDB object from where atoms will be recovered.
-    source : :class:`~luna.MyBio.PDB.Entity.Entity`
-        The reference, which can be any :class:`~luna.MyBio.PDB.Entity.Entity` instance (structure, model, chain, residue, or atom).
-    target : :class:`~luna.MyBio.PDB.Entity.Entity`, optional
-        If provided, only covalent bonds with the ``target`` will be considered.
+    source : :class:`~luna.MyBio.PDB.Residue.Residue`
+        The reference compound.
+    radius : float
+        The cutoff distance (in Å) for defining proximity.
+        The default value is 2.2, which may recover potential residues bound to
+        ``source`` through covalent bonds.
 
     Returns
     -------
-     : set of tuple of (:class:`~luna.MyBio.PDB.Atom.Atom`, :class:`~luna.MyBio.PDB.Atom.Atom`)
-        Pairs of atoms with potential covalent bonds.
+     : list of :class:`~luna.MyBio.PDB.Residue.Residue`
+        The list of proximal compounds always include ``source``.
 
+    Raises
+    ------
+    IllegalArgumentError
+        If ``source`` is not a :class:`~luna.MyBio.PDB.Residue.Residue`
 
     Examples
     --------
 
-    In this example, we will identify all covalent bonds involving a given residue in the PDB 3QQK.
+    In this example, we will identify all proximal compounds to a given residue
+    in the PDB 3QQK.
     So, let's first parse the PDB file.
 
     >>> from luna.util.default_values import LUNA_PATH
     >>> from luna.MyBio.PDB.PDBParser import PDBParser
     >>> pdb_parser = PDBParser(PERMISSIVE=True, QUIET=True)
-    >>> structure = pdb_parser.get_structure("Protein", f"{LUNA_PATH}/tutorial/inputs/3QQK.pdb")
+    >>> structure = pdb_parser.get_structure("Protein", \
+f"{LUNA_PATH}/tutorial/inputs/3QQK.pdb")
 
     Now, we select the residue of our interest.
 
     >>> residue = structure[0]["A"][(' ', 81, ' ')]
 
-    Finally, let`s recover potential covalent bonds involving this residue with :meth:`get_cov_contacts_with`.
-    In the below snippet, pairs of atoms are sorted by atoms` serial number,
-    and the residue information is printed together with the atom name.
+    Finally, we call :meth:`get_proximal_compounds`.
 
-    >>> from luna.interaction.contact import get_cov_contacts_with
-    >>> cov_bonds = sorted(get_cov_contacts_with(structure, residue), key=lambda x: (x[0].serial_number, x[1].serial_number))
-    >>> for atm1, atm2 in cov_bonds:
-    >>>     pair = ("%s%d/%s" % (atm1.parent.resname, atm1.parent.id[1], atm1.name),
-    ...             "%s%d/%s" % (atm2.parent.resname, atm2.parent.id[1], atm2.name))
-    >>>     print(pair)
-    ('PHE80/C', 'GLU81/N')
-    ('GLU81/N', 'GLU81/CA')
-    ('GLU81/CA', 'GLU81/C')
-    ('GLU81/CA', 'GLU81/CB')
-    ('GLU81/C', 'GLU81/O')
-    ('GLU81/C', 'PHE82/N')
-    ('GLU81/CB', 'GLU81/CG')
-    ('GLU81/CG', 'GLU81/CD')
-    ('GLU81/CD', 'GLU81/OE1')
-    ('GLU81/CD', 'GLU81/OE2')
+    >>> from luna.interaction.contact import get_proximal_compounds
+    >>> compounds = get_proximal_compounds(residue)
+    >>> for c in compounds:
+    ...    print(c)
+    <Residue PHE het=  resseq=80 icode= >
+    <Residue GLU het=  resseq=81 icode= >
+    <Residue PHE het=  resseq=82 icode= >
     """
-    entities = get_contacts_with(entity, source, target, radius=COV_SEARCH_RADIUS, level='A')
+    if not isinstance(source, Residue):
+        raise IllegalArgumentError("Invalid object type. "
+                                   "A Residue object is expected instead.")
 
-    cov_bonds = set()
-    for atm1, atm2 in entities:
-        if is_covalently_bound(atm1, atm2):
-            cov_bonds.add(tuple(sorted([atm1, atm2], key=lambda x: x.serial_number)))
+    model = source.get_parent_by_level('M')
+    proximal = get_contacts_with(source, entity=model,
+                                 radius=radius, level='R')
 
-    return cov_bonds
+    # Sorted by the compound order as in the PDB.
+    return sorted(list(set([p[1] for p in proximal])),
+                  key=lambda r: (r.parent.parent.id, r.parent.id, r.idx))
 
 
-def get_proximal_compounds(source, radius=COV_SEARCH_RADIUS):
-    """Recover proximal compounds to ``source``.
+def get_cov_contacts_with(source, target=None, entity=None):
+    """Recover potential covalent bonds with ``source``.
+
+    Covalent bonds between two nearby atoms A and B are determined
+    as in Open Babel:
+
+    .. math:: 0.4 <= \overrightarrow{\|AB\|} <= A_{cov} + B_{cov} + 0.45
+
+    Where :math:`\overrightarrow{\|AB\|}` is the distance
+    between atoms A and B, and :math:`A_{cov}` and :math:`B_{cov}`
+    are the covalent radius of atoms A and B, respectively.
 
     Parameters
     ----------
-    source : :class:`~luna.MyBio.PDB.Residue.Residue`
-        The reference compound.
-    radius : float
-        The cutoff distance (in Å) for defining proximity.\
-        The default value is 2.2, which may recover potential residues bound to ``source`` through covalent bonds.
+    source : :class:`~luna.MyBio.PDB.Entity.Entity`
+        The reference, which can be any :class:`~luna.MyBio.PDB.Entity.Entity`
+        instance (structure, model, chain, residue, or atom).
+    target : :class:`~luna.MyBio.PDB.Entity.Entity`, optional
+        If provided, only covalent bonds with the ``target``
+        will be considered.
+    entity : :class:`~luna.MyBio.PDB.Entity.Entity`
+        The PDB object from where atoms will be recovered.
+        If not provided (the default), the model object that contains
+        ``source`` will be used instead.
 
     Returns
     -------
-     : list of :class:`~luna.MyBio.PDB.Residue.Residue`
-        The list of proximal compounds always include ``source``.
+     : set of tuple of (:class:`~luna.MyBio.PDB.Atom.Atom`, \
+            :class:`~luna.MyBio.PDB.Atom.Atom`)
+        Pairs of atoms with potential covalent bonds.
 
-    Raises
-    ------
-    IllegalArgumentError
-        If ``source`` is not a :class:`~luna.MyBio.PDB.Residue.Residue`
 
     Examples
     --------
 
-    In this example, we will identify all proximal compounds to a given residue in the PDB 3QQK.
-    So, let's first parse the PDB file.
+    In this example, we will identify all covalent bonds involving a given
+    residue in the PDB 3QQK. So, let's first parse the PDB file.
 
     >>> from luna.util.default_values import LUNA_PATH
     >>> from luna.MyBio.PDB.PDBParser import PDBParser
     >>> pdb_parser = PDBParser(PERMISSIVE=True, QUIET=True)
-    >>> structure = pdb_parser.get_structure("Protein", f"{LUNA_PATH}/tutorial/inputs/3QQK.pdb")
+    >>> structure = pdb_parser.get_structure("Protein", \
+f"{LUNA_PATH}/tutorial/inputs/3QQK.pdb")
 
     Now, we select the residue of our interest.
 
     >>> residue = structure[0]["A"][(' ', 81, ' ')]
 
-    Finally, we call :meth:`get_proximal_compounds`.
+    Finally, let`s recover potential covalent bonds involving this residue
+    with :meth:`get_cov_contacts_with`. In the below snippet, pairs of atoms
+    are sorted by atoms` serial number, and the residue information is printed
+    together with the atom name.
 
-    >>> from luna.interaction.contact import get_proximal_compounds
-    >>> compounds = get_proximal_compounds(residue)
-    >>> for c in compounds:
-    ...    print(c)
-    <Residue PHE het=  resseq=80 icode= >
-    <Residue GLU het=  resseq=81 icode= >
-    <Residue PHE het=  resseq=82 icode= >
+    >>> from luna.interaction.contact import get_cov_contacts_with
+    >>> cov_bonds = sorted(get_cov_contacts_with(residue, entity=structure),
+    ...                    key=lambda x: (x[0].serial_number,
+    ...                                   x[1].serial_number))
+    >>> for atm1, atm2 in cov_bonds:
+    >>>     pair = ("%s%d/%s" % (atm1.parent.resname,
+    ...                          atm1.parent.id[1],
+    ...                          atm1.name),
+    ...             "%s%d/%s" % (atm2.parent.resname,
+    ...                          atm2.parent.id[1],
+    ...                          atm2.name))
+    >>>     print(pair)
+    ('PHE80/C', 'GLU81/N')
+    ('GLU81/N', 'GLU81/CA')
+    ('GLU81/CA', 'GLU81/C')
+    ('GLU81/CA', 'GLU81/CB')
+    ('GLU81/C', 'GLU81/O')
+    ('GLU81/C', 'PHE82/N')
+    ('GLU81/CB', 'GLU81/CG')
+    ('GLU81/CG', 'GLU81/CD')
+    ('GLU81/CD', 'GLU81/OE1')
+    ('GLU81/CD', 'GLU81/OE2')
     """
-    if not isinstance(source, Residue):
-        raise IllegalArgumentError("Invalid object type. A Residue object is expected instead.")
 
-    model = source.get_parent_by_level('M')
-    proximal = get_contacts_with(entity=model, source=source, radius=radius, level='R')
+    entity = entity or source.get_parent_by_level("M")
+    entities = get_contacts_with(source,
+                                 target=target,
+                                 entity=entity,
+                                 radius=COV_SEARCH_RADIUS,
+                                 level='A')
 
-    # Sorted by the compound order as in the PDB.
-    return sorted(list(set([p[1] for p in proximal])), key=lambda r: (r.parent.parent.id, r.parent.id, r.idx))
+    cov_bonds = set()
+    for atm1, atm2 in entities:
+        if is_covalently_bound(atm1, atm2):
+            cov_bonds.add(tuple(sorted([atm1, atm2],
+                                       key=lambda x: x.serial_number)))
+
+    return cov_bonds
```

### Comparing `luna-0.12.2/luna/interaction/filter.py` & `luna-0.13.0/luna/interaction/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     """ Filter interactions based on their components.
 
     Parameters
     ----------
     ignore_self_inter : bool
         If True, ignore interactions involving atoms of the same compound.
     ignore_intra_chain : bool
-        If True, ignore intra-chain interactions (e.g., interactions between
-        residues in the same protein chain).
+        If True, ignore intra-chain interactions (e.g., interactions
+        between residues in the same protein chain).
     ignore_inter_chain : bool
         If True, ignore interactions between different chains.
     ignore_res_res : bool
         If True, ignore residue-residue interactions.
     ignore_res_nucl : bool
         If True, ignore residue-nucleotide interactions.
     ignore_res_hetatm : bool
@@ -45,16 +45,16 @@
         If True, ignore ligand-ligand interactions.
     ignore_h2o_h2o : bool
         If True, ignore water-water interactions.
     ignore_any_h2o : bool
         If True, ignore all interactions involving water.
     ignore_multi_comps : bool
         If True, ignore interactions established by atom groups composed of
-        multiple compounds (e.g.: amides formed by peptide bonds involve two
-        residues).
+        multiple compounds (e.g.: amides formed by peptide bonds involve
+        two residues).
     ignore_mixed_class : bool
         If True, ignore interactions established by atom groups comprising
         mixed compound classes (e.g. residues and ligands bound by a
         covalent bond).
     """
 
     def __init__(self, ignore_self_inter=True, ignore_intra_chain=True,
@@ -154,17 +154,77 @@
          : `InteractionFilter`
         """
         return cls(ignore_nucl_hetatm=ignore_nucl_hetatm,
                    ignore_hetatm_hetatm=ignore_hetatm_hetatm,
                    ignore_any_h2o=ignore_any_h2o,
                    ignore_self_inter=ignore_self_inter, **kwargs)
 
+    @classmethod
+    def from_config_file(cls, config_file):
+        """Initialize from a configuration file.
+
+        Parameters
+        ----------
+        config_file : str
+            The configuration file pathname.
+
+        Returns
+        -------
+         : `InteractionFilter`
+        """
+
+        if not path.exists(config_file):
+            raise OSError("File '%s' does not exist." % config_file)
+
+        params = Config(config_file)
+
+        inter_filter = None
+        if "default" in params.sections():
+            params_dict = params.get_section_map("default")
+            filter_type = params_dict.pop("type", None)
+
+            if filter_type is not None:
+                filter_type = filter_type.upper()
+
+                available_filters = ["PLI", "PPI", "PNI", "NNI", "NLI"]
+                if filter_type not in available_filters:
+                    raise KeyError("The accepted default filter types are: "
+                                   "%s." % ", ".join(available_filters))
+
+                if filter_type == "PLI":
+                    inter_filter = cls.new_pli_filter()
+
+                elif filter_type == "PPI":
+                    inter_filter = cls.new_ppi_filter()
+
+                elif filter_type == "PNI":
+                    inter_filter = cls.new_pni_filter()
+
+                elif filter_type == "NNI":
+                    inter_filter = cls.new_nni_filter()
+
+                elif filter_type == "NLI":
+                    inter_filter = cls.new_nli_filter()
+
+        if "ignore" in params.sections():
+            params_dict = params.get_section_map("ignore")
+            params_dict = {"ignore_" + k: v
+                           for k, v in params_dict.items()}
+
+            if inter_filter:
+                for prop, val in params_dict.items():
+                    setattr(inter_filter, prop, val)
+            else:
+                inter_filter = cls(**params_dict)
+
+        return inter_filter
+
     def is_valid_pair(self, src_grp, trgt_grp):
-        """Evaluate if a pair of atom groups are valid according to the
-        flags defined in this class.
+        """Evaluate if a pair of atom groups are valid according to the flags
+        defined in this class.
 
         src_grp, trgt_grp : :class:`luna.mol.groups.AtomGroup`
         """
 
         # It will always ignore interactions involving the same atom groups.
         # Loops in the graph is not permitted and does not make any sense.
         if src_grp == trgt_grp:
@@ -174,16 +234,16 @@
         # to which they belong to. For example, the centroid of an aromatic
         # ring cannot interact with an atom that belongs to the ring.
         # It is a type of Loop.
         if src_grp.contain_group(trgt_grp) or trgt_grp.contain_group(src_grp):
             return False
 
         # If one of the groups contain atoms from different compounds.
-        has_multi_comps \
-            = (len(src_grp.compounds) > 1 or len(trgt_grp.compounds) > 1)
+        has_multi_comps = (len(src_grp.compounds) > 1
+                           or len(trgt_grp.compounds) > 1)
         if self.ignore_multi_comps and has_multi_comps:
             return False
 
         # If one of the groups contain compounds from different classes as,
         # for instance, residue and ligand. It means that compounds from
         # different classes are covalently bonded to each other.
         has_any_mixed = (src_grp.is_mixed() or trgt_grp.is_mixed())
@@ -279,64 +339,22 @@
         #       residue -- residue -- h2o -- h2o -- ligand.
         is_h2o_h2o = (src_grp.is_water() and trgt_grp.is_water())
         if self.ignore_h2o_h2o and is_h2o_h2o:
             return False
 
         return True
 
-    @classmethod
-    def from_config_file(cls, config_file):
-
-        if not path.exists(config_file):
-            raise OSError("File '%s' does not exist." % config_file)
-
-        params = Config(config_file)
-
-        inter_filter = None
-        if "default" in params.sections():
-            params_dict = params.get_section_map("default")
-            filter_type = params_dict.pop("type", None)
-
-            if filter_type is not None:
-                filter_type = filter_type.upper()
-
-                available_filters = ["PLI", "PPI", "PNI", "NNI", "NLI"]
-                if filter_type not in available_filters:
-                    raise KeyError("The accepted default filter types are: "
-                                   "%s." % ", ".join(available_filters))
-
-                if filter_type == "PLI":
-                    inter_filter = cls.new_pli_filter()
-
-                elif filter_type == "PPI":
-                    inter_filter = cls.new_ppi_filter()
-
-                elif filter_type == "PNI":
-                    inter_filter = cls.new_pni_filter()
-
-                elif filter_type == "NNI":
-                    inter_filter = cls.new_nni_filter()
-
-                elif filter_type == "NLI":
-                    inter_filter = cls.new_nli_filter()
-
-        if "ignore" in params.sections():
-            params_dict = params.get_section_map("ignore")
-            params_dict = {"ignore_" + k: params.parse_value("ignore", k)
-                           for k in params_dict}
-
-            if inter_filter:
-                for prop, val in params_dict.items():
-                    setattr(inter_filter, prop, val)
-            else:
-                inter_filter = cls(**params_dict)
-
-        return inter_filter
-
     def save_config_file(self, config_file):
+        """Save the interaction filter parameters into a configuration file.
+
+        Parameters
+        ----------
+        config_file : str
+            The output configuration file.
+        """
         with open(config_file, "w") as OUT:
             OUT.write("[ignore]\n")
             OUT.write("self_inter = %s\n" % self.ignore_self_inter)
             OUT.write("intra_chain = %s\n" % self.ignore_intra_chain)
             OUT.write("inter_chain = %s\n" % self.ignore_inter_chain)
             OUT.write("res_res = %s\n" % self.ignore_res_res)
             OUT.write("res_nucl = %s\n" % self.ignore_res_nucl)
@@ -377,28 +395,28 @@
     accept_all : bool
         If True, all chains, compounds, and atoms will be considered valid.
     accept_all_chains : bool
         If True, all chains will be considered valid.
     accept_all_comps : bool
         If True, all compound names will be considered valid.
     accept_all_comp_nums : bool
-        If True, all compound numbers (residue sequence number
-        in the PDB format) will be considered valid.
+        If True, all compound numbers (residue sequence number in the PDB
+        format) will be considered valid.
     accept_all_atoms : bool
         If True, all atoms will be considered valid.
     chain_id : str or None
         If provided, accept only chains whose id matches ``chain_id``.
     comp_name : str or None
         If provided, accept only compounds whose name matches ``comp_name``.
     comp_num : int or None
-        If provided, accept only compounds whose sequence number
-        matches ``comp_num``.
+        If provided, accept only compounds whose sequence number matches
+        ``comp_num``.
     comp_icode : str or None
-        If provided, accept only compounds whose insertion code
-        matches ``comp_icode``.
+        If provided, accept only compounds whose insertion code matches
+        ``comp_icode``.
     atom : str or None
         If provided, accept only atoms whose name matches ``atom``.
     """
 
     def __init__(self, condition):
         self.accept_all = False
         self.accept_all_chains = False
@@ -482,17 +500,18 @@
                 and self.accept_all_comp_nums and self.accept_all_atoms):
             return True
 
         # Tries to identify the first valid compound in the atom group.
         for atm in atm_grp.atoms:
             comp = atm.parent
 
-            is_chain_valid, is_comp_valid, is_comp_num_valid, is_atom_valid = \
-                (self.accept_all_chains, self.accept_all_comps,
-                 self.accept_all_comp_nums, self.accept_all_atoms)
+            is_chain_valid = self.accept_all_chains
+            is_comp_valid = self.accept_all_comps
+            is_comp_num_valid = self.accept_all_comp_nums
+            is_atom_valid = self.accept_all_atoms
 
             if self.chain_id is not None and self.chain_id == comp.parent.id:
                 is_chain_valid = True
 
             if self.comp_name is not None and self.comp_name == comp.resname:
                 is_comp_valid = True
 
@@ -542,15 +561,15 @@
 
     @classmethod
     def from_config_file(cls, config_file):
         """Initialize from a configuration file.
 
         Parameters
         ----------
-        ``config_file`` : str
+        config_file : str
             The configuration file pathname.
 
         Returns
         -------
          : `BindingModeFilter`
 
         Examples
@@ -561,15 +580,15 @@
             ; To configurate an interaction type, create a new line and define
             ; the interaction: [New interaction]. Then you can define whether
             ; or not all interactions must be accepted by setting 'accept_only'
             ; to True or False.
 
             ; If you want to specify binding modes, use the variable
             ; 'accept_only', which expects a list of strings in the format:
-            ;       <CHAIN ID>/<COMPOUND NAME>/<COMPOUND NUMBER>/<ATOM>.
+            ; <CHAIN ID>/<COMPOUND NAME>/<COMPOUND NUMBER>/<ATOM>.
             ;
             ; Wildcards are accepted for the expected fields.
             ; For example, "*/HIS/*/*" represents all histidines' atoms from \
 all chains.
             ;               "A/CBL/*/*" represents all ligands named CBL from \
 chain A.
             ;               "B/HIS/*/N*" represents all histidines' nitrogens \
@@ -632,16 +651,16 @@
 
             filtering_config[inter_type] = conditions
             names_mapping[inter_type] = ori_name
 
         return cls(filtering_config, names_mapping)
 
     def is_valid(self, inter):
-        """Check if an interaction is valid or not based on this
-        binding mode configuration.
+        """Check if an interaction is valid or not based on this binding mode
+        configuration.
 
         inter : :class:`luna.interaction.type.InteractionType`
         """
         if inter.type.lower() in self.config:
             inter_type = inter.type.lower()
 
         elif ("aromatic stacking" in self.config
@@ -660,14 +679,22 @@
 
             if is_src_grp_valid or is_trgt_grp_valid:
                 return True
 
         return False
 
     def save_config_file(self, config_file):
+        """Save the binding mode filter parameters into a
+        configuration file.
+
+        Parameters
+        ----------
+        config_file : str
+            The output configuration file.
+        """
         args_by_section = defaultdict(list)
 
         for inter, conditions in self.config.items():
             section_name = self.names_map.get(inter, inter)
 
             multi_conditions = []
             for condition in conditions:
```

### Comparing `luna-0.12.2/luna/interaction/fp/fingerprint.py` & `luna-0.13.0/luna/interaction/fp/fingerprint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from rdkit.DataStructs.cDataStructs import ExplicitBitVect, SparseBitVect
 from scipy.sparse import issparse, csr_matrix
 from collections import defaultdict
 from rdkit import DataStructs
 
-from luna.util.exceptions import (BitsValueError, InvalidFingerprintType, IllegalArgumentError, FingerprintCountsError)
+from luna.util.exceptions import (BitsValueError, InvalidFingerprintType,
+                                  IllegalArgumentError, FingerprintCountsError)
 from luna.version import __version__
 
 
 import logging
 
 logger = logging.getLogger()
 
@@ -21,34 +22,42 @@
     """A fingerprint that stores indices of "on" bits.
 
     Parameters
     ----------
     indices : array_like of int
         Indices of "on" bits.
     fp_length : int
-        The fingerprint length (total number of bits). The default value is :math:`2^{32}`.
+        The fingerprint length (total number of bits).
+        The default value is :math:`2^{32}`.
     unfolded_fp : `Fingerprint` or None
         The unfolded version of this fingerprint.
         If None, this fingerprint may have not been folded yet.
     unfolding_map : dict, optional
-        A mapping between current indices and indices from the unfolded version of this fingerprint
-        what makes it possible to trace folded bits back to the original shells (features).
+        A mapping between current indices and indices from the unfolded version
+        of this fingerprint what makes it possible to trace folded bits back to
+        the original shells (features).
     props: dict, optional
-        Custom properties of the fingerprint, consisting of a string keyword and
-        some value. It can be used, for instance, to save the ligand name
+        Custom properties of the fingerprint, consisting of a string keyword
+        and some value. It can be used, for instance, to save the ligand name
         and parameters used to generate shells (IFP features).
     """
 
-    def __init__(self, indices, fp_length=DEFAULT_FP_LENGTH, unfolded_fp=None, unfolding_map=None, props=None):
+    def __init__(self,
+                 indices,
+                 fp_length=DEFAULT_FP_LENGTH,
+                 unfolded_fp=None,
+                 unfolding_map=None,
+                 props=None):
 
         indices = np.asarray(indices, dtype=np.long)
 
         if np.any(np.logical_or(indices < 0, indices >= fp_length)):
-            logger.exception("Provided indices are in a different bit scale.")
-            raise BitsValueError("Provided indices are in a different bit scale.")
+            error_msg = "Provided indices are in a different bit scale."
+            logger.exception(error_msg)
+            raise BitsValueError(error_msg)
 
         self._indices = np.unique(indices)
         self._fp_length = fp_length
         self._unfolded_fp = unfolded_fp
         self._unfolding_map = unfolding_map or {}
         self._props = props or {}
 
@@ -59,15 +68,16 @@
         """Initialize from an array of indices.
 
         Parameters
         ----------
         indices : array_like of int
             Indices of "on" bits.
         fp_length : int
-            The fingerprint length (total number of bits). The default value is :math:`2^{32}`.
+            The fingerprint length (total number of bits).
+            The default value is :math:`2^{32}`.
         **kwargs : dict, optional
             Extra arguments to `Fingerprint`. Refer to the documentation for a
             list of all possible arguments.
 
         Returns
         -------
          : `Fingerprint`
@@ -92,19 +102,20 @@
 
     @classmethod
     def from_vector(cls, vector, fp_length=None, **kwargs):
         """Initialize from a vector.
 
         Parameters
         ----------
-        vector : :class:`numpy.ndarray` or :class:`scipy.sparse.csr_matrix`
+        vector : :class:`numpy.ndarray` or `scipy.sparse.csr_matrix`
             Array of bits.
         fp_length : int, optional
             The fingerprint length (total number of bits).
-            If not provided, the fingerprint length will be defined based on the ``vector`` shape.
+            If not provided, the fingerprint length will be defined based on
+            the ``vector`` shape.
         **kwargs : dict, optional
             Extra arguments to `Fingerprint`. Refer to the documentation for a
             list of all possible arguments.
 
         Returns
         -------
          : `Fingerprint`
@@ -143,15 +154,16 @@
 
         Parameters
         ----------
         bit_string : str
             String of 0s and 1s.
         fp_length : int, optional
             The fingerprint length (total number of bits).
-            If not provided, the fingerprint length will be defined based on the string length.
+            If not provided, the fingerprint length will be defined based on
+            the string length.
         **kwargs : dict, optional
             Extra arguments to `Fingerprint`. Refer to the documentation for a
             list of all possible arguments.
 
         Returns
         -------
          : `Fingerprint`
@@ -173,27 +185,31 @@
 
     @classmethod
     def from_rdkit(cls, rdkit_fp, **kwargs):
         """Initialize from an RDKit fingerprint.
 
         Parameters
         ----------
-        rdkit_fp : :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` or :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`
+        rdkit_fp : :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` or\
+                        :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`
             An existing RDKit fingerprint.
         **kwargs : dict, optional
             Extra arguments to `Fingerprint`. Refer to the documentation for a
             list of all possible arguments.
 
         Returns
         -------
          : `Fingerprint`
         """
-        if not (isinstance(rdkit_fp, ExplicitBitVect) or isinstance(rdkit_fp, SparseBitVect)):
-            logger.exception("Invalid fingerprint type. RDKit only accepts a SparseBitVect or ExplicitBitVect object.")
-            raise TypeError("Invalid fingerprint type. RDKit only accepts a SparseBitVect or ExplicitBitVect object.")
+        if (not (isinstance(rdkit_fp, ExplicitBitVect)
+                 or isinstance(rdkit_fp, SparseBitVect))):
+            error_msg = ("Invalid fingerprint type. RDKit only accepts a "
+                         "SparseBitVect or ExplicitBitVect object.")
+            logger.exception(error_msg)
+            raise TypeError(error_msg)
 
         fp_length = rdkit_fp.GetNumBits()
         indices = np.asarray(rdkit_fp.GetOnBits(), dtype=np.long)
 
         return cls.from_indices(indices, fp_length, **kwargs)
 
     @classmethod
@@ -209,22 +225,29 @@
             list of all possible arguments.
 
         Returns
         -------
          : `Fingerprint`
         """
         if not isinstance(fp, Fingerprint):
-            logger.exception("Informed fingerprint is not an instance of %s." % (cls.__class__))
-            raise InvalidFingerprintType("Informed fingerprint is not an instance of %s." % (cls.__class__))
+            error_msg = ("Informed fingerprint is not an instance of %s."
+                         % (cls.__class__))
+            logger.exception(error_msg)
+            raise InvalidFingerprintType(error_msg)
 
-        unfolded_fp = fp.__class__.from_fingerprint(fp.unfolded_fp) if fp.unfolded_fp is not None else None
+        unfolded_fp = (fp.__class__.from_fingerprint(fp.unfolded_fp)
+                       if fp.unfolded_fp is not None else None)
         unfolding_map = dict(fp.unfolding_map)
         props = dict(fp.props)
 
-        return cls.from_indices(fp.indices, fp.fp_length, unfolded_fp=unfolded_fp, unfolding_map=unfolding_map, props=props)
+        return cls.from_indices(fp.indices,
+                                fp.fp_length,
+                                unfolded_fp=unfolded_fp,
+                                unfolding_map=unfolding_map,
+                                props=props)
 
     @property
     def indices(self):
         """array_like of int, read-only: Indices of "on" bits."""
         return self._indices
 
     @property
@@ -235,87 +258,93 @@
     @property
     def density(self):
         """float, read-only: Proportion of "on" bits in fingerprint."""
         return self.bit_count / self.fp_length
 
     @property
     def counts(self):
-        """dict, read-only: Mapping between each index in ``indices`` to the number of counts, which is always 1 for bit fingerprints."""
+        """dict, read-only: Mapping between each index in ``indices`` to the \
+        number of counts, which is always 1 for bit fingerprints."""
         return dict([(k, 1) for k in self.indices])
 
     @property
     def fp_length(self):
         """int, read-only: The fingerprint length (total number of bits)."""
         return self._fp_length
 
     @property
     def unfolded_fp(self):
-        """`Fingerprint` or None, read-only: The unfolded version of this fingerprint. If None, this fingerprint may have not been folded yet."""
+        """`Fingerprint` or None, read-only: The unfolded version of this \
+        fingerprint. If None, this fingerprint may have not been folded yet."""
         if self._unfolded_fp is None:
             logger.warning("This fingerprint was not previously folded.")
             return None
         return self._unfolded_fp
 
     @property
     def unfolded_indices(self):
-        """array_like of int, read-only: Indices of "on" bits in the unfolded fingerprint."""
+        """array_like of int, read-only: Indices of "on" bits in the unfolded \
+        fingerprint."""
         if self._unfolding_map is None:
             logger.warning("This fingerprint was not previously folded.")
             return None
         return self.unfolded_fp.indices
 
     @property
     def unfolding_map(self):
-        """dict, read-only: The mapping between current indices and indices from the unfolded version of this fingerprint
-        what makes it possible to trace folded bits back to the original shells (features)."""
+        """dict, read-only: The mapping between current indices and indices \
+        from the unfolded version of this fingerprint what makes it possible \
+        to trace folded bits back to the original shells (features)."""
         if self._unfolding_map is None:
             logger.warning("This fingerprint was not previously folded.")
             return None
         return self._unfolding_map
 
     @property
     def props(self):
         """dict, read-only: The custom properties of the fingerprint."""
         return self._props
 
     @property
     def name(self):
-        """str: The property 'name'. If it was not provided, then return an empty string."""
+        """str: The property 'name'. If it was not provided, then return an \
+        empty string."""
         return self.props.get("name", "")
 
     @name.setter
     def name(self, name):
         self.props["name"] = str(name)
 
     @property
     def num_levels(self):
-        """int: The property 'num_levels' used to generate this fingerprint \
-        (see :class:`~luna.interaction.fp.shell.ShellGenerator`). \
+        """int: The property `num_levels` used to generate this fingerprint
+        (see :class:`~luna.interaction.fp.shell.ShellGenerator`).
         If it was not provided, then return None."""
         return self.props.get("num_levels", None)
 
     @num_levels.setter
     def num_levels(self, num_levels):
         self.props["num_levels"] = str(num_levels)
 
     @property
     def radius_step(self):
-        """float: The property 'radius_step' used to generate this fingerprint \
-        (see :class:`~luna.interaction.fp.shell.ShellGenerator`). \
+        """float: The property 'radius_step' used to generate this
+        fingerprint (see \
+        :class:`~luna.interaction.fp.shell.ShellGenerator`). \
         If it was not provided, then return None."""
         return self.props.get("radius_step", None)
 
     @radius_step.setter
     def radius_step(self, radius_step):
         self.props["radius_step"] = str(radius_step)
 
     @property
     def num_shells(self):
-        """int: The property 'num_shells' \
-        (see :class:`~luna.interaction.fp.shell.ShellGenerator`). \
+        """int: The property `num_shells`
+        (see :class:`~luna.interaction.fp.shell.ShellGenerator`).
         If it was not provided, then return None."""
         return self.props.get("num_shells", None)
 
     @num_shells.setter
     def num_shells(self, num_shells):
         self.props["num_shells"] = str(num_shells)
 
@@ -352,192 +381,221 @@
             If the provided index is in a different bit scale.
         """
         if index in self.counts:
             return self.counts[index]
         elif index >= 0 and index < self.fp_length:
             return 0
         else:
-            logger.exception("The provided index is in a different bit scale.")
-            raise BitsValueError("The provided index is in a different bit scale.")
+            error_msg = "The provided index is in a different bit scale."
+            logger.exception(error_msg)
+            raise BitsValueError(error_msg)
 
     def get_on_bits(self):
         """Get "on" bits.
 
         Returns
         -------
          : :class:`numpy.ndarray`
         """
         return np.array([k for (k, v) in self.counts.items() if v > 0])
 
     def to_vector(self, compressed=True, dtype=DEFAULT_FP_DTYPE):
         """Convert this fingerprint to a vector of bits/counts.
 
         .. warning::
-            This function may raise a `MemoryError` exception when using huge indices vectors.
-            If you found this issue, you may want to try a different data type
-            or apply a folding operation before calling `to_vector`.
+            This function may raise a `MemoryError` exception when using
+            huge indices vectors. If you found this issue, you may want
+            to try a different data type or apply a folding operation
+            before calling `to_vector`.
 
         Parameters
         -------
         compressed : bool
-            If True, build a compressed sparse matrix (scipy.sparse.csr_matrix).
+            If True, build a compressed sparse matrix
+            (scipy.sparse.csr_matrix).
         dtype : data-type
             The default value is np.int32.
 
         Returns
         -------
-         : :class:`numpy.ndarray` or :class:`scipy.sparse.csr_matrix`
+         : :class:`numpy.ndarray` or `scipy.sparse.csr_matrix`
             Vector of bits/counts.
-            Return a compressed sparse matrix (`scipy.sparse.csr_matrix`) if ``compressed`` is True.
-            Otherwise, return a Numpy array (:class:`numpy.ndarray`)
+            Return a compressed sparse matrix (`scipy.sparse.csr_matrix`)
+            if ``compressed`` is True. Otherwise, return a Numpy array
+            (:class:`numpy.ndarray`)
 
         Raises
         ------
         BitsValueError
-            If some of the fingerprint indices are greater than the fingerprint length.
+            If some of the fingerprint indices are greater than the
+            fingerprint length.
         MemoryError
             If the operation ran out of memory.
         """
         data = [self.counts[i] for i in self.indices]
         if compressed:
             try:
                 row = np.zeros(self.bit_count)
                 col = self.indices
-                vector = csr_matrix((data, (row, col)), shape=(1, self.fp_length), dtype=dtype)
+                vector = csr_matrix((data, (row, col)),
+                                    shape=(1, self.fp_length),
+                                    dtype=dtype)
             except ValueError as e:
                 logger.exception(e)
-                raise BitsValueError("Sparse matrix construction failed. Invalid indices or input data.")
+                raise BitsValueError("Sparse matrix construction failed. "
+                                     "Invalid indices or input data.")
         else:
             try:
-                # This function is causing a MemoryError exception when using a 2**32 vector.
+                # This function is causing a MemoryError exception
+                # when using a 2**32 vector.
                 vector = np.zeros(self.fp_length, dtype=dtype)
             except MemoryError as e:
                 logger.exception(e)
-                raise MemoryError("Huge indices vector detected. An operation ran out of memory. "
-                                  "Use a different data type or apply a folding operation.")
+                raise MemoryError("Huge indices vector detected. "
+                                  "An operation ran out of memory. "
+                                  "Use a different data type or apply a "
+                                  "folding operation.")
 
             try:
                 vector[self.indices] = data
             except IndexError as e:
                 logger.exception(e)
-                raise BitsValueError("Some of the provided indices are greater than the fingerprint length.")
+                raise BitsValueError("Some of the provided indices are "
+                                     "greater than the fingerprint length.")
 
         return vector
 
     def to_bit_vector(self, compressed=True):
         """Convert this fingerprint to a vector of bits.
 
         .. warning::
-            This function may raise a `MemoryError` exception when using huge indices vectors.
-            If you found this issue, you may want to try a different data type
-            or apply a folding operation before calling `to_bit_vector`.
+            This function may raise a `MemoryError` exception when using huge
+            indices vectors. If you found this issue, you may want to try a
+            different data type or apply a folding operation before calling
+            `to_bit_vector`.
 
         Parameters
         -------
         compressed : bool
-            If True, build a compressed sparse matrix (scipy.sparse.csr_matrix).
+            If True, build a compressed sparse matrix
+            (scipy.sparse.csr_matrix).
 
         Returns
         -------
-         : :class:`numpy.ndarray` or :class:`scipy.sparse.csr_matrix`
+         : :class:`numpy.ndarray` or `scipy.sparse.csr_matrix`
             Vector of bits/counts.
-            Return a compressed sparse matrix (`scipy.sparse.csr_matrix`) if ``compressed`` is True.
-            Otherwise, return a Numpy array (:class:`numpy.ndarray`)
+            Return a compressed sparse matrix (`scipy.sparse.csr_matrix`)
+            if ``compressed`` is True. Otherwise, return a Numpy array
+            (:class:`numpy.ndarray`)
 
         Raises
         ------
         BitsValueError
-            If some of the fingerprint indices are greater than the fingerprint length.
+            If some of the fingerprint indices are greater than the
+            fingerprint length.
         MemoryError
             If the operation ran out of memory.
         """
-        return self.to_vector(compressed=compressed, dtype=np.bool_).astype(np.int8)
+        return self.to_vector(compressed=compressed,
+                              dtype=np.bool_).astype(np.int8)
 
     def to_bit_string(self):
         """Convert this fingerprint to a string of bits.
 
         .. warning::
-            This function may raise a `MemoryError` exception when using huge indices vectors.
-            If you found this issue, you may want to try a different data type
-            or apply a folding operation before calling `to_bit_string`.
+            This function may raise a `MemoryError` exception when using huge
+            indices vectors. If you found this issue, you may want to try a
+            different data type or apply a folding operation before calling
+            `to_bit_string`.
 
         Returns
         -------
          : str
 
         Raises
         ------
         MemoryError
             If the operation ran out of memory.
         """
         try:
-            # This function is causing a MemoryError exception when using a 2**32 vector.
+            # This function is causing a MemoryError exception
+            # when using a 2**32 vector.
             bit_vector = self.to_bit_vector(compressed=False).astype(np.int8)
             return "".join(map(str, bit_vector))
         except MemoryError as e:
             logger.exception(e)
-            raise MemoryError("Huge indices vector detected. An operation ran out of memory. "
-                              "Use a different data type or apply a folding operation.")
+            raise MemoryError("Huge indices vector detected. An operation ran "
+                              "out of memory. Use a different data type or "
+                              "apply a folding operation.")
 
     def to_rdkit(self, rdkit_fp_cls=None):
         """Convert this fingerprint to an RDKit fingerprint.
 
         .. note::
-            If the fingerprint length exceeds the maximum RDKit fingerprint length (:math:`2^{31} - 1`),
-            this fingerprint will be folded to length :math:`2^{31} - 1` before conversion.
+            If the fingerprint length exceeds the maximum RDKit fingerprint
+            length (:math:`2^{31} - 1`), this fingerprint will be folded to
+            length :math:`2^{31} - 1` before conversion.
 
         Returns
         -------
-         : :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` or :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`
-            If ``fp_length`` is less than :math:`1e5`, :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` is used.
-            Otherwise, :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect` is used.
+         : :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` or \
+                :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`
+            If ``fp_length`` is less than :math:`1e5`,
+            :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` is used.
+            Otherwise, :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`
+            is used.
         """
         if rdkit_fp_cls is None:
-            # Classes to store explicit bit vectors: ExplicitBitVect or SparseBitVect.
-            # ExplicitBitVect is most useful for situations where the size of the vector is
-            # relatively small (tens of thousands or smaller).
+            # Classes to store explicit bit vectors: ExplicitBitVect or
+            #    SparseBitVect.
+            # ExplicitBitVect is most useful for situations where the size of
+            # the vector is relatively small (tens of thousands or smaller).
             # For larger vectors, use the _SparseBitVect_ class instead.
             if self.fp_length < 1e5:
                 rdkit_fp_cls = ExplicitBitVect
             else:
                 rdkit_fp_cls = SparseBitVect
 
-        # RDKit data structure defines fingerprints as a std:set composed of ints (signed int).
-        # Since we always have values higher than 0 and since the data structure contains only signed ints,
-        # then the max length for a RDKit fingerprint is 2^31 - 1.
+        # RDKit data structure defines fingerprints as a std:set composed of
+        # ints (signed int). Since we always have values higher than 0 and
+        # since the data structure contains only signed ints, then the max
+        # length for a RDKit fingerprint is 2^31 - 1.
         # C signed int (32 bit) ranges: [-2^31, 2^31-1].
         max_rdkit_fp_length = 2**31 - 1
         fp_length = self.fp_length
         if max_rdkit_fp_length < fp_length:
-            logger.warning("The current fingerprint will be folded as its size is higher than the maximum "
-                           "size accepted by RDKit, which is 2**31 - 1.")
+            logger.warning("The current fingerprint will be folded as its "
+                           "size is higher than the maximum size accepted "
+                           "by RDKit, which is 2**31 - 1.")
             fp_length = max_rdkit_fp_length
         indices = self.indices % max_rdkit_fp_length
 
         rdkit_fp = rdkit_fp_cls(fp_length)
         rdkit_fp.SetBitsFromList(indices.tolist())
         return rdkit_fp
 
     def fold(self, new_length=DEFAULT_FOLDED_FP_LENGTH):
         """Fold this fingerprint to size ``new_length``.
 
         Parameters
         ----------
         new_length : int
-            Length of the new fingerprint, ideally multiple of 2. The default value is 4096.
+            Length of the new fingerprint, ideally multiple of 2.
+            The default value is 4096.
 
         Returns
         -------
          : `Fingerprint`
             Folded `Fingerprint`.
 
         Raises
         ------
         BitsValueError
-            If the new fingerprint length is not a multiple of 2 or is greater than the existing fingerprint length.
+            If the new fingerprint length is not a multiple of 2 or is greater
+            than the existing fingerprint length.
 
         Examples
         --------
         >>> from luna.interaction.fp.fingerprint import Fingerprint
         >>> import numpy as np
         >>> np.random.seed(0)
         >>> on_bits = 8
@@ -553,35 +611,40 @@
         >>> folded_fp = fp.fold(8)
         >>> print(folded_fp.indices)
         [0 3 4 5 7]
         >>> print(folded_fp.to_vector(compressed=False))
         [1 0 0 1 1 1 0 1]
         """
         if new_length > self.fp_length:
-            error_msg = ("The new fingerprint length must be smaller than the existing fingerprint length.")
+            error_msg = ("The new fingerprint length must be smaller than the "
+                         "existing fingerprint length.")
             logger.exception(error_msg)
             raise BitsValueError(error_msg)
 
         if not np.log2(self.fp_length / new_length).is_integer():
-            error_msg = ("It is not possible to fold the current fingerprint into the informed new length. "
-                         "The current length divided by the new one is not a power of 2 number.")
+            error_msg = ("It is not possible to fold the current fingerprint "
+                         "into the informed new length. The current length "
+                         "divided by the new one is not a power of 2 number.")
             logger.exception(error_msg)
             raise BitsValueError(error_msg)
 
         folded_indices = self.indices % new_length
 
         unfolding_map = defaultdict(set)
         for k, v in sorted(zip(folded_indices, self.indices)):
             unfolding_map[k].add(v)
 
         props = dict(self.props)
         if "fp_length" in props:
             props["fp_length"] = new_length
-        new_fp = self.__class__(indices=folded_indices, fp_length=new_length,
-                                unfolded_fp=self, unfolding_map=unfolding_map, props=props)
+        new_fp = self.__class__(indices=folded_indices,
+                                fp_length=new_length,
+                                unfolded_fp=self,
+                                unfolding_map=unfolding_map,
+                                props=props)
 
         return new_fp
 
     def unfold(self):
         """Unfold this fingerprint and return its parent fingerprint.
 
         Returns
@@ -601,16 +664,18 @@
         ------
         InvalidFingerprintType
             If the informed fingerprint is not an instance of `Fingerprint`.
         BitsValueError
             If the fingerprints have different lengths.
         """
         if not isinstance(other, Fingerprint):
-            logger.exception("The informed fingerprint is not an instance of %s." % (other.__class__))
-            raise InvalidFingerprintType("The informed fingerprint is not an instance of %s." % (other.__class__))
+            error_msg = ("The informed fingerprint is not an instance of %s."
+                         % (other.__class__))
+            logger.exception(error_msg)
+            raise InvalidFingerprintType(error_msg)
 
         if self.fp_length != other.fp_length:
             raise BitsValueError("Fingerprints are in a different bit scale")
 
         return np.union1d(self.indices, other.indices)
 
     def intersection(self, other):
@@ -624,16 +689,18 @@
         ------
         InvalidFingerprintType
             If the informed fingerprint is not an instance of `Fingerprint`.
         BitsValueError
             If the fingerprints have different lengths.
         """
         if not isinstance(other, Fingerprint):
-            logger.exception("Informed fingerprint is not an instance of %s." % (other.__class__))
-            raise InvalidFingerprintType("Informed fingerprint is not an instance of %s." % (other.__class__))
+            error_msg = ("Informed fingerprint is not an instance of %s."
+                         % (other.__class__))
+            logger.exception(error_msg)
+            raise InvalidFingerprintType(error_msg)
 
         if self.fp_length != other.fp_length:
             raise BitsValueError("Fingerprints are in a different bit scale")
 
         return np.intersect1d(self.indices, other.indices, assume_unique=True)
 
     def difference(self, other):
@@ -647,16 +714,18 @@
         ------
         InvalidFingerprintType
             If the informed fingerprint is not an instance of `Fingerprint`.
         BitsValueError
             If the fingerprints have different lengths.
         """
         if not isinstance(other, Fingerprint):
-            logger.exception("Informed fingerprint is not an instance of %s." % (other.__class__))
-            raise InvalidFingerprintType("Informed fingerprint is not an instance of %s." % (other.__class__))
+            error_msg = ("Informed fingerprint is not an instance of %s."
+                         % (other.__class__))
+            logger.exception(error_msg)
+            raise InvalidFingerprintType(error_msg)
 
         if self.fp_length != other.fp_length:
             raise BitsValueError("Fingerprints are in a different bit scale")
 
         return np.setdiff1d(self.indices, other.indices, assume_unique=True)
 
     def symmetric_difference(self, other):
@@ -670,48 +739,56 @@
         ------
         InvalidFingerprintType
             If the informed fingerprint is not an instance of `Fingerprint`.
         BitsValueError
             If the fingerprints have different lengths.
         """
         if not isinstance(other, Fingerprint):
-            logger.exception("Informed fingerprint is not an instance of %s." % (other.__class__))
-            raise InvalidFingerprintType("Informed fingerprint is not an instance of %s." % (other.__class__))
+            error_msg = ("Informed fingerprint is not an instance of %s."
+                         % (other.__class__))
+            logger.exception(error_msg)
+            raise InvalidFingerprintType(error_msg)
 
         if self.fp_length != other.fp_length:
             raise BitsValueError("Fingerprints are in a different bit scale")
 
         return np.setxor1d(self.indices, other.indices, assume_unique=True)
 
     def calc_similarity(self, other):
-        """Calculates the Tanimoto similarity between this fingeprint and ``other``.
+        """Calculates the Tanimoto similarity between this fingeprint
+        and ``other``.
 
         Returns
         -------
          : float
 
         Examples
         --------
         >>> from luna.interaction.fp.fingerprint import Fingerprint
         >>> fp1 = Fingerprint.from_bit_string("0010101110000010")
         >>> fp2 = Fingerprint.from_bit_string("1010100110010010")
         >>> print(fp1.calc_similarity(fp2))
         0.625
         """
-        return DataStructs.FingerprintSimilarity(self.to_rdkit(), other.to_rdkit())
+        return DataStructs.FingerprintSimilarity(self.to_rdkit(),
+                                                 other.to_rdkit())
 
     def __repr__(self):
         return ("<%s: indices=%s length=%d>" %
-                (self.__class__, repr(self.indices).replace('\n', '').replace(' ', ''), self.fp_length))
+                (self.__class__,
+                 repr(self.indices).replace('\n', '').replace(' ', ''),
+                 self.fp_length))
 
     def __eq__(self, other):
         if isinstance(other, Fingerprint):
             return (self.__class__ == other.__class__
                     and self.fp_length == other.fp_length
-                    and np.all(np.in1d(self.indices, other.indices, assume_unique=True)))
+                    and np.all(np.in1d(self.indices,
+                                       other.indices,
+                                       assume_unique=True)))
         return False
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __or__(self, other):
         return self.union(other)
@@ -734,166 +811,194 @@
     ----------
     indices : array_like of int, optional
         Indices of "on" bits. It is optional if ``counts`` is provided.
     counts : dict, optional
         Mapping between each index in ``indices`` to the number of counts.
         If not provided, the default count value of 1 will be used instead.
     fp_length : int
-        The fingerprint length (total number of bits). The default value is :math:`2^{32}`.
+        The fingerprint length (total number of bits).
+        The default value is :math:`2^{32}`.
     unfolded_fp : `Fingerprint` or None
         The unfolded version of this fingerprint.
         If None, this fingerprint may have not been folded yet.
     unfolding_map : dict, optional
-        A mapping between current indices and indices from the unfolded version of this fingerprint
-        what makes it possible to trace folded bits back to the original shells (features).
+        A mapping between current indices and indices from the unfolded version
+        of this fingerprint what makes it possible to trace folded bits back to
+        the original shells (features).
     props: dict, optional
-        Custom properties of the fingerprint, consisting of a string keyword and
-        some value. It can be used, for instance, to save the ligand name
+        Custom properties of the fingerprint, consisting of a string keyword
+        and some value. It can be used, for instance, to save the ligand name
         and parameters used to generate shells (IFP features).
     """
 
     def __init__(self, indices=None, counts=None, fp_length=DEFAULT_FP_LENGTH,
                  unfolded_fp=None, unfolding_map=None, props=None):
 
         if indices is None and counts is None:
             logger.exception("Indices or counts must be provided.")
             raise IllegalArgumentError("Indices or counts must be provided.")
 
         if indices is not None:
             indices = np.asarray(indices, dtype=np.long)
 
             if np.any(np.logical_or(indices < 0, indices >= fp_length)):
-                logger.exception("Provided indices are in a different bit scale.")
-                raise BitsValueError("Provided indices are in a different bit scale.")
+                error_msg = "Provided indices are in a different bit scale."
+                logger.exception(error_msg)
+                raise BitsValueError(error_msg)
 
             if counts is None:
                 indices, counts = np.unique(indices, return_counts=True)
                 counts = dict(zip(indices, counts))
             else:
                 indices = np.unique(indices)
                 if not np.all([x in indices for x in counts]):
-                    logger.exception("At least one index from 'counts' is not in 'indices'.")
-                    raise FingerprintCountsError("At least one index from 'counts' is not in 'indices'.")
+                    error_msg = ("At least one index from 'counts' is not in "
+                                 "'indices'.")
+                    logger.exception(error_msg)
+                    raise FingerprintCountsError(error_msg)
+
                 if len(set(indices).symmetric_difference(counts)) > 0:
-                    logger.exception("At least one index in 'indices' is not in 'counts'.")
-                    raise FingerprintCountsError("At least one index in 'indices' is not in 'counts'.")
+                    error_msg = ("At least one index in 'indices' is not "
+                                 "in 'counts'.")
+                    logger.exception(error_msg)
+                    raise FingerprintCountsError(error_msg)
         else:
             indices = np.asarray(sorted(counts.keys()), dtype=np.long)
 
             if np.any(np.logical_or(indices < 0, indices >= fp_length)):
-                logger.exception("Provided indices are in a different bit scale.")
-                raise BitsValueError("Provided indices are in a different bit scale.")
+                error_msg = ("Provided indices are in a different bit scale.")
+                logger.exception(error_msg)
+                raise BitsValueError(error_msg)
 
         self._counts = counts
         super().__init__(indices, fp_length, unfolded_fp, unfolding_map, props)
 
     @classmethod
-    def from_indices(cls, indices=None, counts=None, fp_length=DEFAULT_FP_LENGTH, **kwargs):
+    def from_indices(cls,
+                     indices=None,
+                     counts=None,
+                     fp_length=DEFAULT_FP_LENGTH,
+                     **kwargs):
         """Initialize from an array of indices.
 
         Parameters
         ----------
         indices : array_like of int, optional
             Indices of "on" bits. It is optional if ``counts`` is provided.
         counts : dict, optional
             Mapping between each index in ``indices`` to the number of counts.
             If not provided, the default count value of 1 will be used instead.
         fp_length : int
-            The fingerprint length (total number of bits). The default value is :math:`2^{32}`.
+            The fingerprint length (total number of bits).
+            The default value is :math:`2^{32}`.
         **kwargs : dict, optional
-            Extra arguments to `CountFingerprint`. Refer to the documentation for a
-            list of all possible arguments.
+            Extra arguments to `CountFingerprint`. Refer to the documentation
+            for a list of all possible arguments.
 
         Returns
         -------
          : `CountFingerprint`
 
         Examples
         --------
         >>> from luna.interaction.fp.fingerprint import CountFingerprint
         >>> import numpy as np
         >>> np.random.seed(0)
         >>> on_bits = 8
         >>> fp_length = 32
-        >>> indices, counts = np.unique(np.random.randint(0, fp_length, on_bits), return_counts=True)
+        >>> indices, counts = np.unique(np.random.randint(0, \
+fp_length, on_bits), return_counts=True)
         >>> counts = dict(zip(indices, counts))
         >>> print(counts)
         {0: 1, 3: 2, 7: 1, 12: 1, 15: 1, 21: 1, 27: 1}
-        >>> fp = CountFingerprint.from_indices(indices, counts=counts, fp_length=fp_length)
+        >>> fp = CountFingerprint.from_indices(indices, counts=counts, \
+fp_length=fp_length)
         >>> print(fp.indices)
         [ 0  3  7 12 15 21 27]
         >>> print(fp.to_vector(compressed=False))
         [1 0 0 2 0 0 0 1 0 0 0 0 1 0 0 1 0 0 0 0 0 1 0 0 0 0 0 1 0 0 0 0]
         """
-        return cls(indices=indices, counts=counts, fp_length=fp_length, **kwargs)
+        return cls(indices=indices, 
+                   counts=counts,
+                   fp_length=fp_length,
+                   **kwargs)
 
     @classmethod
     def from_counts(cls, counts, fp_length=DEFAULT_FP_LENGTH, **kwargs):
         """Initialize from a counting map.
 
         Parameters
         ----------
         counts : dict
             Mapping between each index in ``indices`` to the number of counts.
         fp_length : int
-            The fingerprint length (total number of bits). The default value is :math:`2^{32}`.
+            The fingerprint length (total number of bits).
+            The default value is :math:`2^{32}`.
         **kwargs : dict, optional
-            Extra arguments to `CountFingerprint`. Refer to the documentation for a
-            list of all possible arguments.
+            Extra arguments to `CountFingerprint`. Refer to the documentation
+            for a list of all possible arguments.
 
         Returns
         -------
          : `CountFingerprint`
 
         Examples
         --------
         >>> from luna.interaction.fp.fingerprint import CountFingerprint
         >>> import numpy as np
         >>> np.random.seed(0)
         >>> on_bits = 8
         >>> fp_length = 32
-        >>> counts = dict(zip(*np.unique(np.random.randint(0, fp_length, on_bits),
+        >>> counts = dict(zip(*np.unique(np.random.randint(0, fp_length, \
+on_bits),
         ...                              return_counts=True)))
         >>> print(counts)
         {0: 1, 3: 2, 7: 1, 12: 1, 15: 1, 21: 1, 27: 1}
-        >>> fp = CountFingerprint.from_counts(counts=counts, fp_length=fp_length)
+        >>> fp = CountFingerprint.from_counts(counts=counts,
+        ...                                   fp_length=fp_length)
         >>> print(fp.indices)
         [ 0  3  7 12 15 21 27]
         >>> print(fp.to_vector(compressed=False))
         1 0 0 2 0 0 0 1 0 0 0 0 1 0 0 1 0 0 0 0 0 1 0 0 0 0 0 1 0 0 0 0]
         """
         return cls(counts=counts, fp_length=fp_length, **kwargs)
 
     @classmethod
-    def from_bit_string(cls, bit_string, counts=None, fp_length=None, **kwargs):
+    def from_bit_string(cls,
+                        bit_string,
+                        counts=None,
+                        fp_length=None,
+                        **kwargs):
         """Initialize from a bit string (e.g. '0010100110').
 
         Parameters
         ----------
         bit_string : str
             String of 0s and 1s.
         counts : dict, optional
             Mapping between each index in ``indices`` to the number of counts.
             If not provided, the default count value of 1 will be used instead.
         fp_length : int, optional
             The fingerprint length (total number of bits).
-            If not provided, the fingerprint length will be defined based on the string length.
+            If not provided, the fingerprint length will be defined based on
+            the string length.
         **kwargs : dict, optional
             Extra arguments to `Fingerprint`. Refer to the documentation for a
             list of all possible arguments.
 
         Returns
         -------
          : `CountFingerprint`
 
         Examples
         --------
         >>> from luna.interaction.fp.fingerprint import CountFingerprint
         >>> fp = CountFingerprint.from_bit_string("0010100110000010",
-        ...                                       counts={2: 5, 4: 1, 7: 3, 8: 1, 14: 2})
+        ...                                       counts={2: 5, 4: 1, 7: 3, \
+8: 1, 14: 2})
         >>> print(fp.indices)
         [ 2  4  7  8 14]
         >>> print(fp.counts)
         {2: 5, 4: 1, 7: 3, 8: 1, 14: 2}
         """
         indices = [i for i, char in enumerate(bit_string) if char != '0']
         if fp_length is None:
@@ -903,41 +1008,44 @@
 
     @classmethod
     def from_vector(cls, vector, fp_length=None, **kwargs):
         """Initialize from a vector.
 
         Parameters
         ----------
-        vector : :class:`numpy.ndarray` or :class:`scipy.sparse.csr_matrix`
+        vector : :class:`numpy.ndarray` or `scipy.sparse.csr_matrix`
             Array of counts.
         fp_length : int, optional
             The fingerprint length (total number of bits).
-            If not provided, the fingerprint length will be defined based on the ``vector`` shape.
+            If not provided, the fingerprint length will be defined based on
+            the ``vector`` shape.
         **kwargs : dict, optional
             Extra arguments to `Fingerprint`. Refer to the documentation for a
             list of all possible arguments.
 
         Returns
         -------
          : `CountFingerprint`
 
         Examples
         --------
         >>> from luna.interaction.fp.fingerprint import CountFingerprint
         >>> import numpy as np
         >>> np.random.seed(0)
         >>> fp_length = 32
-        >>> vector = np.random.choice(5, size=(fp_length,), p=[0.76, 0.1, 0.1, 0.02, 0.02])
+        >>> vector = np.random.choice(5, size=(fp_length,),
+        ...                           p=[0.76, 0.1, 0.1, 0.02, 0.02])
         >>> print(vector)
         [0 0 0 0 2 3 0 1 0 0 2 0 0 0 1 1 2 3 1 0 1 0 0 0 2 0 0 0 1 0 0 0]
         >>> fp = CountFingerprint.from_vector(vector)
         >>> print(fp.indices)
         [ 4  5  7 10 14 15 16 17 18 20 24 28]
         >>> print(fp.counts)
-        {4: 2, 5: 3, 7: 1, 10: 2, 14: 1, 15: 1, 16: 2, 17: 3, 18: 1, 20: 1, 24: 2, 28: 1}
+        {4: 2, 5: 3, 7: 1, 10: 2, 14: 1, 15: 1, 16: 2, 17: 3, 18: 1, 20: 1, \
+24: 2, 28: 1}
         """
         if fp_length is None:
             try:
                 fp_length = vector.shape[1]
             except IndexError:
                 fp_length = vector.shape[0]
 
@@ -964,87 +1072,104 @@
             list of all possible arguments.
 
         Returns
         -------
          : `CountFingerprint`
         """
         if not isinstance(fp, Fingerprint):
-            logger.exception("Informed fingerprint is not an instance of %s." % (cls.__class__))
-            raise InvalidFingerprintType("Informed fingerprint is not an instance of %s." % (cls.__class__))
+            error_msg = ("Informed fingerprint is not an instance of %s."
+                         % (cls.__class__))
+            logger.exception(error_msg)
+            raise InvalidFingerprintType(error_msg)
 
         counts = dict([(i, c) for i, c in fp.counts.items() if c > 0])
-        unfolded_fp = fp.__class__.from_fingerprint(fp.unfolded_fp) if fp.unfolded_fp is not None else None
+        unfolded_fp = (fp.__class__.from_fingerprint(fp.unfolded_fp)
+                       if fp.unfolded_fp is not None else None)
         unfolding_map = dict(fp.unfolding_map)
         props = dict(fp.props)
 
         new_fp = cls.from_counts(counts, fp.fp_length, unfolded_fp=unfolded_fp,
                                  unfolding_map=unfolding_map, props=props)
 
         return new_fp
 
     @property
     def counts(self):
-        """dict, read-only: Mapping between each index in ``indices`` to the number of counts."""
+        """dict, read-only: Mapping between each index in ``indices`` \
+        to the number of counts."""
         return self._counts
 
     def get_count(self, index):
-        """Get the count value at index ``index``. Return 0 if index is not in ``counts``."""
+        """Get the count value at index ``index``. Return 0 if index \
+        is not in ``counts``."""
         return self.counts.get(index, 0)
 
     def fold(self, new_length=DEFAULT_FOLDED_FP_LENGTH):
         """Fold this fingerprint to size ``new_length``.
 
         Parameters
         ----------
         new_length : int
-            Length of the new fingerprint, ideally multiple of 2. The default value is 4096.
+            Length of the new fingerprint, ideally multiple of 2.
+            The default value is 4096.
 
         Returns
         -------
          : `Fingerprint`
             Folded `Fingerprint`.
 
         Raises
         ------
         BitsValueError
-            If the new fingerprint length is not a multiple of 2 or is greater than the existing fingerprint length.
+            If the new fingerprint length is not a multiple of 2 or is greater
+            than the existing fingerprint length.
 
         Examples
         --------
         >>> from luna.interaction.fp.fingerprint import CountFingerprint
         >>> import numpy as np
         >>> np.random.seed(0)
         >>> on_bits = 8
         >>> fp_length = 32
-        >>> indices, counts = np.unique(np.random.randint(0, fp_length, on_bits), return_counts=True)
+        >>> indices, counts = np.unique(np.random.randint(0, fp_length, \
+on_bits),
+        ...                             return_counts=True)
         >>> counts = dict(zip(indices, counts))
         >>> print(counts)
         {0: 1, 3: 2, 7: 1, 12: 1, 15: 1, 21: 1, 27: 1}
-        >>> fp = CountFingerprint.from_indices(indices, counts=counts, fp_length=fp_length)
+        >>> fp = CountFingerprint.from_indices(indices, counts=counts,
+        ...                                    fp_length=fp_length)
         >>> print(fp.indices)
         [ 0  3  7 12 15 21 27]
         >>> print(fp.to_vector(compressed=False))
         [1 0 0 2 0 0 0 1 0 0 0 0 1 0 0 1 0 0 0 0 0 1 0 0 0 0 0 1 0 0 0 0]
         >>> folded_fp = fp.fold(8)
         >>> print(folded_fp.indices)
         [0 3 4 5 7]
         >>> print(folded_fp.to_vector(compressed=False))
         [1 0 0 3 1 1 0 2]
         """
         new_fp = super().fold(new_length)
 
-        new_fp._counts = dict([(folded_idx, sum([self.get_count(x) for x in unfolded_set]))
-                               for folded_idx, unfolded_set in new_fp.unfolding_map.items()])
+        new_fp._counts = dict([(folded_idx, sum([self.get_count(x)
+                                                 for x in unfolded_set]))
+                               for folded_idx, unfolded_set
+                               in new_fp.unfolding_map.items()])
 
         return new_fp
 
     def __repr__(self):
         return ("<%s: counts={%s} length=%d>" %
-                (self.__class__, tuple([(k, v) for k, v in self.counts.items()]), self.fp_length))
+                (self.__class__,
+                 tuple([(k, v)
+                        for k, v in self.counts.items()]),
+                 self.fp_length))
 
     def __eq__(self, other):
         if isinstance(other, Fingerprint):
             return (self.__class__ == other.__class__
                     and self.counts == other.counts
                     and self.fp_length == other.fp_length
-                    and np.all(np.in1d(self.indices, other.indices, assume_unique=True)))
+                    and np.all(np.in1d(self.indices,
+                                       other.indices,
+                                       assume_unique=True)))
         return False
```

### Comparing `luna-0.12.2/luna/interaction/fp/shell.py` & `luna-0.13.0/luna/interaction/fp/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from enum import Enum
 import numpy as np
 import mmh3
 
 from luna.version import __version__
 from luna.util.exceptions import ShellCenterNotFound
 from luna.util.default_values import CHEMICAL_FEATURE_IDS, INTERACTION_IDS
-from luna.interaction.fp.fingerprint import DEFAULT_FP_LENGTH, Fingerprint, CountFingerprint
+from luna.interaction.fp.fingerprint import (DEFAULT_FP_LENGTH, Fingerprint,
+                                             CountFingerprint)
 from luna.interaction.fp.type import IFPType
 from luna.mol.groups import PseudoAtomGroup, AtomGroupNeighborhood
 from luna.mol.features import ChemicalFeature
 
 
 import logging
 
@@ -36,25 +37,25 @@
 
     Parameters
     ----------
     num_levels : int
         The maximum number of iterations for fingerprint generation.
     radius_step : float
         The multiplier used to increase shell size at each iteration.
-        At iteration 0, shell radius is 0 * ``radius_step``, at iteration 1, radius is
-        1 * ``radius_step``, etc.
+        At iteration 0, shell radius is 0 * ``radius_step``, at iteration 1,
+        radius is 1 * ``radius_step``, etc.
     fp_length : int
         The fingerprint length (total number of bits).
     ifp_type : :class:`~luna.interaction.fp.type.IFPType`
         The fingerprint type (EIFP, FIFP, or HIFP).
     shells : iterable of :class:`Shell`, optional
         An initial sequence of :class:`Shell` objects (fingerprint features).
     verbose : bool
-        If True, warnings issued during the usage of this `ShellManager` will be displayed.
-        The default value is False.
+        If True, warnings issued during the usage of this `ShellManager` will
+        be displayed. The default value is False.
 
     Attributes
     ----------
     num_levels : int
         The maximum number of iterations for fingerprint generation.
     radius_step : float
         The multiplier used to increase shell size at each iteration.
@@ -65,25 +66,33 @@
     shells : iterable of :class:`Shell`
         The sequence of shells (fingerprint features).
     verbose : bool
         The verbosity state.
     version : str
         The LUNA's version with which shells were generated.
     levels : dict of {int: list of `Shell`}
-        Register shells by level, where keys are levels and values are lists of `Shell` objects.
+        Register shells by level, where keys are levels and values are
+        lists of `Shell` objects.
 
         .. note::
             Levels are 0-indexed. So, the first level is 0, second is 1, etc.
             That means if ``num_levels`` is 5, the last level will be 4.
     centers : dict of dict of {int: `Shell`}
-        Register shells by center, where keys are :class:`~luna.mol.groups.AtomGroup` objects and
-        values are dict that store all shells generated for that center at each iteration (level).
+        Register shells by center, where keys are \
+        :class:`~luna.mol.groups.AtomGroup` objects and values are dict that
+        store all shells generated for that center at each iteration (level).
     """
 
-    def __init__(self, num_levels, radius_step, fp_length, ifp_type, shells=None, verbose=False):
+    def __init__(self,
+                 num_levels,
+                 radius_step,
+                 fp_length,
+                 ifp_type,
+                 shells=None,
+                 verbose=False):
         self.num_levels = num_levels
         self.radius_step = radius_step
         self.fp_length = fp_length
         self.ifp_type = ifp_type
 
         self.shells = shells or []
         self.verbose = verbose
@@ -100,77 +109,83 @@
     @property
     def num_unique_shells(self):
         """int, read-only: Total number of unique shells in ``shells``."""
         return len(self.unique_shells)
 
     @property
     def unique_shells(self):
-        """iterable of `Shell`, read-only: Unique shells. Return the same as :meth:`get_valid_shells`."""
+        """iterable of `Shell`, read-only: Unique shells. \
+        Return the same as :meth:`get_valid_shells`."""
         return self.get_valid_shells()
 
     def find_similar_shell(self, shell):
         """Find a shell in ``shells`` similar to ``shell``.
 
-        Two shells are similar if they represent the same substructural information.
+        Two shells are similar if they represent the same substructural
+        information.
 
         Parameters
         ----------
         shell : `Shell`
 
         Returns
         -------
          : `Shell` or None
             Return a similar shell or None if it does not find any.
         """
         for added_shell in self.shells:
-            # For each group of similar shells, it will exist only one valid shell.
+            # For each group of similar shells, it will exist only
+            # one valid shell.
             if added_shell.is_valid():
                 if shell.is_similar(added_shell):
                     return added_shell
         return None
 
     def add_shell(self, shell):
         """Add a new shell to ``shells``.
 
         Parameters
         ----------
         shell : `Shell`
         """
 
-        # Any new shell without interactions from level 1 onwards will be automatically considered invalid.
+        # Any new shell without interactions from level 1 onwards will be
+        # automatically considered invalid.
         if shell.level > 0 and len(shell.interactions) == 0:
             shell.valid = False
         else:
             found_shell = self.find_similar_shell(shell)
 
             if found_shell:
                 if found_shell.level < shell.level:
                     shell.valid = False
 
-                elif found_shell.level == shell.level and found_shell.identifier <= shell.identifier:
+                elif (found_shell.level == shell.level
+                        and found_shell.identifier <= shell.identifier):
                     shell.valid = False
 
                 else:
                     found_shell.valid = False
 
         self.shells.append(shell)
         self.levels[shell.level].append(shell)
         self.centers[shell.central_atm_grp][shell.level] = shell
 
     def get_valid_shells(self):
         """Return only valid shells.
 
-        A shell is considered invalid if, by the time it is added in ``shells``, there is another
-        shell representing the same substructural information.
-        That means this shell is not unique and does not contributes to any new information.
-
-        On the other hand, if the shell contributes by adding new information to ``shells``,
-        then it will be considered valid and unique.
-        So, the first shell of a series of shells containing the same information is considered
-        valid and the others invalid.
+        A shell is considered invalid if, by the time it is added in
+        ``shells``, there is another shell representing the same
+        substructural information. That means this shell is not unique
+        and does not contributes to any new information.
+
+        On the other hand, if the shell contributes by adding new information
+        to ``shells``, then it will be considered valid and unique. So, the
+        first shell of a series of shells containing the same information is
+        considered valid and the others invalid.
 
         Returns
         -------
          : list of `Shell`
         """
         return [s for s in self.shells if s.is_valid()]
 
@@ -179,22 +194,24 @@
 
         Parameters
         ----------
         identifier : int
             The shell identifier.
         unique_shells : bool
             If True, return only unique shells.
-            Otherwise, return all shells having the identifier ``identifier`` (the default).
+            Otherwise, return all shells having the identifier
+            ``identifier`` (the default).
 
         Returns
         -------
          : list of `Shell`
         """
         if unique_shells:
-            return [s for s in self.shells if s.identifier == identifier and s.is_valid()]
+            return [s for s in self.shells
+                    if s.identifier == identifier and s.is_valid()]
         else:
             return [s for s in self.shells if s.identifier == identifier]
 
     def get_shells_by_level(self, level, unique_shells=False):
         """Get shells by level (iteration number).
 
         Parameters
@@ -222,118 +239,136 @@
 
     def get_shells_by_center(self, center, unique_shells=False):
         """Get shells by center (:class:`~luna.mol.groups.AtomGroup` object).
 
         Parameters
         ----------
         center : :class:`~luna.mol.groups.AtomGroup`
-            The center of a shell, which consists of an :class:`~luna.mol.groups.AtomGroup` object.
+            The center of a shell, which consists of an
+            :class:`~luna.mol.groups.AtomGroup` object.
         unique_shells : bool
             If True, return only unique shells.
-            Otherwise, return all shells generated for center ``center`` (the default).
+            Otherwise, return all shells generated for center
+            ``center`` (the default).
 
 
         Returns
         -------
          : dict of {int: `Shell`}
             All shells generated for center ``center`` at each iteration (key).
         """
         shells = {}
 
         if center in self.centers:
             if unique_shells:
-                shells = {i: s for i, s in self.centers[center].items() if s.is_valid()}
+                shells = {i: s for i, s in self.centers[center].items()
+                          if s.is_valid()}
             else:
                 shells = self.centers[center]
         elif self.verbose:
             logger.warning("The informed center '%s' does not exist." % center)
 
         return shells
 
-    def get_shell_by_center_and_level(self, center, level, unique_shells=False):
+    def get_shell_by_center_and_level(self,
+                                      center,
+                                      level,
+                                      unique_shells=False):
         """Get the shell generated for center ``center``
-        (:class:`~luna.mol.groups.AtomGroup` object) at level (iteration) ``level``.
+        (:class:`~luna.mol.groups.AtomGroup` object) at level (iteration)
+        ``level``.
 
         Parameters
         ----------
         center : :class:`~luna.mol.groups.AtomGroup`
-            The center of a shell, which consists of an :class:`~luna.mol.groups.AtomGroup` object.
+            The center of a shell, which consists of an
+            :class:`~luna.mol.groups.AtomGroup` object.
         level : int
             The target level (iteration).
         unique_shells : bool
-            If True, return the `Shell` object if it is unique and None otherwise.
-            The default value is False.
+            If True, return the `Shell` object if it is unique and None
+            otherwise. The default value is False.
 
         Returns
         -------
          : `Shell` or None
             The shell generated for center ``center`` at level ``level``.
             If the `Shell` object is not unique, return None.
         """
         shell = self.centers.get(center, {}).get(level)
 
         if shell is None and self.verbose:
-            logger.warning("The informed center '%s' does not exist in the level '%d'." % (center, level))
+            logger.warning("The informed center '%s' does not exist in "
+                           "the level '%d'." % (center, level))
 
         if unique_shells:
             shell = shell if shell.is_valid() else None
             if shell is None and self.verbose:
-                logger.warning("The shell found with center '%s' and level '%d' is not unique." % (center, level))
+                logger.warning("The shell found with center '%s' and level "
+                               "'%d' is not unique." % (center, level))
 
         return shell
 
     def get_previous_shell(self, center, curr_level, unique_shells=False):
-        """Get the last shell having center ``center`` that was generated before level ``curr_level``.
-        For instance, if the current level (iteration) is 5 and the last valid shell generated for
-        center :math:`C` was at level 4, then :meth:`get_previous_shell` would return that shell at level 4.
+        """Get the last shell having center ``center`` that was generated
+        before level ``curr_level``. For instance, if the current level
+        (iteration) is 5 and the last valid shell generated for center
+        :math:`C` was at level 4, then :meth:`get_previous_shell` would
+        return that shell at level 4.
 
         Parameters
         ----------
         center : :class:`~luna.mol.groups.AtomGroup`
-            The center of a shell, which consists of an :class:`~luna.mol.groups.AtomGroup` object.
+            The center of a shell, which consists of an
+            :class:`~luna.mol.groups.AtomGroup` object.
         curr_level : int
             The current level (iteration).
         unique_shells : bool
-            If True, ignore non-valid shells and go down to inferior levels until a valid shell is found.
-            If level 0 was reached and no valid shell was found, then return None.
+            If True, ignore non-valid shells and go down to inferior
+            levels until a valid shell is found. If level 0 was reached
+            and no valid shell was found, then return None.
             The default value is False.
 
         Returns
         -------
          : `Shell` or None
             The first previous valid shell or None if no valid shell was found.
         """
         shell = None
         while curr_level != 0 and shell is None:
             level = curr_level - 1
-            shell = self.get_shell_by_center_and_level(center, level, unique_shells)
+            shell = self.get_shell_by_center_and_level(center,
+                                                       level,
+                                                       unique_shells)
             curr_level = level
 
         if shell is None and self.verbose:
-            logger.warning("No previous shell centered on '%s' departing from the level '%d' was found."
-                           % (center, level))
+            logger.warning("No previous shell centered on '%s' departing from "
+                           "the level '%d' was found." % (center, level))
 
         return shell
 
     def get_last_shell(self, center, unique_shells=False):
         """Get the last shell generated for center ``center``.
 
         Parameters
         ----------
         center : :class:`~luna.mol.groups.AtomGroup`
-            The center of a shell, which consists of an :class:`~luna.mol.groups.AtomGroup` object.
+            The center of a shell, which consists of an
+            :class:`~luna.mol.groups.AtomGroup` object.
         unique_shells : bool
             If True, ignore non-valid shells.
-            That means shells generated at superior levels may be ignored if they are not valid.
-            The default value is False.
+            That means shells generated at superior levels may be ignored
+            if they are not valid. The default value is False.
 
         Returns
         -------
          : `Shell` or None
-            The last shell generated for center ``center`` or None if no valid shell was found.
+            The last shell generated for center ``center`` or None if
+            no valid shell was found.
         """
         shell = None
 
         shells = self.get_shells_by_center(center, unique_shells)
         if shells:
             # Sort by key and get a shell based on the latest value.
             shell = shells[sorted(shells, key=int)[-1]]
@@ -346,90 +381,113 @@
         """Get all shells' identifier.
 
         Parameters
         ----------
         level : int, optional
             If provided, only return identifiers of shells at level ``level``.
         unique_shells : bool
-            If True, ignore identifiers of non-valid shells. The default value is False.
+            If True, ignore identifiers of non-valid shells.
+            The default value is False.
 
         Returns
         -------
          : list of int
         """
         if level is not None:
             if unique_shells:
-                identifiers = [s.identifier for s in self.get_shells_by_level(level) if s.is_valid()]
+                identifiers = [s.identifier
+                               for s in self.get_shells_by_level(level)
+                               if s.is_valid()]
             else:
-                identifiers = [s.identifier for s in self.get_shells_by_level(level)]
+                identifiers = [s.identifier
+                               for s in self.get_shells_by_level(level)]
         else:
             if unique_shells:
-                identifiers = [s.identifier for s in self.shells if s.is_valid()]
+                identifiers = [s.identifier for s in self.shells
+                               if s.is_valid()]
             else:
                 identifiers = [s.identifier for s in self.shells]
 
         return sorted(identifiers)
 
-    def to_fingerprint(self, fold_to_length=None, count_fp=False, unique_shells=False):
+    def to_fingerprint(self,
+                       fold_to_length=None,
+                       count_fp=False,
+                       unique_shells=False):
         """Encode shells into an interaction fingerprint.
 
         Parameters
         ----------
         fold_to_length : int, optional
             If provided, fold the fingerprint to length ``fold_to_length``.
         count_fp : bool
-            If True, create a count fingerprint (:class:`~luna.interaction.fp.fingerprint.CountFingerprint`).
-            Otherwise, return a bit fingerprint (:class:`~luna.interaction.fp.fingerprint.Fingerprint`).
+            If True, create a count fingerprint
+            (:class:`~luna.interaction.fp.fingerprint.CountFingerprint`).
+            Otherwise, return a bit fingerprint
+            (:class:`~luna.interaction.fp.fingerprint.Fingerprint`).
         unique_shells : bool
-            If True, only unique shells are used to create the fingerprint. The default value is False.
+            If True, only unique shells are used to create the fingerprint.
+            The default value is False.
 
         Returns
         -------
-         : :class:`~luna.interaction.fp.fingerprint.CountFingerprint` or :class:`~luna.interaction.fp.fingerprint.Fingerprint`
+         : :class:`~luna.interaction.fp.fingerprint.CountFingerprint` or \
+                :class:`~luna.interaction.fp.fingerprint.Fingerprint`
         """
         indices = self.get_identifiers(unique_shells=unique_shells)
         props = {"num_levels": self.num_levels,
                  "fp_length": self.fp_length,
                  "radius_step": self.radius_step}
 
         if count_fp:
-            fp = CountFingerprint(indices, fp_length=self.fp_length, props=props)
+            fp = CountFingerprint(indices,
+                                  fp_length=self.fp_length,
+                                  props=props)
         else:
-            fp = Fingerprint(indices, fp_length=self.fp_length, props=props)
+            fp = Fingerprint(indices,
+                             fp_length=self.fp_length,
+                             props=props)
 
         if fold_to_length:
             return fp.fold(fold_to_length)
         return fp
 
-    def trace_back_feature(self, feature_id, ifp, unique_shells=False):
-        """Trace a feature from a fingerprint back to the shells that originated that feature.
+    def trace_back_feature(self,
+                           feature_id, ifp,
+                           unique_shells=False):
+        """Trace a feature from a fingerprint back to the shells
+        that originated that feature.
 
         .. note::
-            Due to fingerprint folding, multiple substructures may end up encoded in the same bit,
-            the so-called collision problem. So, if the provided feature contains collisions,
-            shells representing different substructures may be returned by :meth:`trace_back_feature`.
+            Due to fingerprint folding, multiple substructures may end up
+            encoded in the same bit, the so-called collision problem.
+            So, if the provided feature contains collisions, shells
+            representing different substructures may be returned by
+            :meth:`trace_back_feature`.
 
         Parameters
         ----------
         feature_id: int
             The target feature id.
         ifp : `Fingerprint`
             The fingerprint containing the feature ``feature_id``.
         unique_shells : bool
-            If True, ignore identifiers of non-valid shells. The default value is False.
+            If True, ignore identifiers of non-valid shells.
+            The default value is False.
 
         Yields
         -------
          : `Shell`
 
         Examples
         --------
 
-        In the below example, we will assume a LUNA project object named ``proj_obj`` already exists.
-        Then, we will generate an EIFP fingerprint for the first :class:`~luna.mol.groups.AtomGroupsManager`
+        In the below example, we will assume a LUNA project object named
+        ``proj_obj`` already exists. Then, we will generate an EIFP
+        fingerprint for the first :class:`~luna.mol.groups.AtomGroupsManager`
         object at ``proj_obj``.
 
         >>> from luna.interaction.fp.shell import ShellGenerator
         >>> from luna.interaction.fp.type import IFPType
         >>> atm_grps_mngr = list(proj_obj.atm_grps_mngrs)[0]
         >>> num_levels, radius_step = 2, 3
         >>> sg = ShellGenerator(num_levels, radius_step, ifp_type=IFPType.EIFP)
@@ -440,23 +498,28 @@
            93  109  138  140  157  162  181  182  186  187  191  194  206  209
           211  237  246  251  263  271  281  296  304  315  323  358  370  374
           388  392  399  400  419  439  476  481  487  509  519  527  532  578
           587  592  604  605  629  635  645  661  668  698  711  713  732  736
           740  753  764  795  813  815  820  824  825  831  836  855  873  882
           911  926  967  975  976  984  990  996 1020]
 
-        Now, we can trace features back to original identifiers and investigate its substructural information.
+        Now, we can trace features back to original identifiers and investigate
+        its substructural information.
 
-        >>> ori_indices = list(sm.trace_back_feature(34, fp, unique_shells=True))
+        >>> ori_indices = list(sm.trace_back_feature(34, fp, \
+unique_shells=True))
         >>> print(ori_indices)
-        [(494318626, [<Shell: level=0, radius=0.000000, center=<AtomGroup: [<ExtendedAtom: 3QQK/0/A/GLN/85/CD>, <ExtendedAtom: 3QQK/0/A/GLN/85/NE2>, <ExtendedAtom: 3QQK/0/A/GLN/85/OE1>]>, interactions=0>])]
+        [(494318626, [<Shell: level=0, radius=0.000000, center=<AtomGroup: \
+[<ExtendedAtom: 3QQK/0/A/GLN/85/CD>, <ExtendedAtom: 3QQK/0/A/GLN/85/NE2>, \
+<ExtendedAtom: 3QQK/0/A/GLN/85/OE1>]>, interactions=0>])]
 
         """
         for ori_feature in ifp.unfolding_map[feature_id]:
-            yield (ori_feature, self.get_shells_by_identifier(ori_feature, unique_shells))
+            yield (ori_feature,
+                   self.get_shells_by_identifier(ori_feature, unique_shells))
 
     def _init_controllers(self):
         levels = defaultdict(list)
         centers = defaultdict(lambda: defaultdict(lambda: None))
 
         for shell in self.shells:
             levels[shell.level].append(shell)
@@ -464,85 +527,100 @@
 
         self.levels = levels
         self.centers = centers
 
 
 class Shell:
 
-    """
-    A container to store substructural information, which is the base for LUNA fingerprints.
+    """ A container to store substructural information, which is the base for
+    LUNA fingerprints.
 
-    Shells are centered on an atom or atom group (:class:`~luna.mol.groups.AtomGroup` objects)
-    and represent all atoms and interactions explicitly within it.
+    Shells are centered on an atom or atom group
+    (:class:`~luna.mol.groups.AtomGroup` objects) and represent all atoms and
+    interactions explicitly within it.
 
     Parameters
     ----------
     central_atm_grp : :class:`~luna.mol.groups.AtomGroup`
         The shell center.
     level : int
         The level (iteration) at which the shell was generated.
     radius : float
         The shell radius.
     neighborhood : iterable of :class:`~luna.mol.groups.AtomGroup`
-        All atoms and atom groups within a shell of radius ``radius`` centered on ``central_atm_grp``.
-    inter_tuples : iterable of (:class:`~luna.interaction.type.InteractionType`, :class:`~luna.mol.groups.AtomGroup`)
-        All interactions within a shell of radius ``radius`` centered on ``central_atm_grp``.
-        Each tuple contains an :class:`~luna.interaction.type.InteractionType` object
-        and one of the :class:`~luna.mol.groups.AtomGroup` objects participating to the interaction.
+        All atoms and atom groups within a shell of radius ``radius`` centered
+        on ``central_atm_grp``.
+    inter_tuples : iterable of \
+            (:class:`~luna.interaction.type.InteractionType`, \
+             :class:`~luna.mol.groups.AtomGroup`)
+        All interactions within a shell of radius ``radius`` centered on
+        ``central_atm_grp``. Each tuple contains an
+        :class:`~luna.interaction.type.InteractionType` object and one of the
+        :class:`~luna.mol.groups.AtomGroup` objects participating to the
+        interaction.
 
         .. note::
-            As an interaction involves two participants, it would be expected that each interaction produces two tuples.
-            However, by default, ShellGenerator sorts atom groups and considers only the first tuple that appears, \
-            which guarantees that only one of the possible tuples is added to avoid information duplication.
+            As an interaction involves two participants, it would be expected
+            that each interaction produces two tuples. However, by default,
+            ShellGenerator sorts atom groups and considers only the first tuple
+            that appears, which guarantees that only one of the possible tuples
+            is added to avoid information duplication.
     diff_comp_classes : bool
-        If True (the default), include differentiation between compound classes.
-        That means structural information originated from :class:`~luna.mol.groups.AtomGroup` objects
-        belonging to residues, nucleotides,  ligands, or water molecules will be considered different
-        even if their structural information are the same.
-        This is useful for example to differentiate protein-ligand interactions from residue-residue ones.
+        If True (the default), include differentiation between
+        compound classes. That means structural information originated from
+        :class:`~luna.mol.groups.AtomGroup` objects belonging to residues,
+        nucleotides,  ligands, or water molecules will be considered different
+        even if their structural information are the same. This is useful for
+        example to differentiate protein-ligand interactions from
+        residue-residue ones.
     dtype : data-type
-        Use arrays of type ``dtype`` to store information. The default value is np.int64.
+        Use arrays of type ``dtype`` to store information.
+        The default value is np.int64.
     seed : int
-        A seed to generate shell identifiers through the MurmurHash3 hash function.
-        The default value is 0.
+        A seed to generate shell identifiers through the MurmurHash3 hash
+        function. The default value is 0.
     manager : `ShellManager`
         The `ShellManager` object that stores and controls this `Shell` object.
     valid : bool
-        If the shell is valid or not. By default, all shells are considered valid.
+        If the shell is valid or not. By default, all shells are considered
+        valid.
     feature_mapper : dict, optional
         A dict that maps atoms and interactions to unique values.
-        If not provided, ``feature_mapper`` will inherit from the default mappings
-        ``CHEMICAL_FEATURE_IDS`` and ``INTERACTION_IDS``.
+        If not provided, ``feature_mapper`` will inherit from the default
+        mappings ``CHEMICAL_FEATURE_IDS`` and ``INTERACTION_IDS``.
 
     Attributes
     ----------
     central_atm_grp : :class:`~luna.mol.groups.AtomGroup`
     level : int
     radius : float
     diff_comp_classes : bool
     dtype : data-type
     seed : int
     valid : bool
     feature_mapper : dict
     """
 
-    def __init__(self, central_atm_grp, level, radius, neighborhood=None, inter_tuples=None,
+    def __init__(self, central_atm_grp,
+                 level, radius, neighborhood=None, inter_tuples=None,
                  diff_comp_classes=True, dtype=np.int64, seed=0, manager=None,
                  valid=True, feature_mapper=None):
 
         self.central_atm_grp = central_atm_grp
         self.level = level
         self.radius = radius
         self.valid = valid
         self.diff_comp_classes = diff_comp_classes
 
         if not neighborhood:
-            # If inter_tuples was not defined, initialize the neighborhood as an empty list.
-            # Otherwise, define the neighborhood as the atom groups interacting with the central atom group.
-            neighborhood = [] if not inter_tuples else [x[1] for x in self._inter_tuples]
+            # If inter_tuples was not defined, initialize the neighborhood
+            # as an empty list. Otherwise, define the neighborhood as the
+            # atom groups interacting with the central atom group.
+            neighborhood = ([] if not inter_tuples
+                            else [x[1] for x in self._inter_tuples])
         self._neighborhood = set(neighborhood)
 
         # Always add the central atom in its own neighborhood.
         self._neighborhood.add(central_atm_grp)
 
         inter_tuples = inter_tuples or []
         self._inter_tuples = set(inter_tuples)
@@ -559,147 +637,175 @@
         self.feature_mapper = feature_mapper
 
         self.dtype = dtype
         self.seed = seed
 
         self._manager = manager
 
-        # Encode the interactions. It represents the substructures comprised by this shell.
+        # Encode the interactions. It represents the substructures comprised by
+        # this shell.
         self._encoded_data = self._encode_interactions()
         # Defined in the hash function
         self._identifier = self.hash_shell()
 
     @property
     def neighborhood(self):
-        """iterable of :class:`~luna.mol.groups.AtomGroup`, read-only: All atoms and atom groups within this shell."""
+        """iterable of :class:`~luna.mol.groups.AtomGroup`, read-only: \
+                All atoms and atom groups within this shell."""
         return self._neighborhood
 
     @property
     def interactions(self):
-        """iterable of :class:`~luna.interaction.type.InteractionType`, read-only: All interactions within this shell."""
+        """iterable of :class:`~luna.interaction.type.InteractionType`, \
+                read-only: All interactions within this shell."""
         return self._interactions
 
     @property
     def inter_tuples(self):
-        """iterable of tuple, read-only: Each tuple contains an :class:`~luna.interaction.type.InteractionType` object \
-        and one of the :class:`~luna.mol.groups.AtomGroup` objects participating to the interaction."""
+        """iterable of tuple, read-only: Each tuple contains an \
+                :class:`~luna.interaction.type.InteractionType` object \
+                and one of the :class:`~luna.mol.groups.AtomGroup` objects \
+                participating to the interaction."""
         return self._inter_tuples
 
     @property
     def manager(self):
-        """`ShellManager`, read-only: The `ShellManager` object that stores and controls this `Shell` object."""
+        """`ShellManager`, read-only: The `ShellManager` object that stores \
+        and controls this `Shell` object."""
         return self._manager
 
     @property
     def identifier(self):
-        """int, read-only: This shell identifier, which is generated by hashing its
-        encoded data with a hash function. By default, LUNA uses MurmurHash3 as the hash function."""
+        """int, read-only: This shell identifier, which is generated by \
+        hashing its encoded data with a hash function. By default, LUNA \
+        uses MurmurHash3 as the hash function."""
         return self._identifier
 
     @property
     def encoded_data(self):
         """iterable of tuple, read-only: The data encoded in this shell."""
         return self._encoded_data
 
     @property
     def previous_shell(self):
-        """`Shell`, read-only: The previous shell, i.e., a shell centered on the same central \
-        :class:`~luna.mol.groups.AtomGroup` object from a previous level. \
-        For example, if this shell is in level 5, return a shell from level 4 having the same center."""
-        shell = self._manager.get_previous_shell(self.central_atm_grp, self.level)
+        """`Shell`, read-only: The previous shell, i.e., a shell centered \
+        on the same central :class:`~luna.mol.groups.AtomGroup` object from \
+        a previous level. For example, if this shell is in level 5, return \
+        a shell from level 4 having the same center."""
+        shell = self._manager.get_previous_shell(self.central_atm_grp,
+                                                 self.level)
         if shell is None:
-            logger.exception("No previous shell centered in '%s' was found." % self.central_atm_grp)
-            raise ShellCenterNotFound("No previous shell centered in '%s' was found." % self.central_atm_grp)
+            error_msg = ("No previous shell centered in '%s' was found."
+                         % self.central_atm_grp)
+            logger.exception(error_msg)
+            raise ShellCenterNotFound(error_msg)
         return shell
 
     def is_valid(self):
         """If the shell is valid or not.
 
         Returns
         -------
          : bool
         """
         return self.valid
 
     def is_similar(self, shell):
         """ If this shell is similar to ``shell``.
 
-        Two shells are similar if they represent the same substructural information.
+        Two shells are similar if they represent the same substructural
+        information.
 
         Parameters
         ----------
         shell : `Shell`
 
         Returns
         -------
          : bool
         """
 
-        # The shells' identifiers will be equal when the shells encode the same information and were constructed in the same level.
+        # The shells' identifiers will be equal when the shells encode the same
+        # information and were constructed in the same level.
         if self.level == shell.level:
             if self.identifier == shell.identifier:
                 return True
             return False
 
-        # If none of the shells have interactions, check if the shells have equal identifiers.
+        # If none of the shells have interactions, check if the shells have
+        # equal identifiers.
         if not self.interactions and not shell.interactions:
-            # If the identifiers are different, but the shells' central group is the same, it means the shells encode the same
-            # information even if their levels are different.
+            # If the identifiers are different, but the shells' central group
+            # is the same, it means the shells encode the same information
+            # even if their levels are different.
             #
-            # OBS: this test is only for fast identification without doing a recursive procedure as the one applied in the ELSE statement.
+            # OBS: this test is only for fast identification without doing a
+            # recursive procedure as the one applied in the ELSE statement.
             if self.central_atm_grp == shell.central_atm_grp:
                 return True
-            # Although two shells contain different identifiers and their centroids are not the same, they can still be equal if they
+            # Although two shells contain different identifiers and their
+            # centroids are not the same, they can still be equal if they
             # were obtained in different levels.
             else:
                 if self.level > shell.level:
                     return self.previous_shell.is_similar(shell)
                 return self.is_similar(shell.previous_shell)
 
-        # If both shells have interactions, check if the interactions are equal.
+        # If both shells have interactions, check if the interactions are
+        # equal.
         elif self.interactions and shell.interactions:
             if self.encoded_data == shell.encoded_data:
                 return True
         return False
 
     def hash_shell(self):
-        """Hash this shells' substructural information into a 32-bit integer using MurmurHash3.
+        """Hash this shells' substructural information into a 32-bit integer
+        using MurmurHash3.
 
         Returns
         -------
          : int
-            A 32-bit integer representing this shell's substructural information.
+            A 32-bit integer representing this shell's substructural
+            information.
         """
 
         if self.level == 0:
-            # Get the initial data for the first shell according to the IFP type the user has chosen.
+            # Get the initial data for the first shell according to the IFP
+            # type the user has chosen.
             data = self._initial_shell_data()
         else:
             cent_prev_id = self.previous_shell.identifier
 
             # Initialization of a new feature vector
             data = [(self.level, cent_prev_id)]
 
             inter_tuples = []
             for (inter, nb_atm_grp) in self._inter_tuples:
                 if isinstance(nb_atm_grp, PseudoAtomGroup):
-                    # Pseudo-groups that represents only the atoms involved in a specific interaction don't generate shells.
-                    # Only their parents do, i.e., the whole group generates shells. So, use it instead.
+                    # Pseudo-groups that represents only the atoms involved in
+                    # a specific interaction don't generate shells.
+                    # Only their parents do, i.e., the whole group generates
+                    # shells. So, use it instead.
                     nb_atm_grp = nb_atm_grp.parent_grp
 
-                prev_nb_shell = self._manager.get_previous_shell(nb_atm_grp, self.level)
+                prev_nb_shell = \
+                    self._manager.get_previous_shell(nb_atm_grp, self.level)
                 if prev_nb_shell is None:
-                    logger.exception("No previous shell centered in %s was found." % nb_atm_grp)
-                    raise ShellCenterNotFound("No previous shell centered in %s was found." % nb_atm_grp)
+                    error_msg = ("No previous shell centered in %s was found."
+                                 % nb_atm_grp)
+                    logger.exception(error_msg)
+                    raise ShellCenterNotFound(error_msg)
 
                 # 1st elem: interaction type.
                 # 2nd elem: previous identifier of the neighbor atom group;
-                inter_tuples.append((self.feature_mapper[inter.type], prev_nb_shell.identifier))
+                inter_tuples.append((self.feature_mapper[inter.type],
+                                     prev_nb_shell.identifier))
 
-            # Sort the tuples to avoid dependence on the order in which tuples are added.
+            # Sort the tuples to avoid dependence on the order in which tuples
+            # are added.
             sorted_list = sorted(inter_tuples)
 
             # Join the interaction information to the feature vector.
             data += sorted_list
 
         np_array = np.array(data, self.dtype)
 
@@ -709,54 +815,66 @@
         return hashed_shell
 
     def _initial_shell_data(self):
         data = []
 
         # EIFP uses atomic invariants.
         if self.manager.ifp_type == IFPType.EIFP:
-            # Shells use atomic invariants as data. In case of atom groups, the data consists of a list of invariants.
-            data = sorted([atm.invariants for atm in self.central_atm_grp.atoms])
+            # Shells use atomic invariants as data. In case of atom groups,
+            # the data consists of a list of invariants.
+            data = sorted([atm.invariants
+                           for atm in self.central_atm_grp.atoms])
 
-        # HIFP uses atomic invariants for atoms and pharmacophore information for atom groups.
+        # HIFP uses atomic invariants for atoms and pharmacophore information
+        # for atom groups.
         elif self.manager.ifp_type == IFPType.HIFP:
 
             if len(self.central_atm_grp.atoms) == 1:
                 # Shells whose centroid are atoms use invariants as data.
-                data = sorted([atm.invariants for atm in self.central_atm_grp.atoms])
+                data = sorted([atm.invariants
+                               for atm in self.central_atm_grp.atoms])
             else:
-                # Shells whose centroid are atoms' group use pharmacophore as data.
-                data = [[self.feature_mapper[cf.format_name()] for cf in self.central_atm_grp.features]]
+                # Shells whose centroid are atoms' group use pharmacophore
+                # as data.
+                data = [[self.feature_mapper[cf.format_name()]
+                         for cf in self.central_atm_grp.features]]
 
         # FIFP uses pharmacophore properties for atoms and atoms' group.
         elif self.manager.ifp_type == IFPType.FIFP:
 
-            atm_grp_data = [self.feature_mapper[cf.format_name()] for cf in self.central_atm_grp.features]
+            atm_grp_data = [self.feature_mapper[cf.format_name()]
+                            for cf in self.central_atm_grp.features]
 
             if len(self.central_atm_grp.atoms) == 1:
                 features = set()
-                # It will loop only through one atom and, therefore, it can be removed without
-                # losing information. However, if someday I decide to remove the If, then the code for capturing
-                # all atom derived features will be already working.
+                # It will loop only through one atom and, therefore, it can be
+                # removed without losing information. However, if someday I
+                # decide to remove the If, then the code for capturing all atom
+                # derived features will be already working.
                 for atm in self.central_atm_grp.atoms:
                     for atm_grp in atm.atm_grps:
                         if atm_grp != self.central_atm_grp:
                             features.update(atm_grp.features)
 
-                atm_grp_data += [self.feature_mapper[cf.format_name()] for cf in features]
+                atm_grp_data += [self.feature_mapper[cf.format_name()]
+                                 for cf in features]
 
             data = [sorted(atm_grp_data)]
 
-        #
-        #
-        # Include differentiation between compound classes, i.e., groups belonging to Residues, Nucleotides, Ligands, or Waters
-        # are treated as being different even when the group would be considered the same.
+        # Include differentiation between compound classes, i.e., groups
+        # belonging to Residues, Nucleotides, Ligands, or Waters are
+        # treated as being different even when the group would be considered
+        # the same.
         if self.diff_comp_classes:
-            # `classes` is a list because an atom group can be formed by multiple compounds, which can be from different
-            # (e.g., residue and ligand bound covalently) or same (e.g., amide groups formed by backbone residues) classes.
-            classes = sorted([CompoundClassIds[c.get_class().upper()].value for c in self.central_atm_grp.compounds])
+            # `classes` is a list because an atom group can be formed by
+            # multiple compounds, which can be from different (e.g., residue
+            # and ligand bound covalently) or same (e.g., amide groups formed
+            # by backbone residues) classes.
+            classes = sorted([CompoundClassIds[c.get_class().upper()].value
+                              for c in self.central_atm_grp.compounds])
 
             np_data = np.array(data, self.dtype)
             np_classes = np.array(classes, self.dtype)
 
             # Add padding to np_classes
             if np_data.shape[1] > np_classes.shape[0]:
                 np_classes = np.pad(np_classes, (0, (np_data.shape[1] - np_classes.shape[0])), 'constant', constant_values=PAD_DEFAULT)
@@ -767,52 +885,60 @@
             data = np.vstack((np_data, np_classes))
 
         return data
 
     def _encode_interactions(self):
         encoded_data = []
         for inter in self.interactions:
-            init_src_shell = self._manager.get_previous_shell(inter.src_grp, 1)
-            init_trgt_shell = self._manager.get_previous_shell(inter.trgt_grp, 1)
-            shell_ids = tuple(sorted([init_src_shell.identifier, init_trgt_shell.identifier]))
+            init_src_shell = \
+                self._manager.get_previous_shell(inter.src_grp, 1)
+            init_trgt_shell = \
+                self._manager.get_previous_shell(inter.trgt_grp, 1)
+            shell_ids = tuple(sorted([init_src_shell.identifier,
+                                      init_trgt_shell.identifier]))
             encoded_data.append((shell_ids, self.feature_mapper[inter.type]))
         return sorted(encoded_data)
 
     def __repr__(self):
         return ("<Shell: level=%d, radius=%f, center=%s, interactions=%d>"
-                % (self.level, self.radius, self.central_atm_grp, len(self.interactions)))
+                % (self.level, self.radius,
+                   self.central_atm_grp, len(self.interactions)))
 
 
 class ShellGenerator:
 
     """Generate shells, the base information of LUNA fingerprints.
 
     Parameters
     ----------
     num_levels : int
         The maximum number of iterations for fingerprint generation.
     radius_step : float
         The multiplier used to increase shell size at each iteration.
-        At iteration 0, shell radius is 0 * ``radius_step``, at iteration 1, radius is
-        1 * ``radius_step``, etc.
+        At iteration 0, shell radius is 0 * ``radius_step``, at iteration 1,
+        radius is 1 * ``radius_step``, etc.
     fp_length : int
-        The fingerprint length (total number of bits). The default value is :math:`2^{32}`.
+        The fingerprint length (total number of bits).
+        The default value is :math:`2^{32}`.
     ifp_type : :class:`~luna.interaction.fp.type.IFPType`
         The fingerprint type (EIFP, FIFP, or HIFP). The default value is EIFP.
     diff_comp_classes : bool
-        If True (the default), include differentiation between compound classes.
-        That means structural information originated from :class:`~luna.mol.groups.AtomGroup` objects
-        belonging to residues, nucleotides,  ligands, or water molecules will be considered different
-        even if their structural information are the same.
-        This is useful for example to differentiate protein-ligand interactions from residue-residue ones.
+        If True (the default), include differentiation between compound
+        classes. That means structural information originated from
+        :class:`~luna.mol.groups.AtomGroup` objects belonging to residues,
+        nucleotides,  ligands, or water molecules will be considered different
+        even if their structural information are the same. This is useful for
+        example to differentiate protein-ligand interactions from
+        residue-residue ones.
     dtype : data-type
-        Use arrays of type ``dtype`` to store information. The default value is np.int64.
+        Use arrays of type ``dtype`` to store information.
+        The default value is np.int64.
     seed : int
-        A seed to generate shell identifiers through the MurmurHash3 hash function.
-        The default value is 0.
+        A seed to generate shell identifiers through the MurmurHash3
+        hash function. The default value is 0.
     bucket_size : int
         Bucket size of KD tree.
         You can play around with this to optimize speed if you feel like it.
         The default value is 10.
 
     Attributes
     ----------
@@ -824,29 +950,32 @@
     dtype : data-type
     seed : int
     bucket_size : int
 
     Examples
     --------
 
-    In the below example, we will assume a LUNA project object named ``proj_obj`` already exists.
+    In the below example, we will assume a LUNA project object named
+    ``proj_obj`` already exists.
 
-    First, let's define a `ShellGenerator` object that will create shells over 2 iterations (levels).
-    At each iteration, the shell radius will be increased by 3 and substructural
-    information will be encoded following EIFP definition.
+    First, let's define a `ShellGenerator` object that will create shells over
+    2 iterations (levels). At each iteration, the shell radius will be
+    increased by 3 and substructural information will be encoded following EIFP
+    definition.
 
     >>> from luna.interaction.fp.shell import ShellGenerator
     >>> from luna.interaction.fp.type import IFPType
     >>> num_levels, radius_step = 2, 3
     >>> sg = ShellGenerator(num_levels, radius_step, ifp_type=IFPType.EIFP)
 
-    After defining the generator, we can create shells by calling :meth:`create_shells`, which
-    expects an :class:`~luna.mol.groups.AtomGroupsManager` object.
-    In this example, we will the first :class:`~luna.mol.groups.AtomGroupsManager` object
-    from an existing LUNA project (``proj_obj``).
+    After defining the generator, we can create shells by calling
+    :meth:`create_shells`, which expects an
+    :class:`~luna.mol.groups.AtomGroupsManager` object. In this example, we
+    will the first :class:`~luna.mol.groups.AtomGroupsManager` object from an
+    existing LUNA project (``proj_obj``).
 
     >>> atm_grps_mngr = list(proj_obj.atm_grps_mngrs)[0]
     >>> sm = sg.create_shells(atm_grps_mngr)
     >>> print(sm.num_shells)
     528
 
     Now, with shells stored in the `ShellManager` object you can, for instance:
@@ -862,51 +991,61 @@
               587  592  604  605  629  635  645  661  668  698  711  713  732  736
               740  753  764  795  813  815  820  824  825  831  836  855  873  882
               911  926  967  975  976  984  990  996 1020]
 
         * Visualize substructural information in Pymol\:
 
             >>> from luna.interaction.fp.view import ShellViewer
-            >>> shell_tuples = [(atm_grps_mngr.entry, sm.unique_shells, proj_obj.pdb_path)]
+            >>> shell_tuples = [(atm_grps_mngr.entry,
+            ...                  sm.unique_shells,
+            ...                  proj_obj.pdb_path)]
             >>> sv = ShellViewer()
             >>> sv.new_session(shell_tuples, "example.pse")
     """
-    def __init__(self, num_levels, radius_step, fp_length=DEFAULT_FP_LENGTH, ifp_type=IFPType.EIFP,
-                 diff_comp_classes=True, dtype=np.int64, seed=0, bucket_size=10):
+
+    def __init__(self, num_levels, radius_step,
+                 fp_length=DEFAULT_FP_LENGTH, ifp_type=IFPType.EIFP,
+                 diff_comp_classes=True, dtype=np.int64, seed=0,
+                 bucket_size=10):
 
         self.num_levels = num_levels
         self.radius_step = radius_step
         self.fp_length = fp_length
         self.ifp_type = ifp_type
         self.diff_comp_classes = diff_comp_classes
 
         self.seed = seed
         self.dtype = dtype
         self.bucket_size = bucket_size
 
     def create_shells(self, atm_grps_mngr):
-        """Perceive substructural information from :class:`~luna.mol.groups.AtomGroup` objects
-        and their interactions, and represent such information as shells.
+        """Perceive substructural information from
+        :class:`~luna.mol.groups.AtomGroup` objects and their interactions,
+        and represent such information as shells.
 
         Parameters
         ----------
         atm_grps_mngr : :class:`~luna.mol.groups.AtomGroupsManager`
-            Container of :class:`~luna.mol.groups.AtomGroup` objects and their interactions.
+            Container of :class:`~luna.mol.groups.AtomGroup` objects and their
+            interactions.
 
         Returns
         -------
          : `ShellManager`
 
         Raises
         ------
         ShellCenterNotFound
             If it fails to recover a shell having a given center.
         """
 
-        sm = ShellManager(self.num_levels, self.radius_step, self.fp_length, self.ifp_type)
+        sm = ShellManager(self.num_levels,
+                          self.radius_step,
+                          self.fp_length,
+                          self.ifp_type)
 
         all_interactions = atm_grps_mngr.get_all_interactions()
 
         neighborhood = set(atm_grps_mngr.atm_grps)
 
         # Create pseudo-groups for hydrophobic interactions.
         pseudo_grps = set(self._generate_pseudo_grps(atm_grps_mngr))
@@ -933,166 +1072,215 @@
 
         level = -1
         for level in range(self.num_levels):
             radius = self.radius_step * level
 
             for atm_grp in sorted_neighborhood:
 
-                # Ignore centroids that already reached the limit of possible substructures.
+                # Ignore centroids that already reached the limit of possible
+                # substructures.
                 if atm_grp in skip_atm_grps:
                     continue
 
-                # It stores all possible expansions each group can do. Each expansion is a derived group.
-                # Initially, the list contains only the groups derived from the central atom group.
-                # But, later it may also contain derived groups from interacting partner groups.
-                all_derived_atm_grps = self._get_derived_grps(atm_grp, pseudo_grps_mapping)
+                # It stores all possible expansions each group can do.
+                # Each expansion is a derived group. Initially, the list
+                # contains only the groups derived from the central atom
+                # group. But, later it may also contain derived groups
+                # from interacting partner groups.
+                all_derived_atm_grps = \
+                    self._get_derived_grps(atm_grp, pseudo_grps_mapping)
 
-                # In level 0, the number of unique derived groups is 0 as the shell initially only contains
-                # information of the centroid.
+                # In level 0, the number of unique derived groups is 0 as the
+                # shell initially only contains information of the centroid.
                 unique_derived_atm_grps = []
 
                 shell = None
 
                 if radius > 0:
                     prev_shell = sm.get_previous_shell(atm_grp, level)
                     if not prev_shell:
-                        logger.exception("No previous shell centered in %s was found." % atm_grp)
-                        raise ShellCenterNotFound("There are no shells initialized to the atom group '%s'." % atm_grp)
+                        error_msg = ("No previous shell centered in %s "
+                                     "was found." % atm_grp)
+                        logger.exception(error_msg)
+                        raise ShellCenterNotFound(error_msg)
 
                     prev_atm_grps = prev_shell.neighborhood
                     prev_interactions = prev_shell.interactions
 
                     nb_atm_grps = set(nbs.search(atm_grp.centroid, radius))
 
                     inter_tuples = set()
                     interactions_to_add = set()
 
                     # For each atom group from the previous shell.
                     for prev_atm_grp in sorted(prev_atm_grps):
-                        # Include the partner's derived groups to the set of all derived groups.
+                        # Include the partner's derived groups to the set of
+                        # all derived groups.
                         all_derived_atm_grps.update(self._get_derived_grps(prev_atm_grp, pseudo_grps_mapping))
 
                         for inter in prev_atm_grp.interactions:
-                            # Only PseudoAtomGroup objects should deal with hydrophobic interactions.
+                            # Only PseudoAtomGroup objects should deal with
+                            # hydrophobic interactions.
                             if isinstance(prev_atm_grp, PseudoAtomGroup) is False and inter.type == "Hydrophobic":
                                 continue
 
                             partner_grp = self._recover_partner_grp(prev_atm_grp, inter, pseudo_grps_mapping)
 
                             if partner_grp is not None:
                                 if inter not in interactions_to_add and partner_grp in nb_atm_grps:
                                     new_tuple = (inter, partner_grp)
 
-                                    # Ignore interactions that already exists in the previous shell to avoid duplications
-                                    # in the list of interactions. For example, without this control, an interaction I
-                                    # between atom A1 and A2 would appear twice in the list: (I, A1) and (I, A2).
-                                    # Thus, it keeps only the first interaction that appears while increasing the shell.
+                                    # Ignore interactions that already exists
+                                    # in the previous shell to avoid
+                                    # duplications in the list of interactions.
+                                    # For example, without this control, an
+                                    # interaction I between atom A1 and A2
+                                    # would appear twice in the list: (I, A1)
+                                    # and (I, A2). Thus, it keeps only the
+                                    # first interaction that appears while
+                                    # increasing the shell.
                                     if inter in prev_interactions and new_tuple not in prev_shell.inter_tuples:
                                         continue
 
                                     inter_tuples.add(new_tuple)
                                     interactions_to_add.add(inter)
 
-                    # Get valid derived groups, which are those ones inside the current sphere.
-                    valid_derived_atm_grps = set([ag for ag in all_derived_atm_grps if ag in nb_atm_grps])
+                    # Get valid derived groups, which are those ones inside the
+                    # current sphere.
+                    valid_derived_atm_grps = \
+                        set([ag for ag in all_derived_atm_grps
+                             if ag in nb_atm_grps])
 
-                    unique_derived_atm_grps = valid_derived_atm_grps - prev_atm_grps
+                    unique_derived_atm_grps = \
+                        valid_derived_atm_grps - prev_atm_grps
 
-                    # It adds a new shell only if there are new interactions and derived atom groups inside the shell.
+                    # It adds a new shell only if there are new interactions
+                    # and derived atom groups inside the shell.
                     shell_nb = set([x[1] for x in inter_tuples]) | valid_derived_atm_grps
                     shell_nb.add(atm_grp)
 
-                    shell = Shell(atm_grp, level, radius, neighborhood=shell_nb, inter_tuples=inter_tuples,
-                                  manager=sm, diff_comp_classes=self.diff_comp_classes,
+                    shell = Shell(atm_grp, level, radius,
+                                  neighborhood=shell_nb,
+                                  inter_tuples=inter_tuples,
+                                  manager=sm,
+                                  diff_comp_classes=self.diff_comp_classes,
                                   seed=self.seed, dtype=self.dtype)
                 else:
-                    shell = Shell(atm_grp, level, radius, manager=sm, diff_comp_classes=self.diff_comp_classes,
+                    shell = Shell(atm_grp, level, radius, manager=sm,
+                                  diff_comp_classes=self.diff_comp_classes,
                                   seed=self.seed, dtype=self.dtype)
 
                 if shell:
                     sm.add_shell(shell)
                     last_shell = shell
                 else:
                     last_shell = sm.get_last_shell(atm_grp)
 
-                # Evaluate if the limit of possible substructures for the current centroid (atom group) was reached.
+                # Evaluate if the limit of possible substructures for the
+                # current centroid (atom group) was reached.
                 if last_shell:
-                    # The limit will be reached when the last shell already contains all interactions
-                    # established by the atom groups inside the shell. In this case, expanding the radius
-                    # will not result in any new shell because a shell is only created when the atoms inside
-                    # the last shell establish interactions with the atom groups found after increasing the radius.
+                    # The limit will be reached when the last shell already
+                    # contains all interactions established by the atom
+                    # groups inside the shell. In this case, expanding the
+                    # radius will not result in any new shell because a shell
+                    # is only created when the atoms inside the last shell
+                    # establish interactions with the atom groups found after
+                    # increasing the radius.
                     all_nb_interactions = set(chain.from_iterable([g.interactions for g in last_shell.neighborhood]))
-                    # It considers only interactions whose atom groups exist in the neighborhood.
+                    # It considers only interactions whose atom groups exist in
+                    # the neighborhood.
                     valid_interactions = set([i for i in all_nb_interactions if i.src_grp in neighborhood and i.trgt_grp in neighborhood])
 
-                    # It identifies if the convergence for the interactions was reached.
+                    # It identifies if the convergence for the interactions
+                    # was reached.
                     interactions_converged = valid_interactions == last_shell.interactions
 
-                    # It identifies if the convergence for the expansion of atom groups was reached, which happens when all derived groups
-                    # were already included in the centroid neighborhood. However, it may happen that this requirement was fulfilled
-                    # by the time new unique derived groups were included in the centroid neighborhood. Thus, the second test provides
-                    # a chance to all of these recently discovered groups to expand.
+                    # It identifies if the convergence for the expansion of
+                    # atom groups was reached, which happens when all derived
+                    # groups were already included in the centroid
+                    # neighborhood. However, it may happen that this
+                    # requirement was fulfilled by the time new unique derived
+                    # groups were included in the centroid neighborhood.
+                    # Thus, the second test provides a chance to all of these
+                    # recently discovered groups to expand.
                     grp_expansions_converged = all_derived_atm_grps == last_shell.neighborhood and len(unique_derived_atm_grps) == 0
 
-                    # The local convergence is reached when no atom group inside the current sphere can expand or all of its interactions
-                    # were already included to the sphere.
-                    local_convergence = interactions_converged and grp_expansions_converged
-                    # The global convergence occurs when all interactions in the binding site were already included in the sphere.
-                    global_convergence = all_interactions == last_shell.interactions
+                    # The local convergence is reached when no atom group
+                    # inside the current sphere can expand or all of its
+                    # interactions were already included to the sphere.
+                    local_convergence = \
+                        interactions_converged and grp_expansions_converged
+                    # The global convergence occurs when all interactions in
+                    # the binding site were already included in the sphere.
+                    global_convergence = \
+                        all_interactions == last_shell.interactions
 
-                    # If the limit was reached for this centroid, in the next level it can be ignored.
+                    # If the limit was reached for this centroid, in the next
+                    # level it can be ignored.
                     if local_convergence or global_convergence:
                         skip_atm_grps.add(atm_grp)
 
-            # If all atom groups reached the limit of possible substructures, just leave the loop.
+            # If all atom groups reached the limit of possible substructures,
+            # just leave the loop.
             if len(skip_atm_grps) == len(neighborhood):
-                logger.debug("The list of shells cannot be expanded anymore. The maximum number "
-                             "of substructures were reached.")
+                logger.debug("The list of shells cannot be expanded anymore. "
+                             "The maximum number of substructures were "
+                             "reached.")
                 break
 
         logger.debug("Shells creation finished.")
         logger.debug("The last level executed was: %d." % level)
         logger.debug("The number of levels defined was: %d." % self.num_levels)
         logger.debug("Total number of shells created: %d" % sm.num_shells)
-        logger.debug("Total number of unique shells created: %d" % sm.num_unique_shells)
+        logger.debug("Total number of unique shells created: %d"
+                     % sm.num_unique_shells)
 
         return sm
 
     def _generate_pseudo_grps(self, atm_grps_mngr):
         pseudo_grps = {}
         mapped_interactions = set()
 
         for hydrop_grp in atm_grps_mngr.filter_by_types(["Hydrophobe"]):
             for inter in hydrop_grp.interactions:
 
-                # Ignore non-hydrophobic interactions or interactions already mapped.
+                # Ignore non-hydrophobic interactions or interactions already
+                # mapped.
                 if inter.type != "Hydrophobic" or inter in mapped_interactions:
                     continue
 
                 src_tuple = (inter.src_grp, tuple(sorted(inter.src_interacting_atms)))
                 trgt_tuple = (inter.trgt_grp, tuple(sorted(inter.trgt_interacting_atms)))
 
                 for atm_grp, atms in [src_tuple, trgt_tuple]:
-                    # It will get a pseudo-group already created or create a new one.
-                    pseudo_grp = pseudo_grps.get(atms, PseudoAtomGroup(atm_grp, atms, [ChemicalFeature("Hydrophobe")]))
+                    # It will get a pseudo-group already created or create
+                    # a new one.
+                    feats = [ChemicalFeature("Hydrophobe")]
+                    pseudo_grp = \
+                        pseudo_grps.get(atms,
+                                        PseudoAtomGroup(atm_grp, atms, feats))
 
                     pseudo_grp.add_interactions([inter])
 
                     pseudo_grps[atms] = pseudo_grp
 
                 mapped_interactions.add(inter)
 
         return pseudo_grps.values()
 
     def _get_derived_grps(self, atm_grp, pseudo_grps_mapping):
         # Get derived groups for the informed atom group.
-        derived_atm_grps = set([ag for a in atm_grp.atoms for ag in a.atm_grps])
+        derived_atm_grps = set([ag
+                                for a in atm_grp.atoms
+                                for ag in a.atm_grps])
 
         # Get derived pseudo-groups for the informed atom group.
-        derived_atm_grps.update(set([pseudo_grp for a in atm_grp.atoms for pseudo_grp in pseudo_grps_mapping.get((a,), [])]))
+        derived_atm_grps.update(set([pseudo_grp
+                                     for a in atm_grp.atoms
+                                     for pseudo_grp in pseudo_grps_mapping.get((a,), [])]))
 
         return derived_atm_grps
 
     def _recover_partner_grp(self, atm_grp, interaction, pseudo_grps_mapping):
         if isinstance(atm_grp, PseudoAtomGroup):
             atoms = sorted(atm_grp.atoms)
 
@@ -1103,17 +1291,19 @@
                 partner_atms = trgt_atms
             elif atoms == trgt_atms:
                 partner_atms = src_atms
             else:
                 return None
 
             partner_grp = None
-            # Recover the partner groups based on the interacting atoms. Then, it will check which returned
-            # pseudo-group corresponds to the interacting atoms, i.e., the one that contains exactly the same atoms.
-            # This verification is mainly necessary for pseudo-groups composed only by one atom as such groups tend
+            # Recover the partner groups based on the interacting atoms.
+            # Then, it will check which returned pseudo-group corresponds to
+            # the interacting atoms, i.e., the one that contains exactly the
+            # same atoms. This verification is mainly necessary for
+            # pseudo-groups composed only by one atom as such groups tend
             # to belong to more than one pseudo-group.
             for pseudo_grp in pseudo_grps_mapping.get(tuple(partner_atms), []):
                 if sorted(pseudo_grp.atoms) == partner_atms:
                     partner_grp = pseudo_grp
                     break
 
             return partner_grp
```

### Comparing `luna-0.12.2/luna/interaction/fp/view.py` & `luna-0.13.0/luna/interaction/fp/view.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,29 +40,29 @@
     >>> from luna.interaction.fp.type import IFPType
     >>> num_levels, radius_step = 2, 3
     >>> sg = ShellGenerator(num_levels, radius_step, ifp_type=IFPType.EIFP)
     >>> atm_grps_mngr = list(proj_obj.atm_grps_mngrs)[0]
     >>> sm = sg.create_shells(atm_grps_mngr)
 
     The function
-    :meth:`~luna.interaction.fp.shell.ShellGenerator.create_shells`
-    returns a :class:`~luna.interaction.fp.shell.ShellManager` object, which
-    provides built-in methods to access the created shells. Therefore, you can
-    interact with it to select the shells you want to visualize in Pymol.
-    As an example, let's select all unique shells at the last level:
+    :meth:`~luna.interaction.fp.shell.ShellGenerator.create_shells` returns a
+    :class:`~luna.interaction.fp.shell.ShellManager` object, which provides
+    built-in methods to access the created shells. Therefore, you can interact
+    with it to select the shells you want to visualize in Pymol. As an example,
+    let's select all unique shells at the last level:
 
     >>> shells = sm.get_shells_by_level(num_levels - 1, unique_shells=True)
 
     .. note::
         Levels are 0-indexed. So, the first level is 0, second is 1, etc.
         That means if ``num_levels`` is 5, the last level will be 4.
 
-    As `ShellViewer` expects a list of tuples, we will define it now.
-    The first item of the tuple is the :class:`~luna.mol.entry.Entry` instance,
-    which represents a ligand. This can be obtained directly from the
+    As `ShellViewer` expects a list of tuples, we will define it now. The first
+    item of the tuple is the :class:`~luna.mol.entry.Entry` instance, which
+    represents a ligand. This can be obtained directly from the
     :class:`~luna.mol.groups.AtomGroupsManager` object. The second item is the
     list of shells you want to visualize. Finally, the third item can be either
     a PDB file or a directory. In this example, we will use the PDB directory
     defined during the LUNA project initialization.
 
     >>> shell_tuples = [(atm_grps_mngr.entry, shells, proj_obj.pdb_path)]
 
@@ -73,24 +73,24 @@
 
     >>> from luna.interaction.fp.view import ShellViewer
     >>> sv = ShellViewer()
     >>> sv.new_session(shell_tuples, "example.pse")
     """
 
     def set_view(self, shell_tuples):
-        """Depict shells (IFP features) and interactions into the
-        current Pymol session.
+        """Depict shells (IFP features) and interactions into the current
+        Pymol session.
 
         Parameters
         ----------
         shell_tuples : iterable of tuple
             Each tuple must contain three items: an
-            :class:`~luna.mol.entry.Entry` instance, an iterable of
-            :class:`~luna.interaction.fp.shell.Shell`, and a PDB
-            file or the directory where the PDB file is located.
+            :class:`~luna.mol.entry.Entry` instance,
+            an iterable of :class:`~luna.interaction.fp.shell.Shell`,
+            and a PDB file or the directory where the PDB file is located.
         """
 
         if not isinstance(self.wrapper, PymolWrapper):
             raise PymolSessionNotInitialized("No session was initialized.")
 
         for target_entry, shells, pathname in shell_tuples:
 
@@ -111,35 +111,35 @@
             residue_selections = set()
             for index, shell in enumerate(shells):
                 sphere_obj = ("%s.spheres.s%d_lvl%d_center%d"
                               % (main_grp, index, shell.level,
                                  hash(shell.central_atm_grp)))
                 centroid_obj = "%s.centroid" % (sphere_obj)
 
-                centroid_coords = shell.central_atm_grp.centroid
+                centroids = list(shell.central_atm_grp.centroid)
                 self.wrapper.add_pseudoatom(centroid_obj,
                                             {"color": "white",
-                                             "pos": list(centroid_coords)})
-
+                                             "pos": centroids})
                 self.wrapper.hide([("nonbonded", centroid_obj)])
                 self.wrapper.show([("spheres", centroid_obj),
                                    ("nb_spheres", centroid_obj),
                                    ("dots", centroid_obj)])
                 self.wrapper.set("dot_color", "red")
-                self.wrapper.set("sphere_scale", shell.radius,
+                self.wrapper.set("sphere_scale",
+                                 shell.radius,
                                  {"selection": centroid_obj})
                 self.wrapper.set("sphere_transparency", 0.85,
                                  {"selection": centroid_obj})
                 self.wrapper.run_cmds([("center",
                                         {"selection": centroid_obj})])
 
-                atoms = shell.central_atm_grp.atoms
-                labels = [(centroid_obj,
-                           '"%s"' % "+".join([a.name for a in sorted(atoms)]))]
-                self.wrapper.label(labels)
+                atm_names = [a.name
+                             for a in sorted(shell.central_atm_grp.atoms)]
+                self.wrapper.label([(centroid_obj,
+                                     '"%s"' % "+".join(atm_names))])
 
                 # Add interactions and styles.
                 interacting_residue_sels = \
                     self.set_interactions_view(shell.interactions,
                                                main_grp, sphere_obj)
 
                 residue_selections.update(interacting_residue_sels)
```

### Comparing `luna-0.12.2/luna/interaction/type.py` & `luna-0.13.0/luna/interaction/type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,177 +1,238 @@
 import numpy as np
 
 from luna.util.math import atom_coordinates, centroid
 from luna.util.default_values import PYMOL_INTERACTION_COLOR_AS_RGB
 from luna.util import rgb2hex
 
 
-NUCLEOPHILE_INTERS = ["Orthogonal multipolar", "Parallel multipolar", "Antiparallel multipolar", "Tilted multipolar", "Multipolar",
-                      "Cation-nucleophile", "Unfavorable anion-nucleophile", "Unfavorable nucleophile-nucleophile"]
-
-ELECTROPHILE_INTERS = ["Orthogonal multipolar", "Parallel multipolar", "Antiparallel multipolar", "Tilted multipolar", "Multipolar",
-                       "Anion-electrophile", "Unfavorable cation-electrophile", "Unfavorable electrophile-electrophile"]
-
-UNFAVORABLE_INTERS = ["Repulsive", "Unfavorable anion-nucleophile", "Unfavorable cation-electrophile",
-                      "Unfavorable nucleophile-nucleophile", "Unfavorable electrophile-electrophile"]
+NUCLEOPHILE_INTERS = ["Orthogonal multipolar", "Parallel multipolar",
+                      "Antiparallel multipolar", "Tilted multipolar",
+                      "Multipolar", "Cation-nucleophile",
+                      "Unfavorable anion-nucleophile",
+                      "Unfavorable nucleophile-nucleophile"]
+
+ELECTROPHILE_INTERS = ["Orthogonal multipolar", "Parallel multipolar",
+                       "Antiparallel multipolar", "Tilted multipolar",
+                       "Multipolar", "Anion-electrophile",
+                       "Unfavorable cation-electrophile",
+                       "Unfavorable electrophile-electrophile"]
+
+UNFAVORABLE_INTERS = ["Repulsive",
+                      "Unfavorable anion-nucleophile",
+                      "Unfavorable cation-electrophile",
+                      "Unfavorable nucleophile-nucleophile",
+                      "Unfavorable electrophile-electrophile"]
 
 
 class InteractionType:
     """Define an interaction type.
 
     Parameters
     ----------
     src_grp : :class:`~luna.mol.groups.AtomGroup`
         The interaction’s first atom or atom group.
         For directional interactions such as hydrogen bonds, ``src_grp``
-        represents donor atoms and atom groups that act as nucleophiles, i.e., from where the interaction "comes from".
+        represents donor atoms and atom groups that act as nucleophiles, i.e.,
+        from where the interaction "comes from".
     trgt_grp : :class:`~luna.mol.groups.AtomGroup`
         The interaction’s second atom or atom group.
         For directional interactions such as hydrogen bonds, ``trgt_grp``
-        represents acceptor atoms and atom groups that act as electrophiles, i.e., the interaction "receiver".
+        represents acceptor atoms and atom groups that act as electrophiles,
+        i.e., the interaction "receiver".
     inter_type : str
         The interaction type.
-    src_interacting_atms : iterable of :class:`~luna.mol.atom.ExtendedAtom`, optional
-        If provided, represent the set of atoms from ``src_grp`` that in fact participate in the interaction.
-        For example, in hydrophobic islands, not all of their atoms are in direct contact with another hydrophobic surface.
-    trgt_interacting_atms : iterable of :class:`~luna.mol.atom.ExtendedAtom`, optional
-        If provided, represent the set of atoms from ``trgt_grp`` that in fact participate in the interaction.
-        For example, in hydrophobic islands, not all of their atoms are in direct contact with another hydrophobic surface.
+    src_interacting_atms : iterable of :class:`~luna.mol.atom.ExtendedAtom`, \
+            optional
+        If provided, represent the set of atoms from ``src_grp`` that in fact
+        participate in the interaction. For example, in hydrophobic islands,
+        not all of their atoms are in direct contact with another hydrophobic
+        surface.
+    trgt_interacting_atms : iterable of :class:`~luna.mol.atom.ExtendedAtom`, \
+            optional
+        If provided, represent the set of atoms from ``trgt_grp`` that in fact
+        participate in the interaction. For example, in hydrophobic islands,
+        not all of their atoms are in direct contact with another hydrophobic
+        surface.
     src_centroid : array_like of float (size 3), optional
         Atomic coordinates (x, y, z) of the centroid of ``src_grp``.
-        If not provided, it will be calculated automatically from ``src_grp`` or ``src_interacting_atms``.
+        If not provided, it will be calculated automatically from ``src_grp``
+        or ``src_interacting_atms``.
     trgt_centroid : array_like of float (size 3), optional
         Atomic coordinates (x, y, z) of the centroid of ``trgt_grp``.
-        If not provided, it will be calculated automatically from ``trgt_grp`` or ``trgt_interacting_atms``.
+        If not provided, it will be calculated automatically from ``trgt_grp``
+        or ``trgt_interacting_atms``.
     directional : bool
-        Indicate if the interaction has a direction as in hydrogen bonds and multipolar interactions.
+        Indicate if the interaction has a direction as in hydrogen bonds and
+        multipolar interactions.
     params : dict, optional
         Interaction parameters (distances, angles, etc).
     """
 
-    def __init__(self, src_grp, trgt_grp, inter_type, src_interacting_atms=None, trgt_interacting_atms=None,
-                 src_centroid=None, trgt_centroid=None, directional=False, params=None):
+    def __init__(self,
+                 src_grp,
+                 trgt_grp,
+                 inter_type,
+                 src_interacting_atms=None,
+                 trgt_interacting_atms=None,
+                 src_centroid=None,
+                 trgt_centroid=None,
+                 directional=False,
+                 params=None):
 
         self._src_grp = src_grp
         self._trgt_grp = trgt_grp
 
         src_interacting_atms = src_interacting_atms or []
         self._src_interacting_atms = list(src_interacting_atms)
 
         trgt_interacting_atms = trgt_interacting_atms or []
         self._trgt_interacting_atms = list(trgt_interacting_atms)
 
-        self._src_centroid = np.array(src_centroid) if src_centroid is not None else None
-        self._trgt_centroid = np.array(trgt_centroid) if trgt_centroid is not None else None
+        self._src_centroid = (np.array(src_centroid)
+                              if src_centroid is not None else None)
+        self._trgt_centroid = (np.array(trgt_centroid)
+                               if trgt_centroid is not None else None)
 
         self._type = inter_type
         self.directional = directional
         self._params = params or {}
         self._hash_cache = None
 
         self._apply_refs()
         self._expand_dict()
 
     @property
     def src_grp(self):
-        """:class:`~luna.mol.groups.AtomGroup`: The interaction’s first atom or atom group."""
+        """:class:`~luna.mol.groups.AtomGroup`: The interaction’s first \
+                atom or atom group."""
         return self._src_grp
 
     @src_grp.setter
     def src_grp(self, atm_grp):
         self._src_grp = atm_grp
 
         # Reset hash.
         self._hash_cache = None
         self._apply_refs()
 
     @property
     def trgt_grp(self):
-        """:class:`~luna.mol.groups.AtomGroup`: The interaction’s second atom or atom group."""
+        """:class:`~luna.mol.groups.AtomGroup`: The interaction’s second atom \
+                or atom group."""
         return self._trgt_grp
 
     @trgt_grp.setter
     def trgt_grp(self, atm_grp):
         self._trgt_grp = atm_grp
 
         # Reset hash.
         self._hash_cache = None
         self._apply_refs()
 
     @property
     def src_interacting_atms(self):
-        """iterable of :class:`~luna.mol.atom.ExtendedAtom`: The set of atoms from ``src_grp`` that in fact
-        participate in the interaction. If a sequence of atoms is not provided during the initialization of this class,
-        then all atoms from ``src_grp`` are returned."""
+        """iterable of :class:`~luna.mol.atom.ExtendedAtom`: The set of atoms \
+            from ``src_grp`` that in fact participate in the interaction. \
+            If a sequence of atoms is not provided during the initialization \
+            of this class, then all atoms from ``src_grp`` are returned."""
         return self._src_interacting_atms or self.src_grp.atoms
 
     @property
     def trgt_interacting_atms(self):
-        """iterable of :class:`~luna.mol.atom.ExtendedAtom`: The set of atoms from ``trgt_grp`` that in fact
-        participate in the interaction. If a sequence of atoms is not provided during the initialization of this class,
-        then all atoms from ``trgt_grp`` are returned."""
+        """iterable of :class:`~luna.mol.atom.ExtendedAtom`: The set of atoms \
+            from ``trgt_grp`` that in fact participate in the interaction. \
+            If a sequence of atoms is not provided during the initialization \
+            of this class, then all atoms from ``trgt_grp`` are returned."""
         return self._trgt_interacting_atms or self.trgt_grp.atoms
 
     @property
     def src_centroid(self):
-        """array_like of float (size 3): Atomic coordinates (x, y, z) of the centroid of ``src_grp``.
-        If it is not provided during the initialization of this class, then it will be calculated
+        """array_like of float (size 3): Atomic coordinates (x, y, z) of the \
+        centroid of ``src_grp``. If it is not provided during the \
+        initialization of this class, then it will be calculated \
         automatically from ``src_grp`` or ``src_interacting_atms``.
         """
         if self._src_centroid is None:
             if self._src_interacting_atms:
-                self._src_centroid = centroid(atom_coordinates(self._src_interacting_atms))
+                self._src_centroid = \
+                    centroid(atom_coordinates(self._src_interacting_atms))
             else:
                 src_centroid = self._src_grp.centroid
-                # Define the centroid in a nucleophile with two atoms as the position of its more electronegative atom.
-                # Remember that the position in the interaction object matters. We have defined that the first group is always
-                # the nucleophile for both dipole-dipole and ion-dipole interactions.
-                if self.type in NUCLEOPHILE_INTERS and len(self.src_grp.atoms) == 2:
-                    dipole_atm = self.src_grp.atoms[0] if (self.src_grp.atoms[0].electronegativity
-                                                           > self.src_grp.atoms[1].electronegativity) else self.src_grp.atoms[1]
+                # Define the centroid in a nucleophile with two atoms as the
+                # position of its more electronegative atom. Remember that the
+                # position in the interaction object matters. We have defined
+                # that the first group is always the nucleophile for both
+                # dipole-dipole and ion-dipole interactions.
+                if (self.type in NUCLEOPHILE_INTERS
+                        and len(self.src_grp.atoms) == 2):
+                    dipole_atm = \
+                        (self.src_grp.atoms[0]
+                         if (self.src_grp.atoms[0].electronegativity
+                             > self.src_grp.atoms[1].electronegativity)
+                         else self.src_grp.atoms[1])
                     src_centroid = dipole_atm.coord
-                # For unfavorable multipolar interactions, it may happen that the first atom group is an electrophile as well.
-                elif self.type == "Unfavorable electrophile-electrophile" and len(self.src_grp.atoms) == 2:
-                    dipole_atm = self.src_grp.atoms[0] if (self.src_grp.atoms[0].electronegativity
-                                                           < self.src_grp.atoms[1].electronegativity) else self.src_grp.atoms[1]
+
+                # For unfavorable multipolar interactions, it may happen that
+                # the first atom group is an electrophile as well.
+                elif (self.type == "Unfavorable electrophile-electrophile"
+                        and len(self.src_grp.atoms) == 2):
+                    dipole_atm = \
+                        (self.src_grp.atoms[0]
+                         if (self.src_grp.atoms[0].electronegativity
+                             < self.src_grp.atoms[1].electronegativity)
+                         else self.src_grp.atoms[1])
                     src_centroid = dipole_atm.coord
 
                 self._src_centroid = src_centroid
         return self._src_centroid
 
     @src_centroid.setter
     def src_centroid(self, centroid):
         if centroid is None:
             self._src_centroid = None
         else:
             self._src_centroid = np.array(centroid)
 
     @property
     def trgt_centroid(self):
-        """array_like of float (size 3): Atomic coordinates (x, y, z) of the centroid of ``trgt_grp``.
-        If it is not provided during the initialization of this class, then it will be calculated
+        """array_like of float (size 3): Atomic coordinates (x, y, z) of the \
+        centroid of ``trgt_grp``. If it is not provided during the \
+        initialization of this class, then it will be calculated \
         automatically from ``trgt_grp`` or ``trgt_interacting_atms``.
         """
         if self._trgt_centroid is None:
             if self._trgt_interacting_atms:
-                self._trgt_centroid = centroid(atom_coordinates(self._trgt_interacting_atms))
+                self._trgt_centroid = \
+                    centroid(atom_coordinates(self._trgt_interacting_atms))
             else:
                 trgt_centroid = self._trgt_grp.centroid
 
-                # Define the centroid in an electrophile with two atoms as the position of its less electronegative atom.
-                # Remember that the position in the interaction object matters. We have defined that the second group is always
-                # the electrophile for both dipole-dipole and ion-dipole interactions.
-                if self.type in ELECTROPHILE_INTERS and len(self.trgt_grp.atoms) == 2:
-                    dipole_atm = self.trgt_grp.atoms[0] if (self.trgt_grp.atoms[0].electronegativity
-                                                            < self.trgt_grp.atoms[1].electronegativity) else self.trgt_grp.atoms[1]
+                # Define the centroid in an electrophile with two atoms as the
+                # position of its less electronegative atom. Remember that the
+                # position in the interaction object matters. We have defined
+                # that the second group is always the electrophile for both
+                # dipole-dipole and ion-dipole interactions.
+                if (self.type in ELECTROPHILE_INTERS
+                        and len(self.trgt_grp.atoms) == 2):
+                    dipole_atm = \
+                        (self.trgt_grp.atoms[0]
+                         if (self.trgt_grp.atoms[0].electronegativity
+                             < self.trgt_grp.atoms[1].electronegativity)
+                         else self.trgt_grp.atoms[1])
                     trgt_centroid = dipole_atm.coord
-                # For unfavorable multipolar interactions, it may happen that the second atom group is a nucleophile as well.
-                elif self.type == "Unfavorable nucleophile-nucleophile" and len(self.trgt_grp.atoms) == 2:
-                    dipole_atm = self.trgt_grp.atoms[0] if (self.trgt_grp.atoms[0].electronegativity
-                                                            > self.trgt_grp.atoms[1].electronegativity) else self.trgt_grp.atoms[1]
+                # For unfavorable multipolar interactions, it may happen that
+                # the second atom group is a nucleophile as well.
+                elif (self.type == "Unfavorable nucleophile-nucleophile"
+                        and len(self.trgt_grp.atoms) == 2):
+                    dipole_atm = \
+                        (self.trgt_grp.atoms[0]
+                         if (self.trgt_grp.atoms[0].electronegativity
+                             > self.trgt_grp.atoms[1].electronegativity)
+                         else self.trgt_grp.atoms[1])
                     trgt_centroid = dipole_atm.coord
 
                 self._trgt_centroid = trgt_centroid
         return self._trgt_centroid
 
     @trgt_centroid.setter
     def trgt_centroid(self, centroid):
@@ -195,28 +256,31 @@
     @property
     def params(self):
         """dict: Interaction parameters (distances, angles, etc)."""
         return self._params
 
     @property
     def required_interactions(self):
-        """list of `InteractionType`: If this interaction depends on other interactions, then return them as a list.
-        Currently, by default, only water-bridged hydrogen bonds and salt bridges have a dependency on
-        other interactions. The first, depends on two or more hydrogen bonds, while the second depends on
-        an ionic and a hydrogen bond."""
+        """list of `InteractionType`: If this interaction depends on other \
+        interactions, then return them as a list. Currently, by default, \
+        only water-bridged hydrogen bonds and salt bridges have a dependency \
+        on other interactions. The first, depends on two or more \
+        hydrogen bonds, while the second depends on an ionic and a \
+        hydrogen bond."""
 
         interactions = []
         if "depends_on" in self._params:
             interactions = self._params["depends_on"]
 
         return interactions
 
     def get_partner(self, comp):
-        """Get the partner atom group that forms this interaction with ``comp``. \
-        Return None if ``comp`` is neither the ``src_grp`` nor ``trgt_grp``.
+        """Get the partner atom group that forms this interaction with
+        ``comp``. Return None if ``comp`` is neither the ``src_grp``
+        nor ``trgt_grp``.
 
         Parameters
         ----------
         comp : :class:`~luna.mol.groups.AtomGroup`
             Get the partner of this atom group.
 
         Returns
@@ -226,15 +290,16 @@
         if comp == self.src_grp:
             return self.trgt_grp
         elif comp == self.trgt_grp:
             return self.src_grp
         return None
 
     def is_directional(self):
-        """Indicate if the interaction has a direction as in hydrogen bonds and multipolar interactions.
+        """Indicate if the interaction has a direction as in hydrogen bonds
+        and multipolar interactions.
 
         Returns
         -------
          : bool
         """
         return self.directional
 
@@ -257,56 +322,65 @@
          : bool
         """
         return not self.is_intramol_interaction()
 
     def _show_src_centroid(self):
         show_centroid = True
 
-        # Define the centroid in a nucleophile with two atoms as the position of its more electronegative atom.
-        # Remember that the position in the interaction object matters. We have defined that the first group is always
-        # the nucleophile for both dipole-dipole and ion-dipole interactions.
+        # Define the centroid in a nucleophile with two atoms as the position
+        # of its more electronegative atom. Remember that the position in the
+        # interaction object matters. We have defined that the first group is
+        # always the nucleophile for both dipole-dipole and ion-dipole
+        # interactions.
         if self.type in NUCLEOPHILE_INTERS and len(self.src_grp.atoms) == 2:
             show_centroid = False
-        # For unfavorable multipolar interactions, it may happen that the first atom group is an electrophile as well.
-        elif self.type == "Unfavorable electrophile-electrophile" and len(self.src_grp.atoms) == 2:
+        # For unfavorable multipolar interactions, it may happen that the
+        # first atom group is an electrophile as well.
+        elif (self.type == "Unfavorable electrophile-electrophile"
+                and len(self.src_grp.atoms) == 2):
             show_centroid = False
 
         return show_centroid
 
     def _show_trgt_centroid(self):
         show_centroid = True
 
-        # Define the centroid in an electrophile with two atoms as the position of its less electronegative atom.
-        # Remember that the position in the interaction object matters. We have defined that the second group is always
-        # the electrophile for both dipole-dipole and ion-dipole interactions.
+        # Define the centroid in an electrophile with two atoms as the position
+        # of its less electronegative atom. Remember that the position in the
+        # interaction object matters. We have defined that the second group is
+        # always the electrophile for both dipole-dipole and ion-dipole
+        # interactions.
         if self.type in ELECTROPHILE_INTERS and len(self.trgt_grp.atoms) == 2:
             show_centroid = False
-        # For unfavorable multipolar interactions, it may happen that the second atom group is a nucleophile as well.
-        elif self.type == "Unfavorable nucleophile-nucleophile" and len(self.trgt_grp.atoms) == 2:
+        # For unfavorable multipolar interactions, it may happen that the
+        # second atom group is a nucleophile as well.
+        elif (self.type == "Unfavorable nucleophile-nucleophile"
+                and len(self.trgt_grp.atoms) == 2):
             show_centroid = False
 
         return show_centroid
 
     def _apply_refs(self):
         self.src_grp.add_interactions([self])
         self.trgt_grp.add_interactions([self])
 
     def clear_refs(self):
-        """References to this `InteractionType` instance will be removed from the list of interactions of
-        ``src_grp`` and ``trgt_grp``."""
+        """References to this `InteractionType` instance will be removed from
+        the list of interactions of ``src_grp`` and ``trgt_grp``."""
         self.src_grp.remove_interactions([self])
         self.trgt_grp.remove_interactions([self])
 
     def _expand_dict(self):
         for key in self._params:
             self.__dict__[key] = self._params[key]
 
     def as_json(self):
-        """Represent this interaction as a dict containing the interaction type, flags indicating if
-        its directional or not and if it is an intra- or intermolecular interaction, its default color for visual
+        """Represent this interaction as a dict containing the interaction
+        type, flags indicating if its directional or not and if it is an
+        intra- or intermolecular interaction, its default color for visual
         representations, and information related to each involved atom group.
 
         The dict is defined as follows:
             * ``type`` (str): the interaction type;
             * ``is_directional`` (bool`): if it is a directional interaction;
             * ``is_intramol_interaction`` (bool`): if it is an intramolecular interaction;
             * ``is_intermol_interaction`` (bool`): if it is an intermolecular interaction;
@@ -325,76 +399,87 @@
         """
         inter_obj = {}
         inter_obj["type"] = self.type
 
         inter_obj["is_directional"] = self.is_directional()
         inter_obj["is_intramol_interaction"] = self.is_intramol_interaction()
         inter_obj["is_intermol_interaction"] = self.is_intermol_interaction()
+
         inter_obj["color"] = rgb2hex(*PYMOL_INTERACTION_COLOR_AS_RGB.get_unnormalized_color(self.type))
 
         src_grp_obj = self.src_grp.as_json()
         src_grp_obj["add_pseudo_group"] = len(self.src_grp.atoms) > 1
         src_grp_obj["centroid"] = self.src_centroid.tolist()
         src_grp_obj["show_centroid"] = self._show_src_centroid()
 
         if src_grp_obj["add_pseudo_group"]:
-            src_grp_obj["pseudo_group_name"] = "+".join([a.name for a in sorted(self.src_grp.atoms)])
+            src_grp_obj["pseudo_group_name"] = \
+                "+".join([a.name for a in sorted(self.src_grp.atoms)])
 
         inter_obj["src_grp"] = src_grp_obj
 
         #
         # Target atom group
         #
         trgt_grp_obj = self.trgt_grp.as_json()
         trgt_grp_obj["add_pseudo_group"] = len(self.trgt_grp.atoms) > 1
         trgt_grp_obj["centroid"] = self.trgt_centroid.tolist()
         trgt_grp_obj["show_centroid"] = self._show_trgt_centroid()
 
         if trgt_grp_obj["add_pseudo_group"]:
-            trgt_grp_obj["pseudo_group_name"] = "+".join([a.name for a in sorted(self.trgt_grp.atoms)])
+            trgt_grp_obj["pseudo_group_name"] = \
+                "+".join([a.name for a in sorted(self.trgt_grp.atoms)])
 
         inter_obj["trgt_grp"] = trgt_grp_obj
 
         return inter_obj
 
     def __eq__(self, other):
         """Overrides the default implementation"""
         if isinstance(self, other.__class__):
-            is_equal_compounds = ((self.src_grp == other.src_grp and self.trgt_grp == other.trgt_grp)
-                                  or (self.src_grp == other.trgt_grp and self.trgt_grp == other.src_grp))
+            is_equal_compounds = ((self.src_grp == other.src_grp
+                                   and self.trgt_grp == other.trgt_grp)
+                                  or (self.src_grp == other.trgt_grp
+                                      and self.trgt_grp == other.src_grp))
 
             is_equal_interactions = self.type == other.type
             has_equal_params = self.params == other.params
 
-            return is_equal_compounds and is_equal_interactions and has_equal_params
+            return (is_equal_compounds and is_equal_interactions
+                    and has_equal_params)
         return False
 
     def __ne__(self, other):
         """Overrides the default implementation"""
         return not self.__eq__(other)
 
     def __hash__(self):
         """Overrides the default implementation"""
 
         if self._hash_cache is None:
             # First, it flats the dictionary by transforming it to a list.
-            # Then, it transforms the list into an immutable data structure (tuple).
+            # Then, it transforms the list into an immutable data structure
+            # (tuple).
             params_values = []
             for key in sorted(self.params):
                 if type(self.params[key]) is list:
                     val = tuple(self.params[key])
                 else:
                     val = self.params[key]
                 params_values.append(val)
             params_as_tuple = tuple(params_values)
 
-            # The properties src_grp and trgt_grp properties makes an InteractionType object order dependent.
-            # For example, Class(X,Y) would be considered different from Class(Y,X).
-            # However, in both cases the interactions should be considered the same.
-            # Then, the next line turns the order dependent arguments into an independent order data.
+            # The properties src_grp and trgt_grp properties makes an
+            # InteractionType object order dependent.
+            # For example, Class(X,Y) would be considered different
+            # from Class(Y,X). However, in both cases the interactions
+            # should be considered the same. Then, the next line turns
+            # the order dependent arguments into an independent order data.
             comp_values_as_tuple = tuple(sorted([self.src_grp, self.trgt_grp]))
-            self._hash_cache = hash(tuple([comp_values_as_tuple, self.type, params_as_tuple]))
+            self._hash_cache = hash(tuple([comp_values_as_tuple,
+                                           self.type, params_as_tuple]))
 
         return self._hash_cache
 
     def __repr__(self):
-        return ('<InteractionType: compounds=(%s, %s) type=%s>' % (self.src_grp, self.trgt_grp, self.type))
+        return ('<InteractionType: compounds=(%s, %s) type=%s>'
+                % (self.src_grp, self.trgt_grp, self.type))
```

### Comparing `luna-0.12.2/luna/interaction/view.py` & `luna-0.13.0/luna/interaction/view.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,115 +1,145 @@
 from luna.mol.entry import MolFileEntry
 from luna.interaction.calc import InteractionsManager
-from luna.wrappers.pymol import PymolWrapper, PymolSessionManager, mybio_to_pymol_selection
+from luna.wrappers.pymol import (PymolWrapper, PymolSessionManager,
+                                 mybio_to_pymol_selection)
 from luna.util.file import is_file_valid
 from luna.util.exceptions import PymolSessionNotInitialized
 from luna.MyBio.util import entity_to_string
 
 
 class InteractionViewer(PymolSessionManager):
 
-    """Class that inherits from :class:`~luna.wrappers.pymol.PymolSessionManager` and implements :meth:`set_view`
-    to depict interactions in Pymol and save the view as a Pymol session.
-
-    This class can be used to visualize multiple complexes into the same Pymol session, for instance, to compare
-    binding modes. To do so, it is recommended that the protein structures are in the same coordinate system, i.e.,
-    they should be aligned first. This can be achieved with :func:`luna.align.tmalign.align_2struct`
-    or any other tool of your preference.
+    """Class that inherits from
+    :class:`~luna.wrappers.pymol.PymolSessionManager` and implements
+    :meth:`set_view` to depict interactions in Pymol and save the view
+    as a Pymol session.
+
+    This class can be used to visualize multiple complexes into the same Pymol
+    session, for instance, to compare binding modes. To do so, it is
+    recommended that the protein structures are in the same coordinate system,
+    i.e., they should be aligned first. This can be achieved with
+    :func:`luna.align.tmalign.align_2struct` or any other tool of your
+    preference.
 
     Parameters
     ----------
     show_hydrop_surface : bool
-        If True, highlight hydrophobic surfaces. The default value is False
+        If True, highlight hydrophobic surfaces. The default value is False.
     **kwargs : dict, optional
-        Extra arguments to `InteractionViewer`. Refer to :class:`~luna.wrappers.pymol.PymolSessionManager`
+        Extra arguments to `InteractionViewer`.
+        Refer to :class:`~luna.wrappers.pymol.PymolSessionManager`
         documentation for a list of all possible arguments.
 
     Examples
     --------
 
-    In the below examples, we will assume a LUNA project object named ``proj_obj`` already exists.
+    In the below examples, we will assume a LUNA project object named
+    ``proj_obj`` already exists.
 
-    **Example 1)** In the first example, we will visualize all interactions identified in the first protein-ligand complex.
-    To do so, we will provide a tuple containing an :class:`~luna.interaction.calc.InteractionsManager` from where
-    the interactions will be recovered.
+    **Example 1)** In the first example, we will visualize all interactions
+    identified in the first protein-ligand complex. To do so, we will provide
+    a tuple containing an :class:`~luna.interaction.calc.InteractionsManager`
+    from where the interactions will be recovered.
 
     First access the property ``interactions_mngrs`` to get an iterable of
-    :class:`~luna.interaction.calc.InteractionsManager` objects and get the first one.
+    :class:`~luna.interaction.calc.InteractionsManager` objects and get the
+    first one.
 
     >>> interactions_mngr = list(proj_obj.interactions_mngrs)[0]
 
-    As `InteractionViewer` expects a list of tuples, we will define it now. The first item of the tuple
-    is the :class:`~luna.mol.entry.Entry` instance, which represents a ligand. This can be obtained directly from
-    the :class:`~luna.interaction.calc.InteractionsManager` object.
-    The :class:`~luna.mol.entry.Entry` instance is necessary because the second item in the tuple (interactions)
-    may be an iterable of :class:`~luna.interaction.type.InteractionType` from where such information
-    cannot be recovered. Finally, the third item can be either a PDB file or a directory.
-    In this example, we will use the PDB directory defined during the LUNA project initialization.
-
-    >>> inter_tuples = [(interactions_mngr.entry, interactions_mngr, proj_obj.pdb_path)]
+    As `InteractionViewer` expects a list of tuples, we will define it now.
+    The first item of the tuple is the :class:`~luna.mol.entry.Entry` instance,
+    which represents a ligand. This can be obtained directly from the
+    :class:`~luna.interaction.calc.InteractionsManager` object.
+    The :class:`~luna.mol.entry.Entry` instance is necessary because the second
+    item in the tuple (interactions) may be an iterable of
+    :class:`~luna.interaction.type.InteractionType` from where such
+    information cannot be recovered. Finally, the third item can be either a
+    PDB file or a directory. In this example, we will use the PDB directory
+    defined during the LUNA project initialization.
+
+    >>> inter_tuples = [(interactions_mngr.entry,
+    ...                  interactions_mngr,
+    ...                  proj_obj.pdb_path)]
 
     Now, we create a new `InteractionViewer` object and call
-    :meth:`~luna.wrappers.pymol.PymolSessionManager.new_session`, which will initialize the session, depict the interactions, and save
-    the session to an output PSE file.
+    :meth:`~luna.wrappers.pymol.PymolSessionManager.new_session`, which will
+    initialize the session, depict the interactions, and save the session to
+    an output PSE file.
 
     >>> inter_view = InteractionViewer()
     >>> inter_view.new_session(inter_tuples, "output.pse")
 
 
-    **Example 2)** In this example, we will create a new Pymol session where a given set of interactions will be shown.
-    Let's say, for instance, we only want to visualize hydrogen bonds.
-
-    To do so, instead of defining a tuple with an :class:`~luna.interaction.calc.InteractionsManager` instance, we will
-    define a list of :class:`~luna.interaction.type.InteractionType` objects, which will contain only hydrogen bonds.
-
-    Let's start with the selection of hydrogen bonds. Here, we will use the built-in method
-    :meth:`luna.interaction.calc.InteractionsManager.filter_by_types`, which permits to filter interactions by type.
+    **Example 2)** In this example, we will create a new Pymol session where
+    a given set of interactions will be shown. Let's say, for instance, we
+    only want to visualize hydrogen bonds.
+
+    To do so, instead of defining a tuple with an
+    :class:`~luna.interaction.calc.InteractionsManager` instance, we will
+    define a list of :class:`~luna.interaction.type.InteractionType` objects,
+    which will contain only hydrogen bonds.
+
+    Let's start with the selection of hydrogen bonds. Here, we will use the
+    built-in method
+    :meth:`luna.interaction.calc.InteractionsManager.filter_by_types`, which
+    permits to filter interactions by type.
 
     >>> interactions_mngr = list(proj_obj.interactions_mngrs)[0]
     >>> hydrogen_bonds = interactions_mngr.filter_by_types(['Hydrogen bond'])
 
-    Now, we just create the tuple as we did before and define the list of interactions we want to depict in the Pymol session.
+    Now, we just create the tuple as we did before and define the list of
+    interactions we want to depict in the Pymol session.
 
-    >>> inter_tuples = [(interactions_mngr.entry, hydrogen_bonds, proj_obj.pdb_path)]
+    >>> inter_tuples = [(interactions_mngr.entry, \
+    ...                  hydrogen_bonds,
+    ...                  proj_obj.pdb_path)]
 
     Finally, we create a new `InteractionViewer` object and call
-    :meth:`InteractionViewer.new_session`, which will initialize the session, depict the interactions, and save
-    the session to an output PSE file.
+    :meth:`InteractionViewer.new_session`, which will initialize the session,
+    depict the interactions, and save the session to an output PSE file.
 
     >>> inter_view = InteractionViewer()
     >>> inter_view.new_session(inter_tuples, "output.pse")
 
-    **Example 3)** In this final example, we will create a new Pymol session to visualize all complexes in a LUNA project.
-    To do so, we create a list with one tuple for each complex:
+    **Example 3)** In this final example, we will create a new Pymol session to
+    visualize all complexes in a LUNA project. To do so, we create a list with
+    one tuple for each complex:
 
-    >>> inter_tuples = [(im.entry, im, proj_obj.pdb_path) for im in proj_obj.interactions_mngrs]
+    >>> inter_tuples = [(im.entry, im, proj_obj.pdb_path) \
+for im in proj_obj.interactions_mngrs]
 
-    Then, as we did before, just create a new `InteractionViewer` object and call :meth:`InteractionViewer.new_session`.
+    Then, as we did before, just create a new `InteractionViewer` object and
+    call :meth:`InteractionViewer.new_session`.
 
     >>> inter_view = InteractionViewer()
     >>> inter_view.new_session(inter_tuples, "output.pse")
 
-    **Note:** it is recommended that all complexes have the same atomic coordinates to make the analysis and comparisons easier.
-    If that's not the case, you may want to align the structures first. To do so, you can use :func:`luna.align.tmalign.align_2struct`
-    or any other tool of your preference.
+    **Note:** it is recommended that all complexes have the same atomic
+    coordinates to make the analysis and comparisons easier. If that's
+    not the case, you may want to align the structures first. To do so,
+    you can use :func:`luna.align.tmalign.align_2struct` or any other tool
+    of your preference.
     """
 
     def __init__(self, show_hydrop_surface=False, **kwargs):
         self.show_hydrop_surface = show_hydrop_surface
         super().__init__(**kwargs)
 
     def set_view(self, inter_tuples):
         """Depict interactions into the current Pymol session.
 
         Parameters
         ----------
         inter_tuples : iterable of tuple
-            Each tuple must contain three items: an :class:`~luna.mol.entry.Entry` instance,
-            an iterable of :class:`~luna.interaction.type.InteractionType` or an :class:`~luna.interaction.calc.InteractionsManager`,
+            Each tuple must contain three items: an
+            :class:`~luna.mol.entry.Entry` instance, an iterable of
+            :class:`~luna.interaction.type.InteractionType` or an
+            :class:`~luna.interaction.calc.InteractionsManager`,
             and a PDB file or the directory where the PDB file is located.
         """
 
         if not isinstance(self.wrapper, PymolWrapper):
             raise PymolSessionNotInitialized("No session was initialized.")
 
         for target_entry, inter_data, pathname in inter_tuples:
@@ -117,72 +147,107 @@
             if is_file_valid(pathname):
                 pdb_file = pathname
             else:
                 pdb_file = "%s/%s.pdb" % (pathname, target_entry.pdb_id)
 
             main_grp = target_entry.to_string(sep="-").replace("'", "-")
 
-            mol_block = (entity_to_string(target_entry.get_biopython_structure())
-                         if isinstance(target_entry, MolFileEntry) else None)
+            mol_block = \
+                (entity_to_string(target_entry.get_biopython_structure())
+                 if isinstance(target_entry, MolFileEntry) else None)
 
             # Load PDB and extract hetatm.
             self.load_pdb(pdb_file, main_grp, mol_block)
 
             if isinstance(inter_data, InteractionsManager):
                 interactions = inter_data.interactions
             else:
                 interactions = inter_data
 
             # Add interactions and styles.
-            interacting_residue_sels = self.set_interactions_view(interactions, main_grp)
+            interacting_residue_sels = \
+                self.set_interactions_view(interactions, main_grp)
             if interacting_residue_sels:
-                self.wrapper.select(name="%s.inter_residues" % main_grp, selection=" or ".join(interacting_residue_sels))
+                sel = " or ".join(interacting_residue_sels)
+                self.wrapper.select(name="%s.inter_residues" % main_grp,
+                                    selection=sel)
 
             if self.show_hydrop_surface:
                 self.wrapper.color([("white", "%s and !name PS*" % main_grp)])
 
-                # It will display all hydrophobic groups if an AtomGroupsManager is available.
+                # It will display all hydrophobic groups if an
+                # AtomGroupsManager is available.
                 atm_grp_mngr = interactions[0].src_grp.manager
                 if atm_grp_mngr is not None:
                     interacting_atms = set()
-                    for atm_grp in atm_grp_mngr.filter_by_types(["Hydrophobe", "Hydrophobic"], must_contain_all=False):
+                    for atm_grp in \
+                        atm_grp_mngr.filter_by_types(["Hydrophobe",
+                                                      "Hydrophobic"],
+                                                     must_contain_all=False):
 
-                        inters = [i for i in atm_grp.interactions if i.type == "Hydrophobic"]
+                        inters = [i for i in atm_grp.interactions
+                                  if i.type == "Hydrophobic"]
 
                         for comp in atm_grp.compounds:
-                            comp_sel = "%s and %s" % (main_grp, mybio_to_pymol_selection(comp))
+                            comp_sel = ("%s and %s"
+                                        % (main_grp,
+                                           mybio_to_pymol_selection(comp)))
                             self.wrapper.show([("sticks", comp_sel)])
 
                         if len(inters) > 0:
                             for inter in inters:
-                                for atm in inter.src_grp.atoms + inter.trgt_grp.atoms:
+                                for atm in (inter.src_grp.atoms
+                                            + inter.trgt_grp.atoms):
+                                    sel = mybio_to_pymol_selection(atm)
                                     if atm not in interacting_atms:
-                                        self.wrapper.color([("pink", "%s and %s" % (main_grp, mybio_to_pymol_selection(atm)))])
-
-                                for atm in inter.src_interacting_atms + inter.trgt_interacting_atms:
-                                    self.wrapper.color([("hotpink", "%s and %s" % (main_grp, mybio_to_pymol_selection(atm)))])
+                                        self.wrapper.color([("pink",
+                                                             "%s and %s"
+                                                             % (main_grp,
+                                                                sel))])
+
+                                for atm in (inter.src_interacting_atms
+                                            + inter.trgt_interacting_atms):
+                                    sel = mybio_to_pymol_selection(atm)
+                                    self.wrapper.color([("hotpink",
+                                                         "%s and %s"
+                                                         % (main_grp, sel))])
                                     interacting_atms.add(atm)
 
                         else:
                             for atm in atm_grp.atoms:
-                                self.wrapper.color([("wheat", "%s and %s" % (main_grp, mybio_to_pymol_selection(atm)))])
-
-                    self.wrapper.hide([("sticks", "%s and not hetatm" % main_grp)])
-                    self.wrapper.show([("sticks", "%s.inter_residues" % main_grp)])
-                    self.wrapper.color([("white", "%s and not hetatm and not %s.inter_residues and !name PS*" % (main_grp, main_grp))])
+                                sel = mybio_to_pymol_selection(atm)
+                                self.wrapper.color([("wheat",
+                                                     "%s and %s"
+                                                     % (main_grp, sel))])
+
+                    self.wrapper.hide([("sticks",
+                                        "%s and not hetatm" % main_grp)])
+                    self.wrapper.show([("sticks",
+                                        "%s.inter_residues" % main_grp)])
+                    self.wrapper.color([("white",
+                                         "%s and not hetatm and not "
+                                         "%s.inter_residues and !name PS*"
+                                         % (main_grp, main_grp))])
 
-                # Otherwise, it will display only hydrophobic groups comprising the interacting groups.
+                # Otherwise, it will display only hydrophobic groups comprising
+                # the interacting groups.
                 else:
                     interacting_atms = set()
                     for inter in interactions:
                         if inter.type != "Hydrophobic":
                             continue
 
                         for atm in inter.src_grp.atoms + inter.trgt_grp.atoms:
+                            sel = mybio_to_pymol_selection(atm)
                             if atm not in interacting_atms:
-                                self.wrapper.color([("pink", "%s and %s" % (main_grp, mybio_to_pymol_selection(atm)))])
+                                self.wrapper.color([("pink", 
+                                                     "%s and %s"
+                                                     % (main_grp, sel))])
 
                         for atm in inter.src_interacting_atms + inter.trgt_interacting_atms:
-                            self.wrapper.color([("hotpink", "%s and %s" % (main_grp, mybio_to_pymol_selection(atm)))])
+                            sel = mybio_to_pymol_selection(atm)
+                            self.wrapper.color([("hotpink",
+                                                 "%s and %s"
+                                                 % (main_grp, sel))])
                             interacting_atms.add(atm)
 
         self.set_last_details_to_view()
```

### Comparing `luna-0.12.2/luna/mol/atom.py` & `luna-0.13.0/luna/mol/atom.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from openbabel import openbabel as ob
 
 import logging
 logger = logging.getLogger()
 
 
 class AtomData:
-    """Store atomic data (atomic number, coordinates,
-    bond type, and serial number).
+    """Store atomic data (atomic number, coordinates, bond type,
+    and serial number).
 
     Parameters
     ----------
     atomic_num : int
         Atomic number.
     coord : array_like of float (size 3)
         Atomic coordinates (x, y, z).
@@ -30,19 +30,23 @@
         The bond type.
     full_id : tuple
         The atom' full id
     serial_number : int or None
         The atom serial number.
     """
 
-    def __init__(self, atomic_num, coord, bond_type,
-                 full_id=None, serial_number=None):
+    def __init__(self,
+                 atomic_num,
+                 coord,
+                 bond_type,
+                 full_id=None,
+                 serial_number=None):
         self.atomic_num = atomic_num
-        # Standardize all coordinate data to the same Numpy data
-        # type for consistence.
+        # Standardize all coordinate data to the same Numpy data type
+        # for consistence.
         self._coord = np.array(coord, "f")
         self.bond_type = bond_type
         self.full_id = full_id
         self.serial_number = serial_number
 
     @property
     def x(self):
@@ -62,16 +66,16 @@
     @property
     def coord(self):
         """array_like of float (size 3): The atomic coordinates (x, y, z)."""
         return self._coord
 
     @coord.setter
     def coord(self, xyz):
-        # Standardize all coordinate data to the same Numpy
-        # data type for consistence.
+        # Standardize all coordinate data to the same Numpy data type for
+        # consistence.
         self._coord = np.array(xyz, "f")
 
     def __repr__(self):
         full_atom_name = ""
         if self.full_id is not None:
             full_atom_name = "%s/%s/%s" % self.full_id[0:3]
             res_name = "%d%s" % (self.full_id[3][1],
@@ -80,16 +84,16 @@
 
             if self.full_id[4][1] != " ":
                 atom_name += "-%s" % self.full_id[4][1]
             full_atom_name += "/%s/%s" % (res_name, atom_name)
 
         return ("<ExtendedAtomData: atomic number=%d, "
                 "coord=(%.3f, %.3f, %.3f), atom='%s', serial number=%s>"
-                % (self.atomic_num, self.x, self.y, self.z,
-                   full_atom_name, str(self.serial_number)))
+                % (self.atomic_num, self.x, self.y, self.z, full_atom_name,
+                   str(self.serial_number)))
 
     def __eq__(self, other):
         """Overrides the default implementation"""
         if isinstance(self, other.__class__):
             return (self.atomic_num == other.atomic_num
                     and np.all(self._coord == other._coord)
                     and self.full_id == other.full_id
@@ -104,16 +108,16 @@
         """Overrides the default implementation"""
         return hash((self.atomic_num, tuple(self._coord),
                      self.full_id, self.bond_type,
                      self.serial_number))
 
 
 class ExtendedAtom:
-    """Extend :class:`~luna.MyBio.PDB.Atom.Atom` with additional
-    properties and methods.
+    """Extend :class:`~luna.MyBio.PDB.Atom.Atom` with additional properties
+    and methods.
 
     Parameters
     ----------
     atom : :class:`~luna.MyBio.PDB.Atom.Atom`
         An atom.
     nb_info : iterable of `AtomData`, optional
         A sequence of `AtomData` containing information about atoms covalently
@@ -136,22 +140,27 @@
         return self._atom
 
     @property
     def neighbors_info(self):
         """list of `AtomData`, read-only: The list of `AtomData`
         containing information about atoms covalently bound to ``atom``.
 
-        To add or remove neighbors information from ``neighbors_info`` use
-        :py:meth:`add_nb_info` or :py:meth:`remove_nb_info`, respectively."""
+        To add or remove neighbors information from ``neighbors_info``
+        use :py:meth:`add_nb_info` or :py:meth:`remove_nb_info`,
+        respectively."""
         return self._nb_info
 
+    @neighbors_info.setter
+    def neighbors_info(self, nb_info):
+        self._nb_info = nb_info
+
     @property
     def atm_grps(self):
-        """list of :class:`~luna.groups.AtomGroup`, read-only: The list of atom
-        groups that contain ``atom``.
+        """list of :class:`~luna.groups.AtomGroup`, read-only: The list of
+        atom groups that contain ``atom``.
 
         To add or remove atom groups from ``atm_grps`` use
         :py:meth:`add_atm_grps` or :py:meth:`remove_atm_grps`, respectively."""
         return self._atm_grps
 
     @property
     def invariants(self):
@@ -172,25 +181,24 @@
     def electronegativity(self):
         """float, read-only: The Pauling electronegativity for this atom.
         This information is obtained from Open Babel."""
         return ob.GetElectroNeg(ob.GetAtomicNum(self.element))
 
     @property
     def full_id(self):
-        """tuple, read-only: The full id of an atom is the tuple
-        (structure id, model id, chain id, residue id, atom name,
-        alternate location)."""
+        """tuple, read-only: The full id of an atom is the tuple (structure id,
+        model id, chain id, residue id, atom name, alternate location)."""
         return self._atom.get_full_id()
 
     @property
     def full_atom_name(self):
         """str, read-only: The full name of an atom is composed by the
-        structure id, model id, chain id, residue name, residue id,
-        atom name, and alternate location if available.
-        Fields are slash-separated."""
+                structure id, model id, chain id, residue name, residue id,
+                atom name, and alternate location if available.
+                Fields are slash-separated."""
         full_atom_name = "%s/%s/%s" % self.get_full_id()[0:3]
         res_name = "%s/%d%s" % (self._atom.parent.resname,
                                 self._atom.parent.id[1],
                                 self._atom.parent.id[2].strip())
         atom_name = "%s" % self._atom.name
         if self.altloc != " ":
             atom_name += "-%s" % self.altloc
@@ -249,17 +257,16 @@
                 "res_id": full_id[3],
                 "name": full_id[4]}
 
     def __getattr__(self, attr):
         if hasattr(self._atom, attr):
             return getattr(self._atom, attr)
         else:
-            error_msg = ("The attribute '%s' does not exist in the class %s."
-                         % (attr, self.__class__.__name__))
-            raise AttributeError(error_msg)
+            raise AttributeError("The attribute '%s' does not exist in the "
+                                 "class %s." % (attr, self.__class__.__name__))
 
     def __getstate__(self):
         return self.__dict__
 
     def __setstate__(self, state):
         self.__dict__.update(state)
 
@@ -277,16 +284,16 @@
         return False
 
     def __ne__(self, other):
         """Overrides the default implementation"""
         return not self.__eq__(other)
 
     def __lt__(self, a2):
-        # It substitutes the residue id for its index in order to keep the
-        # same order as in the PDB.
+        # It substitutes the residue id for its index in order to keep
+        # the same order as in the PDB.
         full_id1 = self.full_id[0:2] + (self.parent.idx, ) + self.full_id[4:]
         full_id2 = a2.full_id[0:2] + (a2.parent.idx, ) + a2.full_id[4:]
 
         return full_id1 < full_id2
 
     def __hash__(self):
         """Overrides the default implementation"""
```

### Comparing `luna-0.12.2/luna/mol/charge_model.py` & `luna-0.13.0/luna/mol/charge_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 
 class OpenEyeModel(ChargeModel):
     """Implementation of OpenEye charge model."""
 
     def get_charge(self, atm_obj):
         """Get the formal charge for atom ``atom_obj``.
 
-        Currently, only formal charges for the elements Hydrogen, Carbon, Nitrogen, Oxygen, Phosphorus,
-        Sulfur, Chlorine, Fluorine, Bromine, Iodine, Magnesium, Calcium, Zinc, Lithium, Sodium,
-        Potassium, and Boron can be recovered.
+        Currently, only formal charges for the elements Hydrogen, Carbon,
+        Nitrogen, Oxygen, Phosphorus, Sulfur, Chlorine, Fluorine, Bromine,
+        Iodine, Magnesium, Calcium, Zinc, Lithium, Sodium, Potassium,
+        and Boron can be recovered.
 
         Parameters
         ----------
         atm_obj : :class:`~luna.wrappers.base.AtomWrapper`
             The target atom.
 
         Examples
@@ -54,14 +55,15 @@
 
         # Hydrogen
         if atm_num == 1:
             if valence != 1:
                 formal_charge = 1
             elif valence == 1:
                 formal_charge = 0
+
         # Carbon
         elif atm_num == 6:
             if valence == 3:
                 has_polar_nb = False
                 nbs = atm_obj.get_neighbors()
                 for nb_atm_obj in nbs:
                     nb_atm_obj = AtomWrapper(nb_atm_obj)
@@ -71,82 +73,94 @@
                         break
                 if has_polar_nb is True:
                     formal_charge = 1
                 else:
                     formal_charge = -1
             elif valence == 4:
                 formal_charge = 0
+
         # Nitrogen
         elif atm_num == 7:
             if valence == 2:
                 formal_charge = -1
             elif valence == 4:
                 formal_charge = 1
             elif valence == 3:
                 formal_charge = 0
+
         # Oxygen
         elif atm_num == 8:
             if valence == 1:
                 formal_charge = -1
             elif valence == 3:
                 formal_charge = 1
             elif valence == 2:
                 formal_charge = 0
+
         # Phosphorus
         elif atm_num == 15:
             if valence == 4:
                 formal_charge = 1
+
         # Sulfur
         elif atm_num == 16:
             if valence == 1:
                 formal_charge = -1
             elif valence == 3:
                 formal_charge = 1
             elif valence == 5:
                 formal_charge = -1
             elif valence == 4:
                 if atm_obj.get_degree() == 4:
                     formal_charge = 2
             elif valence == 2 or valence == 6:
                 formal_charge == 0
+
         # Chlorine
         elif atm_num == 17:
             if valence == 0:
                 formal_charge = -1
             elif valence == 4:
                 formal_charge = 3
             elif valence == 1:
                 formal_charge = 0
+
         # Fluorine, Bromine, Iodine
         elif atm_num == 9 or atm_num == 35 or atm_num == 53:
             if valence == 0:
                 formal_charge = -1
             elif valence == 1:
                 formal_charge = 0
+
         # Magnesium, Calcium, Zinc
         elif atm_num == 12 or atm_num == 20 or atm_num == 30:
             if valence == 0:
                 formal_charge = 2
             elif valence == 2:
                 formal_charge = 0
+
         # Lithium, Sodium, Potassium
         elif atm_num == 3 or atm_num == 11 or atm_num == 19:
             if valence == 0:
                 formal_charge = 1
             elif valence == 1:
                 formal_charge = 0
+
         # Boron
         elif atm_num == 5:
             # If the valence is four, the formal charge is -1.
-            # OBS: there is an error in OpenEye chargel model text, they said that Boron should have a
-            # charge of +1 when the valence is 4. However, the MDL Valence Model says it should be -1.
+            # OBS: there is an error in OpenEye chargel model text,
+            # they said that Boron should have a charge of +1 when
+            # the valence is 4.
+            # However, the MDL Valence Model says it should be -1.
             if valence == 4:
                 formal_charge = -1
             elif valence == 3:
                 formal_charge = 0
+
         # Iron: 26
         # If the valence is zero, the formal charge is +3 if the partial charge is 3.0, and +2 otherwise.
         # Copper: 29
         # If the valence is zero, the formal charge is +2 if the partial charge is 2.0, and +1 otherwise.
         # else:
         # For the remaining elements, if the valence of an atom is zero, its formal charge is set from its partial charge.
```

### Comparing `luna-0.12.2/luna/mol/clustering.py` & `luna-0.13.0/luna/mol/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,29 @@
 def available_similarity_functions():
     """Return a list of all similarity metrics available at RDKit."""
     regex = re.compile("Bulk([a-zA-Z]+)Similarity", flags=0)
     return list(filter(regex.match, dir(DataStructs)))
 
 
 def calc_distance_matrix(fps, similarity_func="BulkTanimotoSimilarity"):
-    """Calculate the pairwise distance (dissimilarity) between fingerprints in ``fps`` using
-        the similarity metric ``similarity_func``.
+    """Calculate the pairwise distance (dissimilarity) between fingerprints
+     in ``fps`` using the similarity metric ``similarity_func``.
 
     Parameters
     ----------
-    fps : iterable of RDKit :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` or :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`
+    fps : iterable of RDKit \
+            :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` or \
+            :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`
         A sequence of fingerprints.
     similarity_func : str
-        A similarity metric to calculate the distance between the provided fingerprints. The default value is 'BulkTanimotoSimilarity'.
+        A similarity metric to calculate the distance between the provided
+        fingerprints. The default value is 'BulkTanimotoSimilarity'.
 
-        To check out the list of available similarity metrics, call the function :py:meth:`available_similarity_functions`.
+        To check out the list of available similarity metrics, call the
+        function :py:meth:`available_similarity_functions`.
 
     Examples
     --------
 
     First, let's define a set of molecules.
 
     >>> from luna.wrappers.base import MolWrapper
@@ -39,15 +43,16 @@
     ...         MolWrapper.from_smiles("CCCCCCCCO").unwrap()]
 
     Now, we generate fingerprints for those molecules.
 
     >>> from luna.mol.fingerprint import generate_fp_for_mols
     >>> fps = [d["fp"] for d in generate_fp_for_mols(mols, "morgan_fp")]
 
-    Finally, calculate the distance between the molecules based on their fingerprints.
+    Finally, calculate the distance between the molecules based on their
+    fingerprints.
 
     >>> from luna.mol.clustering import calc_distance_matrix
     >>> print(calc_distance_matrix(fps))
     [0.125, 0.46153846153846156, 0.3846153846153846]
 
     Returns
     -------
@@ -68,26 +73,32 @@
         sims = getattr(DataStructs, similarity_func)(*params)
         dists.extend([1 - x for x in sims])
 
     return dists
 
 
 def cluster_fps(fps, cutoff=0.2, similarity_func="BulkTanimotoSimilarity"):
-    """Clusterize molecules based on fingerprints using the Butina clustering algorithm.
+    """Clusterize molecules based on fingerprints using the Butina
+    clustering algorithm.
 
     Parameters
     ----------
-    fps : iterable of RDKit :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` or :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`
+    fps : iterable of RDKit \
+            :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` or
+            :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`
         A sequence of fingerprints.
     cutoff : float
-        Elements within this range of each other are considered to be neighbors.
+        Elements within this range of each other are considered
+        to be neighbors.
     similarity_func : str
-        A similarity metric to calculate the distance between the provided fingerprints.  The default value is 'BulkTanimotoSimilarity'.
+        A similarity metric to calculate the distance between the provided
+        fingerprints.  The default value is 'BulkTanimotoSimilarity'.
 
-        To check out the list of available similarity metrics, call the function :py:meth:`available_similarity_functions`.
+        To check out the list of available similarity metrics, call the
+        function :py:meth:`available_similarity_functions`.
 
     Examples
     --------
 
     First, let's define a set of molecules.
 
     >>> from luna.wrappers.base import MolWrapper
@@ -105,18 +116,20 @@
     >>> from luna.mol.clustering import cluster_fps
     >>> print(cluster_fps(fps, cutoff=0.2))
     ((1, 0), (2,))
 
     Returns
     -------
     clusters : tuple of tuples
-        Each cluster is defined as a tuple of tuples, where the first element for each cluster is its centroid.
+        Each cluster is defined as a tuple of tuples, where the first
+        element for each cluster is its centroid.
     """
     logger.debug("Trying to clusterize %d molecules." % len(fps))
-    logger.debug("Defined cutoff: %.2f. Defined similarity function: %s." % (cutoff, similarity_func))
+    logger.debug("Defined cutoff: %.2f. Defined similarity function: %s."
+                 % (cutoff, similarity_func))
 
     # first generate the distance matrix.
     dists = calc_distance_matrix(fps, similarity_func)
     logger.debug("Distance matrix created.")
 
     # now cluster the data.
     cs = Butina.ClusterData(dists, len(fps), cutoff, isDistData=True)
```

### Comparing `luna-0.12.2/luna/mol/depiction.py` & `luna-0.13.0/luna/mol/depiction.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,60 +12,75 @@
     """Draw molecules and depict pharmacophoric properties as colored circles.
 
     Parameters
     ----------
     feature_extractor : :class:`~luna.mol.features.FeatureExtractor`
         Perceive pharmacophoric properties from molecules.
     colors : :class:`~luna.util.ColorPallete`
-        Color scheme for pharmacophoric properties perceived by ``feature_extractor``.
-        The default value is :const:`~luna.util.default_values.ATOM_TYPES_COLOR`.
+        Color scheme for pharmacophoric properties perceived by
+        ``feature_extractor``. The default value is \
+        :const:`~luna.util.default_values.ATOM_TYPES_COLOR`.
     format : {'png', 'svg'}
         The output file format. The default value is 'png'.
     figsize : tuple of (float, float)
         Width and height in inches. The default value is (800, 800).
     font_size : float
-        The font size. The units are, roughly, pixels. The default value is 0.5.
+        The font size. The units are, roughly, pixels.
+        The default value is 0.5.
     circle_dist : float
-        Distance between circles (pharmacophoric properties). The default value is 0.2.
+        Distance between circles (pharmacophoric properties).
+        The default value is 0.2.
     circle_radius :
-        Circles' radius size of pharmacophoric properties. The default value is 0.3.
+        Circles' radius size of pharmacophoric properties.
+        The default value is 0.3.
     use_bw_atom_palette : bool
         Use a black & white palette for atoms and bonds.
 
     Examples
     --------
 
     First, let's read a molecule (glutamine).
 
     >>> from luna.wrappers.base import MolWrapper
     >>> mol = MolWrapper.from_smiles("N[C@@H](CCC(N)=O)C(O)=O")
 
-    Now, create a feature factory and instantiate a new FeatureExtractor object.
+    Now, create a feature factory and instantiate a new FeatureExtractor
+    object.
 
     >>> from luna.util.default_values import ATOM_PROP_FILE
     >>> from rdkit.Chem import ChemicalFeatures
     >>> from luna.mol.features import FeatureExtractor
     >>> feature_factory = ChemicalFeatures.BuildFeatureFactory(ATOM_PROP_FILE)
     >>> feature_extractor = FeatureExtractor(feature_factory)
 
-    Instantiate a new PharmacophoreDepiction object with the desired configuration.
-    For example, you can provide a color scheme for pharmacophoric properties, the image size, and its format.
+    Instantiate a new PharmacophoreDepiction object with the desired
+    configuration. For example, you can provide a color scheme for
+    pharmacophoric properties, the image size, and its format.
 
     >>> from luna.util.default_values import ATOM_TYPES_COLOR
     >>> from luna.mol.depiction import PharmacophoreDepiction
-    pd = PharmacophoreDepiction(feature_extractor=feature_extractor, colors=ATOM_TYPES_COLOR,
-                                fig_size=(500, 500), format="svg")
+    pd = PharmacophoreDepiction(feature_extractor=feature_extractor,
+                                colors=ATOM_TYPES_COLOR,
+                                fig_size=(500, 500),
+                                format="svg")
 
-    Finally, you can draw the molecule with annotated pharmacophoric properties.
+    Finally, you can draw the molecule with annotated pharmacophoric
+    properties.
 
     >>> pd.plot_fig(mol, "output.svg")
     """
 
-    def __init__(self, feature_extractor=None, colors=ATOM_TYPES_COLOR, format="png",
-                 fig_size=(800, 800), font_size=0.5, circle_dist=0.2, circle_radius=0.3,
+    def __init__(self,
+                 feature_extractor=None,
+                 colors=ATOM_TYPES_COLOR,
+                 format="png",
+                 fig_size=(800, 800),
+                 font_size=0.5,
+                 circle_dist=0.2,
+                 circle_radius=0.3,
                  use_bw_atom_palette=True):
 
         self.feature_extractor = feature_extractor
         self.colors = colors
         self.format = format
         self.fig_size = fig_size
         self.font_size = font_size
@@ -74,35 +89,45 @@
         self.use_bw_atom_palette = use_bw_atom_palette
 
     def _perceive_atm_types(self, rdmol):
         if self.feature_extractor is not None:
             return self.feature_extractor.get_features_by_atoms(rdmol)
         return {}
 
-    def plot_fig(self, mol_obj, output=None, atm_types=None, legend=None):
-        """Draw the molecule ``mol_obj`` and depict its pharmacophoric properties.
+    def plot_fig(self,
+                 mol_obj,
+                 output=None,
+                 atm_types=None,
+                 legend=None):
+        """Draw the molecule ``mol_obj`` and depict its pharmacophoric
+        properties.
 
         Parameters
         ----------
-        mol_obj : :class:`~luna.wrappers.base.MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`
+        mol_obj : :class:`~luna.wrappers.base.MolWrapper`, \
+                    :class:`rdkit.Chem.rdchem.Mol`, or \
+                    :class:`openbabel.pybel.Molecule`
             The molecule.
         output : str
             The output file where the molecule will be drawn.
-            If None, returns a drawing object (:class:`~rdkit.Chem.Draw.rdMolDraw2D.MolDraw2DCairo` or
+            If None, returns a drawing object
+            (:class:`~rdkit.Chem.Draw.rdMolDraw2D.MolDraw2DCairo` or
             :class:`~rdkit.Chem.Draw.rdMolDraw2D.MolDraw2DSVG`).
         atm_types : dict or None
-            A pre-annotated dictionary for mapping atoms and pharmacophoric properties.
-            If None, try to perceive properties with ``feature_extractor``.
+            A pre-annotated dictionary for mapping atoms and pharmacophoric
+            properties. If None, try to perceive properties with
+            ``feature_extractor``.
         legend : str
             A title for the figure.
 
         Returns
         -------
-        drawer : None or a drawing object (:class:`~rdkit.Chem.Draw.rdMolDraw2D.MolDraw2DCairo` or \
-        :class:`~rdkit.Chem.Draw.rdMolDraw2D.MolDraw2DSVG`)
+        drawer : None or a drawing object \
+            (:class:`~rdkit.Chem.Draw.rdMolDraw2D.MolDraw2DCairo` or \
+             :class:`~rdkit.Chem.Draw.rdMolDraw2D.MolDraw2DSVG`)
         """
 
         rdmol = MolWrapper(mol_obj).as_rdkit()
 
         # Make a copy of the molecule
         rwm = Chem.RWMol(rdmol)
         Compute2DCoords(rwm)
@@ -119,30 +144,36 @@
             pass
 
         opts = drawer.drawOptions()
 
         highlight = {}
         for atm_id in atm_types:
             centroid = list(rwm.GetConformer().GetAtomPosition(atm_id))
-            valid_features = [f for f in atm_types[atm_id] if f.name in self.colors]
+            valid_features = [f for f in atm_types[atm_id]
+                              if f.name in self.colors]
 
             if valid_features:
                 if len(valid_features) == 1:
                     pos = centroid
                     atmIdx = self._add_dummy_atom(rwm, centroid)
-                    highlight[atmIdx] = self.colors.get_normalized_color(valid_features[0].name)
+                    feat_name = valid_features[0].name
+                    highlight[atmIdx] = \
+                        self.colors.get_normalized_color(feat_name)
                     opts.atomLabels[atmIdx] = ''
                 else:
                     sliceRad = radians(360 / len(valid_features))
                     for i, feature in enumerate(valid_features):
                         rad = i * sliceRad
-                        pos = [self.circle_dist * cos(rad), self.circle_dist * sin(rad), 0]
+                        pos = [self.circle_dist * cos(rad),
+                               self.circle_dist * sin(rad),
+                               0]
                         adj_Pos = [x + y for x, y in zip(centroid, pos)]
                         new_atm_id = self._add_dummy_atom(rwm, adj_Pos)
-                        highlight[new_atm_id] = self.colors.get_normalized_color(feature.name)
+                        highlight[new_atm_id] = \
+                            self.colors.get_normalized_color(feature.name)
                         opts.atomLabels[new_atm_id] = ''
 
         atoms = [x for x in highlight]
         radius = {a: self.circle_radius for a in atoms}
 
         opts.flagCloseContactsDist = -1000
         opts.legendFontSize = 20
@@ -152,16 +183,20 @@
             opts.useBWAtomPalette()
         else:
             opts.useDefaultAtomPalette()
 
         legend = legend or ""
 
         drawer.SetFontSize(self.font_size)
-        drawer.DrawMolecule(rwm, highlightAtoms=atoms, highlightAtomColors=highlight,
-                            highlightBonds=[], highlightAtomRadii=radius, legend=legend)
+        drawer.DrawMolecule(rwm,
+                            highlightAtoms=atoms,
+                            highlightAtomColors=highlight,
+                            highlightBonds=[],
+                            highlightAtomRadii=radius,
+                            legend=legend)
         drawer.FinishDrawing()
 
         if output:
             if self.format == "png":
                 drawer.WriteDrawingText(output)
             elif self.format == "svg":
                 svg = drawer.GetDrawingText().replace('svg:', '')
```

### Comparing `luna-0.12.2/luna/mol/entry.py` & `luna-0.13.0/luna/mol/entry.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,119 +7,141 @@
 
 from rdkit.Chem import Mol as RDMol
 from openbabel import OBMol
 from openbabel.pybel import readfile
 from openbabel.pybel import Molecule as PybelMol
 from openbabel.pybel import informats as OB_FORMATS
 
-from luna.wrappers.rdkit import RDKIT_FORMATS, read_multimol_file, read_mol_from_file
+from luna.wrappers.rdkit import (RDKIT_FORMATS, read_multimol_file,
+                                 read_mol_from_file)
 from luna.wrappers.base import MolWrapper
-from luna.util.default_values import ACCEPTED_MOL_OBJ_TYPES, ENTRY_SEPARATOR, ARTIFACTS_LIST
+from luna.util.default_values import (ACCEPTED_MOL_OBJ_TYPES, ENTRY_SEPARATOR,
+                                      ARTIFACTS_LIST)
 from luna.util.file import get_file_format, get_filename
-from luna.util.exceptions import InvalidEntry, IllegalArgumentError, MoleculeObjectError, MoleculeObjectTypeError, MoleculeNotFoundError
+from luna.util.exceptions import (InvalidEntry,
+                                  IllegalArgumentError,
+                                  MoleculeObjectError,
+                                  MoleculeObjectTypeError,
+                                  MoleculeNotFoundError)
 from luna.MyBio.PDB.PDBParser import PDBParser, WATER_NAMES, DEFAULT_CHAIN_ID
 from luna.MyBio.PDB.Entity import Entity
 
 
 logger = logging.getLogger()
 
-PCI_ENTRY_REGEX = re.compile(r'^.{1,255}:\w:\w[\w+\-]{0,2}:\-?\d{1,4}[a-zA-z]?$')
+PCI_ENTRY_REGEX = re.compile(r'^.{1,255}:\w:\w[\w+\-]{0,2}:'
+                             r'\-?\d{1,4}[a-zA-z]?$')
 PPI_ENTRY_REGEX = re.compile(r'^.{1,255}:\w$')
 
 REGEX_RESNUM_ICODE = re.compile(r'^([\-\+]?\d+)([a-zA-z]?)$')
 
 
 class Entry:
-    """Entries determine the target molecule to which interactions and other properties
-    will be calculated. They can be ligands, chains, etc, and can be defined in a number of ways.
-    Each entry has an associated PDB file that may contain macromolecules (protein, RNA, DNA) and
-    other small molecules, water, and ions.
-    The PDB file provides the context to where the interactions with the target molecule will be calculated.
+    """Entries determine the target molecule to which interactions and other
+    properties will be calculated. They can be ligands, chains, etc, and can
+    be defined in a number of ways. Each entry has an associated PDB file that
+    may contain macromolecules (protein, RNA, DNA) and other small molecules,
+    water, and ions. The PDB file provides the context to where the
+    interactions with the target molecule will be calculated.
 
     Parameters
     ----------
     pdb_id : str
-        A 4-symbols structure id from PDB or a local PDB filename. Example: '3QL8' or 'file1'.
+        A 4-symbols structure id from PDB or a local PDB filename.
+        Example: '3QL8' or 'file1'.
     chain_id : str
         A 1-symbol chain id. Example: 'A'.
     comp_name : str, optional
-        A 1 to 3-symbols compound name (residue name in the PDB format).
+        A 1 to 3-symbols molecule name (residue name in the PDB format).
         Obligatory if ``is_hetatm`` is True. Example: 'X01'.
     comp_num : int, optional
         A valid 4-digits integer (residue sequence number in the PDB format).
         Obligatory if ``is_hetatm`` is True. Example: 300 or -1.
     comp_icode : str, optional
-        A 1-character compound insertion code (residue insertion code in the PDB format). Example: 'A'.
+        A 1-character molecule insertion code (residue insertion code in the
+        PDB format). Example: 'A'.
     is_hetatm : bool
-        If the compound is a ligand or not. The default value is True.
+        If the molecule is a ligand or not. The default value is True.
     sep : str
-        A separator character to format the entry string. The default value is ':'.
-    parser : :class:`~luna.MyBio.PDB.PDBParser.PDBParser` or :class:`~luna.MyBio.PDB.FTMapParser.FTMapParser`, optional
-            Define a PDB parser object. If not provided, the default parser will be used.
+        A separator character to format the entry string.
+        The default value is ':'.
+    parser : :class:`~luna.MyBio.PDB.PDBParser.PDBParser` or \
+                :class:`~luna.MyBio.PDB.FTMapParser.FTMapParser`, optional
+            Define a PDB parser object. If not provided, the default parser
+            will be used.
 
     Raises
     ------
     IllegalArgumentError
-        If ``is_hetatm`` is True, but the compound name and number are not provided.
-        If the compound number is provided but it is not an integer.
-        If ``comp_icode`` is provided but it is not a valid character.
+        If ``is_hetatm`` is True, but the molecule name and number are
+        not provided. If the molecule number is provided but it is not
+        an integer. If ``comp_icode`` is provided but it is not a
+        valid character.
     InvalidEntry
         If the provided information does not match the PDB format.
 
     Examples
     --------
 
     Chain entry: can be used to calculate interactions with a given chain.
 
     >>> from luna.mol.entry import Entry
     >>> e = Entry(pdb_id="3QL8", chain_id="A")
     >>> print(e)
     <Entry: 3QL8:A>
 
-    Compound entry: can be used to calculate interactions with a given compound (residue or nucleotide).
+    Molecule entry: can be used to calculate interactions with a given molecule
+    (residue or nucleotide).
 
     >>> from luna.mol.entry import Entry
-    >>> e = Entry(pdb_id="3QL8", chain_id="A", comp_name="HIS", comp_num=125, is_hetatm=False)
+    >>> e = Entry(pdb_id="3QL8", chain_id="A", comp_name="HIS", comp_num=125, \
+is_hetatm=False)
     >>> print(e)
     <Entry: 3QL8:A:HIS:125>
 
     Ligand entry: can be used to calculate interactions with a given ligand.
 
     >>> from luna.mol.entry import Entry
-    >>> e = Entry(pdb_id="3QL8", chain_id="A", comp_name="X01", comp_num=300, is_hetatm=True)
+    >>> e = Entry(pdb_id="3QL8", chain_id="A", comp_name="X01", comp_num=300, \
+is_hetatm=True)
     >>> print(e)
     <Entry: 3QL8:A:X01:300>
 
     You can use a different character separator for the entries. For example:
 
     >>> from luna.mol.entry import Entry
-    >>> e = Entry(pdb_id="3QL8", chain_id="A", comp_name="X01", comp_num=300, is_hetatm=True, sep="/")
+    >>> e = Entry(pdb_id="3QL8", chain_id="A", comp_name="X01", comp_num=300, \
+is_hetatm=True, sep="/")
     >>> print(e)
     <Entry: 3QL8/A/X01/300>
     """
 
     def __init__(self, pdb_id, chain_id, comp_name=None,
                  comp_num=None, comp_icode=None,
                  is_hetatm=True, sep=ENTRY_SEPARATOR, parser=None):
 
         if xor(comp_name is None, comp_num is None):
-            raise IllegalArgumentError("You tried to define a compound, so "
+            raise IllegalArgumentError("You tried to define a molecule, so "
                                        "you must inform its name and number.")
 
         if comp_num is not None:
             try:
                 assert float(comp_num).is_integer()
                 comp_num = int(comp_num)
             except (ValueError, AssertionError):
-                raise IllegalArgumentError("The informed compound number '%s' is invalid. It must be an integer." % str(comp_num))
+                error_msg = ("The informed molecule number '%s' is invalid. "
+                             "It must be an integer." % str(comp_num))
+                raise IllegalArgumentError(error_msg)
 
         if comp_icode is not None:
             comp_icode = str(comp_icode)
             if comp_icode.isdigit() or len(comp_icode) > 1:
-                raise IllegalArgumentError("The informed compound icode '%s' is invalid. It must be a character." % str(comp_icode))
+                error_msg = ("The informed molecule icode '%s' is invalid. "
+                             "It must be a character." % str(comp_icode))
+                raise IllegalArgumentError(error_msg)
 
         self._pdb_id = pdb_id
         self._chain_id = chain_id
         self._comp_name = comp_name
         self._comp_num = comp_num
         self._comp_icode = comp_icode
         self.is_hetatm = is_hetatm
@@ -135,107 +157,201 @@
         """Initialize from a string.
 
         Parameters
         ----------
         entry_str : str
             A string representing the entry. Example: '3QL8:A:X01:300'.
         is_hetatm : bool
-            Defines if the compound is a ligand or not. The default value is True.
+            Defines if the molecule is a ligand or not.
+            The default value is True.
         sep : str
-            The separator character used in ``entry_str``. The default value is ':'.
-            For example: if ``entry_str`` is set to '3QL8|A|X01|300', then ``sep`` should be defined as '|'.
+            The separator character used in ``entry_str``.
+            The default value is ':'. For example: if ``entry_str`` is set to
+            '3QL8|A|X01|300', then ``sep`` should be defined as '|'.
 
         Returns
         -------
          : `Entry`
 
         Raises
         ------
         IllegalArgumentError
-            If the fields in ``entry_str`` do not match the format expected to define a
-            chain (ChainEntry) or a compound (MolEntry).
+            If the fields in ``entry_str`` do not match the format expected to
+            define a chain (`ChainEntry`) or a molecule (`MolEntry`).
 
         Examples
         --------
 
         Chain entry: can be used to calculate interactions with a given chain.
 
         >>> from luna.mol.entry import Entry
         >>> e = Entry.from_string("3QL8:A", sep=":")
         >>> print(e)
         <Entry: 3QL8:A>
 
-        Compound entry: can be used to calculate interactions with a given compound (residue or nucleotide).
+        Molecule entry: can be used to calculate interactions with a given
+        molecule (residue or nucleotide).
 
         >>> from luna.mol.entry import Entry
         >>> e = Entry.from_string("3QL8:A:HIS:125", sep=":")
         >>> print(e)
         <Entry: 3QL8:A:HIS:125>
 
-        Ligand entry: can be used to calculate interactions with a given ligand.
+        Ligand entry: can be used to calculate interactions with a given
+        ligand.
 
         >>> from luna.mol.entry import Entry
         >>> e = Entry.from_string("3QL8:A:X01:300", sep=":")
         >>> print(e)
         <Entry: 3QL8:A:X01:300>
         """
 
         entries = entry_str.split(sep)
 
         # Try to initialize a new ChainEntry.
         if len(entries) == 2:
             if any([str(i).strip() == "" for i in entries]):
-                raise IllegalArgumentError("The number of fields in the informed string '%s' is incorrect. A valid ChainEntry must contain "
-                                           "two obligatory fields: PDB and chain id." % entry_str)
+                error_msg = ("The number of fields in the informed string "
+                             "'%s' is incorrect. A valid ChainEntry must "
+                             "contain two obligatory fields: PDB and chain "
+                             "id." % entry_str)
+                raise IllegalArgumentError(error_msg)
 
             return cls(*entries, is_hetatm=False, sep=sep)
 
         # Try to initialize a new MolEntry.
         elif len(entries) == 4:
             if any([str(i).strip() == "" for i in entries]):
-                raise IllegalArgumentError("The number of fields in the informed string '%s' is incorrect. A valid MolEntry "
-                                           "must contain four obligatory fields: PDB, chain id, compound name, and compound "
-                                           "number followed by its insertion code when applicable." % entry_str)
+                error_msg = ("The number of fields in the informed string "
+                             "'%s' is incorrect. A valid MolEntry must "
+                             "contain four obligatory fields: PDB, chain id, "
+                             "molecule name, and molecule number followed by "
+                             "its insertion code when applicable." % entry_str)
+                raise IllegalArgumentError(error_msg)
 
             # Separate ligand number from insertion code.
             matched = REGEX_RESNUM_ICODE.match(entries[3])
             if matched:
                 comp_num = matched.group(1)
                 try:
                     assert float(comp_num).is_integer()
                     comp_num = int(comp_num)
                 except (ValueError, AssertionError):
-                    raise IllegalArgumentError("The informed compound number '%s' is invalid. It must be an integer." % str(comp_num))
+                    error_msg = ("The informed molecule number '%s' is "
+                                 "invalid. It must be an integer."
+                                 % str(comp_num))
+                    raise IllegalArgumentError(error_msg)
 
                 icode = None if matched.group(2) == "" else matched.group(2)
                 entries = entries[0:3] + [comp_num, icode]
             else:
-                raise IllegalArgumentError("The compound number and its insertion code (if applicable) '%s' is invalid. "
-                                           "It must be an integer followed by one insertion code character when applicable."
-                                           % entries[3])
+                error_msg = ("The molecule number and its insertion code "
+                             "(if applicable) '%s' is invalid. It must be an "
+                             "integer followed by one insertion code "
+                             "character when applicable." % entries[3])
+                raise IllegalArgumentError(error_msg)
 
             return cls(*entries, is_hetatm=is_hetatm, sep=sep)
         else:
-            raise IllegalArgumentError("The number of fields in the informed string '%s' is incorrect. A valid string must contain "
-                                       "two obligatory fields (PDB and chain id) and it may contain two optional fields (compound name "
-                                       "and compound number followed by its insertion code when applicable)." % entry_str)
+            error_msg = ("The number of fields in the informed string '%s' is "
+                         "incorrect. A valid string must contain two "
+                         "obligatory fields (PDB and chain id) and it may "
+                         "contain two optional fields (molecule name and "
+                         "molecule number followed by its insertion code when "
+                         "applicable)." % entry_str)
+            raise IllegalArgumentError(error_msg)
 
     @classmethod
     def from_file(cls, input_file, pdb_id=None, mol_file=None,
                   entries_sep=":", fields_sep=",", **kwargs):
-        #     """Initialize from a list of strings representing compounds.
+        """Initialize from a file containing a list of strings
+        representing entries.
 
-        #     Parameters
-        #     ----------
-        #     input_file : str
-        #         The file from where the list of strings (one per line) will be read from.
-        #     sep : str
-        #         The separator character used in ``input_file``. The default value is ':'.
-        #         For example: if entries from ``input_file`` use '|' as the separator, then ``sep`` should be defined as '|'.
+        Parameters
+        ----------
+        input_file : str
+            The file from where the list of strings (one per line) will
+            be read from.
+
+            .. note::
+                The list of strings can be a mix of complexes whose
+                molecules lie all in the same PDB file, or whose protein
+                structure is in a PDB file and whose ligand is on a
+                molecular file. See ``entries_sep`` and ``fields_sep``.
+        pdb_id : str
+            A 4-symbols structure id from PDB or a local PDB filename.
+            Example: '3QL8' or 'file1'.
+
+            .. note::
+                Mandatory if there is any line containing only the ligand name.
+                This only applies to ligands that will be read from
+                multimolecular files.
+        mol_file : str
+            Pathname of the molecular file.
+
+            .. note::
+                Mandatory if there is any line containing only the ligand name.
+                This only applies to ligands that will be read from
+                multimolecular files.
+        entries_sep : str
+            a separator for entries whose molecules lie all in the same PDB
+            file, not requiring, therefore, an additional molecular file.
+            Such entries cause the function to yield `ChainEntry` or
+            `MolEntry` objects. Default: ':'. E.g.: 3QQK:A:X02:497.
+        fields_sep : str
+            a character used to separate fields in ``input_file`` for
+            complexes whose protein structure is in a PDB file and
+            whose ligand is on a molecular file. Such entries cause the
+            function to yield `MolFileEntry` objects. Default: ','
+
+            Each line should contain either the ligand name only or the
+            following fields:
+
+                * ``pdb_id`` (str): a 4-symbols structure id from \
+PDB or a local PDB filename. Example: '3QL8' or 'file1'.
+                * ``mol_id`` (str): the ligand id in the molecular file.
+
+                * ``mol_file`` (str): pathname of the molecular file.
+
+                * ``is_multimol_file`` (bool): if ``mol_file`` contains \
+multiple molecules or not. If True, ``mol_id`` should match some ligand name \
+in ``mol_file``.
+
+            .. note::
+                If a line contains only the ligand name, providing a value to
+                the arguments ``pdb_id`` and ``mol_file`` is mandatory.
+        kwargs : dict, optional
+            Extra arguments to lines that yield `MolFileEntry` objects.
+            Refer to the documentation for a list of all possible arguments.
+
+        Yields
+        ------
+        `ChainEntry`, `MolEntry`, `MolFileEntry`
+            Define a chain, a molecule from a PDB file, or a molecule from
+            a molecular file, respectively, according to a string
+            from ``input_file``.
+
+        Raises
+        ------
+        IllegalArgumentError
+            If a given line contain a string that do not match the format
+            expected to define a chain (`ChainEntry`) or a molecule from a PDB
+            file (`MolEntry`), or a molecule from a molecular file
+            (`MolFileEntry`).
+
+        Examples
+        --------
+
+        Example of a file containing a mix of entry types:
 
+        >>> 3QQK:A:X02:497
+        >>> ZINC000065293174
+        >>> protein,ZINC000012442563,inputs/ligands.mol2,True
+        >>> protein,ZINC000007786517,inputs/ZINC000007786517.mol,False
+        """
         if not exists(input_file):
             raise OSError("File '%s' does not exist." % input_file)
 
         with open(input_file, "r") as IN:
             c = 1
             for row in IN:
                 row = row.strip()
@@ -300,79 +416,86 @@
     @property
     def chain_id(self):
         """str, read-only: the chain id."""
         return self._chain_id
 
     @property
     def comp_name(self):
-        """str, read-only: the compound name."""
+        """str, read-only: the molecule name."""
         return self._comp_name
 
     @property
     def comp_num(self):
-        """int, read-only: the compound number."""
+        """int, read-only: the molecule number."""
         return self._comp_num
 
     @property
     def comp_icode(self):
-        """str, read-only: the compound insertion code."""
+        """str, read-only: the molecule insertion code."""
         if isinstance(self._comp_icode, str):
             return self._comp_icode
         else:
             return ' '
 
     @property
     def full_id(self):
-        """tuple, read-only: The full id of the entry is the tuple (PDB id or filename, chain id)
-        for entries representing chains and (PDB id or filename, chain id,
-        compound name, compound number, insertion code) for entries representing compounds."""
+        """tuple, read-only: The full id of the entry is the tuple
+        (PDB id or filename, chain id) for entries representing chains and
+        (PDB id or filename, chain id, molecule name, molecule number,
+        insertion code) for entries representing molecules."""
 
         entry = [self.pdb_id, self.chain_id]
         if self.comp_name is not None and self.comp_num is not None:
             entry.append(self.comp_name)
             entry.append(self.comp_num)
             entry.append(self.comp_icode)
         return tuple(entry)
 
     def to_string(self, sep=None):
-        """ Convert the entry to a string using ``sep`` as a separator character.
+        """ Convert the entry to a string using ``sep`` as a
+        separator character.
 
         Parameters
         ----------
         sep : str or None
-            If None (the default), use the separator character defined during the entry object creation.
-            Otherwise, uses ``sep`` as the separator character.
+            If None (the default), use the separator character defined during
+            the entry object creation. Otherwise, uses ``sep`` as the
+            separator character.
 
         Examples
         --------
 
         >>> from luna.mol.entry import Entry
-        >>> e = Entry(pdb_id="3QL8", chain_id="A", comp_name="X01", comp_num=300, is_hetatm=True, sep=":")
+        >>> e = Entry(pdb_id="3QL8", chain_id="A", comp_name="X01", \
+comp_num=300, is_hetatm=True, sep=":")
         >>> print(e.to_string("/"))
         3QL8/A/X01/300
         """
 
         full_id = self.full_id
 
         # An entry object will always have a PDB and chain id.
         entry = list(full_id[0:2])
 
-        # If it contains additional information about the compound it will also include them.
+        # If it contains additional information about the molecule it
+        # will also include them.
         if len(full_id) > 2:
             if full_id[2] is not None and full_id[3] is not None:
                 comp_name = str(full_id[2]).strip()
-                comp_num_and_icode = str(full_id[3]).strip() + str(full_id[4]).strip()
+                comp_num_and_icode = \
+                    str(full_id[3]).strip() + str(full_id[4]).strip()
                 entry += [comp_name, comp_num_and_icode]
 
         sep = sep or self.sep
 
         return sep.join(entry)
 
     def is_valid(self):
-        """Check if the entry matches the expected format for protein-protein or protein-compound complexes.
+        """Check if the entry matches the expected format for protein-protein
+        or protein-molecule complexes.
 
         Returns
         -------
          : bool
         """
         full_id = self.full_id
 
@@ -384,47 +507,50 @@
         elif len(full_id) == 5:
             return PCI_ENTRY_REGEX.match(self.to_string(":")) is not None
 
         # Return False for anything else
         return False
 
     def get_biopython_key(self, full_id=False):
-        """Represent the entry as a key to select chains or compounds from Biopython Entity objects.
+        """Represent the entry as a key to select chains or molecules from
+        Biopython Entity objects.
 
         Parameters
         full_id : bool
             If True, return the full id of a chain or ligand.
-            For chains, it consists of a tuple containing the PDB and the chain id.
-            For ligands, it consists of a tuple containing the PDB, the chain, and the ligand id.
-            The default value is False.
+            For chains, it consists of a tuple containing the PDB and the
+            chain id. For ligands, it consists of a tuple containing the PDB,
+            the chain, and the ligand id. The default value is False.
 
         Returns
         -------
          : str or tuple
-            Return str if the entry represents a chain and if ``full_id`` is False.
-            Otherwise, return a tuple.
+            Return str if the entry represents a chain and if ``full_id``
+            is False. Otherwise, return a tuple.
 
         Examples
         --------
 
         >>> from luna.mol.entry import Entry
-        >>> e = Entry(pdb_id="3QL8", chain_id="A", comp_name="X01", comp_num=300, is_hetatm=True, sep=":")
+        >>> e = Entry(pdb_id="3QL8", chain_id="A", comp_name="X01", \
+comp_num=300, is_hetatm=True, sep=":")
         >>> print(e.get_biopython_key())
         ('H_X01', 300, ' ')
 
         """
         key = []
         if full_id:
             key = [self.pdb_id, 0, self.chain_id]
 
         if self.comp_name is not None and self.comp_num is not None:
             if self.comp_name == 'HOH' or self.comp_name == 'WAT':
                 comp_id = ('W', self.comp_num, self.comp_icode)
             elif self.is_hetatm:
-                comp_id = ('H_%s' % self.comp_name, self.comp_num, self.comp_icode)
+                comp_id = ('H_%s' % self.comp_name, self.comp_num,
+                           self.comp_icode)
             else:
                 comp_id = (' ', self.comp_num, self.comp_icode)
 
             if full_id:
                 key.append(comp_id)
                 return tuple(key)
             return comp_id
@@ -440,19 +566,21 @@
 
 class ChainEntry(Entry):
     """Define a chain.
 
     Parameters
     ----------
     pdb_id : str
-        A 4-symbols structure id from PDB or a local PDB filename. Example: '3QL8' or 'file1'.
+        A 4-symbols structure id from PDB or a local PDB filename.
+        Example: '3QL8' or 'file1'.
     chain_id : str
         A 1-symbol chain id. Example: 'A'.
     sep : str
-        A separator character to format the entry string. The default value is ':'.
+        A separator character to format the entry string.
+        The default value is ':'.
 
     Raises
     ------
     InvalidEntry
         If the provided information does not match the PDB format.
 
     Examples
@@ -461,95 +589,110 @@
     >>> e = ChainEntry(pdb_id="3QL8", chain_id="A")
     >>> print(e)
     <ChainEntry: 3QL8:A>
 
     """
 
     def __init__(self, pdb_id, chain_id, sep=ENTRY_SEPARATOR, parser=None):
-        super().__init__(pdb_id, chain_id, is_hetatm=False, sep=sep, parser=parser)
+        super().__init__(pdb_id, chain_id, is_hetatm=False, sep=sep,
+                         parser=parser)
 
     @classmethod
     def from_string(cls, entry_str, sep=ENTRY_SEPARATOR):
         """Initialize from a string.
 
         Parameters
         ----------
         entry_str : str
             A string representing the entry. Example: '3QL8:A'.
         sep : str
-            The separator character used in ``entry_str``. The default value is ':'.
-            For example: if ``entry_str`` is set to '3QL8|A', then ``sep`` should be defined as '|'.
+            The separator character used in ``entry_str``.
+            The default value is ':'. For example: if ``entry_str`` is set to
+            '3QL8|A', then ``sep`` should be defined as '|'.
 
         Returns
         -------
          : `Entry`
 
         Raises
         ------
         IllegalArgumentError
-            If the fields in ``entry_str`` do not match the format expected to define a chain.
+            If the fields in ``entry_str`` do not match the format expected
+            to define a chain.
 
         Examples
         --------
         >>> from luna.mol.entry import ChainEntry
         >>> e = ChainEntry.from_string("3QL8:A", sep=":")
         >>> print(e)
         <ChainEntry: 3QL8:A>
 
         """
         entries = entry_str.split(sep)
         if len(entries) == 2:
             return cls(*entries, sep=sep)
         else:
-            raise IllegalArgumentError("The number of fields in the informed string '%s' is incorrect. A valid string must contain "
-                                       "two obligatory fields: PDB and chain id." % entry_str)
+            error_msg = ("The number of fields in the informed string '%s' is "
+                         "incorrect. A valid string must contain two "
+                         "obligatory fields: PDB and chain id." % entry_str)
+            raise IllegalArgumentError(error_msg)
 
     @property
     def full_id(self):
-        """tuple, read-only: The full id of the entry is the tuple (PDB id or filename, chain id)."""
+        """tuple, read-only: The full id of the entry is the tuple
+        (PDB id or filename, chain id)."""
         return (self.pdb_id, self.chain_id)
 
 
 class MolEntry(Entry):
-    """Define a compound from a PDB file, which can be a residue, nucleotide, or ligand.
+    """Define a molecule from a PDB file, which can be a residue,
+    nucleotide, ligand, water, or ion.
 
     Parameters
     ----------
     pdb_id : str
-        A 4-symbols structure id from PDB or a local PDB filename. Example: '3QL8' or 'file1'.
+        A 4-symbols structure id from PDB or a local PDB filename.
+        Example: '3QL8' or 'file1'.
     chain_id : str
         A 1-symbol chain id. Example: 'A'.
     comp_name : str
-        A 1 to 3-symbols compound name (residue name in the PDB format). Example: 'X01'.
+        A 1 to 3-symbols molecule name (residue name in the PDB format).
+        Example: 'X01'.
     comp_num : int
-        A valid 4-digits integer (residue sequence number in the PDB format). Example: 300 or -1.
+        A valid 4-digits integer (residue sequence number in the PDB format).
+        Example: 300 or -1.
     comp_icode : str, optional
-        A 1-character compound insertion code (residue insertion code in the PDB format). Example: 'A'.
+        A 1-character molecule insertion code (residue insertion code in the
+        PDB format). Example: 'A'.
     sep : str
-        A separator character to format the entry string. The default value is ':'.
+        A separator character to format the entry string.
+        The default value is ':'.
 
     Raises
     ------
     InvalidEntry
         If the provided information does not match the PDB format.
 
     Examples
     --------
 
-    Compound entry: can be used to calculate interactions with a given compound (residue or nucleotide).
+    Molecule entry: can be used to calculate interactions with a given
+    molecule (residue or nucleotide).
 
     >>> from luna.mol.entry import MolEntry
-    >>> e = MolEntry(pdb_id="3QL8", chain_id="A", comp_name="HIS", comp_num=125, is_hetatm=False)
+    >>> e = MolEntry(pdb_id="3QL8", chain_id="A", comp_name="HIS", \
+comp_num=125, is_hetatm=False)
     >>> print(e)
     <MolEntry: 3QL8:A:HIS:125>
 
     Ligand entry: can be used to calculate interactions with a given ligand.
 
     >>> from luna.mol.entry import MolEntry
-    >>> e = MolEntry(pdb_id="3QL8", chain_id="A", comp_name="X01", comp_num=300, is_hetatm=True)
+    >>> e = MolEntry(pdb_id="3QL8", chain_id="A", comp_name="X01", \
+comp_num=300, is_hetatm=True)
     >>> print(e)
     <MolEntry: 3QL8:A:X01:300>
 
     """
 
     def __init__(self, pdb_id, chain_id, comp_name, comp_num,
                  comp_icode=None, sep=ENTRY_SEPARATOR, parser=None):
@@ -564,53 +707,65 @@
             # Separate ligand number from insertion code.
             matched = REGEX_RESNUM_ICODE.match(entries[3])
             if matched:
                 comp_num = matched.group(1)
                 icode = None if matched.group(2) == "" else matched.group(2)
                 entries = entries[0:3] + [comp_num, icode]
             else:
-                raise IllegalArgumentError("The compound number and its insertion code (if applicable) '%s' is invalid. "
-                                           "It must be an integer followed by one insertion code character when applicable." % entries[3])
+                error_msg = ("The molecule number and its insertion code "
+                             "(if applicable) '%s' is invalid. It must be an "
+                             "integer followed by one insertion code "
+                             "character when applicable." % entries[3])
+                raise IllegalArgumentError(error_msg)
             return cls(*entries, sep=sep)
         else:
-            raise IllegalArgumentError("The number of fields in the informed string '%s' is incorrect. A valid compound entry must contain "
-                                       "four obligatory fields: PDB, chain id, compound name, and compound number followed by its "
-                                       "insertion code when applicable." % entry_str)
+            error_msg = ("The number of fields in the informed string '%s' is "
+                         "incorrect. A valid molecule entry must contain four "
+                         "obligatory fields: PDB, chain id, molecule name, "
+                         "and molecule number followed by its insertion code "
+                         "when applicable." % entry_str)
+            raise IllegalArgumentError(error_msg)
 
 
 class MolFileEntry(Entry):
 
     """Define a ligand from a molecular file.
-    This class should be used for docking and molecular dynamics campaigns where usually one has
-    the protein structure in the PDB format and the ligand structure in a separate molecular file.
+    This class should be used for docking and molecular dynamics campaigns
+    where usually one has the protein structure in the PDB format and the
+    ligand structure in a separate molecular file.
 
     Parameters
     ----------
     pdb_id : str
-        A 4-symbols structure id from PDB or a local PDB filename. Example: '3QL8' or 'file1'.
+        A 4-symbols structure id from PDB or a local PDB filename.
+        Example: '3QL8' or 'file1'.
     mol_id : str
         The ligand id in the molecular file.
     sep : str
-        A separator character to format the entry string. The default value is ':'.
+        A separator character to format the entry string.
+        The default value is ':'.
 
     Attributes
     ----------
     mol_id : str
         The ligand id.
     mol_file : str
         Pathname of the molecular file.
     mol_file_ext : str
         The molecular file format.
-        If not provided, try to recover the molecular file extension directly from ``mol_file``.
+        If not provided, try to recover the molecular file extension
+        directly from ``mol_file``.
     mol_obj_type : {'rdkit', 'openbabel'}
-        Define which library (RDKit or Open Babel) to use to parse the molecular file.
+        Define which library (RDKit or Open Babel) to use to parse
+        the molecular file.
     overwrite_mol_name : bool
-        If True, substitute the ligand name in the parsed molecular object with ``mol_id``.
-        Only works for single-molecule files (``is_multimol_file`` = False)
-        as in these cases ``mol_id`` does not need to match the ligand name in the molecular file.
+        If True, substitute the ligand name in the parsed molecular object
+        with ``mol_id``. Only works for single-molecule files
+        (``is_multimol_file`` = False) as in these cases ``mol_id`` does not
+        need to match the ligand name in the molecular file.
     is_multimol_file : bool
         If ``mol_file`` contains multiple molecules or not.
         If True, ``mol_id`` should match some ligand name in ``mol_file``.
     """
 
     def __init__(self, pdb_id, mol_id, sep=ENTRY_SEPARATOR):
 
@@ -636,49 +791,59 @@
 
         This function is useful in cases where a molecular object is parsed and
         pre-processed using a different protocol defined by the user.
 
         Parameters
         ----------
         pdb_id : str
-            A 4-symbols structure id from PDB or a local PDB filename. Example: '3QL8' or 'file1'.
+            A 4-symbols structure id from PDB or a local PDB filename.
+            Example: '3QL8' or 'file1'.
         mol_id : str
             The ligand id.
-            As the molecular object is already provided, the ligand id does not need to match the ligand name in the molecular object.
-        mol_obj : :class:`~luna.wrappers.base.MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`
+            As the molecular object is already provided, the ligand id does
+            not need to match the ligand name in the molecular object.
+        mol_obj : :class:`~luna.wrappers.base.MolWrapper`, \
+                    :class:`rdkit.Chem.rdchem.Mol`, or \
+                    :class:`openbabel.pybel.Molecule`
             The molecular object.
         sep : str
-            A separator character to format the entry string. The default value is ':'.
+            A separator character to format the entry string.
+            The default value is ':'.
 
         Returns
         -------
          : `MolFileEntry`
 
         Raises
         ------
         MoleculeObjectTypeError
             If the molecular object is not an instance
-            of :class:`~luna.wrappers.base.MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`.
+            of :class:`~luna.wrappers.base.MolWrapper`,
+            :class:`rdkit.Chem.rdchem.Mol`,
+            or :class:`openbabel.pybel.Molecule`.
         IllegalArgumentError
             If ``entity`` is not a valid Biopython object.
 
         Examples
         --------
 
-        In this example, we will initialize a new MolFileEntry with the ligand 'ZINC000007786517' and
-        the structure located in a PDB file of name 'D4', which is the structure used for docking the molecule.
+        In this example, we will initialize a new MolFileEntry with the ligand
+        'ZINC000007786517' and the structure located in a PDB file of name
+        'D4', which is the structure used for docking the molecule.
 
         First, let's parse the molecular file.
 
         >>> from luna.wrappers.rdkit import read_mol_from_file
-        >>> mol_obj = read_mol_from_file("tutorial/inputs/ZINC000007786517.mol", mol_format="mol")
+        >>> mol_file = "tutorial/inputs/ZINC000007786517.mol"
+        >>> mol_obj = read_mol_from_file(mol_file, mol_format="mol")
 
         Now, we create the new MolFileEntry object as follows:
 
-        >>> e = MolFileEntry.from_mol_obj("D4", "ZINC000007786517", mol_obj, sep=ENTRY_SEPARATOR)
+        >>> e = MolFileEntry.from_mol_obj("D4", "ZINC000007786517",
+        ...                               mol_obj, sep=ENTRY_SEPARATOR)
         >>> print(e)
         <MolFileEntry: D4:ZINC000007786517>
         >>> print(e.mol_obj.to_smiles())
         Cc1cccc(NC(=O)C[N@@H+](C)C2CCCCC2)c1C
         """
 
         if mol_obj is not None:
@@ -695,16 +860,19 @@
                 logger.exception("Objects of type '%s' are not currently "
                                  "accepted." % mol_obj.__class__)
                 raise MoleculeObjectTypeError("Objects of type '%s' are not "
                                               "currently accepted."
                                               % mol_obj.__class__)
         else:
             if mol_obj_type not in ACCEPTED_MOL_OBJ_TYPES:
-                raise IllegalArgumentError("Objects of type '%s' are not currently accepted. "
-                                           "The available options are: %s." % (mol_obj_type, ", ".join(ACCEPTED_MOL_OBJ_TYPES)))
+                error_msg = ("Objects of type '%s' are not currently "
+                             "accepted. The available options are: %s."
+                             % (mol_obj_type,
+                                ", ".join(ACCEPTED_MOL_OBJ_TYPES)))
+                raise IllegalArgumentError(error_msg)
 
         entry = cls(pdb_id, mol_id, sep)
         entry.mol_obj = mol_obj
         entry.mol_obj_type = mol_obj_type
 
         # TODO: Find a way to assume the Mol file type when not provided
         # mol_file_ext
@@ -717,90 +885,111 @@
                       autoload=False, overwrite_mol_name=False,
                       sep=ENTRY_SEPARATOR):
         """Initialize from a molecular file.
 
         Parameters
         ----------
         pdb_id : str
-            A 4-symbols structure id from PDB or a local PDB filename. Example: '3QL8' or 'file1'.
+            A 4-symbols structure id from PDB or a local PDB filename.
+            Example: '3QL8' or 'file1'.
         mol_id : str
             The ligand id in the molecular file.
         mol_file : str
             Pathname of the molecular file.
         is_multimol_file : bool
             If ``mol_file`` contains multiple molecules or not.
             If True, ``mol_id`` should match some ligand name in ``mol_file``.
         mol_file_ext : str, optional
             The molecular file format.
-            If not provided, try to recover the molecular file extension directly from ``mol_file``.
+            If not provided, try to recover the molecular file extension
+            directly from ``mol_file``.
         mol_obj_type : {'rdkit', 'openbabel'}
-            If "rdkit", parse the converted molecule with RDKit and return an instance of :class:`rdkit.Chem.rdchem.Mol`.
-            If "openbabel", parse the converted molecule with Open Babel and return an instance of
+            If "rdkit", parse the converted molecule with RDKit and return an
+            instance of :class:`rdkit.Chem.rdchem.Mol`. If "openbabel", parse
+            the converted molecule with Open Babel and return an instance of
             :class:`openbabel.pybel.Molecule`. The default value is 'rdkit'.
         autoload : bool
-            If True, parse the ligand from the molecular file during the entry initialization.
-            Otherwise, only load the ligand when first used.
+            If True, parse the ligand from the molecular file during the entry
+            initialization. Otherwise, only load the ligand when first used.
         overwrite_mol_name : bool
-            If True, substitute the ligand name in the parsed molecular object with ``mol_id``.
-            Only works for single-molecule files (``is_multimol_file`` = False)
-            as in these cases ``mol_id`` does not need to match the ligand name in the molecular file.
+            If True, substitute the ligand name in the parsed molecular object
+            with ``mol_id``. Only works for single-molecule files
+            (``is_multimol_file`` = False) as in these cases ``mol_id`` does
+            not need to match the ligand name in the molecular file.
         sep : str
-            A separator character to format the entry string. The default value is ':'.
+            A separator character to format the entry string.
+            The default value is ':'.
 
         Returns
         -------
          : `MolFileEntry`
 
         Raises
         ------
         FileNotFoundError
             If ``mol_file`` does not exist.
         IllegalArgumentError
             If ``mol_obj_type`` is not either 'rdkit' nor 'openbabel'.
         MoleculeObjectError
-            If any errors occur while parsing the molecular file.
-            Detailed information about the errors can be found in the logging outputs.
+            If any errors occur while parsing the molecular file. Detailed
+            information about the errors can be found in the logging outputs.
         MoleculeNotFoundError
-            If the ligand ``mol_id`` was not found in the input file and ``is_multimol_file`` is True.
+            If the ligand ``mol_id`` was not found in the input file and
+            ``is_multimol_file`` is True.
 
         Examples
         --------
 
-        In this first example, we will read the ligand 'ZINC000007786517' from a single-molecule file.
-        As we are working with a single-molecule file, ``mol_id`` can be any value you prefer.
+        In this first example, we will read the ligand 'ZINC000007786517' from
+        a single-molecule file. As we are working with a single-molecule file,
+        ``mol_id`` can be any value you prefer.
 
         >>> from luna.mol.entry import MolFileEntry
-        >>> e = MolFileEntry.from_mol_file(pdb_id="D4", mol_id="Ligand", mol_file="tutorial/inputs/ZINC000007786517.mol",
-        ...                                mol_obj_type='rdkit', is_multimol_file=False)
+        >>> mol_file = "tutorial/inputs/ZINC000007786517.mol"
+        >>> e = MolFileEntry.from_mol_file(pdb_id="D4", mol_id="Ligand",
+        ...                                mol_file=mol_file, \
+mol_obj_type='rdkit',
+        ...                                is_multimol_file=False)
         >>> print(e)
         D4:Ligand
         >>> print(e.mol_obj.to_smiles())
         Cc1cccc(NC(=O)C[N@@H+](C)C2CCCCC2)c1C
 
-        Now, let's say we need to read the ligand 'ZINC000096459890' from a multi-molecular file and that we
-        want to use Open Babel to parse the molecule.
-        To do so, remember that it should exist a ligand with the name ``mol_id`` in ``mol_file``.
-        Otherwise, it will raise the exception MoleculeNotFoundError.
+        Now, let's say we need to read the ligand 'ZINC000096459890' from a
+        multi-molecular file and that we want to use Open Babel to parse the
+        molecule. To do so, remember that it should exist a ligand with the
+        name ``mol_id`` in ``mol_file``. Otherwise, it will raise the
+        exception MoleculeNotFoundError.
 
         >>> from luna.mol.entry import MolFileEntry
-        >>> e = MolFileEntry.from_mol_file(pdb_id="D4", mol_id="ZINC000096459890", mol_file="tutorial/inputs/ligands.mol2",
-        ...                                mol_obj_type='openbabel', is_multimol_file=True)
+        >>> mol_file = "tutorial/inputs/ligands.mol2"
+        >>> e = MolFileEntry.from_mol_file(pdb_id="D4", \
+mol_id="ZINC000096459890",
+        ...                                mol_file=mol_file, \
+mol_obj_type='openbabel',
+        ...                                is_multimol_file=True)
         >>> print(e)
         <MolFileEntry: D4:ZINC000096459890>
         >>> print(e.mol_obj.to_smiles())
         O=C(OCCCN1C=CC=CC1=O)c1ccc2ccc(Cl)cc2n1
 
-        Below, we show what happens if ``mol_id`` does not exist in ``mol_file``. Observe we set ``autoload`` to True
-        to parse the molecule right away.
+        Below, we show what happens if ``mol_id`` does not exist in
+        ``mol_file``. Observe we set ``autoload`` to True to parse the
+        molecule right away.
 
         >>> from luna.mol.entry import MolFileEntry
-        >>> e = MolFileEntry.from_mol_file(pdb_id="D4", mol_id="Ligand", mol_file="tutorial/inputs/ligands.mol2",
-        ...                                mol_obj_type='openbabel', is_multimol_file=True, autoload=True)
-        luna.util.exceptions.MoleculeNotFoundError: "The ligand 'Ligand' was not found in the input file \
-        or generated errors while parsing it with Open Babel."
+        >>> mol_file = "tutorial/inputs/ligands.mol2"
+        >>> e = MolFileEntry.from_mol_file(pdb_id="D4", mol_id="Ligand",
+        ...                                mol_file=mol_file, \
+mol_obj_type='openbabel',
+        ...                                 is_multimol_file=True, \
+autoload=True)
+        luna.util.exceptions.MoleculeNotFoundError: "The ligand 'Ligand' was \
+not found in the
+        input file or generated errors while parsing it with Open Babel."
         """
 
         entry = cls(pdb_id, mol_id, sep)
 
         entry.mol_file = mol_file
         entry.is_multimol_file = is_multimol_file
         entry.mol_file_ext = mol_file_ext or get_file_format(mol_file)
@@ -854,20 +1043,23 @@
                                         curr_mol_file,
                                         is_multimol_file=is_multimol_file,
                                         **kwargs)
                 c += 1
 
     @property
     def full_id(self):
-        """tuple, read-only: The full id of the entry is the tuple (PDB id or filename, ligand id)."""
+        """tuple, read-only: The full id of the entry is the tuple
+        (PDB id or filename, ligand id)."""
         return (self.pdb_id, self.mol_id)
 
     @property
     def mol_obj(self):
-        """:class:`~luna.wrappers.base.MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`: The molecule."""
+        """:class:`~luna.wrappers.base.MolWrapper`, \
+        :class:`rdkit.Chem.rdchem.Mol`, \
+        or :class:`openbabel.pybel.Molecule`: The molecule."""
         if self._mol_obj is None and self.mol_file is not None:
             self._load_mol_from_file()
         return self._mol_obj
 
     @mol_obj.setter
     def mol_obj(self, mol_obj):
         self._mol_obj = MolWrapper(mol_obj)
@@ -890,143 +1082,179 @@
         """
         return self._mol_obj is not None
 
     def _load_mol_from_file(self):
         logger.debug("It will try to load the molecule '%s'." % self.mol_id)
 
         if self.mol_file is None:
-            raise IllegalArgumentError("It cannot load the molecule as no molecular file was provided.")
+            raise IllegalArgumentError("It cannot load the molecule as no "
+                                       "molecular file was provided.")
 
-        available_formats = OB_FORMATS if self.mol_obj_type == "openbabel" else RDKIT_FORMATS
+        available_formats = (OB_FORMATS if self.mol_obj_type == "openbabel"
+                             else RDKIT_FORMATS)
         tool = "Open Babel" if self.mol_obj_type == "openbabel" else "RDKit"
         if self.mol_file_ext not in available_formats:
-            raise IllegalArgumentError("Extension '%s' informed or assumed from the filename is not a format "
-                                       "recognized by %s." % (self.mol_file_ext, tool))
+            raise IllegalArgumentError("Extension '%s' informed or assumed "
+                                       "from the filename is not a format "
+                                       "recognized by %s."
+                                       % (self.mol_file_ext, tool))
 
         if not exists(self.mol_file):
-            raise FileNotFoundError("The file '%s' was not found." % self.mol_file)
+            raise FileNotFoundError("The file '%s' was not found."
+                                    % self.mol_file)
 
         try:
             if self.mol_obj_type == "openbabel":
                 mols = readfile(self.mol_file_ext, self.mol_file)
-                # If it is a multimol file, then we need to loop over the molecules to find the target one.
-                # Note that in this case, the ids must match.
+                # If it is a multimol file, then we need to loop over the
+                # molecules to find the target one. Note that in this case,
+                # the ids must match.
                 if self.is_multimol_file:
                     for ob_mol in mols:
-                        if self.mol_id == get_filename(ob_mol.OBMol.GetTitle()):
+                        filename = get_filename(ob_mol.OBMol.GetTitle())
+                        if self.mol_id == filename:
                             self.mol_obj = ob_mol
                             break
                 else:
                     self.mol_obj = mols.__next__()
             else:
                 if self.mol_file_ext == "pdb":
-                    self.mol_obj = read_mol_from_file(self.mol_file, mol_format=self.mol_file_ext, removeHs=False)
+                    self.mol_obj = \
+                        read_mol_from_file(self.mol_file,
+                                           mol_format=self.mol_file_ext,
+                                           removeHs=False)
                 else:
-                    # If 'targets' is None, then the entire Mol file will be read.
+                    # If 'targets' is None, then the entire Mol file
+                    # will be read.
                     targets = None
-                    # If it is a multimol file than loop through it until the informed molecule (by its mol_id) is found.
+                    # If it is a multimol file than loop through it until the
+                    # informed molecule (by its mol_id) is found.
                     if self.is_multimol_file:
                         targets = [self.mol_id]
 
-                    for rdk_mol, mol_id in read_multimol_file(self.mol_file, mol_format=self.mol_file_ext, targets=targets, removeHs=False):
-                        # It returns None if the molecule parsing generated errors.
+                    for rdk_mol, mol_id \
+                        in read_multimol_file(self.mol_file,
+                                              mol_format=self.mol_file_ext,
+                                              targets=targets,
+                                              removeHs=False):
+                        # It returns None if the molecule parsing
+                        # generated errors.
                         self.mol_obj = rdk_mol
                         break
         except Exception as e:
             logger.exception(e)
-            raise MoleculeObjectError("An error occurred while parsing the molecular file with %s and the molecule "
-                                      "object for the entry '%s' could not be created. Check the logs for more information."
-                                      % (tool, self.to_string()))
+
+            error_msg = ("An error occurred while parsing the molecular file "
+                         "with %s and the molecule object for the entry '%s' "
+                         "could not be created. Check the logs for more "
+                         "information." % (tool, self.to_string()))
+            raise MoleculeObjectError(error_msg)
 
         if self._mol_obj is None:
-            raise MoleculeNotFoundError("The ligand '%s' was not found in the input file or generated errors while parsing it with %s."
-                                        % (self.mol_id, tool))
+            error_msg = ("The ligand '%s' was not found in the input file or "
+                         "generated errors while parsing it with %s."
+                         % (self.mol_id, tool))
+            raise MoleculeNotFoundError(error_msg)
         else:
             if not self.mol_obj.has_name() or self.overwrite_mol_name:
                 self.mol_obj.set_name(self.mol_id)
 
         logger.debug("Molecule '%s' was successfully loaded." % self.mol_id)
 
     def get_biopython_structure(self, entity=None, parser=None):
         """Transform the molecular object into a Biopython Entity object.
 
-        If ``entity`` is provided, the molecular object is appended to it, i.e., this function
-        can be used to join a ligand and the structure used during docking or molecular dynamics.
+        If ``entity`` is provided, the molecular object is appended to it,
+        i.e., this function can be used to join a ligand and the structure
+        used during docking or molecular dynamics.
 
         By default, the ligand is added to a chain of id `z`.
 
         Parameters
         ----------
         entity : :class:`~luna.MyBio.PDB.Entity.Entity`, optional
             Append the molecular object to ``entity``.
-            If not provided, a new :class:`~luna.MyBio.PDB.Entity.Entity` is created.
+            If not provided, a new :class:`~luna.MyBio.PDB.Entity.Entity`
+            is created.
         parser : :class:`~luna.MyBio.PDB.PDBParser.PDBParser`, optional
-            Define a PDB parser object. If not provided, the default parser will be used.
+            Define a PDB parser object. If not provided, the default parser
+            will be used.
 
         Returns
         -------
          : :class:`~luna.MyBio.PDB.Entity.Entity`
 
         Raises
         ------
         IllegalArgumentError
             If ``entity`` is not a valid Biopython object.
 
         Examples
         --------
 
-        In this example, we will demonstrate how to join a protein structure and a ligand docked against it.
+        In this example, we will demonstrate how to join a protein structure
+        and a ligand docked against it.
 
         First, let's parse the PDB file.
 
         >>> from luna.MyBio.PDB.PDBParser import PDBParser
         >>> pdb_parser = PDBParser(PERMISSIVE=True, QUIET=True)
-        >>> structure = pdb_parser.get_structure("Protein", "tutorial/inputs/D4.pdb")
+        >>> pdb_file = "tutorial/inputs/D4.pdb"
+        >>> structure = pdb_parser.get_structure("Protein", pdb_file)
 
-        Observe that the list of chains in the parsed structure contains only one element.
+        Observe that the list of chains in the parsed structure contains
+        only one element.
 
         >>> print(structure[0].child_list)
         [<Chain id=A>]
 
-        Now, we will read the ligand and append it to the existing protein structure.
+        Now, we will read the ligand and append it to the existing protein
+        structure.
 
         >>> from luna.mol.entry import MolFileEntry
-        >>> e = MolFileEntry.from_mol_file("D4", "ZINC000007786517", "tutorial/inputs/ZINC000007786517.mol",
-        ...                                mol_obj_type='rdkit', is_multimol_file=False)
+        >>> mol_file = "tutorial/inputs/ZINC000007786517.mol"
+        >>> e = MolFileEntry.from_mol_file("D4", "ZINC000007786517", mol_file,
+        ...                                mol_obj_type='rdkit', \
+is_multimol_file=False)
         >>> joined_structure = e.get_biopython_structure(structure)
 
-        Observe that now the list of chains contains chains 'A' and 'z', which is the default chain where
-        ligands are added.
+        Observe that now the list of chains contains chains 'A' and 'z',
+        which is the default chain where ligands are added.
 
         >>> print(joined_structure[0].child_list)
         [<Chain id=A>, <Chain id=z>]
 
         If we loop over the residues in chain 'z', we will find our ligand.
 
         >>> for r in structure[0]["z"]:
         >>>     print(r)
         <Residue LIG het=H_LIG resseq=9999 icode= >
         """
 
         if parser is None:
-            parser = PDBParser(PERMISSIVE=True, QUIET=True, FIX_EMPTY_CHAINS=True,
-                               FIX_ATOM_NAME_CONFLICT=True, FIX_OBABEL_FLAGS=False)
+            parser = PDBParser(PERMISSIVE=True, QUIET=True,
+                               FIX_EMPTY_CHAINS=True,
+                               FIX_ATOM_NAME_CONFLICT=True,
+                               FIX_OBABEL_FLAGS=False)
 
         mol_file_ext = self.mol_file_ext
         if mol_file_ext is None and self.mol_file is not None:
             mol_file_ext = get_file_format(self.mol_file)
 
         if self.mol_obj_type == "openbabel":
             pdb_block = self.mol_obj.to_pdb_block()
 
             atm = self.mol_obj.unwrap().GetFirstAtom()
             residue_info = atm.GetResidue()
 
-            # When the PDBParser finds an empty chain, it automatically replace it by 'z'.
-            chain_id = residue_info.GetChain() if residue_info.GetChain().strip() != "" else self.chain_id
+            # When the PDBParser finds an empty chain, it automatically
+            # replace it by 'z'.
+            chain_id = (residue_info.GetChain()
+                        if residue_info.GetChain().strip() != ""
+                        else self.chain_id)
             comp_num = residue_info.GetNum()
 
             if residue_info.GetName() in WATER_NAMES:
                 comp_name = "W"
             elif residue_info.IsHetAtom(atm):
                 comp_name = "H_%s" % residue_info.GetName()
             else:
@@ -1037,64 +1265,74 @@
                 self.comp_name = residue_info.GetName()
                 self.comp_num = comp_num
                 self.is_hetatm = residue_info.IsHetAtom(atm)
         else:
             pdb_block = self.mol_obj.to_pdb_block()
 
             if mol_file_ext == "pdb":
-                residue_info = self.mol_obj.unwrap().GetAtoms()[0].GetPDBResidueInfo()
-                # When the PDBParser finds an empty chain, it automatically replace it by 'z'.
-                chain_id = residue_info.GetChainId() if residue_info.GetChainId().strip() != "" else self.chain_id
+                residue_info = (self.mol_obj.unwrap()
+                                .GetAtoms()[0].GetPDBResidueInfo())
+                # When the PDBParser finds an empty chain, it automatically
+                # replace it by 'z'.
+                chain_id = (residue_info.GetChainId()
+                            if residue_info.GetChainId().strip() != ""
+                            else self.chain_id)
                 comp_num = residue_info.GetResidueNumber()
 
                 if residue_info.GetResidueName() in WATER_NAMES:
                     comp_name = "W"
                 elif residue_info.GetIsHeteroAtom():
                     comp_name = "H_%s" % residue_info.GetResidueName()
                 else:
                     comp_name = " "
 
                 self.chain_id = chain_id
                 self.comp_name = residue_info.GetResidueName()
                 self.comp_num = comp_num
                 self.is_hetatm = residue_info.GetIsHeteroAtom()
             else:
-                # When the PDBParser finds an empty chain, it automatically replace it by 'z'.
+                # When the PDBParser finds an empty chain,
+                # it automatically replace it by 'z'.
                 chain_id = self.chain_id
                 comp_name = "H_UNL"
                 comp_num = 1
 
-        comp_structure = parser.get_structure_from_pdb_block(self.pdb_id, pdb_block)
+        comp_structure = parser.get_structure_from_pdb_block(self.pdb_id,
+                                                             pdb_block)
 
         chain = comp_structure[0][chain_id]
         if self.chain_id != chain.id:
             chain.id = self.chain_id
 
         lig = chain[(comp_name, comp_num, " ")]
 
-        # It only substitutes the ligand id if it is different from the id defined by the MolFileEntry object property.
-        # This update will never happen when the ligand file is a PDB file as the ids are guaranteed to be equal.
+        # It only substitutes the ligand id if it is different from the id
+        # defined by the MolFileEntry object property. This update will never
+        # happen when the ligand file is a PDB file as the ids are guaranteed
+        # to be equal.
         if lig.id != ("H_%s" % self.comp_name, self.comp_num, " "):
             lig.id = ("H_%s" % self.comp_name, self.comp_num, " ")
 
         lig.resname = self.comp_name
 
         if entity is not None:
             if isinstance(entity, Entity):
                 structure = entity.get_parent_by_level('S')
                 if self.chain_id not in structure[0].child_dict:
                     chain = chain.copy()
                     structure[0].add(chain)
                 else:
                     lig = lig.copy()
-                    # Update the ligand index according to the number of compounds already present in the chain.
+                    # Update the ligand index according to the number of
+                    # molecules already present in the chain.
                     lig.idx = len(structure[0][self.chain_id].child_list)
                     structure[0][self.chain_id].add(lig)
             else:
-                raise IllegalArgumentError("The informed entity is not a valid Biopython object.")
+                raise IllegalArgumentError("The informed entity is not a "
+                                           "valid Biopython object.")
         else:
             entity = comp_structure
 
         return entity
 
     def __repr__(self):
         return '<MolFileEntry: %s%s%s>' % (self.pdb_id, self.sep, self.mol_id)
@@ -1104,54 +1342,67 @@
             self.mol_obj = MolWrapper(self.mol_obj)
         return self.__dict__
 
     def __setstate__(self, state):
         self.__dict__.update(state)
 
 
-def recover_entries_from_entity(entity, get_small_molecules=True, get_chains=False,
-                                ignore_artifacts=True, by_cluster=False, sep=ENTRY_SEPARATOR):
-    """ Search for chains and small molecules in ``entity`` and return them as strings.
+def recover_entries_from_entity(entity, get_small_molecules=True,
+                                get_chains=False, ignore_artifacts=True,
+                                by_cluster=False, sep=ENTRY_SEPARATOR):
+    """ Search for chains and small molecules in ``entity`` and return
+    them as strings.
 
     Parameters
     ----------
     entity : :class:`~luna.MyBio.PDB.Entity.Entity`
         An entity from where chains or small molecules will be recovered.
     get_small_molecules : bool
-        If True, identify small molecules and return them as `MolEntry` objects. The default value is True.
+        If True, identify small molecules and return them as `MolEntry`
+        objects. The default value is True.
     get_chains : bool
-        If True, identify chains and return them as `ChainEntry` objects. The default value is False.
+        If True, identify chains and return them as `ChainEntry` objects.
+        The default value is False.
     ignore_artifacts : bool
-        If True, ignore the following crystallography artifacts: ACE, ACT, BME, CSD, CSW, EDO, FMT, GOL, MSE,
-        NAG, NO3, PO4, SGM, SO4, or TPO. The default value is True.
+        If True, ignore the following crystallography artifacts: ACE, ACT,
+        BME, CSD, CSW, EDO, FMT, GOL, MSE, NAG, NO3, PO4, SGM, SO4, or
+        TPO. The default value is True.
     by_cluster : bool
-        If True, aggregate entries by cluster. Cluster ids are exclusive to :class:`~luna.MyBio.PDB.Residue.Residue` instances and are
-        automatically set by :class:`~luna.MyBio.PDB.FTMapParser.FTMapParser`, a parser for FTMap results.
-        By default, the cluster id of :class:`~luna.MyBio.PDB.Residue.Residue` instances are set to None, therefore,
-        if the cluster id is not explicitly defined, all entries will be aggregated to the same key ``None``.
+        If True, aggregate entries by cluster. Cluster ids are exclusive
+        to :class:`~luna.MyBio.PDB.Residue.Residue` instances and are
+        automatically set by :class:`~luna.MyBio.PDB.FTMapParser.FTMapParser`,
+        a parser for FTMap results. By default, the cluster id of
+        :class:`~luna.MyBio.PDB.Residue.Residue` instances are set to None,
+        therefore, if the cluster id is not explicitly defined, all entries
+        will be aggregated to the same key ``None``.
     sep : str
-        A separator character to format the entry string. The default value is ':'.
+        A separator character to format the entry string.
+        The default value is ':'.
 
     Returns
     ------
      : list or dict
-        If ``by_cluster`` is set to False, a list of `ChainEntry` or `MolEntry` objects is returned.
-        Otherwise, a dict is returned, in which keys are clusters and values are lists of `ChainEntry` or `MolEntry` objects.
-        When no cluster information is available, all entries are aggregated in a key of value ``None``.
-        Cluster ids are exclusive to :class:`~luna.MyBio.PDB.Residue.Residue` instances, therefore, `ChainEntry` objects
-        are always placed in a key of value ``None``.
+        If ``by_cluster`` is set to False, a list of `ChainEntry` or
+        `MolEntry` objects is returned. Otherwise, a dict is returned,
+        in which keys are clusters and values are lists of `ChainEntry`
+        or `MolEntry` objects. When no cluster information is available, all
+        entries are aggregated in a key of value ``None``. Cluster ids are
+        exclusive to :class:`~luna.MyBio.PDB.Residue.Residue` instances,
+        therefore, `ChainEntry` objects are always placed in a key of
+        value ``None``.
 
     Examples
     --------
 
     First, let's parse a PDB file.
 
     >>> from luna.MyBio.PDB.PDBParser import PDBParser
     >>> pdb_parser = PDBParser(PERMISSIVE=True, QUIET=True)
-    >>> structure = pdb_parser.get_structure("Protein", "tutorial/inputs/3QQK.pdb")
+    >>> pdb_file = "tutorial/inputs/3QQK.pdb"
+    >>> structure = pdb_parser.get_structure("Protein", pdb_file)
 
     Now, we can recover entries from the parsed PDB file:
 
     >>> from luna.mol.entry import recover_entries_from_entity
     >>> entries = recover_entries_from_entity(structure, get_chains=True)
     >>> for e in entries:
     >>>     print(e)
@@ -1172,34 +1423,37 @@
     elif entity.level == "M":
         if get_small_molecules:
             residues = entity.get_residues()
         if get_chains:
             chains = entity.get_chains()
     else:
         if get_small_molecules:
-            # If the entity is already a Chain, get_parent_by_level() returns the same object.
-            # But, if the entity is a Residue or Atom, it will return its corresponding chain parent.
+            # If the entity is already a Chain, get_parent_by_level() returns
+            # the same object. But, if the entity is a Residue or Atom, it will
+            # return its corresponding chain parent.
             residues = entity.get_parent_by_level("C").get_residues()
         if get_chains:
             chains = entity.get_parent_by_level("M").get_chains()
 
     if get_small_molecules:
         pdb_id = entity.get_parent_by_level("S").id
         for res in residues:
             if res.is_hetatm():
                 if ignore_artifacts and res.resname in ARTIFACTS_LIST:
                     continue
 
                 comp_num_and_icode = ""
                 if isinstance(res.id[1], int):
                     comp_num_and_icode = str(res.id[1])
-                comp_num_and_icode += str(res.id[2]) if res.id[2].strip() else ""
+                comp_num_and_icode += \
+                    str(res.id[2]) if res.id[2].strip() else ""
 
                 entry = MolEntry.from_string(sep.join([pdb_id, res.parent.id,
-                                                       res.resname, comp_num_and_icode]))
+                                                       res.resname,
+                                                       comp_num_and_icode]))
                 if by_cluster:
                     clusters[res.cluster_id].append(entry)
                 else:
                     entries.append(entry)
 
     if get_chains:
         pdb_id = entity.get_parent_by_level("S").id
```

### Comparing `luna-0.12.2/luna/mol/features.py` & `luna-0.13.0/luna/mol/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 
     def format_name(self, case_func="sentencecase"):
         """Convert chemical feature names to another string case.
 
         Parameters
         ----------
         name : str
-            The name of a string case function from :py:mod:`luna.util.stringcase`.
+            The name of a string case function from
+            :py:mod:`luna.util.stringcase`.
         """
 
         func = getattr(case, case_func)
         return func(self.name)
 
     # Special methods
     def __repr__(self):
@@ -56,15 +57,16 @@
         return self.name < other.name
 
     def __hash__(self):
         return hash(self.name)
 
 
 class OBMolChemicalFeature:
-    """Mimic :class:`rdkit.Chem.rdMolChemicalFeatures.MolChemicalFeature` for Open Babel.
+    """Mimic :class:`rdkit.Chem.rdMolChemicalFeatures.MolChemicalFeature`
+    for Open Babel.
 
     Parameters
     ----------
     family : str
         The family name, which is the term used by RDKit for chemical features.
     atom_ids : list
         List of atom identifiers.
@@ -75,35 +77,38 @@
         self.atom_ids = atom_ids
 
     def GetAtomIds(self):
         """Get the IDs of the atoms that participate in the feature."""
         return self.atom_ids
 
     def GetFamily(self):
-        """Get the family to which the feature belongs (e.g., donor, acceptor, etc.)"""
+        """Get the family to which the feature belongs (e.g., donor,
+        acceptor, etc.)"""
         return self.family
 
 
 class FeatureExtractor:
     """Perceive chemical features from molecules.
 
     Parameters
     ----------
-    feature_factory : :class:`~rdkit.Chem.rdMolChemicalFeatures.MolChemicalFeatureFactory`
-        An RDKit feature factory.
+    feature_factory : \
+        :class:`~rdkit.Chem.rdMolChemicalFeatures.MolChemicalFeatureFactory`
+            An RDKit feature factory.
 
     Examples
     --------
 
     First, let's read a molecule (glutamine).
 
     >>> from luna.wrappers.base import MolWrapper
     >>> mol = MolWrapper.from_smiles("N[C@@H](CCC(N)=O)C(O)=O").unwrap()
 
-    Now, create a feature factory and instantiate a new `FeatureExtractor` object.
+    Now, create a feature factory and instantiate a new
+    `FeatureExtractor` object.
 
     >>> from luna.util.default_values import ATOM_PROP_FILE
     >>> from rdkit.Chem import ChemicalFeatures
     >>> from luna.mol.features import FeatureExtractor
     >>> feature_factory = ChemicalFeatures.BuildFeatureFactory(ATOM_PROP_FILE)
     >>> feature_extractor = FeatureExtractor(feature_factory)
 
@@ -118,94 +123,101 @@
         self.feature_factory = feature_factory
 
     def get_features_by_atoms(self, mol_obj, atm_map=None):
         """Perceive chemical features from the molecule ``mol_obj`` by atom.
 
         Parameters
         ----------
-        mol_obj : :class:`~luna.wrappers.base.MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`
+        mol_obj : :class:`~luna.wrappers.base.MolWrapper`, \
+                :class:`rdkit.Chem.rdchem.Mol`, or \
+                :class:`openbabel.pybel.Molecule`
             The molecule.
         atm_map : dict
             A dictionary to map an atom's index to a different value.
 
         Returns
         -------
         atm_features : dict of {int : list of `ChemicalFeature`}
-            Chemical features by atoms that are represented by their index or by a value from ``atm_map``.
+            Chemical features by atoms that are represented by their index or
+            by a value from ``atm_map``.
 
         """
         if isinstance(mol_obj, MolWrapper):
             mol_obj = mol_obj.unwrap()
 
         if isinstance(mol_obj, RDMol):
-            perceived_features = self.feature_factory.GetFeaturesForMol(mol_obj)
+            perceived_features = \
+                self.feature_factory.GetFeaturesForMol(mol_obj)
         elif isinstance(mol_obj, OBMol):
             perceived_features = self._get_features_from_obmol(mol_obj)
         elif isinstance(mol_obj, PybelMol):
             perceived_features = self._get_features_from_obmol(mol_obj.OBMol)
         else:
-            logger.exception("Objects of type '%s' are not currently accepted." % mol_obj.__class__)
-            raise MoleculeObjectTypeError("Objects of type '%s' are not currently accepted." % mol_obj.__class__)
+            error_msg = ("Objects of type '%s' are not currently accepted."
+                         % mol_obj.__class__)
+            logger.exception(error_msg)
+            raise MoleculeObjectTypeError(error_msg)
 
         atm_features = defaultdict(set)
         for f in perceived_features:
             for atm_idx in f.GetAtomIds():
                 tmp_atm_idx = atm_idx
                 if atm_map is not None:
                     if atm_idx in atm_map:
                         tmp_atm_idx = atm_map[atm_idx]
                     else:
-                        logger.warning("There is no corresponding mapping to the index '%d'. It will be ignored." % atm_idx)
+                        logger.warning("There is no corresponding mapping to "
+                                       "the index '%d'. It will be ignored."
+                                       % atm_idx)
 
                 feature = ChemicalFeature(f.GetFamily())
                 atm_features[tmp_atm_idx].add(feature)
 
         return atm_features
 
     def get_features_by_groups(self, mol_obj, atm_map=None):
-        """Perceive chemical features from the molecule
-        ``mol_obj`` by atom groups.
+        """Perceive chemical features from the molecule ``mol_obj``
+        by atom groups.
 
         Parameters
         ----------
         mol_obj : :class:`~luna.wrappers.base.MolWrapper`, \
-            :class:`rdkit.Chem.rdchem.Mol`, \
-            or :class:`openbabel.pybel.Molecule`
-                The molecule.
+                :class:`rdkit.Chem.rdchem.Mol`, or \
+                :class:`openbabel.pybel.Molecule`
+            The molecule.
         atm_map : dict
             A dictionary to map an atom's index to a different value.
 
         Returns
         -------
         grp_features : dict of {str : dict}
-            Chemical features by groups.
-            Each dictionary value is defined as follows:
+            Chemical features by groups. Each dictionary value is
+            defined as follows:
 
-            * ``atm_ids`` (list): list of atoms represented by
-            their index or by a value from ``atm_map`` ;
-            * ``features`` (list of `ChemicalFeature`): list of
-            chemical features.
+            * ``atm_ids`` (list): list of atoms represented by their \
+                    index or by a value from ``atm_map`` ;
+            * ``features`` (list of `ChemicalFeature`): list of chemical \
+                    features.
 
         """
         if isinstance(mol_obj, MolWrapper):
             mol_obj = mol_obj.unwrap()
 
         if isinstance(mol_obj, RDMol):
             perceived_features = \
                 self.feature_factory.GetFeaturesForMol(mol_obj)
         elif isinstance(mol_obj, OBMol):
             perceived_features = self._get_features_from_obmol(mol_obj)
         elif isinstance(mol_obj, PybelMol):
             perceived_features = self._get_features_from_obmol(mol_obj.OBMol)
         else:
-            logger.exception("Objects of type '%s' are not currently "
-                             "accepted." % mol_obj.__class__)
-            raise MoleculeObjectTypeError("Objects of type '%s' are not "
-                                          "currently accepted."
-                                          % mol_obj.__class__)
+            error_msg = ("Objects of type '%s' are not currently accepted."
+                         % mol_obj.__class__)
+            logger.exception(error_msg)
+            raise MoleculeObjectTypeError(error_msg)
 
         grp_features = {}
         for f in perceived_features:
             atm_ids = sorted(list(f.GetAtomIds()))
 
             if atm_map is not None:
                 tmp_atm_ids = []
```

### Comparing `luna-0.12.2/luna/mol/fingerprint.py` & `luna-0.13.0/luna/mol/fingerprint.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,51 +18,59 @@
 
 
 class FingerprintGenerator():
     """Generate molecular fingerprints for the molecule ``mol``.
 
     Parameters
     ----------
-    mol : :class:`~luna.wrappers.base.MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`, optional
+    mol : :class:`~luna.wrappers.base.MolWrapper`, \
+            :class:`rdkit.Chem.rdchem.Mol`, or \
+            :class:`openbabel.pybel.Molecule`, optional
         The molecule.
 
     Examples
     --------
 
     First, create a new `FingerprintGenerator` object.
 
     >>> from luna.mol.fingerprint import FingerprintGenerator
     >>> fg = FingerprintGenerator()
 
-    Now, let's read a molecule (glutamine) and set it to the `FingerprintGenerator` object.
+    Now, let's read a molecule (glutamine) and set it to the
+    `FingerprintGenerator` object.
 
     >>> from luna.wrappers.base import MolWrapper
     >>> fg.mol = MolWrapper.from_smiles("N[C@@H](CCC(N)=O)C(O)=O")
 
-    Finally, you can call any available function to generate the desired fingerprint type.
-    In the below example, a count ECFP4 fingerprint of size 1,024 is created.
+    Finally, you can call any available function to generate the desired
+    fingerprint type. In the below example, a count ECFP4 fingerprint of
+    size 1,024 is created.
 
     >>> fp = fg.morgan_fp(radius=2, length=1024, type=2)
     >>> print(fp.GetNonzeroElements())
-    {1: 1, 80: 2, 140: 1, 147: 2, 389: 1, 403: 1, 540: 1, 545: 1, 650: 2, 728: 1, 739: 1, 767: 1, 786: 1, 807: 3, 820: 1, 825: 1, 874: 1, 893: 2, 900: 1}
+    {1: 1, 80: 2, 140: 1, 147: 2, 389: 1, 403: 1, 540: 1, 545: 1, 650: 2,\
+728: 1, 739: 1, 767: 1, 786: 1, 807: 3, 820: 1, 825: 1, 874: 1, 893: 2, 900: 1}
 
-    You can then continue using the `FingerprintGenerator` object to create other fingerprint types.
-    For example, let's create a 2D pharmacophore fingerprint.
+    You can then continue using the `FingerprintGenerator` object to
+    create other fingerprint types. For example, let's create a 2D
+    pharmacophore fingerprint.
 
     >>> fp = fg.pharm2d_fp()
     >>> print(fp.GetNumOnBits())
     90
     """
 
     def __init__(self, mol_obj=None):
         self.mol = mol_obj
 
     @property
     def mol(self):
-        """:class:`~luna.wrappers.base.MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`: The molecule."""
+        """:class:`~luna.wrappers.base.MolWrapper`, \
+                :class:`rdkit.Chem.rdchem.Mol`, or \
+                :class:`openbabel.pybel.Molecule`: The molecule."""
         return self._mol_obj
 
     @mol.setter
     def mol(self, mol_obj):
         self._mol_obj = mol_obj
 
         if mol_obj:
@@ -115,38 +123,49 @@
 
         Raises
         ------
         FingerprintNotCreated
             If the fingerprint could not be created.
         """
         try:
-            return Torsions.GetTopologicalTorsionFingerprintAsIntVect(self._rdmol)
+            func = Torsions.GetTopologicalTorsionFingerprintAsIntVect
+            return func(self._rdmol)
         except Exception as e:
             logger.exception(e)
             raise FingerprintNotCreated("Fingerprint could not be created.")
 
     def morgan_fp(self, radius=2, length=2048, features=False, type=1):
         """Generate a Morgan fingerprint for the molecule ``mol``.
 
         Parameters
         ----------
         radius : int
-            Define the maximum radius of the circular neighborhoods considered for each atom.
-            The default value is 2, which is roughly equivalent to ECFP4 and FCFP4.
+            Define the maximum radius of the circular neighborhoods
+            considered for each atom. The default value is 2, which is
+            roughly equivalent to ECFP4 and FCFP4.
         length : int
             The length of the fingerprint. The default value is 2,048.
         features : bool
-            If True, use pharmacophoric properties (FCFP) instead of atomic invariants (ECFP).
-            The default value is False.
+            If True, use pharmacophoric properties (FCFP) instead of
+            atomic invariants (ECFP). The default value is False.
         type : {1, 2, 3}
-            Define the type of the Morgan fingerprint function to be used, where:
+            Define the type of the Morgan fingerprint function to be
+            used, where:
 
-            * ``1`` means **GetMorganFingerprintAsBitVect()**. It returns an explicit bit vector of size ``length`` (hashed fingerprint), where 0s and 1s represent the presence or absence of a given feature, respectively.
-            * ``2`` means **GetHashedMorganFingerprint()**. It returns a sparse int vector ``length`` elements long (hashed fingerprint) containing the occurrence number of each feature.
-            * ``3`` means **GetMorganFingerprint()**. It returns a sparse int vector 2^32 elements long containing the occurrence number of each feature.
+            * ``1`` means **GetMorganFingerprintAsBitVect()**. \
+                    It returns an explicit bit vector of size ``length`` \
+                    (hashed fingerprint), where 0s and 1s represent the \
+                    presence or absence of a given feature, respectively.
+            * ``2`` means **GetHashedMorganFingerprint()**. \
+                    It returns a sparse int vector ``length`` elements \
+                    long (hashed fingerprint) containing the occurrence \
+                    number of each feature.
+            * ``3`` means **GetMorganFingerprint()**. \
+                    It returns a sparse int vector 2^32 elements long \
+                    containing the occurrence number of each feature.
 
             The default value is ``2``.
 
         Raises
         ------
         FingerprintNotCreated
             If the fingerprint could not be created.
@@ -176,38 +195,44 @@
 
     def pharm2d_fp(self, sig_factory=None):
         """Generate a 2D pharmacophore fingerprint for the molecule ``mol``.
 
         Parameters
         ----------
         sig_factory : RDKit :class:`~rdkit.Chem.Pharm2D.SigFactory`, optional
-            Factory object for producing signatures. The default signature factory is defined as shown below:
+            Factory object for producing signatures. The default signature
+            factory is defined as shown below:
 
-            >>> feat_factory = ChemicalFeatures.BuildFeatureFactory(MIN_FDEF_FILE)
-            >>> sig_factory = SigFactory(feat_factory, minPointCount=2,
-            ...                          maxPointCount=3, trianglePruneBins=False)
+            >>> feat_factory = \
+ChemicalFeatures.BuildFeatureFactory(MIN_FDEF_FILE)
+            >>> sig_factory = SigFactory(feat_factory,
+            ...                          minPointCount=2,
+            ...                          maxPointCount=3,
+            ...                          trianglePruneBins=False)
             >>> sig_factory.SetBins([(0, 2), (2, 5), (5, 8)])
             >>> sig_factory.Init()
 
         Raises
         ------
         FingerprintNotCreated
             If the fingerprint could not be created.
         """
         try:
             if sig_factory is None:
                 sig_factory = _prepare_pharm2d_fp()["sigFactory"]
             return Generate.Gen2DFingerprint(self._rdmol, sig_factory)
         except Exception as e:
             logger.exception(e)
-            raise FingerprintNotCreated("The fingerprint could not be created.")
+            raise FingerprintNotCreated("The fingerprint could not "
+                                        "be created.")
 
 
 def available_fp_functions():
-    """Return a list of all fingerprints available at `FingerprintGenerator`."""
+    """Return a list of all fingerprints available at
+    `FingerprintGenerator`."""
     regex = re.compile(".*([a-zA-Z]+)_fp", flags=0)
     funcs = list(filter(regex.match, dir(FingerprintGenerator)))
     return funcs
 
 
 def _prepare_morgan_fp(fp_opt):
     params = {}
@@ -250,62 +275,73 @@
 
 
 def generate_fp_for_mols(mols, fp_function=None, fp_opt=None, critical=False):
     """Generate molecular fingerprints for a sequence of molecules.
 
     Parameters
     ----------
-    mols : iterable of :class:`~luna.wrappers.base.MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`
+    mols : iterable of :class:`~luna.wrappers.base.MolWrapper`, \
+                :class:`rdkit.Chem.rdchem.Mol`, or \
+                :class:`openbabel.pybel.Molecule`
         A sequence of molecules.
     fp_function : str
         The fingerprint function to use. The default value is 'pharm2d_fp'.
 
-        To check out the list of available functions, call the function :py:meth:`available_fp_functions`.
+        To check out the list of available functions, call the function
+        :py:meth:`available_fp_functions`.
     fp_opt : dict, optional
         A set of parameters to pass to ``fp_function``.
     critical : bool
-        If True, raises any exceptions caught during the generation of fingerprints.
-        Otherwise, ignores all exceptions (the default). The error messages are always printed to the logging output.
+        If True, raises any exceptions caught during the generation of
+        fingerprints.Otherwise, ignores all exceptions (the default).
+        The error messages are always printed to the logging output.
 
     Returns
     -------
      : list of dict
-        A list of dictionaries where each item contains the molecule name and its fingerprint.
+        A list of dictionaries where each item contains the molecule name
+        and its fingerprint.
 
         The dict is defined as follows:
 
             * ``mol`` (str): the molecule name;
-            * ``fp`` (RDKit :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` \
-            or :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`): the fingerprint;
+            * ``fp`` (RDKit \
+:class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` \
+or :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`): the fingerprint;
 
     Raises
     ------
     IllegalArgumentError
-        If ``fp_function`` is not a function available in `FingerprintGenerator`.
+        If ``fp_function`` is not a function available in
+        `FingerprintGenerator`.
 
     Examples
     --------
 
     First, let's define a set of molecules.
 
     >>> from luna.wrappers.base import MolWrapper
     >>> mols = [MolWrapper.from_smiles("N[C@@H](CCC(N)=O)C(O)=O"),
     ...         MolWrapper.from_smiles("C[C@@H](C(=O)O)N"),
     ...         MolWrapper.from_smiles("C1=CC(=CC=C1CC(C(=O)O)N)O")]
 
-    Now, you can generate fingerprints for these molecules using the function :meth:`generate_fp_for_mols`.
-    For example, let's create count ECFP4 fingerprints of size 1,024 for the above molecules.
+    Now, you can generate fingerprints for these molecules using the function
+    :meth:`generate_fp_for_mols`. For example, let's create count ECFP4
+    fingerprints of size 1,024 for the above molecules.
 
     >>> from luna.mol.fingerprint import generate_fp_for_mols
-    >>> fps = generate_fp_for_mols(mols, fp_function="morgan_fp", fp_opt={"length": 1024})
+    >>> fps = generate_fp_for_mols(mols,
+    ...                            fp_function="morgan_fp",
+    ...                            fp_opt={"length": 1024})
 
     Then, you can loop through the results as shown below:
 
     >>> for d in fps:
-    >>>     print(f"{d['mol'].ljust(25)} - {len(d['fp'].GetNonzeroElements())}")
+    >>>     print(f"{d['mol'].ljust(25)} - \
+{len(d['fp'].GetNonzeroElements())}")
     N[C@@H](CCC(N)=O)C(O)=O   - 19
     C[C@@H](C(=O)O)N          - 12
     C1=CC(=CC=C1CC(C(=O)O)N)O - 24
     """
 
     funcs = available_fp_functions()
     if fp_function not in funcs:
@@ -334,10 +370,10 @@
             logger.error("Molecule at position %d failed. Name: %s"
                          % (idx, mol.GetProp("_Name")))
             logger.exception(e)
 
             if critical:
                 raise
 
-    logger.debug("%d molecular sfingerprint(s) created." % len(fp_mols))
+    logger.debug("%d molecular fingerprint(s) created." % len(fp_mols))
 
     return fp_mols
```

### Comparing `luna-0.12.2/luna/mol/groups.py` & `luna-0.13.0/luna/mol/groups.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,31 +7,35 @@
 from networkx.algorithms.shortest_paths.weighted import single_source_dijkstra
 
 from Bio.KDTree import KDTree
 
 from luna.MyBio.selector import Selector, AtomSelector
 from luna.MyBio.util import biopython_entity_to_mol
 from luna.interaction.contact import get_proximal_compounds
+from luna.interaction.contact import get_contacts_with
 from luna.interaction.type import InteractionType
 from luna.mol.atom import ExtendedAtom, AtomData
+from luna.mol.precomp_data import DefaultResidueData
 from luna.mol.charge_model import OpenEyeModel
 from luna.mol.features import ChemicalFeature
 from luna.wrappers.base import MolWrapper
 from luna.util.exceptions import MoleculeSizeError, IllegalArgumentError
-from luna.util.default_values import ACCEPTED_MOL_OBJ_TYPES, COV_SEARCH_RADIUS
+from luna.util.default_values import COV_SEARCH_RADIUS, METAL_COMPLEX_DIST
 from luna.util import math as im
 from luna.util.file import pickle_data, unpickle_data
 from luna.version import __version__
 
 import logging
 logger = logging.getLogger()
 
 
 SS_BOND_FEATURES = ["Atom", "Acceptor", "ChalcogenDonor", "Hydrophobic"]
 
+DEFAULT_RES_DATA = DefaultResidueData()
+
 
 class AtomGroupsManager():
     """Store and manage `AtomGroup` objects.
 
     Parameters
     ----------
     atm_grps : iterable of `AtomGroup`, optional
@@ -60,74 +64,82 @@
 
         self._compounds = set()
 
         self.add_atm_grps(atm_grps)
 
     @property
     def atm_grps(self):
-        """iterable of `AtomGroup`, read-only: The sequence of `AtomGroup` objects.\
-        Additional objects should be added using the method :py:meth:`add_atm_grps`."""
+        """iterable of `AtomGroup`, read-only: The sequence of `AtomGroup`
+        objects. Additional objects should be added using the method
+        :py:meth:`add_atm_grps`."""
         return self._atm_grps
 
     @property
     def compounds(self):
         """set of :class:`~luna.MyBio.PDB.Residue.Residue`, read-only:
         Compounds comprising the ``atm_grps``."""
         return self._compounds
 
     @property
     def child_dict(self):
-        """dict, read-only: Mapping between atoms (`ExtendedAtom`) and atom groups (`AtomGroup`).
+        """dict, read-only: Mapping between atoms (`ExtendedAtom`) and atom
+        groups (`AtomGroup`).
 
-        The mapping is a dict of {tuple of `ExtendedAtom` instances : `AtomGroup`} and is automatically
-        updated when :py:meth:`add_atm_grps` is called."""
+        The mapping is a dict of {tuple of `ExtendedAtom` instances :
+        `AtomGroup`} and is automatically updated when :py:meth:`add_atm_grps`
+        is called."""
         return self._child_dict
 
     @property
     def size(self):
         """int, read-only: The number of atom groups in ``atm_grps``."""
         return len(self._atm_grps)
 
     @property
     def summary(self):
-        """dict, read-only: The number of physicochemical features in ``atm_grps``."""
+        """dict, read-only: The number of physicochemical features in
+        ``atm_grps``."""
         summary = defaultdict(int)
         for grp in self.atm_grps:
             for feature in grp.features:
                 summary[feature] += 1
 
         return summary
 
     def find_atm_grp(self, atoms):
         """ Find the atom group that contains the sequence of atoms ``atoms``.
 
         Returns
         -------
          : `AtomGroup` or None
-            An atom group object or None if ``atoms`` is not in the ``child_dict`` mapping.
+            An atom group object or None if ``atoms`` is not in the
+            ``child_dict`` mapping.
         """
         return self.child_dict.get(tuple(sorted(atoms)), None)
 
     def get_all_interactions(self):
-        """Return all interactions established by the atom groups in ``atm_grps``.
+        """Return all interactions established by the atom groups in
+        ``atm_grps``.
 
         Returns
         -------
          : set of :class:`~luna.interactions.type.InteractionType`
             All interactions.
         """
-        return set(chain.from_iterable([atm_grp.interactions for atm_grp in self.atm_grps]))
+        return set(chain.from_iterable([atm_grp.interactions
+                                        for atm_grp in self.atm_grps]))
 
     def apply_filter(self, func):
         """Apply a filtering function over the atom groups in ``atm_grps`.
 
         Parameters
         ----------
         func : callable
-            A filtering function that returns True case an `AtomGroup` object is valid and False otherwise.
+            A filtering function that returns True case an `AtomGroup`
+            object is valid and False otherwise.
 
         Yields
         ------
         `AtomGroup`
             A valid `AtomGroup` object.
         """
         for atm_grp in self.atm_grps:
@@ -138,16 +150,17 @@
         """Filter `AtomGroup` objects by their physicochemical features.
 
         Parameters
         ----------
         types : iterable of str
             A sequence of physicochemical features.
         must_contain_all : bool
-            If True, an `AtomGroup` object should contain all physicochemical features in ``types`` to be accepted.
-            Otherwise, it will be filtered out.
+            If True, an `AtomGroup` object should contain all physicochemical
+            features in ``types`` to be accepted. Otherwise, it will be
+            filtered out.
 
         Yields
         ------
         `AtomGroup`
             A valid `AtomGroup` object.
         """
         for atm_grp in self.atm_grps:
@@ -155,55 +168,64 @@
                 if set(types).issubset(set(atm_grp.feature_names)):
                     yield atm_grp
             else:
                 if len(set(types) & set(atm_grp.feature_names)) > 0:
                     yield atm_grp
 
     def add_atm_grps(self, atm_grps):
-        """Add one or more `AtomGroup` objects to ``atm_grps`` and automatically update ``child_dict``."""
+        """Add one or more `AtomGroup` objects to ``atm_grps`` and
+        automatically update ``child_dict``."""
 
         atm_grps = atm_grps or []
 
         self._atm_grps = list(set(self._atm_grps + list(atm_grps)))
 
         for atm_grp in atm_grps:
             self.child_dict[tuple(sorted(atm_grp.atoms))] = atm_grp
             self._compounds.update(atm_grp.compounds)
             atm_grp.manager = self
 
     def remove_atm_grps(self, atm_grps):
-        """Remove one or more `AtomGroup` objects from ``atm_grps`` and automatically update ``child_dict``.
+        """Remove one or more `AtomGroup` objects from ``atm_grps`` and
+        automatically update ``child_dict``.
 
         Any recursive references to the removed objects will also be cleared.
         """
         self._atm_grps = list(set(self._atm_grps) - set(atm_grps))
 
         for atm_grp in atm_grps:
-            # ExtendedAtom objects keep a list of all AtomGroup objects to which they belong to. So, if we don't clear the references
-            # directly, the AtomGroup objects will still exist in the ExtendedAtom list even when they were already removed from an
+            # ExtendedAtom objects keep a list of all AtomGroup objects to
+            # which they belong to. So, if we don't clear the references
+            # directly, the AtomGroup objects will still exist in the
+            # ExtendedAtom list even when they were already removed from an
             # instance of AtomGroupsManager().
             atm_grp.clear_refs()
 
             # Remove the atom group from the dict.
             key = tuple(sorted(atm_grp.atoms))
             if key in self.child_dict:
                 del self.child_dict[key]
 
     def new_atm_grp(self, atoms, features=None, interactions=None):
-        """Create a new `AtomGroup` object for ``atoms`` if one does not exist yet.
-        Otherwise, return the existing `AtomGroup` object.
+        """Create a new `AtomGroup` object for ``atoms`` if one does not exist
+        yet. Otherwise, return the existing `AtomGroup` object, and add
+        any new features and interactions to it if provided.
 
         Parameters
         ----------
         atoms : iterable of :class:`~luna.mol.atom.ExtendedAtom`
             A sequence of atoms.
-        features : iterable of :class:`~luna.mol.features.ChemicalFeature`, optional
-            If provided, add ``features`` to a new or an already existing `AtomGroup` object.
-        interactions : iterable of :class:`~luna.interaction.type.InteractionType`, optional
-            If provided, add ``interactions`` to a new or an already existing `AtomGroup` object.
+        features : iterable of :class:`~luna.mol.features.ChemicalFeature`, \
+                        optional
+            If provided, add ``features`` to a new or an already existing
+            `AtomGroup` object.
+        interactions : iterable of \
+                :class:`~luna.interaction.type.InteractionType`, optional
+            If provided, add ``interactions`` to a new or an already existing
+            `AtomGroup` object.
 
         Returns
         -------
          : AtomGroup
             A new or an already existing `AtomGroup` object.
         """
         key = tuple(sorted(atoms))
@@ -221,48 +243,58 @@
 
         if interactions:
             atm_grp.add_interactions(interactions)
 
         return atm_grp
 
     def merge_hydrophobic_atoms(self, interactions_mngr):
-        """Create hydrophobic islands by merging covalently bonded hydrophobic atoms in ``atm_grps``.
-        Hydrophobic islands are atom groups having the feature `Hydrophobe`.
+        """Create hydrophobic islands by merging covalently bonded hydrophobic
+        atoms in ``atm_grps``. Hydrophobic islands are atom groups having the
+        feature `Hydrophobe`.
 
-        Atom-atom hydrophobic interactions in ``interactions_mngr`` are also converted to
-        island-island interactions.
+        Atom-atom hydrophobic interactions in ``interactions_mngr`` are also
+        converted to island-island interactions.
 
         Parameters
         ----------
         interactions_mngr : :class:`~luna.interaction.calc.InteractionsManager`
-            An :class:`~luna.interaction.calc.InteractionsManager` object from where
-            hydrophobic interactions are selected and convert from atom-atom to island-island interactions.
+            An :class:`~luna.interaction.calc.InteractionsManager` object from
+            where hydrophobic interactions are selected and convert from
+            atom-atom to island-island interactions.
         """
 
         # Only hydrophobic atom groups.
         hydrop_atm_grps = list(self.filter_by_types(["Hydrophobic"]))
 
-        # Hydrophobic islands dictionary. Keys are integer values and items are defined by a set of atom groups.
+        # Hydrophobic islands dictionary. Keys are integer values and items are
+        # defined by a set of atom groups.
         hydrop_islands = defaultdict(set)
 
-        # It stores a mapping of an atom (represented by its full id) and a hydrophobic island (defined by its keys).
+        # It stores a mapping of an atom (represented by its full id) and a
+        # hydrophobic island (defined by its keys).
         atm_mapping = {}
 
         island_id = 0
         for atm_grp in hydrop_atm_grps:
             # Hydrophobic atoms are defined always as only one atom.
             atm = atm_grp.atoms[0]
 
-            # Recover the groups of all neighbors of this atom (it will merge all existing islands).
-            nb_grps = set([atm_mapping[nbi.full_id] for nbi in atm.neighbors_info if nbi.full_id in atm_mapping])
+            # Recover the groups of all neighbors of this atom (it will merge
+            # all existing islands).
+            nb_grps = set([atm_mapping[nbi.full_id]
+                           for nbi in atm.neighbors_info
+                           if nbi.full_id in atm_mapping])
 
-            # Already there are hydrophobic islands formed by the neighbors of this atom.
+            # Already there are hydrophobic islands formed by the neighbors of
+            # this atom.
             if nb_grps:
                 # Merge all groups of the neighbors of this atom.
-                new_island = set(chain.from_iterable([hydrop_islands.pop(nb_grp_id) for nb_grp_id in nb_grps]))
+                new_island = \
+                    set(chain.from_iterable([hydrop_islands.pop(nb_grp_id)
+                                             for nb_grp_id in nb_grps]))
                 # Include this atom to the merged group.
                 new_island.add(atm)
 
                 for k in atm_mapping:
                     if atm_mapping[k] in nb_grps:
                         atm_mapping[k] = island_id
 
@@ -272,27 +304,31 @@
                 atm_mapping[atm.get_full_id()] = island_id
                 hydrop_islands[island_id].add(atm)
 
             island_id += 1
 
         # Create AtomGroup objects for the hydrophobic islands
         for island_id in hydrop_islands:
-            # It will update an existing atom group or create a new one with the informed parameters.
-            hydrophobe = self.new_atm_grp(hydrop_islands[island_id], [ChemicalFeature("Hydrophobe")])
+            # It will update an existing atom group or create a new one
+            # with the informed parameters.
+            hydrophobe = self.new_atm_grp(hydrop_islands[island_id],
+                                          [ChemicalFeature("Hydrophobe")])
             # Update the island information
             hydrop_islands[island_id] = hydrophobe
 
-        hydrop_interactions = list(interactions_mngr.filter_by_types(["Hydrophobic"]))
+        hydrop_interactions = \
+            list(interactions_mngr.filter_by_types(["Hydrophobic"]))
         island_island_inter = defaultdict(set)
         for inter in hydrop_interactions:
             src_atm = inter.src_grp.atoms[0]
             trgt_atm = inter.trgt_grp.atoms[0]
 
             # The two island ids are used as key.
-            key = tuple(sorted([atm_mapping[src_atm.get_full_id()], atm_mapping[trgt_atm.get_full_id()]]))
+            key = tuple(sorted([atm_mapping[src_atm.get_full_id()],
+                                atm_mapping[trgt_atm.get_full_id()]]))
 
             island_island_inter[key].add(inter)
 
         interactions = set()
         for k in island_island_inter:
             island_atms = defaultdict(set)
             for inter in island_island_inter[k]:
@@ -304,87 +340,105 @@
 
             centroid1 = im.centroid(im.atom_coordinates(island_atms[k[0]]))
             centroid2 = im.centroid(im.atom_coordinates(island_atms[k[1]]))
             cc_dist = im.euclidean_distance(centroid1, centroid2)
 
             params = {"dist_hydrop_inter": cc_dist}
 
-            inter = InteractionType(hydrop_islands[k[0]], hydrop_islands[k[1]], "Hydrophobic",
-                                    src_interacting_atms=island_atms[k[0]], trgt_interacting_atms=island_atms[k[1]], params=params)
+            inter = InteractionType(hydrop_islands[k[0]],
+                                    hydrop_islands[k[1]],
+                                    "Hydrophobic",
+                                    src_interacting_atms=island_atms[k[0]],
+                                    trgt_interacting_atms=island_atms[k[1]],
+                                    params=params)
             interactions.add(inter)
 
-        # Update the list of interactions with the new island-island interactions.
+        # Update the list of interactions with the new island-island
+        # interactions.
         interactions_mngr.add_interactions(interactions)
         # Remove atom-atom hydrophobic interactions.
         interactions_mngr.remove_interactions(hydrop_interactions)
 
         for atm_grp in hydrop_atm_grps:
             features = [f for f in atm_grp.features if f.name != "Hydrophobic"]
 
-            # It may happen that a atom group ends up having no feature after the remotion of the feature "Hydrophobic".
-            # This is unlikely to occur as all atoms (by default) will have at least the feature 'Atom'. But, depending one the
-            # pharmacophore rules definition, it can occur.
+            # It may happen that a atom group ends up having no feature after
+            # the remotion of the feature "Hydrophobic". This is unlikely to
+            # occur as all atoms (by default) will have at least the feature
+            # 'Atom'. But, depending one the pharmacophore rules definition,
+            # it can occur.
             atm_grp.features = features
 
     def get_shortest_path_length(self, src_grp, trgt_grp, cutoff=None):
-        """Compute the shortest path length between two atom groups ``src_grp`` and ``trgt_grp``.
+        """Compute the shortest path length between two atom groups ``src_grp``
+        and ``trgt_grp``.
 
-        The shortest path between two atom groups is defined as the shortest path between any of their atoms,
-        which are calculated using Dijkstra’s algorithm and the graph ``graph``.
+        The shortest path between two atom groups is defined as the shortest
+        path between any of their atoms, which are calculated using Dijkstra’s
+        algorithm and the graph ``graph``.
 
-        If there is not any path between ``src_grp`` and ``trgt_grp``, infinite is returned.
+        If there is not any path between ``src_grp`` and ``trgt_grp``,
+        infinite is returned.
 
         Parameters
         ----------
         src_grp, trgt_grp : `AtomGroup`
             Two atom groups to calculate the shortest path.
         cutoff : int
-            Only paths of length <= ``cutoff`` are returned. If None, all path lengths are considered.
+            Only paths of length <= ``cutoff`` are returned.
+            If None, all path lengths are considered.
 
         Returns
         -------
          : int or float('inf'):
             The shortest path.
         """
         shortest_path_size = float('inf')
         for src_atm in src_grp.atoms:
             for trgt_atm in trgt_grp.atoms:
                 try:
-                    dist, path = single_source_dijkstra(self.graph, src_atm, trgt_atm, cutoff=cutoff)
+                    dist, path = single_source_dijkstra(self.graph,
+                                                        src_atm,
+                                                        trgt_atm,
+                                                        cutoff=cutoff)
                     if dist < shortest_path_size:
                         shortest_path_size = dist
                 except Exception:
                     pass
         return shortest_path_size
 
     def save(self, output_file, compressed=True):
-        """Write the pickled representation of the `AtomGroupsManager` object to the file ``output_file``.
+        """Write the pickled representation of the `AtomGroupsManager` object
+        to the file ``output_file``.
 
         Parameters
         ----------
         output_file : str
             The output file.
         compressed : bool, optional
-            If True (the default), compress the pickled representation as a gzip file (.gz).
+            If True (the default), compress the pickled representation as a
+            gzip file (.gz).
 
         Raises
         -------
         FileNotCreated
             If the file could not be created.
         """
         pickle_data(self, output_file, compressed)
 
     @staticmethod
     def load(input_file):
-        """Load the pickled representation of an `AtomGroupsManager` object saved at the file ``input_file``.
+        """Load the pickled representation of an `AtomGroupsManager` object
+        saved at the file ``input_file``.
 
         Returns
         ----------
          : `AtomGroupsManager`
-            The reconstituted `AtomGroupsManager` object, including its set of atom groups and interactions.
+            The reconstituted `AtomGroupsManager` object, including its set of
+            atom groups and interactions.
 
         Raises
         -------
         PKLNotReadError
             If the file could not be loaded.
         """
         return unpickle_data(input_file)
@@ -396,31 +450,40 @@
     def __iter__(self):
         """Iterate over children."""
         for atm_grp in self.atm_grps:
             yield atm_grp
 
 
 class AtomGroup():
-    """ Represent single atoms, chemical functional groups, or simply an arrangement of atoms as in hydrophobes.
+    """ Represent single atoms, chemical functional groups, or simply an
+    arrangement of atoms as in hydrophobes.
 
     Parameters
     ----------
     atoms : iterable of :class:`~luna.mol.atom.ExtendedAtom`
         A sequence of atoms.
-    features : iterable of :class:`~luna.mol.features.ChemicalFeature`, optional
+    features : iterable of :class:`~luna.mol.features.ChemicalFeature`, \
+                    optional
         A sequence of chemical features.
-    interactions : iterable of :class:`~luna.interaction.type.InteractionType`, optional
+    interactions : iterable of \
+                    :class:`~luna.interaction.type.InteractionType`, optional
         A sequence of interactions established by an atom group.
     recursive : bool
-        If True, add the new atom group to the list of atom groups of each atom in ``atoms``.
+        If True, add the new atom group to the list of atom groups of each atom
+        in ``atoms``.
     manager : `AtomGroupsManager`, optional
         The `AtomGroupsManager` object that contains this `AtomGroup` object.
     """
 
-    def __init__(self, atoms, features=None, interactions=None, recursive=True, manager=None):
+    def __init__(self,
+                 atoms,
+                 features=None,
+                 interactions=None,
+                 recursive=True,
+                 manager=None):
         self._atoms = sorted(atoms)
 
         # Atom properties
         self._coords = im.atom_coordinates(atoms)
         self._centroid = im.centroid(self.coords)
         self._normal = None
 
@@ -436,89 +499,100 @@
 
         if recursive:
             for atm in self.atoms:
                 atm.add_atm_grps([self])
 
     @property
     def atoms(self):
-        """iterable of :class:`~luna.mol.atom.ExtendedAtom`, read-only: The sequence of atoms that belong to an atom group."""
+        """iterable of :class:`~luna.mol.atom.ExtendedAtom`, read-only: \
+            The sequence of atoms that belong to an atom group."""
         return self._atoms
 
     @property
     def compounds(self):
-        """set of :class:`~luna.MyBio.PDB.Residue.Residue`, read-only: The set of unique compounds that contain the atoms in ``atoms``.
+        """set of :class:`~luna.MyBio.PDB.Residue.Residue`, read-only: \
+            The set of unique compounds that contain the atoms in ``atoms``.
 
-        As an atom group can be formed by the union of two or more compounds (e.g., amide of peptide bonds), it may return
-        more than one compound.
+        As an atom group can be formed by the union of two or more compounds
+        (e.g., amide of peptide bonds), it may return more than one compound.
         """
         return set([a.parent for a in self._atoms])
 
     @property
     def coords(self):
-        """ array-like of floats : Atomic coordinates (x, y, z) of each atom in ``atoms``."""
+        """ array-like of floats : Atomic coordinates (x, y, z) of each \
+        atom in ``atoms``."""
         return self._coords
 
     @property
     def centroid(self):
-        """ array-like of floats, read-only: The centroid (x, y, z) of the atom group.
+        """ array-like of floats, read-only: The centroid (x, y, z) of the \
+        atom group.
 
-        If ``atoms`` contains only one atom, then ``centroid`` returns the same as ``coords``.
+        If ``atoms`` contains only one atom, then ``centroid`` returns the same
+        as ``coords``.
         """
         return self._centroid
 
     @property
     def normal(self):
-        """array-like of floats, read-only: The normal vector (x, y, z) of the points given by ``coords``."""
+        """array-like of floats, read-only: The normal vector (x, y, z) of \
+        the points given by ``coords``."""
         if self._normal is None:
             self._normal = im.calc_normal(self.coords)
         return self._normal
 
     @property
     def features(self):
-        """iterable of :class:`~luna.mol.features.ChemicalFeature`: A sequence of chemical features.
+        """iterable of :class:`~luna.mol.features.ChemicalFeature`: \
+                A sequence of chemical features.
 
         To add or remove a feature use :py:meth:`add_features`
         or :py:meth:`remove_features`, respectively."""
         return self._features
 
     @features.setter
     def features(self, features):
         self._features = sorted(features)
         # Reset hash.
         self._hash_cache = None
 
     @property
     def feature_names(self):
-        """iterable of str: The name of each chemical feature in ``features``."""
+        """iterable of str: The name of each chemical feature in \
+        ``features``."""
         return [f.name for f in self.features]
 
     @property
     def interactions(self):
-        """iterable of :class:`~luna.interaction.type.InteractionType`: The sequence of interactions
-        established by an atom group.
+        """iterable of :class:`~luna.interaction.type.InteractionType`: \
+            The sequence of interactions established by an atom group.
 
         To add or remove an interaction use :py:meth:`add_interactions`
         or :py:meth:`remove_interactions`, respectively."""
         return self._interactions
 
     @interactions.setter
     def interactions(self, interactions):
         self._interactions = interactions
 
     @property
     def manager(self):
-        """`AtomGroupsManager`: The `AtomGroupsManager` object that contains an `AtomGroup` object."""
+        """`AtomGroupsManager`: The `AtomGroupsManager` object that contains \
+        an `AtomGroup` object."""
         return self._manager
 
     @manager.setter
     def manager(self, manager):
         if isinstance(manager, AtomGroupsManager):
             self._manager = manager
         else:
-            raise IllegalArgumentError("The informed atom group manager must be an instance of '%s'." % AtomGroupsManager)
+            raise IllegalArgumentError("The informed atom group manager must "
+                                       "be an instance of '%s'."
+                                       % AtomGroupsManager)
 
     @property
     def size(self):
         """int: The number of atoms comprising an atom group."""
         return len(self.atoms)
 
     def has_atom(self, atom):
@@ -535,18 +609,19 @@
         """
         return atom in self.atoms
 
     def contain_group(self, atm_grp):
         """Check if the atom group ``atm_grp`` is a subset of this atom group.
 
         For example, consider the benzene molecule.
-        Its aromatic ring itself forms an `AtomGroup` object composed of all of its six atoms.
-        Consider now any subset of carbons in the benzene molecule.
-        This subset forms an `AtomGroup` object that is part of the group formed by the aromatic ring.
-        Therefore, in this example, :meth:`contain_group` will return True because the aromatic ring
+        Its aromatic ring itself forms an `AtomGroup` object composed of all of
+        its six atoms. Consider now any subset of carbons in the benzene
+        molecule. This subset forms an `AtomGroup` object that is part of the
+        group formed by the aromatic ring. Therefore, in this example,
+        :meth:`contain_group` will return True because the aromatic ring
         contains the subset of hydrophobic atoms.
 
         Parameters
         ----------
         atm_grp : :class:`~luna.mol.groups.AtomGroup`
 
         Returns
@@ -561,154 +636,189 @@
         return [a.get_serial_number() for a in self.atoms]
 
     def get_chains(self):
         """Get all unique chains in an atom group."""
         return sorted(set([a.get_parent_by_level("C").id for a in self.atoms]))
 
     def get_interactions_with(self, atm_grp):
-        """Get all interactions that an atom group establishes with another atom group ``atm_grp``.
+        """Get all interactions that an atom group establishes with another
+        atom group ``atm_grp``.
 
         Returns
         -------
          : iterable of :class:`~luna.interactions.type.InteractionType`
            All interactions established with the atom group ``atm_grp``.
         """
         target_interactions = []
 
         for inter in self.interactions:
             if inter.src_grp == atm_grp or inter.trgt_grp == atm_grp:
                 target_interactions.append(inter)
         return target_interactions
 
     def get_shortest_path_length(self, trgt_grp, cutoff=None):
-        """Compute the shortest path length between this atom group to another atom group ``trgt_grp``.
+        """Compute the shortest path length between this atom group to another
+        atom group ``trgt_grp``.
 
-        The shortest path between two atom groups is defined as the shortest path between any of their atoms,
-        which are calculated using Dijkstra’s algorithm.
+        The shortest path between two atom groups is defined as the shortest
+        path between any of their atoms, which are calculated using
+        Dijkstra’s algorithm.
 
         If ``manager`` is not provided, None is returned.
 
-        If there is not any path between ``src_grp`` and ``trgt_grp``, infinite is returned.
+        If there is not any path between ``src_grp`` and ``trgt_grp``,
+        infinite is returned.
 
         Parameters
         ----------
         trgt_grp : `AtomGroup`
             The target atom group to calculate the shortest path.
         cutoff : int, optional
-            Only paths of length <= ``cutoff`` are returned. If None, all path lengths are considered.
+            Only paths of length <= ``cutoff`` are returned.
+            If None, all path lengths are considered.
 
         Returns
         -------
          : int, float('inf'), or None:
             The shortest path.
         """
         if self.manager is not None:
-            return self.manager.get_shortest_path_length(self, trgt_grp, cutoff)
+            return self.manager.get_shortest_path_length(self,
+                                                         trgt_grp,
+                                                         cutoff)
         return None
 
     def add_features(self, features):
-        """ Add :class:`~luna.mol.features.ChemicalFeature` objects to ``features``."""
+        """ Add :class:`~luna.mol.features.ChemicalFeature` objects
+        to ``features``."""
         self._features = sorted(set(self.features + list(features)))
         # Reset hash.
         self._hash_cache = None
 
     def remove_features(self, features):
-        """ Remove :class:`~luna.mol.features.ChemicalFeature` objects from ``features``."""
+        """ Remove :class:`~luna.mol.features.ChemicalFeature` objects
+        from ``features``."""
         self._features = sorted(set(self.features) - set(features))
         # Reset hash.
         self._hash_cache = None
 
     def add_interactions(self, interactions):
-        """ Add :class:`~luna.interaction.type.InteractionType` objects to ``interactions``."""
+        """ Add :class:`~luna.interaction.type.InteractionType` objects
+        to ``interactions``."""
         self._interactions = list(set(self.interactions + list(interactions)))
 
     def remove_interactions(self, interactions):
-        """ Remove :class:`~luna.interaction.type.InteractionType` objects from ``interactions``."""
+        """ Remove :class:`~luna.interaction.type.InteractionType` objects
+        from ``interactions``."""
         self._interactions = list(set(self.interactions) - set(interactions))
 
     def is_water(self):
-        """Return True if all atoms in the atom group belong to water molecules."""
+        """Return True if all atoms in the atom group belong to water
+        molecules."""
         return all([a.parent.is_water() for a in self.atoms])
 
     def is_hetatm(self):
-        """Return True if all atoms in the atom group belong to hetero group, i.e., non-standard residues of proteins,
-        DNAs, or RNAs, as well as atoms in other kinds of groups, such as carbohydrates,
-        substrates, ligands, solvent, and metal ions.
+        """Return True if all atoms in the atom group belong to hetero group,
+        i.e., non-standard residues of proteins, DNAs, or RNAs, as well as
+        atoms in other kinds of groups, such as carbohydrates, substrates,
+        ligands, solvent, and metal ions.
 
         Hetero groups are designated by the flag HETATM in the PDB format."""
         return all([a.parent.is_hetatm() for a in self.atoms])
 
+    def is_metal(self):
+        """Return True if all atoms in the atom group are metal ions."""
+        return all([a.parent.is_metal() for a in self.atoms])
+
     def is_residue(self):
-        """Return True if all atoms in the atom group belong to standard residues of proteins."""
+        """Return True if all atoms in the atom group belong to standard
+        residues of proteins."""
         return all([a.parent.is_residue() for a in self.atoms])
 
     def is_nucleotide(self):
         """Return True if all atoms in the atom group belong to nucleotides."""
         return all([a.parent.is_nucleotide() for a in self.atoms])
 
     def is_mixed(self):
-        """Return True if the atoms in the atom group belong to different compound classes
-        (water, hetero group, residue, or nucleotide)."""
+        """Return True if the atoms in the atom group belong to different
+        compound classes (water, hetero group, residue, or nucleotide)."""
         return len(set([a.parent.get_class() for a in self.atoms])) > 1
 
     def has_water(self):
-        """Return True if at least one atom in the atom group belongs to a water molecule."""
+        """Return True if at least one atom in the atom group belongs to a
+        water molecule."""
         return any([a.parent.is_water() for a in self.atoms])
 
     def has_hetatm(self):
-        """Return True if at least one atom in the atom group belongs to a hetero group, i.e., non-standard residues of proteins,
-        DNAs, or RNAs, as well as atoms in other kinds of groups, such as carbohydrates,
+        """Return True if at least one atom in the atom group belongs to a
+        hetero group, i.e., non-standard residues of proteins, DNAs, or RNAs,
+        as well as atoms in other kinds of groups, such as carbohydrates,
         substrates, ligands, solvent, and metal ions."""
         return any([a.parent.is_hetatm() for a in self.atoms])
 
+    def has_metal(self):
+        """Return True if at least one atom in the atom group is a metal."""
+        return any([a.parent.is_metal() for a in self.atoms])
+
     def has_residue(self):
-        """Return True if at least one atom in the atom group belongs to a standard residue of proteins."""
+        """Return True if at least one atom in the atom group belongs to a
+        standard residue of proteins."""
         return any([a.parent.is_residue() for a in self.atoms])
 
     def has_nucleotide(self):
-        """Return True if at least one atom in the atom group belongs to a nucleotide."""
+        """Return True if at least one atom in the atom group belongs to a
+        nucleotide."""
         return any([a.parent.is_nucleotide() for a in self.atoms])
 
     def has_target(self):
-        """Return True if at least one compound is the target of LUNA's analysis"""
+        """Return True if at least one compound is the target of LUNA's
+        analysis"""
         return any([a.parent.is_target() for a in self.atoms])
 
     def as_json(self):
         """Represent the atom group as a dict containing the atoms, compounds,
-        features, and compound classes (water, hetero group, residue, or nucleotide).
+        features, and compound classes (water, hetero group, residue,
+        or nucleotide).
 
         The dict is defined as follows:
 
-            * ``atoms`` (iterable of :class:`~luna.mol.atom.ExtendedAtom`): the list of atoms comprising the atom group;
-            * ``compounds`` (iterable of :class:`~luna.MyBio.PDB.Residue.Residue`): the list of unique compounds that contain the atoms;
+            * ``atoms`` (iterable of :class:`~luna.mol.atom.ExtendedAtom`): \
+                    the list of atoms comprising the atom group;
+            * ``compounds`` (iterable of \
+                    :class:`~luna.MyBio.PDB.Residue.Residue`): the list of \
+                    unique compounds that contain the atoms;
             * ``classes`` (iterable of str): the list of compound classes;
-            * ``features`` (iterable of :class:`~luna.mol.features.ChemicalFeature`): the atom group's list of chemical features.
+            * ``features`` (iterable of \
+                    :class:`~luna.mol.features.ChemicalFeature`): the atom \
+                    group's list of chemical features.
         """
         grp_obj = {}
         grp_obj["atoms"] = [atm.as_json() for atm in self.atoms]
         grp_obj["compounds"] = [comp.as_json() for comp in self.compounds]
-        grp_obj["features"] = [feat.name for feat in self.features if feat.name != "Atom"]
+        grp_obj["features"] = [feat.name for feat in self.features
+                               if feat.name != "Atom"]
         grp_obj["classes"] = [comps.get_class() for comps in self.compounds]
 
         return grp_obj
 
     def clear_refs(self):
-        """References to this `AtomGroup` instance will be removed from the list of atom groups of
-        each atom in ``atoms``."""
+        """References to this `AtomGroup` instance will be removed from the
+        list of atom groups of each atom in ``atoms``."""
         if self._recursive:
             for atm in self.atoms:
                 atm.remove_atm_grps([self])
 
     def __repr__(self):
         return '<AtomGroup: [%s]>' % ', '.join([str(x) for x in self.atoms])
 
     def __eq__(self, other):
         """Overrides the default implementation"""
         if type(self) == type(other):
-            return self.atoms == other.atoms and self.features == other.features
+            return (self.atoms == other.atoms
+                    and self.features == other.features)
         return False
 
     def __ne__(self, other):
         """Overrides the default implementation"""
         return not self.__eq__(other)
 
     def __lt__(self, other):
@@ -719,46 +829,52 @@
     def __len__(self):
         # Number of atoms.
         return self.size
 
     def __hash__(self):
         """Overrides the default implementation"""
         if self._hash_cache is None:
-            # Transform atoms and features list into an imutable data structure.
-            # The lists are sorted in order to avoid dependence on appending order.
+            # Transform atoms and features list into an imutable data
+            # structure. The lists are sorted in order to avoid
+            # dependence on appending order.
             atoms_tuple = tuple(self.atoms)
             feat_tuple = tuple(self.features)
             self._hash_cache = hash((atoms_tuple, feat_tuple, self.__class__))
         return self._hash_cache
 
 
 class PseudoAtomGroup(AtomGroup):
-    """Represent only the atoms from an `AtomGroup` object that are involved in an interaction.
+    """Represent only the atoms from an `AtomGroup` object that are involved
+    in an interaction.
 
-    Currently, this class is only used during the generation of LUNA's fingerprints.
+    Currently, this class is only used during the generation of LUNA's
+    fingerprints.
 
     Parameters
     ----------
     parent_grp : `AtomGroup`
         The atom group that contains the subset of atoms ``atoms``.
     atoms : iterable of :class:`~luna.mol.atom.ExtendedAtom`
         A sequence of atoms.
-    features : iterable of :class:`~luna.mol.features.ChemicalFeature`, optional
+    features : iterable of :class:`~luna.mol.features.ChemicalFeature`, \
+                optional
         A sequence of chemical features.
-    interactions : iterable of :class:`~luna.interaction.type.InteractionType`, optional
+    interactions : iterable of \
+                :class:`~luna.interaction.type.InteractionType`, optional
         A sequence of interactions established by an atom group.
     """
 
     def __init__(self, parent_grp, atoms, features=None, interactions=None):
         self.parent_grp = parent_grp
 
         super().__init__(atoms, features, interactions, recursive=False)
 
     def __repr__(self):
-        return '<PseudoAtomGroup: [%s]>' % ', '.join([str(x) for x in self.atoms])
+        return ('<PseudoAtomGroup: [%s]>'
+                % ', '.join([str(x) for x in self.atoms]))
 
 
 class AtomGroupPerceiver():
 
     """Perceive and create atom groups for molecules.
 
     Parameters
@@ -766,71 +882,61 @@
     feature_extractor : :class:`~luna.mol.features.FeatureExtractor`
         Perceive pharmacophoric properties from molecules.
     add_h : bool
         If True, add hydrogen to the molecules.
     ph : float, optional
         If not None, add hydrogens appropriate for pH ``ph``.
     amend_mol : bool
-        If True, apply validation and standardization of molecules read from a PDB file.
+        If True, apply validation and standardization of molecules read
+        from a PDB file.
     charge_model : class:`~luna.mol.charge_model.ChargeModel`
-        A charge model object. By default, the implementation of OpenEye charge model is used.
-    mol_obj_type : {"rdkit", "openbabel"}
-        If "rdkit", parse the converted molecule with RDKit and return an instance of :class:`rdkit.Chem.rdchem.Mol`.
-        If "openbabel", parse the converted molecule with Open Babel and return an instance of
-        :class:`openbabel.pybel.Molecule`.
+        A charge model object. By default, the implementation of OpenEye
+        charge model is used.
     expand_selection : bool
-        If True (the default), perceive features for a given molecule considering all nearby molecules.
-        The goal is to identify any covalently bonded molecules that may alter the
-        pharmacophoric properties or chemical functional groups.
+        If True (the default), perceive features for a given molecule
+        considering all nearby molecules. The goal is to identify any
+        covalently bonded molecules that may alter the pharmacophoric
+        properties or chemical functional groups.
 
         For instance, consider an amide of a peptide bond.
-        If ``expand_selection`` is False, the residues forming the peptide bond will be analyzed separately,
-        which will make the oxygen and the nitrogen of the amide to be perceived as carbonyl oxygen
-        and amine, respectively.
-        On the other hand, if ``expand_selection`` is True, the covalent bond between the residues will be
-        identified and the amide will be correctly perceived.
+        If ``expand_selection`` is False, the residues forming the peptide
+        bond will be analyzed separately, which will make the oxygen and the
+        nitrogen of the amide to be perceived as carbonyl oxygen and amine,
+        respectively. On the other hand, if ``expand_selection`` is True, the
+        covalent bond between the residues will be identified and the amide
+        will be correctly perceived.
     radius : float
-        If ``expand_selection`` is True, select all molecules up to a maximum of ``radius`` away (measured in Å).
-        The default value is 2.2, which comprises covalent bond distances.
+        If ``expand_selection`` is True, select all molecules up to a maximum
+        of ``radius`` away (measured in Å). The default value is 2.2, which
+        comprises covalent bond distances.
     tmp_path : str, optional
         A temporary directory to where temporary files will be saved.
-        If not provided, the system's default temporary directory will be used instead.
+        If not provided, the system's default temporary directory will be used
+        instead.
     critical : bool
-        If False, ignore any errors during the processing a molecule and continue to the next one.
-        The default value is True, which implies that any errors will raise an exception.
-
-    Raises
-    ------
-    IllegalArgumentError
-        If ``mol_obj_type`` is not either 'rdkit' nor 'openbabel'.
+        If False, ignore any errors during the processing a molecule and
+        continue to the next one. The default value is True, which implies
+        that any errors will raise an exception.
     """
 
     def __init__(self, feature_extractor, add_h=False, ph=None, amend_mol=True,
-                 charge_model=OpenEyeModel(), mol_obj_type="rdkit",
-                 expand_selection=True, radius=COV_SEARCH_RADIUS,
-                 cache=None, tmp_path=None, critical=True):
-
-        if mol_obj_type not in ACCEPTED_MOL_OBJ_TYPES:
-            acc_mol_obj_types = ", ".join(ACCEPTED_MOL_OBJ_TYPES)
-            raise IllegalArgumentError("Objects of type '%s' are not currently"
-                                       "accepted. The available options are: "
-                                       "%s." % (mol_obj_type,
-                                                acc_mol_obj_types))
+                 charge_model=OpenEyeModel(), expand_selection=True,
+                 radius=COV_SEARCH_RADIUS, cache=None, tmp_path=None,
+                 critical=True):
 
         self.feature_extractor = feature_extractor
 
         self.add_h = add_h
         self.ph = ph
         # If the user decided not to add hydrogens,
         # it will try to use the existing ones.
         self.keep_hydrog = not self.add_h
 
         self.amend_mol = amend_mol
         self.charge_model = charge_model
-        self.mol_obj_type = mol_obj_type
         self.expand_selection = expand_selection
         self.radius = radius
 
         self.cache = cache
         self.tmp_path = tmp_path
 
         # If the pharmacophoric perception is critical, any exception during
@@ -841,26 +947,28 @@
         """Perceive and create atom groups for each molecule in ``compounds``.
 
         Parameters
         ----------
         compounds : iterable of :class:`~luna.MyBio.PDB.Residue.Residue`
             A sequence of molecules.
         mol_objs_dict : dict
-            Map a compound, represented by its id, to a molecular object (:class:`~luna.wrappers.base.MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`,
+            Map a compound, represented by its id, to a molecular object
+            (:class:`~luna.wrappers.base.MolWrapper`,
+            :class:`rdkit.Chem.rdchem.Mol`,
             or :class:`openbabel.pybel.Molecule`).
 
-            This parameter can be used in cases where the ligand is read from a molecular file
-            and no standardization or validation is required.
+            This parameter can be used in cases where the ligand is read from a
+            molecular file and no standardization or validation is required.
 
         Returns
         -------
          : `AtomGroupsManager`
-            An `AtomGroupsManager` object containing all atom groups perceived for the molecules in ``compounds``.
+            An `AtomGroupsManager` object containing all atom groups perceived
+            for the molecules in ``compounds``.
         """
-
         mol_objs_dict = mol_objs_dict or {}
 
         self.atm_grps_mngr = AtomGroupsManager()
         self.atm_mapping = {}
 
         compounds = set(compounds)
         init_comps_set = set(compounds)
@@ -872,74 +980,346 @@
 
         # Controls which compounds are allowed to expand
         # when 'expand_selection' is set ON.
         pruned_comps = set()
         # Create a queue of compounds to be processed.
         comp_queue = set(compounds)
 
+        # Map Residue objects to a MolWrapper object.
+        new_mol_objs_dict = {}
+        # Initial compounds + border compounds.
+        target_compounds = set()
+        # Metals are prepared separatelly.
+        metals = set()
+
         while comp_queue:
-            try:
-                comp = comp_queue.pop()
+            comp = comp_queue.pop()
+
+            # Skip molecules provided as a molecular object.
+            if comp.id in mol_objs_dict:
+                new_mol_objs_dict[comp] = mol_objs_dict[comp.id]
+                continue
 
-                logger.debug("It will try to perceive the features of the "
-                             "compound '%s' as no predefined properties "
-                             "were provided." % comp.full_name)
-
-                mol_obj = mol_objs_dict.get(comp.id, None)
-
-                # If no OBMol object was defined and expand_selection
-                # was set ON and it is not a border compound, it will
-                # get all compounds around the target and create a new
-                # OBMol object with them.
-                if mol_obj is None and self.expand_selection:
-                    # Remove the ligand from the list when
-                    # it was provided as an OBMol object.
-                    comp_list = [c for c in get_proximal_compounds(comp)
-                                 if c.id not in mol_objs_dict]
-
-                    # Expands the queue of compounds
-                    # with any new border compound.
-                    if comp not in pruned_comps:
-                        border_comps = set(comp_list) - compounds
-                        pruned_comps |= border_comps
-                        comp_queue |= border_comps
+            # Add this compound to the binding site set.
+            if not comp.is_metal():
+                target_compounds.add(comp)
+            else:
+                metals.add(comp)
 
-                # Otherwise, the compound list will be composed
-                # only by the target compound.
-                else:
-                    comp_list = [comp]
+            if self.expand_selection:
+                # Remove the ligand from the list when
+                # it was provided as an OBMol object.
+                comp_list = [c for c in get_proximal_compounds(comp)
+                             if c.id not in mol_objs_dict]
+
+                for prox_comp in comp_list:
+                    if not prox_comp.is_metal():
+                        target_compounds.add(prox_comp)
+                    else:
+                        metals.add(prox_comp)
+
+                # Expands the queue of compounds
+                # with any new border compound.
+                if comp not in pruned_comps:
+                    border_comps = set(comp_list) - compounds
+                    pruned_comps |= border_comps
+                    comp_queue |= border_comps
 
-                # Recover all atoms from the previous selected compounds.
-                selector = Selector(keep_altloc=False,
-                                    keep_hydrog=self.keep_hydrog)
-                atoms = tuple([a for r in comp_list
-                               for a in r.get_unpacked_list()
-                               if selector.accept_atom(a)])
-
-                self._assign_properties(comp, atoms, mol_obj)
-            except Exception:
-                logger.debug("Features for the compound '%s' were "
-                             "not correctly perceived." % comp)
+            # Otherwise, the compound list will be composed
+            # only by the target compound.
+            else:
+                comp_list = [comp]
 
-                if self.critical:
-                    raise
+        # Stores atoms involved in metal coordination as a dict of dict,
+        # where the first key is the residue and the second key is an atom.
+        # The values are sets of metals (Residue objects).
+        metals_coord = self._find_metal_coordination(target_compounds, metals)
+
+        # Assign properties for ligands provided as external MOL files.
+        for comp, mol_obj in new_mol_objs_dict.items():
+            target_atoms = self._get_atoms(comp)
+            self._assign_properties(mol_obj, target_atoms)
+
+        # Assign properties for molecules from PDB files.
+        if target_compounds:
+            mol_obj, target_atoms = \
+                self._get_mol_from_entity(target_compounds,
+                                          metals_coord=metals_coord)
+            self._assign_properties(mol_obj, target_atoms)
+
+        # Assign properties to metals.
+        if metals:
+            self._assing_metal_properties(metals)
 
+        # Apply cache.
         if self.cache and cached_compounds:
+            print("\n\nSetting cache...\n\n")
             self._apply_cache(cached_compounds, comp.get_parent_by_level("M"))
 
         # Remove atom groups not comprising the provided
         # compound list (parameter 'compounds').
         remove_atm_grps = []
         for atm_grp in self.atm_grps_mngr:
             if any([c in init_comps_set for c in atm_grp.compounds]) is False:
                 remove_atm_grps.append(atm_grp)
         self.atm_grps_mngr.remove_atm_grps(remove_atm_grps)
 
         return self.atm_grps_mngr
 
+    def _find_metal_coordination(self, compounds, metals):
+
+        # Stores atoms involved in metal coordination as a dict of dict,
+        # where the first key is the residue and the second key is an atom.
+        # The values are sets of metals (Residue objects).
+        custom_dict = lambda: {"atm_idx": None, "metals": set()}
+        metals_coord = defaultdict(lambda: defaultdict(custom_dict))
+
+        for metal in metals:
+            # Identifies potential dative bonds with metals.
+            atm_pairs = get_contacts_with(metal, radius=METAL_COMPLEX_DIST)
+            for atm1, atm2 in atm_pairs:
+                if atm1.parent.is_metal() and not atm2.parent.is_metal():
+                    other_atm = atm2
+                elif not atm1.parent.is_metal() and atm2.parent.is_metal():
+                    other_atm = atm1
+                # Skip if the pair contains two metals or no metal.
+                else:
+                    continue
+
+                # Skip pairs whose non-metal compound is not
+                # in ``target_compounds``
+                if other_atm.parent not in compounds:
+                    continue
+
+                # Skip pairs whose atom is not an O, N, or S.
+                if other_atm.element not in ["O", "N", "S"]:
+                    continue
+
+                # Add this metal to the set of metals being
+                # coordinated by the non-metal atom.
+                other_atm.metal_coordination.add(metal)
+
+                # Add the pair to the dict 'metals_coord'.
+                metals_coord[other_atm.parent][other_atm]["metals"].add(metal)
+
+        return metals_coord
+
+    def _assign_properties(self, mol_obj, target_atoms=None):
+        try:
+            # Create a new MolWrapper object.
+            mol_obj = MolWrapper(mol_obj)
+
+            if mol_obj.get_num_heavy_atoms() != len(target_atoms):
+                raise MoleculeSizeError("The number of heavy atoms in the PDB "
+                                        "selection and in the MOL file are "
+                                        "different.")
+
+            # Ignore hydrogen atoms.
+            atm_obj_list = [atm for atm in mol_obj.get_atoms()
+                            if atm.get_atomic_num() != 1]
+
+            atm_map = {}
+            trgt_atms = {}
+            ob_atms_map = {}
+            for i, atm_obj in enumerate(atm_obj_list):
+                atm_key = target_atoms[i].get_full_id()
+
+                atm_map[atm_obj.get_idx()] = atm_key
+                ob_atms_map[atm_key] = atm_obj
+
+                trgt_atms[atm_key] = self._new_extended_atom(target_atoms[i])
+                # Update atomic invariants for new ExtendedAtoms created.
+                trgt_atms[atm_key].invariants = \
+                    atm_obj.get_atomic_invariants()
+
+            # Set all neighbors, i.e., covalently bonded atoms.
+            for bond_obj in mol_obj.get_bonds():
+                bgn_atm_obj = bond_obj.get_begin_atom()
+                end_atm_obj = bond_obj.get_end_atom()
+
+                # At least one of the atoms must be a non-hydrogen atom.
+                if (bgn_atm_obj.get_atomic_num() != 1
+                        or end_atm_obj.get_atomic_num() != 1):
+
+                    # If the atom 1 is not a hydrogen, add atom 2 to its
+                    # neighbor list.
+                    if bgn_atm_obj.get_atomic_num() != 1:
+                        full_id = atm_map.get(end_atm_obj.get_idx())
+                        coord = \
+                            mol_obj.get_atom_coord_by_id(end_atm_obj.get_id())
+                        atom_info = AtomData(end_atm_obj.get_atomic_num(),
+                                             coord,
+                                             bond_obj.get_bond_type(),
+                                             full_id)
+
+                        bgn_atm = atm_map[bgn_atm_obj.get_idx()]
+                        trgt_atms[bgn_atm].add_nb_info([atom_info])
+
+                    # If the atom 2 is not a hydrogen, add atom 1 to its
+                    # neighbor list.
+                    if end_atm_obj.get_atomic_num() != 1:
+                        full_id = atm_map.get(bgn_atm_obj.get_idx())
+                        coord = \
+                            mol_obj.get_atom_coord_by_id(bgn_atm_obj.get_id())
+                        atom_info = AtomData(bgn_atm_obj.get_atomic_num(),
+                                             coord,
+                                             bond_obj.get_bond_type(),
+                                             full_id)
+                        end_atm = atm_map[end_atm_obj.get_idx()]
+                        trgt_atms[end_atm].add_nb_info([atom_info])
+
+            # Perceive pharmacophoric properties and create AtomGroup objects.
+            group_features = \
+                self.feature_extractor.get_features_by_groups(mol_obj, atm_map)
+            for key in group_features:
+                grp_obj = group_features[key]
+                atoms = [trgt_atms[i] for i in grp_obj["atm_ids"]]
+
+                self.atm_grps_mngr.new_atm_grp(atoms, grp_obj["features"])
+
+            self._fix_pharmacophoric_rules(ob_atms_map)
+
+            # Update the graph in the AtomGroupsManager object
+            # with the current network.
+            for atm in trgt_atms.values():
+                for nb_info in atm.neighbors_info:
+                    if nb_info.full_id in trgt_atms:
+                        pair = atm, trgt_atms[nb_info.full_id]
+                        self.atm_grps_mngr.graph.add_edge(*pair, weight=1)
+
+        except Exception:
+            logger.debug("Features were not correctly perceived.")
+
+            if self.critical:
+                raise
+
+    def _get_default_invariants(self, pdb_atm):
+        # Metal properties.
+        data = DEFAULT_RES_DATA.get(pdb_atm.parent.resname, {})
+        props = data.get("atoms", {})
+
+        invariants = None
+        if pdb_atm.name in props:
+            invariants = props[pdb_atm.name]["invariants"]
+            invariants = [int(i) for i in invariants.split(",")]
+        return invariants
+
+    def _assing_metal_properties(self, metals):
+        for metal in metals:
+            atms = self._get_atoms(metal)
+
+            if len(atms) == 0:
+                logger.error("No atom has been found for residue %s."
+                             % metal.full_name)
+                continue
+
+            if len(atms) > 1:
+                logger.error("An unexpected number of atoms (%d) has been "
+                             "found for residue %s, while 1 was expected."
+                             % (len(atms), metal.full_name))
+                continue
+
+            # Create/recover an extended atom object
+            # and set its atomic invariant.
+            atm = self._new_extended_atom(atms[0])
+            atm.invariants = self._get_default_invariants(atm)
+
+            # Define a new group and add it to 'atm_grps_mngr'.
+            feats = [ChemicalFeature("Atom"), ChemicalFeature("Metal")]
+            self.atm_grps_mngr.new_atm_grp([atm], feats)
+
+    def _fix_pharmacophoric_rules(self, atms_map):
+        """ Fix atom groups where one of its atoms coordinate a metal
+        if necessary.
+
+        For example, an imidazole group may be perceived as a
+        positive ionizable group due to the set of pharmacophoric rules
+        even when its nitrogens are coordinating a metal. In this case,
+        we should not consider the group as ionizable as the N's lone
+        pairs are involved in the dative bond."""
+        for atm_grp1 in self.atm_grps_mngr:
+            atoms = atm_grp1.atoms
+
+            if not any([atm.has_metal_coordination() for atm in atoms]):
+                continue
+
+            is_imidazole = False
+            for atm in atoms:
+                if atm.element not in ["O", "N", "S"]:
+                    continue
+
+                invariants = atm.invariants
+                atm_obj = atms_map[atm.get_full_id()]
+
+                # Imidazole-like, but not tetrazoles.
+                tetrazole_smarts = \
+                    "$([nR1r5;$(n:n:n:n:c),$(n:n:n:c:n)])"
+                imidazole_smarts = \
+                    ("[$([n;H1]cn),$(nc[n;H1]),$([n;H0-1]cn);R1r5;"
+                     f"!{tetrazole_smarts}]")
+                is_imidazole = \
+                    atm_obj.matches_smarts(imidazole_smarts)
+
+                for atm_grp2 in atm.atm_grps:
+                    # Skip groups containing more than one atom.
+                    if len(atm_grp2.atoms) > 1:
+                        continue
+
+                    features = []
+                    for feature in atm_grp2.features:
+                        # If an atom is coordinating a metal
+                        # and it is a donor, but it has no H
+                        # bound to it, remove this feature.
+                        if (atm.has_metal_coordination()
+                                and feature.name == "Donor"
+                                and invariants[5] == 0):
+                            continue
+
+                        # If a N is coordinating a metal
+                        # and it is an acceptor, remove this
+                        # feature because its lone pair is already
+                        # being shared with the metal.
+                        if (atm.has_metal_coordination()
+                                and feature.name == "Acceptor"
+                                and atm.element == "N"):
+                            continue
+
+                        if (atm.has_metal_coordination()
+                                and feature.name == "PositivelyIonizable"
+                                and atm.element == "N"):
+                            continue
+
+                        # If the imidazole N having an H bound to
+                        # it (NH) is not coordinating a metal,
+                        # obligatory the other N is doing so,
+                        # otherwise this N would not reach this
+                        # part of the code.
+                        #
+                        # In this case, remove its feature
+                        # 'Acceptor' because the ring cannot form
+                        # tautomers anymore.
+                        if (not atm.has_metal_coordination()
+                                and feature.name == "Acceptor"
+                                and atm.element == "N"
+                                and is_imidazole):
+                            continue
+
+                        features.append(feature)
+
+                    # Update this atom group's features.
+                    atm_grp2.features = features
+
+            if is_imidazole:
+                features = []
+                for feature in atm_grp1.features:
+                    if feature.name == "PositivelyIonizable":
+                        continue
+                    features.append(feature)
+                atm_grp1.features = features
+
     def _apply_cache(self, compounds, model):
 
         def copy_atom(ref_atm, force_update=False):
             ref_res = ref_atm.parent
             ref_chain = ref_res.parent
 
             # Recover current structure entities.
@@ -954,14 +1334,15 @@
             # Define a new ExtendedAtom.
             ext_atm = self._new_extended_atom(atm)
 
             # Set its atomic invariants.
             ext_atm.invariants = ref_atm.invariants
 
             # Add neighbors' information to the new ExtendedAtom.
+            ext_atm.neighbors_info = []
             for nbi in ref_atm.neighbors_info:
                 atom_info = AtomData(nbi.atomic_num,
                                      nbi.coord, nbi.bond_type,
                                      nbi.full_id)
                 ext_atm.add_nb_info([atom_info])
 
             return ext_atm
@@ -974,17 +1355,20 @@
                 for atm in atm_grp.atoms:
                     # Copy extended atom, i.e., create a new extended
                     # atom or recover an existing one and set invariants
                     # and neighbors' information when necessary.
                     ext_atm = copy_atom(atm, force_update=True)
                     atoms.append(ext_atm)
 
-                # Create the new atom group.
+                # Current features.
                 features = atm_grp.features
-                self.atm_grps_mngr.new_atm_grp(atoms, features)
+
+                # Create the new atom group.
+                atm_grp = self.atm_grps_mngr.new_atm_grp(atoms)
+                atm_grp.features = features
 
         for edge in sorted(self.cache.atm_grps_mngr.graph.edges):
             # Skip already existing edges.
             if edge in self.atm_grps_mngr.graph.edges:
                 continue
 
             atoms = []
@@ -995,133 +1379,62 @@
                 # if necessary.
                 ext_atm = copy_atom(atm)
                 atoms.append(ext_atm)
 
             # Update the AtomGroupsManager object with a new edge.
             self.atm_grps_mngr.graph.add_edge(atoms[0], atoms[1], weight=1)
 
-    def _assign_properties(self, target_compound, target_atoms, mol_obj=None):
-
-        # If no OBMol was defined, create a new one with the compound list.
-        ignored_atoms = []
-        if mol_obj is None:
-            mol_obj, ignored_atoms = self._get_mol_from_entity(target_compound, target_atoms)
-        # Create a new MolWrapper object.
-        mol_obj = MolWrapper(mol_obj)
-
-        # If the add_h property is set to False, the code will not remove any existing hydrogens from the PDB structure.
-        # In these situations, the list of atoms may contain hydrogens. But, we do not need to attribute properties to hydrogens.
-        # We just need them to correctly set properties to heavy atoms. So let's just ignore them.
-        target_atoms = [atm for atm in target_atoms if atm.element != "H" and atm not in ignored_atoms]
-
-        if mol_obj.get_num_heavy_atoms() != len(target_atoms):
-            raise MoleculeSizeError("The number of heavy atoms in the PDB selection and in the MOL file are different.")
-
-        # Ignore hydrogen atoms.
-        atm_obj_list = [atm for atm in mol_obj.get_atoms() if atm.get_atomic_num() != 1]
-
-        atm_map = {}
-        trgt_atms = {}
-        for i, atm_obj in enumerate(atm_obj_list):
-            atm_map[atm_obj.get_idx()] = target_atoms[i].get_full_id()
-
-            trgt_atms[target_atoms[i].get_full_id()] = self._new_extended_atom(target_atoms[i])
-
-            # Invariants are still None, so it means a new ExtendedAtom has just been created.
-            if trgt_atms[target_atoms[i].get_full_id()].invariants is None:
-                # Update atomic invariants for new ExtendedAtoms created.
-                trgt_atms[target_atoms[i].get_full_id()].invariants = atm_obj.get_atomic_invariants()
-
-            # The current atom already has its invariants updated, which means the atom was created previously
-            # by another target compound.
-            else:
-                # In this case, if the current atom belongs to the target compound, we need to prioritize the current target compound
-                # and overwrite the atom's invariants. By doing so, we always guarantee the most accurate information of an atom.
-                #
-                # It is done because some atoms are updated by centroids (target compound) not corresponding to its real compound.
-                # When it happens, the information of covalently bonded atoms may be lost due to the short COV_SEARCH_RADIUS used when
-                # selecting nearby compounds. As a consequence, these atoms will have their properties and topology incorrectly
-                # perceived.
-                #
-                # However, we need to highlight that the main goal of selecting atoms using COV_SEARCH_RADIUS is to find atoms
-                # covalently bonded to the current compound. Therefore, atoms in the border of nearby molecules are not important
-                # right now and they will be updated in their own time.
-                if trgt_atms[target_atoms[i].get_full_id()].parent == target_compound:
-                    # Update the atomic invariants for an ExtendedAtom.
-                    trgt_atms[target_atoms[i].get_full_id()].invariants = atm_obj.get_atomic_invariants()
-
-        # Set all neighbors, i.e., covalently bonded atoms.
-        for bond_obj in mol_obj.get_bonds():
-            bgn_atm_obj = bond_obj.get_begin_atom()
-            end_atm_obj = bond_obj.get_end_atom()
-
-            # At least one of the atoms must be a non-hydrogen atom.
-            if bgn_atm_obj.get_atomic_num() != 1 or end_atm_obj.get_atomic_num() != 1:
-                # If the atom 1 is not a hydrogen, add atom 2 to its neighbor list.
-                if bgn_atm_obj.get_atomic_num() != 1:
-                    # If the current bgn_atm_obj consists of an atom from the current target compound, we can update its information.
-                    # Other compounds are ignored for now as they will have their own time to update its information.
-                    if trgt_atms[atm_map[bgn_atm_obj.get_idx()]].parent == target_compound:
-                        full_id = atm_map.get(end_atm_obj.get_idx())
-                        coord = mol_obj.get_atom_coord_by_id(end_atm_obj.get_id())
-                        atom_info = AtomData(end_atm_obj.get_atomic_num(), coord, bond_obj.get_bond_type(), full_id)
-                        trgt_atms[atm_map[bgn_atm_obj.get_idx()]].add_nb_info([atom_info])
-
-                # If the atom 2 is not a hydrogen, add atom 1 to its neighbor list.
-                if end_atm_obj.get_atomic_num() != 1:
-                    # If the current end_atm_obj consists of an atom from the current target compound, we can update its information.
-                    # Other compounds are ignored for now as they will have their own time to update its information.
-                    if trgt_atms[atm_map[end_atm_obj.get_idx()]].parent == target_compound:
-                        full_id = atm_map.get(bgn_atm_obj.get_idx())
-                        coord = mol_obj.get_atom_coord_by_id(bgn_atm_obj.get_id())
-                        atom_info = AtomData(bgn_atm_obj.get_atomic_num(), coord, bond_obj.get_bond_type(), full_id)
-                        trgt_atms[atm_map[end_atm_obj.get_idx()]].add_nb_info([atom_info])
-
-        group_features = self.feature_extractor.get_features_by_groups(mol_obj, atm_map)
-        for key in group_features:
-            grp_obj = group_features[key]
-
-            # It only accepts groups containing at least one atom from the target compound.
-            if any([trgt_atms[i].parent == target_compound for i in grp_obj["atm_ids"]]) is False:
-                continue
-
-            atoms = [trgt_atms[i] for i in grp_obj["atm_ids"]]
-            self.atm_grps_mngr.new_atm_grp(atoms, grp_obj["features"])
-
-        # Update the graph in the AtomGroupsManager object with the current compound information.
-        for mybio_atm in target_compound.get_atoms():
-            if mybio_atm.get_full_id() in trgt_atms and mybio_atm.parent == target_compound:
-                atm = trgt_atms[mybio_atm.get_full_id()]
-
-                for nb_info in atm.neighbors_info:
-                    if nb_info.full_id in trgt_atms:
-                        self.atm_grps_mngr.graph.add_edge(atm, trgt_atms[nb_info.full_id], weight=1)
-        return True
-
     def _new_extended_atom(self, atm, invariants=None):
         if atm not in self.atm_mapping:
             self.atm_mapping[atm] = ExtendedAtom(atm, invariants=invariants)
 
         return self.atm_mapping[atm]
 
-    def _get_mol_from_entity(self, target_compound, target_atoms):
-        validate_mol = self.amend_mol
-        standardize_mol = self.amend_mol and target_compound.is_residue()
-
-        atom_selector = AtomSelector(target_atoms, keep_altloc=False, keep_hydrog=self.keep_hydrog)
-
-        return biopython_entity_to_mol(target_compound.get_parent_by_level('M'), atom_selector,
-                                       validate_mol=validate_mol, standardize_mol=standardize_mol, add_h=self.add_h,
-                                       ph=self.ph, mol_obj_type=self.mol_obj_type, tmp_path=self.tmp_path)
+    def _get_atoms(self, compound):
+        selector = Selector(keep_altloc=False,
+                            keep_hydrog=self.keep_hydrog)
+
+        return [atm for atm in compound.get_unpacked_list()
+                if selector.accept_atom(atm)]
+
+    def _get_mol_from_entity(self, compounds, metals_coord=None):
+
+        atoms = [atm
+                 for comp in sorted(compounds,
+                                    key=lambda c: (c.parent.parent.id,
+                                                   c.parent.id, c.idx))
+                 for atm in self._get_atoms(comp)]
+
+        model = atoms[0].get_parent_by_level('M')
+        atom_selector = AtomSelector(atoms, keep_altloc=False,
+                                     keep_hydrog=self.keep_hydrog)
+
+        mol_obj, ignored_atoms = \
+            biopython_entity_to_mol(model, atom_selector,
+                                    amend_mol=self.amend_mol,
+                                    add_h=self.add_h, ph=self.ph,
+                                    metals_coord=metals_coord,
+                                    tmp_path=self.tmp_path)
+
+        # If the add_h property is set to False, the code will not remove any
+        # existing hydrogens from the PDB structure. In these situations, the
+        # list of atoms may contain hydrogens. But, we do not need to attribute
+        # properties to hydrogens. We just need them to correctly set
+        # properties to heavy atoms. So let's just ignore them.
+        target_atoms = [atm for atm in atoms if atm.element != "H"
+                        and atm not in ignored_atoms]
+
+        return mol_obj, target_atoms
 
 
 class AtomGroupNeighborhood:
     """ Class for fast neighbor atom groups searching.
 
-    ``AtomGroupNeighborhood`` makes use of a KD Tree implemented in C, so it's fast.
+    ``AtomGroupNeighborhood`` makes use of a KD Tree implemented in C,
+    so it's fast.
 
     Parameters
     ----------
     atm_grps : iterable of `AtomGroup`, optional
         A sequence of `AtomGroup` objects, which is used in the queries.
         It can contain atom groups from different molecules.
     bucket_size : int
@@ -1141,17 +1454,19 @@
         self.coords = np.array(coord_list).astype("f")
         assert(bucket_size > 1)
         assert(self.coords.shape[1] == 3)
         self.kdt = KDTree(3, bucket_size)
         self.kdt.set_coords(self.coords)
 
     def search(self, center, radius):
-        """Return all atom groups in ``atm_grps`` that is up to a maximum of ``radius`` away (measured in Å) of ``center``.
+        """Return all atom groups in ``atm_grps`` that is up to a maximum of
+        ``radius`` away (measured in Å) of ``center``.
 
-        For atom groups with more than one atom, their centroid is used as a reference.
+        For atom groups with more than one atom, their centroid is used as a
+        reference.
         """
         self.kdt.search(center, radius)
         indices = self.kdt.get_indices()
         n_grps_list = []
         atm_grps = self.atm_grps
         for i in indices:
             a = atm_grps[i]
```

### Comparing `luna-0.12.2/luna/mol/templates.py` & `luna-0.13.0/luna/mol/templates.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,91 +11,115 @@
 logger = logging.getLogger()
 
 
 class Template:
     """Standardize small molecules based on templates."""
 
     def assign_bond_order(self):
-        """Assign bond order to a molecular object. However, this method is not implemented by default.
-        Instead, you should use a class that inherits from `Template` and
-        implements :meth:`assign_bond_order`. An example is the class `LigandExpoTemplate` that assigns bonds
-        order based on ligands SMILES from `LigandExpo <http://ligand-expo.rcsb.org/>`_.
-        Therefore, you should define your own logic beyond :meth:`assign_bond_order` that meets your goals."""
+        """Assign bond order to a molecular object. However, this method
+        is not implemented by default. Instead, you should use a class
+        that inherits from `Template` and implements :meth:`assign_bond_order`.
+        An example is the class `LigandExpoTemplate` that assigns bonds
+        order based on ligands SMILES from
+        `LigandExpo <http://ligand-expo.rcsb.org/>`_. Therefore, you should
+        define your own logic beyond :meth:`assign_bond_order` that meets
+        your goals."""
         raise NotImplementedError("Subclasses should implement this.")
 
 
 class LigandExpoTemplate(Template):
-    """Standardize small molecules based on templates (SMILES) from `LigandExpo <http://ligand-expo.rcsb.org/>`_.
+    """Standardize small molecules based on templates (SMILES)
+    from `LigandExpo <http://ligand-expo.rcsb.org/>`_.
 
     Parameters
     ----------
     lig_expo_file : str
-        The `LigandExpo <http://ligand-expo.rcsb.org/>`_ file containing the SMILES and ligand ids.
+        The `LigandExpo <http://ligand-expo.rcsb.org/>`_ file containing
+        the SMILES and ligand ids.
     """
 
     def __init__(self, lig_expo_file=LIGAND_EXPO_FILE):
 
         self.lig_expo_file = lig_expo_file
         self._data = None
 
     @property
     def data(self):
-        """:py:class:`pandas.DataFrame` : The `LigandExpo <http://ligand-expo.rcsb.org/>`_ data."""
+        """:py:class:`pandas.DataFrame` : \
+                The `LigandExpo <http://ligand-expo.rcsb.org/>`_ data."""
         if self._data is None:
-            self._data = pd.read_csv(self.lig_expo_file, sep="\t+", na_filter=False,
-                                     names=["smiles", "ligand_id"], usecols=[0, 1], engine='python').dropna()
+            self._data = pd.read_csv(self.lig_expo_file,
+                                     sep="\t+",
+                                     na_filter=False,
+                                     names=["smiles", "ligand_id"],
+                                     usecols=[0, 1],
+                                     engine='python').dropna()
         return self._data
 
     def get_ligand_smiles(self, lig_id):
         """Get SMILES for the ligand ``lig_id``.
 
         Parameters
         ----------
         lig_id : str
-            The ligand identifier (PDB id) in `LigandExpo <http://ligand-expo.rcsb.org/>`_.
+            The ligand identifier (PDB id) in
+            `LigandExpo <http://ligand-expo.rcsb.org/>`_.
 
         Returns
         ----------
         smiles : str or None
             The ligand SMILES.
         """
 
         data = self.data[self.data["ligand_id"] == lig_id]["smiles"]
         if data.shape[0] == 0:
             return None
         return data.values[0]
 
     def assign_bond_order(self, mol_obj, lig_id):
-        """Assign bond order to a molecular object based on its `LigandExpo <http://ligand-expo.rcsb.org/>`_ SMILES.
+        """Assign bond order to a molecular object based on its
+        `LigandExpo <http://ligand-expo.rcsb.org/>`_ SMILES.
 
         Parameters
         ----------
-        mol_obj : :class:`~luna.wrappers.base.MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`
+        mol_obj : :class:`~luna.wrappers.base.MolWrapper`, \
+                    :class:`rdkit.Chem.rdchem.Mol`, or \
+                    :class:`openbabel.pybel.Molecule`
             A molecule to standardise.
         lig_id : str
-            The ligand identifier (PDB id) in `LigandExpo <http://ligand-expo.rcsb.org/>`_.
+            The ligand identifier (PDB id) in \
+                `LigandExpo <http://ligand-expo.rcsb.org/>`_.
 
         Returns
         -------
-        new_mol : :class:`~luna.wrappers.base.MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`
+        new_mol : :class:`~luna.wrappers.base.MolWrapper`, \
+                    :class:`rdkit.Chem.rdchem.Mol`, or \
+                    :class:`openbabel.pybel.Molecule`
             A standardized molecular object of the same type as ``mol_obj``.
         """
-
         tmp_mol_obj = MolWrapper(mol_obj)
         if tmp_mol_obj.is_rdkit_obj():
             smiles = self.get_ligand_smiles(lig_id)
             # Raise an exception when the template is not found.
             if smiles is None:
-                raise MoleculeNotFoundError("It is not possible to assign the bond orders to the ligand %s because "
-                                            "its corresponding template was not found at Ligand Expo." % lig_id)
-
-            template = MolWrapper.from_smiles(smiles, mol_obj_type="rdkit").unwrap()
-
-            # Note that the template molecule should have no explicit hydrogens else the algorithm will fail.
-            new_mol = AssignBondOrdersFromTemplate(template, tmp_mol_obj.unwrap())
+                error_msg = ("It is not possible to assign the bond orders to "
+                             "the ligand %s because its corresponding "
+                             "template was not found at Ligand Expo." % lig_id)
+                raise MoleculeNotFoundError(error_msg)
+
+            template = MolWrapper.from_smiles(smiles,
+                                              mol_obj_type="rdkit").unwrap()
+
+            # Note that the template molecule should have no explicit
+            # hydrogens else the algorithm will fail.
+            new_mol = AssignBondOrdersFromTemplate(template,
+                                                   tmp_mol_obj.unwrap())
 
             if isinstance(mol_obj, MolWrapper):
                 return MolWrapper(mol_obj)
             return new_mol
         else:
-            logger.exception("Objects of type '%s' are not currently accepted." % mol_obj.__class__)
-            raise MoleculeObjectTypeError("Objects of type '%s' are not currently accepted." % mol_obj.__class__)
+            logger.exception("Objects of type '%s' are not currently accepted."
+                             % mol_obj.__class__)
+            raise MoleculeObjectTypeError("Objects of type '%s' are not "
+                                          "currently accepted."
+                                          % mol_obj.__class__)
```

### Comparing `luna-0.12.2/luna/projects.py` & `luna-0.13.0/luna/projects.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,197 +64,229 @@
 class EntryResults:
 
     """Store entry results.
 
     Parameters
     ----------
     entry: :class:`~luna.mol.entry.Entry`
-        An :class:`~luna.mol.entry.Entry` object that represents a molecule or an entire chain.
+        An :class:`~luna.mol.entry.Entry` object that represents a molecule or
+        an entire chain.
     atm_grps_mngr: :class:`~luna.mol.groups.AtomGroupsManager`
-        An :class:`~luna.mol.groups.AtomGroupsManager` object that stores the perceived atoms and
-        atom groups in the vicinity given by ``entry``.
+        An :class:`~luna.mol.groups.AtomGroupsManager` object that stores the
+        perceived atoms and atom groups in the vicinity given by ``entry``.
     interactions_mngr: :class:`~luna.interaction.calc.InteractionsManager`
-        An :class:`~luna.interaction.calc.InteractionsManager` object that interactions in the vicinity
-        given by ``entry``.
+        An :class:`~luna.interaction.calc.InteractionsManager` object that
+        interactions in the vicinity given by ``entry``.
     ifp: :class:`~luna.interaction.fp.fingerprint.Fingerprint`, optional
         An interaction fingerprint (IFP) generated for ``entry``.
-    mfp: RDKit :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` or :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`, optional
+    mfp: RDKit :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` or \
+            :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`, optional
         A molecular fingerprint generated for ``entry``.
 
     Attributes
     ----------
     entry : :class:`~luna.mol.entry.Entry`
     atm_grps_mngr: :class:`~luna.mol.groups.AtomGroupsManager`
     interactions_mngr: :class:`~luna.interaction.calc.InteractionsManager`
     ifp: :class:`~luna.interaction.fp.fingerprint.Fingerprint`
-    mfp: RDKit :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` or :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`
+    mfp: RDKit :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` or \
+            :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`
     version : str
         The LUNA's version with which results were generated.
     """
 
-    def __init__(self, entry, atm_grps_mngr, interactions_mngr, ifp=None, mfp=None):
+    def __init__(self,
+                 entry,
+                 atm_grps_mngr,
+                 interactions_mngr,
+                 ifp=None,
+                 mfp=None):
+
         self.entry = entry
         self.atm_grps_mngr = atm_grps_mngr
         self.interactions_mngr = interactions_mngr
         self.ifp = ifp
         self.mfp = mfp
         self.version = __version__
 
     def save(self, output_file, compressed=True):
-        """Write the pickled representation of this object to the file ``output_file``.
+        """Write the pickled representation of this object to the file
+        ``output_file``.
 
         Parameters
         ----------
         output_file : str
             The output file where the pickled representation will be saved.
         compressed : bool, optional
-            If True (the default), compress the pickled representation as a  gzip file (.gz).
+            If True (the default), compress the pickled representation as a
+            gzip file (.gz).
 
         Raises
         -------
         FileNotCreated
             If the file could not be created.
         """
         pickle_data(self, output_file, compressed)
 
     @staticmethod
     def load(input_file):
-        """Read the pickled representation of an `EntryResults` object from the file
-        ``input_file`` and return the reconstituted object hierarchy specified therein.
-        ``input_file`` can be a gzip-compressed file.
+        """Read the pickled representation of an `EntryResults` object from
+        the file ``input_file`` and return the reconstituted object hierarchy
+        specified therein. ``input_file`` can be a gzip-compressed file.
 
         Raises
         -------
         PKLNotReadError
             If the file could not be loaded.
         """
         return unpickle_data(input_file)
 
 
 class Project:
 
     """Define a LUNA project.
 
     .. note::
-        This class is not intended to be used directly because :meth:`run` is not implemented by default.
-        Instead, you should use a class that inherits from `Project` and implements :meth:`run`.
-        An example is the class :class:`LocalProject` that implements a custom :meth:`run` that saves results
-        as local files.
+        This class is not intended to be used directly because :meth:`run` is
+        not implemented by default. Instead, you should use a class that
+        inherits from `Project` and implements :meth:`run`.
+        An example is the class :class:`LocalProject` that implements a custom
+        :meth:`run` that saves results as local files.
 
     Parameters
     ----------
     entries : iterable of :class:`~luna.mol.entry.Entry`
-        Entries determine the target molecule to which interactions and other properties
-        will be calculated. They can be ligands, chains, etc, and can be defined in a number of ways.
-        Each entry has an associated PDB file that may contain macromolecules (protein, RNA, DNA) and
-        other small molecules, water, and ions. Refer to :class:`~luna.mol.entry.Entry` for more information.
+        Entries determine the target molecule to which interactions and other
+        properties will be calculated. They can be ligands, chains, etc, and
+        can be defined in a number of ways. Each entry has an associated PDB
+        file that may contain macromolecules (protein, RNA, DNA) and other
+        small molecules, water, and ions.
+        Refer to :class:`~luna.mol.entry.Entry` for more information.
     working_path : str
         Where project results will be saved.
     pdb_path : str
-        Path containing local PDB files or to where the PDB files will be downloaded.
-        PDB filenames must match that defined for the entries.
+        Path containing local PDB files or to where the PDB files will be
+        downloaded. PDB filenames must match that defined for the entries.
         If not provided, the default PDB path will be used.
     overwrite_path : bool
-        If True, allow LUNA to overwrite any existing directory, which may remove files from a previous project.
-        The default value is False.
+        If True, allow LUNA to overwrite any existing directory, which may
+        remove files from a previous project. The default value is False.
     add_h : bool
         Define if you need to add hydrogens or not. The default value is True.
 
         .. note::
-            To be cautious, it does not add hydrogens to NMR-solved structures and ligands initialized from molecular files
-            (:class:`~luna.mol.entry.MolFileEntry` objects) as they usually already contain hydrogens.
+            To be cautious, it does not add hydrogens to NMR-solved structures
+            and ligands initialized from molecular files
+            (:class:`~luna.mol.entry.MolFileEntry` objects) as they usually
+            already contain hydrogens.
     ph : float
-        Control the pH and how the hydrogens are going to be added. The default value is 7.4.
+        Control the pH and how the hydrogens are going to be added.
+        The default value is 7.4.
 
         .. note::
-            To be cautious, it does not modify the protonation of molecular files defined by a
-            :class:`~luna.mol.entry.MolFileEntry` object.
+            To be cautious, it does not modify the protonation of molecular
+            files defined by a :class:`~luna.mol.entry.MolFileEntry` object.
     amend_mol : bool
-        If True (the default), try to fix atomic charges, valence, and bond types for small molecules and residues at PDB files.
-        Only molecules at PDB files are validated because they do not contain charge, valence, and bond types, which may
-        cause molecules to be incorrectly perceived. More information :ref:`here <Ligands in PDB files>`.
+        If True (the default), try to fix atomic charges, valence, and bond
+        types for small molecules and residues at PDB files. Only molecules
+        at PDB files are validated because they do not contain charge, valence,
+        and bond types, which may cause molecules to be incorrectly perceived.
+        More information :ref:`here <Ligands in PDB files>`.
 
         .. note::
-            Molecules from external files (:class:`~luna.mol.entry.MolFileEntry` objects) will not be modified.
-    mol_obj_type : {'rdkit', 'openbabel'}
-        Define which library (RDKit or Open Babel) to use to parse molecules.
-        The default value is 'rdkit'.
+            Molecules from external files
+            (:class:`~luna.mol.entry.MolFileEntry` objects) will not be
+            modified.
     atom_prop_file : str
-        A feature definition file (FDef) containing all information needed to define a set of
-        chemical or pharmacophoric features. The default value is 'LUNA.fdef', which contains
-        default LUNA features definition.
+        A feature definition file (FDef) containing all information needed to
+        define a set of chemical or pharmacophoric features.
+        The default value is 'LUNA.fdef', which contains default LUNA features
+        definition.
     inter_calc : :class:`~luna.interaction.calc.InteractionCalculator`
         Define which and how interactions are calculated.
     binding_mode_filter : :class:`~luna.interaction.filter.BindingModeFilter`
         Define how to filter interactions based on binding modes.
     calc_mfp : bool
-        If True, generate ECFP4 fingerprints for each entry in ``entries``. The default value is False.
+        If True, generate ECFP4 fingerprints for each entry in ``entries``.
+        The default value is False.
     mfp_output : str
-        If ``calc_mfp`` is True, save ECFP4 fingerprints to file ``mfp_output``.
-        If not provided, fingerprints are saved at <``working_path``>/results/fingerprints/mfp.csv.
+        If ``calc_mfp`` is True, save ECFP4 fingerprints to file
+        ``mfp_output``. If not provided, fingerprints are saved at
+        <``working_path``>/results/fingerprints/mfp.csv.
     calc_ifp : bool
-        If True (the default), generate LUNA interaction fingerprints (IFPs) for each entry in ``entries``.
+        If True (the default), generate LUNA interaction fingerprints (IFPs)
+        for each entry in ``entries``.
     ifp_num_levels : int
-        The maximum number of iterations for fingerprint generation. The default value is 2.
+        The maximum number of iterations for fingerprint generation.
+        The default value is 2.
     ifp_radius_step : float
         The multiplier used to increase shell size at each iteration.
-        At iteration 0, shell radius is 0 * ``radius_step``, at iteration 1, radius is
-        1 * ``radius_step``, etc. The default value is 5.73171.
+        At iteration 0, shell radius is 0 * ``radius_step``, at iteration 1,
+        radius is 1 * ``radius_step``, etc. The default value is 5.73171.
     ifp_length : int
-        The fingerprint length (total number of bits). The default value is 4096.
+        The fingerprint length (total number of bits).
+        The default value is 4096.
     ifp_count : bool
-        If True (the default), create a count fingerprint (:class:`~luna.interaction.fp.fingerprint.CountFingerprint`).
-        Otherwise, return a bit fingerprint (:class:`~luna.interaction.fp.fingerprint.Fingerprint`).
+        If True (the default), create a count fingerprint
+        (:class:`~luna.interaction.fp.fingerprint.CountFingerprint`).
+        Otherwise, return a bit fingerprint
+        (:class:`~luna.interaction.fp.fingerprint.Fingerprint`).
     ifp_diff_comp_classes :
-        If True (the default), include differentiation between compound classes.
-        That means structural information originated from :class:`~luna.mol.groups.AtomGroup` objects
-        belonging to residues, nucleotides,  ligands, or water molecules will be considered different
+        If True (the default), include differentiation between compound
+        classes. That means structural information originated from
+        :class:`~luna.mol.groups.AtomGroup` objects belonging to residues,
+        nucleotides,  ligands, or water molecules will be considered different
         even if their structural information are the same.
-        This is useful for example to differentiate protein-ligand interactions from residue-residue ones.
+        This is useful for example to differentiate protein-ligand interactions
+        from residue-residue ones.
     ifp_type : :class:`~luna.interaction.fp.type.IFPType`
         The fingerprint type (EIFP, FIFP, or HIFP). The default value is EIFP.
     ifp_output : str
-        If ``calc_ifp`` is True, save LUNA interaction fingerprints (IFPs) to file ``ifp_output``.
-        If not provided, fingerprints are saved at <``working_path``>/results/fingerprints/ifp.csv.
+        If ``calc_ifp`` is True, save LUNA interaction fingerprints (IFPs) to
+        file ``ifp_output``. If not provided, fingerprints are saved at
+        <``working_path``>/results/fingerprints/ifp.csv.
     ifp_sim_matrix_output : str, optional
-        If provided, compute Tanimoto similarity between interaction fingerprints (IFPs)
-        and save the similarity matrix to ``ifp_sim_matrix_output``.
+        If provided, compute Tanimoto similarity between interaction
+        fingerprints (IFPs) and save the similarity matrix to
+        ``ifp_sim_matrix_output``.
     out_pse : bool
         If True, depict interactions save them as Pymol sessions (PSE file).
-        The default value is False. PSE files are saved at <``working_path``>/results/pse.
+        The default value is False. PSE files are saved at
+        <``working_path``>/results/pse.
     append_mode : bool
-        If True, skip entries from processing if a result for them already exists in ``working_path``.
-        This can save processing time in case additional entries are to be added to an existing project.
+        If True, skip entries from processing if a result for them already
+        exists in ``working_path``. This can save processing time in case
+        additional entries are to be added to an existing project.
     verbosity : int
-        Verbosity level. The higher the verbosity level the more information is displayed.
-        Valid values are:
+        Verbosity level. The higher the verbosity level the more information
+        is displayed. Valid values are:
 
             * 4: DEBUG messages;
             * 3: INFO messages (the default);
             * 2: WARNING messages;
             * 1: ERROR messages;
             * 0: CRITICAL messages.
     logging_enabled : bool
         If True (the default), enable the logging system.
     nproc : int
-        The number of CPUs to use. The default value is the ``maximum number of CPUs - 1``.
-        If ``nproc`` is smaller than 1 or greater than the maximum amount of available CPUs at your PC,
-        then ``nproc`` is set to its default value. If you set it to None, LUNA will be run serially.
+        The number of CPUs to use. The default value is the ``maximum number
+        of CPUs - 1``. If ``nproc`` is smaller than 1 or greater than the
+        maximum amount of available CPUs at your PC, then ``nproc`` is set to
+        its default value. If you set it to None, LUNA will be run serially.
 
 
     Attributes
     ----------
     entries : iterable of :class:`~luna.mol.entry.Entry`
     working_path : str
     pdb_path : str
     overwrite_path : bool
     add_h : bool
     ph : float
     amend_mol : bool
-    mol_obj_type : {'rdkit', 'openbabel'}
     atom_prop_file : str
     inter_calc : :class:`~luna.interaction.calc.InteractionCalculator`
     binding_mode_filter : :class:`~luna.interaction.filter.BindingModeFilter`
     calc_mfp : bool
     mfp_output : str
     calc_ifp : bool
     ifp_num_levels : int
@@ -269,27 +301,27 @@
     append_mode : bool
     logging_file : str
         The file to where logging messages are saved.
     version : str
         The LUNA's version with which results were generated.
     errors : list of tuple
         Any errors found during the processing of an entry.
-        Each tuple contains the input and the exception raised during the execution of a task with that input.
+        Each tuple contains the input and the exception raised during the
+        execution of a task with that input.
     """
 
     def __init__(self,
                  entries,
                  working_path,
                  pdb_path=PDB_PATH,
                  overwrite_path=False,
 
                  add_h=True,
                  ph=7.4,
                  amend_mol=True,
-                 mol_obj_type='rdkit',
                  atom_prop_file=ATOM_PROP_FILE,
 
                  inter_calc=None,
                  binding_mode_filter=None,
 
                  calc_mfp=False,
                  mfp_output=None,
@@ -312,23 +344,14 @@
                  verbosity=3,
                  logging_enabled=True,
                  nproc=MAX_NPROCS):
 
         # Property required by self._log()
         self.logging_enabled = logging_enabled
 
-        if mol_obj_type not in ACCEPTED_MOL_OBJ_TYPES:
-            mobj_types = ["'%s'" % m for m in ACCEPTED_MOL_OBJ_TYPES]
-            raise IllegalArgumentError("Invalid value for 'mol_obj_type'. "
-                                       "Objects of type '%s' are not "
-                                       "currently accepted. "
-                                       "The available options are: %s."
-                                       % (mol_obj_type,
-                                          ", ".join(mobj_types)))
-
         self._log("info", "LUNA version: %s." % __version__)
 
         if (inter_calc is not None
                 and isinstance(inter_calc, InteractionCalculator) is False):
             msg = ".".join([InteractionCalculator.__module__,
                             InteractionCalculator.__name__])
             raise IllegalArgumentError("The informed interaction "
@@ -345,15 +368,14 @@
         self.entries = entries
         self.working_path = working_path
         self.pdb_path = pdb_path
         self.overwrite_path = overwrite_path
         self.atom_prop_file = atom_prop_file or ATOM_PROP_FILE
         self.ph = ph
         self.amend_mol = amend_mol
-        self.mol_obj_type = mol_obj_type
         self.add_h = add_h
 
         if inter_calc is None:
             inter_calc = InteractionCalculator(inter_config=INTERACTION_CONFIG)
         self.inter_calc = inter_calc
 
         self.binding_mode_filter = binding_mode_filter
@@ -396,38 +418,41 @@
 
     def __call__(self):
         raise NotImplementedError("This class is not callable. Use a class "
                                   "that implements this method.")
 
     @property
     def project_file(self):
-        """str: Where the pickled representation of the LUNA project is saved."""
+        """str: Where the pickled representation of the LUNA project is \
+        saved."""
         return "%s/project_v%s.pkl.gz" % (self.working_path, __version__)
 
     @property
     def results(self):
         """iterable of `EntryResults`: LUNA results for each entry."""
         for entry in self.entries:
             results = self.get_entry_results(entry)
             if results:
                 yield results
 
     @property
     def interactions_mngrs(self):
         """iterable of :class:`~luna.interaction.calc.InteractionsManager`: \
-            An :class:`~luna.interaction.calc.InteractionsManager` object for each entry."""
+            An :class:`~luna.interaction.calc.InteractionsManager` object \
+            for each entry."""
         for entry in self.entries:
             results = self.get_entry_results(entry)
             if results:
                 yield results.interactions_mngr
 
     @property
     def atm_grps_mngrs(self):
         """iterable of :class:`~luna.mol.groups.AtomGroupsManager`: \
-            An :class:`~luna.mol.groups.AtomGroupsManager` object for each entry."""
+            An :class:`~luna.mol.groups.AtomGroupsManager` object for \
+            each entry."""
         for entry in self.entries:
             results = self.get_entry_results(entry)
             if results:
                 yield results.atm_grps_mngr
 
     @property
     def ifps(self):
@@ -436,15 +461,16 @@
         for entry in self.entries:
             results = self.get_entry_results(entry)
             if results:
                 yield entry, results.ifp
 
     @property
     def mfps(self):
-        """iterable of RDKit :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` \
+        """iterable of \
+            RDKit :class:`~rdkit.DataStructs.cDataStructs.ExplicitBitVect` \
             or :class:`~rdkit.DataStructs.cDataStructs.SparseBitVect`: \
                 A molecular fingerprint for each entry."""
         for entry in self.entries:
             results = self.get_entry_results(entry)
             if results:
                 yield entry, results.mfp
 
@@ -453,23 +479,30 @@
         """int: The number of CPUs to use."""
         return self._nproc
 
     @nproc.setter
     def nproc(self, nproc):
         if nproc is not None:
             if not isinstance(nproc, int) or isinstance(nproc, bool):
-                self._log("warning", "The number of processes must be an integer value, but a(n) %s was provided instead. "
-                          "Therefore, the number of processes 'nproc' was set to its maximum accepted capacity "
-                          "(%d - 1 = %d)." % (nproc.__class__.__name__, mp.cpu_count(), MAX_NPROCS))
+                msg = ("The number of processes must be an integer value, but "
+                       "a(n) %s was provided instead. Therefore, the number "
+                       "of processes 'nproc' was set to its maximum accepted "
+                       "capacity (%d - 1 = %d)."
+                       % (nproc.__class__.__name__, mp.cpu_count(),
+                          MAX_NPROCS))
+                self._log("warning", msg)
                 nproc = MAX_NPROCS
 
             elif nproc < 1:
-                self._log("warning", "It was trying to create an invalid number of processes (%s). Therefore, the number of "
-                          "processes 'nproc' was set to its maximum accepted capacity (%d - 1 = %d)." % (str(nproc), mp.cpu_count(),
-                                                                                                         MAX_NPROCS))
+                msg = ("It was trying to create an invalid number of "
+                       "processes (%s). Therefore, the number of processes "
+                       "'nproc' was set to its maximum accepted capacity "
+                       "(%d - 1 = %d)." % (str(nproc), mp.cpu_count(),
+                                           MAX_NPROCS))
+                self._log("warning", msg)
                 nproc = MAX_NPROCS
 
             elif nproc >= mp.cpu_count():
                 self._log("warning", "It was trying to create %d processes, "
                           "which is equal to or greater than the maximum "
                           "amount of available CPUs (%d). Therefore, the "
                           "number of processes 'nproc' was set to %d "
@@ -652,15 +685,16 @@
     def _validate_entry_format(self, entry):
         if not entry.is_valid():
             raise InvalidEntry("Entry '%s' does not match a LUNA's entry "
                                "format." % entry.to_string())
 
     def verify_pdb_files_existence(self):
         """Verify if a local PDB file exists for each entry in ``entries``.
-            If it does not find a given PDB file, then LUNA will try to download it from RCSB."""
+            If it does not find a given PDB file, then LUNA will try to
+            download it from RCSB."""
         all_pdb_ids = set()
         to_download = set()
         for entry in self.entries:
             pdb_file = "%s/%s.pdb" % (self.pdb_path, entry.pdb_id)
             if not exists(pdb_file):
                 to_download.add(entry.pdb_id)
 
@@ -736,15 +770,14 @@
     def _get_perceiver(self, add_h, cache=None):
         feats_factory_func = ChemicalFeatures.BuildFeatureFactory
         feature_factory = feats_factory_func(self.atom_prop_file)
         feature_extractor = FeatureExtractor(feature_factory)
 
         perceiver = AtomGroupPerceiver(feature_extractor, add_h=add_h,
                                        ph=self.ph, amend_mol=self.amend_mol,
-                                       mol_obj_type=self.mol_obj_type,
                                        cache=cache,
                                        tmp_path="%s/tmp" % self.working_path)
 
         return perceiver
 
     def cache_protein_properties(self, entry):
         self._log("info",
@@ -753,35 +786,49 @@
 
         pdb_parser, structure, ligand = self._parse_complex(entry)
         add_h = self._decide_hydrogen_addition(pdb_parser.get_header(), entry)
 
         inter_config = self.inter_calc.inter_config
         radius = inter_config.get("cache_cutoff",
                                   BOUNDARY_CONFIG["cache_cutoff"])
-        nb_pairs = get_contacts_with(structure[0], ligand,
-                                     level='R', radius=radius)
-        nb_compounds = set([p[1] for p in nb_pairs
-                            if not p[1].is_target()])
-
+        nb_pairs = get_contacts_with(ligand,
+                                     entity=structure[0],
+                                     radius=radius,
+                                     level='R')
+        nb_compounds = set([p[1] for p in nb_pairs])
         mol_objs_dict = {}
         if isinstance(entry, MolFileEntry):
             mol_objs_dict[entry.get_biopython_key()] = entry.mol_obj
 
         perceiver = self._get_perceiver(add_h)
-        atm_grps_mngr = perceiver.perceive_atom_groups(nb_compounds,
-                                                       mol_objs_dict=mol_objs_dict)
+        atm_grps_mngr = \
+            perceiver.perceive_atom_groups(nb_compounds,
+                                           mol_objs_dict=mol_objs_dict)
 
         # Remove any edges involving the ligand.
         valid_edges = set()
         for edge in atm_grps_mngr.graph.edges:
-            if any([atm.parent.is_target() for atm in edge]) is False:
+            if any([atm.parent.is_hetatm() or atm.parent.is_metal()
+                    for atm in edge]) is False:
                 valid_edges.add(edge)
         atm_grps_mngr.graph = nx.Graph()
         atm_grps_mngr.graph.add_edges_from(valid_edges)
 
+        # Remove hetatm and metals from the cache.
+        invalid_atm_grps = [ag for ag in atm_grps_mngr
+                            if (ag.has_hetatm()
+                                or ag.has_metal())]
+        atm_grps_mngr.remove_atm_grps(invalid_atm_grps)
+
+        # Update the list of valid compounds used to generate the cache.
+        invalid_comps = set([c for ag in invalid_atm_grps
+                             for c in ag.compounds
+                             if c.is_hetatm() or c.is_metal()])
+        nb_compounds = nb_compounds - invalid_comps
+
         # Remove dummy chain if the ligand comes from an
         # external molecular file.
         if isinstance(entry, MolFileEntry):
             chain = ligand.parent
             chain.detach_child(ligand.id)
 
             if len(chain.child_list) == 0:
@@ -793,25 +840,29 @@
                                   add_h=False, cache=None):
         self._log("debug", "Starting pharmacophore perception "
                   "for entry '%s'" % entry.to_string())
 
         inter_config = self.inter_calc.inter_config
         radius = inter_config.get("bsite_cutoff",
                                   BOUNDARY_CONFIG["bsite_cutoff"])
-        nb_pairs = get_contacts_with(entity, ligand, level='R', radius=radius)
+        nb_pairs = get_contacts_with(ligand,
+                                     entity=entity,
+                                     radius=radius,
+                                     level='R')
 
         mol_objs_dict = {}
         if isinstance(entry, MolFileEntry):
             mol_objs_dict[entry.get_biopython_key()] = entry.mol_obj
 
         nb_compounds = set([x[1] for x in nb_pairs])
 
         perceiver = self._get_perceiver(add_h, cache)
-        atm_grps_mngr = perceiver.perceive_atom_groups(nb_compounds,
-                                                       mol_objs_dict=mol_objs_dict)
+        atm_grps_mngr = \
+            perceiver.perceive_atom_groups(nb_compounds,
+                                           mol_objs_dict=mol_objs_dict)
 
         self._log("debug", "Pharmacophore perception for entry '%s' has "
                   "finished." % entry.to_string())
 
         return atm_grps_mngr
 
     def _create_mfp(self, entry):
@@ -891,29 +942,31 @@
         pj = ParallelJobs(self.nproc)
         return pj.run_jobs(args=args, consumer_func=self._calc_similarity,
                            output_file=output_file, output_header=header,
                            job_name="Calculate similarities")
 
     def run(self):
         """Run LUNA. However, this method is not implemented by default.
-        Instead, you should use a class that inherits from `Project` and implements :meth:`run`.
-        An example is the class :class:`LocalProject` that implements a custom :meth:`run` that saves results
-        as local files.
+        Instead, you should use a class that inherits from `Project` and
+        implements :meth:`run`. An example is the class :class:`LocalProject`
+        that implements a custom :meth:`run` that saves results as local files.
         """
         self()
 
     def save(self, output_file, compressed=True):
-        """Write the pickled representation of this project to the file ``output_file``.
+        """Write the pickled representation of this project to the file
+        ``output_file``.
 
         Parameters
         ----------
         output_file : str
             The output file where the pickled representation will be saved.
         compressed : bool, optional
-            If True (the default), compress the pickled representation as a  gzip file (.gz).
+            If True (the default), compress the pickled representation as a
+            gzip file (.gz).
 
         Raises
         -------
         FileNotCreated
             If the file could not be created.
         """
         pickle_data(self, output_file, compressed)
@@ -921,43 +974,46 @@
     @staticmethod
     def get_project_file(working_path):
         """Get the pickled project file at ``working_path``."""
         return "%s/project_v%s.pkl.gz" % (working_path, __version__)
 
     @staticmethod
     def load(pathname, verbosity=3, logging_enabled=True):
-        """Read the pickled representation of a `Project` object from a file or project path \
-         and return the reconstituted object hierarchy specified therein. \
-        The ``pathname`` can be a gzip-compressed file.
+        """Read the pickled representation of a `Project` object from a file or
+        project path and return the reconstituted object hierarchy specified
+        therein. The ``pathname`` can be a gzip-compressed file.
 
         Parameters
         ----------
         pathname : str
             A file containing the pickled representation of a `Project` object
-            or the project path (``working_path``) from where the pickled representation will be recovered.
+            or the project path (``working_path``) from where the pickled
+            representation will be recovered.
         verbosity : int
-            Verbosity level. The higher the verbosity level the more information is displayed.
-            Valid values are:
+            Verbosity level. The higher the verbosity level the more
+            information is displayed. Valid values are:
 
                 * 4: DEBUG messages;
                 * 3: INFO messages (the default);
                 * 2: WARNING messages;
                 * 1: ERROR messages;
                 * 0: CRITICAL messages.
         logging_enabled : bool
             If True (the default), enable the logging system.
 
         Raises
         -------
         CompatibilityError
-            If the project version is not compatible with the current LUNA version.
+            If the project version is not compatible with the current
+            LUNA version.
         PKLNotReadError
             If the file could not be loaded.
         IllegalArgumentError
-            If the provided pathname does not exist or is an invalid file/directory.
+            If the provided pathname does not exist or is an invalid
+            file/directory.
         """
 
         # Check if the provided input path is a valid file
         # or a directory containing saved projects.
         if is_file_valid(pathname):
             input_file = pathname
         elif is_directory_valid(pathname):
@@ -1021,34 +1077,41 @@
 
         params = ProjectParams.from_project_obj(self)
         params.save_config_file(config_file)
 
 
 class LocalProject(Project):
 
-    """Define a local LUNA project, i.e., results are saved locally and not to a database.
+    """Define a local LUNA project, i.e., results are saved locally and not to
+    a database.
 
-        This class inherits from `Project` and implements :meth:`~luna.projects.Project.run`.
+    This class inherits from `Project` and implements
+        :meth:`~luna.projects.Project.run`.
 
     Examples
     --------
 
-    In this minimum example, we will calculate protein-ligand interactions for dopamine D4 complexes.
+    In this minimum example, we will calculate protein-ligand interactions for
+    dopamine D4 complexes.
 
-    First, we should define the ligand entries and initialize a new :class:`~luna.interaction.calc.InteractionCalculator`
-    object.
+    First, we should define the ligand entries and initialize a new
+    :class:`~luna.interaction.calc.InteractionCalculator` object.
 
     >>> from luna.util.default_values import LUNA_PATH
     >>> from luna.interaction.calc import InteractionCalculator
-    >>> entries = list(MolFileEntry.from_file(input_file=f"{LUNA_PATH}/tutorial/inputs/MolEntries.txt",
-    ...                                       pdb_id="D4", mol_file=f"{LUNA_PATH}/tutorial/inputs/ligands.mol2"))
-    >>> ic = InteractionCalculator(inter_filter=InteractionFilter.new_pli_filter())
-
-    Finally, just create the new LUNA project with desired parameters and call :meth:`~luna.projects.Project.run`.
-    Here, we opted to define the parameters first as a dict, and then we pass it as an argument to `LocalProject`.
+    >>> entries = list(MolFileEntry.from_file(\
+input_file=f"{LUNA_PATH}/tutorial/inputs/MolEntries.txt",
+    ...                                       pdb_id="D4", \
+mol_file=f"{LUNA_PATH}/tutorial/inputs/ligands.mol2"))
+    >>> ic = InteractionCalculator(inter_filter=\
+InteractionFilter.new_pli_filter())
+
+    Finally, just create the new LUNA project with desired parameters and call
+    :meth:`~luna.projects.Project.run`. Here, we opted to define the parameters
+    first as a dict, and then we pass it as an argument to `LocalProject`.
 
     >>> from luna import LocalProject
     >>> opts = {}
     >>> opts["working_path"] = "%s/Results/Test3" % main_path
     >>> opts["pdb_path"] = f"{LUNA_PATH}/tutorial/inputs/"
     >>> opts["entries"] = entries
     >>> opts["inter_calc"] = ic
@@ -1132,15 +1195,15 @@
 
             # Saving interactions into a Pymol session.
             if self.out_pse:
                 from luna.interaction.view import InteractionViewer
                 pse_path = (self.pse_path
                             or "%s/results/pse/" % self.working_path)
                 pse_file = "%s/%s.pse" % (pse_path, entry.to_string())
-                piv = InteractionViewer(add_directional_arrows=False)
+                piv = InteractionViewer(add_directional_arrows=True)
                 piv.new_session([(entry, interactions_mngr,
                                   entry.pdb_file)], pse_file)
 
             self._log("debug",
                       "Processing of entry '%s' finished successfully."
                       % entry.to_string())
```

### Comparing `luna-0.12.2/luna/run.py` & `luna-0.13.0/luna/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import argparse
 import os
 import shutil
 import configparser
 
-import sys
-scripts = '/media/data/Workspace/Keiser lab/LUNA'
-sys.path.append(scripts)
-
-
 from luna.projects import LocalProject, EntryResults
-from luna.version import __version__ as version
 from luna.config.params import ProjectParams
 from luna.interaction.view import InteractionViewer
 from luna.interaction.fp.type import IFPType
 from luna.util.file import create_directory
 from luna.interaction.calc import InteractionsManager
 from luna.util.logging import VERBOSITY_LEVEL
 
@@ -39,15 +33,15 @@
 
     group = parser.add_argument_group('Entries')
     group.add_argument('-e', "--entries", type=str,
                        help="an input file containing a list of "
                             "entries to process.")
     group.add_argument("-p", "--prot", dest="pdb_id",
                        type=str,
-                       help="the protein PDB id. "
+                       help="A local PDB filename. "
                             "Mandatory if there is at least one entry "
                             "containing only the ligand name. "
                             "This only applies to ligands to be read "
                             "from a multimolecular file.")
     group.add_argument('-l', "--lig", dest="mol_file", type=str,
                        help="a molecular file containing 1 or more ligands. "
                             "Mandatory if there is at least one entry "
```

### Comparing `luna-0.12.2/luna/util/__init__.py` & `luna-0.13.0/luna/util/__init__.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/util/config.py` & `luna-0.13.0/luna/util/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,32 +26,44 @@
         try:
             self.config.read(config_file)
         except Exception as e:
             logger.exception(e)
             raise IOError('Configuration file %s not read.' % config_file)
 
     def parse_value(self, section, property_name):
+        """Transform the value of property ``property_name`` from
+        section ``section`` to a Python object.
+
+        Returns
+        -------
+         : object
+        """
         value = self.config.get(section, property_name)
         return ast.literal_eval(value)
 
     def get_section_map(self, section):
         """Try to access the section ``section`` from the parsed
         configuration file.
+
+        Returns
+        -------
+         : dict
         """
         section_map = {}
         options = self.config.options(section)
         for option in options:
             try:
                 section_map[option] = self.config.get(section, option)
             except Exception as e:
                 logger.exception(e)
                 section_map[option] = None
         return section_map
 
     def as_dict(self, only_props=True):
+        """Return the object parameters as :py:class:`dict`."""
         if only_props:
             return {k: v
                     for s in self.config.sections()
                     for k, v in self.config.items(s)}
         return {s: dict(self.config.items(s)) for s in self.config.sections()}
 
     def __getattr__(self, attr):
```

### Comparing `luna-0.12.2/luna/util/default_values.py` & `luna-0.13.0/luna/util/default_values.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,20 +20,24 @@
 INTERACTION_CONFIG = DefaultInteractionConfig()
 BOUNDARY_CONFIG = InteractionConfig({"bsite_cutoff": 6.2,
                                      "cache_cutoff": 10})
 
 NMR_METHODS = ["SOLID-STATE NMR", "SOLUTION NMR"]
 
 COV_SEARCH_RADIUS = 2.2
+METAL_COMPLEX_DIST = 2.8
 
 IFP_LENGTH = 4096
 
 ACCEPTED_MOL_OBJ_TYPES = ("rdkit", "openbabel")
 
 OPENBABEL = "obabel"
+ANTECHAMBER = "antechamber"
+DOCK6_PATH = "/opt/dock6"
+DOCK6 = f"{DOCK6_PATH}/bin/dock6"
 
 RECURSION_LIMIT = 600000
 
 ATOM_TYPES_COLOR = ColorPallete({
     "Aromatic": (255, 187, 204),
     "Acceptor": (158, 154, 200),
     "Donor": (17, 170, 119),
@@ -116,15 +120,16 @@
     "Displaced face-to-face pi-stacking": 36,
     "Displaced face-to-edge pi-stacking": 37,
     "Displaced face-to-slope pi-stacking": 38,
     "Single bond": 39,
     "Double bond": 40,
     "Triple bond": 41,
     "Aromatic bond": 42,
-    "Other bond": 43
+    "Other bond": 43,
+    "Metal coordination": 44,
 }
 
 INTERACTION_SHORT_NAMES = {
     "Proximal": "prox",
     "Hydrogen bond": "hbond",
     "Ionic": "ionic",
     "Salt bridge": "salt_bridge",
@@ -164,14 +169,15 @@
     "Displaced face-to-edge pi-stacking": "disp_face-to-edge_stack",
     "Displaced face-to-slope pi-stacking": "disp_face-to-slope_stack",
     "Single bond": "single-bond",
     "Double bond": "double-bond",
     "Triple bond": "triple-bond",
     "Aromatic bond": "aromatic-bond",
     "Other bond": "other-bond",
+    "Metal coordination": "metal-coord",
 }
 
 PYMOL_INTERACTION_COLOR = ColorPallete({
     "Proximal": "gray60",
     "Hydrogen bond": "tv_blue",
     "Water-bridged hydrogen bond": "lightblue",
     "Weak hydrogen bond": "lightteal",
@@ -211,14 +217,15 @@
     "Displaced face-to-edge pi-stacking": "tv_red",
     "Displaced face-to-slope pi-stacking": "tv_red",
     "Single bond": "black",
     "Double bond": "black",
     "Triple bond": "black",
     "Aromatic bond": "black",
     "Other bond": "black",
+    "Metal coordination": "olive"
 }, "white")
 
 PYMOL_INTERACTION_COLOR_AS_RGB = ColorPallete({
     "Proximal": (0.6, 0.6, 0.6),
     "Hydrogen bond": (0.3, 0.3, 1.0),
     "Water-bridged hydrogen bond": (0.75, 0.75, 1.0),
     "Weak hydrogen bond": (0.4, 0.7, 0.7),
@@ -258,11 +265,12 @@
     "Displaced face-to-edge pi-stacking": (1.0, 0.2, 0.2),
     "Displaced face-to-slope pi-stacking": (1.0, 0.2, 0.2),
     "Single bond": (0.0, 0.0, 0.0),
     "Double bond": (0.0, 0.0, 0.0),
     "Triple bond": (0.0, 0.0, 0.0),
     "Aromatic bond": (0.0, 0.0, 0.0),
     "Other bond": (0.0, 0.0, 0.0),
+    "Metal coordination": (0.0, 0.0, 0.0)
 }, (1.0, 1.0, 1.0))
 
 
 ARTIFACTS_LIST = ["ACE", "ACT", "BME", "CSD", "CSW", "EDO", "FMT", "GOL", "MSE", "NAG", "NO3", "PO4", "SGM", "SO4", "TPO"]
```

### Comparing `luna-0.12.2/luna/util/exceptions.py` & `luna-0.13.0/luna/util/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,22 @@
     pass
 
 
 class EntityLevelError(KeyError):
     pass
 
 
+class MissingAtomsError(ValueError):
+    pass
+
+
+class AtomsListError(ValueError):
+    pass
+
+
 class ChainNotFoundError(KeyError):
     pass
 
 
 class MoleculeNotFoundError(KeyError):
     pass
 
@@ -104,7 +112,11 @@
 
 class MoleculeObjectTypeError(TypeError):
     pass
 
 
 class MoleculeObjectError(RuntimeError):
     pass
+
+
+class LicenseNotFoundError(RuntimeError):
+    pass
```

### Comparing `luna-0.12.2/luna/util/file.py` & `luna-0.13.0/luna/util/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,19 @@
     """Detect the file format from pathname ``path``.
 
     Parameters
     ----------
     path : str
         The pathname.
     max_split : int or None
-        Specifies how many splits to do. The default value is None, which is "all occurrences".
+        Specifies how many splits to do. The default value is None,
+        which is "all occurrences".
     ignore_compression: bool, optional
-        Ignore compression format. The default value is False, which does not ignore compression format.
+        Ignore compression format. The default value is False,
+        which does not ignore compression format.
 
     Returns
     -------
     filename : str
         The file format.
     """
     if ignore_compression is True:
@@ -56,15 +58,16 @@
     """Detect the filename from pathname ``path``.
 
     Parameters
     ----------
     path : str
         The pathname.
     max_split : int or None
-        Specifies how many splits to do. The default value is None, which is "all occurrences".
+        Specifies how many splits to do. The default value is None,
+        which is "all occurrences".
 
     Returns
     -------
     filename : str
         The filename.
     """
     return generic_splitext(path, max_split)[0]
@@ -74,15 +77,16 @@
     """Split the pathname ``path`` into a pair (``filename``, ``ext``).
 
     Parameters
     ----------
     path : str
         The pathname.
     max_split : int or None
-        Specifies how many splits to do. The default value is None, which is "all occurrences".
+        Specifies how many splits to do. The default value is None,
+        which is "all occurrences".
 
     Returns
     -------
     filename : str
         The filename.
     ext: str
         The file extension.
@@ -102,37 +106,42 @@
         ext = tmp_ext + ext
         max_split -= 1
 
     return (filename, ext)
 
 
 def generate_json_file(json_data, output_file, indent=4, sort_keys=True):
-    """Serialize ``json_data`` to a JSON formatted string and save it at ``output_file``.
+    """Serialize ``json_data`` to a JSON formatted string and save it
+    at ``output_file``.
 
     Parameters
     ----------
     json_data : object
         The data to be serialized.
     output_file : str
         The output file where the serialized data will be saved.
     indent : int
-        If indent is a non-negative integer or string, then JSON array elements and object members
-        will be pretty-printed with that indent level. An indent level of 0, negative, or "" will only insert newlines.
-        None selects the most compact representation. Using a positive integer indent indents that many spaces per level.
-        If indent is a string (such as "\t"), that string is used to indent each level.
+        If indent is a non-negative integer or string, then JSON array
+        elements and object members will be pretty-printed with that indent
+        level. An indent level of 0, negative, or "" will only insert newlines.
+        None selects the most compact representation. Using a positive integer
+        indent indents that many spaces per level. If indent is a string
+        (such as "\t"), that string is used to indent each level.
         The default value is 4.
 
     sort_keys : bool
-        If ``sort_keys`` is True, the output of dictionaries will be sorted by key.
+        If ``sort_keys`` is True, the output of dictionaries will be
+        sorted by key.
     """
     try:
         import simplejson as json
         logger.warning("Module 'simplejson' imported.")
     except ImportError:
-        logger.warning("Module 'simplejson' not available. Built-in module 'json' will be imported.")
+        logger.warning("Module 'simplejson' not available. "
+                       "Built-in module 'json' will be imported.")
         import json
 
     try:
         with open(output_file, "w") as IN:
             json.dump(json_data, IN, indent=indent, sort_keys=sort_keys)
     except Exception as e:
         logger.exception(e)
@@ -213,41 +222,48 @@
     """Remove the directory given by the pathname ``path``.
 
     Parameters
     ----------
     path : str
         The pathname.
     only_empty_paths: bool, optional
-        If True, do not remove non-empty directories. The default value is False, which removes all directories.
+        If True, do not remove non-empty directories.
+        The default value is False, which removes all directories.
     """
     if isdir(path):
-        # Do nothing if the directory is not empty and if only empty paths must be removed.
+        # Do nothing if the directory is not empty and if only
+        # empty paths must be removed.
         if only_empty_paths and len(listdir(path)) != 0:
             return
 
         try:
             rmtree(path, ignore_errors=True)
         except OSError:
             raise
 
 
-def new_unique_filename(path, size=32, chars=string.ascii_uppercase + string.digits, retries=5):
+def new_unique_filename(path,
+                        size=32,
+                        chars=string.ascii_uppercase + string.digits,
+                        retries=5):
     """Generate a new unique random pathname.
 
     Parameters
     ----------
     path : str
         The target pathname.
     size : int, optional
         The size of the new filename. The default value is 32.
     chars : iterable, optional
-        A sequence of characters to choose from. The default value is 'ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789'.
+        A sequence of characters to choose from.
+        The default value is 'ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789'.
     retries : int, optional
-        The function will keep trying to generate a unique filename (not exist in the pathname ``path``)
-        until the maximum number of retries ``retries`` is reached.
+        The function will keep trying to generate a unique filename
+        (not exist in the pathname ``path``) until the maximum number
+        of retries ``retries`` is reached.
 
     Returns
     -------
     unique_pathname : str
         A new random unique pathname (path + random filename).
     """
     for r in range(retries):
@@ -267,15 +283,16 @@
         The filesystem type.
 
     Raises
     -------
     FileNotFoundError
         If the file or directory given by the pathname ``path`` does not exist.
     IsADirectoryError
-        If a file is provided but a directory is found instead at the pathname ``path``.
+        If a file is provided but a directory is found instead at the
+        pathname ``path``.
     NotADirectoryError
         If the filesystem given by the pathname ``path`` is not a directory.
     """
     if exists(path) is False:
         raise FileNotFoundError("File or directory '%s' does not exist" % path)
 
     if type == "file" and isfile(path) is False:
@@ -309,24 +326,26 @@
 
 def validate_file(path):
     """Validate ``path`` as a file."""
     validate_filesystem(path, "file")
 
 
 def pickle_data(data, output_file, compressed=True):
-    """Write the pickled representation of the object ``data`` to the file ``output_file``.
+    """Write the pickled representation of the object ``data`` to
+    the file ``output_file``.
 
     Parameters
     ----------
     data : object
         The object to be pickled.
     output_file : str
         The output file where the pickled representation will be saved.
     compressed : bool, optional
-        If True (the default), compress the pickled representation as a gzip file (.gz).
+        If True (the default), compress the pickled representation as
+        a gzip file (.gz).
 
     Raises
     -------
     FileNotCreated
         If the file could not be created.
     """
     open_func = open
@@ -335,35 +354,38 @@
         if output_file.endswith(".gz") is False:
             output_file += ".gz"
 
     try:
         with open_func(output_file, "wb") as OUT:
             pickle.dump(data, OUT, pickle.HIGHEST_PROTOCOL)
     except OSError as e:
-        raise FileNotCreated("File '%s' could not be created." % output_file) from e
+        raise FileNotCreated("File '%s' could not be created."
+                             % output_file) from e
     except Exception:
         raise
 
 
 def unpickle_data(input_file):
-    """Read the pickled representation of an object from the file ``input_file`` and
-    return the reconstituted object hierarchy specified therein.
-    ``input_file`` can be a gzip-compressed file.
+    """Read the pickled representation of an object from the file
+    ``input_file`` and return the reconstituted object hierarchy
+    specified therein. ``input_file`` can be a gzip-compressed file.
 
     Raises
     -------
     PKLNotReadError
         If the file could not be loaded.
     """
     try:
         # Try to decompress and unpickle the data first.
         with gzip.open(input_file, "rb") as IN:
             return pickle.load(IN)
     except Exception:
         pass
 
-    # If the decompression failed, let's try to unpickle the file directly. Maybe it is not a compressed file.
+    # If the decompression failed, let's try to unpickle the file directly.
+    # Maybe it is not a compressed file.
     try:
         with open(input_file, "rb") as IN:
             return pickle.load(IN)
     except OSError as e:
-        raise PKLNotReadError("File '%s' could not be loaded." % input_file) from e
+        raise PKLNotReadError("File '%s' could not be loaded."
+                              % input_file) from e
```

### Comparing `luna-0.12.2/luna/util/jobs.py` & `luna-0.13.0/luna/util/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,23 @@
 class Sentinel:
     """Custom sentinel to stop workers"""
     pass
 
 
 class ArgsGenerator:
     """Custom generator that implements __len__().
-       This class can be used in conjunction with :class:`~luna.util.progress_tracker.ProgressTracker` in cases
-       where the tasks are obtained from generators. Note that :class:`~luna.util.progress_tracker.ProgressTracker`
-       requires a pre-defined number of tasks to calculate the progress, therefore a standard generator cannot be
-       used directly as it does not implement __len__(). Then, with `ArgsGenerator`, one may take advantage of
-       generators and :class:`~luna.util.progress_tracker.ProgressTracker` by explicitly providing the number
-       of tasks that will be generated.
+       This class can be used in conjunction with
+       :class:`~luna.util.progress_tracker.ProgressTracker` in cases
+       where the tasks are obtained from generators. Note that
+       :class:`~luna.util.progress_tracker.ProgressTracker` requires a
+       pre-defined number of tasks to calculate the progress, therefore a
+       standard generator cannot be used directly as it does not implement
+       __len__(). Then, with `ArgsGenerator`, one may take advantage of
+       generators and :class:`~luna.util.progress_tracker.ProgressTracker`
+       by explicitly providing the number of tasks that will be generated.
 
        Parameters
        ----------
        generator : generator
            The tasks generator.
        nargs : int
            The number of tasks that will be generated.
@@ -44,28 +47,31 @@
     def __iter__(self):
         for d in self.generator:
             yield d
 
 
 class ParallelJobs:
 
-    """Executes a set of tasks in parallel (:py:class:`~multiprocessing.JoinableQueue`) or sequentially.
+    """Executes a set of tasks in parallel
+    (:py:class:`~multiprocessing.JoinableQueue`) or sequentially.
 
     Parameters
     ----------
     nproc : int or None
-       The number of CPUs to use. The default value is the ``maximum number of CPUs - 1``.
-       If ``nproc`` is None, 0, or 1, run the jobs sequentially. Otherwise, use the ``maximum number of CPUs - 1``.
+       The number of CPUs to use. The default value is the ``maximum number
+       of CPUs - 1``. If ``nproc`` is None, 0, or 1, run the jobs sequentially.
+       Otherwise, use the ``maximum number of CPUs - 1``.
 
     Attributes
     ----------
     nproc : int
         The number of CPUs to use.
     progress_tracker : ProgressTracker
-        A :class:`~luna.util.progress_tracker.ProgressTracker` object to track the tasks' progress.
+        A :class:`~luna.util.progress_tracker.ProgressTracker` object to track
+        the tasks' progress.
     """
 
     # TODO: add option to Threads/Multiprocessing
     def __init__(self, nproc=MAX_NPROCS):
 
         if nproc is not None:
             # Use 'MAX_NPROCS' if a non-integer has been provided.
@@ -118,20 +124,25 @@
             # Execute the provided function.
             output, exception, proc_time = self._exec_func(data, func)
 
             if output is not None and output_queue is not None:
                 output_queue.put((data, output))
 
             # Update progress tracker.
-            pd = ProgressData(input_data=data, output_data=output, exception=exception, proc_time=proc_time, func=func)
+            pd = ProgressData(input_data=data,
+                              output_data=output,
+                              exception=exception,
+                              proc_time=proc_time,
+                              func=func)
             progress_queue.put(pd)
 
             job_queue.task_done()
 
-    def _saver(self, output_queue, output_file, proc_func=None, output_header=None):
+    def _saver(self, output_queue, output_file,
+               proc_func=None, output_header=None):
 
         with open(output_file, "w") as OUT:
             if output_header is not None:
                 OUT.write(output_header.strip())
                 OUT.write("\n")
 
             while True:
@@ -167,52 +178,65 @@
     def _sequential(self, args, func, progress_queue):
         # Run jobs sequentially.
         for data in args:
             # Execute provided function.
             output, exception, proc_time = self._exec_func(data, func)
 
             # Save data.
-            pd = ProgressData(input_data=data, output_data=output, exception=exception, proc_time=proc_time)
+            pd = ProgressData(input_data=data,
+                              output_data=output,
+                              exception=exception,
+                              proc_time=proc_time)
 
             # Update progress tracker.
             progress_queue.put(pd)
 
-    def run_jobs(self, args, consumer_func, output_file=None, proc_output_func=None, output_header=None, job_name=None):
+    def run_jobs(self, args, consumer_func, output_file=None,
+                 proc_output_func=None, output_header=None, job_name=None):
         """
-        Run a set of tasks in parallel or sequentially according to the ``nproc``.
+        Run a set of tasks in parallel or sequentially according to the
+        ``nproc``.
 
         Parameters
         ----------
         args : iterable of iterables, `ArgsGenerator`
-            A sequence of arguments to be provided to the consumer function ``consumer_func``.
+            A sequence of arguments to be provided to the consumer function
+            ``consumer_func``.
         consumer_func : function
-            The function that will be executed for each set of arguments in ``args``.
+            The function that will be executed for each set of arguments in
+            ``args``.
         output_file : str, optional
             Save outputs to this file.
-            If ``proc_output_func`` is not provided, it tries to save a stringified version of each output data.
-            Otherwise, it executes ``proc_output_func`` first and its output will be printed to the output file instead.
-
-            Note: if ``proc_output_func`` is provided but not ``output_file``, a new random unique filename will
-            be generated and the file will be saved in the current directory.
+            If ``proc_output_func`` is not provided, it tries to save a
+            stringified version of each output data. Otherwise, it executes
+            ``proc_output_func`` first and its output will be printed to the
+            output file instead.
+
+            Note: if ``proc_output_func`` is provided but not ``output_file``,
+            a new random unique filename will be generated and the file will be
+            saved in the current directory.
         proc_output_func : function, optional
-            Post-processing function that is executed for each output data produced by ``consumer_func``.
+            Post-processing function that is executed for each output data
+            produced by ``consumer_func``.
         output_header : str, optional
             A header for the output file.
         job_name : str, optional
             A name to identify the job.
 
         Returns
         -------
          : :class:`~luna.util.progress_tracker.ProgressResult`
         """
         if proc_output_func is not None and output_file is None:
             output_file = new_unique_filename(".") + ".output"
-            logger.warning("No output file was defined. So, it will try to save results at '%s'." % output_file)
+            logger.warning("No output file was defined. So, it will try to "
+                           "save results at '%s'." % output_file)
         elif output_file is not None:
-            logger.warning("The output file '%s' was defined. So, it will try to save results at it." % output_file)
+            logger.warning("The output file '%s' was defined. So, it will "
+                           "try to save results at it." % output_file)
 
         # Queue for progress tracker.
         progress_queue = mp.JoinableQueue(maxsize=1)
 
         # Progress tracker
         self.progress_tracker = ProgressTracker(len(args), progress_queue,
                                                 job_name)
```

### Comparing `luna-0.12.2/luna/util/logging.py` & `luna-0.13.0/luna/util/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,32 +48,33 @@
                     f_in.close()
             if os.path.exists(self.baseFilename):
                 os.remove(self.baseFilename)
         self.mode = 'w'
         self.stream = self._open()
 
 
-def new_logging_file(filename, logging_level=logging.INFO, 
+def new_logging_file(filename, logging_level=logging.INFO,
                      logger_name=None, propagate=True,
                      log_format=None, mode='a'):
     # Set the LOG file at the working path
     fh = CompressedRotatingFileHandler(filename, mode, 5 * 1024 * 1024, 20)
     file_format = log_format or FILE_FORMAT
     file_formatter = logging.Formatter(file_format, '%Y-%m-%d %H:%M:%S')
     fh.setFormatter(file_formatter)
     fh.setLevel(logging.DEBUG)
 
     ch = logging.StreamHandler()
     console_format = log_format or CONSOLE_FORMAT
-    console_formatter = colorlog.ColoredFormatter(console_format, '%Y-%m-%d %H:%M:%S',
-                                                  log_colors={'DEBUG': 'cyan',
-                                                              'INFO': 'green',
-                                                              'WARNING': 'yellow',
-                                                              'ERROR': 'red',
-                                                              'CRITICAL': 'bold_red'})
+    console_formatter = \
+        colorlog.ColoredFormatter(console_format, '%Y-%m-%d %H:%M:%S',
+                                  log_colors={'DEBUG': 'cyan',
+                                              'INFO': 'green',
+                                              'WARNING': 'yellow',
+                                              'ERROR': 'red',
+                                              'CRITICAL': 'bold_red'})
     ch.setFormatter(console_formatter)
     ch.setLevel(logging_level)
 
     logger = logging.getLogger(logger_name)
 
     if logger_name is not None:
         logger.propagate = propagate
```

### Comparing `luna-0.12.2/luna/util/math.py` & `luna-0.13.0/luna/util/math.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/util/multiprocessing_logging.py` & `luna-0.13.0/luna/util/multiprocessing_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 
         self.setLevel(self.sub_handler.level)
         self.setFormatter(self.sub_handler.formatter)
 
         self.queue = multiprocessing.Queue(-1)
         self._is_closed = False
         # The thread handles receiving records asynchronously.
-        self._receive_thread = threading.Thread(target=self._receive, name=name)
+        self._receive_thread = threading.Thread(target=self._receive,
+                                                name=name)
         self._receive_thread.daemon = True
         self._receive_thread.start()
 
     def setFormatter(self, fmt):
         super(MultiProcessingHandler, self).setFormatter(fmt)
         self.sub_handler.setFormatter(fmt)
 
@@ -64,15 +65,15 @@
                 self.sub_handler.emit(record)
             except (KeyboardInterrupt, SystemExit):
                 raise
             except EOFError:
                 break
             except queue.Empty:
                 pass  # This periodically checks if the logger is closed.
-            except:
+            except Exception:
                 traceback.print_exc(file=sys.stderr)
 
         self.queue.close()
         self.queue.join_thread()
 
     def _send(self, s):
         self.queue.put_nowait(s)
@@ -93,15 +94,15 @@
 
     def emit(self, record):
         try:
             s = self._format_record(record)
             self._send(s)
         except (KeyboardInterrupt, SystemExit):
             raise
-        except:
+        except Exception:
             self.handleError(record)
 
     def close(self):
         if not self._is_closed:
             self._is_closed = True
             self._receive_thread.join(5.0)  # Waits for receive queue to empty.
```

### Comparing `luna-0.12.2/luna/util/progress_tracker.py` & `luna-0.13.0/luna/util/progress_tracker.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,33 +22,34 @@
         The input data of the executed task.
     proc_time : float
         How long a task took to be executed.
     output_data : any, optional
         The output data produced by a given task.
         The data type is the same as the executed function's return.
     exception : :py:class:`Exception`, optional
-        If an exception was raised, then ``exception`` stores an Exception object.
-        Otherwise, ``exception`` will be set to None.
+        If an exception was raised, then ``exception`` stores an
+        Exception object. Otherwise, ``exception`` will be set to None.
     func : function, optional
         The executed function for reference.
     """
 
-    def __init__(self, input_data, proc_time, output_data=None, exception=None, func=None):
+    def __init__(self, input_data, proc_time,
+                 output_data=None, exception=None, func=None):
 
         self.input_data = input_data
         self.output_data = output_data
         self.proc_time = proc_time
         self.exception = exception
         self.func = func
 
 
 class ProgressResult:
     """
-    Custom iterable class to store `ProgressData` objects as they are produced during the
-    execution of a set of tasks.
+    Custom iterable class to store `ProgressData` objects as they are produced
+    during the execution of a set of tasks.
 
     This class implements append() and __iter__() by default.
 
     Parameters
     ----------
     results : list, optional
         A pre-populated list of `ProgressData` objects.
@@ -57,42 +58,51 @@
     ----------
     results : list
         The list of `ProgressData` objects.
     """
 
     def __init__(self, results=None):
         if results and not isinstance(results, list):
-            raise TypeError("A list was expected but a different data type was provided.")
+            raise TypeError("A list was expected but a different data type "
+                            "was provided.")
         self.results = results or []
 
     @property
     def inputs(self):
-        """list: Inputs from each `ProgressData` object stored in ``results``."""
+        """list: Inputs from each `ProgressData` object stored in \
+        ``results``."""
         try:
             return [r.input_data for r in self.results]
         except AttributeError:
-            raise TypeError("An invalid object was found in 'results'. Only ProgressData objects are valid.")
+            raise TypeError("An invalid object was found in 'results'. "
+                            "Only ProgressData objects are valid.")
 
     @property
     def outputs(self):
-        """list of tuple: Outputs from each `ProgressData` object stored in ``results``.
-        Each tuple contains the input and the output produced for that input."""
+        """list of tuple: Outputs from each `ProgressData` object stored in
+        ``results``. Each tuple contains the input and the output produced for
+        that input."""
         try:
             return [(r.input_data, r.output_data) for r in self.results]
         except AttributeError:
-            raise TypeError("An invalid object was found in 'results'. Only ProgressData objects are valid.")
+            raise TypeError("An invalid object was found in 'results'. "
+                            "Only ProgressData objects are valid.")
 
     @property
     def errors(self):
-        """list of tuple: Errors from each `ProgressData` object stored in ``results``.
-        Each tuple contains the input and the exception raised during the execution of a task with that input."""
+        """list of tuple: Errors from each `ProgressData` object stored in \
+        ``results``.
+        Each tuple contains the input and the exception raised during the
+        execution of a task with that input."""
         try:
-            return [(r.input_data, r.exception) for r in self.results if r.exception is not None]
+            return [(r.input_data, r.exception) for r in self.results
+                    if r.exception is not None]
         except AttributeError:
-            raise TypeError("An invalid object was found in 'results'. Only ProgressData objects are valid.")
+            raise TypeError("An invalid object was found in 'results'. "
+                            "Only ProgressData objects are valid.")
 
     def append(self, r):
         """Add a new `ProgressData` object to ``results``"""
         if not isinstance(r, ProgressData):
             raise TypeError("Only ProgressData objects are valid.")
         self.results.append(r)
 
@@ -152,37 +162,46 @@
         self._end_time = None
 
     def _show_progress_bar(self, p, perc):
         task_name = ""
         if self.task_name:
             task_name = " - %s" % self.task_name
 
-        msg = '%s%% [%s] %d/%d [Avg: %.2fs/task; Errors: %d]%s.' % (int(perc), ("\u25A0" * int(perc / 2)).ljust(50, ' '),
-                                                                    p, self.ntasks, self.avg_running_time, self.nerrors, task_name)
+        msg = ('%s%% [%s] %d/%d [Avg: %.2fs/task; Errors: %d]%s.'
+               % (int(perc), ("\u25A0" * int(perc / 2)).ljust(50, ' '),
+                  p, self.ntasks, self.avg_running_time,
+                  self.nerrors, task_name))
 
         format_str = '\r[%s]    %s%s %s%s  %s'
-        progress_str = format_str % (time.strftime('%Y-%m-%d %H:%M:%S'), parse_colors("purple"),
-                                     "PROGRESS".ljust(10, " "), escape_codes["reset"], "".rjust(26, " "), msg)
+        progress_str = \
+            (format_str % (time.strftime('%Y-%m-%d %H:%M:%S'),
+             parse_colors("purple"),
+             "PROGRESS".ljust(10, " "),
+             escape_codes["reset"],
+             "".rjust(26, " "),
+             msg))
 
         sys.stdout.write(progress_str)
         sys.stdout.flush()
 
     def _print_progress(self, e, q):
         """Updates a progress bar on stdout anytime progress is made"""
 
         while True:
             while not q.full():
-                # Stops the loop if function end() is called before the queue gets full.
+                # Stops the loop if function end() is called before the queue
+                # gets full.
                 if e.is_set():
                     break
                 # wait for more progress to be made
                 time.sleep(0.1)
 
             # If our event is set and there is any progress in the queue,
-            # break out of the infinite loop and prepare to terminate this thread
+            # break out of the infinite loop and prepare to terminate this
+            # thread
             if e.is_set() and q.full() is False:
                 break
 
             # get the current progress data.
             progress_data = q.get()
 
             if progress_data is not None:
@@ -214,15 +233,17 @@
             return round(self._end_time - self._start_time, 2)
         return None
 
     @property
     def avg_running_time(self):
         """float: Average running time."""
         if self._running_times:
-            return round(sum(self._running_times) / len(self._running_times), 2)
+            total = sum(self._running_times)
+            count = len(self._running_times)
+            return round(total / count, 2)
         else:
             return 0
 
     def start(self):
         """ Start the progress tracker. """
         self._start_time = round(time.time(), 2)
         self._progress_bar.start()
```

### Comparing `luna-0.12.2/luna/util/stringcase.py` & `luna-0.13.0/luna/util/stringcase.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/version.py` & `luna-0.13.0/luna/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
        - MINOR stands for updates that "break" the compatibility
             between pharmacophoric perception, interactions,
             and interaction fingerprints;
 
        - PATCH stands for backward compatible bug fixes.
 """
-version_info = (0, 12, 2)
+version_info = (0, 13, 0)
 version = '.'.join(str(c) for c in version_info)
 __version__ = version
 
 
 def has_version_compatibility(v):
     version_to_check = v
     if isinstance(v, str):
```

### Comparing `luna-0.12.2/luna/wrappers/base.py` & `luna-0.13.0/luna/wrappers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from enum import Enum, unique
 from rdkit.Chem import Atom as RDAtom
 from rdkit.Chem import Mol as RDMol
 from rdkit.Chem import Bond as RDBond
 from rdkit.Chem import BondType as RDBondType
 from rdkit.Chem import (MolFromSmiles, MolToSmiles, MolToPDBBlock,
-                        MolToMolBlock, GetPeriodicTable)
+                        MolToMolBlock, GetPeriodicTable, GetFormalCharge)
+from rdkit.Chem import rdFMCS
+
 from openbabel import openbabel as ob
 from openbabel.pybel import Molecule as PybelMol
-from openbabel.pybel import readstring
+from openbabel.pybel import readstring, readfile
 
-from luna.wrappers.rdkit import new_mol_from_block
+from luna.wrappers.rdkit import new_mol_from_block, read_mol_from_file
+from luna.util.math import euclidean_distance
 from luna.util.exceptions import (AtomObjectTypeError, BondObjectTypeError,
                                   IllegalArgumentError, MoleculeObjectError,
                                   MoleculeObjectTypeError)
 
 import logging
-
 logger = logging.getLogger()
 
 
 @unique
 class BondType(Enum):
     """An enumeration of bond types available at RDKit."""
 
@@ -60,76 +62,92 @@
 
 class AtomWrapper:
     """This class provides util functions to access atomic properties and
     other information from RDKit and Open Babel objects.
 
     Parameters
     ----------
-    atm_obj : :class:`AtomWrapper`, :class:`rdkit.Chem.rdchem.Atom`, or :class:`openbabel.OBAtom`
+    atm_obj : :class:`AtomWrapper`, :class:`rdkit.Chem.rdchem.Atom`, \
+                    or :class:`openbabel.OBAtom`
         An atom to wrap.
-    mol_obj : `MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, :class:`openbabel.pybel.Molecule`, or None
-        The molecule that contains the atom ``atom``. If None, the molecule is recovered directly from the atom object.
+    mol_obj : `MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, \
+                    :class:`openbabel.pybel.Molecule`, or None
+        The molecule that contains the atom ``atom``. If None, the molecule is
+        recovered directly from the atom object.
 
     Raises
     ------
     AtomObjectTypeError
         If the atom object is not an instance
-            of `MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`.
+            of `MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or
+            :class:`openbabel.pybel.Molecule`.
     """
 
     def __init__(self, atm_obj, mol_obj=None):
         if isinstance(atm_obj, self.__class__):
             atm_obj = atm_obj.unwrap()
 
-        if not isinstance(atm_obj, RDAtom) and not isinstance(atm_obj, ob.OBAtom):
-            logger.exception("Objects of type '%s' are not currently accepted." % atm_obj.__class__)
-            raise AtomObjectTypeError("Objects of type '%s' are not currently accepted." % atm_obj.__class__)
+        if (not isinstance(atm_obj, RDAtom)
+                and not isinstance(atm_obj, ob.OBAtom)):
+            error_msg = ("Objects of type '%s' are not currently accepted."
+                         % atm_obj.__class__)
+            logger.exception(error_msg)
+            raise AtomObjectTypeError(error_msg)
 
         self._atm_obj = atm_obj
         self._parent = None
 
         if mol_obj is None:
             mol_obj = self.get_parent()
         self._parent = MolWrapper(mol_obj)
 
     @property
     def atm_obj(self):
-        """:class:`rdkit.Chem.rdchem.Atom` or :class:`openbabel.OBAtom`: The wrapped atom object."""
+        """:class:`rdkit.Chem.rdchem.Atom` or :class:`openbabel.OBAtom`: \
+                The wrapped atom object."""
         return self._atm_obj
 
     @atm_obj.setter
     def atm_obj(self, atm_obj):
-        if not isinstance(atm_obj, RDAtom) and not isinstance(atm_obj, ob.OBAtom):
-            logger.exception("Objects of type '%s' are not currently accepted." % atm_obj.__class__)
-            raise AtomObjectTypeError("Objects of type '%s' are not currently accepted." % atm_obj.__class__)
+        if (not isinstance(atm_obj, RDAtom)
+                and not isinstance(atm_obj, ob.OBAtom)):
+            error_msg = ("Objects of type '%s' are not currently accepted."
+                         % atm_obj.__class__)
+            logger.exception(error_msg)
+            raise AtomObjectTypeError(error_msg)
         else:
             self._atm_obj = atm_obj
 
     @property
     def parent(self):
-        """`MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`: The molecule that contains this atom."""
+        """`MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, \
+                or :class:`openbabel.pybel.Molecule`: \
+            The molecule that contains this atom."""
         return self.get_parent()
 
     @parent.setter
     def parent(self, mol_obj):
         self._parent = MolWrapper(mol_obj)
 
     def get_idx(self):
         """Get this atom's internal index within a molecule.
 
         Returns
         -------
          : int
         """
-        return self._atm_obj.GetIdx()  # Both RDKit and Open Babel have the same function name.
+
+        # Both RDKit and Open Babel have the same function name.
+        return self._atm_obj.GetIdx()
 
     def get_id(self):
         """Get this atom's unique id.
 
-        When using RDKit, :py:meth:`get_id` and :py:meth:`get_idx` returns the same value.
+        When using RDKit, :py:meth:`get_id` and :py:meth:`get_idx` returns
+        the same value.
 
         Returns
         -------
          : int
         """
         if self.is_rdkit_obj():
             return self._atm_obj.GetIdx()
@@ -138,19 +156,21 @@
 
     def get_parent(self, wrapped=True):
         """Get the molecule that contains this atom.
 
         Parameters
         ----------
         wrapped : bool
-            If True, wrap the molecule with :class:`~luna.wrappers.base.MolWrapper`.
+            If True, wrap the molecule with
+            :class:`~luna.wrappers.base.MolWrapper`.
 
         Returns
         -------
-         : `MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`
+         : `MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, \
+                            or :class:`openbabel.pybel.Molecule`
         """
         if self._parent is None:
             if self.is_rdkit_obj():
                 mol_obj = self._atm_obj.GetOwningMol()
             elif self.is_openbabel_obj():
                 mol_obj = self._atm_obj.GetParent()
 
@@ -163,15 +183,15 @@
     def get_atomic_num(self):
         """Get this atom's atomic number.
 
         Returns
         -------
          : int
         """
-        
+
         # Both RDKit and Open Babel have the same function name.
         return self._atm_obj.GetAtomicNum()
 
     def get_symbol(self):
         """Get the element symbol of this atom.
 
         Returns
@@ -186,15 +206,17 @@
     def get_charge(self):
         """Get this atom's formal charge.
 
         Returns
         -------
          : int
         """
-        return self._atm_obj.GetFormalCharge()  # Both RDKit and Open Babel have the same function name.
+
+        # Both RDKit and Open Babel have the same function name.
+        return self._atm_obj.GetFormalCharge()
 
     def get_isotope(self):
         """Get this atom's isotope number.
 
         Returns
         -------
          : int
@@ -213,15 +235,16 @@
         """
         if self.is_rdkit_obj():
             return self._atm_obj.GetMass()
         elif self.is_openbabel_obj():
             return self._atm_obj.GetExactMass()
 
     def get_atomic_mass(self):
-        """Get this atom's atomic mass given by standard IUPAC average molar mass.
+        """Get this atom's atomic mass given by standard IUPAC average
+        molar mass.
 
         Returns
         -------
          : float
         """
         if self.is_rdkit_obj():
             return GetPeriodicTable().GetAtomicWeight(self.get_atomic_num())
@@ -237,29 +260,32 @@
             If True, count only heavy atoms.
 
         Returns
         -------
          : int
         """
 
-        # Subtract the number of hydrogens from the degree if only heavy atoms must be considered.
+        # Subtract the number of hydrogens from the degree if only heavy atoms
+        # must be considered.
         penalty = 0 if only_heavy_atoms is False else self.get_h_count()
         return self.get_degree() - penalty
 
     def get_neighbors(self, wrapped=True):
         """Get all atoms that are bound to this atom.
 
         Parameters
         ----------
         wrapped : bool
-            If True, wrap each atom with :class:`~luna.wrappers.base.AtomWrapper`.
+            If True, wrap each atom with
+            :class:`~luna.wrappers.base.AtomWrapper`.
 
         Returns
         -------
-         : iterable of `AtomWrapper`, :py:class:`rdkit.Chem.rdchem.Atom`, or :class:`openbabel.OBAtom`
+         : iterable of `AtomWrapper`, :py:class:`rdkit.Chem.rdchem.Atom`, \
+                or :class:`openbabel.OBAtom`
         """
         atoms = []
         if self.is_rdkit_obj():
             atoms = self._atm_obj.GetNeighbors()
         elif self.is_openbabel_obj():
             atoms = ob.OBAtomAtomIter(self._atm_obj)
 
@@ -278,83 +304,93 @@
             return self._atm_obj.GetTotalDegree()
         elif self.is_openbabel_obj():
             return self._atm_obj.GetTotalDegree()
 
     def get_valence(self):
         """Get this atom's total valence (implicit and explicit)."""
         if self.is_rdkit_obj():
-            return self._atm_obj.GetExplicitValence() + self._atm_obj.GetImplicitValence()
+            valence = (self._atm_obj.GetExplicitValence()
+                       + self._atm_obj.GetImplicitValence())
+            return valence
         elif self.is_openbabel_obj():
             return self._atm_obj.GetTotalValence()
 
-            bonds = [b.GetBondOrder() for b in ob.OBAtomBondIter(self._atm_obj)]
-            return sum(bonds) + self._atm_obj.ImplicitHydrogenCount()
-
     def get_h_count(self):
-        """Get the total number of hydrogens (implicit and explicit) bound to this atom.
+        """Get the total number of hydrogens (implicit and explicit) bound to
+        this atom.
 
         Returns
         -------
          : int
         """
         if self.is_rdkit_obj():
             return self._atm_obj.GetTotalNumHs(includeNeighbors=True)
         elif self.is_openbabel_obj():
-            return self._atm_obj.GetImplicitHCount() + self._atm_obj.ExplicitHydrogenCount()
+            h_count = (self._atm_obj.GetImplicitHCount()
+                       + self._atm_obj.ExplicitHydrogenCount())
+            return h_count
 
     def get_bonds(self, wrapped=True):
         """Get this atom’s bonds.
 
         Parameters
         ----------
         wrapped : bool
-            If True, wrap each bond with :class:`~luna.wrappers.base.BondWrapper`.
+            If True, wrap each bond with
+            :class:`~luna.wrappers.base.BondWrapper`.
 
         Returns
         -------
-         : iterable of `BondWrapper`, :class:`rdkit.Chem.rdchem.Bond`, or :class:`openbabel.OBBond`
+         : iterable of `BondWrapper`, :class:`rdkit.Chem.rdchem.Bond`,
+            or :class:`openbabel.OBBond`
         """
         bonds = []
         if self.is_rdkit_obj():
             bonds = self._atm_obj.GetBonds()
         elif self.is_openbabel_obj():
             bonds = ob.OBAtomBondIter(self._atm_obj)
 
         if bonds and wrapped:
             return [BondWrapper(bond) for bond in bonds]
         return bonds
 
+    def get_coord(self):
+        return self.parent.get_atom_coord_by_id(self.get_id())
+
     def get_atomic_invariants(self):
         """Get the atomic invariants of this atom.
 
-        Atomic invariants are derived from ECFP [1]_ and E3FP [2]_ and consists of seven fields:
+        Atomic invariants are derived from ECFP [1]_ and E3FP [2]_ and
+        consists of seven fields:
 
-            * Number of heavy atoms;
+            * Number of neighboring heavy atoms;
             * Valence - Number of hydrogens;
             * Atomic number;
             * Isotope number;
             * Formal charge;
             * Number of hydrogens;
             * If the atom belongs to a ring or not.
 
         Returns
         -------
          : list
         """
-        return [self.get_neighbors_number(only_heavy_atoms=True),       # Number of heavy atoms
-                (self.get_valence() - self.get_h_count()),              # Valence - Num. Hs
-                self.get_atomic_num(),                                  # Atomic number
-                self.get_isotope(),                                     # Isotope number
-                self.get_charge(),                                      # Formal charge
-                self.get_h_count(),                                     # Num. Hs
-                int(self.is_in_ring())]                                 # If the atom belongs to a ring or not
+        return [self.get_neighbors_number(only_heavy_atoms=True),
+                (self.get_valence() - self.get_h_count()),
+                self.get_atomic_num(),
+                self.get_isotope(),
+                self.get_charge(),
+                self.get_h_count(),
+                int(self.is_in_ring())]
 
     def is_in_ring(self):
         """Check if this atom is in a ring."""
-        return self._atm_obj.IsInRing()  # Both RDKit and Open Babel have the same function name.
+
+        # Both RDKit and Open Babel have the same function name.
+        return self._atm_obj.IsInRing()
 
     def is_aromatic(self):
         """Check if this atom is aromatic."""
 
         if self.is_rdkit_obj():
             return self._atm_obj.GetIsAromatic()
         elif self.is_openbabel_obj():
@@ -369,43 +405,51 @@
 
         Raises
         ------
         IllegalArgumentError
             If the informed bond type is not an instance of `BondType`.
         """
         if isinstance(bond_type, BondType):
-            return any([bond_obj.get_bond_type() == bond_type for bond_obj in self.get_bonds()])
+            return any([bond_obj.get_bond_type() == bond_type
+                        for bond_obj in self.get_bonds()])
         else:
-            raise IllegalArgumentError("The informed bond type must be an instance of '%s'." % BondType)
+            msg = ("The informed bond type must be an instance of '%s'."
+                   % BondType)
+            raise IllegalArgumentError(msg)
 
     def has_only_bond_type(self, bond_type):
         """Check if this atom has only bonds of type ``bond_type``.
 
         Parameters
         ----------
         bond_type : `BondType`
 
         Raises
         ------
         IllegalArgumentError
             If the informed bond type is not an instance of `BondType`.
         """
         if isinstance(bond_type, BondType):
-            return all([bond_obj.get_bond_type() == bond_type for bond_obj in self.get_bonds()])
+            return all([bond_obj.get_bond_type() == bond_type
+                        for bond_obj in self.get_bonds()])
         else:
-            raise IllegalArgumentError("The informed bond type must be an instance of '%s'." % BondType)
+            msg = ("The informed bond type must be an instance of '%s'."
+                   % BondType)
+            raise IllegalArgumentError(msg)
 
     def set_charge(self, charge):
         """Set the formal charge of this atom.
 
         Parameters
         ----------
         charge : int
         """
-        self._atm_obj.SetFormalCharge(charge)  # Both RDKit and Open Babel have the same function name.
+
+        # Both RDKit and Open Babel have the same function name.
+        self._atm_obj.SetFormalCharge(charge)
 
     def set_as_aromatic(self, is_aromatic):
         """Set whether this atom is aromatic or not.
 
         Parameters
         ----------
         is_aromatic : bool
@@ -420,63 +464,73 @@
 
         Parameters
         ----------
         in_ring : bool
         """
         if self.is_rdkit_obj():
             # TODO
-            raise NotImplementedError("Currently, there is no function in RDKit to define if an atom belongs to a ring or not. "
-                                      "Please, use Open Babel instead.")
+            error_msg = ("Currently, there is no function in RDKit to define "
+                         "if an atom belongs to a ring or not. Please, use "
+                         "Open Babel instead.")
+            raise NotImplementedError(error_msg)
 
         elif self.is_openbabel_obj():
             self._atm_obj.SetInRing(in_ring)
 
     def matches_smarts(self, smarts):
-        """Check if this atom matches the substructure through a SMARTS substructure search.
+        """Check if this atom matches the substructure through a SMARTS
+        substructure search.
 
-        **Note:** currently, this function only works with molecules read with Open Babel.
+        **Note:** currently, this function only works with molecules
+        read with Open Babel.
 
         Parameters
         ----------
         smarts : str
             A substructure defined as SMARTS.
 
         Returns
         -------
          : bool or None
-            Whether matches occurred. Return None if the molecule was read with RDKit.
+            Whether matches occurred. Return None if the molecule was read
+            with RDKit.
 
         Examples
         --------
         First, let's read a molecule (glutamine) using Open Babel.
 
         >>> from luna.wrappers.base import MolWrapper
-        >>> mol_obj = MolWrapper.from_smiles("N[C@@H](CCC(N)=O)C(O)=O", mol_obj_type="openbabel")
+        >>> mol_obj = MolWrapper.from_smiles("N[C@@H](CCC(N)=O)C(O)=O",
+        ...                                  mol_obj_type="openbabel")
 
-        Now, we'll loop over the list of atoms in the glutamine and check which atom is the amide's carbon.
-        To do so, we can call the function :py:meth:`MolWrapper.get_atoms`, which, by default,
-        returns `AtomWrapper` objects and then call :py:meth:`matches_smarts`.
+        Now, we'll loop over the list of atoms in the glutamine and check which
+        atom is the amide's carbon. To do so, we can call the function
+        :py:meth:`MolWrapper.get_atoms`, which, by default, returns
+        `AtomWrapper` objects and then call :py:meth:`matches_smarts`.
 
         >>> for atm in mol_obj.get_atoms():
-        >>>     print("%d\t%s\t%s" % (atm.get_idx(), atm.get_symbol(), atm.matches_smarts("C(N)(C)=O")))
+        >>>     print("%d\t%s\t%s" % (atm.get_idx(),
+        ...                           atm.get_symbol(),
+        ...                           atm.matches_smarts("C(N)(C)=O")))
         1   N   False
         2   C   False
         3   C   False
         4   C   False
         5   C   True
         6   N   False
         7   O   False
         8   C   False
         9   O   False
         10  O   False
         """
         if self.is_rdkit_obj():
             # TODO: Implement
-            raise NotImplementedError("Currently, matches_smarts() does not support RDKit objects. "
-                                      "Please, use Open Babel objects instead.")
+            error_msg = ("Currently, matches_smarts() does not support RDKit "
+                         "objects. Please, use Open Babel objects instead.")
+            raise NotImplementedError(error_msg)
 
         elif self.is_openbabel_obj():
             ob_smart = ob.OBSmartsPattern()
             ob_smart.Init(smarts)
 
             if ob_smart.Match(self.parent):
                 for match in ob_smart.GetMapList():
@@ -504,67 +558,84 @@
         if isinstance(self._atm_obj, ob.OBAtom):
             return True
         return False
 
     def __getattr__(self, attr):
         return getattr(self._atm_obj, attr)
 
+    def __sub__(self, other):
+        if not isinstance(other, AtomWrapper):
+            other = AtomWrapper(other)
+
+        return euclidean_distance(self.get_coords(), other.get_coords())
+
 
 class BondWrapper:
     """This class provides util functions to access bond properties and
     other information from RDKit and Open Babel objects.
 
     Parameters
     ----------
-    bond_obj : `BondWrapper`, :py:class:`rdkit.Chem.rdchem.Bond`, or :py:class:`openbabel.OBBond`
+    bond_obj : `BondWrapper`, :py:class:`rdkit.Chem.rdchem.Bond`, \
+            or :py:class:`openbabel.OBBond`
         A bond to wrap.
 
     Raises
     ------
     BondObjectTypeError
         If the bond object is not an instance
-            of `BondWrapper`, :class:`rdkit.Chem.rdchem.Bond`, or :class:`openbabel.pybel.OBBond`.
+            of `BondWrapper`, :class:`rdkit.Chem.rdchem.Bond`, \
+                or :class:`openbabel.pybel.OBBond`.
     """
 
     def __init__(self, bond_obj):
         if isinstance(bond_obj, self.__class__):
             bond_obj = bond_obj.unwrap()
 
-        if not isinstance(bond_obj, RDBond) and not isinstance(bond_obj, ob.OBBond):
-            logger.exception("Objects of type '%s' are not currently accepted." % bond_obj.__class__)
-            raise BondObjectTypeError("Objects of type '%s' are not currently accepted." % bond_obj.__class__)
+        if (not isinstance(bond_obj, RDBond)
+                and not isinstance(bond_obj, ob.OBBond)):
+            error_msg = ("Objects of type '%s' are not currently accepted."
+                         % bond_obj.__class__)
+            logger.exception(error_msg)
+            raise BondObjectTypeError(error_msg)
 
         self._bond_obj = bond_obj
 
     @property
     def bond_obj(self):
-        """:class:`rdkit.Chem.rdchem.Bond` or :class:`openbabel.OBBond`: The wrapped bond object."""
+        """:class:`rdkit.Chem.rdchem.Bond` or :class:`openbabel.OBBond`: \
+                The wrapped bond object."""
         return self._bond_obj
 
     @bond_obj.setter
     def bond_obj(self, bond_obj):
-        if not isinstance(bond_obj, RDBond) and not isinstance(bond_obj, ob.OBBond):
-            logger.exception("Objects of type '%s' are not currently accepted." % bond_obj.__class__)
-            raise AtomObjectTypeError("Objects of type '%s' are not currently accepted." % bond_obj.__class__)
+        if (not isinstance(bond_obj, RDBond)
+                and not isinstance(bond_obj, ob.OBBond)):
+            error_msg = ("Objects of type '%s' are not currently accepted."
+                         % bond_obj.__class__)
+            logger.exception(error_msg)
+            raise AtomObjectTypeError(error_msg)
         else:
             self._bond_obj = bond_obj
 
     def get_partner_atom(self, atm, wrapped=True):
         """Get the partner atom that forms this bond with ``atm``.
 
         Parameters
         ----------
-        atm : `AtomWrapper`, :py:class:`rdkit.Chem.rdchem.Atom`, or :class:`openbabel.OBAtom`
+        atm : `AtomWrapper`, :py:class:`rdkit.Chem.rdchem.Atom`, \
+                    or :class:`openbabel.OBAtom`
             Get the partner of this atom.
         wrapped : bool
             If True, wrap the partner atom with `AtomWrapper`.
 
         Returns
         -------
-         : `AtomWrapper`, :py:class:`rdkit.Chem.rdchem.Atom`, or :class:`openbabel.OBAtom`
+         : `AtomWrapper`, :py:class:`rdkit.Chem.rdchem.Atom`, \
+                or :class:`openbabel.OBAtom`
         """
         if isinstance(atm, AtomWrapper):
             atm = atm.unwrap()
 
         partner = None
         if atm == self._bond_obj.GetBeginAtom():
             partner = self._bond_obj.GetEndAtom()
@@ -581,15 +652,16 @@
         Parameters
         ----------
         wrapped : bool
             If True, wrap the atom with `AtomWrapper`.
 
         Returns
         -------
-         : `AtomWrapper`, :py:class:`rdkit.Chem.rdchem.Atom`, or :class:`openbabel.OBAtom`
+         : `AtomWrapper`, :py:class:`rdkit.Chem.rdchem.Atom`, \
+                or :class:`openbabel.OBAtom`
         """
 
         # Both RDKit and Open Babel have the same function name.
         if wrapped:
             return AtomWrapper(self._bond_obj.GetBeginAtom())
         return self._bond_obj.GetBeginAtom()
 
@@ -599,15 +671,16 @@
         Parameters
         ----------
         wrapped : bool
             If True, wrap the atom with `AtomWrapper`.
 
         Returns
         -------
-         : `AtomWrapper`, :py:class:`rdkit.Chem.rdchem.Atom`, or :class:`openbabel.OBAtom`
+         : `AtomWrapper`, :py:class:`rdkit.Chem.rdchem.Atom`, \
+                or :class:`openbabel.OBAtom`
         """
 
         # Both RDKit and Open Babel have the same function name.
         if wrapped:
             return AtomWrapper(self._bond_obj.GetEndAtom())
         return self._bond_obj.GetEndAtom()
 
@@ -617,14 +690,21 @@
         Returns
         -------
          : `BondType`
         """
         if self.is_rdkit_obj():
             return BondType[self._bond_obj.GetBondType().name]
         elif self.is_openbabel_obj():
+            # Open Babel does not have a type specific for aromatic bonds.
+            # Instead, they use a flag to specify if a bond is aromatic
+            # or not. Therefore, if a bond is aromatic, then it returns
+            # BondType.AROMATIC.
+            if self._bond_obj.IsAromatic():
+                return BondType["AROMATIC"]
+
             # Map Open Babel bonds to BondType.
             return BondType[OBBondType(self._bond_obj.GetBondOrder()).name]
 
     def is_aromatic(self):
         """Check if this bond is aromatic or not."""
         if self.is_rdkit_obj():
             return self._bond_obj.GetIsAromatic()
@@ -646,17 +726,20 @@
                     bond_type = RDBondType.values[bond_type.value]
                 elif self.is_openbabel_obj():
                     bond_type = OBBondType[bond_type.name].value
             except KeyError as e:
                 logger.exception(e)
 
                 tool = "Open Babel" if self.is_openbabel_obj() else "RDKit"
-                raise KeyError("The bond type '%s' is not a valid %s bond type." % (bond_type.name, tool))
+                raise KeyError("The bond type '%s' is not a valid %s "
+                               "bond type." % (bond_type.name, tool))
         else:
-            raise IllegalArgumentError("The informed bond type must be an instance of '%s'." % BondType)
+            error_msg = ("The informed bond type must be an instance "
+                         "of '%s'." % BondType)
+            raise IllegalArgumentError(error_msg)
 
         if self.is_rdkit_obj():
             try:
                 self._bond_obj.SetBondType(bond_type)
             except Exception as e:
                 logger.exception(e)
                 raise
@@ -702,49 +785,79 @@
 
 class MolWrapper:
     """This class provides util functions to access molecule properties and
     other information from RDKit and Open Babel objects.
 
     Parameters
     ----------
-    mol_obj : `MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`
+    mol_obj : `MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, \
+                    or :class:`openbabel.pybel.Molecule`
         A molecule to wrap.
 
     Raises
     ------
     MoleculeObjectTypeError
         If the molecular object is not an instance
-            of `MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, or :class:`openbabel.pybel.Molecule`.
+            of `MolWrapper`, :class:`rdkit.Chem.rdchem.Mol`, \
+                or :class:`openbabel.pybel.Molecule`.
     """
 
     def __init__(self, mol_obj):
         if isinstance(mol_obj, self.__class__):
             mol_obj = mol_obj.unwrap()
         elif isinstance(mol_obj, PybelMol):
             mol_obj = mol_obj.OBMol
 
-        if not isinstance(mol_obj, RDMol) and not isinstance(mol_obj, ob.OBMol):
-            logger.exception("Objects of type '%s' are not currently accepted." % mol_obj.__class__)
-            raise MoleculeObjectTypeError("Objects of type '%s' are not currently accepted." % mol_obj.__class__)
+        if (not isinstance(mol_obj, RDMol)
+                and not isinstance(mol_obj, ob.OBMol)):
+            msg = ("Objects of type '%s' are not currently accepted."
+                   % mol_obj.__class__)
+            logger.exception(msg)
+            raise MoleculeObjectTypeError(msg)
 
         self._mol_obj = mol_obj
 
     @classmethod
+    def from_mol_file(cls, file, mol_format, mol_obj_type="rdkit"):
+        """Initialize a molecule from a molecular file.
+
+        Parameters
+        ----------
+        file : str
+            The molecular file.
+        mol_format : str
+            Define the format in which the molecule is represented
+                (e.g., 'mol2' or 'mol').
+        mol_obj_type : {'rdkit', 'openbabel'}
+            Define which library (RDKit or Open Babel) to use to parse the
+            molecular block. The default value is RDKit.
+
+        Returns
+        -------
+         : `MolWrapper`
+        """
+        if mol_obj_type == "rdkit":
+            return cls(read_mol_from_file(file, mol_format))
+        elif mol_obj_type == "openbabel":
+            return cls(list(readfile(mol_format, file))[0])
+
+    @classmethod
     def from_mol_block(cls, block, mol_format, mol_obj_type="rdkit"):
         """Initialize a molecule from a string block.
 
         Parameters
         ----------
         block : str
             The molecular string block.
         mol_format : str
-            Define the format in which the molecule is represented (e.g., 'mol2' or 'mol').
+            Define the format in which the molecule is represented
+            (e.g., 'mol2' or 'mol').
         mol_obj_type : {'rdkit', 'openbabel'}
-            Define which library (RDKit or Open Babel) to use to parse the molecular block.
-            The default value is RDKit.
+            Define which library (RDKit or Open Babel) to use to parse the
+            molecular block. The default value is RDKit.
 
         Returns
         -------
          : `MolWrapper`
         """
         if mol_obj_type == "rdkit":
             return cls(new_mol_from_block(block, mol_format))
@@ -755,18 +868,19 @@
     def from_smiles(cls, smiles, mol_obj_type="rdkit", name=None):
         """Initialize a molecule from a SMILES string.
 
         Parameters
         ----------
         smiles : str
             The SMILES string.
-            Define the format in which the molecule is represented (e.g., 'mol2' or 'mol').
+            Define the format in which the molecule is represented
+            (e.g., 'mol2' or 'mol').
         mol_obj_type : {'rdkit', 'openbabel'}
-            Define which library (RDKit or Open Babel) to use to parse the molecular block.
-            The default value is RDKit.
+            Define which library (RDKit or Open Babel) to use to parse the
+            molecular block. The default value is RDKit.
         name : str, optional
             A name to identify the molecule.
 
         Returns
         -------
          : `MolWrapper`
 
@@ -775,62 +889,75 @@
         MoleculeObjectError
             If it could not create a molecule from the provided SMILES.
 
         Examples
         --------
 
         >>> from luna.wrappers.base import MolWrapper
-        >>> mol_obj = MolWrapper.from_smiles("N[C@@H](CCC(N)=O)C(O)=O", mol_obj_type="openbabel", name="Glutamine")
+        >>> mol_obj = MolWrapper.from_smiles("N[C@@H](CCC(N)=O)C(O)=O",
+        ...                                  mol_obj_type="openbabel",
+        ...                                  name="Glutamine")
 
         """
         if mol_obj_type == "rdkit":
             mol = MolFromSmiles(smiles)
         elif mol_obj_type == "openbabel":
             mol = readstring("smi", smiles)
 
         # Raise an error if the molecule could not be created.
         if mol is None:
-            raise MoleculeObjectError("It could not create a molecule from the provided SMILES '%s'." % smiles)
+            msg = ("It could not create a molecule from the "
+                   "provided SMILES '%s'." % smiles)
+            raise MoleculeObjectError(msg)
 
         mol = cls(mol)
         mol.set_name(name or smiles)
 
         return mol
 
     @property
     def mol_obj(self):
-        """:class:`rdkit.Chem.rdchem.Mol` or :class:`openbabel.pybel.Molecule`: The wrapped molecular object."""
+        """:class:`rdkit.Chem.rdchem.Mol` or \
+                :class:`openbabel.pybel.Molecule`: \
+            The wrapped molecular object."""
         return self._mol_obj
 
     @mol_obj.setter
     def mol_obj(self, mol_obj):
         if isinstance(mol_obj, PybelMol):
             mol_obj = mol_obj.OBMol
 
-        if not isinstance(mol_obj, RDMol) and not isinstance(mol_obj, ob.OBMol):
-            logger.exception("Objects of type '%s' are not currently accepted." % mol_obj.__class__)
-            raise MoleculeObjectTypeError("Objects of type '%s' are not currently accepted." % mol_obj.__class__)
+        if (not isinstance(mol_obj, RDMol)
+                and not isinstance(mol_obj, ob.OBMol)):
+            msg = ("Objects of type '%s' are not currently accepted."
+                   % mol_obj.__class__)
+            logger.exception(msg)
+            raise MoleculeObjectTypeError(msg)
 
         self._mol_obj = mol_obj
 
     def as_rdkit(self):
-        """If the molecule is an Open Babel object, convert it to an RDKit object."""
+        """If the molecule is an Open Babel object, convert it to an
+        RDKit object."""
         if self.is_rdkit_obj():
             return self._mol_obj
         elif self.is_openbabel_obj():
-            new_mol = MolWrapper.from_smiles(self.to_smiles(), mol_obj_type="rdkit")
+            new_mol = MolWrapper.from_smiles(self.to_smiles(),
+                                             mol_obj_type="rdkit")
             new_mol.set_name(self.get_name())
             return new_mol.unwrap()
 
     def as_openbabel(self):
-        """If the molecule is an RDKit object, convert it to an Open Babel object."""
+        """If the molecule is an RDKit object, convert it to an
+        Open Babel object."""
         if self.is_openbabel_obj():
             return self._mol_obj
         elif self.is_rdkit_obj():
-            new_mol = MolWrapper.from_smiles(self.to_smiles(), mol_obj_type="openbabel")
+            new_mol = MolWrapper.from_smiles(self.to_smiles(),
+                                             mol_obj_type="openbabel")
             new_mol.set_name(self.get_name())
             return new_mol.unwrap()
 
     def get_name(self):
         """Get the molecule name.
 
         Returns
@@ -850,48 +977,68 @@
         Parameters
         ----------
         wrapped : bool
             If True, wrap all atoms with `AtomWrapper`.
 
         Returns
         -------
-         : iterable of `AtomWrapper`, :py:class:`rdkit.Chem.rdchem.Atom`, or :class:`openbabel.OBAtom`
+         : iterable of `AtomWrapper`, :py:class:`rdkit.Chem.rdchem.Atom`, \
+                or :class:`openbabel.OBAtom`
         """
         atoms = []
         if self.is_rdkit_obj():
             atoms = self._mol_obj.GetAtoms()
         elif self.is_openbabel_obj():
             atoms = ob.OBMolAtomIter(self._mol_obj)
 
         if atoms and wrapped:
             return [AtomWrapper(atm, self) for atm in atoms]
         return atoms
 
+    def get_atom_by_idx(self, idx, wrapped=True):
+        """Return the atom whose index is ``idx``."""
+        try:
+            atm = [a for a in self.get_atoms() if a.get_idx() == idx][0]
+
+            if wrapped:
+                return atm
+            return atm.unwrap()
+        except Exception:
+            return None
+
     def get_bonds(self, wrapped=True):
         """Get all molecule's bonds.
 
         Parameters
         ----------
         wrapped : bool
             If True, wrap all bonds with `BondWrapper`.
 
         Returns
         -------
-         : iterable of `BondWrapper`, :class:`rdkit.Chem.rdchem.Bond`, or :class:`openbabel.OBBond`
+         : iterable of `BondWrapper`, :class:`rdkit.Chem.rdchem.Bond`, \
+                or :class:`openbabel.OBBond`
         """
         bonds = []
         if self.is_rdkit_obj():
             bonds = self._mol_obj.GetBonds()
         elif self.is_openbabel_obj():
             bonds = ob.OBMolBondIter(self._mol_obj)
 
         if bonds and wrapped:
             return [BondWrapper(bond) for bond in bonds]
         return bonds
 
+    def get_total_charge(self):
+        """Get total molecular charge."""
+        if self.is_rdkit_obj():
+            return GetFormalCharge(self._mol_obj)
+        elif self.is_openbabel_obj():
+            return self._mol_obj.GetTotalCharge()
+
     def get_num_heavy_atoms(self):
         """Get the number of heavy atoms in this molecule."""
         if self.is_rdkit_obj():
             return self._mol_obj.GetNumHeavyAtoms()
         elif self.is_openbabel_obj():
             return self._mol_obj.NumHvyAtoms()
 
@@ -912,14 +1059,27 @@
     def get_obj_type(self):
         """Get the object type ("rdkit" or "openbabel")."""
         if self.is_rdkit_obj():
             return "rdkit"
         elif self.is_openbabel_obj():
             return "openbabel"
 
+    def find_mcs(self, other, match_valences=True,
+                 ring_matches_ring_only=True, complete_rings_only=True):
+        other = MolWrapper(other)
+        other = other.unwrap() if other.is_rdkit_obj() else other.as_rdkit()
+
+        mol_obj = self.unwrap() if self.is_rdkit_obj() else self.as_rdkit()
+
+        # Maximum Common Substructure.
+        return rdFMCS.FindMCS([other, mol_obj],
+                              matchValences=match_valences,
+                              ringMatchesRingOnly=ring_matches_ring_only,
+                              completeRingsOnly=complete_rings_only)
+
     def has_name(self):
         """Check if this molecule has a name."""
         if self.get_name():
             return True
         return False
 
     def set_name(self, name):
@@ -986,22 +1146,25 @@
 
     def __getattr__(self, attr):
         if self.mol_obj is None:
             return None
         return getattr(self._mol_obj, attr)
 
     def __getstate__(self):
-        # Creates a copy of the class' dictionary in case we need to modify the molecular object to pickle it.
+        # Creates a copy of the class' dictionary in case we need to modify the
+        # molecular object to pickle it.
         my_dict = self.__dict__.copy()
         if self.is_openbabel_obj():
             my_dict["_mol_block"] = self.to_mol_block()
             my_dict["_mol_obj_type"] = self.get_obj_type()
             my_dict["_mol_obj"] = None
         return my_dict
 
     def __setstate__(self, state):
         if "_mol_obj_type" in state and "_mol_block" in state:
-            state["_mol_obj"] = self.from_mol_block(state["_mol_block"], "mol", "openbabel").unwrap()
+            state["_mol_obj"] = \
+                self.from_mol_block(state["_mol_block"],
+                                    "mol", "openbabel").unwrap()
             del state["_mol_obj_type"]
             del state["_mol_block"]
 
         self.__dict__.update(state)
```

### Comparing `luna-0.12.2/luna/wrappers/cgo_arrow.py` & `luna-0.13.0/luna/wrappers/cgo_arrow.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/wrappers/cif.py` & `luna-0.13.0/luna/wrappers/cif.py`

 * *Files identical despite different names*

### Comparing `luna-0.12.2/luna/wrappers/obabel.py` & `luna-0.13.0/luna/wrappers/obabel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 from subprocess import Popen, PIPE, TimeoutExpired
 
 from openbabel.pybel import informats, outformats
 
-from luna.util.exceptions import FileNotCreated, InvalidFileFormat
+from luna.util.exceptions import (FileNotCreated, InvalidFileFormat,
+                                  IllegalArgumentError, ProcessingFailed)
 from luna.util.default_values import OPENBABEL
 from luna.util.file import is_file_valid, validate_file, get_file_format
 
 import logging
 logger = logging.getLogger()
 
 
 def _prep_opts(opts, prefix=""):
     opt_list = []
     if opts is not None:
         for key in opts:
-            if len(key) > 1:
-                opt_list.append("--%s%s" % (prefix, key))
+            if key == "x" and prefix == "":
+                opt_list.append("-%s%s" % (key, str(opts[key])))
             else:
-                opt_list.append("-%s%s" % (prefix, key))
+                if len(key) > 1:
+                    opt_list.append("--%s%s" % (prefix, key))
+                else:
+                    opt_list.append("-%s%s" % (prefix, key))
 
-            if opts[key] is not None:
-                opt_list.append(str(opts[key]))
+                if opts[key] is not None:
+                    opt_list.append(str(opts[key]))
     return opt_list
 
 
 def mol_to_svg(infile, output, opts=None):
     """Depict a molecule as SVG using Open Babel.
 
     Parameters
     ----------
     infile : str
         The pathname of a molecular file.
     output : str
         Save the SVG to this file.
     opts : dict
-        A set of depiction options. Check `Open Babel <http://openbabel.org/docs/dev/FileFormats/SVG_depiction.html>`_ \
+        A set of depiction options. Check `Open Babel <http://openbabel.org/docs/dev/FileFormats/SVG_depiction.html>`_
         to discover which options are available.
 
     Examples
     --------
 
     In this example, we will depict the molecule ZINC000007786517 as SVG.
     The following options will be used:
@@ -71,88 +75,142 @@
         else:
             logger.debug("SVG diagram for '%s' created." % infile)
     except Exception as e:
         logger.exception(e)
         raise
 
 
-def convert_molecule(infile, output, infile_format=None,
-                     output_format=None, opts=None, openbabel=OPENBABEL):
+def convert_molecule(mol_input, input_format=None,
+                     output_file=None, output_format=None,
+                     opts=None, openbabel=OPENBABEL):
     """Convert a molecular file to another format using Open Babel.
 
     Parameters
     ----------
 
-    infile : str
-        The pathname of the molecular file to be converted.
-    output : str
+    mol_input : str
+        The pathname of a molecular file or a SMILES string.
+    input_format : str, optional
+        The molecular format of ``mol_input``.
+        If not provided, the format will be defined by the file ``mol_input``
+        extension. If the extension could not be identified, an
+        `InvalidFileFormat` exception will be raised.
+    output_file : str or None
         Save the converted molecule to this file.
-    infile_format : str, optional
-        The molecular format of ``infile``.
-        If not provided, the format will be defined by the file extension.
+        If None, return the output molecule as string.
     output_format : str, optional
-        The molecular format of ``output``.
-        If not provided, the format will be defined by the file extension.
+        The molecular format of ``output_file``.
+        If not provided, the format will be defined by the ``output_file`` when
+        it is not None.
+        Otherwise, it will raise an `InvalidFileFormat` exception.
     opts : dict
-        A set of convertion options. Check `Open Babel <https://openbabel.org/docs/dev/Command-line_tools/babel.html>`_ to discover which options are available.
+        A set of convertion options.
+        Check `Open Babel <https://openbabel.org/docs/dev/Command-line_tools/babel.html>`_
+        to discover which options are available.
     openbabel : str, optional
-        The Open Babel binary location. If not provided, the default binary ('obabel') will be used.
+        The Open Babel binary location.
+        If not provided, the default binary ('obabel') will be used.
+
+
+    Returns
+    -------
+     : str or None
+        Return the converted molecule as a string if ``output_file`` is None.
+        Otherwise, return None.
 
     Raises
     ------
     InvalidFileFormat
         If the provided molecular formats are not accepted by Open Babel.
 
     Examples
     --------
 
-    In this example, we will convert the molecule ZINC000007786517 from the format MOL to MOL2
-    and add hydrogens to it considering a pH of 7 (option "p").
+    In this example, we will convert the molecule ZINC000007786517 from
+    the format MOL to MOL2 and add hydrogens to it considering a pH of 7
+    (option "p").
 
     >>> from luna.util.default_values import LUNA_PATH
     >>> from luna.wrappers.obabel import convert_molecule
-    >>> convert_molecule(infile=f"{LUNA_PATH}/tutorial/inputs/ZINC000007786517.mol",
-    ...                  output="example.mol2",
+    >>> convert_molecule(mol_input=f"{LUNA_PATH}/tutorial/inputs/\
+ZINC000007786517.mol",
+    ...                  output_file="example.mol2",
     ...                  opts={"p": 7})
     """
-    logger.debug("Trying to convert the file '%s' to '%s'." % (infile, output))
-
-    try:
-        # It raises an error if it is not valid.
-        validate_file(infile)
-
-        if infile_format is None:
-            logger.debug("Input file format not defined. It will assume the format from the file extension.")
-            infile_format = get_file_format(infile)
+    logger.info("Molecule or file '%s' will be converted to format '%s'."
+                % (mol_input, input_format))
 
-        if infile_format not in informats:
-            raise InvalidFileFormat("Infile format '%s' does not exist." % infile_format)
-
-        logger.debug("Input format: %s" % infile_format)
+    if is_file_valid(mol_input):
+        if input_format is None:
+            msg = ("Input file format not defined. "
+                   "It will assume the format from the file extension.")
+            logger.debug(msg)
+            input_format = get_file_format(mol_input)
+
+        if input_format not in informats:
+            msg = "Input format '%s' does not exist." % input_format
+            raise InvalidFileFormat(msg)
+
+        logger.debug("Input format: %s" % input_format)
+
+    else:
+        if input_format != "smi":
+            msg = ("File '%s' does not exist or is not a valid file."
+                   % mol_input)
+            raise OSError(msg)
 
+    if isinstance(output_file, str):
         if output_format is None:
-            logger.debug("Output file format not defined. It will assume the format by the file extension.")
-            output_format = get_file_format(output, 1)
+            msg = ("Output file format not defined. It will assume the format "
+                   "by the file extension.")
+            logger.debug(msg)
+            output_format = get_file_format(output_file, 1)
 
         if output_format not in outformats:
-            raise InvalidFileFormat("Infile format '%s' does not exist." % output_format)
+            msg = "Output format '%s' does not exist." % output_format
+            raise InvalidFileFormat(msg)
 
         logger.debug("Output format: %s" % output_format)
 
-        opt_list = _prep_opts(opts)
-        args = [openbabel, "-i", infile_format, infile, "-o", output_format, "-O", output] + opt_list
+    elif output_file is not None:
+        msg = "The 'output_file' should be a string or None."
+        raise IllegalArgumentError(msg)
+
+    if output_format is None:
+        msg = "The output format could not be identified."
+        raise IllegalArgumentError(msg)
+
+    if input_format == "smi":
+        input_list = [f'-:{mol_input}']
+    else:
+        input_list = ['-i', input_format, mol_input]
+
+    if output_file is None:
+        output_list = ['-o', output_format]
+    else:
+        output_list = ['-o', output_format, '-O', output_file]
+
+    opts = opts or {}
+
+    timeout = 30
+    if "gen3d" in opts or "minimize" in opts:
+        timeout = None
 
-        p = Popen(args, stdout=PIPE, stderr=PIPE)
-        try:
-            stdout, stderr = p.communicate(timeout=30)
-        except TimeoutExpired:
-            p.kill()
-            raise
-
-        output_lines = stderr.decode().strip().split("\n")
-        is_mol_converted = output_lines[-1] != "0 molecule converted"
-        if not is_file_valid(output) or not is_mol_converted:
-            raise FileNotCreated("File '%s' not converted to '%s'." % (infile, output))
-        else:
-            logger.debug("File '%s' converted to '%s'." % (infile, output))
-    except Exception:
+    opt_list = _prep_opts(opts)
+    args = [openbabel] + input_list + output_list + opt_list
+
+    p = Popen(args, stdout=PIPE, stderr=PIPE)
+    try:
+        stdout, stderr = p.communicate(timeout=timeout)
+    except TimeoutExpired:
+        p.kill()
         raise
+
+    error_lines = stderr.decode().strip().split("\n")
+    if (error_lines[-1] == "0 molecules converted"
+            or error_lines[-1] == "0 molecule converted"):
+        raise ProcessingFailed("The provided molecule could not be converted.")
+
+    if output_file is None:
+        return stdout.decode().strip()
+
+    logger.debug("File '%s' created with success." % output_file)
```

### Comparing `luna-0.12.2/luna/wrappers/pymol.py` & `luna-0.13.0/luna/wrappers/pymol.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pymol import cmd
 from pymol import util
 
 
 from luna.wrappers.cgo_arrow import cgo_arrow
-from luna.util.exceptions import PymolSessionNotInitialized, IllegalArgumentError
-from luna.util.default_values import PYMOL_INTERACTION_COLOR, INTERACTION_SHORT_NAMES
+from luna.util.exceptions import (PymolSessionNotInitialized,
+                                  IllegalArgumentError)
+from luna.util.default_values import (PYMOL_INTERACTION_COLOR,
+                                      INTERACTION_SHORT_NAMES)
 from luna.util.file import get_filename, get_file_format
 
 from Bio.Data.SCOPData import protein_letters_3to1
 
 import logging
 
 logger = logging.getLogger()
@@ -174,41 +176,44 @@
         -------
          : array_like of float (size 3)
             Atomic coordinates (x, y, z) of each atom selected.
         """
         return cmd.get_coords(selection)
 
     def distance(self, name, sel1, sel2):
-        """Create a new distance object between two atoms given by their selection-expressions.
+        """Create a new distance object between two atoms given by their
+        selection-expressions.
 
         Parameters
         ----------
         name : str
             Name of the distance object to create.
         sel1 : str
             The expression to select the first atom.
         sel2 : str
             The expression to select the second atom.
         """
         cmd.distance(name, sel1, sel2)
 
     def arrow(self, name, atm_sel1, atm_sel2, opts=None):
-        """Draw an arrow object between two atoms given by their selection-expressions.
+        """Draw an arrow object between two atoms given by their
+        selection-expressions.
 
         Parameters
         ----------
         name : str
             Name of the arrow object to create.
         sel1 : str
             The expression to select the first atom.
         sel2 : str
             The expression to select the second atom.
         opts : dict
             A set of options to create the arrow.
-            Check `Pymol <https://pymolwiki.org/index.php/Cgo_arrow>`_ to discover which options are available.
+            Check `Pymol <https://pymolwiki.org/index.php/Cgo_arrow>`_ to
+            discover which options are available.
         """
         opts = opts or {}
         cgo_arrow(atm_sel1, atm_sel2, name=name, **opts)
 
     def save_png(self, output_file, width=1200, height=1200, dpi=100, ray=1):
         """Save the current Pymol session as a PNG format image file.
 
@@ -219,15 +224,16 @@
         width : int
             The width in pixels. The default value is 1,200.
         height : int or str
             The height in pixels. The default value is 1,200.
         dpi : float
             Dots-per-inch. The default value is 100.
         ray : {0, 1}
-            If ``1`` (the default), run ray first to make high-resolution photos.
+            If ``1`` (the default), run ray first to make high-resolution
+            photos.
         """
         cmd.png(output_file, width, height, dpi, ray)
 
     def save_session(self, output_file):
         """Save the current PyMOL state to a PSE format file to later use.
 
         Parameters
@@ -241,34 +247,39 @@
 
     def color(self, tuples):
         """Color objects and atoms.
 
         Parameters
         ----------
         tuples : iterable of tuple
-            Each tuple should contain a color (e.g., 'red') and a selection (e.g., 'hetatm').
+            Each tuple should contain a color (e.g., 'red') and a selection
+            (e.g., 'hetatm').
         """
         for color, selection in tuples:
             cmd.color(color, selection)
 
     def color_by_element(self, selections, c_color="green"):
         """Color atoms by their default element color (e.g., oxygen in red).
 
         Parameters
         ----------
         selections : iterable of str
-            A sequence of selections to define which atoms will be colored by element.
-        c_color : {'green', 'cyan', 'light magenta', 'yellow', 'salmon', 'white', 'slate', 'bright orange', 'purple', 'pink'}
+            A sequence of selections to define which atoms will be colored by
+            element.
+        c_color : {'green', 'cyan', 'light magenta', 'yellow', 'salmon', \
+                    'white', 'slate', 'bright orange', 'purple', 'pink'}
             The carbon color. The default value is 'green'.
         """
 
-        valid_colors = ['green', 'cyan', 'light magenta', 'yellow', 'salmon', 'white',
-                        'slate', 'bright orange', 'purple', 'pink']
+        valid_colors = ['green', 'cyan', 'light magenta', 'yellow', 'salmon',
+                        'white', 'slate', 'bright orange', 'purple', 'pink']
         if c_color.lower() not in valid_colors:
-            raise IllegalArgumentError("Invalid color '%s'. The accepted colors are: %s." % (c_color, ", ".join(valid_colors)))
+            raise IllegalArgumentError("Invalid color '%s'. The accepted "
+                                       "colors are: %s."
+                                       % (c_color, ", ".join(valid_colors)))
 
         c_color = c_color.lower()
 
         for selection in selections:
             if c_color == 'green':
                 util.cbag(selection)
             elif c_color == 'cyan':
@@ -295,19 +306,22 @@
 
         Parameters
         ----------
         name : str
             The group name to create or update.
         members : iterable of str
             The objects to include in the group.
-        action : {'add', 'remove', 'open', 'close', 'toggle', 'auto', 'empty', 'purge', 'excise'}, optional
-            An action to take. If not provided, the default value 'auto' will be used instead.
-            The description of the actions are described below (source: Pymol documentation):
+        action : {'add', 'remove', 'open', 'close', 'toggle', 'auto', \
+                    'empty', 'purge', 'excise'}, optional
+            An action to take. If not provided, the default value
+            'auto' will be used instead. The description of the actions
+            are described below (source: Pymol documentation):
                 * add:     add members to group.
-                * remove:  remove members from group (members will be ungrouped).
+                * remove:  remove members from group (members will be \
+                    ungrouped).
                 * empty:   remove all members from group.
                 * purge:   remove all members from group and delete them.
                 * excise:  remove all members from group and delete group.
                 * open:    expand group display in object menu panel.
                 * close:   collapse group display in object menu panel.
                 * toggle:  toggle group display in object menu panel.
                 * auto:    add or toggle.
@@ -317,16 +331,16 @@
                 cmd.group(name, member, action)
             else:
                 cmd.group(name, member)
 
     def create(self, name, selection):
         """Create a new molecular object from a selection.
 
-        Note that the selected atoms won't be extracted from the original object.
-        Instead, a copy of them will be created in the new object.
+        Note that the selected atoms won't be extracted from the original
+        object. Instead, a copy of them will be created in the new object.
 
         Parameters
         ----------
         name : str
             The object name to be created.
         selection : str
             The expression to select atoms.
@@ -337,16 +351,17 @@
         """Modify atomic properties.
 
         Parameters
         ----------
         selection : str
             The expression to select atoms.
         expression : str
-            Expression in Python language to define which properties should be modified.
-            This can be used, for instance, to rename an atom or chain.
+            Expression in Python language to define which properties should be
+            modified. This can be used, for instance, to rename an atom or
+            chain.
 
         Examples
         --------
 
         Alter the name of a ligand carbon from 'C1' to 'CA'.
 
         >>> pw_obj.alter("hetatm and name C1", "name='CA'")
@@ -363,30 +378,34 @@
         Parameters
         ----------
         name : str
             The setting name to modify.
         value : str
             The new setting value.
         opts : dict
-            A set of options. Check `Pymol <https://pymolwiki.org/index.php/Pseudoatom>`_ to discover which options are available.
+            A set of options.
+            Check `Pymol <https://pymolwiki.org/index.php/Pseudoatom>`_
+            to discover which options are available.
         """
         opts = opts or {}
         cmd.set(name, value, **opts)
 
     def align(self, mobile, target, opts=None):
         """Align the structure ``mobile`` to the ``target`` structure.
 
         Parameters
         ----------
         mobile : str
             The structure to be aligned given by an atomic selection.
         target : str
             The target structure given by an atomic selection.
         opts : dict
-            Alignment options. Check `Pymol <https://pymolwiki.org/index.php/Align>`_ to discover which options are available.
+            Alignment options.
+            Check `Pymol <https://pymolwiki.org/index.php/Align>`_
+            to discover which options are available.
         """
         opts = opts or {}
         cmd.align(mobile, target, **opts)
 
     def delete(self, selections):
         """Delete the provided selections.
 
@@ -407,21 +426,23 @@
         selections : iterable of str
             A sequence of selections to define which atoms will be removed.
         """
         for selection in selections:
             cmd.remove(selection)
 
     def extract(self, tuples):
-        """Perform multiple extractions, i.e., extract atoms from an object to another object.
+        """Perform multiple extractions, i.e., extract atoms from an object to
+        another object.
 
         Parameters
         ----------
         tuples : iterable of tuple
-            Each tuple should contain the object name to where atoms will be added
-            and the selection itself that defines which atoms will be extracted (e.g., 'hetatm').
+            Each tuple should contain the object name to where atoms will be
+            added and the selection itself that defines which atoms will be
+            extracted (e.g., 'hetatm').
         """
         for name, selection in tuples:
             cmd.extract(name, selection)
 
     def load_mol_from_pdb_block(self, pdb_block, obj_name):
         """Load a molecular file from a PDB block string.
 
@@ -457,54 +478,67 @@
 
     def run_cmds(self, commands):
         """Run a set of Pymol commands.
 
         Parameters
         ----------
         commands : iterable of tuple
-            Each tuple should contain a Pymol command and its parameters. See :meth:`run` to more details.
+            Each tuple should contain a Pymol command and its parameters.
+            See :meth:`run` to more details.
         """
 
         for func_name, opts in commands:
             getattr(cmd, func_name)(**opts)
 
 
 class PymolSessionManager:
 
     """Class to start, manage, and save Pymol sessions.
-    This class provides useful built-in functions to load PDB/Mol files and show interactions.
+    This class provides useful built-in functions to load PDB/Mol files and
+    show interactions.
 
     .. note::
-        This class is not intended to be used directly because :meth:`set_view` is not implemented by default.
-        Instead, you should use a class that inherits from `PymolSessionManager` and implements :meth:`set_view`.
-        An example is the class :class:`~luna.interaction.view.InteractionViewer` that implements a custom
-        :meth:`set_view` to show interactions.
-        Therefore, you should define your own logic beyond :meth:`set_view` to save a Pymol session that meets your goals.
+        This class is not intended to be used directly because :meth:`set_view`
+        is not implemented by default. Instead, you should use a class that
+        inherits from `PymolSessionManager` and implements :meth:`set_view`.
+        An example is the class
+        :class:`~luna.interaction.view.InteractionViewer` that implements a
+        custom :meth:`set_view` to show interactions. Therefore, you should
+        define your own logic beyond :meth:`set_view` to save a Pymol session
+        that meets your goals.
 
     Parameters
     ----------
     show_cartoon : bool
         If True, show the protein structure as cartoons.
     bg_color : str
         The background color. The default value is "white".
-        Check `Pymol <https://pymolwiki.org/index.php/Color_Values>`_ to discover which colors are available.
+        Check `Pymol <https://pymolwiki.org/index.php/Color_Values>`_
+        to discover which colors are available.
     add_directional_arrows : bool
-        If True, show arrows for directional interactions (e.g., hydrogen bonds and multipolar interactions).
+        If True, show arrows for directional interactions (e.g., hydrogen bonds
+        and multipolar interactions).
     show_res_labels : bool
         If True (the default), show residue labels.
     inter_color : :class:`~luna.util.ColorPallete`
         A Pymol-compatible color scheme for interactions.
-        The default value is :const:`~luna.util.default_values.PYMOL_INTERACTION_COLOR`.
+        The default value is
+        :const:`~luna.util.default_values.PYMOL_INTERACTION_COLOR`.
     pse_export_version : str
-        Define a legacy format for saving Pymol sessions (PSE files). The default value os '1.8'.
+        Define a legacy format for saving Pymol sessions (PSE files).
+        The default value os '1.8'.
     """
 
-    def __init__(self, show_cartoon=False, bg_color="white",
-                 add_directional_arrows=True, show_res_labels=True,
-                 inter_color=PYMOL_INTERACTION_COLOR, pse_export_version="1.8"):
+    def __init__(self,
+                 show_cartoon=False,
+                 bg_color="white",
+                 add_directional_arrows=True,
+                 show_res_labels=True,
+                 inter_color=PYMOL_INTERACTION_COLOR,
+                 pse_export_version="1.8"):
 
         self.show_cartoon = show_cartoon
         self.bg_color = bg_color
         self.pse_export_version = pse_export_version
         self.inter_color = inter_color
         self.add_directional_arrows = add_directional_arrows
         self.show_res_labels = show_res_labels
@@ -538,33 +572,40 @@
         self.wrapper.set("pse_export_version", self.pse_export_version)
         self.wrapper.set("transparency_mode", 3)
         self.wrapper.set("group_auto_mode", 2)
         self.wrapper.run_cmds([("bg_color", {"color": self.bg_color})])
         self.wrapper.set("internal_gui_width", 370)
 
     def set_view(self, data):
-        """Set the session view. However, this method is not implemented by default.
-        Instead, you should use a class that inherits from `PymolSessionManager` and
-        implements :meth:`set_view`. An example is the class :class:`~luna.interaction.view.InteractionViewer`
-        that implements a custom :meth:`set_view` to show interactions.
-        Therefore, you should define your own logic beyond :meth:`set_view` to save a Pymol session that meets your goals.
+        """Set the session view. However, this method is not implemented by
+        default. Instead, you should use a class that inherits from
+        `PymolSessionManager` and implements :meth:`set_view`. An example is
+        the class :class:`~luna.interaction.view.InteractionViewer` that
+        implements a custom :meth:`set_view` to show interactions.
+        Therefore, you should define your own logic beyond :meth:`set_view` to
+        save a Pymol session that meets your goals.
 
         Parameters
         ----------
         data : iterable
             The data that will be used to set the Pymol view.
         """
         raise NotImplementedError("Use a class that implements this method.")
 
-    def load_pdb(self, pdb_file, pdb_obj, mol_block=None, is_ftmap_output=False):
+    def load_pdb(self,
+                 pdb_file,
+                 pdb_obj,
+                 mol_block=None,
+                 is_ftmap_output=False):
         """Load molecules from PDB files to the current Pymol session.
 
-        Optionally, ligands can also be loaded from a separate molecular string block.
-        This is especially useful when working with docked molecules in which the
-        protein structure is in a PDB file and ligands are in a separate molecular file.
+        Optionally, ligands can also be loaded from a separate molecular string
+        block. This is especially useful when working with docked molecules in
+        which the protein structure is in a PDB file and ligands are in a
+        separate molecular file.
 
         Parameters
         ----------
         pdb_file : str
             The pathname of the PDB file to be loaded.
         pdb_obj : str
             Pymol object to store the loaded structure.
@@ -582,140 +623,180 @@
         if is_ftmap_output:
             objs = self.wrapper.get_names("objects")
             to_merge = []
             for obj in objs:
                 if obj == "protein":
                     to_merge.append(obj)
 
-                    sel = "protein and not resn %s" % " and not resn ".join(protein_letters_3to1.keys())
+                    sel = \
+                        ("protein and not resn %s"
+                         % " and not resn ".join(protein_letters_3to1.keys()))
                     self.wrapper.alter(sel, "type='HETATM'")
 
                 elif obj.endswith(".pdb"):
                     to_merge.append(obj)
                     self.wrapper.alter(obj, "type='HETATM'")
 
             self.wrapper.create(prot_obj, " | ".join(to_merge))
             self.wrapper.delete(objs)
 
-        self.wrapper.extract([("%s.hets" % pdb_obj, "hetatm and %s" % prot_obj)])
+        self.wrapper.extract([("%s.hets" % pdb_obj,
+                               "hetatm and %s" % prot_obj)])
 
         if mol_block is not None:
-            self.wrapper.load_mol_from_pdb_block(mol_block, "%s.hets" % pdb_obj)
+            self.wrapper.load_mol_from_pdb_block(mol_block,
+                                                 "%s.hets" % pdb_obj)
 
         self.wrapper.color_by_element([pdb_obj])
         self.wrapper.hide([("everything", pdb_obj)])
 
         if self.show_cartoon:
             self.wrapper.show([("cartoon", pdb_obj)])
 
-    def set_interactions_view(self, interactions, main_grp, secondary_grp=None):
+    def set_interactions_view(self,
+                              interactions,
+                              main_grp,
+                              secondary_grp=None):
         """Display molecular interactions.
 
         Parameters
         ----------
-        interactions : iterable of :class:`~luna.interaction.type.InteractionType`
+        interactions : iterable of \
+                :class:`~luna.interaction.type.InteractionType`
             A sequence of interactions to show.
         main_grp : str
             Main Pymol object to store atom groups.
         secondary_grp : str, optional
-            Secondary Pymol object to store interactions. If not provided, ``main_grp`` will be used instead.
+            Secondary Pymol object to store interactions.
+            If not provided, ``main_grp`` will be used instead.
         """
 
         residue_selections = set()
 
         secondary_grp = secondary_grp or main_grp
 
         for i, inter in enumerate(interactions):
 
             #
             # Centroid 1
             #
-            obj1_name = "%s.centroids.%s" % (main_grp, hash(tuple(sorted(inter.src_interacting_atms))))
+            centroid_hash1 = hash(tuple(sorted(inter.src_interacting_atms)))
+            obj1_name = "%s.centroids.%s" % (main_grp, centroid_hash1)
             centroid_obj1 = inter.src_centroid
             centroid_obj1_visible = True
-            # Define the centroid in a nucleophile with two atoms as the position of its more electronegative atom.
-            # Remember that the position in the interaction object matters. We have defined that the first group is always
-            # the nucleophile for both dipole-dipole and ion-dipole interactions.
-            if inter.type in NUCLEOPHILE_INTERS and len(inter.src_grp.atoms) == 2:
-                dipole_atm = inter.src_grp.atoms[0] if (inter.src_grp.atoms[0].electronegativity
-                                                        > inter.src_grp.atoms[1].electronegativity) else inter.src_grp.atoms[1]
+            # Define the centroid in a nucleophile with two atoms as the
+            # position of its more electronegative atom. Remember that
+            # the position in the interaction object matters. We have
+            # defined that the first group is always the nucleophile for
+            # both dipole-dipole and ion-dipole interactions.
+            if (inter.type in NUCLEOPHILE_INTERS
+                    and len(inter.src_grp.atoms) == 2):
+                dipole_atm = \
+                    (inter.src_grp.atoms[0]
+                     if (inter.src_grp.atoms[0].electronegativity
+                         > inter.src_grp.atoms[1].electronegativity)
+                     else inter.src_grp.atoms[1])
                 obj1_name += "_%s" % hash(dipole_atm.name)
                 centroid_obj1 = dipole_atm.coord
                 centroid_obj1_visible = False
-            # For unfavorable multipolar interactions, it may happen that the first atom group is an electrophile as well.
-            elif inter.type == "Unfavorable electrophile-electrophile" and len(inter.src_grp.atoms) == 2:
-                dipole_atm = inter.src_grp.atoms[0] if (inter.src_grp.atoms[0].electronegativity
-                                                        < inter.src_grp.atoms[1].electronegativity) else inter.src_grp.atoms[1]
+            # For unfavorable multipolar interactions, it may happen that the
+            # first atom group is an electrophile as well.
+            elif (inter.type == "Unfavorable electrophile-electrophile"
+                    and len(inter.src_grp.atoms) == 2):
+                dipole_atm = \
+                    (inter.src_grp.atoms[0]
+                     if (inter.src_grp.atoms[0].electronegativity
+                         < inter.src_grp.atoms[1].electronegativity)
+                     else inter.src_grp.atoms[1])
                 obj1_name += "_%s" % hash(dipole_atm.name)
                 centroid_obj1 = dipole_atm.coord
                 centroid_obj1_visible = False
 
             #
             # Centroid 2
             #
-            obj2_name = "%s.centroids.%s" % (main_grp, hash(tuple(sorted(inter.trgt_interacting_atms))))
+            centroid_hash2 = hash(tuple(sorted(inter.trgt_interacting_atms)))
+            obj2_name = "%s.centroids.%s" % (main_grp, centroid_hash2)
             centroid_obj2 = inter.trgt_centroid
             centroid_obj2_visible = True
             # Define the centroid in an electrophile with two atoms as
-            # the position of its less electronegative atom. Remember that 
+            # the position of its less electronegative atom. Remember that
             # the position in the interaction object matters. We have defined
-            # that the second group is always the electrophile for both 
+            # that the second group is always the electrophile for both
             # dipole-dipole and ion-dipole interactions.
-            if inter.type in ELECTROPHILE_INTERS and len(inter.trgt_grp.atoms) == 2:
-                dipole_atm = inter.trgt_grp.atoms[0] if (inter.trgt_grp.atoms[0].electronegativity
-                                                         < inter.trgt_grp.atoms[1].electronegativity) else inter.trgt_grp.atoms[1]
+            if (inter.type in ELECTROPHILE_INTERS
+                    and len(inter.trgt_grp.atoms) == 2):
+                dipole_atm = \
+                    (inter.trgt_grp.atoms[0]
+                     if (inter.trgt_grp.atoms[0].electronegativity
+                         < inter.trgt_grp.atoms[1].electronegativity)
+                     else inter.trgt_grp.atoms[1])
                 obj2_name += "_%s" % hash(dipole_atm.name)
                 centroid_obj2 = dipole_atm.coord
                 centroid_obj2_visible = False
-            # For unfavorable multipolar interactions, it may happen that the second atom group is a nucleophile as well.
-            elif inter.type == "Unfavorable nucleophile-nucleophile" and len(inter.trgt_grp.atoms) == 2:
-                dipole_atm = inter.trgt_grp.atoms[0] if (inter.trgt_grp.atoms[0].electronegativity
-                                                         > inter.trgt_grp.atoms[1].electronegativity) else inter.trgt_grp.atoms[1]
+            # For unfavorable multipolar interactions, it may happen that the
+            # second atom group is a nucleophile as well.
+            elif (inter.type == "Unfavorable nucleophile-nucleophile"
+                    and len(inter.trgt_grp.atoms) == 2):
+                dipole_atm = \
+                    (inter.trgt_grp.atoms[0]
+                     if (inter.trgt_grp.atoms[0].electronegativity
+                         > inter.trgt_grp.atoms[1].electronegativity)
+                     else inter.trgt_grp.atoms[1])
                 obj2_name += "_%s" % hash(dipole_atm.name)
                 centroid_obj2 = dipole_atm.coord
                 centroid_obj2_visible = False
 
             # Add pseudoatoms
             if not self.wrapper.obj_exists(obj1_name):
                 self.wrapper.add_pseudoatom(obj1_name,
                                             {"vdw": 1,
                                              "pos": list(centroid_obj1)})
             if not self.wrapper.obj_exists(obj2_name):
                 self.wrapper.add_pseudoatom(obj2_name,
                                             {"vdw": 1,
                                              "pos": list(centroid_obj2)})
 
-            # Set the representation for each compound in the groups involved in the interaction.
-            for compound in inter.src_grp.compounds.union(inter.trgt_grp.compounds):
-                if compound.is_water():
+            # Set the representation for each compound in the groups involved
+            # in the interaction.
+            compounds = inter.src_grp.compounds.union(inter.trgt_grp.compounds)
+            for compound in compounds:
+                if compound.is_water() or compound.is_metal():
                     comp_repr = "sphere"
                 elif compound.is_hetatm():
-                    if len(compound.child_list) == 1 or len([atm for atm in compound.child_list if atm.element != "H"]) == 1:
+                    if (len(compound.child_list) == 1
+                            or len([atm for atm in compound.child_list
+                                    if atm.element != "H"]) == 1):
                         comp_repr = "sphere"
                     else:
                         comp_repr = "sticks"
                 else:
                     comp_repr = "sticks"
 
-                comp_sel = "%s and %s" % (main_grp, mybio_to_pymol_selection(compound))
+                comp_sel = ("%s and %s"
+                            % (main_grp, mybio_to_pymol_selection(compound)))
                 self.wrapper.show([(comp_repr, comp_sel)])
                 carb_color = "green" if compound.is_target() else "gray"
                 self.wrapper.color([(carb_color, comp_sel + " AND elem C")])
 
                 if compound.is_residue():
                     residue_selections.add(comp_sel)
 
                     # Show residue label if required.
                     if self.show_res_labels:
-                        self.wrapper.label([("%s AND name CA" % comp_sel, '"%s-%s" % (resn, resi)')])
+                        self.wrapper.label([("%s AND name CA" % comp_sel,
+                                             '"%s-%s" % (resn, resi)')])
 
-            # Check if the interaction involves the same compound: intramolecular interactions.
+            # Check if the interaction involves the same
+            # compound: intramolecular interactions.
             inter_grp = "intra" if inter.is_intramol_interaction() else "inter"
 
-            src_grp_name = "+".join(["%s-%s-%d%s" % (c.parent.id, c.resname, c.id[1], c.id[2].strip())
+            src_grp_name = "+".join(["%s-%s-%d%s"
+                                     % (c.parent.id, c.resname,
+                                        c.id[1], c.id[2].strip())
                                      for c in sorted(inter.src_grp.compounds)])
 
             trgt_grp_name = \
                 "+".join(["%s-%s-%d%s" % (c.parent.id, c.resname,
                                           c.id[1], c.id[2].strip())
                           for c in sorted(inter.trgt_grp.compounds)])
 
@@ -725,92 +806,112 @@
                             i, src_grp_name, trgt_grp_name))
 
             inter_name = "%s.line" % inter_grp
 
             self.wrapper.distance(inter_name, obj1_name, obj2_name)
             self.wrapper.hide([("label", inter_name)])
 
+            inter_color = self.inter_color.get_color(inter.type)
+
             # Set styles to the interactions.
-            self.wrapper.color([(self.inter_color.get_color(inter.type), inter_name)])
+            self.wrapper.color([(inter_color,
+                                 inter_name)])
 
             if self.add_directional_arrows:
 
                 if inter.type in UNFAVORABLE_INTERS:
                     arrow_name1 = "%s.arrow1" % inter_grp
                     arrow_name2 = "%s.arrow2" % inter_grp
 
                     square_name = "%s.block" % inter_grp
 
-                    arrow_opts = {"radius": 0.03, "gap": 0.9, "hlength": 0.5, "hradius": 0.2,
-                                  "color": self.inter_color.get_color(inter.type)}
-                    square_opts = {"radius": 0.3, "gap": 1.5, "hlength": 0, "hradius": 0,
-                                   "color": self.inter_color.get_color(inter.type)}
+                    arrow_opts = {"radius": 0.03, "gap": 0.9,
+                                  "hlength": 0.5, "hradius": 0.2,
+                                  "color": inter_color}
+                    square_opts = {"radius": 0.3,
+                                   "gap": 1.5, "hlength": 0,
+                                   "hradius": 0, "color": inter_color}
 
                     # Two arrows in different directions
-                    self.wrapper.arrow(arrow_name1, obj1_name, obj2_name, arrow_opts)
+                    self.wrapper.arrow(arrow_name1,
+                                       obj1_name,
+                                       obj2_name,
+                                       arrow_opts)
 
                     if not inter.is_directional():
-                        self.wrapper.arrow(arrow_name2, obj2_name, obj1_name, arrow_opts)
-                    self.wrapper.arrow(arrow_name2, obj2_name, obj1_name, arrow_opts)
+                        self.wrapper.arrow(arrow_name2,
+                                           obj2_name,
+                                           obj1_name,
+                                           arrow_opts)
+                    self.wrapper.arrow(arrow_name2,
+                                       obj2_name,
+                                       obj1_name,
+                                       arrow_opts)
 
                     # Add a square-like object
                     self.wrapper.arrow(square_name, obj1_name,
                                        obj2_name, square_opts)
 
                 # Add arrows over the interaction lines to
                 # represent directional interactions
                 elif inter.is_directional():
                     arrow_name = "%s.arrow" % inter_grp
-
-                    inter_color = self.inter_color.get_color(inter.type)
                     arrow_opts = {"radius": 0.03, "gap": 0.9,
                                   "hlength": 0.5, "hradius": 0.2,
                                   "color": inter_color}
-
-                    self.wrapper.arrow(arrow_name, obj1_name, obj2_name, arrow_opts)
+                    self.wrapper.arrow(arrow_name,
+                                       obj1_name,
+                                       obj2_name,
+                                       arrow_opts)
 
             # If a group object contains more than one atom.
             if inter.src_grp.size > 1 and centroid_obj1_visible:
-                # Add the centroids to the group "centroids" and append them to the main group
+                # Add the centroids to the group "centroids" and append them
+                # to the main group
                 self._set_centroid_style(obj1_name)
-            # Otherwise, just remove the centroid as it will not add any new information (the atom represented
-            # by the centroid is already the atom itself).
+            # Otherwise, just remove the centroid as it will not add any new
+            # information (the atom represented by the centroid is already the
+            # atom itself).
             else:
                 self.wrapper.delete([obj1_name])
 
             # If a group object contains more than one atom.
             if inter.trgt_grp.size > 1 and centroid_obj2_visible:
-                # Add the centroids to the group "centroids" and append them to the main group
+                # Add the centroids to the group "centroids" and append them
+                # to the main group
                 self._set_centroid_style(obj2_name)
-            # Otherwise, just remove the centroid as it will not add any new information (the atom represented
-            # by the centroid is already been displayed).
+            # Otherwise, just remove the centroid as it will not add any new
+            # information (the atom represented by the centroid is already
+            # been displayed).
             else:
                 self.wrapper.delete([obj2_name])
 
         return residue_selections
 
     def _set_centroid_style(self, centroid):
         # Set styles to the centroid.
         self.wrapper.hide([("nonbonded", centroid)])
         self.wrapper.show([("sphere", centroid)])
         self.wrapper.set("sphere_scale", 0.2, {"selection": centroid})
 
     def set_last_details_to_view(self):
-        """This method can be called to apply final modifications to the Pymol session.
-        In its default version, the following modifications are applied:
+        """This method can be called to apply final modifications to the
+        Pymol session. In its default version, the following modifications
+        are applied:
             * Dash radius for interactions is set to 0.08;
             * Labels are set to bold and their size is set to 20;
             * Atomic spheres' scale is set to 0.3;
             * Hydrogen atoms are hidden;
             * The view is centered within the visible objects.
         """
         self.wrapper.set("dash_radius", 0.08)
         self.wrapper.set("label_font_id", "13")
         self.wrapper.set("label_size", "20")
-        self.wrapper.set("sphere_scale", "0.3", {"selection": "visible and not name PS*"})
+        self.wrapper.set("sphere_scale", "0.3",
+                         {"selection": "visible and not name PS*"})
         self.wrapper.hide([("everything", "elem H+D")])
         self.wrapper.center("visible")
 
     def save_session(self, output_file):
         """Save the Pymol session as a PSE file of name ``output_file``."""
         if not isinstance(self.wrapper, PymolWrapper):
             raise PymolSessionNotInitialized("No session was initialized.")
@@ -823,16 +924,17 @@
             raise PymolSessionNotInitialized("No session was initialized.")
 
         self.wrapper.reinitialize()
         self.wrapper = None
 
 
 def mybio_to_pymol_selection(entity):
-    """Transform an :class:`~luna.MyBio.PDB.Entity.Entity` instance into a Pymol selection-expression,
-    which can then be used to select atoms in a Pymol session.
+    """Transform an :class:`~luna.MyBio.PDB.Entity.Entity` instance into a
+    Pymol selection-expression, which can then be used to select atoms in a
+    Pymol session.
 
     Parameters
     ----------
     entity : :class:`~luna.MyBio.PDB.Entity.Entity`
         An entity to be transformed into a Pymol selection-expression.
 
     Returns
@@ -844,15 +946,17 @@
     --------
 
     First, let's parse a PDB file to work with.
 
     >>> from luna.util.default_values import LUNA_PATH
     >>> from luna.MyBio.PDB.PDBParser import PDBParser
     >>> pdb_parser = PDBParser(PERMISSIVE=True, QUIET=True)
-    >>> structure = pdb_parser.get_structure("Protein", f"{LUNA_PATH}/tutorial/inputs/3QQK.pdb")
+    >>> structure = pdb_parser.get_structure("Protein",
+    ...                                      f"{LUNA_PATH}/tutorial/\
+inputs/3QQK.pdb")
 
     Now, let's get the Pymol selection-expression for the chain A.
 
     >>> from luna.wrappers.pymol import mybio_to_pymol_selection
     >>> print(mybio_to_pymol_selection(structure[0]['A']))
     chain A
```

### Comparing `luna-0.12.2/luna/wrappers/rdkit.py` & `luna-0.13.0/luna/wrappers/rdkit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from rdkit.Chem import MolFromMol2File, MolFromPDBFile, MolFromMolFile, MolFromMolBlock, MolFromMol2Block, SanitizeFlags, SanitizeMol
+from rdkit.Chem import (MolFromMol2File, MolFromPDBFile, MolFromMolFile,
+                        MolFromMolBlock, MolFromMol2Block, SanitizeFlags,
+                        SanitizeMol)
 from xopen import xopen
 
 from luna.util.file import get_file_format
 from luna.util.exceptions import IllegalArgumentError
 
 import re
 import logging
@@ -39,34 +41,41 @@
         If the provided molecular format is not accepted by RDKit.
 
     Examples
     --------
 
     >>> from luna.util.default_values import LUNA_PATH
     >>> from luna.wrappers.rdkit import read_mol_from_file
-    >>> rdk_mol = read_mol_from_file(mol_file=f"{LUNA_PATH}/tutorial/inputs/ZINC000007786517.mol",
+    >>> rdk_mol = read_mol_from_file(mol_file=f"{LUNA_PATH}/tutorial/inputs/\
+ZINC000007786517.mol",
     ...                              mol_format="mol")
     >>> print(rdk_mol.GetProp("_Name"))
      ZINC000007786517
     """
 
     if mol_format == "mol2":
-        # First it creates the molecule without applying the sanitization function.
+        # First it creates the molecule without applying the
+        # sanitization function.
         rdk_mol = MolFromMol2File(mol_file, sanitize=False, removeHs=removeHs)
     elif mol_format == "pdb":
-        # First it creates the molecule without applying the sanitization function.
+        # First it creates the molecule without applying the
+        # sanitization function.
         rdk_mol = MolFromPDBFile(mol_file, sanitize=False, removeHs=removeHs)
     elif mol_format in RDKIT_FORMATS:
-        # First it creates the molecule without applying the sanitization function.
+        # First it creates the molecule without applying the
+        # sanitization function.
         rdk_mol = MolFromMolFile(mol_file, sanitize=False, removeHs=removeHs)
     else:
-        raise IllegalArgumentError("Invalid '%s' format. The accepted formats are: %s." % (mol_format, ",".join(RDKIT_FORMATS)))
+        raise IllegalArgumentError("Invalid '%s' format. The accepted formats "
+                                   "are: %s." % (mol_format,
+                                                 ",".join(RDKIT_FORMATS)))
 
     # Now it sanitizes the molecule if necessary.
-    # We do it here in order to catch an Exception while performing the sanitization.
+    # We do it here in order to catch an Exception while performing the
+    # sanitization.
     if sanitize:
         try:
             SanitizeMol(rdk_mol, SanitizeFlags.SANITIZE_ALL)
         except Exception as e:
             logger.exception(e)
             return None
     return rdk_mol
@@ -104,34 +113,43 @@
     ...           mol_block = IN.read()
     >>> rdk_mol = new_mol_from_block(block=mol_block, mol_format="sdf")
     >>> print(rdk_mol.GetProp("_Name"))
     GLY
     """
 
     if mol_format == "mol2":
-        # First it creates the molecule without applying the sanitization function.
+        # First it creates the molecule without applying the
+        # sanitization function.
         rdk_mol = MolFromMol2Block(block, sanitize=False, removeHs=removeHs)
     elif mol_format in RDKIT_FORMATS:
-        # First it creates the molecule without applying the sanitization function.
+        # First it creates the molecule without applying the
+        # sanitization function.
         rdk_mol = MolFromMolBlock(block, sanitize=False, removeHs=removeHs)
     else:
-        raise IllegalArgumentError("Invalid '%s' format. The accepted formats are: %s." % (mol_format, ",".join(RDKIT_FORMATS)))
+        raise IllegalArgumentError("Invalid '%s' format. The accepted formats "
+                                   "are: %s." % (mol_format,
+                                                 ",".join(RDKIT_FORMATS)))
 
     # Now it sanitizes the molecule if necessary.
-    # We do it here in order to catch an Exception while performing the sanitization.
+    # We do it here in order to catch an Exception while performing the
+    # sanitization.
     if sanitize:
         try:
             SanitizeMol(rdk_mol, SanitizeFlags.SANITIZE_ALL)
         except Exception as e:
             logger.exception(e)
             return None
     return rdk_mol
 
 
-def read_multimol_file(mol_file, targets=None, mol_format=None, sanitize=True, removeHs=True):
+def read_multimol_file(mol_file,
+                       targets=None,
+                       mol_format=None,
+                       sanitize=True,
+                       removeHs=True):
     """Read molecules from a multimolecular file using RDKit.
 
     Parameters
     ----------
     mol_file : str
         The pathname of the molecular file to be read.
     targets : iterable of str
@@ -148,69 +166,85 @@
     -------
      : tuple of (:class:`rdkit.Chem.rdchem.Mol`, int)
         A tuple containing the parsed molecule and its id.
 
     Raises
     ------
     IllegalArgumentError
-        If the provided or identified molecular format is not accepted by RDKit.
+        If the provided or identified molecular format is not accepted
+        by RDKit.
 
     Examples
     --------
 
-    In this first example, we will read all molecules from a multimolecular file.
+    In this first example, we will read all molecules from a multimolecular
+    file.
 
     >>> from luna.util.default_values import LUNA_PATH
     >>> from luna.wrappers.rdkit import read_multimol_file
-    >>> for mol_tuple in read_multimol_file(mol_file=f"{LUNA_PATH}/tutorial/inputs/ligands.mol2"):
+    >>> for mol_tuple in read_multimol_file(mol_file=f"{LUNA_PATH}/tutorial/\
+inputs/ligands.mol2"):
     ...     print(mol_tuple[0].GetProp("_Name"))
      ZINC000343043015
      ZINC000065293174
      ZINC000575033470
      ZINC000096459890
      ZINC000012442563
 
-    Now, we will only read two molecules (ZINC000065293174, ZINC000096459890) from the same multimolecular file.
+    Now, we will only read two molecules (ZINC000065293174, ZINC000096459890)
+    from the same multimolecular file.
 
     >>> from luna.util.default_values import LUNA_PATH
     >>> from luna.wrappers.rdkit import read_multimol_file
-    >>> for mol_tuple in read_multimol_file(mol_file=f"{LUNA_PATH}/tutorial/inputs/ligands.mol2",
-    ...                                     targets=["ZINC000065293174", "ZINC000096459890"]):
+    >>> for mol_tuple in read_multimol_file(mol_file=f"{LUNA_PATH}/tutorial/\
+inputs/ligands.mol2",
+    ...                                     targets=["ZINC000065293174", \
+"ZINC000096459890"]):
     ...     print(mol_tuple[0].GetProp("_Name"))
      ZINC000065293174
      ZINC000096459890
     """
 
     def apply_mol_format(lines):
-        # Check if the MOL file contains a valid header comprising a Title line, Program/file timestamp line, and a Comment line.
-        # Thus, the Counts line must be in line 4 (index 3). If it's not, add blank lines to match the format.
+        # Check if the MOL file contains a valid header comprising a Title
+        # line, Program/file timestamp line, and a Comment line.
+        # Thus, the Counts line must be in line 4 (index 3). If it's not,
+        # add blank lines to match the format.
         # This amendment is necessary otherwise RDKit will crash.
         if not REGEX_MOL_FILE.search(lines[3]):
-            logger.warning("While parsing the file '%s', we found a molecule starting at line #%d that does not contain a valid header. "
-                           "We will add empty lines to its header to match the MOL file format." % (mol_file, mol_starts_at))
+            logger.warning("While parsing the file '%s', we found a molecule "
+                           "starting at line #%d that does not contain a "
+                           "valid header. We will add empty lines to its "
+                           "header to match the MOL file format."
+                           % (mol_file, mol_starts_at))
 
             counts_line_pos = None
             for i, line in enumerate(lines):
                 if REGEX_MOL_FILE.search(line):
                     counts_line_pos = i
                     break
 
             missing_lines = ["\n"] * (3 - counts_line_pos)
             lines = missing_lines + lines
 
         if lines[-1].strip() != "M  END":
-            logger.warning("While parsing the file '%s', we found a molecule starting at line #%d that does not contain the END line. "
-                           "We will add it to the block end to match the MOL file format." % (mol_file, mol_starts_at))
+            logger.warning("While parsing the file '%s', we found a molecule "
+                           "starting at line #%d that does not contain the "
+                           "END line. We will add it to the block end to "
+                           "match the MOL file format."
+                           % (mol_file, mol_starts_at))
             lines.append("M  END\n")
         return lines
 
     ext = mol_format or get_file_format(mol_file, ignore_compression=True)
 
     if ext not in RDKIT_FORMATS:
-        raise IllegalArgumentError("Format '%s' informed or assumed from the filename is invalid. The accepted formats are: %s."
+        raise IllegalArgumentError("Format '%s' informed or assumed from the "
+                                   "filename is invalid. The accepted formats "
+                                   "are: %s."
                                    % (ext, ",".join(RDKIT_FORMATS)))
 
     with xopen(mol_file, "r") as IN:
         if targets is not None:
             targets = set(targets)
 
         mol = []
@@ -231,72 +265,97 @@
                     mol_starts_at = line_count
 
                 if ext == "mol2":
                     if line.startswith("#"):
                         continue
                     # New molecule block definition is starting...
                     if line.startswith("@<TRIPOS>MOLECULE"):
-                        # New molecule identified but an old one already exists.
+                        # New molecule identified but an old one
+                        # already exists.
                         if mol:
                             mol_id = mol[1].strip()
-                            # If a target list is not informed, create a new molecule object.
+                            # If a target list is not informed, create a new
+                            # molecule object.
                             if targets is None:
                                 # Create a new RDKit object
-                                rdk_mol = new_mol_from_block("".join(mol), ext, sanitize, removeHs)
+                                rdk_mol = new_mol_from_block("".join(mol),
+                                                             ext,
+                                                             sanitize,
+                                                             removeHs)
                                 yield ((rdk_mol, mol_id))
-                            # Otherwise, create a new molecule only if it is in the list.
+                            # Otherwise, create a new molecule only if it
+                            # is in the list.
                             elif mol_id in targets:
                                 targets.remove(mol_id)
                                 # Create a new RDKit object
-                                rdk_mol = new_mol_from_block("".join(mol), ext, sanitize, removeHs)
+                                rdk_mol = new_mol_from_block("".join(mol),
+                                                             ext,
+                                                             sanitize,
+                                                             removeHs)
                                 yield ((rdk_mol, mol_id))
                         # Restart the molecule block.
                         mol = []
                     mol.append(line)
                 else:
                     if line.startswith("M  END"):
                         mol.append(line)
-                        # Fix the MOL block in cases where the header or end lines do not match the MOL file format.
+                        # Fix the MOL block in cases where the header or end
+                        # lines do not match the MOL file format.
                         mol = apply_mol_format(mol)
                         mol_id = mol[0].strip()
 
-                        # If a target list is informed, create a new molecule only if it is in the list.
+                        # If a target list is informed, create a new molecule
+                        # only if it is in the list.
                         if targets is None:
                             # Create a new RDKit object
-                            rdk_mol = new_mol_from_block("".join(mol), ext, sanitize, removeHs)
+                            rdk_mol = new_mol_from_block("".join(mol),
+                                                         ext,
+                                                         sanitize,
+                                                         removeHs)
                             yield((rdk_mol, mol_id))
 
                         elif mol[0].strip() in targets:
                             targets.remove(mol_id)
                             # Create a new RDKit object
-                            rdk_mol = new_mol_from_block("".join(mol), ext, sanitize, removeHs)
+                            rdk_mol = new_mol_from_block("".join(mol),
+                                                         ext,
+                                                         sanitize,
+                                                         removeHs)
                             yield((rdk_mol, mol_id))
                         # Restart the molecule block.
                         mol = []
-                        # After finding a molecule block, ignore any following lines until it finds a line "$$$$".
+                        # After finding a molecule block, ignore any following
+                        # lines until it finds a line "$$$$".
                         ignore_lines = True
                     elif line.startswith("$$$$") is False:
                         # Ignore lines util it finds a line "$$$$".
                         if ignore_lines:
                             continue
                         mol.append(line)
                     else:
                         ignore_lines = False
 
             except StopIteration:
                 if mol:
                     if ext == "mol":
-                        # Fix the MOL block in cases where the header or end lines do not match the MOL file format.
+                        # Fix the MOL block in cases where the header or end
+                        # lines do not match the MOL file format.
                         mol = apply_mol_format(mol)
 
-                    mol_id = mol[1].strip() if ext == "mol2" else mol[0].strip()
+                    mol_id = (mol[1].strip() if ext == "mol2"
+                              else mol[0].strip())
 
-                    # If a target list is informed, create a new molecule only if it is in the list.
-                    if targets is None or (targets is not None and mol_id in targets):
+                    # If a target list is informed, create a new molecule only
+                    # if it is in the list.
+                    if (targets is None
+                            or (targets is not None and mol_id in targets)):
                         # Create a new RDKit object
-                        rdk_mol = new_mol_from_block("".join(mol), ext, sanitize, removeHs)
+                        rdk_mol = new_mol_from_block("".join(mol),
+                                                     ext,
+                                                     sanitize,
+                                                     removeHs)
                         yield ((rdk_mol, mol_id))
                 break
 
             # If all target compounds were already found, just break the loop.
             if targets is not None and len(targets) == 0:
                 break
```

### Comparing `luna-0.12.2/luna.egg-info/PKG-INFO` & `luna-0.13.0/luna.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: luna
-Version: 0.12.2
+Version: 0.13.0
 Summary: LUNA: drug discovery toolkit
 Home-page: https://github.com/keiserlab/LUNA
-Download-URL: https://github.com/keiserlab/LUNA/tarball/v0.12.2
+Download-URL: https://github.com/keiserlab/LUNA/tarball/v0.13.0
 Author: Alexandre Fassio
 Author-email: afassio@keiserlab.org
 License: MIT
 Project-URL: Bug Reports, https://github.com/keiserlab/LUNA/issues
 Project-URL: Source, https://github.com/keiserlab/LUNA/
 Keywords: luna eifp fifp hifp ifp interaction fingerprint protein-ligand molecule docking
 Platform: UNKNOWN
@@ -42,17 +42,31 @@
 
 Documentation is hosted by ReadTheDocs_, and development occurs on GitHub_.
 
 
 Installation and Usage
 ----------------------
 
-For installation and usage instructions, see the `documentation <http://luna-toolkit.readthedocs.io>`_.
+The latest stable release (and required dependencies) can be installed as follows:
 
-See the LUNA `paper repository`_ for an application of LUNA and all code used for the LUNA paper [1]_.
+1. Download LUNA’s `environment.yml <https://github.com/keiserlab/LUNA/blob/master/luna-env.yml>`_ file.
+
+2. Create the Conda environment using the downloaded file:
+
+    conda env create -f <LUNA-ENV-FILE>
+
+3. After creating the Conda environment, activate it:
+
+    conda activate luna-env
+
+4. Finally, install LUNA from Pip:
+
+    pip install luna
+
+For additional installation options and usage instructions, refer to the `documentation <http://luna-toolkit.readthedocs.io>`_.
 
 
 License
 -------
 
 LUNA is available under the |license|.
```

### Comparing `luna-0.12.2/luna.egg-info/SOURCES.txt` & `luna-0.13.0/luna.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 luna.egg-info/SOURCES.txt
 luna.egg-info/dependency_links.txt
 luna.egg-info/entry_points.txt
 luna.egg-info/requires.txt
 luna.egg-info/top_level.txt
 luna/MyBio/__init__.py
 luna/MyBio/extractor.py
+luna/MyBio/neighbors.py
 luna/MyBio/selector.py
 luna/MyBio/util.py
 luna/MyBio/version_control.py
 luna/MyBio/PDB/AbstractPropertyMap.py
 luna/MyBio/PDB/Atom.py
 luna/MyBio/PDB/Chain.py
 luna/MyBio/PDB/DSSP.py
@@ -57,20 +58,28 @@
 luna/config/params.py
 luna/data/BaseFeatures.fdef
 luna/data/BaseFeatures_DIP2_NoMicrospecies.fdef
 luna/data/LUNA.fdef
 luna/data/MinimalFeatures.fdef
 luna/data/ligand_expo.tsv
 luna/data/precomputed_residue_atom_features.json
+luna/data/precomputed_residue_data.json
+luna/data/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+luna/docking/__init__.py
+luna/docking/dock6/__init__.py
+luna/docking/dock6/default.cfg
+luna/docking/dock6/ligands.py
+luna/docking/dock6/params.py
 luna/interaction/__init__.py
 luna/interaction/bind.cfg
 luna/interaction/calc.py
 luna/interaction/config.cfg
 luna/interaction/config.py
 luna/interaction/contact.py
+luna/interaction/cov.py
 luna/interaction/filter.cfg
 luna/interaction/filter.py
 luna/interaction/type.py
 luna/interaction/view.py
 luna/interaction/fp/__init__.py
 luna/interaction/fp/fingerprint.py
 luna/interaction/fp/shell.py
@@ -81,14 +90,15 @@
 luna/mol/charge_model.py
 luna/mol/clustering.py
 luna/mol/depiction.py
 luna/mol/entry.py
 luna/mol/features.py
 luna/mol/fingerprint.py
 luna/mol/groups.py
+luna/mol/precomp_data.py
 luna/mol/standardiser.py
 luna/mol/templates.py
 luna/mol/validator.py
 luna/util/__init__.py
 luna/util/config.py
 luna/util/default_values.py
 luna/util/exceptions.py
@@ -98,13 +108,21 @@
 luna/util/logging.py
 luna/util/logging_ini.py
 luna/util/math.py
 luna/util/multiprocessing_logging.py
 luna/util/progress_tracker.py
 luna/util/stringcase.py
 luna/wrappers/__init__.py
+luna/wrappers/antechamber.py
 luna/wrappers/base.py
 luna/wrappers/cgo_arrow.py
 luna/wrappers/cif.py
 luna/wrappers/obabel.py
 luna/wrappers/pymol.py
-luna/wrappers/rdkit.py
+luna/wrappers/rdkit.py
+luna/wrappers/chemaxon/__init__.py
+luna/wrappers/chemaxon/conformer.py
+luna/wrappers/chemaxon/stereoisomers.py
+luna/wrappers/chemaxon/tautomers.py
+luna/wrappers/chemaxon/util.py
+luna/wrappers/chimera/__init__.py
+luna/wrappers/chimera/add_charges.py
```

### Comparing `luna-0.12.2/setup.py` & `luna-0.13.0/setup.py`

 * *Files identical despite different names*

