# Comparing `tmp/complex-network-link-prediction-1.2.tar.gz` & `tmp/complex-network-link-prediction-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex-network-link-prediction-1.2.tar", last modified: Mon May  1 14:05:37 2023, max compression
+gzip compressed data, was "complex-network-link-prediction-1.3.tar", last modified: Sun May  7 15:48:27 2023, max compression
```

## Comparing `complex-network-link-prediction-1.2.tar` & `complex-network-link-prediction-1.3.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:05:37.743896 complex-network-link-prediction-1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-01 14:05:37.743896 complex-network-link-prediction-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:05:37.739896 complex-network-link-prediction-1.2/cnlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/cnlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/cnlp/dimensionality_reduction_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:05:37.739896 complex-network-link-prediction-1.2/cnlp/other_methods/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/cnlp/other_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/cnlp/other_methods/information_theory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:05:37.739896 complex-network-link-prediction-1.2/cnlp/probabilistic_methods/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/cnlp/probabilistic_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/cnlp/probabilistic_methods/sbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:05:37.739896 complex-network-link-prediction-1.2/cnlp/similarity_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/cnlp/similarity_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/cnlp/similarity_methods/global_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/cnlp/similarity_methods/local_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/cnlp/similarity_methods/quasi_local_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/cnlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:05:37.743896 complex-network-link-prediction-1.2/complex_network_link_prediction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-01 14:05:37.000000 complex-network-link-prediction-1.2/complex_network_link_prediction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-01 14:05:37.000000 complex-network-link-prediction-1.2/complex_network_link_prediction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:05:37.000000 complex-network-link-prediction-1.2/complex_network_link_prediction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 14:05:37.000000 complex-network-link-prediction-1.2/complex_network_link_prediction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 14:05:37.000000 complex-network-link-prediction-1.2/complex_network_link_prediction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 14:05:37.743896 complex-network-link-prediction-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-01 14:05:34.000000 complex-network-link-prediction-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:48:27.141005 complex-network-link-prediction-1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-07 15:48:27.141005 complex-network-link-prediction-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:48:27.137004 complex-network-link-prediction-1.3/cnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/cnlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/cnlp/dimensionality_reduction_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:48:27.137004 complex-network-link-prediction-1.3/cnlp/other_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/cnlp/other_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/cnlp/other_methods/information_theory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/cnlp/probabilistic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:48:27.141005 complex-network-link-prediction-1.3/cnlp/similarity_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/cnlp/similarity_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/cnlp/similarity_methods/global_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/cnlp/similarity_methods/local_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/cnlp/similarity_methods/quasi_local_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/cnlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:48:27.141005 complex-network-link-prediction-1.3/complex_network_link_prediction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-07 15:48:27.000000 complex-network-link-prediction-1.3/complex_network_link_prediction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-07 15:48:27.000000 complex-network-link-prediction-1.3/complex_network_link_prediction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 15:48:27.000000 complex-network-link-prediction-1.3/complex_network_link_prediction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 15:48:27.000000 complex-network-link-prediction-1.3/complex_network_link_prediction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 15:48:27.000000 complex-network-link-prediction-1.3/complex_network_link_prediction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 15:48:27.141005 complex-network-link-prediction-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-07 15:48:25.000000 complex-network-link-prediction-1.3/setup.py
```

### Comparing `complex-network-link-prediction-1.2/LICENSE` & `complex-network-link-prediction-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.2/PKG-INFO` & `complex-network-link-prediction-1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,87 @@
 Metadata-Version: 2.1
 Name: complex-network-link-prediction
