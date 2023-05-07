# Comparing `tmp/intervalframe-1.0.0.tar.gz` & `tmp/intervalframe-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intervalframe-1.0.0.tar", last modified: Mon Jan  3 18:58:18 2022, max compression
+gzip compressed data, was "intervalframe-1.1.1.tar", max compression
```

## Comparing `intervalframe-1.0.0.tar` & `intervalframe-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,43 @@
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-03 18:58:18.317504 intervalframe-1.0.0/
--rwxr--r--   0 ksmith10 (271238760) 633320910    17895 2019-08-12 18:05:36.000000 intervalframe-1.0.0/LICENSE.md
--rw-r--r--   0 ksmith10 (271238760) 633320910     2378 2022-01-03 18:58:18.317772 intervalframe-1.0.0/PKG-INFO
--rwxr--r--   0 ksmith10 (271238760) 633320910     1041 2021-08-28 15:06:59.000000 intervalframe-1.0.0/README.md
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-03 18:58:18.308586 intervalframe-1.0.0/intervalframe/
--rw-r--r--   0 ksmith10 (271238760) 633320910      444 2022-01-03 18:58:14.000000 intervalframe-1.0.0/intervalframe/__init__.py
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-03 18:58:18.312205 intervalframe-1.0.0/intervalframe/core/
--rw-r--r--   0 ksmith10 (271238760) 633320910    25370 2022-01-03 04:00:38.000000 intervalframe-1.0.0/intervalframe/core/IntervalFrame.py
--rw-r--r--   0 ksmith10 (271238760) 633320910    18368 2021-06-07 16:02:28.000000 intervalframe-1.0.0/intervalframe/core/IntervalSeries.py
--rw-r--r--   0 ksmith10 (271238760) 633320910     1244 2020-06-30 16:23:05.000000 intervalframe-1.0.0/intervalframe/core/groupby.py
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-03 18:58:18.312486 intervalframe-1.0.0/intervalframe/core/index/
--rw-r--r--   0 ksmith10 (271238760) 633320910     6726 2021-12-17 13:29:58.000000 intervalframe-1.0.0/intervalframe/core/index/indexers.py
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-03 18:58:18.313558 intervalframe-1.0.0/intervalframe/read/
--rw-r--r--   0 ksmith10 (271238760) 633320910    20974 2021-02-11 01:01:08.000000 intervalframe-1.0.0/intervalframe/read/h5_utilities.py
--rw-r--r--   0 ksmith10 (271238760) 633320910     3354 2021-04-21 15:10:52.000000 intervalframe-1.0.0/intervalframe/read/read_h5.py
--rw-r--r--   0 ksmith10 (271238760) 633320910     1454 2021-12-10 18:58:10.000000 intervalframe-1.0.0/intervalframe/read/read_text.py
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-03 18:58:18.313876 intervalframe-1.0.0/intervalframe/utilities/
--rw-r--r--   0 ksmith10 (271238760) 633320910    20967 2020-07-10 01:08:55.000000 intervalframe-1.0.0/intervalframe/utilities/h5_utilities.py
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-03 18:58:18.315400 intervalframe-1.0.0/intervalframe/write/
--rw-r--r--   0 ksmith10 (271238760) 633320910    20967 2020-07-10 01:08:55.000000 intervalframe-1.0.0/intervalframe/write/h5_utilities.py
--rw-r--r--   0 ksmith10 (271238760) 633320910     3714 2021-04-19 20:02:54.000000 intervalframe-1.0.0/intervalframe/write/write_h5.py
--rw-r--r--   0 ksmith10 (271238760) 633320910        0 2020-07-22 20:58:51.000000 intervalframe-1.0.0/intervalframe/write/write_text.py
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-03 18:58:18.310862 intervalframe-1.0.0/intervalframe.egg-info/
--rw-r--r--   0 ksmith10 (271238760) 633320910     2378 2022-01-03 18:58:18.000000 intervalframe-1.0.0/intervalframe.egg-info/PKG-INFO
--rw-r--r--   0 ksmith10 (271238760) 633320910      677 2022-01-03 18:58:18.000000 intervalframe-1.0.0/intervalframe.egg-info/SOURCES.txt
--rw-r--r--   0 ksmith10 (271238760) 633320910        1 2022-01-03 18:58:18.000000 intervalframe-1.0.0/intervalframe.egg-info/dependency_links.txt
--rw-r--r--   0 ksmith10 (271238760) 633320910        1 2022-01-03 18:57:52.000000 intervalframe-1.0.0/intervalframe.egg-info/not-zip-safe
--rw-r--r--   0 ksmith10 (271238760) 633320910       42 2022-01-03 18:58:18.000000 intervalframe-1.0.0/intervalframe.egg-info/requires.txt
--rw-r--r--   0 ksmith10 (271238760) 633320910       14 2022-01-03 18:58:18.000000 intervalframe-1.0.0/intervalframe.egg-info/top_level.txt
--rwxr--r--   0 ksmith10 (271238760) 633320910       79 2022-01-03 18:58:18.318593 intervalframe-1.0.0/setup.cfg
--rwxr--r--   0 ksmith10 (271238760) 633320910     4349 2022-01-03 18:55:49.000000 intervalframe-1.0.0/setup.py
-drwxr-xr-x   0 ksmith10 (271238760) 633320910        0 2022-01-03 18:58:18.316901 intervalframe-1.0.0/test/
--rw-r--r--   0 ksmith10 (271238760) 633320910     2061 2021-02-12 22:18:27.000000 intervalframe-1.0.0/test/test.py
+-rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 intervalframe-1.1.1/LICENSE.md
+-rwxr-xr-x   0        0        0     1017 2022-01-03 18:58:56.000000 intervalframe-1.1.1/README.md
+-rw-r--r--   0        0        0     6148 2023-05-06 21:49:29.742968 intervalframe-1.1.1/intervalframe/.DS_Store
+-rw-r--r--   0        0        0      444 2023-05-07 12:06:17.723328 intervalframe-1.1.1/intervalframe/__init__.py
+-rw-r--r--   0        0        0     6148 2023-02-02 16:32:30.612368 intervalframe-1.1.1/intervalframe/core/.DS_Store
+-rw-r--r--   0        0        0    35644 2023-04-20 03:11:01.689833 intervalframe-1.1.1/intervalframe/core/IntervalFrame.py
+-rw-r--r--   0        0        0    17962 2023-05-06 21:51:36.202476 intervalframe-1.1.1/intervalframe/core/IntervalSeries.py
+-rw-r--r--   0        0        0    13847 2021-02-11 01:00:19.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalFrame.cpython-36.pyc
+-rw-r--r--   0        0        0     2412 2020-06-20 18:07:35.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalFrame.cpython-37.pyc
+-rw-r--r--   0        0        0    14936 2020-08-07 02:06:35.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalFrame.cpython-38.pyc
+-rw-r--r--   0        0        0    17497 2022-01-10 22:35:33.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalFrame.cpython-39.pyc
+-rw-r--r--   0        0        0    16411 2020-08-12 17:39:28.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalFrame2.cpython-36.pyc
+-rw-r--r--   0        0        0    15354 2020-08-07 16:54:53.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalFrame2.cpython-38.pyc
+-rw-r--r--   0        0        0    14341 2021-09-21 15:04:53.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/IntervalSeries.cpython-39.pyc
+-rw-r--r--   0        0        0     1668 2020-06-30 16:23:11.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/groupby.cpython-36.pyc
+-rw-r--r--   0        0        0     1705 2020-07-23 15:49:38.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/groupby.cpython-38.pyc
+-rw-r--r--   0        0        0    13606 2020-08-05 01:16:10.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/indexing.cpython-36.pyc
+-rw-r--r--   0        0        0    13148 2020-08-03 18:50:48.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/indexing.cpython-38.pyc
+-rw-r--r--   0        0        0     6239 2020-08-12 17:39:28.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/indexing2.cpython-36.pyc
+-rw-r--r--   0        0        0     6207 2020-08-07 14:44:23.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/indexing2.cpython-38.pyc
+-rw-r--r--   0        0        0    20091 2020-08-05 01:16:10.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/multi_indexing.cpython-36.pyc
+-rw-r--r--   0        0        0    19570 2020-08-07 02:07:14.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/multi_indexing.cpython-38.pyc
+-rw-r--r--   0        0        0    11416 2020-08-12 18:16:35.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/multi_indexing2.cpython-36.pyc
+-rw-r--r--   0        0        0     9820 2020-08-07 16:58:33.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/multi_indexing2.cpython-38.pyc
+-rw-r--r--   0        0        0      611 2020-07-04 18:32:05.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/utilities.cpython-36.pyc
+-rw-r--r--   0        0        0      636 2020-07-23 15:49:38.000000 intervalframe-1.1.1/intervalframe/core/__pycache__/utilities.cpython-38.pyc
+-rw-r--r--   0        0        0     1244 2020-06-30 16:23:05.000000 intervalframe-1.1.1/intervalframe/core/groupby.py
+-rw-r--r--   0        0        0     4299 2022-01-10 22:35:34.000000 intervalframe-1.1.1/intervalframe/core/index/__pycache__/indexers.cpython-39.pyc
+-rw-r--r--   0        0        0     6980 2023-02-02 17:51:34.367876 intervalframe-1.1.1/intervalframe/core/index/indexers.py
+-rw-r--r--   0        0        0     2473 2021-09-21 15:04:53.000000 intervalframe-1.1.1/intervalframe/read/__pycache__/read_h5.cpython-39.pyc
+-rw-r--r--   0        0        0     1191 2022-01-10 22:35:34.000000 intervalframe-1.1.1/intervalframe/read/__pycache__/read_text.cpython-39.pyc
+-rw-r--r--   0        0        0    20974 2021-02-11 01:01:08.000000 intervalframe-1.1.1/intervalframe/read/h5_utilities.py
+-rw-r--r--   0        0        0     6848 2023-03-25 17:26:19.423023 intervalframe-1.1.1/intervalframe/read/read_h5.py
+-rw-r--r--   0        0        0      815 2023-01-26 17:56:39.789523 intervalframe-1.1.1/intervalframe/read/read_parquet.py
+-rw-r--r--   0        0        0     2453 2023-01-26 20:00:28.520286 intervalframe-1.1.1/intervalframe/read/read_text.py
+-rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.1/intervalframe/utilities/h5_utilities.py
+-rw-r--r--   0        0        0     2856 2021-09-21 15:04:53.000000 intervalframe-1.1.1/intervalframe/write/__pycache__/write_h5.cpython-39.pyc
+-rw-r--r--   0        0        0    20967 2020-07-10 01:08:55.000000 intervalframe-1.1.1/intervalframe/write/h5_utilities.py
+-rw-r--r--   0        0        0     7192 2023-03-25 13:52:13.113838 intervalframe-1.1.1/intervalframe/write/write_h5.py
+-rw-r--r--   0        0        0      736 2023-01-30 21:43:29.435395 intervalframe-1.1.1/intervalframe/write/write_parquet.py
+-rw-r--r--   0        0        0        0 2020-07-22 20:58:51.000000 intervalframe-1.1.1/intervalframe/write/write_text.py
+-rw-r--r--   0        0        0     1992 2023-05-07 12:06:29.926871 intervalframe-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 intervalframe-1.1.1/PKG-INFO
```

### Comparing `intervalframe-1.0.0/LICENSE.md` & `intervalframe-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `intervalframe-1.0.0/README.md` & `intervalframe-1.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 ```
     pip install -r requirements.txt
 ```
 
 PyPI install, presuming you have all its requirements installed:
 ```
