# Comparing `tmp/matgl-0.2.1.tar.gz` & `tmp/matgl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.2.1.tar", last modified: Tue May  2 14:06:49 2023, max compression
+gzip compressed data, was "matgl-0.3.0.tar", last modified: Sun May  7 20:32:51 2023, max compression
```

## Comparing `matgl-0.2.1.tar` & `matgl-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,53 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.759614 matgl-0.2.1/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.2.1/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)     8113 2023-05-02 14:06:49.759712 matgl-0.2.1/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     6963 2023-04-30 16:12:51.000000 matgl-0.2.1/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.752371 matgl-0.2.1/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      128 2023-05-02 13:55:59.000000 matgl-0.2.1/matgl/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1937 2023-05-02 13:54:04.000000 matgl-0.2.1/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.753846 matgl-0.2.1/matgl/dataloader/
--rw-r--r--   0 shyue      (501) staff       (20)       53 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/dataloader/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    11497 2023-05-02 13:08:40.000000 matgl-0.2.1/matgl/dataloader/dataset.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.754617 matgl-0.2.1/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5323 2023-05-02 13:08:40.000000 matgl-0.2.1/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)     6802 2023-05-02 13:08:40.000000 matgl-0.2.1/matgl/graph/converters.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.757342 matgl-0.2.1/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)       60 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2099 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     3586 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     2168 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/bond_expansion.py
--rw-r--r--   0 shyue      (501) staff       (20)     6124 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/core.py
--rw-r--r--   0 shyue      (501) staff       (20)      809 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/layers/cutoff_functions.py
--rw-r--r--   0 shyue      (501) staff       (20)     3144 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/embedding_block.py
--rw-r--r--   0 shyue      (501) staff       (20)    16058 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/graph_conv.py
--rw-r--r--   0 shyue      (501) staff       (20)     3972 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/readout_block.py
--rw-r--r--   0 shyue      (501) staff       (20)     3726 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.758509 matgl-0.2.1/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      124 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    12940 2023-03-24 14:41:18.000000 matgl-0.2.1/matgl/models/ase_interface.py
--rw-r--r--   0 shyue      (501) staff       (20)    12307 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/models/m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)    12878 2023-05-02 13:54:32.000000 matgl-0.2.1/matgl/models/megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     3089 2023-03-24 14:22:00.000000 matgl-0.2.1/matgl/models/potential.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.759407 matgl-0.2.1/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1451 2023-05-02 14:06:01.000000 matgl-0.2.1/matgl/utils/data.py
--rw-r--r--   0 shyue      (501) staff       (20)    17700 2023-05-02 13:08:40.000000 matgl-0.2.1/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/utils/sb_roots.npy
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.753390 matgl-0.2.1/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)     8113 2023-05-02 14:06:49.000000 matgl-0.2.1/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)      855 2023-05-02 14:06:49.000000 matgl-0.2.1/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-05-02 14:06:49.000000 matgl-0.2.1/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       10 2023-05-02 14:06:49.000000 matgl-0.2.1/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-05-02 14:06:49.000000 matgl-0.2.1/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     3121 2023-03-24 14:22:00.000000 matgl-0.2.1/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)      603 2023-05-02 14:06:49.760017 matgl-0.2.1/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     2074 2023-05-02 13:08:40.000000 matgl-0.2.1/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.781227 matgl-0.3.0/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.3.0/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)     8114 2023-05-07 20:32:51.781087 matgl-0.3.0/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     6964 2023-05-07 18:00:44.000000 matgl-0.3.0/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.774402 matgl-0.3.0/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      128 2023-05-07 20:31:54.000000 matgl-0.3.0/matgl/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.775451 matgl-0.3.0/matgl/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.3.0/matgl/apps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3574 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/apps/pes.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2819 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.775967 matgl-0.3.0/matgl/ext/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.3.0/matgl/ext/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15713 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/ext/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5404 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/ext/pymatgen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.776732 matgl-0.3.0/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.3.0/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5323 2023-05-02 13:08:40.000000 matgl-0.3.0/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)      551 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/graph/converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11083 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/graph/data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.777668 matgl-0.3.0/matgl/graph/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:28:02.000000 matgl-0.3.0/matgl/graph/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4907 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/graph/tests/test_compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5528 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/graph/tests/test_converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7995 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/graph/tests/test_data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.779068 matgl-0.3.0/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)      551 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2099 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3586 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2168 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6124 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_core.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3336 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16489 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3961 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3726 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/layers/_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.779481 matgl-0.3.0/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      158 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11793 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/models/_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12277 2023-05-07 18:28:45.000000 matgl-0.3.0/matgl/models/_megnet.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.780836 matgl-0.3.0/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.3.0/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      809 2023-05-07 18:00:44.000000 matgl-0.3.0/matgl/utils/cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)    17696 2023-05-03 17:18:57.000000 matgl-0.3.0/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1916 2023-05-07 18:28:45.000000 matgl-0.3.0/matgl/utils/remote.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.3.0/matgl/utils/sb_roots.npy
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-07 20:32:51.775219 matgl-0.3.0/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)     8114 2023-05-07 20:32:51.000000 matgl-0.3.0/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)      972 2023-05-07 20:32:51.000000 matgl-0.3.0/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-05-07 20:32:51.000000 matgl-0.3.0/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       10 2023-05-07 20:32:51.000000 matgl-0.3.0/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-05-07 20:32:51.000000 matgl-0.3.0/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     3117 2023-05-07 18:00:44.000000 matgl-0.3.0/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)       38 2023-05-07 20:32:51.781270 matgl-0.3.0/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     2074 2023-05-02 13:08:40.000000 matgl-0.3.0/setup.py
```

### Comparing `matgl-0.2.1/LICENSE` & `matgl-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.2.1/PKG-INFO` & `matgl-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.2.1
+Version: 0.3.0
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
 Author-email: ongsp@eng.ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@eng.ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -115,15 +115,15 @@
 # Usage
 
 The pre-trained MEGNet models for the Materials Project formation energy and multi-fidelity band gap are now available.
 The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Structure, Lattice
-from matgl.models.megnet import MEGNet
+from matgl.models._megnet import MEGNet
 
 # load the pre-trained MEGNet model for formation energy model.
 model = MEGNet.load("MEGNet-MP-2018.6.1-Eform")
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.14), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):5f} eV/atom.")
```

### Comparing `matgl-0.2.1/README.md` & `matgl-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 # Usage
 
 The pre-trained MEGNet models for the Materials Project formation energy and multi-fidelity band gap are now available.
 The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Structure, Lattice
-from matgl.models.megnet import MEGNet
+from matgl.models._megnet import MEGNet
 
 # load the pre-trained MEGNet model for formation energy model.
 model = MEGNet.load("MEGNet-MP-2018.6.1-Eform")
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.14), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):5f} eV/atom.")
```

### Comparing `matgl-0.2.1/matgl/config.py` & `matgl-0.3.0/matgl/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,23 +4,114 @@
 import os
 from pathlib import Path
 
 import numpy as np
 import torch
 
 # CWD = os.path.dirname(os.path.abspath(__file__))
+DEFAULT_ELEMENT_TYPES = (
+    "H",
+    "He",
+    "Li",
+    "Be",
+    "B",
+    "C",
+    "N",
+    "O",
+    "F",
+    "Ne",
+    "Na",
+    "Mg",
+    "Al",
+    "Si",
+    "P",
+    "S",
+    "Cl",
+    "Ar",
+    "K",
+    "Ca",
+    "Sc",
+    "Ti",
+    "V",
+    "Cr",
+    "Mn",
+    "Fe",
+    "Co",
+    "Ni",
+    "Cu",
+    "Zn",
+    "Ga",
+    "Ge",
+    "As",
+    "Se",
+    "Br",
+    "Kr",
+    "Rb",
+    "Sr",
+    "Y",
+    "Zr",
+    "Nb",
+    "Mo",
+    "Tc",
+    "Ru",
+    "Rh",
+    "Pd",
+    "Ag",
+    "Cd",
+    "In",
+    "Sn",
+    "Sb",
+    "Te",
+    "I",
+    "Xe",
+    "Cs",
+    "Ba",
+    "La",
+    "Ce",
+    "Pr",
+    "Nd",
+    "Pm",
+    "Sm",
+    "Eu",
+    "Gd",
+    "Tb",
+    "Dy",
+    "Ho",
+    "Er",
+    "Tm",
+    "Yb",
+    "Lu",
+    "Hf",
+    "Ta",
+    "W",
+    "Re",
+    "Os",
+    "Ir",
+    "Pt",
+    "Au",
+    "Hg",
+    "Tl",
+    "Pb",
+    "Bi",
+    "Ac",
+    "Th",
+    "Pa",
+    "U",
+    "Np",
+    "Pu",
+)
 
 DTYPES = {
     "float32": {"numpy": np.float32, "torch": torch.float32},
     "float16": {"numpy": np.float16, "torch": torch.float16},
     "int32": {"numpy": np.int32, "torch": torch.int32},
     "int16": {"numpy": np.int16, "torch": torch.int16},
 }
 
-PRETRAINED_MODELS_PATH = Path(os.path.expanduser("~")) / ".matgl" / "models"
+MATGL_CACHE = Path(os.path.expanduser("~")) / ".matgl"
 PRETRAINED_MODELS_BASE_URL = "https://github.com/materialsvirtuallab/matgl/raw/main/pretrained_models/"
 
 
 class DataType:
     """
     Tensorflow and numpy data types. Used to choose between float16 and float32
     """
```

### Comparing `matgl-0.2.1/matgl/dataloader/dataset.py` & `matgl-0.3.0/matgl/graph/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 """
-Tools to construct a dataloader for DGL grphs
+Tools to construct a data for DGL grphs
 """
 from __future__ import annotations
 
 import json
 import os
 from typing import Callable
 
 import dgl
 import numpy as np
 import torch
 from dgl.data import DGLDataset
 from dgl.data.utils import load_graphs, save_graphs
 from dgl.dataloading import GraphDataLoader
-from pymatgen.core import Structure
 from tqdm import trange
 
 from matgl.graph.compute import compute_pair_vector_and_distance, create_line_graph
-from matgl.graph.converters import Pmg2Graph
-from matgl.layers.bond_expansion import BondExpansion
+from matgl.graph.converters import GraphConverter
+from matgl.layers import BondExpansion
 
 
 def _collate_fn(batch):
     """
     Merge a list of dgl graphs to form a batch
     """
-    graphs, labels, graph_attr = map(list, zip(*batch))
+    graphs, labels, state_attr = map(list, zip(*batch))
     g = dgl.batch(graphs)
     labels = torch.tensor(labels, dtype=torch.float32)
-    graph_attr = torch.stack(graph_attr)
-    return g, labels, graph_attr
+    state_attr = torch.stack(state_attr)
+    return g, labels, state_attr
 
 
 def _collate_fn_efs(batch):
     """
     Merge a list of dgl graphs to form a batch
     """
-    graphs, line_graphs, graph_attr, energies, forces, stresses = map(list, zip(*batch))
+    graphs, line_graphs, state_attr, energies, forces, stresses = map(list, zip(*batch))
     g = dgl.batch(graphs)
     l_g = dgl.batch(line_graphs)
     e = torch.tensor(energies, dtype=torch.float32)
     f = torch.vstack(forces)
     s = torch.vstack(stresses)
