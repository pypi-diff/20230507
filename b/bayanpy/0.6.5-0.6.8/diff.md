# Comparing `tmp/bayanpy-0.6.5.tar.gz` & `tmp/bayanpy-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.6.5.tar", last modified: Thu Apr 20 14:32:35 2023, max compression
+gzip compressed data, was "bayanpy-0.6.8.tar", last modified: Sun May  7 16:01:02 2023, max compression
```

## Comparing `bayanpy-0.6.5.tar` & `bayanpy-0.6.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-20 14:32:35.021626 bayanpy-0.6.5/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.5/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-20 14:32:35.021626 bayanpy-0.6.5/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5056 2023-04-11 16:11:47.000000 bayanpy-0.6.5/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-20 14:32:35.021626 bayanpy-0.6.5/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    52486 2023-04-13 15:23:37.000000 bayanpy-0.6.5/bayanpy/BayanImplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.6.5/bayanpy/__init__.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-20 14:32:35.021626 bayanpy-0.6.5/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-04-20 14:32:34.000000 bayanpy-0.6.5/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-04-20 14:32:34.000000 bayanpy-0.6.5/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-20 14:32:34.000000 bayanpy-0.6.5/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       61 2023-04-20 14:32:34.000000 bayanpy-0.6.5/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-20 14:32:34.000000 bayanpy-0.6.5/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-20 14:32:35.021626 bayanpy-0.6.5/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      583 2023-04-20 14:32:28.000000 bayanpy-0.6.5/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-07 16:01:02.612158 bayanpy-0.6.8/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.8/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-07 16:01:02.612158 bayanpy-0.6.8/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5041 2023-05-07 15:46:50.000000 bayanpy-0.6.8/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-07 16:01:02.612158 bayanpy-0.6.8/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    57258 2023-05-07 15:37:43.000000 bayanpy-0.6.8/bayanpy/BayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.6.8/bayanpy/__init__.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-07 16:01:02.612158 bayanpy-0.6.8/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-07 16:01:02.000000 bayanpy-0.6.8/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-05-07 16:01:02.000000 bayanpy-0.6.8/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-05-07 16:01:02.000000 bayanpy-0.6.8/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-05-07 16:01:02.000000 bayanpy-0.6.8/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-05-07 16:01:02.000000 bayanpy-0.6.8/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-05-07 16:01:02.612158 bayanpy-0.6.8/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-05-07 16:00:44.000000 bayanpy-0.6.8/setup.py
```

### Comparing `bayanpy-0.6.5/LICENSE` & `bayanpy-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.5/README.md` & `bayanpy-0.6.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 Bayanpy has the following dependencies:
 
 - requests>=2.25.1
 - pandas>=1.3.0
 - networkx>=2.6.3
 - numpy>=1.21.0
 - gurobipy>=9.5
-- cdlib>=0.2.6
 - joblib>=1.1.0
 
 These packages will be automatically installed when you install Bayanpy using pip.
 
 
 
 ### Gurobi Installation with Free Academic License
```

### Comparing `bayanpy-0.6.5/bayanpy/BayanImplied.py` & `bayanpy-0.6.8/bayanpy/BayanImplied.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import requests, zipfile, shutil, json
 import pandas as pd
 import networkx as nx
 from io import BytesIO
 import numpy as np
 import time
 import multiprocessing
+import pycombo
 from itertools import combinations 
 from gurobipy import *
-from cdlib import algorithms
 from networkx.algorithms.connectivity import minimum_st_node_cut
 from joblib import Parallel, delayed, parallel_backend
 from itertools import chain
-
+# from pyomo.environ import *
+# from pyomo.opt import SolverFactory
 
 def get_graph_from_network_name(network_name, sub_name=None):
     """
     Method to create a networkx Graph from network names listed at https://networks.skewed.de/
     """
     #Defining the network information url
     info_url = "https://networks.skewed.de/api/net/%s" % network_name
@@ -115,31 +116,29 @@
     if is_multigraph:
         print("%s is a multigraph but has been loaded as a simple graph" % network_name)
     
     shutil.rmtree(network_name + "_files")
     return G
 
 
-# In[4]:
-
-
 def get_local_clustering_coefficient(G, node: int):
     """
     Returns the clustering coefficient for the input node in the input graph
     """
-    neighbours = nx.adjacency_matrix(G)[node].indices
+    neighbours = nx.adjacency_matrix(G)[:node].indices
     if neighbours.shape[0] <= 1:
         return 0.0
     num_possible_edges = ((neighbours.shape[0])*(neighbours.shape[0]-1)) / 2
     num_actual_edges = 0
     for neighbour in neighbours:
-        num_actual_edges += np.intersect1d(neighbours, nx.adjacency_matrix(G)[neighbour].indices).shape[0]
+        num_actual_edges += np.intersect1d(neighbours, nx.adjacency_matrix(G)[:neighbour].indices).shape[0]
     num_actual_edges = num_actual_edges / 2
     return num_actual_edges / num_possible_edges
 
