# Comparing `tmp/bayanpy-0.6.8.tar.gz` & `tmp/bayanpy-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.6.8.tar", last modified: Sun May  7 16:01:02 2023, max compression
+gzip compressed data, was "bayanpy-0.6.9.tar", last modified: Sun May  7 16:47:29 2023, max compression
```

## Comparing `bayanpy-0.6.8.tar` & `bayanpy-0.6.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-07 16:01:02.612158 bayanpy-0.6.8/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.8/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-07 16:01:02.612158 bayanpy-0.6.8/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5041 2023-05-07 15:46:50.000000 bayanpy-0.6.8/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-07 16:01:02.612158 bayanpy-0.6.8/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    57258 2023-05-07 15:37:43.000000 bayanpy-0.6.8/bayanpy/BayanImplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.6.8/bayanpy/__init__.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-07 16:01:02.612158 bayanpy-0.6.8/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-07 16:01:02.000000 bayanpy-0.6.8/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-05-07 16:01:02.000000 bayanpy-0.6.8/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-05-07 16:01:02.000000 bayanpy-0.6.8/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-05-07 16:01:02.000000 bayanpy-0.6.8/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-05-07 16:01:02.000000 bayanpy-0.6.8/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-05-07 16:01:02.612158 bayanpy-0.6.8/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-05-07 16:00:44.000000 bayanpy-0.6.8/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-07 16:47:29.716472 bayanpy-0.6.9/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.9/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-07 16:47:29.716472 bayanpy-0.6.9/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5041 2023-05-07 15:46:50.000000 bayanpy-0.6.9/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-07 16:47:29.716472 bayanpy-0.6.9/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    57440 2023-05-07 16:46:56.000000 bayanpy-0.6.9/bayanpy/BayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.6.9/bayanpy/__init__.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-07 16:47:29.716472 bayanpy-0.6.9/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-07 16:47:29.000000 bayanpy-0.6.9/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-05-07 16:47:29.000000 bayanpy-0.6.9/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-05-07 16:47:29.000000 bayanpy-0.6.9/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-05-07 16:47:29.000000 bayanpy-0.6.9/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-05-07 16:47:29.000000 bayanpy-0.6.9/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-05-07 16:47:29.716472 bayanpy-0.6.9/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-05-07 16:47:17.000000 bayanpy-0.6.9/setup.py
```

### Comparing `bayanpy-0.6.8/LICENSE` & `bayanpy-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.8/README.md` & `bayanpy-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.8/bayanpy/BayanImplied.py` & `bayanpy-0.6.9/bayanpy/BayanImplied.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,15 @@
     solver.options['Threads'] = min(64, multiprocessing.cpu_count())
     solver.options['OutputFlag'] = 0
 
     # Using a warm start
     if warmstart == 1:
         # Solution from Combo algorithm to be used as warm-start
         partition = pycombo.execute(Graph, modularity_resolution=resolution)
-        community_combo = list(partition.communities)
+        community_combo = convert_to_com_list(partition[0])
         for i in (Graph).nodes():
             for j in filter(lambda x: x > i, (Graph).nodes()):
                 if find_in_list_of_list(community_combo, i) == find_in_list_of_list(community_combo, j):
                     model.x[i, j].value = 0
                 else:
                     model.x[i, j].value = 1
         solver.options['WarmStart'] = 1
@@ -398,15 +398,15 @@
 
 
 def run_lp_pyomo(model, Graph, fixed_ones, fixed_zeros, resolution, lp_method):
     """
     Run the LP based on model and the original Graph as input
     """
     ModularityMatrix = get_modularity_matrix(Graph, resolution)
-    AdjacencyMatrix = nx.to_numpy_matrix(Graph, weight='actual_weight')
+    AdjacencyMatrix = nx.adjacency_matrix(Graph, weight='actual_weight')
 
     # Fix variables
     for (i, j) in fixed_ones:
         model.x[i, j].fix(1)
     for (i, j) in fixed_zeros:
         model.x[i, j].fix(0)
 
@@ -502,15 +502,15 @@
     # Using a warm start
     # A known partition can be used as a starting point to "warm-start" the algorithm.
     # It can be provided to the model here by giving start values to the decision variables:
     # If this optional step is skipped, you should comment out these five lines
     if warmstart==1:
         #Solution from Combo algorithm to be used as warm-start
         partition = pycombo.execute(Graph, modularity_resolution=resolution)