-    graph_attr = torch.stack(graph_attr)
-    return g, l_g, graph_attr, e, f, s
+    state_attr = torch.stack(state_attr)
+    return g, l_g, state_attr, e, f, s
 
 
 def MGLDataLoader(
     train_data: dgl.data.utils.Subset,
     val_data: dgl.data.utils.Subset,
     collate_fn: Callable,
     batch_size: int,
@@ -104,15 +103,15 @@
     """
 
     def __init__(
         self,
         structures: list,
         labels: list,
         label_name: str,
-        converter: Pmg2Graph,
+        converter: GraphConverter,
         initial: float = 0.0,
         final: float = 5.0,
         num_centers: int = 100,
         width: float = 0.5,
         name: str = "MEGNETDataset",
         graph_labels: list | None = None,
     ):
@@ -152,65 +151,62 @@
 
     def process(self) -> tuple:
         """
         Convert Pymatgen structure into dgl graphs
         """
         num_graphs = self.labels.shape[0]
         self.graphs = []
-        self.graph_attr = []
+        self.state_attr = []
         bond_expansion = BondExpansion(
             rbf_type="Gaussian", initial=self.initial, final=self.final, num_centers=self.num_centers, width=self.width
         )
         for idx in trange(num_graphs):
             structure = self.structures[idx]
-            if isinstance(structure, Structure):
-                graph, state_attr = self.converter.get_graph_from_structure(structure=structure)
-            else:
-                graph, state_attr = self.converter.get_graph_from_molecule(mol=structure)
+            graph, state_attr = self.converter.get_graph(structure)
             bond_vec, bond_dist = compute_pair_vector_and_distance(graph)
             graph.edata["edge_attr"] = bond_expansion(bond_dist)
             self.graphs.append(graph)
-            self.graph_attr.append(state_attr)
+            self.state_attr.append(state_attr)
         if self.graph_labels is not None:
             if np.array(self.graph_labels).dtype == "int64":
-                self.graph_attr = torch.tensor(self.graph_labels).long()  # type: ignore
+                self.state_attr = torch.tensor(self.graph_labels).long()  # type: ignore
             else:
-                self.graph_attr = torch.tensor(self.graph_labels)  # type: ignore
+                self.state_attr = torch.tensor(self.graph_labels)  # type: ignore
         else:
-            self.graph_attr = torch.tensor(self.graph_attr)  # type: ignore
+            self.state_attr = torch.tensor(self.state_attr)  # type: ignore
 
-        return self.graphs, self.graph_attr
+        return self.graphs, self.state_attr
 
-    def save(self, filename: str = "dgl_graph.bin", filename_graph_attr: str = "graph_attr.pt"):
+    def save(self, filename: str = "dgl_graph.bin", filename_state_attr: str = "state_attr.pt"):
         """
         Save dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
-        :filename_graph_attr: Name of file storing graph attrs
+        :filename_state_attr: Name of file storing graph attrs
         """
         labels_with_key = {self.label_name: self.labels}
         save_graphs(filename, self.graphs, labels_with_key)
-        torch.save(self.graph_attr, filename_graph_attr)
+        torch.save(self.state_attr, filename_state_attr)
 
-    def load(self, filename: str = "dgl_graph.bin", filename_graph_attr: str = "graph_attr.pt"):
+    def load(self, filename: str = "dgl_graph.bin", filename_state_attr: str = "state_attr.pt"):
         """
         Load dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
         :filename: Name of file storing state attrs
         """
         self.graphs, label_dict = load_graphs(filename)
         self.label = torch.stack([label_dict[key] for key in self.label_keys], dim=1)
-        self.graph_attr = torch.load("graph_attr.pt")
+        self.state_attr = torch.load("state_attr.pt")
 
     def __getitem__(self, idx: int):
         """
         Get graph and label with idx
         """
-        return self.graphs[idx], self.labels[idx], self.graph_attr[idx]
+        return self.graphs[idx], self.labels[idx], self.state_attr[idx]
 
     def __len__(self):
         """
         Get size of dataset
         """
         return len(self.graphs)
 
@@ -222,15 +218,15 @@
 
     def __init__(
         self,
         structures: list,
         energies: list,
         forces: list,
         stresses: None | list,
-        converter: Pmg2Graph,
+        converter: GraphConverter,
         threebody_cutoff: float,
         name="M3GNETDataset",
         graph_labels: list | None = None,
     ):
         """
         Args:
         structures: Pymatgen strutcure
@@ -263,86 +259,83 @@
     def process(self) -> tuple:
         """
         Convert Pymatgen structure into dgl graphs
         """
         num_graphs = len(self.energies)
         self.graphs = []
         self.line_graphs = []
-        self.graph_attr = []
+        self.state_attr = []
         for idx in trange(num_graphs):
             structure = self.structures[idx]
-            if isinstance(structure, Structure):
-                graph, state_attr = self.converter.get_graph_from_structure(structure=structure)
-            else:
-                graph, state_attr = self.converter.get_graph_from_molecule(mol=structure)
+            graph, state_attr = self.converter.get_graph(structure)
             self.graphs.append(graph)
-            self.graph_attr.append(state_attr)
+            self.state_attr.append(state_attr)
             bond_vec, bond_dist = compute_pair_vector_and_distance(graph)
             graph.edata["bond_vec"] = bond_vec
             graph.edata["bond_dist"] = bond_dist
             line_graph = create_line_graph(graph, self.threebody_cutoff)
             line_graph.ndata.pop("bond_vec")
             line_graph.ndata.pop("bond_dist")
             line_graph.ndata.pop("pbc_offset")
             self.line_graphs.append(line_graph)
         if self.graph_labels is not None:
-            self.graph_attr = torch.tensor(self.graph_labels).long()  # type: ignore
+            self.state_attr = torch.tensor(self.graph_labels).long()  # type: ignore
         else:
-            self.graph_attr = torch.tensor(self.graph_attr)  # type: ignore
+            self.state_attr = torch.tensor(self.state_attr)  # type: ignore
 
-        return self.graphs, self.line_graphs, self.graph_attr
+        return self.graphs, self.line_graphs, self.state_attr
 
     def save(
         self,
         filename: str = "dgl_graph.bin",
         filename_line_graph: str = "dgl_line_graph.bin",
-        filename_graph_attr: str = "graph_attr.pt",
+        filename_state_attr: str = "state_attr.pt",
     ):
         """
         Save dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
-        :filename_graph_attr: Name of file storing graph attrs
+        :filename_state_attr: Name of file storing graph attrs
         """
         labels_with_key = {"energies": self.energies, "forces": self.forces, "stresses": self.stresses}
         save_graphs(filename, self.graphs)
         save_graphs(filename_line_graph, self.line_graphs)
-        torch.save(self.graph_attr, filename_graph_attr)
+        torch.save(self.state_attr, filename_state_attr)
         with open("labels.json", "w") as file:
             file.write("".join(str(labels_with_key).split("\n")))
 
     def load(
         self,
         filename: str = "dgl_graph.bin",
         filename_line_graph: str = "dgl_line_graph.bin",
-        filename_graph_attr: str = "graph_attr.pt",
+        filename_state_attr: str = "state_attr.pt",
     ):
         """
         Load dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
         :filename: Name of file storing state attrs
         """
         self.graphs = load_graphs(filename)
         self.line_graphs = load_graphs(filename_line_graph)
         with open("labels.json") as file:
             labels = json.load(file)
         self.energies = labels["energies"]
         self.forces = labels["forces"]
         self.stresses = labels["stresses"]
-        self.graph_attr = torch.load("graph_attr.pt")
+        self.state_attr = torch.load("state_attr.pt")
 
     def __getitem__(self, idx: int):
         """
         Get graph and label with idx
         """
         return (
             self.graphs[idx],
             self.line_graphs[idx],
-            self.graph_attr[idx],
+            self.state_attr[idx],
             self.energies[idx],
             torch.tensor(self.forces[idx]),
             torch.tensor(self.stresses[idx]),
         )
 
     def __len__(self):
         """
```

### Comparing `matgl-0.2.1/matgl/graph/compute.py` & `matgl-0.3.0/matgl/graph/compute.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.1/matgl/graph/converters.py` & `matgl-0.3.0/matgl/ext/pymatgen.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
-Tools to convert materials representations from Pymatgen and other codes to DGLGraphs.
+Interface with pymatgen objects.
 """
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import scipy.sparse as sp
 import torch
-from ase import Atoms
 from dgl.backend import tensor
 from pymatgen.core import Element, Molecule, Structure
 from pymatgen.optimization.neighbors import find_points_in_spheres
 
+from matgl.graph.converters import GraphConverter
+
 
 def get_element_list(train_structures: list[Structure | Molecule]) -> tuple[str]:
     """Get the dictionary containing elements in the training set for atomic features
 
     Args:
         train_structures: pymatgen Molecule/Structure object
 
@@ -24,17 +25,17 @@
     """
     elements = set()
     for s in train_structures:
         elements.update(s.composition.get_el_amt_dict().keys())
     return tuple(sorted(elements, key=lambda el: Element(el).Z))  # type: ignore
 
 
-class Pmg2Graph:
+class Molecule2Graph(GraphConverter):
     """
-    Construct a DGL graph from Pymatgen Molecules or Structures, ASE atoms is also added.
+    Construct a DGL graph from Pymatgen Molecules.
     """
 
     def __init__(
         self,
         element_types: tuple[str, ...],
         cutoff: float = 5.0,
     ):
@@ -44,15 +45,15 @@
         element_types: List of elements present in dataset for graph conversion. This ensures all graphs are
             constructed with the same dimensionality of features.
         cutoff: Cutoff radius for graph representation
         """
         self.element_types = tuple(element_types)
         self.cutoff = cutoff
 
-    def get_graph_from_molecule(self, mol: Molecule) -> tuple[dgl.DGLGraph, list]:
+    def get_graph(self, mol: Molecule) -> tuple[dgl.DGLGraph, list]:
         """
         Get a DGL graph from an input molecule.
 
         :param mol: pymatgen molecule object
         :return: (dgl graph, state features)
         """
         natoms = len(mol)
@@ -76,15 +77,36 @@
         g.edata["pbc_offset"] = torch.zeros(g.num_edges(), 3)
         g.edata["lattice"] = torch.zeros(g.num_edges(), 3, 3)
         state_attr = [weight, nbonds]
         g.edata["pbc_offshift"] = torch.zeros(g.num_edges(), 3)
 
         return g, state_attr
 
-    def get_graph_from_structure(self, structure: Structure) -> tuple[dgl.DGLGraph, list]:
+
+class Structure2Graph(GraphConverter):
+    """
+    Construct a DGL graph from Pymatgen Structure.
+    """
+
+    def __init__(
+        self,
+        element_types: tuple[str, ...],
+        cutoff: float = 5.0,
+    ):
+        """
+        Parameters
+        ----------
+        element_types: List of elements present in dataset for graph conversion. This ensures all graphs are
+            constructed with the same dimensionality of features.
+        cutoff: Cutoff radius for graph representation
+        """
+        self.element_types = tuple(element_types)
+        self.cutoff = cutoff
+
+    def get_graph(self, structure: Structure) -> tuple[dgl.DGLGraph, list]:
         """
         Get a DGL graph from an input Structure.
 
         :param structure: pymatgen structure object
         :return:
             g: DGL graph
             state_attr: state features
@@ -119,52 +141,7 @@
         g.ndata["attr"] = tensor(Z)
         g.ndata["node_type"] = tensor(np.hstack([[element_types.index(site.specie.symbol)] for site in structure]))
         g.ndata["pos"] = tensor(cart_coords)
         g.ndata["volume"] = tensor([volume for i in range(atomic_number.shape[0])])
         state_attr = [0.0, 0.0]
         g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix))
         return g, state_attr