+
 def clique_filtering(G, resolution):
     """
     Returns G' which is a clique reduction on the input graph G 
     """
     lcc_dict = {}
     for node in G.nodes():
         lcc_dict[node] = get_local_clustering_coefficient(G, node)
@@ -148,15 +147,15 @@
         skip = False
         for n in G.nodes():
             if n in shrink_dict and shrink_dict[n] == node and n != node:
                 skip = True
         if skip:
             shrink_dict[node] = node
             continue
-        neighbours = nx.adjacency_matrix(G)[node].indices
+        neighbours = nx.adjacency_matrix(G)[:node].indices
         if neighbours.shape[0] == 1:
             shrink_dict[node] = neighbours[0]
             continue
         count_of_ones = 0
         count_of_not_one = 0
         not_one_neighbour = -1
         for neighbour in neighbours:
@@ -194,27 +193,21 @@
 #     ModularityMatrix = nx.modularity_matrix(G_prime, weight="actual_weight")
     ModularityMatrix = get_modularity_matrix(G_prime, resolution)
     for edge in G_prime.edges():
         G_prime.edges[edge[0], edge[1]]["weight"] = ModularityMatrix[edge[0], edge[1]]
     return G_prime
 
 
-# In[5]:
-
-
 def find_in_list_of_list(mylist, char):
     for sub_list in mylist:
         if char in sub_list:
             return (mylist.index(sub_list))
     raise ValueError("'{char}' is not in list".format(char = char))
 
 
-# In[6]:
-
-
 def model_to_communities(var_vals, Graph):
     """
     Method that outputs communities with input model variable values and the Graph
     """
     clustered = []
     
     for v in var_vals:
@@ -258,17 +251,14 @@
     for c in range(len(group)):
         group[c].sort()
     group.sort()
     
     return group
 
 
-# In[7]:
-
-
 def decluster_communities(group, Graph, isolated_nodes):
     """
     Method to get communities based on the original graph. Note, input Graph is the reduced graph.
     """
     group_declustered = []
     for comm in group:
         new_comm = []
@@ -283,62 +273,188 @@
         group_declustered.append([n])
     for c in range(len(group_declustered)):
         group_declustered[c].sort()
     group_declustered.sort()
     return group_declustered
 
 
-# In[8]:
-
-
 def separating_set_parallel(i, j, Graph):
     triads = []
     minimum_vertex_cut=minimum_st_node_cut(Graph, i, j)
     for k in minimum_vertex_cut:
         triads.append(list(np.sort([i,j,k])))
     return triads
 
 
-# In[9]:
+def lp_formulation_pyomo(Graph, AdjacencyMatrix, ModularityMatrix, size, order, isolated_nodes, lp_method, warmstart=int(0),
+                   branching_priotiy=int(0)):
+    """
+    Method to create the LP model and run it for the root node
+    """
+
+    formulation_time_start = time.time()
+    list_of_cut_triads = []
+    pairs = set(combinations(np.sort(list((Graph).nodes())), 2))
+    self_edges = set([(i, i) for i in (Graph).nodes()])
+    pairs_with_edges = set((Graph).edges()) - self_edges
+    pairs_without_edges = pairs - pairs_with_edges
+    pairs_without_edges = list(pairs_without_edges)
+    pairs_with_edges = list(pairs_with_edges)
+
+    # JOBLIB
+    with parallel_backend(backend='loky', n_jobs=-1):
+        res = Parallel()(delayed(separating_set_parallel)(pair[0], pair[1], Graph) for pair in pairs_without_edges)
+
+    list_of_cut_triads = list(chain(*res))
+
+    for pair in pairs_with_edges:
+        i = pair[0]
+        j = pair[1]
+        removed_edge = False
+        if Graph.has_edge(i, j):
+            removed_edge = True
+            attr_dict = Graph.edges[i, j]
+            Graph.remove_edge(i, j)
+        minimum_vertex_cut = minimum_st_node_cut(Graph, i, j)
+        for k in minimum_vertex_cut:
+            list_of_cut_triads.append(list(np.sort([i, j, k])))
+        if removed_edge:
+            Graph.add_edge(i, j, weight=attr_dict["weight"], constrained_modularity=attr_dict["constrained_modularity"],
+                           actual_weight=attr_dict["actual_weight"])
+
+    # Create model
+    model = ConcreteModel()
+
+    # Define index sets
+    model.node_pairs = Set(
+        initialize=[(i, j) for i in range(len(Graph.nodes())) for j in range(i + 1, len(Graph.nodes()))], ordered=True)
+
+    # Define variables
+    model.x = Var(model.node_pairs, within=Binary)
+
+    # Define objective
+    def obj_expression(m):
+        return sum(ModularityMatrix[i, j] * (1 - m.x[i, j]) for (i, j) in m.node_pairs)
+
+    model.obj = Objective(rule=obj_expression, sense=maximize)
 