-        community_combo=list(partition.communities)
+        community_combo=convert_to_com_list(partition[0])
         for i in (Graph).nodes():
             for j in filter(lambda x: x>i, (Graph).nodes()):
                 if find_in_list_of_list(community_combo,i)==find_in_list_of_list(community_combo,j):
                     x[(i, j)].start = 0
                 else:
                     x[(i, j)].start = 1
     # branching priority is based on total degrees of pairs of nodes
@@ -545,15 +545,15 @@
 
 def run_lp(model, Graph, fixed_ones, fixed_zeros, resolution):
     """
     Run the LP based on model and the original Graph as input
     """
 #     ModularityMatrix = nx.modularity_matrix(Graph, weight='actual_weight')
     ModularityMatrix = get_modularity_matrix(Graph, resolution)
-    AdjacencyMatrix = nx.to_numpy_matrix(Graph, weight='actual_weight')
+    AdjacencyMatrix = nx.adjacency_matrix(Graph, weight='actual_weight')
     
     for var_name in fixed_ones:
         var = model.getVarByName(var_name)
         var.setAttr("LB", 1.0)
     model.update()
     for var_name in fixed_zeros:
         var = model.getVarByName(var_name)
@@ -851,16 +851,15 @@
     """
     for edge in edge_list:
         Graph.remove_edge(edge[0], edge[1])
     return Graph
 
 
 def reduced_cost_variable_fixing(model, var_vals, obj_value, lower_bound, Graph, resolution):
-    AdjacencyMatrix = nx.to_numpy_matrix(Graph, weight="actual_weight")
-#     ModularityMatrix = nx.modularity_matrix(Graph, weight="actual_weight")
+    AdjacencyMatrix = nx.adjacency_matrix(Graph, weight="actual_weight")
     ModularityMatrix = get_modularity_matrix(Graph, resolution)
 #     new_obj_val = ((obj_value*np.sum(AdjacencyMatrix)) - ModularityMatrix.trace()[0, 0])/2
 #     new_lower_bound = ((lower_bound*np.sum(AdjacencyMatrix)) - ModularityMatrix.trace()[0, 0])/2
     new_obj_val = ((obj_value*np.sum(AdjacencyMatrix)) - ModularityMatrix.trace())/2
     new_lower_bound = ((lower_bound*np.sum(AdjacencyMatrix)) - ModularityMatrix.trace())/2
     vars_one = []
     vars_zero = []
@@ -965,38 +964,51 @@
             isolated.append(x)
     for x in isolated:
         Graph.remove_node(x)
     Graph = nx.convert_node_labels_to_integers(Graph)
     return Graph, isolated
 
 
+def convert_to_com_list(com_dict):
+    out = {}
+    for node, com_id in com_dict.items():
+        if com_id in out.keys():
+            out[com_id].append(node)
+        else:
+            out[com_id] = [node]
+
+    out = [com for com in out.values()]
+    return out
+
+
 def get_modularity_matrix(Graph, resolution):
     AdjacencyMatrix = nx.adjacency_matrix(Graph, weight="actual_weight")
     ModularityMatrix = np.empty(AdjacencyMatrix.shape)
     for i in Graph.nodes():
         for j in Graph.nodes():
             deg_i = Graph.degree(i, weight="actual_weight") - AdjacencyMatrix[i, i]
             deg_j = Graph.degree(j, weight="actual_weight") - AdjacencyMatrix[j, j]
             mod = AdjacencyMatrix[i, j] - (((deg_i*deg_j)/(np.sum(AdjacencyMatrix)))*resolution)
             ModularityMatrix[i, j] = mod
     return ModularityMatrix
 
 
-def output(mapping, develop, state, lower_bound, upper_bound, communities, preprocessing_time, formulation_time, solve_time):
-    communities = [[mapping[i] for i in com] for com in communities]
+def output(develop, state, lower_bound, upper_bound, communities, preprocessing_time, formulation_time, solve_time):
+
     if develop:
         out = state, lower_bound, upper_bound, communities, preprocessing_time, formulation_time, solve_time
     else:
         gap = (upper_bound - lower_bound) / upper_bound
         out = lower_bound, gap, communities, preprocessing_time+formulation_time, solve_time
     return out
 
 
 def bayan(G, threshold=0.001, time_allowed=600, delta=0.7, resolution=1, lp_method=4, develop_mode=False):
-
+    G = nx.convert_node_labels_to_integers(G, label_attribute="original_label")
+    mapping = nx.get_node_attributes(G, 'original_label')
     # Running Bayan for a network with multiple connected components
     optimal_partition = []
     list_of_subgraphs = [G.subgraph(c).copy() for c in nx.connected_components(G)]
     n_sub = len(list_of_subgraphs)
     sub_results = {}
     total_gap = 0
     total_modeling_time = 0
@@ -1016,17 +1028,19 @@
             total_solve_time += bayan_output[6]
 
         else:
             optimal_partition += bayan_output[2]
             total_gap += bayan_output[1]
             total_modeling_time += bayan_output[3]
             total_solve_time += bayan_output[4]
-
+    print(optimal_partition)
     lower_bound = calculate_modularity(optimal_partition, G, resolution)
 
+    optimal_partition = [[mapping[i] for i in com] for com in optimal_partition]
+
     if develop_mode:
         for sub_inx, sub_graph in enumerate(list_of_subgraphs):
             print(f"Connected component {sub_inx}")
             print(sub_results[sub_inx])
         out = lower_bound, optimal_partition,  total_preprocessing_time, total_formulation_time,total_solve_time
     else:
         out = lower_bound, total_gap, optimal_partition, total_modeling_time, total_solve_time
@@ -1036,39 +1050,37 @@
 
 def alg(G, threshold=0.001, time_allowed=600, delta=0.7, resolution=1, lp_method=4, develop_mode=False):
     """
     Run bayan on input Graph while MIP gap > threshold and runtime < time_allowed (default is 60 seconds)
     """
     run_start = time.time()
     preprocessing_time_start = time.time()
-    G = nx.convert_node_labels_to_integers(G, label_attribute="original_label")
-    mapping = nx.get_node_attributes(G, 'original_label')
-
     G1 = G.copy()
     orig_graph = create_bayan_edge_attributes(G1, resolution)
     G2 = orig_graph.copy()
     Graph, isolated_nodes = handle_isolated_nodes(G2)
     Graph = clique_filtering(Graph, resolution)
     AdjacencyMatrix = nx.adjacency_matrix(Graph, weight="actual_weight")
     ModularityMatrix = get_modularity_matrix(Graph, resolution)
     #size = int(Graph.size(weight='actual_weight'))
     #order = len(AdjacencyMatrix)
     preprocessing_time = time.time() - preprocessing_time_start
     mod_lp, var_vals, model, list_of_cut_triads, formulation_time, root_lp_time = \
         lp_formulation(Graph, AdjacencyMatrix, ModularityMatrix, isolated_nodes, lp_method)
     if is_integer_solution(Graph, var_vals):
-        return output(mapping, develop_mode, 1, mod_lp, mod_lp, decluster_communities(model_to_communities(var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, root_lp_time)
+        return output(develop_mode, 1, mod_lp, mod_lp, decluster_communities(model_to_communities(var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, root_lp_time)
     root_combo_time_start = time.time()
     partition_combo = pycombo.execute(Graph, weight="actual_weight", modularity_resolution=resolution)
-    communities_combo = list(partition_combo.communities)
+    communities_combo = convert_to_com_list(partition_combo[0])
     communities_combo_declustered = decluster_communities(communities_combo, Graph, isolated_nodes)
     mod_combo = calculate_modularity(communities_combo_declustered, orig_graph, resolution)
     root_combo_time = time.time() - root_combo_time_start
+
     if mod_lp - mod_combo < threshold:
-        return output(mapping, develop_mode,2, mod_combo, mod_lp, communities_combo_declustered, preprocessing_time, formulation_time, root_combo_time+root_lp_time)
+        return output(develop_mode,2, mod_combo, mod_lp, communities_combo_declustered, preprocessing_time, formulation_time, root_combo_time+root_lp_time)
     best_bound = mod_lp
     incumbent = mod_combo
     root = Node([], var_vals, Graph, communities_combo_declustered)
     root.set_level(0)
     root.set_bounds(mod_combo, mod_lp)
     var_fixed_ones, var_fixed_zeros = reduced_cost_variable_fixing(model, var_vals, mod_lp, incumbent, Graph, resolution)
     root.set_fixed_ones(var_fixed_ones)
@@ -1084,19 +1096,19 @@
         nodes_current_level = []
         lower_bounds = []
         upper_bounds = []
         for node in nodes_previous_level:
             if time.time() - solve_start - root_time >= time_allowed:
                 if best_combo.is_integer:
                     if best_combo.lower_bound <= best_combo.upper_bound:
-                        return output(mapping, develop_mode,3, best_combo.upper_bound, best_combo.upper_bound, decluster_communities(model_to_communities(best_combo.var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, time.time() - solve_start + root_time)
+                        return output(develop_mode,3, best_combo.upper_bound, best_combo.upper_bound, decluster_communities(model_to_communities(best_combo.var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, time.time() - solve_start + root_time)
                     else:
-                        return output(mapping, develop_mode,4, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time)
+                        return output(develop_mode,4, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time)
                 else:
-                    return output(mapping, develop_mode,5, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time)
+                    return output(develop_mode,5, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time)
             current_node = node
             left_node, right_node = perform_branch(node, model, incumbent, best_bound, Graph, orig_graph, isolated_nodes, list_of_cut_triads, delta, resolution)
             if left_node.close:
                 print("Left node is closed")
                 if left_node.is_integer and incumbent <= left_node.upper_bound:
                     incumbent = left_node.upper_bound
                     best_combo = left_node
@@ -1161,19 +1173,19 @@
                 nodes_p_level.append(a)
         nodes_previous_level = nodes_p_level
         
 #     print(best_combo.lower_bound, best_combo.upper_bound)
 #     print(best_lp.lower_bound, best_lp.upper_bound)
     if best_combo.is_integer:
         if best_combo.lower_bound <= best_combo.upper_bound:
-            return output(mapping, develop_mode,6, best_combo.upper_bound, best_combo.upper_bound, decluster_communities(model_to_communities(best_combo.var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, time.time() - solve_start + root_time)
+            return output(develop_mode, 6, best_combo.upper_bound, best_combo.upper_bound, decluster_communities(model_to_communities(best_combo.var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, time.time() - solve_start + root_time)
         else:
-            return output(mapping, develop_mode,7, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time)
+            return output(develop_mode,7, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time)
     else:
-        return output(mapping, develop_mode,8, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time)
+        return output(develop_mode,8, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time)
 
 def left_implied(left_fix_ones, left_fix_zeros, branch_triple):
     ones = left_fix_ones.copy()
     zeros = left_fix_zeros.copy()
     i = branch_triple[0]
     j = branch_triple[1]
     k = branch_triple[2]
@@ -1250,15 +1262,15 @@
     
     for i in range(count):
         model.remove(model.getConstrByName('branch_' + str(i)))
     model.update()
     
     left_graph, edges_added = reduce_triple(node.graph, branch_triple, Graph, resolution)
     left_partition_combo = pycombo.execute(left_graph, treat_as_modularity=True, modularity_resolution=resolution)
-    left_communities_combo = list(left_partition_combo.communities)
+    left_communities_combo = convert_to_com_list(left_partition_combo[0])
     left_decluster_combo = decluster_communities(left_communities_combo, left_graph, isolated_nodes)
     left_graph = remove_extra_edges(left_graph, edges_added)
     left_lower_bound = calculate_modularity(left_decluster_combo, original_graph, resolution)
 #    print(left_lower_bound)
     left_constraints = node.constraints.copy()
     left_constraints.append(branch_triple + (0,))
     left_node = Node(left_constraints, left_var_vals, left_graph, left_decluster_combo)
@@ -1308,15 +1320,15 @@
     
     for i in range(count):
         model.remove(model.getConstrByName('branch_' + str(i)))
     model.update()
     
     right_graph, edges_added = alter_modularity(node.graph, branch_triple, Graph, delta, resolution)
     right_partition_combo = pycombo.execute(right_graph, treat_as_modularity=True, modularity_resolution=resolution)
-    right_communities_combo = list(right_partition_combo.communities)
+    right_communities_combo = convert_to_com_list(right_partition_combo[0])
     right_decluster_combo = decluster_communities(right_communities_combo, right_graph, isolated_nodes)
     right_lower_bound = calculate_modularity(right_decluster_combo, original_graph, resolution)
     right_graph = remove_extra_edges(right_graph, edges_added)
 #    print(right_lower_bound)
     right_constraints = node.constraints.copy()
     right_constraints.append(branch_triple + (2,))
     right_constraints += implied_constraints
```

### Comparing `bayanpy-0.6.8/setup.py` & `bayanpy-0.6.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.6.8",
+    version="0.6.9",
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
```