-
-    def get_graph_from_atoms(self, atoms: Atoms) -> tuple[dgl.DGLGraph, list]:
-        """
-        Get a DGL graph from an input Structure.
-
-        :param structure: pymatgen structure object
-        :return:
-            g: DGL graph
-            state_attr: state features
-        """
-
-        numerical_tol = 1.0e-8
-        pbc = np.array([1, 1, 1], dtype=int)
-        element_types = self.element_types
-        Z = np.array([np.eye(len(element_types))[element_types.index(i.symbol)] for i in atoms])
-        atomic_number = np.array(atoms.get_atomic_numbers())
-        lattice_matrix = np.ascontiguousarray(np.array(atoms.get_cell()), dtype=float)
-        volume = atoms.get_volume()
-        cart_coords = np.ascontiguousarray(np.array(atoms.get_positions()), dtype=float)
-        src_id, dst_id, images, bond_dist = find_points_in_spheres(
-            cart_coords,
-            cart_coords,
-            r=self.cutoff,
-            pbc=pbc,
-            lattice=lattice_matrix,
-            tol=numerical_tol,
-        )
-        exclude_self = (src_id != dst_id) | (bond_dist > numerical_tol)
-        src_id, dst_id, images, bond_dist = (
-            src_id[exclude_self],
-            dst_id[exclude_self],
-            images[exclude_self],
-            bond_dist[exclude_self],
-        )
-        u, v = tensor(src_id), tensor(dst_id)
-        g = dgl.graph((u, v))
-        g.edata["pbc_offset"] = torch.tensor(images)
-        g.edata["lattice"] = tensor([[lattice_matrix] for i in range(g.num_edges())])
-        g.ndata["attr"] = tensor(Z)
-        g.ndata["node_type"] = tensor(np.hstack([[element_types.index(i.symbol)] for i in atoms]))
-        g.ndata["pos"] = tensor(cart_coords)
-        g.ndata["volume"] = tensor([volume for i in range(atomic_number.shape[0])])
-        state_attr = [0.0, 0.0]
-        g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix))
-        return g, state_attr
```

### Comparing `matgl-0.2.1/matgl/layers/activations.py` & `matgl-0.3.0/matgl/layers/_activations.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.1/matgl/layers/atom_ref.py` & `matgl-0.3.0/matgl/layers/_atom_ref.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.1/matgl/layers/bond_expansion.py` & `matgl-0.3.0/matgl/layers/_bond.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.1/matgl/layers/core.py` & `matgl-0.3.0/matgl/layers/_core.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.1/matgl/layers/cutoff_functions.py` & `matgl-0.3.0/matgl/utils/cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.1/matgl/layers/embedding_block.py` & `matgl-0.3.0/matgl/layers/_embedding.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,58 +2,63 @@
 Embedding node, edge and optional state attributes
 """
 from __future__ import annotations
 
 import torch
 import torch.nn as nn
 
-from matgl.layers.core import MLP
+from ._core import MLP
 
 
 class EmbeddingBlock(nn.Module):
     """
     Embedding block for generating node, bond and state features
     """
 
     def __init__(
         self,
         degree_rbf: int,
         activation: nn.Module,
-        num_node_feats: int,
-        num_edge_feats: int,
-        num_node_types: int | None = None,
-        num_state_feats: int | None = None,
-        include_states: bool = False,
-        num_state_types: int | None = None,
-        state_embedding_dim: int | None = None,
+        dim_node_embedding: int,
+        dim_edge_embedding: int,
+        dim_state_feats: int | None = None,
+        ntypes_node: int | None = None,
+        include_state_embedding: bool = False,
+        ntypes_state: int | None = None,
+        dim_state_embedding: int | None = None,
     ):
         """
-        Parameters:
-        -----------
-        num_node_feats (int): dimensionality of node features
-        num_edge_feats (int): dimensionality of edge features
-        num_state_feats (int): dimensionality of state features
-        include_states (bool): whether including state for M3GNet or not
-        state_embedding_dim (int): dimensionality of state embedding
-        activation (str): activation function type
+
+        Args:
+            degree_rbf (int): number of rbf
+            activation (nn.Module): activation type
+            dim_node_embedding (int): dimensionality of node features
+            dim_edge_embedding (int): dimensionality of edge features
+            dim_state_feats: dimensionality of state features
+            ntypes_node: number of node labels
+            include_state_embedding: Whether to include state embedding
+            ntypes_state: number of state labels
+            dim_state_embedding: dimensionality of state embedding
         """
         super().__init__()
-        self.include_states = include_states
-        self.num_state_types = num_state_types
-        self.num_node_feats = num_node_feats
-        self.num_edge_feats = num_edge_feats
-        self.num_state_feats = num_state_feats
-        self.num_node_types = num_node_types
-        self.state_embedding_dim = state_embedding_dim
+        self.include_states = include_state_embedding
+        self.ntypes_state = ntypes_state
+        self.dim_node_embedding = dim_node_embedding
+        self.dim_edge_embedding = dim_edge_embedding
+        self.dim_state_feats = dim_state_feats
+        self.ntypes_node = ntypes_node
+        self.dim_state_embedding = dim_state_embedding
         self.activation = activation
-        if num_state_types and state_embedding_dim is not None:
-            self.state_embedding = nn.Embedding(num_state_types, state_embedding_dim)  # type: ignore
-        if num_node_types is not None:
-            self.node_embedding = nn.Embedding(num_node_types, num_node_feats)
-        self.edge_embedding = MLP([degree_rbf, self.num_edge_feats], activation=activation, activate_last=True)
+        if ntypes_state and dim_state_embedding is not None:
+            self.layer_state_embedding = nn.Embedding(ntypes_state, dim_state_embedding)  # type: ignore
+        if ntypes_node is not None:
+            self.layer_node_embedding = nn.Embedding(ntypes_node, dim_node_embedding)
+        self.layer_edge_embedding = MLP(
+            [degree_rbf, self.dim_edge_embedding], activation=activation, activate_last=True
+        )
 
     def forward(self, node_attr, edge_attr, state_attr):
         """
         Output embedded features
 
         Args:
         node_attr: node attribute
@@ -62,24 +67,24 @@
 
         Returns:
         node_feat: embedded node features
         edge_feat: embedded edge features
         state_feat: embedded state features
         """
 
-        if self.num_node_types is not None:
-            node_feat = self.node_embedding(node_attr)
+        if self.ntypes_node is not None:
+            node_feat = self.layer_node_embedding(node_attr)
         else:
-            node_embed = MLP([node_attr.shape[-1], self.num_node_feats], activation=self.activation)
+            node_embed = MLP([node_attr.shape[-1], self.dim_node_embedding], activation=self.activation)
             node_feat = node_embed(node_attr.to(torch.float32))
 
-        edge_feat = self.edge_embedding(edge_attr.to(torch.float32))
+        edge_feat = self.layer_edge_embedding(edge_attr.to(torch.float32))
         if self.include_states is True:
-            if self.num_state_types and self.state_embedding_dim is not None:
-                state_feat = self.state_embedding(state_attr)
+            if self.ntypes_state and self.dim_state_embedding is not None:
+                state_feat = self.layer_state_embedding(state_attr)
             else:
                 state_attr = torch.unsqueeze(state_attr, 0)
-                state_embed = MLP([state_attr.shape[-1], self.num_state_feats], activation=self.activation)
+                state_embed = MLP([state_attr.shape[-1], self.dim_state_feats], activation=self.activation)
                 state_feat = state_embed(state_attr.to(torch.float32))
         else:
             state_feat = None
         return node_feat, edge_feat, state_feat
```

### Comparing `matgl-0.2.1/matgl/layers/graph_conv.py` & `matgl-0.3.0/matgl/layers/_graph_convolution.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,59 +5,60 @@
 
 import dgl
 import dgl.function as fn
 import torch
 import torch.nn as nn
 from torch.nn import Dropout, Identity, Module
 
-from matgl.layers.core import MLP, GatedMLP
 from matgl.utils.maths import broadcast_states_to_bonds
 
+from ._core import MLP, GatedMLP
+
 
 class MEGNetGraphConv(Module):
     """
     A MEGNet graph convolution layer in DGL.
     """
 
     def __init__(
         self,
         edge_func: Module,
         node_func: Module,
-        attr_func: Module,
+        state_func: Module,
     ) -> None:
         """
         :param edge_func: Edge update function.
         :param node_func: Node update function.
-        :param attr_func: Global state update function.
+        :param state_func: Global state update function.
         """
         super().__init__()
         self.edge_func = edge_func
         self.node_func = node_func
-        self.attr_func = attr_func
+        self.state_func = state_func
 
     @staticmethod
     def from_dims(
         edge_dims: list[int],
         node_dims: list[int],
-        attr_dims: list[int],
+        state_dims: list[int],
         activation: Module,
     ) -> MEGNetGraphConv:
         """
         TODO: Add docs.
-        :param edge_dims:
-        :param node_dims:
-        :param attr_dims:
-        :param activation:
+        :param edge_dims: dense layers for message functions
+        :param node_dims: dense layers for node update functions
+        :param state_dims: dense layers for state update functions
+        :param activation: activation function
         :return:
         """
         # TODO(marcel): Softplus doesn't exactly match paper's SoftPlus2
         # TODO(marcel): Should we activate last?
         edge_update = MLP(edge_dims, activation, activate_last=True)
         node_update = MLP(node_dims, activation, activate_last=True)
-        attr_update = MLP(attr_dims, activation, activate_last=True)
+        attr_update = MLP(state_dims, activation, activate_last=True)
         return MEGNetGraphConv(edge_update, node_update, attr_update)
 
     def _edge_udf(self, edges: dgl.udf.EdgeBatch):
         vi = edges.src["v"]
         vj = edges.dst["v"]
         u = edges.src["u"]
         eij = edges.data.pop("e")
@@ -87,75 +88,76 @@
         ve = graph.ndata.pop("ve")
         v = graph.ndata.pop("v")
         u = graph.ndata.pop("u")
         inputs = torch.hstack([v, ve, u])
         graph.ndata["v"] = self.node_func(inputs)
         return graph.ndata["v"]
 
-    def attr_update_(self, graph: dgl.DGLGraph, attrs: torch.Tensor) -> torch.Tensor:
+    def state_update_(self, graph: dgl.DGLGraph, state_attrs: torch.Tensor) -> torch.Tensor:
         """
         Perform attribute (global state) update.
 
         :param graph: Input graph
-        :param attrs: Input attributes
+        :param state_attrs: Input attributes
         :return: Output tensor for attributes
         """
-        u = attrs
+        u = state_attrs
         ue = dgl.readout_edges(graph, feat="e", op="mean")
         uv = dgl.readout_nodes(graph, feat="v", op="mean")
         ue = torch.squeeze(ue)
         uv = torch.squeeze(uv)
         u = torch.squeeze(u)
         inputs = torch.hstack([u, ue, uv])
-        graph_attr = self.attr_func(inputs)
-        return graph_attr
+        state_attr = self.state_func(inputs)
+        return state_attr
 
     def forward(
         self,
         graph: dgl.DGLGraph,
         edge_feat: torch.Tensor,
         node_feat: torch.Tensor,
-        graph_attr: torch.Tensor,
+        state_attr: torch.Tensor,
     ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         """
         Perform sequence of edge->node->attribute updates.
 
         :param graph: Input graph
         :param edge_feat: Edge features
         :param node_feat: Node features