+    # Define constraints
+    def triangle_constraints(m, i, j, k):
+        return m.x[i, k] <= m.x[i, j] + m.x[j, k]
 
-def lp_formulation (Graph, AdjacencyMatrix, ModularityMatrix, size, order, isolated_nodes, lp_method, warmstart=int(0), branching_priotiy=int(0)):
+    model.triangle1 = Constraint(list_of_cut_triads, rule=triangle_constraints)
+
+    def triangle_constraints2(m, i, j, k):
+        return m.x[i, j] <= m.x[i, k] + m.x[j, k]
+
+    model.triangle2 = Constraint(list_of_cut_triads, rule=triangle_constraints2)
+
+    def triangle_constraints3(m, i, j, k):
+        return m.x[j, k] <= m.x[i, j] + m.x[i, k]
+
+    model.triangle3 = Constraint(list_of_cut_triads, rule=triangle_constraints3)
+
+    formulation_time = time.time() - formulation_time_start
+
+    # Create a solver
+
+    solver = SolverFactory("appsi_highs") # SolverFactory('gurobi')
+    solver.options['Method'] = lp_method
+    solver.options['Crossover'] = 0
+
+    # Set solver options
+    solver.options['Threads'] = min(64, multiprocessing.cpu_count())
+    solver.options['OutputFlag'] = 0
+
+    # Using a warm start
+    if warmstart == 1:
+        # Solution from Combo algorithm to be used as warm-start
+        partition = pycombo.execute(Graph, modularity_resolution=resolution)
+        community_combo = list(partition.communities)
+        for i in (Graph).nodes():
+            for j in filter(lambda x: x > i, (Graph).nodes()):
+                if find_in_list_of_list(community_combo, i) == find_in_list_of_list(community_combo, j):
+                    model.x[i, j].value = 0
+                else:
+                    model.x[i, j].value = 1
+        solver.options['WarmStart'] = 1
+
+    # Solve the model
+    start_time = time.time()
+    results = solver.solve(model, tee=False)
+    solveTime = (time.time() - start_time)
+
+    if results.solver.status == SolverStatus.ok and results.solver.termination_condition == TerminationCondition.optimal:
+        # Objective value
+        objectivevalue = np.round(((2 * model.obj() + (ModularityMatrix.trace())) / np.sum(AdjacencyMatrix)), 8)
+
+        # Variable values
+        var_vals = {str(i) + ',' + str(j): model.x[i, j].value for (i, j) in model.node_pairs}
+
+        return objectivevalue, var_vals, model, list_of_cut_triads, formulation_time, solveTime
+    else:
+        print("Solver status:", results.solver.status)
+        print("Termination condition:", results.solver.termination_condition)
+        raise ValueError("The solver did not find an optimal solution.")
+
+
+def run_lp_pyomo(model, Graph, fixed_ones, fixed_zeros, resolution, lp_method):
     """
-    Method to create the LP model and run it for the root node
+    Run the LP based on model and the original Graph as input
     """
+    ModularityMatrix = get_modularity_matrix(Graph, resolution)
+    AdjacencyMatrix = nx.to_numpy_matrix(Graph, weight='actual_weight')
 
-    objectivevalue=0
-    solveTime=0
-    effectiveBranchingFactors=0
-    number_of_subsets=[]
-    communities=[]
+    # Fix variables
+    for (i, j) in fixed_ones:
+        model.x[i, j].fix(1)
+    for (i, j) in fixed_zeros:
+        model.x[i, j].fix(0)
+
+    # Create a solver
+    solver = SolverFactory('gurobi')
+    solver.options['Method'] = lp_method
+    solver.options['Crossover'] = 0
+    solver.options['Threads'] = min(64, multiprocessing.cpu_count())
+    solver.options['OutputFlag'] = 0
 
-    #This code lists all sorted triples of nodes (open and closed)
-#     list_of_tuples=list(combinations(np.sort(list((Graph).nodes())),3))
-#     list_of_triads=[list(elem) for elem in list_of_tuples]
+    # Solve the model
+    start_time = time.time()
+    results = solver.solve(model, tee=False)
+    solveTime = (time.time() - start_time)
+
+    if results.solver.status == SolverStatus.ok and results.solver.termination_condition == TerminationCondition.optimal:
+        # Objective value
+        objectivevalue = np.round(((2 * model.obj() + (ModularityMatrix.trace())) / np.sum(AdjacencyMatrix)), 8)
+
+        # Variable values
+        var_vals = {(i, j): model.x[i, j].value for (i, j) in model.node_pairs}
+
+        return objectivevalue, var_vals, model
+    else:
+        print("Solver status:", results.solver.status)
+        print("Termination condition:", results.solver.termination_condition)
+        return -1, -1, model
+
+
+def lp_formulation (Graph, AdjacencyMatrix, ModularityMatrix, isolated_nodes,
+                    lp_method, warmstart=int(0), branching_priotiy=int(0)):
+    """
+    Method to create the LP model and run it for the root node
+    """
     formulation_time_start = time.time()
     list_of_cut_triads=[]