-Version: 1.2
+Version: 1.3
+Summary: A python library for link prediction in social networks
 Home-page: https://github.com/Typing-Monkeys/social-network-link-prediction
 Author: Cristian Cosci, Fabrizio Fagiolo, Nicolò Vescera, Nicolò Posta, Tommaso Romani
 License: MIT
 Keywords: Link Prediction,Social Network,Complex Network Analisys
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **Complex Network Link Prediction**
 
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) <!-- [![PyPi](https://badge.fury.io/py/nomepacchetto.svg)](https://badge.fury.io/py/nomepacchetto) --> <!-- [![Downloads](https://pepy.tech/badge/nomepacchetto/month)](https://pepy.tech/project/nomepacchetto) --> [![Wiki](https://img.shields.io/badge/howTo-Wiki-blue.svg)](https://github.com/Typing-Monkeys/social-network-link-prediction/wiki) [![GitHubIssues](https://img.shields.io/badge/issue_tracking-github-blue.svg)](https://github.com/Typing-Monkeys/social-network-link-prediction/issues) [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPi](https://badge.fury.io/py/complex-network-link-prediction.svg)](https://badge.fury.io/py/complex-network-link-prediction) [![Documentation](https://img.shields.io/badge/Documentation-blue.svg)](https://typing-monkeys.github.io/social-network-link-prediction/) [![Downloads](https://pepy.tech/badge/complex-network-link-prediction/month)](https://pepy.tech/project/complex-network-link-prediction) [![Wiki](https://img.shields.io/badge/howTo-Wiki-blue.svg)](https://github.com/Typing-Monkeys/social-network-link-prediction/wiki) [![GitHubIssues](https://img.shields.io/badge/issue_tracking-github-blue.svg)](https://github.com/Typing-Monkeys/social-network-link-prediction/issues) [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 
 
 #### **Complex Network Link Prediction** is a python library that implements some of the main techniques and algorithms to perform link predictions.
 
-
-Check out our [home page](docs link)link pages qui for more information.
-
 <img src="https://raw.githubusercontent.com/Typing-Monkeys/social-network-link-prediction/develop/imgs/logo.png" alt="logo" width="70%" />
 
-This library implemented in python allows you to use some of the main algorithms and methods to perform link predictions. It was designed to carry out these tasks in **Complex Networks** and, specifically, in **Social Networks**. Each method has its own specific documentation available on the following page ---- where it is possible to see the required parameters and the output of the method itself. <br>
+This library, implemented in python, allows you to use some of the main algorithms and methods to perform link predictions. It was designed to carry out these tasks in **Complex Networks** and, specifically, in **Social Networks**. Each method has its own specific documentation available on the [official documentation page](https://typing-monkeys.github.io/social-network-link-prediction/), where it is possible to see the required parameters and the output of the method itself. <br>
 The methods are distinguished by belonging to categories and subcategories, below is an example image with all the categories.
 
-<img src="https://raw.githubusercontent.com/Typing-Monkeys/social-network-link-prediction/develop/imgs/methods_list.jpg" alt="methods list" width="50%" />
+<img src="https://raw.githubusercontent.com/Typing-Monkeys/social-network-link-prediction/develop/imgs/methods_list.jpg" alt="methods list" width="70%" />
 
-The speed of computation differs both from the type of method and from the input graph. However, for convention and efficiency we have chosen to use the `csr_matrix` sparse matrix structure from the ***scipy*** library in each algorithm.
+The speed of computation differs both from the type of method and from the input graph. However, for convention and efficiency, we have chosen to use the `csr_matrix` sparse matrix structure from the ***scipy*** library in each algorithm.
 
 
 ## Install
 ```
-pip install cnlp
+pip install complex-network-link-prediction
 ```
 
 <hr>
 
 
 ## How to use
 ```python
 import networkx as nx
 import matplotlib.pyplot as plt
-from cnlp.utils import to_adjacency_matrix
-from cnlp.probabilistich_methods import stochastic_block_model
+from cnlp.similarity_methods.local_similarity import common_neighbors
+from cnlp.utils import nodes_to_indexes, get_top_predicted_link
 
 G = nx.karate_club_graph()
-A = to_adjacency_matrix(G)
 
-res = stochastic_block_model(G, 10)
+name_index_map = list(nodes_to_indexes(G).items())
 
-predicted_edges = []
-for u in range(res.shape[0]):
-    for v in range(u + 1, res.shape[1]):
-        if G.has_edge(u, v):
-            continue
-        w = res[u, v]
-        predicted_edges.append((u, v, w))
-
-# Sort the predicted edges by weight in descending order
-predicted_edges.sort(key=lambda x: x[2], reverse=True)
-
-# Print the predicted edges with their weight score
-print("Top Predicted edges:")
-for edge in predicted_edges[:50]:
-    print(f"({edge[0]}, {edge[1]}): {edge[2]}")
+predicted_adj_matrix_common_neighbors = common_neighbors(G)
 
-nx.draw(G)
-plt.show()
+new_links = get_top_predicted_link(predicted_adj_matrix_common_neighbors, G.number_of_nodes(), pct_new_link=5, name_index_map=name_index_map, verbose=True)
 ```
 
+You can also check [this project](https://github.com/CristianCosci/ComplexNetworkAnalysis/) to see a real case study for Social Network Analysis and link prediction, with the use of our Python Library.
 <hr>
 
 ### Contribute 💥
 As there are still many methods to implement and, at the same time, maintaining a library takes up a lot of time, we are always happy to accept new willing and able people to contribute and support our project.
 
 If you want to contribute or you've found a bug, you can open a **Pull Request**.
 
-Check this [tutorial](#https://github.com/Typing-Monkeys/social-network-link-prediction/wiki/monkeflow-Workflow-🦍) if you want to use our preferred *Workflow* 🦍 for developing.
+Check this [tutorial](https://github.com/Typing-Monkeys/social-network-link-prediction/wiki/monkeflow-Workflow-🦍) if you want to use our preferred *Workflow* 🦍 for developing.
 
 Otherwise you can open a normal Pull Request using `git` and help us to make this project even better!
 
 ### Help ❓
-If you encounter any bug or you have some problem with this package you can open an [issue](#https://github.com/Typing-Monkeys/social-network-link-prediction/wiki/monkeflow-Workflow-🦍) to report it, we will resolve that asap.
+If you encounter any bug or you have some problem with this package you can open an [issue](https://github.com/Typing-Monkeys/social-network-link-prediction/wiki/monkeflow-Workflow-🦍) to report it, we will resolve that asap.
 
 <hr>
 
 ### Building From Source
-???
+Download the repository and run:
+```
+pip install -e .
+```
 
 ### Dependencies
-If your system does not have some or all of this requirements they will be installed during the istallation of this library
+If your system does not have some or all of this requirements they will be installed during the istallation of the library
 - networkx
 - scipy
 - numpy
-ecc
 
 <hr>
 
 ## References
 
 - ***Ajay Kumar, Shashank Sheshar Singh, Kuldeep Singh, Bhaskar Biswas. 2020.***
     [Link prediction techniques, applications, and performance: A survey](https://www.sciencedirect.com/science/article/pii/S0378437120300856)
@@ -109,11 +94,11 @@
     [A Survey of Link Prediction in Complex Networks](https://dl.acm.org/doi/10.1145/3012704)
     *ACM Comput. Surv. 49, 4, Article 69 (December 2017), 33 pages*. https://doi.org/10.1145/3012704
 
 <hr>
 
 ### ***Authors***
 
-| ![cosci](https://avatars.githubusercontent.com/u/44636000?s=421&v=4) | ![vescera](https://avatars.githubusercontent.com/u/10250769?s=421&v=4)| ![fagiolo](https://avatars.githubusercontent.com/u/44865237?v=4) | ![romani](https://avatars.githubusercontent.com/u/44830726?v=4)| ![posta](https://avatars.githubusercontent.com/u/44830740?v=4) 
+| ![cosci](https://avatars.githubusercontent.com/u/44636000?s=250) | ![vescera](https://avatars.githubusercontent.com/u/10250769?s=250)| ![fagiolo](https://avatars.githubusercontent.com/u/44865237?v=47&size=250) | ![romani](https://avatars.githubusercontent.com/u/44830726?v=4&size=250)| ![posta](https://avatars.githubusercontent.com/u/44830740?v=4&size=250) 
 | - | - | - | - | - |
 | [Cristian Cosci](https://github.com/CristianCosci) 🐔 | [Nicolò Vescera](https://github.com/ncvescera) 🦧 | [Fabrizio Fagiolo](https://github.com/F-a-b-r-i-z-i-o) 🐛 |  [Tommaso Romani](https://github.com/TommasoRomani) 🦍 | [Nicolò Posta](https://github.com/NicoloPosta) 🐒
```

### Comparing `complex-network-link-prediction-1.2/README.md` & `complex-network-link-prediction-1.3/complex_network_link_prediction.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,92 +1,87 @@
+Metadata-Version: 2.1
+Name: complex-network-link-prediction
+Version: 1.3
+Summary: A python library for link prediction in social networks
+Home-page: https://github.com/Typing-Monkeys/social-network-link-prediction
+Author: Cristian Cosci, Fabrizio Fagiolo, Nicolò Vescera, Nicolò Posta, Tommaso Romani
+License: MIT
+Keywords: Link Prediction,Social Network,Complex Network Analisys
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # **Complex Network Link Prediction**
 
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) <!-- [![PyPi](https://badge.fury.io/py/nomepacchetto.svg)](https://badge.fury.io/py/nomepacchetto) --> <!-- [![Downloads](https://pepy.tech/badge/nomepacchetto/month)](https://pepy.tech/project/nomepacchetto) --> [![Wiki](https://img.shields.io/badge/howTo-Wiki-blue.svg)](https://github.com/Typing-Monkeys/social-network-link-prediction/wiki) [![GitHubIssues](https://img.shields.io/badge/issue_tracking-github-blue.svg)](https://github.com/Typing-Monkeys/social-network-link-prediction/issues) [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPi](https://badge.fury.io/py/complex-network-link-prediction.svg)](https://badge.fury.io/py/complex-network-link-prediction) [![Documentation](https://img.shields.io/badge/Documentation-blue.svg)](https://typing-monkeys.github.io/social-network-link-prediction/) [![Downloads](https://pepy.tech/badge/complex-network-link-prediction/month)](https://pepy.tech/project/complex-network-link-prediction) [![Wiki](https://img.shields.io/badge/howTo-Wiki-blue.svg)](https://github.com/Typing-Monkeys/social-network-link-prediction/wiki) [![GitHubIssues](https://img.shields.io/badge/issue_tracking-github-blue.svg)](https://github.com/Typing-Monkeys/social-network-link-prediction/issues) [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 
 
 #### **Complex Network Link Prediction** is a python library that implements some of the main techniques and algorithms to perform link predictions.
 
-
-Check out our [home page](docs link)link pages qui for more information.
-
 <img src="https://raw.githubusercontent.com/Typing-Monkeys/social-network-link-prediction/develop/imgs/logo.png" alt="logo" width="70%" />
 
-This library implemented in python allows you to use some of the main algorithms and methods to perform link predictions. It was designed to carry out these tasks in **Complex Networks** and, specifically, in **Social Networks**. Each method has its own specific documentation available on the following page ---- where it is possible to see the required parameters and the output of the method itself. <br>
+This library, implemented in python, allows you to use some of the main algorithms and methods to perform link predictions. It was designed to carry out these tasks in **Complex Networks** and, specifically, in **Social Networks**. Each method has its own specific documentation available on the [official documentation page](https://typing-monkeys.github.io/social-network-link-prediction/), where it is possible to see the required parameters and the output of the method itself. <br>
 The methods are distinguished by belonging to categories and subcategories, below is an example image with all the categories.
 
-<img src="https://raw.githubusercontent.com/Typing-Monkeys/social-network-link-prediction/develop/imgs/methods_list.jpg" alt="methods list" width="50%" />
+<img src="https://raw.githubusercontent.com/Typing-Monkeys/social-network-link-prediction/develop/imgs/methods_list.jpg" alt="methods list" width="70%" />
 
-The speed of computation differs both from the type of method and from the input graph. However, for convention and efficiency we have chosen to use the `csr_matrix` sparse matrix structure from the ***scipy*** library in each algorithm.
+The speed of computation differs both from the type of method and from the input graph. However, for convention and efficiency, we have chosen to use the `csr_matrix` sparse matrix structure from the ***scipy*** library in each algorithm.
 
 
 ## Install
 ```
-pip install cnlp
+pip install complex-network-link-prediction
 ```
 
 <hr>
 
 
 ## How to use
 ```python
 import networkx as nx
 import matplotlib.pyplot as plt
-from cnlp.utils import to_adjacency_matrix
-from cnlp.probabilistich_methods import stochastic_block_model
+from cnlp.similarity_methods.local_similarity import common_neighbors
+from cnlp.utils import nodes_to_indexes, get_top_predicted_link
 
 G = nx.karate_club_graph()
-A = to_adjacency_matrix(G)
 
-res = stochastic_block_model(G, 10)
+name_index_map = list(nodes_to_indexes(G).items())
 
-predicted_edges = []
-for u in range(res.shape[0]):
-    for v in range(u + 1, res.shape[1]):
-        if G.has_edge(u, v):
-            continue
-        w = res[u, v]
-        predicted_edges.append((u, v, w))
-
-# Sort the predicted edges by weight in descending order
-predicted_edges.sort(key=lambda x: x[2], reverse=True)
-
-# Print the predicted edges with their weight score
-print("Top Predicted edges:")
-for edge in predicted_edges[:50]:
-    print(f"({edge[0]}, {edge[1]}): {edge[2]}")
+predicted_adj_matrix_common_neighbors = common_neighbors(G)
 
-nx.draw(G)
-plt.show()
+new_links = get_top_predicted_link(predicted_adj_matrix_common_neighbors, G.number_of_nodes(), pct_new_link=5, name_index_map=name_index_map, verbose=True)
 ```
 
+You can also check [this project](https://github.com/CristianCosci/ComplexNetworkAnalysis/) to see a real case study for Social Network Analysis and link prediction, with the use of our Python Library.
 <hr>
 
 ### Contribute 💥
 As there are still many methods to implement and, at the same time, maintaining a library takes up a lot of time, we are always happy to accept new willing and able people to contribute and support our project.
 
 If you want to contribute or you've found a bug, you can open a **Pull Request**.
 
-Check this [tutorial](#https://github.com/Typing-Monkeys/social-network-link-prediction/wiki/monkeflow-Workflow-🦍) if you want to use our preferred *Workflow* 🦍 for developing.
+Check this [tutorial](https://github.com/Typing-Monkeys/social-network-link-prediction/wiki/monkeflow-Workflow-🦍) if you want to use our preferred *Workflow* 🦍 for developing.
 
 Otherwise you can open a normal Pull Request using `git` and help us to make this project even better!
 
 ### Help ❓
-If you encounter any bug or you have some problem with this package you can open an [issue](#https://github.com/Typing-Monkeys/social-network-link-prediction/wiki/monkeflow-Workflow-🦍) to report it, we will resolve that asap.
+If you encounter any bug or you have some problem with this package you can open an [issue](https://github.com/Typing-Monkeys/social-network-link-prediction/wiki/monkeflow-Workflow-🦍) to report it, we will resolve that asap.
 
 <hr>
 
 ### Building From Source
-???
+Download the repository and run:
+```
+pip install -e .
+```
 
 ### Dependencies
-If your system does not have some or all of this requirements they will be installed during the istallation of this library
+If your system does not have some or all of this requirements they will be installed during the istallation of the library
 - networkx
 - scipy
 - numpy
-ecc
 
 <hr>
 
 ## References
 
 - ***Ajay Kumar, Shashank Sheshar Singh, Kuldeep Singh, Bhaskar Biswas. 2020.***
     [Link prediction techniques, applications, and performance: A survey](https://www.sciencedirect.com/science/article/pii/S0378437120300856)
@@ -99,11 +94,11 @@
     [A Survey of Link Prediction in Complex Networks](https://dl.acm.org/doi/10.1145/3012704)
     *ACM Comput. Surv. 49, 4, Article 69 (December 2017), 33 pages*. https://doi.org/10.1145/3012704
 
 <hr>
 
 ### ***Authors***
 
-| ![cosci](https://avatars.githubusercontent.com/u/44636000?s=421&v=4) | ![vescera](https://avatars.githubusercontent.com/u/10250769?s=421&v=4)| ![fagiolo](https://avatars.githubusercontent.com/u/44865237?v=4) | ![romani](https://avatars.githubusercontent.com/u/44830726?v=4)| ![posta](https://avatars.githubusercontent.com/u/44830740?v=4) 
+| ![cosci](https://avatars.githubusercontent.com/u/44636000?s=250) | ![vescera](https://avatars.githubusercontent.com/u/10250769?s=250)| ![fagiolo](https://avatars.githubusercontent.com/u/44865237?v=47&size=250) | ![romani](https://avatars.githubusercontent.com/u/44830726?v=4&size=250)| ![posta](https://avatars.githubusercontent.com/u/44830740?v=4&size=250) 
 | - | - | - | - | - |
 | [Cristian Cosci](https://github.com/CristianCosci) 🐔 | [Nicolò Vescera](https://github.com/ncvescera) 🦧 | [Fabrizio Fagiolo](https://github.com/F-a-b-r-i-z-i-o) 🐛 |  [Tommaso Romani](https://github.com/TommasoRomani) 🦍 | [Nicolò Posta](https://github.com/NicoloPosta) 🐒
```

### Comparing `complex-network-link-prediction-1.2/cnlp/dimensionality_reduction_methods.py` & `complex-network-link-prediction-1.3/cnlp/dimensionality_reduction_methods.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.2/cnlp/other_methods/information_theory.py` & `complex-network-link-prediction-1.3/cnlp/other_methods/information_theory.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.2/cnlp/probabilistic_methods/sbm.py` & `complex-network-link-prediction-1.3/cnlp/probabilistic_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,184 +1,39 @@
+"""Collection of Probabilistic Methods for Link Prediction."""
 import networkx as nx
 import numpy as np
 from networkx.algorithms.community import louvain_communities
 from cnlp.utils import to_adjacency_matrix
 from scipy.sparse import csr_matrix, lil_matrix
 from scipy.special import comb
 from typing import List, Set
 from itertools import product, combinations_with_replacement
 from cnlp.utils import nodes_to_indexes
 
 
-def __random_changes(A_0: csr_matrix, p: float = .05) -> lil_matrix:
-    """Perform random changes in the Adjacency Matrix
-
-    This function is used to generate chaos in the network
-    for the sample (blocks) collection.
-
-    Parameters
-    ----------
-    A_0: csr_matrix :
-        the original Adjacency Matrix
-    p: float :
-        chaos probability, higher means more
-        chaos
-         (Default value = 0.05)
-
-    Returns
-    -------
-    A_chaos: lil_matrix : the new chaos matrix
-    """
-    A_chaos = A_0.copy().tolil()
-    num_changes = int(A_chaos.shape[0]**2 * p)
-    indexes = []
-
-    while len(indexes) < num_changes:
-        x = np.random.randint(0, high=A_chaos.shape[0])
-        y = np.random.randint(0, high=A_chaos.shape[0])
-
-        if x == y:
-            continue
-
-        if (x, y) in indexes or (y, x) in indexes:
-            continue
-
-        indexes.append((x, y))
-
-    for x, y in indexes:
-        A_chaos[x, y] = abs(A_0[x, y] - 1)
-        A_chaos[y, x] = A_chaos[x, y]
-
-    return A_chaos
-
-
-def __generate_samples(A_0: csr_matrix,
-                       n: int,
-                       p: np.float32 = .05,
-                       seed: int = 42) -> List[List[Set]]:
-    """Generate the samples (block) given the orginal
-    adjacecy matrix.
-
-    Parameters
-    ----------
-    A_0: csr_matrix :
-        the original Adjacency Matrix
-    n: int :
-        number of samples
-    p: float :
-        chaos probability, higher means more
-        chaos
-         (Default value = 0.05)
-    seed: int :
-        seed for random generated values
-         (Default values = 42)
-
-    Returns
-    -------
-    samples_list: List[List[Set]] : all the samples
-    """
-    samples_list = []
-
-    for _ in range(n):
-        A_chaos = __random_changes(A_0, p)
-        G_chaos = nx.Graph(A_chaos)
-        res = louvain_communities(G_chaos, seed)
-        samples_list.append(res)
-
-    return samples_list
-
-
-def __get_node_block(sample: List[Set], x: int) -> Set:
-    """Return the block that node X belongs to
-
-    Parameters
-    ----------
-    samole: List[Set] :
-        current sample to analize
-    x: int :
-        node
-
-    Returns
-    -------
-    Set : the block
-    """
-    for i in sample:
-        if x in i:
-            return i
-
-
-def __l(A_0: lil_matrix, alpha: Set, beta: Set) -> int:
-    """Number of links between groups Alpha and Beta"""
-    return np.sum([A_0[x, y] for x, y in product(alpha, beta)])
-
-
-def __r(alpha: Set, beta: Set) -> int:
-    """Maxmimum possible links between groups Alpha and Beta"""
-    len_a = len(alpha)
-    len_b = len(beta)
-
-    if alpha == beta:
-        return len_a * (len_a - 1)
-
-    return (len_a * len_b)
-
-
-def __H(A_0: csr_matrix, P: List[Set]) -> float:
-    res = 0
-    for a, b in combinations_with_replacement(P, 2):
-        r = __r(a, b)
-        l0 = __l(A_0, a, b)
-
-        res += np.log(r + 1) + np.log(comb(r, l0))
-
-    return res
-
-
-def __link_reliability(A_0: csr_matrix, samples_list: List[List[Set]], x: int,
-                       y: int) -> float:
-    summing_result = 0
-    HP_mem = []
-
-    for sample in samples_list:
-        x_block = __get_node_block(sample, x)
-        y_block = __get_node_block(sample, y)
-
-        l_xy = __l(A_0, x_block, y_block) + 1
-        r_xy = __r(x_block, y_block) + 2
-
-        second_term = np.exp(-__H(A_0, sample))
-        HP_mem.append(second_term)
-
-        tmp_ratio = l_xy / r_xy
-
-        summing_result += tmp_ratio * second_term
-
-    return summing_result / np.sum(HP_mem)
-
-
 def stochastic_block_model(G: nx.Graph,
                            n: int,
                            p: float = .05,
                            seed: int = 42) -> csr_matrix:
     """Compute the Sotchastic Block Model Similarity for
     all the nodes in the network.
 
     This similarity is defined as:
 
     .. math::
         R_{xy} = \\frac{1}{Z} \\sum_{P \\in P^*}
             ( \\frac{l^1_{\\sigma_x \\sigma_y}+1}{r^0_{\\sigma_x \\sigma_y} +2}) exp[-H(P)]
 
     where the sum is over all possible partitions \\(P^*\\) of the network
-    into groups, \\( \\sigma_x \\) and \\( \\sigma_y \\) are vertices \\(x\\) and \\(y\\)
-    groups in partition \\(P\\) respectively.
+    into groups, \\( \\sigma_x \\) and \\( \\sigma_y \\) are vertices \\(x\\)
+    and \\(y\\) groups in partition \\(P\\) respectively.
     Moreover, \\(l^0_{ \\sigma_{\\alpha} \\sigma_{\\beta}} \\)
     and \\(r^0_{ \\sigma_{\\alpha} \\sigma_{\\beta}} \\)
-    are the number of links and maximum possible links in the observed network between
-    groups \\( \\alpha \\) and \\( \\beta \\).
+    are the number of links and maximum possible links in the observed network
+    between groups \\( \\alpha \\) and \\( \\beta \\).
 
     Parameters
     ----------
     G: nx.Graph :
         input Graph (a networkx Graph)
     n: int :
         number of samples
@@ -190,14 +45,154 @@
         seed for the random generated values
          (Default value = 42)
 
     Returns
     -------
     R: csr_matrix : the Similarity Matrix (in sparse format)
     """
+
+    def __random_changes(A_0: csr_matrix, p: float = .05) -> lil_matrix:
+        """Perform random changes in the Adjacency Matrix
+
+        This function is used to generate chaos in the network
+        for the sample (blocks) collection.
+
+        Parameters
+        ----------
+        A_0: csr_matrix :
+            the original Adjacency Matrix
+        p: float :
+            chaos probability, higher means more
+            chaos
+             (Default value = 0.05)
+
+        Returns
+        -------
+        A_chaos: lil_matrix : the new chaos matrix
+        """
+        A_chaos = A_0.copy().tolil()
+        num_changes = int(A_chaos.shape[0]**2 * p)
+        indexes = []
+
+        while len(indexes) < num_changes:
+            x = np.random.randint(0, high=A_chaos.shape[0])
+            y = np.random.randint(0, high=A_chaos.shape[0])
+
+            if x == y:
+                continue
+
+            if (x, y) in indexes or (y, x) in indexes:
+                continue
+
+            indexes.append((x, y))
+
+        for x, y in indexes:
+            A_chaos[x, y] = abs(A_0[x, y] - 1)
+            A_chaos[y, x] = A_chaos[x, y]
+
+        return A_chaos
+
+    def __generate_samples(A_0: csr_matrix,
+                           n: int,
+                           p: np.float32 = .05,
+                           seed: int = 42) -> List[List[Set]]:
+        """Generate the samples (block) given the orginal
+        adjacecy matrix.
+
+        Parameters
+        ----------
+        A_0: csr_matrix :
+            the original Adjacency Matrix
+        n: int :
+            number of samples
+        p: float :
+            chaos probability, higher means more
+            chaos
+             (Default value = 0.05)
+        seed: int :
+            seed for random generated values
+             (Default values = 42)
+
+        Returns
+        -------
+        samples_list: List[List[Set]] : all the samples
+        """
+        samples_list = []
+
+        for _ in range(n):
+            A_chaos = __random_changes(A_0, p)
+            G_chaos = nx.Graph(A_chaos)
+            res = louvain_communities(G_chaos, seed)
+            samples_list.append(res)
+
+        return samples_list
+
+    def __get_node_block(sample: List[Set], x: int) -> Set:
+        """Return the block that node X belongs to
+
+        Parameters
+        ----------
+        samole: List[Set] :
+            current sample to analize
+        x: int :
+            node
+
+        Returns
+        -------
+        Set : the block
+        """
+        for i in sample:
+            if x in i:
+                return i
+
+    def __l(A_0: lil_matrix, alpha: Set, beta: Set) -> int:
+        """Number of links between groups Alpha and Beta"""
+        return np.sum([A_0[x, y] for x, y in product(alpha, beta)])
+
+    def __r(alpha: Set, beta: Set) -> int:
+        """Maxmimum possible links between groups Alpha and Beta"""
+        len_a = len(alpha)
+        len_b = len(beta)
+
+        if alpha == beta:
+            return len_a * (len_a - 1)
+
+        return (len_a * len_b)
+
+    def __H(A_0: csr_matrix, P: List[Set]) -> float:
+        res = 0
+        for a, b in combinations_with_replacement(P, 2):
+            r = __r(a, b)
+            l0 = __l(A_0, a, b)
+
+            res += np.log(r + 1) + np.log(comb(r, l0))
+
+        return res
+
+    def __link_reliability(A_0: csr_matrix, samples_list: List[List[Set]],
+                           x: int, y: int) -> float:
+        summing_result = 0
+        HP_mem = []
+
+        for sample in samples_list:
+            x_block = __get_node_block(sample, x)
+            y_block = __get_node_block(sample, y)
+
+            l_xy = __l(A_0, x_block, y_block) + 1
+            r_xy = __r(x_block, y_block) + 2
+
+            second_term = np.exp(-__H(A_0, sample))
+            HP_mem.append(second_term)
+
+            tmp_ratio = l_xy / r_xy
+
+            summing_result += tmp_ratio * second_term
+
+        return summing_result / np.sum(HP_mem)
+
     np.random.seed(seed)
 
     A_0 = to_adjacency_matrix(G)
     samples_list = __generate_samples(A_0, n, p, seed=seed)
     nodes_to_indexes_map = nodes_to_indexes(G)
 
     R = lil_matrix(A_0.shape)
```

### Comparing `complex-network-link-prediction-1.2/cnlp/similarity_methods/__init__.py` & `complex-network-link-prediction-1.3/cnlp/similarity_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.2/cnlp/similarity_methods/global_similarity.py` & `complex-network-link-prediction-1.3/cnlp/similarity_methods/global_similarity.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.2/cnlp/similarity_methods/local_similarity.py` & `complex-network-link-prediction-1.3/cnlp/similarity_methods/local_similarity.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.2/cnlp/similarity_methods/quasi_local_similarity.py` & `complex-network-link-prediction-1.3/cnlp/similarity_methods/quasi_local_similarity.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.2/complex_network_link_prediction.egg-info/SOURCES.txt` & `complex-network-link-prediction-1.3/complex_network_link_prediction.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 cnlp/__init__.py
 cnlp/dimensionality_reduction_methods.py
+cnlp/probabilistic_methods.py
 cnlp/utils.py
 cnlp/other_methods/__init__.py
 cnlp/other_methods/information_theory.py
-cnlp/probabilistic_methods/__init__.py
-cnlp/probabilistic_methods/sbm.py
 cnlp/similarity_methods/__init__.py
 cnlp/similarity_methods/global_similarity.py
 cnlp/similarity_methods/local_similarity.py
 cnlp/similarity_methods/quasi_local_similarity.py
 complex_network_link_prediction.egg-info/PKG-INFO
 complex_network_link_prediction.egg-info/SOURCES.txt
 complex_network_link_prediction.egg-info/dependency_links.txt
```

### Comparing `complex-network-link-prediction-1.2/setup.py` & `complex-network-link-prediction-1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='complex-network-link-prediction',
-    version='1.2',
+    version='1.3',
     license='MIT',
-    author=
-    "Cristian Cosci, Fabrizio Fagiolo, Nicolò Vescera, Nicolò Posta, Tommaso Romani",
+    description='A python library for link prediction in social networks',
+    author="Cristian Cosci, Fabrizio Fagiolo, Nicolò Vescera, Nicolò Posta, Tommaso Romani",
     packages=find_packages(where='.', include=['cnlp*']),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Typing-Monkeys/social-network-link-prediction',
     keywords='Link Prediction, Social Network, Complex Network Analisys',
     install_requires=[
         'networkx',
```