-        :param graph_attr: Graph attributes (global state)
+        :param state_attr: Graph attributes (global state)
         :return: (edge features, node features, graph attributes)
         """
         with graph.local_scope():
             graph.edata["e"] = edge_feat
             graph.ndata["v"] = node_feat
-            graph.ndata["u"] = dgl.broadcast_nodes(graph, graph_attr)
+            graph.ndata["u"] = dgl.broadcast_nodes(graph, state_attr)
 
             edge_feat = self.edge_update_(graph)
             node_feat = self.node_update_(graph)
-            graph_attr = self.attr_update_(graph, graph_attr)
+            state_attr = self.state_update_(graph, state_attr)
 
-        return edge_feat, node_feat, graph_attr
+        return edge_feat, node_feat, state_attr
 
 
 class MEGNetBlock(Module):
     """
     A MEGNet block comprising a sequence of update operations.
     """
 
     def __init__(
         self, dims: list[int], conv_hiddens: list[int], act: Module, dropout: float | None = None, skip: bool = True
     ) -> None:
         """
         TODO: Add docs.
-        :param dims:
-        :param conv_hiddens:
-        :param act:
-        :param dropout:
-        :param skip:
+        :param dims: architecture of dense layers before graph convolution
+        :param conv_hiddens: architecture of graph convolution
+        :param act: activation type
+        :param dropout: Randomly zeroes some elements in the input tensor with given probability (0 < x < 1) according
+            to a Bernoulli distribution
+        :param skip: residual block
         """
         super().__init__()
         self.has_dense = len(dims) > 1
         self.activation = act
         conv_dim = dims[-1]
         out_dim = conv_hiddens[-1]
 
@@ -163,79 +165,79 @@
             "dims": dims,
             "activation": self.activation,
             "activate_last": True,
             "bias_last": True,
         }
         self.edge_func = MLP(**mlp_kwargs) if self.has_dense else Identity()
         self.node_func = MLP(**mlp_kwargs) if self.has_dense else Identity()
-        self.attr_func = MLP(**mlp_kwargs) if self.has_dense else Identity()
+        self.state_func = MLP(**mlp_kwargs) if self.has_dense else Identity()
 
         # compute input sizes
         edge_in = 2 * conv_dim + conv_dim + conv_dim  # 2*NDIM+EDIM+GDIM
         node_in = out_dim + conv_dim + conv_dim  # EDIM+NDIM+GDIM
         attr_in = out_dim + out_dim + conv_dim  # EDIM+NDIM+GDIM
         self.conv = MEGNetGraphConv.from_dims(
             edge_dims=[edge_in, *conv_hiddens],
             node_dims=[node_in, *conv_hiddens],
-            attr_dims=[attr_in, *conv_hiddens],
+            state_dims=[attr_in, *conv_hiddens],
             activation=self.activation,
         )
 
         self.dropout = Dropout(dropout) if dropout else None
         # TODO(marcel): should this be an 1D dropout
         self.skip = skip
 
     def forward(
         self,
         graph: dgl.DGLGraph,
         edge_feat: torch.Tensor,
         node_feat: torch.Tensor,
-        graph_attr: torch.Tensor,
+        state_attr: torch.Tensor,
     ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         """
         TODO: Add docs.
         :param graph:
         :param edge_feat:
         :param node_feat:
-        :param graph_attr:
+        :param state_attr:
         :return:
         """
-        inputs = (edge_feat, node_feat, graph_attr)
+        inputs = (edge_feat, node_feat, state_attr)
         edge_feat = self.edge_func(edge_feat)
         node_feat = self.node_func(node_feat)
-        graph_attr = self.attr_func(graph_attr)
+        state_attr = self.state_func(state_attr)
 
-        edge_feat, node_feat, graph_attr = self.conv(graph, edge_feat, node_feat, graph_attr)
+        edge_feat, node_feat, state_attr = self.conv(graph, edge_feat, node_feat, state_attr)
 
         if self.dropout:
             edge_feat = self.dropout(edge_feat)  # pylint: disable=E1102
             node_feat = self.dropout(node_feat)  # pylint: disable=E1102
-            graph_attr = self.dropout(graph_attr)  # pylint: disable=E1102
+            state_attr = self.dropout(state_attr)  # pylint: disable=E1102
 
         if self.skip:
             edge_feat = edge_feat + inputs[0]
             node_feat = node_feat + inputs[1]
-            graph_attr = graph_attr + inputs[2]
+            state_attr = state_attr + inputs[2]
 
-        return edge_feat, node_feat, graph_attr
+        return edge_feat, node_feat, state_attr
 
 
 class M3GNetGraphConv(Module):
     """
     A M3GNet graph convolution layer in DGL.
     """
 
     def __init__(
         self,
         include_states: bool,
         edge_update_func: Module,
         edge_weight_func: Module,
         node_update_func: Module,
         node_weight_func: Module,
-        attr_update_func: Module | None,
+        state_update_func: Module | None,
     ):
         """
         Parameters:
         include_states (bool): Whether including state
         edge_update_func (Module): Update function for edges (Eq. 4)
         edge_weight_func (Module): Weight function for radial basis functions (Eq. 4)
         node_update_func (Module): Update function for nodes (Eq. 5)
@@ -244,23 +246,23 @@
         """
         super().__init__()
         self.include_states = include_states
         self.edge_update_func = edge_update_func
         self.edge_weight_func = edge_weight_func
         self.node_update_func = node_update_func
         self.node_weight_func = node_weight_func
-        self.attr_update_func = attr_update_func
+        self.state_update_func = state_update_func
 
     @staticmethod
     def from_dims(
         degree,
         include_states,
         edge_dims: list[int],
         node_dims: list[int],
-        attr_dims: list[int] | None,
+        state_dims: list[int] | None,
         activation: Module,
     ) -> M3GNetGraphConv:
         """
         M3GNetGraphConv initialization
 
         Args:
         degree (int): max_n*max_l
@@ -274,15 +276,15 @@
         M3GNetGraphConv (class)
         """
         edge_update_func = GatedMLP(in_feats=edge_dims[0], dims=edge_dims[1:])
         edge_weight_func = nn.Linear(in_features=degree, out_features=edge_dims[-1], bias=False)
 
         node_update_func = GatedMLP(in_feats=node_dims[0], dims=node_dims[1:])
         node_weight_func = nn.Linear(in_features=degree, out_features=node_dims[-1], bias=False)
-        attr_update_func = MLP(attr_dims, activation, activate_last=True) if include_states else None  # type: ignore
+        attr_update_func = MLP(state_dims, activation, activate_last=True) if include_states else None  # type: ignore
         return M3GNetGraphConv(
             include_states, edge_update_func, edge_weight_func, node_update_func, node_weight_func, attr_update_func
         )
 
     def _edge_udf(self, edges: dgl.udf.EdgeBatch):
         """
         Edge update functions
@@ -314,15 +316,15 @@
         Returns:
         edge_update: edge features update
         """
         graph.apply_edges(self._edge_udf)
         edge_update = graph.edata.pop("mij")
         return edge_update
 
-    def node_update_(self, graph: dgl.DGLGraph, graph_attr: torch.Tensor) -> torch.Tensor:
+    def node_update_(self, graph: dgl.DGLGraph, state_attr: torch.Tensor) -> torch.Tensor:
         """
         Perform node update.
 
         Args:
         graph: DGL graph
 
         Returns:
@@ -332,70 +334,70 @@
         src_id = graph.edges()[0]
         vi = graph.ndata["v"][src_id]
         dst_id = graph.edges()[1]
         vj = graph.ndata["v"][dst_id]
         rbf = graph.edata["rbf"]
         rbf = rbf.float()
         if self.include_states:
-            u = broadcast_states_to_bonds(graph, graph_attr)
+            u = broadcast_states_to_bonds(graph, state_attr)
             inputs = torch.hstack([vi, vj, eij, u])
         else:
             inputs = torch.hstack([vi, vj, eij])
         graph.edata["mess"] = self.node_update_func(inputs) * self.node_weight_func(rbf)
         graph.update_all(fn.copy_e("mess", "mess"), fn.sum("mess", "ve"))
         node_update = graph.ndata.pop("ve")
         return node_update
 
-    def attr_update_(self, graph: dgl.DGLGraph, attrs: torch.Tensor) -> torch.Tensor:
+    def state_update_(self, graph: dgl.DGLGraph, state_attrs: torch.Tensor) -> torch.Tensor:
         """
         Perform attribute (global state) update.
 
         Args:
         graph: DGL graph
         attrs: graph features
 
         Returns:
         state_update: state_features update
         """
-        u = attrs
+        u = state_attrs
         uv = dgl.readout_nodes(graph, feat="v", op="mean")
         inputs = torch.hstack([u, uv])