-    NOT AVAILABLE...YET
 	pip install intervalframe
 ```
 
 ## Usage
 
 ```python
 from intervalframe import IntervalFrame
```

### Comparing `intervalframe-1.0.0/intervalframe/core/IntervalFrame.py` & `intervalframe-1.1.1/intervalframe/core/IntervalSeries.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,200 +1,157 @@
 from ailist import IntervalArray, LabeledIntervalArray
 import pandas as pd
 import numpy as np
 import copy as cp
-from .index.indexers import iLocator, Locator
+from .index import indexers
 from tabulate import tabulate
-from bcpseg import bcpseg
-import cbseg
+import linear_segment
 from collections import Counter
+from . import IntervalFrame
 
 
 #_mpl_repr
-class IntervalFrame(object):
+class IntervalSeries(object):
     """
     Annotated augmented interval list
 
     :class:`~intervalframe.IntervalFrame` stores a intervals
     """
 
-    def __init__(self, intervals=None, df=None, labels=None, columns=None, dtypes=None,
-                 copy_df=False, copy_intervals=False):
+    def __init__(self, intervals, series=None, labels=None, dtype=None,
+                 copy_series=False, copy_intervals=False):
         """
         Initialize IntervalFrame
 
         Parameters
         ----------
             intervals : AIList
                 Intervals to be stored
-            df : pandas.DataFrame
+            sereis : pandas.Series
                 DataFrame to annotate intervals with
             labels : array-like
                 Labels for hierarchical indexing
-            columns :  array-like
-                Columns for DataFrame
-            dtypes : dict
-                Dtype for DataFrame columns
-            copy_df : bool
-                Whether to copy DataFrame
+            dtype : 
+                Dtype of series
+            copy_sereies : bool
+                Whether to copy Series
             copy_intervals : bool
                 Whether to copy AIList
 
         Returns
         -------
             None
 
         """
 
         # Determine if intervals need to be copied
