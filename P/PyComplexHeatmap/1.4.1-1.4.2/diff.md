# Comparing `tmp/PyComplexHeatmap-1.4.1.tar.gz` & `tmp/PyComplexHeatmap-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.4.1.tar", last modified: Tue Apr 11 20:53:50 2023, max compression
+gzip compressed data, was "PyComplexHeatmap-1.4.2.tar", last modified: Sun May  7 03:26:15 2023, max compression
```

## Comparing `PyComplexHeatmap-1.4.1.tar` & `PyComplexHeatmap-1.4.2.tar`

### file list

```diff
@@ -1,40 +1,23 @@
-drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 20:53:50.827531 PyComplexHeatmap-1.4.1/
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       31 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/.gitattributes
-drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 20:53:50.759863 PyComplexHeatmap-1.4.1/.github/
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      810 2023-03-30 00:58:12.000000 PyComplexHeatmap-1.4.1/.github/FUNDING.yml
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       13 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/.gitignore
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1067 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/LICENSE
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      105 2023-04-11 15:37:05.000000 PyComplexHeatmap-1.4.1/MANIFEST.in
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    11667 2023-04-11 20:53:50.826660 PyComplexHeatmap-1.4.1/PKG-INFO
-drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 20:53:50.767924 PyComplexHeatmap-1.4.1/PyComplexHeatmap/
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      375 2023-04-11 20:49:25.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/__init__.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    65860 2023-04-11 02:21:02.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/annotations.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    70631 2023-04-11 20:43:59.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     5495 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/colors.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    21247 2023-04-08 14:53:33.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     6766 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/example.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    17814 2023-04-10 00:47:13.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     6753 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/tools.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    25810 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 20:53:50.771625 PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    11667 2023-04-11 20:53:49.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      818 2023-04-11 20:53:50.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        1 2023-04-11 20:53:49.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       17 2023-04-11 20:53:49.000000 PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    11058 2023-04-11 16:07:29.000000 PyComplexHeatmap-1.4.1/README.md
-drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-04-11 20:53:50.825889 PyComplexHeatmap-1.4.1/comparison/
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    88559 2023-04-11 15:48:21.000000 PyComplexHeatmap-1.4.1/comparison/ComplexHeatmap.pdf
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)   319414 2023-04-11 16:01:23.000000 PyComplexHeatmap-1.4.1/comparison/ComplexHeatmap.png
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)   159732 2023-04-11 15:48:48.000000 PyComplexHeatmap-1.4.1/comparison/PyComplexHeatmap.pdf
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)   666164 2023-04-11 16:01:43.000000 PyComplexHeatmap-1.4.1/comparison/PyComplexHeatmap.png
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1434 2023-04-11 16:30:23.000000 PyComplexHeatmap-1.4.1/comparison/README.md
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755) 15584021 2023-04-11 14:18:01.000000 PyComplexHeatmap-1.4.1/comparison/beta.csv
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      205 2023-04-11 15:29:17.000000 PyComplexHeatmap-1.4.1/comparison/compare.sh
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1236 2023-04-11 14:30:03.000000 PyComplexHeatmap-1.4.1/comparison/df_col.csv
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)  2909164 2023-04-11 14:21:19.000000 PyComplexHeatmap-1.4.1/comparison/df_row.csv
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     2469 2023-04-11 15:46:41.000000 PyComplexHeatmap-1.4.1/comparison/heatmap.R
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)   182760 2023-04-11 20:48:31.000000 PyComplexHeatmap-1.4.1/comparison/heatmap.ipynb
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     2159 2023-04-11 15:43:20.000000 PyComplexHeatmap-1.4.1/comparison/heatmap.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      672 2023-04-11 20:49:16.000000 PyComplexHeatmap-1.4.1/pyproject.toml
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       38 2023-04-11 20:53:50.827631 PyComplexHeatmap-1.4.1/setup.cfg
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1044 2023-04-11 20:49:31.000000 PyComplexHeatmap-1.4.1/setup.py
+drwxrwxr-x   0 wding     (8051) wding    (17694)        0 2023-05-07 03:26:15.502252 PyComplexHeatmap-1.4.2/
+-rw-rw-r--   0 wding     (8051) wding    (17694)     1067 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/LICENSE
+-rw-rw-r--   0 wding     (8051) wding    (17694)      105 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/MANIFEST.in
+-rw-rw-r--   0 wding     (8051) wding    (17694)    11704 2023-05-07 03:26:15.487258 PyComplexHeatmap-1.4.2/PKG-INFO
+drwxrwxr-x   0 wding     (8051) wding    (17694)        0 2023-05-07 03:26:15.460256 PyComplexHeatmap-1.4.2/PyComplexHeatmap/
+-rw-rw-r--   0 wding     (8051) wding    (17694)      375 2023-05-07 03:25:44.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/__init__.py
+-rw-rw-r--   0 wding     (8051) wding    (17694)    65607 2023-05-07 01:41:34.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/annotations.py
+-rw-rw-r--   0 wding     (8051) wding    (17694)    70631 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/clustermap.py
+-rw-rw-r--   0 wding     (8051) wding    (17694)     5495 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/colors.py
+-rw-rw-r--   0 wding     (8051) wding    (17694)    21247 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/dotHeatmap.py
+-rw-rw-r--   0 wding     (8051) wding    (17694)     6766 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/example.py
+-rw-rw-r--   0 wding     (8051) wding    (17694)    17814 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/oncoPrint.py
+-rw-rw-r--   0 wding     (8051) wding    (17694)     6753 2023-05-05 16:24:49.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/tools.py
+-rw-rw-r--   0 wding     (8051) wding    (17694)    25817 2023-05-06 22:12:59.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap/utils.py
+drwxrwxr-x   0 wding     (8051) wding    (17694)        0 2023-05-07 03:26:15.486256 PyComplexHeatmap-1.4.2/PyComplexHeatmap.egg-info/
+-rw-rw-r--   0 wding     (8051) wding    (17694)    11704 2023-05-07 03:26:15.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-rw-r--   0 wding     (8051) wding    (17694)      473 2023-05-07 03:26:15.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 wding     (8051) wding    (17694)        1 2023-05-07 03:26:15.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 wding     (8051) wding    (17694)       17 2023-05-07 03:26:15.000000 PyComplexHeatmap-1.4.2/PyComplexHeatmap.egg-info/top_level.txt
+-rw-rw-r--   0 wding     (8051) wding    (17694)    11095 2023-05-05 17:28:56.000000 PyComplexHeatmap-1.4.2/README.md
+-rw-rw-r--   0 wding     (8051) wding    (17694)      672 2023-05-07 03:25:35.000000 PyComplexHeatmap-1.4.2/pyproject.toml
+-rw-rw-r--   0 wding     (8051) wding    (17694)       38 2023-05-07 03:26:15.502256 PyComplexHeatmap-1.4.2/setup.cfg
+-rw-rw-r--   0 wding     (8051) wding    (17694)     1044 2023-05-07 03:25:27.000000 PyComplexHeatmap-1.4.2/setup.py
```

### Comparing `PyComplexHeatmap-1.4.1/LICENSE` & `PyComplexHeatmap-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.1/PKG-INFO` & `PyComplexHeatmap-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.4.1
+Version: 1.4.2
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
@@ -15,25 +15,25 @@
 License-File: LICENSE
 
 # PyComplexHeatmap [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=total&units=international_system&left_color=blue&right_color=black&left_text=Downloads)](https://pepy.tech/project/pycomplexheatmap) [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=month&units=international_system&left_color=green&right_color=orange&left_text=Last%20Month)](https://pepy.tech/project/pycomplexheatmap) [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=week&units=international_system&left_color=red&right_color=brightgreen&left_text=This%20week)](https://pepy.tech/project/pycomplexheatmap)
 PyComplexHeatmap is a Python package to plot complex heatmap (clustermap). Please click [here](https://dingwb.github.io/PyComplexHeatmap) for documentation.
 
 ## Documentation:
 ----------------------
-[https://dingwb.github.io/PyComplexHeatmap](https://dingwb.github.io/PyComplexHeatmap) 
+[https://dingwb.github.io/PyComplexHeatmap](https://dingwb.github.io/PyComplexHeatmap)
 <br><br>
-PYPI:
-<br>
-[https://pypi.org/project/PyComplexHeatmap/](https://pypi.org/project/PyComplexHeatmap/)
+[PYPI](https://pypi.org/project/PyComplexHeatmap/)
 <br>
 
 ### Wiki
 [wiki/layout](../../wiki/Layout/)
 <br>
 [wiki/Parameters](../../wiki/Parameters/)
+<br>
+[wiki/Features](../../wiki/Features/)
 
 ## Dependencies:
 ----------------------
 - matplotlib>=3.4.3
 - numpy
 - pandas
 - scipy
@@ -62,15 +62,15 @@
 OR
 ```shell
 git clone https://github.com/DingWB/PyComplexHeatmap
 cd PyComplexHeatmap
 python setup.py install
 ```
 
-## **Usage**
+## [**Usage**](https://dingwb.github.io/PyComplexHeatmap)
 ----------------------
 ### **1. [Simple Guide To Get started](https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html).**
 ```py
 from PyComplexHeatmap import *
 
 #Generate example dataset (random)
 df = pd.DataFrame(['GroupA'] * 5 + ['GroupB'] * 5, columns=['AB'])
@@ -197,15 +197,14 @@
         </td>
     </tr>
 </table>
 
 ## **More Examples**
 [https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html](https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html)
 
-
 ## Call for Contributions
 ----------------------
 
 The PyComplexHeatmap project welcomes your expertise and enthusiasm!
 
 Small improvements or fixes are always appreciated. If you are considering larger contributions
 to the source code, please contact us (ding.wu.bin.gm@gmail.com).
```

### Comparing `PyComplexHeatmap-1.4.1/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.4.2/PyComplexHeatmap/annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -715,15 +715,15 @@
         if grid:
             ax.grid(linestyle='--', zorder=-10)
         # bar_ct = ax.bar(x=list(range(1, self.nrows + 1,1)),
         #                 height=self.plot_data.values,**self.plot_kws)
         if type(self.colors) == list:
             colors = self.colors
         else: #dict
-            bad_value_color = matplotlib.colors.rgb2hex(plt.get_cmap(self.cmap).get_bad())
+            #bad_value_color = matplotlib.colors.rgb2hex(plt.get_cmap(self.cmap).get_bad())
             # colors = [[self.colors.get(v, bad_value_color) for v in self.plot_data.iloc[:, 0].values]]
             colors = [[self.colors(v) for v in self.plot_data.iloc[:, 0].values]]
         base_coordinates = [0] * self.plot_data.shape[0]
         for col, color in zip(self.plot_data.columns, colors):
             if axis == 1:
                 ax.set_xticks(ticks=np.arange(0.5, self.nrows, 1))
                 ax.bar(x=np.arange(0.5, self.nrows, 1), height=self.plot_data[col].values,
@@ -897,21 +897,20 @@
     legend_vpad: float
         Vertical space between top of ax and legend, default is 2 [mm].
     orientation: str
         up or down, when axis=1
         left or right, when axis=0;
         When anno_label shows up in annotation, the orientation would be automatically be assigned according
         to the position of anno_label.
-    wspace: float
-        optional. The amount of width reserved for space between subplots, expressed as a fraction of the
-        average axis width. If not given, the values will be inferred from a figure or rcParams when necessary. See also GridSpec.get_subplot_params.
-    hspace: float
-        optional
-        The amount of height reserved for space between subplots, expressed as a fraction of the average axis height.
-        If not given, the values will be inferred from a figure or rcParams when necessary. See also GridSpec.get_subplot_params
+    wgap: float or int
+        optional,  the space used to calculate wspace, default is [0.1] (mm),
+        control the vertical gap between two annotations.
+    hgap: float or int
+        optional,  the space used to calculate hspace, default is [0.1] (mm),
+        control the horizontal gap between two annotations.
     plot_legend : bool
         whether to plot legends.
     args : name-value pair
         key is the annotation label (name), values can be a pandas dataframe,
         series, or annotation such as
         anno_simple, anno_boxplot, anno_scatter, anno_label, or anno_barplot.
 
@@ -920,16 +919,15 @@
     Class HeatmapAnnotation.
 
     """
 
     def __init__(self, df=None, axis=1, cmap='auto', colors=None, label_side=None, label_kws=None,
                  ticklabels_kws=None, plot_kws=None, plot=False, legend=True, legend_side='right',
                  legend_gap=5, legend_width=4.5, legend_hpad=2, legend_vpad=5, orientation=None,
-                 wgap=0.1,hgap=0.1,
-                 plot_legend=True, rasterized=False, verbose=1, **args):
+                 wgap=0.1,hgap=0.1,plot_legend=True, rasterized=False, verbose=1, **args):
         if df is None and len(args) == 0:
             raise ValueError("Please specify either df or other args")
         if not df is None and len(args) > 0:
             raise ValueError("df and Name-value pairs can only be given one, not both.")
         if not df is None:
             self._check_df(df)
         else:
```

### Comparing `PyComplexHeatmap-1.4.1/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.4.2/PyComplexHeatmap/clustermap.py`

 * *Files 0% similar despite different names*

```diff
@@ -692,15 +692,15 @@
                  row_cluster=True, col_cluster=True, row_cluster_method='average', row_cluster_metric='correlation',
                  col_cluster_method='average', col_cluster_metric='correlation',
                  show_rownames=False, show_colnames=False, row_names_side='right', col_names_side='bottom',
                  row_dendrogram=False, col_dendrogram=False, row_dendrogram_size=10, col_dendrogram_size=10,
                  row_split=None, col_split=None, dendrogram_kws=None, tree_kws=None,
                  row_split_order=None, col_split_order=None, row_split_gap=0.5, col_split_gap=0.2, mask=None,
                  subplot_gap=1, legend=True, legend_kws=None, plot=True, plot_legend=True,
-                 legend_anchor='auto', legend_gap=5, legend_width=4.5, legend_hpad=2, legend_vpad=5,
+                 legend_anchor='auto', legend_gap=7, legend_width=4.5, legend_hpad=2, legend_vpad=5,
                  legend_side='right', cmap='jet', label=None, xticklabels_kws=None, yticklabels_kws=None,
                  rasterized=False, legend_delta_x=None, verbose=1, **kwargs):
         self.kwargs = kwargs if not kwargs is None else {}
         self.data2d = self.format_data(data, mask, z_score, standard_scale)
         self.verbose=verbose
         self._define_kws(xticklabels_kws, yticklabels_kws)
         self.top_annotation = top_annotation
```

### Comparing `PyComplexHeatmap-1.4.1/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.4.2/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.1/PyComplexHeatmap/dotHeatmap.py` & `PyComplexHeatmap-1.4.2/PyComplexHeatmap/dotHeatmap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.1/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.4.2/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.1/PyComplexHeatmap/oncoPrint.py` & `PyComplexHeatmap-1.4.2/PyComplexHeatmap/oncoPrint.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.1/PyComplexHeatmap/tools.py` & `PyComplexHeatmap-1.4.2/PyComplexHeatmap/tools.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.4.1/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.4.2/PyComplexHeatmap/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     # Choose default colormaps if not provided
     if cmap is None:
         if center is None:
             cmap = 'jet'
         else:
             cmap = 'exp1'
     if isinstance(cmap, str):
-        cmap1 = matplotlib.cm.get_cmap(cmap)
+        cmap1 = matplotlib.cm.get_cmap(cmap).copy()
     elif isinstance(cmap, list):
         cmap1 = matplotlib.colors.ListedColormap(cmap)
     else:
         cmap1 = cmap
 
     cmap1.set_bad(color=na_col)  # set the color for NaN values
     # Recenter a divergent colormap
```

### Comparing `PyComplexHeatmap-1.4.1/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.4.2/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.4.1
+Version: 1.4.2
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
@@ -15,25 +15,25 @@
 License-File: LICENSE
 
 # PyComplexHeatmap [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=total&units=international_system&left_color=blue&right_color=black&left_text=Downloads)](https://pepy.tech/project/pycomplexheatmap) [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=month&units=international_system&left_color=green&right_color=orange&left_text=Last%20Month)](https://pepy.tech/project/pycomplexheatmap) [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=week&units=international_system&left_color=red&right_color=brightgreen&left_text=This%20week)](https://pepy.tech/project/pycomplexheatmap)
 PyComplexHeatmap is a Python package to plot complex heatmap (clustermap). Please click [here](https://dingwb.github.io/PyComplexHeatmap) for documentation.
 
 ## Documentation:
 ----------------------
-[https://dingwb.github.io/PyComplexHeatmap](https://dingwb.github.io/PyComplexHeatmap) 
+[https://dingwb.github.io/PyComplexHeatmap](https://dingwb.github.io/PyComplexHeatmap)
 <br><br>
-PYPI:
-<br>
-[https://pypi.org/project/PyComplexHeatmap/](https://pypi.org/project/PyComplexHeatmap/)
+[PYPI](https://pypi.org/project/PyComplexHeatmap/)
 <br>
 
 ### Wiki
 [wiki/layout](../../wiki/Layout/)
 <br>
 [wiki/Parameters](../../wiki/Parameters/)
+<br>
+[wiki/Features](../../wiki/Features/)
 
 ## Dependencies:
 ----------------------
 - matplotlib>=3.4.3
 - numpy
 - pandas
 - scipy
@@ -62,15 +62,15 @@
 OR
 ```shell
 git clone https://github.com/DingWB/PyComplexHeatmap
 cd PyComplexHeatmap
 python setup.py install
 ```
 
-## **Usage**
+## [**Usage**](https://dingwb.github.io/PyComplexHeatmap)
 ----------------------
 ### **1. [Simple Guide To Get started](https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html).**
 ```py
 from PyComplexHeatmap import *
 
 #Generate example dataset (random)
 df = pd.DataFrame(['GroupA'] * 5 + ['GroupB'] * 5, columns=['AB'])
@@ -197,15 +197,14 @@
         </td>
     </tr>
 </table>
 
 ## **More Examples**
 [https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html](https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html)
 
-
 ## Call for Contributions
 ----------------------
 
 The PyComplexHeatmap project welcomes your expertise and enthusiasm!
 
 Small improvements or fixes are always appreciated. If you are considering larger contributions
 to the source code, please contact us (ding.wu.bin.gm@gmail.com).
```

### Comparing `PyComplexHeatmap-1.4.1/README.md` & `PyComplexHeatmap-1.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # PyComplexHeatmap [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=total&units=international_system&left_color=blue&right_color=black&left_text=Downloads)](https://pepy.tech/project/pycomplexheatmap) [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=month&units=international_system&left_color=green&right_color=orange&left_text=Last%20Month)](https://pepy.tech/project/pycomplexheatmap) [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=week&units=international_system&left_color=red&right_color=brightgreen&left_text=This%20week)](https://pepy.tech/project/pycomplexheatmap)
 PyComplexHeatmap is a Python package to plot complex heatmap (clustermap). Please click [here](https://dingwb.github.io/PyComplexHeatmap) for documentation.
 
 ## Documentation:
 ----------------------
-[https://dingwb.github.io/PyComplexHeatmap](https://dingwb.github.io/PyComplexHeatmap) 
+[https://dingwb.github.io/PyComplexHeatmap](https://dingwb.github.io/PyComplexHeatmap)
 <br><br>
-PYPI:
-<br>
-[https://pypi.org/project/PyComplexHeatmap/](https://pypi.org/project/PyComplexHeatmap/)
+[PYPI](https://pypi.org/project/PyComplexHeatmap/)
 <br>
 
 ### Wiki
 [wiki/layout](../../wiki/Layout/)
 <br>
 [wiki/Parameters](../../wiki/Parameters/)
+<br>
+[wiki/Features](../../wiki/Features/)
 
 ## Dependencies:
 ----------------------
 - matplotlib>=3.4.3
 - numpy
 - pandas
 - scipy
@@ -46,15 +46,15 @@
 OR
 ```shell
 git clone https://github.com/DingWB/PyComplexHeatmap
 cd PyComplexHeatmap
 python setup.py install
 ```
 
-## **Usage**
+## [**Usage**](https://dingwb.github.io/PyComplexHeatmap)
 ----------------------
 ### **1. [Simple Guide To Get started](https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/advanced_usage.html).**
 ```py
 from PyComplexHeatmap import *
 
 #Generate example dataset (random)
 df = pd.DataFrame(['GroupA'] * 5 + ['GroupB'] * 5, columns=['AB'])
@@ -181,15 +181,14 @@
         </td>
     </tr>
 </table>
 
 ## **More Examples**
 [https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html](https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html)
 
-
 ## Call for Contributions
 ----------------------
 
 The PyComplexHeatmap project welcomes your expertise and enthusiasm!
 
 Small improvements or fixes are always appreciated. If you are considering larger contributions
 to the source code, please contact us (ding.wu.bin.gm@gmail.com).
```

### Comparing `PyComplexHeatmap-1.4.1/pyproject.toml` & `PyComplexHeatmap-1.4.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","matplotlib>=3.5.1","numpy>=1.20.3","pandas>=1.4.1", "scipy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyComplexHeatmap"
-version = "1.4.1"
+version = "1.4.2"
 authors = [
   { name="Wubin Ding", email="ding.wu.bin.gm@gmail.com" },
 ]
 description = "A python package to plot complex heatmap"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `PyComplexHeatmap-1.4.1/setup.py` & `PyComplexHeatmap-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 # print(long_description)
 
 #release new version
 setup(
    name='PyComplexHeatmap',
-   version='1.4.1',
+   version='1.4.2',
    description='A Python package to plot complex heatmap',
    # long_description="#PyComplexHeatmap\n##Documentation:https://dingwb.github.io/PyComplexHeatmap/build/html/index.html",
    # long_description_content_type='text/markdown',
    author='Wubin Ding',
    author_email='ding.wu.bin.gm@gmail.com',
    url="https://github.com/DingWB/PyComplexHeatmap",
    packages=['PyComplexHeatmap'], #src
```