-        graph_attr = self.attr_update_func(inputs)  # type: ignore
-        return graph_attr
+        state_attr = self.state_update_func(inputs)  # type: ignore
+        return state_attr
 
     def forward(
         self,
         graph: dgl.DGLGraph,
         edge_feat: torch.Tensor,
         node_feat: torch.Tensor,
-        graph_attr: torch.Tensor,
+        state_attr: torch.Tensor,
     ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         """
         Perform sequence of edge->node->states updates.
 
         :param graph: Input graph
         :param edge_feat: Edge features
         :param node_feat: Node features
-        :param graph_attr: Graph attributes (global state)
+        :param state_attr: Graph attributes (global state)
         :return: (edge features, node features, graph attributes)
         """
         with graph.local_scope():
             graph.edata["e"] = edge_feat
             graph.ndata["v"] = node_feat
             if self.include_states:
-                graph.ndata["u"] = dgl.broadcast_nodes(graph, graph_attr)
+                graph.ndata["u"] = dgl.broadcast_nodes(graph, state_attr)
 
             edge_update = self.edge_update_(graph)
             graph.edata["e"] = edge_feat + edge_update
-            node_update = self.node_update_(graph, graph_attr)
+            node_update = self.node_update_(graph, state_attr)
             graph.ndata["v"] = node_feat + node_update
             if self.include_states:
-                graph_attr = self.attr_update_(graph, graph_attr)
+                state_attr = self.state_update_(graph, state_attr)
 
-        return edge_feat + edge_update, node_feat + node_update, graph_attr
+        return edge_feat + edge_update, node_feat + node_update, state_attr
 
 
 class M3GNetBlock(Module):
     """
     A M3GNet block comprising a sequence of update operations.
     """
 
@@ -430,46 +432,46 @@
             node_in = 2 * num_node_feats + num_edge_feats + num_state_feats  # type: ignore
             attr_in = num_node_feats + num_state_feats  # type: ignore
             self.conv = M3GNetGraphConv.from_dims(
                 degree,
                 include_states,
                 edge_dims=[edge_in, *conv_hiddens, num_edge_feats],
                 node_dims=[node_in, *conv_hiddens, num_node_feats],
-                attr_dims=[attr_in, *conv_hiddens, num_state_feats],  # type: ignore
+                state_dims=[attr_in, *conv_hiddens, num_state_feats],  # type: ignore
                 activation=self.activation,
             )
         else:
             edge_in = 2 * num_node_feats + num_edge_feats  # 2*NDIM+EDIM
             node_in = 2 * num_node_feats + num_edge_feats  # 2*NDIM+EDIM
             self.conv = M3GNetGraphConv.from_dims(
                 degree,
                 include_states,
                 edge_dims=[edge_in, *conv_hiddens] + [num_edge_feats],
                 node_dims=[node_in, *conv_hiddens] + [num_node_feats],
-                attr_dims=None,  # type: ignore
+                state_dims=None,  # type: ignore
                 activation=self.activation,
             )
 
         self.dropout = Dropout(dropout) if dropout else None
 
     def forward(
         self,
         graph: dgl.DGLGraph,
         edge_feat: torch.tensor,
         node_feat: torch.tensor,
-        graph_feat: torch.tensor,
+        state_feat: torch.tensor,
     ) -> tuple:
         """
         :param graph: DGL graph
         :param edge_feat: Edge features
         :param node_feat: Node features
-        :param graph_attr: State features
+        :param state_attr: State features
         :return: A tuple of updated features
         """
-        edge_feat, node_feat, graph_feat = self.conv(graph, edge_feat, node_feat, graph_feat)
+        edge_feat, node_feat, state_feat = self.conv(graph, edge_feat, node_feat, state_feat)
 
         if self.dropout:
             edge_feat = self.dropout(edge_feat)  # pylint: disable=E1102
             node_feat = self.dropout(node_feat)  # pylint: disable=E1102
-            graph_feat = self.dropout(graph_feat)  # pylint: disable=E1102
+            state_feat = self.dropout(state_feat)  # pylint: disable=E1102
 
-        return edge_feat, node_feat, graph_feat
+        return edge_feat, node_feat, state_feat
```

### Comparing `matgl-0.2.1/matgl/layers/readout_block.py` & `matgl-0.3.0/matgl/layers/_readout.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 import dgl
 import torch
 import torch.nn as nn
 from dgl.nn import Set2Set
 
-from matgl.layers.core import EdgeSet2Set, GatedMLP
+from ._core import EdgeSet2Set, GatedMLP
 
 
 class Set2SetReadOut(nn.Module):
     """
     The Set2Set readout function
     """
```

### Comparing `matgl-0.2.1/matgl/layers/three_body.py` & `matgl-0.3.0/matgl/layers/_three_body.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.1/matgl/models/ase_interface.py` & `matgl-0.3.0/matgl/ext/ase.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
-Dynamics calculations using M3GNet
+Interfaces to the Atomic Simulation Environment package for dynamic simulations.
 """
 
 from __future__ import annotations
 
 import contextlib
 import io
 import pickle
 import sys
 
+import dgl
 import numpy as np
 import torch
 from ase import Atoms, units
 from ase.calculators.calculator import Calculator, all_changes
 from ase.constraints import ExpCellFilter
 from ase.io import Trajectory
 from ase.md.nptberendsen import Inhomogeneous_NPTBerendsen, NPTBerendsen
@@ -20,43 +21,111 @@
 from ase.optimize.bfgs import BFGS
 from ase.optimize.bfgslinesearch import BFGSLineSearch
 from ase.optimize.fire import FIRE
 from ase.optimize.lbfgs import LBFGS, LBFGSLineSearch
 from ase.optimize.mdmin import MDMin
 from ase.optimize.optimize import Optimizer
 from ase.optimize.sciopt import SciPyFminBFGS, SciPyFminCG
+from dgl.backend import tensor
 from pymatgen.core.structure import Molecule, Structure
 from pymatgen.io.ase import AseAtomsAdaptor
+from pymatgen.optimization.neighbors import find_points_in_spheres
 
-from .potential import Potential
+from matgl.apps.pes import Potential
+from matgl.graph.converters import GraphConverter
 
 OPTIMIZERS = {
     "FIRE": FIRE,
     "BFGS": BFGS,
     "LBFGS": LBFGS,
     "LBFGSLineSearch": LBFGSLineSearch,
     "MDMin": MDMin,
     "SciPyFminCG": SciPyFminCG,
     "SciPyFminBFGS": SciPyFminBFGS,
     "BFGSLineSearch": BFGSLineSearch,
 }
 
 
+class Atoms2Graph(GraphConverter):
+    """
+    Construct a DGL graph from ASE atoms.
+    """
+
+    def __init__(
+        self,
+        element_types: tuple[str, ...],
+        cutoff: float = 5.0,
+    ):
+        """
+        Parameters
+        ----------
+        element_types: List of elements present in dataset for graph conversion. This ensures all graphs are
+            constructed with the same dimensionality of features.
+        cutoff: Cutoff radius for graph representation
+        """
+        self.element_types = tuple(element_types)
+        self.cutoff = cutoff
+
+    def get_graph(self, atoms: Atoms) -> tuple[dgl.DGLGraph, list]:
+        """
+        Get a DGL graph from an input Structure.
+
+        :param structure: pymatgen structure object
+        :return:
+            g: DGL graph
+            state_attr: state features
+        """
+
+        numerical_tol = 1.0e-8
+        pbc = np.array([1, 1, 1], dtype=int)
+        element_types = self.element_types
+        Z = np.array([np.eye(len(element_types))[element_types.index(i.symbol)] for i in atoms])
+        atomic_number = np.array(atoms.get_atomic_numbers())
+        lattice_matrix = np.ascontiguousarray(np.array(atoms.get_cell()), dtype=float)
+        volume = atoms.get_volume()
+        cart_coords = np.ascontiguousarray(np.array(atoms.get_positions()), dtype=float)
+        src_id, dst_id, images, bond_dist = find_points_in_spheres(
+            cart_coords,
+            cart_coords,
+            r=self.cutoff,
+            pbc=pbc,
+            lattice=lattice_matrix,
+            tol=numerical_tol,
+        )
+        exclude_self = (src_id != dst_id) | (bond_dist > numerical_tol)
+        src_id, dst_id, images, bond_dist = (
+            src_id[exclude_self],
+            dst_id[exclude_self],
+            images[exclude_self],
+            bond_dist[exclude_self],
+        )
+        u, v = tensor(src_id), tensor(dst_id)
+        g = dgl.graph((u, v))
+        g.edata["pbc_offset"] = torch.tensor(images)
+        g.edata["lattice"] = tensor([[lattice_matrix] for i in range(g.num_edges())])
+        g.ndata["attr"] = tensor(Z)
+        g.ndata["node_type"] = tensor(np.hstack([[element_types.index(i.symbol)] for i in atoms]))
+        g.ndata["pos"] = tensor(cart_coords)
+        g.ndata["volume"] = tensor([volume for i in range(atomic_number.shape[0])])
+        state_attr = [0.0, 0.0]
+        g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix))
+        return g, state_attr
+
+
 class M3GNetCalculator(Calculator):
     """
     M3GNet calculator based on ase Calculator
     """
 
     implemented_properties = ["energy", "free_energy", "forces", "stress", "hessian"]
 
     def __init__(
         self,
         potential: Potential,
-        graph_attr: torch.tensor = None,
-        compute_stress: bool = True,
+        state_attr: torch.tensor = None,
         stress_weight: float = 1.0,
         **kwargs,
     ):
         """
 
         Args:
             potential (Potential): m3gnet.models.Potential
@@ -65,15 +134,17 @@
             **kwargs:
         """
         super().__init__(**kwargs)
         self.potential = potential
         self.compute_stress = potential.calc_stresses
         self.compute_hessian = potential.calc_hessian
         self.stress_weight = stress_weight
-        self.graph_attr = graph_attr
+        self.state_attr = state_attr
+        self.element_types = potential.model.element_types
+        self.cutoff = potential.model.cutoff
 
     def calculate(
         self,
         atoms: Atoms | None = None,
         properties: list | None = None,
         system_changes: list | None = None,
     ):
@@ -86,19 +157,19 @@
                 results will be loaded.
         Returns:
 
         """
         properties = properties or ["energy"]
         system_changes = system_changes or all_changes
         super().calculate(atoms=atoms, properties=properties, system_changes=system_changes)
-        graph, graph_attr_default = self.potential.graph_converter.get_graph_from_atoms(atoms)
-        if self.graph_attr is not None:
-            energies, forces, stresses, hessians = self.potential(graph, self.graph_attr)
+        graph, state_attr_default = Atoms2Graph(self.element_types, self.cutoff).get_graph(atoms)  # type: ignore
+        if self.state_attr is not None:
+            energies, forces, stresses, hessians = self.potential(graph, self.state_attr)
         else:
-            energies, forces, stresses, hessians = self.potential(graph, graph_attr_default)
+            energies, forces, stresses, hessians = self.potential(graph, state_attr_default)
         self.results.update(
             energy=energies.detach().cpu().numpy(),
             free_energy=energies.detach().cpu().numpy(),
             forces=forces.detach().cpu().numpy(),
         )
         if self.compute_stress:
             self.results.update(stress=stresses.detach().cpu().numpy() * self.stress_weight)
@@ -110,15 +181,15 @@
     """
     Relaxer is a class for structural relaxation
     """
 
     def __init__(
         self,
         potential: Potential = None,
-        graph_attr: torch.tensor = None,
+        state_attr: torch.tensor = None,
         optimizer: Optimizer | str = "FIRE",
         relax_cell: bool = True,
         stress_weight: float = 0.01,
     ):
         """
 
         Args:
@@ -136,15 +207,15 @@
         elif optimizer is None:
             raise ValueError("Optimizer cannot be None")
         else:
             optimizer_obj = optimizer
 
         self.opt_class: Optimizer = optimizer_obj
         self.calculator = M3GNetCalculator(
-            potential=potential, graph_attr=graph_attr, stress_weight=stress_weight  # type: ignore
+            potential=potential, state_attr=state_attr, stress_weight=stress_weight  # type: ignore
         )
         self.relax_cell = relax_cell
         self.potential = potential
         self.ase_adaptor = AseAtomsAdaptor()
 
     def relax(
         self,
@@ -254,15 +325,15 @@
     Molecular dynamics class
     """
 
     def __init__(
         self,
         atoms: Atoms,
         potential: Potential,
-        graph_attr: torch.tensor = None,
+        state_attr: torch.tensor = None,
         ensemble: str = "nvt",
         temperature: int = 300,
         timestep: float = 1.0,
         pressure: float = 1.01325 * units.bar,
         taut: float | None = None,
         taup: float | None = None,
         compressibility_au: float | None = None,
@@ -290,15 +361,15 @@
             loginterval (int): write to log file every interval steps
             append_trajectory (bool): Whether to append to prev trajectory
         """
 
         if isinstance(atoms, (Structure, Molecule)):
             atoms = AseAtomsAdaptor().get_atoms(atoms)
         self.atoms = atoms
-        self.atoms.set_calculator(M3GNetCalculator(potential=potential, graph_attr=graph_attr))
+        self.atoms.set_calculator(M3GNetCalculator(potential=potential, state_attr=state_attr))
 
         if taut is None:
             taut = 100 * timestep * units.fs
         if taup is None:
             taup = 1000 * timestep * units.fs
 
         if ensemble.lower() == "nvt":
```

### Comparing `matgl-0.2.1/matgl/models/m3gnet.py` & `matgl-0.3.0/matgl/models/_m3gnet.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,32 +3,36 @@
 """
 from __future__ import annotations
 
 import logging
 import os
 
 import dgl
-import numpy as np
 import torch
 import torch.nn as nn
 
+from matgl.config import DEFAULT_ELEMENT_TYPES
 from matgl.graph.compute import (
     compute_pair_vector_and_distance,
     compute_theta_and_phi,
     create_line_graph,
 )
-from matgl.graph.converters import Pmg2Graph
-from matgl.layers.atom_ref import AtomRef
-from matgl.layers.bond_expansion import BondExpansion
-from matgl.layers.core import MLP, GatedMLP
-from matgl.layers.cutoff_functions import polynomial_cutoff
-from matgl.layers.embedding_block import EmbeddingBlock
-from matgl.layers.graph_conv import M3GNetBlock
-from matgl.layers.readout_block import ReduceReadOut, Set2SetReadOut, WeightedReadOut
-from matgl.layers.three_body import SphericalBesselWithHarmonics, ThreeBodyInteractions
+from matgl.layers import (
+    MLP,
+    BondExpansion,
+    EmbeddingBlock,
+    GatedMLP,
+    M3GNetBlock,
+    ReduceReadOut,
+    Set2SetReadOut,
+    SphericalBesselWithHarmonics,
+    ThreeBodyInteractions,
+    WeightedReadOut,
+)
+from matgl.utils.cutoff import polynomial_cutoff
 
 logger = logging.getLogger(__file__)
 CWD = os.path.dirname(os.path.abspath(__file__))
 
 MODEL_NAME = "m3gnet"
 
 MODEL_PATHS = {"MP-2021.2.8-EFS": os.path.join(CWD, "..", "..", "pretrained_models", "MP-2021.2.8-EFS")}
@@ -38,75 +42,70 @@
     """
     The main M3GNet model
     """
 
     def __init__(
         self,
         element_types: tuple[str],
-        num_node_feats: int = 64,
-        num_edge_feats: int = 64,
-        num_state_feats: int | None = None,
-        num_node_types: int | None = None,
-        num_state_types: int | None = None,
-        state_embedding_dim: int | None = None,
+        dim_node_embedding: int = 64,
+        dim_edge_embedding: int = 64,
+        dim_state_embedding: int | None = None,
+        dim_state_types: int | None = None,
+        dim_state_feats: int | None = None,
         max_n: int = 3,
         max_l: int = 3,
-        n_blocks: int = 3,
+        nblocks: int = 3,
         rbf_type="SphericalBessel",
         is_intensive: bool = True,
         readout_type: str = "weighted_atom",
         task_type: str = "regression",
         cutoff: float = 5.0,
         threebody_cutoff: float = 4.0,
         units: int = 64,
         data_mean: float = 0.0,
         data_std: float = 1.0,
-        num_targets: int = 1,
+        ntargets: int = 1,
         use_smooth: bool = False,
         use_phi: bool = False,
-        num_s2s_steps: int = 3,
-        num_s2s_layers: int = 3,
+        niters_set2set: int = 3,
+        nlayers_set2set: int = 3,
         field: str = "node_feat",
-        include_states: bool = False,
-        element_refs: np.ndarray | None = None,
+        include_state_embedding: bool = False,
         activation: str = "swish",
         **kwargs,
     ):
         r"""
         Args:
             element_types (tuple): list of elements appearing in the dataset
-            num_node_feats (int): number of atomic features
-            num_edge_feats (int): number of edge features
-            num_state_feats (int): number of state features
-            num_node_types (int): number of node types
-            num_state_types (int): number of state labels
-            state_embedding_dim (int): number of hidden neeurons in state embedding
+            dim_node_embedding (int): number of embedded atomic features
+            dim_edge_embedding (int): number of edge features
+            dim_state_embedding (int): number of hidden neurons in state embedding
+            dim_state_feats (int): number of state features after linear layer
+            dim_state_types (int): number of state labels
             max_n (int): number of radial basis expansion
             max_l (int): number of angular expansion
-            n_blocks (int): number of convolution blocks
+            nblocks (int): number of convolution blocks
             rbf_type (str): radial basis function. choose from 'Gaussian' or 'SphericalBessel'
             is_intensive (bool): whether the prediction is intensive
             readout (str): the readout function type. choose from `set2set`,
                 `weighted_atom` and `reduce_atom`, default to `weighted_atom`
             task_type (str): `classification` or `regression`, default to
                 `regression`
             cutoff (float): cutoff radius of the graph
             threebody_cutoff (float): cutoff radius for 3 body interaction
             units (int): number of neurons in each MLP layer
             data_mean (float): optional `mean` value of the target
             data_std (float): optional `std` of the target
-            num_targets (int): number of target properties
+            ntargets (int): number of target properties
             use_smooth (bool): whether using smooth Bessel functions
             use_phi (bool): whether using phi angle
             field (str): using either "node_feat" or "edge_feat" for Set2Set and Reduced readout
-            num_s2s_steps (int): number of set2set iterations
-            num_s2s_layers (int): number of set2set layers
-            include_states (bool): whether to include states features
-            element_refs (np.ndarray): element reference values for each
-                element
+            niters_set2set (int): number of set2set iterations
+            nlayers_set2set (int): number of set2set layers
+            include_state_embedding (bool): whether to include states features
             activation (str): activation type. choose from 'swish', 'tanh', 'sigmoid'
             **kwargs:
         """
 
         # Store M3GNet model args for loading trained model
         self.model_args = {k: v for k, v in locals().items() if k not in ["self", "__class__", "kwargs"]}
         self.model_args.update(kwargs)
@@ -116,96 +115,99 @@
         if activation == "swish":
             self.activation = nn.SiLU()  # type: ignore
         elif activation == "tanh":
             self.activation = nn.Tanh()  # type: ignore
         elif activation == "sigmoid":
             self.activation = nn.Sigmoid()  # type: ignore
 
-        self.graph_converter = Pmg2Graph(element_types=element_types, cutoff=cutoff)
+        if element_types is None:
+            self.element_types = DEFAULT_ELEMENT_TYPES
+        else:
+            self.element_types = element_types  # type: ignore
 
         self.bond_expansion = BondExpansion(max_l, max_n, cutoff, rbf_type=rbf_type, smooth=use_smooth)
 
         degree = max_n * max_l * max_l if use_phi else max_n * max_l
 
         degree_rbf = max_n if use_smooth else max_n * max_l
 
-        if num_node_types is None:
-            num_node_types = len(element_types)
-
         self.embedding = EmbeddingBlock(
             degree_rbf=degree_rbf,
-            num_node_feats=num_node_feats,
-            num_edge_feats=num_edge_feats,
-            num_node_types=num_node_types,
-            num_state_feats=num_state_feats,
-            include_states=include_states,
-            state_embedding_dim=state_embedding_dim,
+            dim_node_embedding=dim_node_embedding,
+            dim_edge_embedding=dim_edge_embedding,
+            ntypes_node=len(element_types),
+            dim_state_feats=dim_state_feats,
+            include_state_embedding=include_state_embedding,
+            dim_state_embedding=dim_state_embedding,
             activation=self.activation,
         )
 
         self.basis_expansion = SphericalBesselWithHarmonics(
             max_n=max_n, max_l=max_l, cutoff=cutoff, use_phi=use_phi, use_smooth=use_smooth
         )
         self.three_body_interactions = nn.ModuleList(
             {
                 ThreeBodyInteractions(
-                    update_network_atom=MLP(dims=[num_node_feats, degree], activation=nn.Sigmoid(), activate_last=True),
-                    update_network_bond=GatedMLP(in_feats=degree, dims=[num_edge_feats], use_bias=False),
+                    update_network_atom=MLP(
+                        dims=[dim_node_embedding, degree], activation=nn.Sigmoid(), activate_last=True
+                    ),
+                    update_network_bond=GatedMLP(in_feats=degree, dims=[dim_edge_embedding], use_bias=False),
                 )
-                for _ in range(n_blocks)
+                for _ in range(nblocks)
             }
         )
 
         self.graph_layers = nn.ModuleList(
             {
                 M3GNetBlock(
                     degree=degree_rbf,
                     activation=self.activation,
                     conv_hiddens=[units, units],
-                    num_node_feats=num_node_feats,
-                    num_edge_feats=num_edge_feats,
-                    num_state_feats=num_state_feats,
-                    include_states=include_states,
+                    num_node_feats=dim_node_embedding,
+                    num_edge_feats=dim_edge_embedding,
+                    num_state_feats=dim_state_feats,
+                    include_states=include_state_embedding,
                 )
-                for _ in range(n_blocks)
+                for _ in range(nblocks)
             }
         )
         if is_intensive:
-            input_feats = num_node_feats if field == "node_feat" else num_edge_feats
+            input_feats = dim_node_embedding if field == "node_feat" else dim_edge_embedding
             if readout_type == "set2set":
-                self.readout = Set2SetReadOut(num_steps=num_s2s_steps, num_layers=num_s2s_layers, field=field)
-                readout_feats = 2 * input_feats + num_state_feats if include_states else 2 * input_feats  # type: ignore
+                self.readout = Set2SetReadOut(num_steps=niters_set2set, num_layers=nlayers_set2set, field=field)
+                readout_feats = (
+                    2 * input_feats + dim_state_feats if include_state_embedding else 2 * input_feats  # type: ignore
+                )
             else:
                 self.readout = ReduceReadOut("mean", field=field)
-                readout_feats = input_feats + num_state_feats if include_states else input_feats  # type: ignore
+                readout_feats = (
+                    input_feats + dim_state_feats if include_state_embedding else input_feats  # type: ignore
+                )
 
-            dims_final_layer = [readout_feats] + [units, units] + [num_targets]
+            dims_final_layer = [readout_feats] + [units, units] + [ntargets]
             self.final_layer = MLP(dims_final_layer, self.activation, activate_last=False)
             if task_type == "classification":
                 self.sigmoid = nn.Sigmoid()
 
         else:
             if task_type == "classification":
                 raise ValueError("Classification task cannot be extensive")
-            self.final_layer = WeightedReadOut(in_feats=num_node_feats, dims=[units, units], num_targets=num_targets)
-        if element_refs is not None:
-            self.element_ref_calc = AtomRef(property_offset=element_refs)
+            self.final_layer = WeightedReadOut(in_feats=dim_node_embedding, dims=[units, units], num_targets=ntargets)
 
         self.max_n = max_n
         self.max_l = max_l
-        self.n_blocks = n_blocks
+        self.n_blocks = nblocks
         self.units = units
         self.cutoff = cutoff
         self.threebody_cutoff = threebody_cutoff
-        self.include_states = include_states
+        self.include_states = include_state_embedding
         self.task_type = task_type
         self.is_intensive = is_intensive
         self.data_mean = data_mean
         self.data_std = data_std
-        self.element_refs = element_refs
 
     def as_dict(self):
         out = {"state_dict": self.state_dict(), "model_args": self.model_args}
         return out
 
     @classmethod
     def from_dict(cls, dict, **kwargs):
@@ -293,12 +295,8 @@
             output = self.final_layer(vec)
             if self.task_type == "classification":
                 output = self.sigmoid(output)
         else:
             g.ndata["atomic_properties"] = self.final_layer(g)
             output = dgl.readout_nodes(g, "atomic_properties", op="sum")
         output = output * self.data_std + self.data_mean
-        output = torch.squeeze(output)
-        if self.element_refs is not None:
-            property_offset = torch.squeeze(self.element_ref_calc(g))
-            output += property_offset
-        return output
+        return torch.squeeze(output)
```

### Comparing `matgl-0.2.1/matgl/models/megnet.py` & `matgl-0.3.0/matgl/models/_megnet.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,208 +8,112 @@
 
 import dgl
 import torch
 import torch.nn as nn
 from dgl.nn import Set2Set
 from pymatgen.core import Structure
 
-from matgl.config import PRETRAINED_MODELS_BASE_URL, PRETRAINED_MODELS_PATH
+from matgl.config import DEFAULT_ELEMENT_TYPES, MATGL_CACHE, PRETRAINED_MODELS_BASE_URL
+from matgl.ext.pymatgen import Structure2Graph
 from matgl.graph.compute import compute_pair_vector_and_distance
-from matgl.graph.converters import Pmg2Graph
-from matgl.layers.activations import SoftExponential, SoftPlus2
-from matgl.layers.bond_expansion import BondExpansion
-from matgl.layers.core import MLP, EdgeSet2Set
-from matgl.layers.graph_conv import MEGNetBlock
-from matgl.utils.data import ModelSource
+from matgl.graph.converters import GraphConverter
+from matgl.layers import MLP, BondExpansion, EdgeSet2Set, MEGNetBlock, SoftExponential, SoftPlus2
+from matgl.utils.remote import RemoteFile
 
 logger = logging.getLogger(__file__)
 
-DEFAULT_ELEMENT_TYPES = (
-    "H",
-    "He",
-    "Li",
-    "Be",
-    "B",
-    "C",
-    "N",
-    "O",
-    "F",
-    "Ne",
-    "Na",
-    "Mg",
-    "Al",
-    "Si",
-    "P",
-    "S",
-    "Cl",
-    "Ar",
-    "K",
-    "Ca",
-    "Sc",
-    "Ti",
-    "V",
-    "Cr",
-    "Mn",
-    "Fe",
-    "Co",
-    "Ni",
-    "Cu",
-    "Zn",
-    "Ga",
-    "Ge",
-    "As",
-    "Se",
-    "Br",
-    "Kr",
-    "Rb",
-    "Sr",
-    "Y",
-    "Zr",
-    "Nb",
-    "Mo",
-    "Tc",
-    "Ru",
-    "Rh",
-    "Pd",
-    "Ag",
-    "Cd",
-    "In",
-    "Sn",
-    "Sb",
-    "Te",
-    "I",
-    "Xe",
-    "Cs",
-    "Ba",
-    "La",
-    "Ce",
-    "Pr",
-    "Nd",
-    "Pm",
-    "Sm",
-    "Eu",
-    "Gd",
-    "Tb",
-    "Dy",
-    "Ho",
-    "Er",
-    "Tm",
-    "Yb",
-    "Lu",
-    "Hf",
-    "Ta",
-    "W",
-    "Re",
-    "Os",
-    "Ir",
-    "Pt",
-    "Au",
-    "Hg",
-    "Tl",
-    "Pb",
-    "Bi",
-    "Ac",
-    "Th",
-    "Pa",
-    "U",
-    "Np",
-    "Pu",
-)
-
 
 class MEGNet(nn.Module):
     """
     DGL implementation of MEGNet.
     """
 
     def __init__(
         self,
         dim_node_embedding: int = 16,
         dim_edge_embedding: int = 100,
-        dim_attr_embedding: int = 2,
+        dim_state_embedding: int = 2,
         nblocks: int = 3,
         hidden_layer_sizes_input: tuple[int, ...] = (64, 32),
         hidden_layer_sizes_conv: tuple[int, ...] = (64, 64, 32),
         hidden_layer_sizes_output: tuple[int, ...] = (32, 16),
         nlayers_set2set: int = 1,
         niters_set2set: int = 2,
         activation_type: str = "softplus2",
         is_classification: bool = False,
         layer_node_embedding: nn.Module | None = None,
         layer_edge_embedding: nn.Module | None = None,
-        layer_attr_embedding: nn.Module | None = None,
+        layer_state_embedding: nn.Module | None = None,
         include_state_embedding: bool = False,
         dropout: float | None = None,
         graph_transformations: list | None = None,
         element_types: tuple[str, ...] | None = None,
         data_mean: torch.tensor | None = None,
         data_std: torch.tensor | None = None,
-        graph_converter: Pmg2Graph | None = None,
         bond_expansion: BondExpansion | None = None,
         cutoff: float = 4.0,
         gauss_width: float = 0.5,
         **kwargs,
-    ) -> None:
+    ):
         """
         Construct a MEGNet model. Useful defaults for all arguments have been specified based on MEGNet formation energy
         model.
 
         Args:
             dim_node_embedding: Dimension of node embedding.
             dim_edge_embedding: Dimension of edge embedding.
-            dim_attr_embedding: Dimension of attr (global state) embedding.
+            dim_state_embedding: Dimension of state embedding.
             nblocks: Number of blocks.
             hidden_layer_sizes_input: Architecture of dense layers before the graph convolution
             hidden_layer_sizes_conv: Architecture of dense layers for message and update functions
             nlayers_set2set: Number of layers in Set2Set layer
             niters_set2set: Number of iteratons in Set2Set layer
             hidden_layer_sizes_output: Architecture of dense layers for concatenated features after graph convolution
             activation_types: Activation used for non-linearity
             is_classification: Whether this is classification task or not
             layer_node_embedding: Architecture of embedding layer for node attributes
             layer_edge_embedding: Architecture of embedding layer for edge attributes
-            layer_attr_embedding: Architecture of embedding layer for state attributes
+            layer_state_embedding: Architecture of embedding layer for state attributes
             include_state_embedding: Whether the state embedding is included
             dropout: Randomly zeroes some elements in the input tensor with given probability (0 < x < 1) according to
                 a Bernoulli distribution
             graph_transformations: Perform a graph transformation, e.g., incorporate three-body interactions, prior to
                 performing the GCL updates.
             element_types: Elements included in the training set
             data_mean: Mean of target properties in the training set. Defaults to 0.
             data_std: Standard deviation of target properties in the training set. Defaults to 1.
-            graph_converter: Pmg2Graph converter
             bond_expansion: Gaussian expansion for edge attributes
             cutoff: cutoff for forming bonds
             gauss_width: width of Gaussian function for bond expansion
             **kwargs:
         """
         # Store MEGNet model args for loading trained model
         self.model_args = {k: v for k, v in locals().items() if k not in ["self", "__class__", "kwargs"]}
         self.model_args.update(kwargs)
 
         super().__init__()
 
         self.element_types = element_types or DEFAULT_ELEMENT_TYPES
-        self.graph_converter = graph_converter or Pmg2Graph(element_types=self.element_types, cutoff=cutoff)
+        self.cutoff = cutoff
         self.bond_expansion = bond_expansion or BondExpansion(
             rbf_type="Gaussian", initial=0.0, final=cutoff + 1.0, num_centers=dim_edge_embedding, width=gauss_width
         )
         self.data_mean = data_mean or torch.zeros(1)
         self.data_std = data_std or torch.ones(1)
 
-        self.edge_embedding_layer = layer_edge_embedding if layer_edge_embedding else nn.Identity()
+        self.layer_edge_embedding = layer_edge_embedding if layer_edge_embedding else nn.Identity()
         if layer_node_embedding is None:
-            self.node_embedding_layer = nn.Embedding(len(self.element_types), dim_node_embedding)
+            self.layer_node_embedding = nn.Embedding(len(self.element_types), dim_node_embedding)
         else:
-            self.node_embedding_layer = layer_node_embedding
-        self.attr_embedding_layer = layer_attr_embedding or nn.Identity()
+            self.layer_node_embedding = layer_node_embedding
+        self.layer_state_embedding = layer_state_embedding or nn.Identity()
 
         node_dims = [dim_node_embedding, *hidden_layer_sizes_input]
         edge_dims = [dim_edge_embedding, *hidden_layer_sizes_input]
-        attr_dims = [dim_attr_embedding, *hidden_layer_sizes_input]
+        state_dims = [dim_state_embedding, *hidden_layer_sizes_input]
 
         if activation_type == "swish":
             activation = nn.SiLU()  # type: ignore
         elif activation_type == "sigmoid":
             activation = nn.Sigmoid()  # type: ignore
         elif activation_type == "tanh":
             activation = nn.Tanh()  # type: ignore
@@ -218,15 +122,15 @@
         elif activation_type == "softexp":
             activation = SoftExponential()  # type: ignore
         else:
             raise Exception("Undefined activation type, please try using swish, sigmoid, tanh, softplus2, softexp")
 
         self.edge_encoder = MLP(edge_dims, activation, activate_last=True)
         self.node_encoder = MLP(node_dims, activation, activate_last=True)
-        self.attr_encoder = MLP(attr_dims, activation, activate_last=True)
+        self.state_encoder = MLP(state_dims, activation, activate_last=True)
 
         dim_blocks_in = hidden_layer_sizes_input[-1]
         dim_blocks_out = hidden_layer_sizes_conv[-1]
         block_args = {
             "conv_hiddens": hidden_layer_sizes_conv,
             "dropout": dropout,
             "act": activation,
@@ -257,71 +161,79 @@
         self.include_state_embedding = include_state_embedding
 
     def forward(
         self,
         graph: dgl.DGLGraph,
         edge_feat: torch.Tensor,
         node_feat: torch.Tensor,
-        graph_attr: torch.Tensor,
+        state_feat: torch.Tensor,
     ):
         """
         Forward pass of MEGnet. Executes all blocks.
 
         :param graph: Input graph
         :param edge_feat: Edge features
         :param node_feat: Node features
-        :param graph_attr: Graph attributes / state features.
+        :param state_feat: State features.
         :return: Prediction
         """
         graph_transformations = self.graph_transformations
-        edge_feat = self.edge_encoder(self.edge_embedding_layer(edge_feat))
-        node_feat = self.node_encoder(self.node_embedding_layer(node_feat))
+        edge_feat = self.edge_encoder(self.layer_edge_embedding(edge_feat))
+        node_feat = self.node_encoder(self.layer_node_embedding(node_feat))
         if self.include_state_embedding:
-            graph_attr = self.attr_encoder(self.attr_embedding_layer(graph_attr))
+            state_feat = self.state_encoder(self.layer_state_embedding(state_feat))
         else:
-            graph_attr = self.attr_encoder(graph_attr)
+            state_feat = self.state_encoder(state_feat)
 
         for gt, block in zip(graph_transformations, self.blocks):
-            output = block(gt(graph), edge_feat, node_feat, graph_attr)
-            edge_feat, node_feat, graph_attr = output
+            output = block(gt(graph), edge_feat, node_feat, state_feat)
+            edge_feat, node_feat, state_feat = output
 
         node_vec = self.node_s2s(graph, node_feat)
         edge_vec = self.edge_s2s(graph, edge_feat)
 
         node_vec = torch.squeeze(node_vec)
         edge_vec = torch.squeeze(edge_vec)
-        graph_attr = torch.squeeze(graph_attr)
+        state_feat = torch.squeeze(state_feat)
 
-        vec = torch.hstack([node_vec, edge_vec, graph_attr])
+        vec = torch.hstack([node_vec, edge_vec, state_feat])
 
         if self.dropout:
             vec = self.dropout(vec)  # pylint: disable=E1102
 
         output = self.output_proj(vec)
         if self.is_classification:
             output = torch.sigmoid(output)
 
         return output
 
-    def predict_structure(self, structure: Structure, attrs: torch.tensor | None = None):
+    def predict_structure(
+        self,
+        structure: Structure,
+        state_feats: torch.tensor | None = None,
+        graph_converter: GraphConverter | None = None,
+    ):
         """
         Convenience method to directly predict property from structure.
         Args:
             structure (Structure): Pymatgen structure
-            attrs (torch.tensor): graph attributes
+            state_feats (torch.tensor): graph attributes
+            graph_converter: Object that implements a get_graph_from_structure.
         Returns:
             output (torch.tensor): output property
         """
-        g, attrs_default = self.graph_converter.get_graph_from_structure(structure)
-        if attrs is None:
-            attrs = torch.tensor(attrs_default)
+        if graph_converter is None:
+            graph_converter = Structure2Graph(element_types=self.element_types, cutoff=self.cutoff)
+        g, state_feats_default = graph_converter.get_graph(structure)
+        if state_feats is None:
+            state_feats = torch.tensor(state_feats_default)
         bond_vec, bond_dist = compute_pair_vector_and_distance(g)
         g.edata["edge_attr"] = self.bond_expansion(bond_dist)
 
-        output = self.data_std * self(g, g.edata["edge_attr"], g.ndata["node_type"], attrs) + self.data_mean
+        output = self.data_std * self(g, g.edata["edge_attr"], g.ndata["node_type"], state_feats) + self.data_mean
 
         return output.detach()
 
     def as_dict(self):
         out = {"state_dict": self.state_dict(), "model_args": self.model_args}
         return out
 
@@ -330,48 +242,51 @@
         """
         build a MEGNet from a saved dictionary
         """
         model = MEGNet(**dict["model_args"])
         model.load_state_dict(dict["state_dict"], **kwargs)
         return model
 
-    @classmethod
-    def from_dir(cls, path: str | Path, **kwargs):
-        """
-        build a MEGNet from a saved directory
-        """
+    def save(self, path: str | Path):
         path = Path(path)
-        if torch.cuda.is_available() is False:
-            state = torch.load(path, map_location=torch.device("cpu"))
-        else:
-            state = torch.load(path)
-        model = MEGNet.from_dict(state["model"], strict=False, **kwargs)
-        return model
+        torch.save(self.model_args, path / "model.pt")
+        torch.save(self.state_dict(), path / "state.pt")
 
     @classmethod
-    def load(cls, model_path: str | Path) -> MEGNet:
+    def load(cls, path: str | Path) -> MEGNet:
         """
-        Load the model weights from pre-trained model (MEGNet-MP-2018.6.1-Eform.pt)
+        Load the model weights from a directory.
+
         Args:
-            model_path (str): Path to saved model or name of pre-trained model. The search order is
-                model_path, followed by model name in PRETRAINED_MODELS_PATH, followed by download from
+            path (str|path): Path to saved model or name of pre-trained model. The search order is
+                path, followed by model name in PRETRAINED_MODELS_PATH, followed by download from
                 PRETRAINED_MODELS_BASE_URL.
 
         Returns: MEGNet object.
         """
-        model_path = Path(model_path)
-
-        try:
-            return cls.from_dir(model_path)
-        except FileNotFoundError:
-            if (PRETRAINED_MODELS_PATH / f"{model_path}.pt").exists():
-                model_path = PRETRAINED_MODELS_PATH / f"{model_path}.pt"
-                return cls.from_dir(model_path)
-
+        path = Path(path)
+        if (path / "model.pt").exists() and (path / "state.pt").exists():
+            model_path = path / "model.pt"
+            state_path = path / "state.pt"
+        elif (MATGL_CACHE / path / "model.pt").exists() and (MATGL_CACHE / path / "state.pt").exists():
+            model_path = MATGL_CACHE / path / "model.pt"
+            state_path = MATGL_CACHE / path / "state.pt"
+        else:
             try:
-                source = ModelSource(f"{PRETRAINED_MODELS_BASE_URL}{model_path}.pt")
-                return cls.from_dir(source.local_path)
+                model_file = RemoteFile(f"{PRETRAINED_MODELS_BASE_URL}{path}/model.pt")
+                state_file = RemoteFile(f"{PRETRAINED_MODELS_BASE_URL}{path}/state.pt")
+                model_path = model_file.local_path
+                state_path = state_file.local_path
             except BaseException:
                 raise ValueError(
                     f"No valid model found in {model_path} or among pre-trained_models at "
-                    f"{PRETRAINED_MODELS_PATH} or {PRETRAINED_MODELS_BASE_URL}."
+                    f"{MATGL_CACHE} or {PRETRAINED_MODELS_BASE_URL}."
                 )
+
+        if not torch.cuda.is_available():
+            state = torch.load(state_path, map_location=torch.device("cpu"))
+        else:
+            state = torch.load(state_path)
+        model_args = torch.load(model_path)
+        model = cls(**model_args)
+        model.load_state_dict(state)
+        return model
```

### Comparing `matgl-0.2.1/matgl/models/potential.py` & `matgl-0.3.0/matgl/apps/pes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,70 @@
 """
-M3GNet potentials
+Implementation of Interatomic Potentials
 """
 from __future__ import annotations
 
 import dgl
+import numpy as np
 import torch
 import torch.nn as nn
 from torch.autograd import grad
 
+from matgl.layers import AtomRef
+
 
 class Potential(nn.Module):
     """
-    A M3GNet potential class.
+    A class representing an interatomic potential.
     """
 
     def __init__(
         self,
         model: nn.Module,
+        element_refs: np.ndarray | None = None,
         calc_forces: bool = True,
         calc_stresses: bool = True,
         calc_hessian: bool = False,
     ):
         """
         :param model: M3GNet model
+        :param element_refs: Element reference values for each element
         :param calc_forces: Enable force calculations
         :param calc_stresses: Enable stress calculations
         :param calc_hessian: Enable hessian calculations
         """
         super().__init__()
         self.model = model
         self.calc_forces = calc_forces
         self.calc_stresses = calc_stresses
         self.calc_hessian = calc_hessian
-        self.graph_converter = model.graph_converter
+        if element_refs is not None:
+            self.element_ref_calc = AtomRef(property_offset=element_refs)
+        self.element_refs = element_refs
 
     def forward(
-        self, g: dgl.DGLGraph, graph_attr: torch.tensor | None = None, l_g: dgl.DGLGraph | None = None
+        self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None, l_g: dgl.DGLGraph | None = None
     ) -> tuple:
         """
         Args:
-        g: DGL graph
-        graph_attr: State attrs
+            g: DGL graph
+            state_attr: State attrs
 
         Returns:
-        energies, forces, stresses, hessian: torch.tensor
+            energies, forces, stresses, hessian: torch.tensor
         """
         forces = torch.zeros(1)
         stresses = torch.zeros(1)
         hessian = torch.zeros(1)
         if self.calc_forces:
             g.ndata["pos"].requires_grad_(True)
-        total_energies = self.model(g=g, state_attr=graph_attr, l_g=l_g)
+        total_energies = self.model(g=g, state_attr=state_attr, l_g=l_g)
+        if self.element_refs is not None:
+            property_offset = torch.squeeze(self.element_ref_calc(g))
+            total_energies += property_offset
         if self.calc_forces:
             grads = grad(
                 total_energies,
                 [g.ndata["pos"], g.edata["bond_vec"]],
                 grad_outputs=torch.ones_like(total_energies),
                 create_graph=True,
                 retain_graph=True,
```

### Comparing `matgl-0.2.1/matgl/utils/data.py` & `matgl-0.3.0/matgl/utils/remote.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,66 @@
+"""
+Provides utilities for managing models and data.
+"""
 from __future__ import annotations
 
 import os
+from pathlib import Path
 
 import requests
 
-from matgl.config import PRETRAINED_MODELS_PATH
+from matgl.config import MATGL_CACHE
 
 
-class ModelSource:
+class RemoteFile:
     """
-    Defines a local or remote source for models.
+    Handling of download of remote files to a local cache.
     """
 
-    def __init__(self, uri, use_cache=True):
+    def __init__(self, uri: str, use_cache: bool = True, force_download: bool = False):
         """
 
         Args:
             uri: Uniform resource identifier.
-            use_cache: By default, downloaded models are saved at $HOME/.matgl/models. If False, models will be
+            use_cache: By default, downloaded models are saved at $HOME/.matgl. If False, models will be
                 downloaded to current working directory.
+            force_download: To speed up access, a model with the same name in the cache location will be used if
+                present. If you want to force a re-download, set this to True.
         """
         self.uri = uri
-        self.model_name = uri.split("/")[-1]
+        toks = uri.split("/")
+        self.model_name = toks[-2]
+        self.fname = toks[-1]
         if use_cache:
-            if not PRETRAINED_MODELS_PATH.exists():
-                os.makedirs(PRETRAINED_MODELS_PATH)
-            self.local_path = PRETRAINED_MODELS_PATH / self.model_name
+            os.makedirs(MATGL_CACHE / self.model_name, exist_ok=True)
+            self.local_path = MATGL_CACHE / self.model_name / self.fname
         else:
-            self.local_path = self.model_name
-        self._download()
+            os.makedirs(self.model_name, exist_ok=True)
+            self.local_path = Path(self.model_name) / self.fname
+        if (not self.local_path.exists()) or force_download:
+            self._download()
 
     def _download(self):
         r = requests.get(self.uri, allow_redirects=True)
-
         with open(self.local_path, "wb") as f:
             f.write(r.content)
-        return self.local_path
 
     def __enter__(self):
         """
         Support with context.
 
         Returns:
             Stream on local path.
         """
         self.stream = open(self.local_path, "rb")
         return self.stream
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """
+        Exit the with context.
 
         Args:
             exc_type:
             exc_val:
             exc_tb:
 
         Returns:
```

### Comparing `matgl-0.2.1/matgl/utils/maths.py` & `matgl-0.3.0/matgl/utils/maths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Various math function implementations.
+Implementations of math functions.
 """
 
 from __future__ import annotations
 
 import os
 from functools import lru_cache
 from math import pi, sqrt
```

### Comparing `matgl-0.2.1/matgl/utils/sb_roots.npy` & `matgl-0.3.0/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.2.1/matgl.egg-info/PKG-INFO` & `matgl-0.3.0/matgl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.2.1
+Version: 0.3.0
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
 Author-email: ongsp@eng.ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@eng.ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -115,15 +115,15 @@
 # Usage
 
 The pre-trained MEGNet models for the Materials Project formation energy and multi-fidelity band gap are now available.
 The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Structure, Lattice
-from matgl.models.megnet import MEGNet
+from matgl.models._megnet import MEGNet
 
 # load the pre-trained MEGNet model for formation energy model.
 model = MEGNet.load("MEGNet-MP-2018.6.1-Eform")
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.14), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):5f} eV/atom.")
```

### Comparing `matgl-0.2.1/pyproject.toml` & `matgl-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 "*/tests/*" = ["D"]
 "tasks.py" = ["D"]
 
 [tool.pytest.ini_options]
-addopts = "-x --durations=30 --quiet -rxXs --color=yes -p no:warnings"
+addopts = "--durations=30 --quiet -rXs --color=yes -p no:warnings"
 
 [tool.mypy]
 ignore_missing_imports = true
 explicit_package_bases = true
 no_implicit_optional = false
 exclude = ['tests', 'examples']
```

### Comparing `matgl-0.2.1/setup.py` & `matgl-0.3.0/setup.py`

 * *Files identical despite different names*