-        if copy_intervals and intervals is not None:
-            intervals = intervals.copy()
+        if copy_intervals:
+            intervals = cp.copy(intervals)
         
         # Initialize Index
         if isinstance(intervals, IntervalArray) or isinstance(intervals, LabeledIntervalArray):
             self.index = intervals
-        elif intervals is None and df is None:
-            self.index = None
-        elif intervals is None and df.shape == (0,0):
-            self.index = None
         else:
             raise TypeError("Unrecognized input for intervals.")
 
-        # Initialize DataFrame
-        if df is None:
+        # Initialize Series
+        if series is None:
             # Intervals given
             if intervals is None:
-                # Columns given
-                if columns is None:
-                    df = pd.DataFrame([], index=range(0))
+                if dtype is None:
+                    series = pd.Series([], index=range(0))
                 else:
-                    if dtypes is None:
-                        df = pd.DataFrame([], index=range(0), columns=columns)
-                    else:
-                        df = pd.DataFrame([], index=range(0), columns=columns).astype(dtypes, copy=False)
+                    series = pd.Series([], index=range(0)).astype(dtype, copy=False)
             else:
-                # Columns given
-                if columns is None:
-                    df = pd.DataFrame([], index=range(len(self.index)))
+                if dtype is None:
+                    series = pd.DataFrame([], index=range(len(self.index)))
                 else:
-                    if dtypes is None:
-                        df = pd.DataFrame([], index=range(len(self.index)), columns=columns)
-                    else:
-                        df = pd.DataFrame([], index=range(len(self.index)), columns=columns).astype(dtypes, copy=False)
-        
-        elif isinstance(df, pd.DataFrame):
-            if copy_df:
-                df = df.copy(deep=True)
-                
-        # Set df
-        self.df = df
+                    series = pd.DataFrame([], index=range(len(self.index))).astype(dtype, copy=False)
         
-        # Check shape
-        if self.index is None:
-            if self.df.shape[0] != 0:
-                raise TypeError("DataFrame and Intervals don't match.")
-        elif self.index.size != self.df.shape[0]:
-            raise TypeError("DataFrame and Intervals don't match.")
+        elif isinstance(series, pd.Series):
+            if copy_series:
+                series = series.copy(deep=True)
+                
+        # Set series
+        self.series = series
 
         # Make sure index is frozen