-    
-#     pairs_with_edges = []
-#     pairs_without_edges = []
-#     for i in (Graph).nodes():
-#         for j in range(i+1, len((Graph).nodes())):
-#             if Graph.has_edge(i, j):
-#                 pairs_with_edges.append((i, j))
-#             else:
-#                 pairs_without_edges.append((i, j))
-
     pairs = set(combinations(np.sort(list((Graph).nodes())),2))
     self_edges =set([(i, i) for i in (Graph).nodes()])
     pairs_with_edges = set((Graph).edges()) - self_edges
     pairs_without_edges = pairs - pairs_with_edges
     pairs_without_edges = list(pairs_without_edges)
     pairs_with_edges = list(pairs_with_edges)
         
-# JOBLIB
+    # JOBLIB
     with parallel_backend(backend='loky', n_jobs=-1):
         res = Parallel()(delayed(separating_set_parallel)(pair[0], pair[1], Graph) for pair in pairs_without_edges)
     
     list_of_cut_triads = list(chain(*res))
 
     for pair in pairs_with_edges:
         i = pair[0]
@@ -348,134 +464,89 @@
             removed_edge = True
             attr_dict = Graph.edges[i, j]
             Graph.remove_edge(i, j)
         minimum_vertex_cut=minimum_st_node_cut(Graph, i, j)
         for k in minimum_vertex_cut:
             list_of_cut_triads.append(list(np.sort([i,j,k])))
         if removed_edge:
-            Graph.add_edge(i, j, weight=attr_dict["weight"], constrained_modularity=attr_dict["constrained_modularity"], actual_weight=attr_dict["actual_weight"])
+            Graph.add_edge(i, j, weight=attr_dict["weight"], constrained_modularity=attr_dict["constrained_modularity"],
+                           actual_weight=attr_dict["actual_weight"])
 
-            
-#     list_of_cut_triads = []
-#     for i in (Graph).nodes():
-#         for j in range(i+1, len((Graph).nodes())):
-#             removed_edge = False
-#             if Graph.has_edge(i, j):
-#                 removed_edge = True
-#                 attr_dict = Graph.edges[i, j]
-#                 Graph.remove_edge(i, j)
-#             minimum_vertex_cut=minimum_st_node_cut(Graph, i, j)
-#             for k in minimum_vertex_cut:
-#                 list_of_cut_triads.append(list(np.sort([i,j,k])))
-#             if removed_edge:
-#                 Graph.add_edge(i, j, weight=attr_dict["weight"], constrained_modularity=attr_dict["constrained_modularity"], actual_weight=attr_dict["actual_weight"])
-#     return list_of_cut_triads
-    
     x={}
-
     model = Model("Modularity maximization")
     model.setParam(GRB.param.OutputFlag, 0) 
     model.setParam(GRB.param.Method, lp_method)
     model.setParam(GRB.Param.Crossover, 0)
     model.setParam(GRB.Param.Threads, min(64,multiprocessing.cpu_count()))
 
-
-
     for i in range(len(Graph.nodes())):
         for j in range(i+1, len(Graph.nodes())):
             x[(i,j)] = model.addVar(lb=0, ub=1, vtype=GRB.CONTINUOUS, name=str(i)+','+str(j))
 
     model.update()
 
     OFV = 0 
     for i in range(len(Graph.nodes())):
         for j in range(i+1, len(Graph.nodes())):
             OFV += ModularityMatrix[i, j] * (1 - x[(i, j)])
 
     model.setObjective(OFV, GRB.MAXIMIZE)
 
-#    print('Adding constraints...')
-#     for [i,j,k] in list_of_triads:
-#     base_constraints = []
     for [i,j,k] in list_of_cut_triads:
         model.addConstr(x[(i,k)] <= x[(i, j)] + x[(j, k)], 'triangle1'+','+str(i)+','+str(j)+','+str(k))
         model.addConstr(x[(i,j)] <= x[(i, k)] + x[(j, k)], 'triangle2'+','+str(i)+','+str(j)+','+str(k))
         model.addConstr(x[(j,k)] <= x[(i, j)] + x[(i, k)], 'triangle3'+','+str(i)+','+str(j)+','+str(k))