-        if self.index is not None:
-            self.index.freeze()
+        self.index.freeze()
 
 
     def __repr__(self):
         """
         IntervalFrame representation
         """
 
         # Initialized string
         repr_string = ""
 
-        # If nothing
-        if self.index is None:
-            repr_string += "None\n"
-
         # If no columns present
-        elif self.df.shape[1] == 0:
+        if self.series.shape[0] == 0:
             repr_string += repr(self.index)
-            repr_string += repr(self.df)
+            repr_string += repr(self.series)
 
         # If columns present
         else:
             # Determine dimensions
-            n_rows = min(self.df.shape[0], 5)
-            n_cols = min(self.df.shape[1], 5)
+            n_rows = min(self.series.shape[0], 5)
             
             # Initialize values
             repr_list = [[] for i in range(n_rows+1)]
             
             # Determine column names
             repr_list[0] = ["interval"]
-            repr_list[0] += list(map(str, list(self.df.columns.values[:n_cols])))
+            repr_list[0] += [str(self.series.name)]
             
             i = 0 # track rows
             for interval in self.index:
                 if i >= n_rows:
                     break
                 #repr_list[i+1].append(repr(interval).split(",")[0] + ")")
                 repr_list[i+1].append(repr(interval))
-                repr_list[i+1] += list(map(str, list(self.df.iloc[i,:n_cols].values)))
+                repr_list[i+1] += [str(self.series.values[i])]
                 i += 1
             
             # Create tabulate table
             repr_string = tabulate(repr_list, headers="firstrow")
 
         return repr_string
 
     
     @property
     def shape(self):
         """
         """
         
-        return self.df.shape
+        return self.series.shape
 
 
     @property
     def iloc(self):
         """
         """
 
-        # If index is None
-        if self.index is None:
-            return None
-
-        return iLocator(self)
+        return indexers.iLocator(self)
 
     
     @property
     def loc(self):
         """
         """
 
-        # If index is None
-        if self.index is None:
-            return None
-
-        return Locator(self)
+        return indexers.Locator(self)
         
     
     @property
     def values(self):
         """
         """
-
-        return self.df.values
-
-    
-    @property
-    def columns(self):
-        """
-        """
-
-        return self.df.columns
+        
+        return self.series.values
 
     
     @staticmethod
     def from_array(starts, ends, labels=None):
         """
         """
 
@@ -202,120 +159,74 @@
         if labels is None:
             index = IntervalArray()
             index.from_array(starts, ends)
         else:
             index = LabeledIntervalArray()
             index.from_array(starts, ends, labels)
             
-        # Create IntervalFrame
-        iframe = IntervalFrame(index)
+        # Create IntervalSeries
+        iseries = IntervalSeries(index)
         
-        return iframe
+        return iseries
                 
                 
     def starts(self):
         """
         """
-
-        # If index is None
-        if self.index is None:
-            return None
         
         # Extract starts in intervals
         starts = self.index.extract_starts()
         
         return starts
         
     
     def ends(self):
         """
         """
-
-        # If index is None
-        if self.index is None:
-            return None
         
         # Extract ends in intervals
         ends = self.index.extract_ends()
         
         return ends
 
 
-    def concat(self, iframe_iter):
-        """
-        Append IntervalFrame to current IntervalFrame
-
-        Parameters
-        ----------
-            ilist : IntervalFrame
-
-        Returns
-        -------
-            None
-
-        """
-
-        # Iterate over iframes
-        concat_iframe = self.copy()
-        if concat_iframe.index is not None:
-            concat_iframe.index.unfreeze()
-        for iframe in iframe_iter:
-            concat_iframe.df = pd.concat([concat_iframe.df, iframe.df], ignore_index=True, join="outer")
-            if concat_iframe.index is None:
-                concat_iframe.index = iframe.index.copy()
-            else:
-                concat_iframe.index.append(iframe.index)
-        concat_iframe.index.construct()
-        concat_iframe.index.freeze()
-
-        # Reset index
-        concat_iframe.df.index = range(concat_iframe.df.shape[0])
-
-        return concat_iframe
-
-
     def intersect(self, start, end, label=None):
         """
         Find intersecting intervals
 
         Paramters
         ---------
             start : int
                 Starting position
             end : int
                 Ending position
-            label : str or list
-                Labels to intersect with [default: None]
+            label : str
+                Label to intersect with [default: None]
 
         Returns
         -------
             overlaps : IntervalFrame
                 Overlapping intervals
             
         """
 
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
         # Intersect
         if label is None:
-            overlaps, overlap_index = self.index.intersect_with_index(start, end)
+            overlaps, overlap_index = self.index.intersect(start, end, return_intervals=True, return_index=True)
         else:
-            overlaps, overlap_index = self.index.intersect_with_index(start, end, label=str(label))
+            overlaps, overlap_index = self.index.intersect(start, end, label=str(label), return_intervals=True, return_index=True)
             
         # Create df
-        if self.df.shape[1] > 0:
-            df = pd.DataFrame(self.df.values[overlap_index,:],
-                            columns=self.df.columns.values).astype(self.df.dtypes.to_dict(), copy=False)
+        if len(self.series) > 0:
+            series = pd.Series(self.series.values[overlap_index])
         else:
-            df = pd.DataFrame([], index=range(len(overlaps)))
+            series = pd.Series([], index=range(len(overlaps)))
 
         # Create IntervalFrame
-        overlaps = IntervalFrame(overlaps, df, copy_intervals=False, copy_df=False)
+        overlaps = IntervalSeries(overlaps, series, copy_intervals=False, copy_series=False)
 
         return overlaps
 
 
     def subtract(self, iframe):
         """
         Subtract intersecting regions for IntervalFrame
@@ -328,18 +239,14 @@
         Returns
         -------
             subtracted_frame : IntervalFrame
                 Intervals with removed regions
 
         """
 
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
         pass
 
 
     def difference(self, iframe):
         """
         Remove any overlapping intervals
 
@@ -350,22 +257,18 @@
 
         Returns
         -------
             diff_frame : IntervalFrame
                 Intervals that do not overlap
         """
 
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
         pass
 
 
-    def nhits(self, start, end, label=None):
+    def nhits(self, start, end):
         """
         Find number of intersecting intervals
 
         Paramters
         ---------
             start : int
                 Starting position
@@ -375,24 +278,15 @@
         Returns
         -------
             n : int
                 Number of overlapping intervals
             
         """
 
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
-        if label is None:
-            nhits = self.index.nhits(start, end)
-        else:
-            nhits = self.index.nhits(start, end, label)
-
-        return nhits
+        pass
 
 
     def nhits_from_array(self, starts, ends):
         """
         Find number of intersecting intervals
 
         Paramters
@@ -405,18 +299,14 @@
         Returns
         -------
             n : numpy.ndarray
                 Number of overlapping intervals
             
         """
 
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
         pass
 
 
     def coverage(self):
         """
         Find number of intervals overlapping every
         position in the IntervalFrame
@@ -427,18 +317,14 @@
 
         Returns
         -------
             pandas.Series{double}
                 Position on index and coverage as values
         """
 
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
         pass
 
 
     def bin_coverage(self, bin_size=100000, min_length=None, max_length=None):
         """
         Find sum of coverage within binned
         positions
@@ -455,18 +341,14 @@
         Returns
         -------
             cov_iframe : IntervalFrame
                 Positions of coverage values
 
         """
 
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
         # Determine nhits
         #ailist_cov = self.intervals.bin_coverage(bin_size=bin_size, min_length=min_length, max_length=max_length)
 
         # Create AIList from pd.Series index
         #positions = AIList()
         #positions.from_array(ailist_cov.index.values,
                             #ailist_cov.index.values + bin_size,
@@ -497,87 +379,23 @@
         Returns
         -------
             nhits_iframe : IntervalFrame
                 Position of nhits values
 
         """
 
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
         # Determine nhits
         nhits_bins, nhits_index = self.index.bin_nhits(bin_size, min_length, max_length)
 
         # Construct IntervalFrame
         nhits_df = pd.DataFrame(nhits_index, index=range(len(nhits_index)), columns=["nhits"])
-        nhits_iframe = IntervalFrame(nhits_bins, nhits_df, copy_intervals=False,
+        nhits_iframe = IntervalSeries(nhits_bins, nhits_df, copy_intervals=False,
                                      copy_df=False)
 
         return nhits_iframe
-    
-
-    def annotate(self, iframe, column, method="mean"):
-        """
-        Annotate values in one IntervalFrame with another
-
-        Parameters
-        ----------
-            iframe : IntervalFrame
-                Intervals used to annotate
-            columns : str
-                Name of the column to use
-            method : str
-                How to annotate ('mean','std','median','label')
-        
-        Returns
-        -------
-            None
-
-        """
-
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
-        # Find overlaps
-        if isinstance(iframe.index, LabeledIntervalArray) and isinstance(self.index, LabeledIntervalArray):
-            query_index, ref_index = self.index.intersect_from_LabeledIntervalArray(iframe.index)
-        elif isinstance(iframe.index, IntervalArray) and isinstance(self.index, IntervalArray):
-            query_index, ref_index = self.index.intersect_from_IntervalArray(iframe.index)
-        else:
-            raise TypeError("IntervalFrames must have same type of index.")
-
-        # Set function
-        if method == "mean":
-            func = np.mean
-        elif method == "median":
-            func = np.median
-        elif method == "std":
-            func = np.std
-        elif method == "var":
-            func = np.var
-
-        # Calculate value
-        if method != "label":
-            values = np.zeros(self.df.shape[0])
-            # Iterate over overlaps
-            for i in pd.unique(ref_index):
-                values[i] = func(iframe.df.loc[query_index[ref_index == i],
-                                               column].values)
-
-        elif method == "label":
-            values = np.repeat("", dtype="S10")
-            # Iterate over overlaps
-            for i in pd.unique(ref_index):
-                values[i] = Counter(iframe.df.loc[query_index[ref_index == i],
-                                                  column].values).most_common(1)[0][0]
-
-        # Append column to df
-        self.df[method] = values
 
 
     def overlap(self, iframe, key="overlap"):
         """
         Find overlaps in one IntervalFrame with another
 
         Parameters
@@ -590,32 +408,25 @@
         Returns
         -------
             results_iframe : IntervalFrame
                 Intervals with column indicating index of overlap
 
         """
 
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
         # Find overlaps
         if isinstance(iframe.index, LabeledIntervalArray) and isinstance(self.index, LabeledIntervalArray):
-            query_index, ref_index = self.index.intersect_from_LabeledIntervalArray(iframe.index)
+            query_index, ref_index = self.index.intersect_from_LabeledIntervalArray(iframe.index, return_intervals=False, return_index=True)
         elif isinstance(iframe.index, IntervalArray) and isinstance(self.index, IntervalArray):
-            query_index, ref_index = self.index.intersect_from_IntervalArray(iframe.index)
+            query_index, ref_index = self.index.intersect_from_IntervalArray(iframe.index, return_intervals=False, return_index=True)
         else:
             raise TypeError("IntervalFrames must have same type of index.")
 
         # Index iframes
-        if ref_index.shape[0] > 0: 
-            results_iframe = self.iloc[ref_index,:]
-            results_iframe.df["overlap"] = query_index
-        else:
-            results_iframe = IntervalFrame()
+        results_iframe = IntervalFrame.IntervalFrame(self.index[ref_index], copy_intervals=False)
+        results_iframe.df["overlap"] = query_index
 
         #Create intervals
         #results_intervals = self.index[ref_index]
 
         # Create df
         #if self.df.shape[1] > 0:
             #df = pd.DataFrame(self.df.values[ref_index,:],
@@ -643,117 +454,99 @@
         Returns
         -------
             merged_iframe : IntervalFrame
                 Merged intervals
 
         """
 
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
         # Merge intervals
         merged_index = self.index.merge(gap=gap)
         
         # Create IntervalFrame
-        merged_iframe = IntervalFrame(merged_index)
+        merged_iframe = IntervalSeries(merged_index, copy_intervals=False)
 
         return merged_iframe
 
     
-    def segment(self, column, method="bcp_online", cutoff=0.5, hazard=100, shuffles=5000, p=0.00005):
+    def segment(self, method="bcp_online", cutoff=0.5, hazard=100, shuffles=5000, p=0.00005):
         """
         Annotate values in one IntervalFrame with another
 
         Parameters
         ----------
-            iframe : IntervalFrame
-                Intervals used to annotate
-            column : str
-                Name of the column to use
+            method : str
+                Method for segmenting intervals
+            cutoff : float (default = 0.5)
+                Cutoff for bcp methods
+            hazard : int (default = 100)
+                Hazard values for bcp methods
+            shuffles : int (default = 5000)
+                Number of shuffles for cbs method
+            p : float (default = 0.00005)
+                Pvalue cutoff for cbs method
         
         Returns
         -------
-            segment_iframe : IntervalFrame
+            segment_iseries : IntervalSeries
                 Segmented Intervals
 
         """
 
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
         # Segment intervals for IntervalArray
-        if method == "bcp_online":
-            if isinstance(self.index, IntervalArray):
-                segment_intervals = bcpseg(self.df[column].values, cutoff=cutoff, method="online", hazard=hazard)
-            else:
-                segment_intervals = bcpseg(self.df[column].values, labels=self.index.extract_labels(), cutoff=cutoff, method="online", hazard=hazard)
-        elif method == "bcp_online_both":
-            if isinstance(self.index, IntervalArray):
-                segment_intervals = bcpseg(self.df[column].values, cutoff=cutoff, method="online_both", hazard=hazard)
-            else:
-                segment_intervals = bcpseg(self.df[column].values, labels=self.index.extract_labels(), cutoff=cutoff, method="online_both", hazard=hazard)
-        elif method == "bcp_offline":
-            if isinstance(self.index, IntervalArray):
-                segment_intervals = bcpseg(self.df[column].values, cutoff=cutoff, method="offline", hazard=hazard)
-            else:
-                segment_intervals = bcpseg(self.df[column].values, labels=self.index.extract_labels(), cutoff=cutoff, method="offline", hazard=hazard)
-        elif method == "cbs":
-            if isinstance(self.index, IntervalArray):
-                segment_intervals = cbseg.segment(self.df[column].values, shuffles=shuffles, p=p)
-            else:
-                segment_intervals = cbseg.segment(self.df[column].values, labels=self.index.extract_labels(), shuffles=shuffles, p=p)
-            segment_intervals = cbseg.validate(self.df[column].values, segment_intervals, shuffles=shuffles, p=p)
-        else:
-            raise NameError("method input not recognized.")
+        if isinstance(self.index, IntervalArray):
+            segment_intervals = linear_segment.segment(self.series.values,
+                                                        labels = None,
+                                                        cutoff = cutoff,
+                                                        method = method,
+                                                        hazard = hazard,
+                                                        shuffles = shuffles,
+                                                        p = p)
+        else:
+            segment_intervals = linear_segment.segment(self.series.values,
+                                                        labels = self.index.labels,
+                                                        cutoff = cutoff,
+                                                        method = method,
+                                                        hazard = hazard,
+                                                        shuffles = shuffles,
+                                                        p = p)
 
         #Re-index segments
-        #print(segment_intervals)
         segment_intervals.index_with_aiarray(self.index)
 
-        # Create IntervalFrame
-        segment_iframe = IntervalFrame(segment_intervals)
+        # Create IntervalSeries
+        segment_iseries = IntervalSeries(segment_intervals)
 