-#         base_constraints.append('triangle1'+','+str(i)+','+str(j)+','+str(k))
     formulation_time = time.time() - formulation_time_start
 
     model.update()
 
     # Using a warm start
     # A known partition can be used as a starting point to "warm-start" the algorithm.
     # It can be provided to the model here by giving start values to the decision variables:
     # If this optional step is skipped, you should comment out these five lines
     if warmstart==1:
         #Solution from Combo algorithm to be used as warm-start
-        partition = algorithms.pycombo(Graph[index], modularity_resolution=resolution)
+        partition = pycombo.execute(Graph, modularity_resolution=resolution)
         community_combo=list(partition.communities)
         for i in (Graph).nodes():
             for j in filter(lambda x: x>i, (Graph).nodes()):
                 if find_in_list_of_list(community_combo,i)==find_in_list_of_list(community_combo,j):
-                    x[(i,j)].start = 0
+                    x[(i, j)].start = 0
                 else:
-                    x[(i,j)].start = 1   
-
-    #branching priority is based on total degrees of pairs of nodes
+                    x[(i, j)].start = 1
+    # branching priority is based on total degrees of pairs of nodes
     if branching_priotiy == 1:
         neighbors={}
         Degree=[]
         for i in range(len(Graph.nodes())):
             for j in range(i+1, len(Graph.nodes())):
                 neighbors[i] = list((Graph)[i])
                 neighbors[j] = list((Graph)[j])
                 Degree.append(len(neighbors[i])+len(neighbors[j]))
         model.setAttr('BranchPriority',model.getVars()[:],Degree)
         model.update()
 
     start_time = time.time()
     model.optimize()
-    solveTime = (time.time() - start_time) 
-
+    solveTime = (time.time() - start_time)
     obj = model.getObjective()
 
-#     objectivevalue = np.round(((2*obj.getValue()+(ModularityMatrix.trace()[0,0]))/np.sum(AdjacencyMatrix)), 8)
+    # objectivevalue = np.round(((2*obj.getValue()+(ModularityMatrix.trace()[0,0]))/np.sum(AdjacencyMatrix)), 8)
     objectivevalue = np.round(((2*obj.getValue()+(ModularityMatrix.trace()))/np.sum(AdjacencyMatrix)), 8)
-
-
-#    print('Instance 0',': modularity equals',objectivevalue) 
-
-    if (model.NodeCount)**(1/((size)+2*(order))) >= 1:
-        effectiveBranchingFactors = ((model.NodeCount)**(1/((size)+2*(order))))  
+    # print('Instance 0',': modularity equals',objectivevalue)
+    # if (model.NodeCount)**(1/((size)+2*(order))) >= 1:
+    #    effectiveBranchingFactors = ((model.NodeCount)**(1/((size)+2*(order))))
     
     var_vals = {}
     for var in model.getVars():
         var_vals[var.varName] = var.x
-        
-    communities = model_to_communities(var_vals, Graph)
-
-#    print("Communities: ", communities)
 
-    communities_declustered = decluster_communities(communities, Graph, isolated_nodes)
-#    print("Communities de-clustered: ", communities_declustered)
-
-    
-
-#    print("\n")
-#    print("Q*:")
-#    print(objectivevalue)
-
-#    print("solve time:",solveTime)
-    
     return objectivevalue, var_vals, model, list_of_cut_triads, formulation_time, solveTime
 
 
-# In[10]:
-
-
 def run_lp(model, Graph, fixed_ones, fixed_zeros, resolution):
     """
     Run the LP based on model and the original Graph as input
     """
 #     ModularityMatrix = nx.modularity_matrix(Graph, weight='actual_weight')
     ModularityMatrix = get_modularity_matrix(Graph, resolution)
     AdjacencyMatrix = nx.to_numpy_matrix(Graph, weight='actual_weight')
@@ -495,34 +566,23 @@
 
     obj = model.getObjective()
     try:
         obj_val = obj.getValue()
     except AttributeError as error:
         return -1, -1, model
 
-#     objectivevalue = np.round((((2*obj_val)+(ModularityMatrix.trace()[0,0]))/np.sum(AdjacencyMatrix)), 8)
     objectivevalue = np.round((((2*obj_val)+(ModularityMatrix.trace()))/np.sum(AdjacencyMatrix)), 8)
 
-
     var_vals = {}
     for var in model.getVars():
         var_vals[var.varName] = var.x
 
-#    print("\n")
-#    print("Q*:")
-#    print(objectivevalue)
-
-#    print("solve time:",solveTime)
-    
     return objectivevalue, var_vals, model
 
 
-# In[11]:
-
-
 def reset_model_varaibles(model, fixed_ones, fixed_zeros):
     for var_name in fixed_ones:
         var = model.getVarByName(var_name)
         var.setAttr("LB", 0.0)
     model.update()
     for var_name in fixed_zeros:
         var = model.getVarByName(var_name)
@@ -534,17 +594,16 @@
 # In[12]:
 
 
 def calculate_modularity(community, Graph, resolution):
     """
     Method that calculates modularity for input community partition on input Graph
     """
-#     ModularityMatrix = nx.modularity_matrix(Graph, weight="actual_weight")
     ModularityMatrix = get_modularity_matrix(Graph, resolution)
-    AdjacencyMatrix = nx.to_numpy_matrix(Graph, weight="actual_weight")
+    AdjacencyMatrix = nx.adjacency_matrix(Graph, weight="actual_weight")
     OFV=0
     for item in community:
         if len(item)>1:
             for i in range(0,len(item)):
                 for j in range(i+1,len(item)):
                     OFV = OFV + 2*(ModularityMatrix[item[i],item[j]])
 #     OFV = OFV + ModularityMatrix.trace()[0,0]
@@ -632,34 +691,27 @@
             score = 1 - np.exp(-alpha) + beta + (delta/len(list(node.graph.nodes())))
             total_score += score
         score_list.append(total_score)
     sum_of_scores = np.sum(score_list)
     probability_list = [x/sum_of_scores for x in score_list]
     index = np.random.choice(len(violated_triples), p=probability_list)
     return violated_triples[index][:3]
-        
 
-    
-    
-    
-    
-    
-    
-    
 
 def is_integer_solution(Graph, var_vals):
     """
     Return whether all the varaible values are integer
     """
     for i in range(len(Graph.nodes())):
         for j in range(i+1, len(Graph.nodes())):
             if var_vals[str(i) + "," + str(j)] != 1 and var_vals[str(i) + "," + str(j)] != 0:
                 return False
     return True
 
+
 def reduce_triple(G, triple, orig_g, resolution):
     """
     Reduces G by creating a supernode for nodes in triple (for left branching). 
     Returns the reduced graph and the additional edges added for running combo
     """
     new_triple = [-1,-1,-1]
 #         for node in G.nodes():    
@@ -747,15 +799,16 @@
                     Graph.edges[(i, j)]['weight'] = ModularityMatrix[i, j]
             else:
                 Graph.add_edge(i, j)
                 Graph.edges[(i, j)]['weight'] = ModularityMatrix[i, j]
                 Graph.edges[(i, j)]['constrained_modularity'] = False
                 edges_added.append((i, j))
     return Graph, edges_added
-    
+
+
 def alter_modularity(G, triple, orig_g, delta, resolution):
     """
     Alter the modularity associated with nodes in triple by input factor (for right branching).
     Returns the reduced graph and additional edges added for running pycombo
     """
     new_triple = [-1,-1,-1]
     value_zero = orig_g.nodes[triple[0]]['super node of'][0]
@@ -901,30 +954,27 @@
     
     #super node of stores all the nodes that are a part of this super node
     for node in G.nodes():
         G.nodes[node]['super node of'] = [node]
         
     return G
 
-
-# In[16]:
-
-
 def handle_isolated_nodes(Graph):
     isolated = []
     for x in Graph.nodes():
         if Graph.degree[x] == 0:
             isolated.append(x)
     for x in isolated:
         Graph.remove_node(x)
     Graph = nx.convert_node_labels_to_integers(Graph)
     return Graph, isolated
 
+
 def get_modularity_matrix(Graph, resolution):
-    AdjacencyMatrix = nx.to_numpy_matrix(Graph, weight="actual_weight")
+    AdjacencyMatrix = nx.adjacency_matrix(Graph, weight="actual_weight")
     ModularityMatrix = np.empty(AdjacencyMatrix.shape)
     for i in Graph.nodes():
         for j in Graph.nodes():
             deg_i = Graph.degree(i, weight="actual_weight") - AdjacencyMatrix[i, i]
             deg_j = Graph.degree(j, weight="actual_weight") - AdjacencyMatrix[j, j]
             mod = AdjacencyMatrix[i, j] - (((deg_i*deg_j)/(np.sum(AdjacencyMatrix)))*resolution)
             ModularityMatrix[i, j] = mod
@@ -938,38 +988,81 @@
     else:
         gap = (upper_bound - lower_bound) / upper_bound
         out = lower_bound, gap, communities, preprocessing_time+formulation_time, solve_time
     return out
 
 
 def bayan(G, threshold=0.001, time_allowed=600, delta=0.7, resolution=1, lp_method=4, develop_mode=False):