-        return segment_iframe
+        return segment_iseries
         
         
     def downsample(self, proportion):
         """
         Randomly downsample intervals
 
         Parameters
         ----------
             proportion : float
                 Proportion of intervals to keep
 
         Returns
         -------
-            filtered_iframe : IntervalFrame
+            filtered_iseries : IntervalSeries
                 Downsampled values
         """
-
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
         
         # Downsample
-        filtered_intervals, filtered_index = self.index.downsample_with_index(proportion)
+        filtered_intervals, filtered_index = self.index.downsample(proportion, return_intervals=True, return_index=True)
         
-        # Create df
-        if self.df.shape[1] > 0:
-            df = pd.DataFrame(self.df.values[filtered_index,:],
-                            columns=self.df.columns.values).astype(self.df.dtypes.to_dict(), copy=False)
-        else:
-            df = pd.DataFrame([], index=range(len(filtered_intervals)))
+        # Create series
+        series = pd.Series([], index=range(len(filtered_intervals)))
 
-        # Create IntervalFrame
-        filtered_iframe = IntervalFrame(filtered_intervals, df, copy_intervals=False, copy_df=False)
+        # Create IntervalSeries
+        filtered_iseries = IntervalSeries(filtered_intervals, series, copy_intervals=False, copy_series=False)
             
-        return filtered_iframe
+        return filtered_iseries
         
         
     def length_dist(self):
         """
         Calculate length distribution of intervals
         
         Parameters
@@ -761,18 +554,14 @@
             None
         
         Returns
         -------
             length_distribution : numpy.ndarray
                 Length distribution
         """
-
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
         
         # Calculate length distribution
         length_distribution = self.index.length_dist()
         
         return length_distribution
         
         
@@ -793,18 +582,14 @@
             
         Returns
         -------
             scores : dict of pandas.Series or pandas.Series
                 Position on index and WPS as values
         
         """
-
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
         
         # Calculate WPS without label
         scores = self.index.wps(protection, min_length, max_length)
             
         return scores
 
 
@@ -815,58 +600,46 @@
         Parameters
         ----------
             iframe : LabeledIntervalArray
                 Intervals to match
 
         Returns
         -------
-            matched_iframe : LabeledIntervalArray
+            filtered_iseries : IntervalSeries
                 Matched intervals
 
         """
 
-        # If index is None
-        if self.index is None:
-            raise AttributeError("LabeledIntervalArray is empty.")
-
         # Determine matches
         filtered_intervals, filtered_index = self.index.filter_exact_match(iframe.index)
 
-        # Create df
-        if self.df.shape[1] > 0:
-            df = pd.DataFrame(self.df.values[filtered_index,:],
-                            columns=self.df.columns.values).astype(self.df.dtypes.to_dict(), copy=False)
-        else:
-            df = pd.DataFrame([], index=range(len(filtered_intervals)))
+        # Create series
+        series = pd.Series([], index=range(len(filtered_intervals)))
 
-        # Create IntervalFrame
-        filtered_iframe = IntervalFrame(filtered_intervals, df, copy_intervals=False, copy_df=False)
+        # Create IntervalSeries
+        filtered_iseries = IntervalSeries(filtered_intervals, series, copy_intervals=False, copy_series=False)
 
-        return filtered_iframe
+        return filtered_iseries
         
     
     def copy(self):
         """
-        Copy IntervalFrame
+        Copy IntervalSeries
         
         Parameters
         ----------
             None
         
         Returns
         -------
-            copy_iframe : IntervalFrame
+            copy_iseries : IntervalSeries
                 Copied intervals
         
         """
-
-        # If index is None
-        #if self.index is None:
-            #raise AttributeError("LabeledIntervalArray is empty.")
         
-        # Make copy of IntervalFrame
-        copy_iframe = IntervalFrame(self.index, self.df,
+        # Make copy of IntervalSeries
+        copy_iseries = IntervalSeries(self.index, self.series,
                                     copy_intervals=True,
-                                    copy_df=True)
+                                    copy_series=True)
         
-        return copy_iframe
+        return copy_iseries
```

### Comparing `intervalframe-1.0.0/intervalframe/core/groupby.py` & `intervalframe-1.1.1/intervalframe/core/groupby.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.0.0/intervalframe/core/index/indexers.py` & `intervalframe-1.1.1/intervalframe/core/index/indexers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import numpy as np
 import pandas as pd
 from ailist import IntervalArray, LabeledIntervalArray
 from ailist import Interval, LabeledInterval
+from typing import List
+from pandas.api.types import is_integer
+
+# Local imports
 from .. import IntervalFrame
 from .. import IntervalSeries
 
 
 class iLocator(object):
     """
     Position indexer
 
     :class:`~intervalframe.iLocator` indexes intervals
     """
     