+
+    # Running Bayan for a network with multiple connected components
+    optimal_partition = []
+    list_of_subgraphs = [G.subgraph(c).copy() for c in nx.connected_components(G)]
+    n_sub = len(list_of_subgraphs)
+    sub_results = {}
+    total_gap = 0
+    total_modeling_time = 0
+    total_solve_time = 0
+    total_preprocessing_time = 0
+    total_formulation_time = 0
+    threshold_sub = threshold / n_sub
+    for sub_inx, sub_graph in enumerate(list_of_subgraphs):
+        bayan_output = alg(sub_graph, threshold=threshold_sub, time_allowed=time_allowed, delta=delta,
+              resolution=resolution, lp_method=lp_method, develop_mode=develop_mode)
+
+        if develop_mode:
+            sub_results[sub_inx] = bayan_output
+            optimal_partition += bayan_output[3]
+            total_preprocessing_time += bayan_output[4]
+            total_formulation_time += bayan_output[5]
+            total_solve_time += bayan_output[6]
+
+        else:
+            optimal_partition += bayan_output[2]
+            total_gap += bayan_output[1]
+            total_modeling_time += bayan_output[3]
+            total_solve_time += bayan_output[4]
+
+    lower_bound = calculate_modularity(optimal_partition, G, resolution)
+
+    if develop_mode:
+        for sub_inx, sub_graph in enumerate(list_of_subgraphs):
+            print(f"Connected component {sub_inx}")
+            print(sub_results[sub_inx])
+        out = lower_bound, optimal_partition,  total_preprocessing_time, total_formulation_time,total_solve_time
+    else:
+        out = lower_bound, total_gap, optimal_partition, total_modeling_time, total_solve_time
+
+    return out
+
+
+def alg(G, threshold=0.001, time_allowed=600, delta=0.7, resolution=1, lp_method=4, develop_mode=False):
     """
     Run bayan on input Graph while MIP gap > threshold and runtime < time_allowed (default is 60 seconds)
     """
     run_start = time.time()
     preprocessing_time_start = time.time()
     G = nx.convert_node_labels_to_integers(G, label_attribute="original_label")
     mapping = nx.get_node_attributes(G, 'original_label')
 
     G1 = G.copy()
     orig_graph = create_bayan_edge_attributes(G1, resolution)
     G2 = orig_graph.copy()
     Graph, isolated_nodes = handle_isolated_nodes(G2)
     Graph = clique_filtering(Graph, resolution)
-    AdjacencyMatrix = nx.to_numpy_matrix(Graph, weight="actual_weight")
+    AdjacencyMatrix = nx.adjacency_matrix(Graph, weight="actual_weight")
     ModularityMatrix = get_modularity_matrix(Graph, resolution)
-    size = int(Graph.size(weight='actual_weight'))
-    order = len(AdjacencyMatrix)
+    #size = int(Graph.size(weight='actual_weight'))
+    #order = len(AdjacencyMatrix)
     preprocessing_time = time.time() - preprocessing_time_start
     mod_lp, var_vals, model, list_of_cut_triads, formulation_time, root_lp_time = \
-        lp_formulation(Graph, AdjacencyMatrix, ModularityMatrix, size, order, isolated_nodes, lp_method)
+        lp_formulation(Graph, AdjacencyMatrix, ModularityMatrix, isolated_nodes, lp_method)
     if is_integer_solution(Graph, var_vals):
         return output(mapping, develop_mode, 1, mod_lp, mod_lp, decluster_communities(model_to_communities(var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, root_lp_time)
     root_combo_time_start = time.time()
-    partition_combo = algorithms.pycombo(Graph, weight="actual_weight", modularity_resolution=resolution)
+    partition_combo = pycombo.execute(Graph, weight="actual_weight", modularity_resolution=resolution)
     communities_combo = list(partition_combo.communities)
     communities_combo_declustered = decluster_communities(communities_combo, Graph, isolated_nodes)
     mod_combo = calculate_modularity(communities_combo_declustered, orig_graph, resolution)
     root_combo_time = time.time() - root_combo_time_start
     if mod_lp - mod_combo < threshold:
         return output(mapping, develop_mode,2, mod_combo, mod_lp, communities_combo_declustered, preprocessing_time, formulation_time, root_combo_time+root_lp_time)
     best_bound = mod_lp
@@ -1094,22 +1187,14 @@
         first, second = var.split(",")
         if first == i:
             #FIX corresponding vars to 1 and append to left_fix_ones
             ones.append(str(j)+","+second)
             ones.append(str(k)+","+second)
     return zeros, ones
         
-        
-        
-    
-
-
-# In[48]:
-
-
 def right_implied(right_fix_zeros, branch_triple):
     zeros = right_fix_zeros.copy()
     i = branch_triple[0]
     j = branch_triple[1]
     k = branch_triple[2]
     constraints_to_be_added = []
     for var in right_fix_zeros:
@@ -1117,18 +1202,14 @@
         if first == i:
             constraint = [int(second), int(j), int(k)]
             constraint.sort()
             constraint_tup = (constraint[0], constraint[1], constraint[2], 2)
             constraints_to_be_added.append(constraint_tup)
     return constraints_to_be_added
 
-
-# In[49]:
-
-
 def perform_branch(node, model, incumbent, best_bound, Graph, original_graph, isolated_nodes, list_of_cut_triads, delta, resolution):
     """
     Perform the left and right branch on input node
     """
     violated_triples_dict = node.get_violated_triples(list_of_cut_triads)
     prev_fixed_ones = node.get_fixed_ones().copy()
     prev_fixed_zeros = node.get_fixed_zeros().copy()
@@ -1168,15 +1249,15 @@
         implied_zeros, implied_ones = left_implied(left_fix_ones, left_fix_zeros, branch_triple)
     
     for i in range(count):
         model.remove(model.getConstrByName('branch_' + str(i)))
     model.update()
     
     left_graph, edges_added = reduce_triple(node.graph, branch_triple, Graph, resolution)
-    left_partition_combo = algorithms.pycombo(left_graph, treat_as_modularity=True, modularity_resolution=resolution)
+    left_partition_combo = pycombo.execute(left_graph, treat_as_modularity=True, modularity_resolution=resolution)
     left_communities_combo = list(left_partition_combo.communities)
     left_decluster_combo = decluster_communities(left_communities_combo, left_graph, isolated_nodes)
     left_graph = remove_extra_edges(left_graph, edges_added)
     left_lower_bound = calculate_modularity(left_decluster_combo, original_graph, resolution)
 #    print(left_lower_bound)
     left_constraints = node.constraints.copy()
     left_constraints.append(branch_triple + (0,))
@@ -1191,20 +1272,15 @@
         left_node.set_fixed_zeros(prev_fixed_zeros + left_fix_zeros + implied_zeros)
         if is_integer_solution(left_graph, left_var_vals):
             print("LP solution is integer")
             left_node.set_is_integer()
             left_node.close_node()
         if left_upper_bound <= incumbent:
             left_node.close_node()
-            
-        
-    
-#     model.reset()
-    
-    #Right branch x_ij + x_jk + x_ik >= 2
+    # Right branch x_ij + x_jk + x_ik >= 2
     x_ij = model.getVarByName(str(branch_triple[0]) + "," + str(branch_triple[1]))
     x_jk = model.getVarByName(str(branch_triple[1]) + "," + str(branch_triple[2]))
     x_ik = model.getVarByName(str(branch_triple[0]) + "," + str(branch_triple[2]))
     count = 0
     if node.constraints == []:
         model.addConstr(x_ij + x_jk + x_ik >= 2, 'branch_0')
         count += 1
@@ -1231,58 +1307,32 @@
         implied_constraints = right_implied(right_fix_zeros, branch_triple)
     
     for i in range(count):
         model.remove(model.getConstrByName('branch_' + str(i)))
     model.update()
     
     right_graph, edges_added = alter_modularity(node.graph, branch_triple, Graph, delta, resolution)
-    right_partition_combo = algorithms.pycombo(right_graph, treat_as_modularity=True, modularity_resolution=resolution)
+    right_partition_combo = pycombo.execute(right_graph, treat_as_modularity=True, modularity_resolution=resolution)
     right_communities_combo = list(right_partition_combo.communities)
     right_decluster_combo = decluster_communities(right_communities_combo, right_graph, isolated_nodes)
     right_lower_bound = calculate_modularity(right_decluster_combo, original_graph, resolution)
     right_graph = remove_extra_edges(right_graph, edges_added)
 #    print(right_lower_bound)
     right_constraints = node.constraints.copy()
     right_constraints.append(branch_triple + (2,))
     right_constraints += implied_constraints
     right_node = Node(right_constraints, right_var_vals, right_graph, right_decluster_combo)
     right_node.set_bounds(right_lower_bound, right_upper_bound)
     
-
-    
     if right_upper_bound == -1 and right_var_vals == -1:
         right_node.close_node()
         right_node.set_is_infeasible()
     else:
         right_node.set_fixed_ones(prev_fixed_ones + right_fix_ones)
         right_node.set_fixed_zeros(prev_fixed_zeros + right_fix_zeros)
         if is_integer_solution(right_graph, right_var_vals):
             print("LP solution is integer")
             right_node.set_is_integer()
             right_node.close_node()
         if right_upper_bound <= incumbent:
             right_node.close_node()
     return left_node, right_node
-    
-    
-    
-
-
-# In[230]:
-
-
-# import BayanPost as bayanpostpy
-
-
-# In[229]:
-
-
-# graph = get_graph_from_network_name("football")
-# post_ans = bayanpostpy.bayan(graph, threshold = 0, time_allowed=60)
-
-
-# In[228]:
-
-
-# G = get_graph_from_network_name("football")
-# ans = bayan(G, threshold=0, time_allowed=60)
-
```

### Comparing `bayanpy-0.6.5/setup.py` & `bayanpy-0.6.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.6.5",
+    version="0.6.8",
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
-        "cdlib",
-	    "joblib",
+	 "joblib",
         "pycombo"
     ],
 )
```