-    def __init__(self, iobject):
+    def __init__(self, 
+                 iobject):
         """
         Initialize iLocator
 
         Parameters
         ----------
             iframe : IntervalFrame or IntervalSeries
                 Intervals to index
@@ -43,39 +48,41 @@
 
         # Get index
         index = self.iobject.index[args[0]]
         
         # Create DataFrame or Series
         if isinstance(self.iobject, IntervalFrame.IntervalFrame):
             if self.iobject.df.shape[1] > 0:
-                if np.issubdtype(type(args[0]), np.integer):
+                if is_integer(args[0]):
                     data = self.iobject.df.iloc[[args[0]], args[1]]
-                elif np.issubdtype(type(args[1]), np.integer):
+                elif is_integer(args[1]):
                     data = self.iobject.df.iloc[args[0], args[1]]
                 else:
                     data = pd.DataFrame(self.iobject.df.values[args],
-                                    columns=self.iobject.df.columns.values).astype(self.iobject.df.dtypes.to_dict(), copy=False)
+                                        columns=self.iobject.df.columns.values).astype(self.iobject.df.dtypes.to_dict(),
+                                        copy=False)
             else:
                 data = pd.DataFrame([], index=range(len(index)))
         else:
             if self.iobject.series.shape[0] > 0:
                 data = pd.Series(self.iobject.series.values[args],
-                                    name=self.iobject.series.name).astype(self.iobject.series.dtype.to_dict(), copy=False)
+                                    name=self.iobject.series.name).astype(self.iobject.series.dtype.to_dict(),
+                                    copy=False)
             else:
                 data = pd.Series([], index=range(len(index)))
                           
         # Create IntervalFrame of IntervalSeries
         if isinstance(data, pd.Series):
             if isinstance(index, Interval) or isinstance(index, LabeledInterval):
-                iobject = IntervalSeries.IntervalSeries(index.to_list(), data, copy_series=False, copy_intervals=False)
+                iobject = IntervalSeries.IntervalSeries(index.to_array(), data, copy_series=False, copy_intervals=False)
             else:
                 iobject = IntervalSeries.IntervalSeries(index, data, copy_series=False, copy_intervals=False)
         else:
             if isinstance(index, Interval) or isinstance(index, LabeledInterval):
-                iobject = IntervalFrame.IntervalFrame(index.to_list(), data, copy_df=False, copy_intervals=False)
+                iobject = IntervalFrame.IntervalFrame(index.to_array(), data, copy_df=False, copy_intervals=False)
             else:
                 iobject = IntervalFrame.IntervalFrame(index, data, copy_df=False, copy_intervals=False)
         
         return iobject
     
 
     def __setitem__(self, index, value):
@@ -130,28 +137,28 @@
                 if isinstance(self.iobject, IntervalSeries.IntervalSeries):
                     intervals = self.iobject.index[args]
                 else:
                     intervals = self.iobject.index[args[0]]
                     index = np.arange(self.iobject.shape[0])[args[0]]
             else:
                 if isinstance(self.iobject, IntervalSeries.IntervalSeries):
-                    intervals, index = self.iobject.index.get_with_index(args)
+                    intervals, index = self.iobject.index.get(args, return_intervals=True, return_index=True)
                 else:
-                    intervals, index = self.iobject.index.get_with_index(args[0])
+                    intervals, index = self.iobject.index.get(args[0], return_intervals=True, return_index=True)
         else:
             raise IndexError("No labels in index.")
         
         # Create DataFrame or Series
         if isinstance(self.iobject, IntervalFrame.IntervalFrame):
             if isinstance(args, tuple) and isinstance(args[1], str):
                 if isinstance(args[0], slice):
                     data = self.iobject.df.iloc[args[0],:].loc[:,args[1]].copy()
                 else:
                     data = self.iobject.df.iloc[index,:].loc[:,args[1]].copy()
-            elif isinstance(args, tuple) and np.issubdtype(type(args[1]), np.integer):
+            elif isinstance(args, tuple) and is_integer(args[1]):
                 data = self.iobject.df.iloc[index,:].iloc[:,args[1]].copy()
             else:
                 data = self.iobject.df.iloc[index,:].loc[:,args[1]].copy()
         else:
             if isinstance(args, slice):
                 data = self.iobject.series.iloc[args].copy()
             else:
@@ -173,16 +180,16 @@
 
         # Check if index has keys
         if isinstance(self.iobject, IntervalFrame.IntervalFrame):
             if isinstance(index, tuple) and len(index) == 2:
                 if isinstance(index[0], slice):
                     self.iobject.df.loc[index] = value
                 elif isinstance(self.iobject.index, LabeledIntervalArray):
-                    indices = self.iobject.index.get_index(index[0])
+                    indices = self.iobject.index.get(index[0], return_intervals=False, return_index=True)
                     self.iobject.df.loc[:,index[1]].values[indices] = value
         
         else:
             if isinstance(index, slice):
                 self.iobject.series.loc[index] = value
             elif isinstance(self.iobject.index, LabeledIntervalArray):
-                indices = self.iobject.index.get_index(index)
+                indices = self.iobject.index.get(index, return_intervals=False, return_index=True)
                 self.iobject.series.loc[index].values[indices] = value
```

### Comparing `intervalframe-1.0.0/intervalframe/read/h5_utilities.py` & `intervalframe-1.1.1/intervalframe/read/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.0.0/intervalframe/utilities/h5_utilities.py` & `intervalframe-1.1.1/intervalframe/utilities/h5_utilities.py`

 * *Files identical despite different names*

### Comparing `intervalframe-1.0.0/intervalframe/write/h5_utilities.py` & `intervalframe-1.1.1/intervalframe/write/h5_utilities.py`

 * *Files identical despite different names*

