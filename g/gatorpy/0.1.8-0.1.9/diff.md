# Comparing `tmp/gatorpy-0.1.8.tar.gz` & `tmp/gatorpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gatorpy-0.1.8.tar", max compression
+gzip compressed data, was "gatorpy-0.1.9.tar", max compression
```

## Comparing `gatorpy-0.1.8.tar` & `gatorpy-0.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      100 2023-02-01 23:09:07.112868 gatorpy-0.1.8/README.md
--rw-r--r--   0        0        0     8196 2023-03-12 03:21:55.876314 gatorpy-0.1.8/gatorpy/.DS_Store
--rw-r--r--   0        0        0    32012 2023-03-20 20:58:58.000000 gatorpy-0.1.8/gatorpy/UNet.py
--rw-r--r--   0        0        0      615 2023-03-17 20:22:57.000000 gatorpy-0.1.8/gatorpy/__init__.py
--rw-r--r--   0        0        0     6605 2023-03-17 15:00:03.000000 gatorpy-0.1.8/gatorpy/addPredictions.py
--rw-r--r--   0        0        0     6148 2023-02-04 00:38:46.817125 gatorpy-0.1.8/gatorpy/archives/.DS_Store
--rw-r--r--   0        0        0    30831 2023-02-04 00:24:05.686788 gatorpy-0.1.8/gatorpy/archives/UNet-02032023.py
--rw-r--r--   0        0        0    35278 2023-01-27 16:37:48.000000 gatorpy-0.1.8/gatorpy/archives/gator-01272023.py
--rw-r--r--   0        0        0      727 2023-02-03 20:50:23.880002 gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/GPUselect.py
--rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.479669 gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/PartitionOfImage.py
--rw-r--r--   0        0        0     6075 2023-02-03 20:50:23.880361 gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/PartitionOfImageOM.py
--rw-r--r--   0        0        0      804 2023-02-04 00:05:31.133302 gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc
--rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.131943 gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc
--rw-r--r--   0        0        0     2062 2023-02-04 00:05:31.128022 gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc
--rw-r--r--   0        0        0     9960 2023-02-04 00:25:40.288519 gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc
--rw-r--r--   0        0        0     1408 2023-02-03 20:50:23.880559 gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/ftools.py
--rw-r--r--   0        0        0    10892 2023-02-04 00:25:24.874165 gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/imtools.py
--rw-r--r--   0        0        0     7197 2023-02-03 20:50:23.880964 gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/toolbox.py
--rw-r--r--   0        0        0     9954 2023-03-11 17:51:53.910170 gatorpy-0.1.8/gatorpy/cloneFolder.py
--rw-r--r--   0        0        0    42032 2023-03-11 23:38:47.059383 gatorpy-0.1.8/gatorpy/gator.py
--rw-r--r--   0        0        0     5811 2023-03-12 03:28:54.420440 gatorpy-0.1.8/gatorpy/gatorExport.py
--rw-r--r--   0        0        0    12784 2023-03-11 23:19:19.454850 gatorpy-0.1.8/gatorpy/gatorObject.py
--rw-r--r--   0        0        0    21484 2023-03-11 23:52:20.607558 gatorpy-0.1.8/gatorpy/gatorPhenotype.py
--rw-r--r--   0        0        0    17977 2023-03-12 00:38:53.986809 gatorpy-0.1.8/gatorpy/gatorPipeline.py
--rw-r--r--   0        0        0    12423 2023-03-20 20:58:58.000000 gatorpy-0.1.8/gatorpy/gatorPredict.py
--rw-r--r--   0        0        0    11541 2023-03-11 18:58:50.817277 gatorpy-0.1.8/gatorpy/gatorTrain.py
--rw-r--r--   0        0        0     7725 2023-03-11 23:19:32.493782 gatorpy-0.1.8/gatorpy/generateGatorScore.py
--rw-r--r--   0        0        0    27308 2023-03-09 16:31:07.688882 gatorpy-0.1.8/gatorpy/generateThumbnails.py
--rw-r--r--   0        0        0    13397 2023-03-09 16:49:19.450450 gatorpy-0.1.8/gatorpy/generateTrainTestSplit.py
--rw-r--r--   0        0        0     8831 2023-03-11 23:43:16.763123 gatorpy-0.1.8/gatorpy/mergeGatorObject.py
--rw-r--r--   0        0        0     9697 2023-03-17 20:29:25.000000 gatorpy-0.1.8/gatorpy/scatterPlot.py
--rw-r--r--   0        0        0     6148 2023-03-10 03:05:34.659991 gatorpy-0.1.8/gatorpy/toolbox/.DS_Store
--rw-r--r--   0        0        0      727 2023-02-03 20:50:23.880002 gatorpy-0.1.8/gatorpy/toolbox/GPUselect.py
--rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.479669 gatorpy-0.1.8/gatorpy/toolbox/PartitionOfImage.py
--rw-r--r--   0        0        0      196 2023-03-10 02:36:16.066065 gatorpy-0.1.8/gatorpy/toolbox/__init__.py
--rw-r--r--   0        0        0      804 2023-02-04 00:05:31.133302 gatorpy-0.1.8/gatorpy/toolbox/__pycache__/GPUselect.cpython-39.pyc
--rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.131943 gatorpy-0.1.8/gatorpy/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc
--rw-r--r--   0        0        0      477 2023-03-10 02:39:18.535940 gatorpy-0.1.8/gatorpy/toolbox/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      711 2023-02-04 00:52:32.027418 gatorpy-0.1.8/gatorpy/toolbox/__pycache__/ftools.cpython-39.pyc
--rw-r--r--   0        0        0     1017 2023-02-04 00:52:32.025450 gatorpy-0.1.8/gatorpy/toolbox/__pycache__/imtools.cpython-39.pyc
--rw-r--r--   0        0        0      361 2023-02-04 00:50:12.561879 gatorpy-0.1.8/gatorpy/toolbox/ftools.py
--rw-r--r--   0        0        0      671 2023-02-04 00:46:01.433171 gatorpy-0.1.8/gatorpy/toolbox/imtools.py
--rw-r--r--   0        0        0     1120 2023-03-20 21:55:57.000000 gatorpy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1234 1970-01-01 00:00:00.000000 gatorpy-0.1.8/setup.py
--rw-r--r--   0        0        0     1538 1970-01-01 00:00:00.000000 gatorpy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-02-01 23:09:07.112868 gatorpy-0.1.9/README.md
+-rw-r--r--   0        0        0     8196 2023-03-12 03:21:55.876314 gatorpy-0.1.9/gatorpy/.DS_Store
+-rw-r--r--   0        0        0    32012 2023-03-20 20:58:58.000000 gatorpy-0.1.9/gatorpy/UNet.py
+-rw-r--r--   0        0        0      615 2023-03-17 20:22:57.000000 gatorpy-0.1.9/gatorpy/__init__.py
+-rw-r--r--   0        0        0     6605 2023-03-17 15:00:03.000000 gatorpy-0.1.9/gatorpy/addPredictions.py
+-rw-r--r--   0        0        0     6148 2023-02-04 00:38:46.817125 gatorpy-0.1.9/gatorpy/archives/.DS_Store
+-rw-r--r--   0        0        0    30831 2023-02-04 00:24:05.686788 gatorpy-0.1.9/gatorpy/archives/UNet-02032023.py
+-rw-r--r--   0        0        0    35278 2023-01-27 16:37:48.000000 gatorpy-0.1.9/gatorpy/archives/gator-01272023.py
+-rw-r--r--   0        0        0      727 2023-02-03 20:50:23.880002 gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/GPUselect.py
+-rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.479669 gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/PartitionOfImage.py
+-rw-r--r--   0        0        0     6075 2023-02-03 20:50:23.880361 gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/PartitionOfImageOM.py
+-rw-r--r--   0        0        0      804 2023-02-04 00:05:31.133302 gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc
+-rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.131943 gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc
+-rw-r--r--   0        0        0     2062 2023-02-04 00:05:31.128022 gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc
+-rw-r--r--   0        0        0     9960 2023-02-04 00:25:40.288519 gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc
+-rw-r--r--   0        0        0     1408 2023-02-03 20:50:23.880559 gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/ftools.py
+-rw-r--r--   0        0        0    10892 2023-02-04 00:25:24.874165 gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/imtools.py
+-rw-r--r--   0        0        0     7197 2023-02-03 20:50:23.880964 gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/toolbox.py
+-rw-r--r--   0        0        0     9954 2023-03-11 17:51:53.910170 gatorpy-0.1.9/gatorpy/cloneFolder.py
+-rw-r--r--   0        0        0    42032 2023-03-11 23:38:47.059383 gatorpy-0.1.9/gatorpy/gator.py
+-rw-r--r--   0        0        0     5811 2023-03-12 03:28:54.420440 gatorpy-0.1.9/gatorpy/gatorExport.py
+-rw-r--r--   0        0        0    12784 2023-03-11 23:19:19.454850 gatorpy-0.1.9/gatorpy/gatorObject.py
+-rw-r--r--   0        0        0    21484 2023-03-11 23:52:20.607558 gatorpy-0.1.9/gatorpy/gatorPhenotype.py
+-rw-r--r--   0        0        0    17977 2023-03-12 00:38:53.986809 gatorpy-0.1.9/gatorpy/gatorPipeline.py
+-rw-r--r--   0        0        0    12840 2023-03-21 14:56:48.283143 gatorpy-0.1.9/gatorpy/gatorPredict.py
+-rw-r--r--   0        0        0    11541 2023-03-11 18:58:50.817277 gatorpy-0.1.9/gatorpy/gatorTrain.py
+-rw-r--r--   0        0        0     7725 2023-03-11 23:19:32.493782 gatorpy-0.1.9/gatorpy/generateGatorScore.py
+-rw-r--r--   0        0        0    27308 2023-03-09 16:31:07.688882 gatorpy-0.1.9/gatorpy/generateThumbnails.py
+-rw-r--r--   0        0        0    13397 2023-03-09 16:49:19.450450 gatorpy-0.1.9/gatorpy/generateTrainTestSplit.py
+-rw-r--r--   0        0        0     8831 2023-03-11 23:43:16.763123 gatorpy-0.1.9/gatorpy/mergeGatorObject.py
+-rw-r--r--   0        0        0     9697 2023-03-17 20:29:25.000000 gatorpy-0.1.9/gatorpy/scatterPlot.py
+-rw-r--r--   0        0        0     6148 2023-03-10 03:05:34.659991 gatorpy-0.1.9/gatorpy/toolbox/.DS_Store
+-rw-r--r--   0        0        0      727 2023-02-03 20:50:23.880002 gatorpy-0.1.9/gatorpy/toolbox/GPUselect.py
+-rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.479669 gatorpy-0.1.9/gatorpy/toolbox/PartitionOfImage.py
+-rw-r--r--   0        0        0      196 2023-03-10 02:36:16.066065 gatorpy-0.1.9/gatorpy/toolbox/__init__.py
+-rw-r--r--   0        0        0      804 2023-02-04 00:05:31.133302 gatorpy-0.1.9/gatorpy/toolbox/__pycache__/GPUselect.cpython-39.pyc
+-rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.131943 gatorpy-0.1.9/gatorpy/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc
+-rw-r--r--   0        0        0      477 2023-03-10 02:39:18.535940 gatorpy-0.1.9/gatorpy/toolbox/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      711 2023-02-04 00:52:32.027418 gatorpy-0.1.9/gatorpy/toolbox/__pycache__/ftools.cpython-39.pyc
+-rw-r--r--   0        0        0     1017 2023-02-04 00:52:32.025450 gatorpy-0.1.9/gatorpy/toolbox/__pycache__/imtools.cpython-39.pyc
+-rw-r--r--   0        0        0      361 2023-02-04 00:50:12.561879 gatorpy-0.1.9/gatorpy/toolbox/ftools.py
+-rw-r--r--   0        0        0      671 2023-02-04 00:46:01.433171 gatorpy-0.1.9/gatorpy/toolbox/imtools.py
+-rw-r--r--   0        0        0     1120 2023-03-21 17:38:34.000000 gatorpy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1234 1970-01-01 00:00:00.000000 gatorpy-0.1.9/setup.py
+-rw-r--r--   0        0        0     1538 1970-01-01 00:00:00.000000 gatorpy-0.1.9/PKG-INFO
```

### Comparing `gatorpy-0.1.8/gatorpy/.DS_Store` & `gatorpy-0.1.9/gatorpy/.DS_Store`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/UNet.py` & `gatorpy-0.1.9/gatorpy/UNet.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/__init__.py` & `gatorpy-0.1.9/gatorpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/addPredictions.py` & `gatorpy-0.1.9/gatorpy/addPredictions.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/.DS_Store` & `gatorpy-0.1.9/gatorpy/archives/.DS_Store`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/UNet-02032023.py` & `gatorpy-0.1.9/gatorpy/archives/UNet-02032023.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/gator-01272023.py` & `gatorpy-0.1.9/gatorpy/archives/gator-01272023.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/GPUselect.py` & `gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/GPUselect.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/PartitionOfImage.py` & `gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/PartitionOfImage.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/PartitionOfImageOM.py` & `gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/PartitionOfImageOM.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc` & `gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc` & `gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc` & `gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc` & `gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/ftools.py` & `gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/ftools.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/imtools.py` & `gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/imtools.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/archives/toolbox-02032023/toolbox.py` & `gatorpy-0.1.9/gatorpy/archives/toolbox-02032023/toolbox.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/cloneFolder.py` & `gatorpy-0.1.9/gatorpy/cloneFolder.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/gator.py` & `gatorpy-0.1.9/gatorpy/gator.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/gatorExport.py` & `gatorpy-0.1.9/gatorpy/gatorExport.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/gatorObject.py` & `gatorpy-0.1.9/gatorpy/gatorObject.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/gatorPhenotype.py` & `gatorpy-0.1.9/gatorpy/gatorPhenotype.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/gatorPipeline.py` & `gatorpy-0.1.9/gatorpy/gatorPipeline.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/gatorPredict.py` & `gatorpy-0.1.9/gatorpy/gatorPredict.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,26 +117,35 @@
     
     fileName = pathlib.Path(imagePath).stem
 
     # read the markers.csv
     maper = pd.read_csv(pathlib.Path(markerChannelMapPath))
     columnnames =  [word.lower() for word in maper.columns]
     maper.columns = columnnames
-
+    
+    # making it compatable with mcmicro when no channel info is provided
+    if not set(['channel', 'channels', channelColumnName]).intersection(set(columnnames)):
+        # add a column called 'channel'
+        maper['channel'] = [i + 1 for i in range(len(maper))]
+        columnnames = list(maper.columns)
+        
+        
     # identify the marker column name (doing this to make it easier for people who confuse between marker and markers)
     if markerColumnName not in columnnames:
-           if markerColumnName != 'marker':
-               raise ValueError('markerColumnName not found in markerChannelMap, please check')
-           if 'markers' in columnnames:
-               markerCol = 'markers'
-           else:
-               raise ValueError('markerColumnName not found in markerChannelMap, please check')
+        # ckeck if 'markers' or 'marker_name' or 'marker_names' is in columnnames
+        # if so assign that match to markerCol
+        for colname in columnnames:
+            if 'marker' in colname or 'markers' in colname or 'marker_name' in colname or 'marker_names' in colname:
+                markerCol = colname
+                break
+        else:
+            raise ValueError('markerColumnName not found in markerChannelMap, please check')
     else:
-           markerCol = markerColumnName
-   
+        markerCol = markerColumnName
+
 
    # identify the channel column name (doing this to make it easier for people who confuse between channel and channels)
     if channelColumnName not in columnnames:
         if channelColumnName != 'channel':
             raise ValueError('channelColumnName not found in markerChannelMap, please check')
         if 'channels' in columnnames:
             channelCol = 'channels'
@@ -147,26 +156,25 @@
 
 
     # identify the gator model column name (doing this to make it easier for people who confuse between gatormodel and gatormodels)
     if modelColumnName not in columnnames:
         if modelColumnName != 'gatormodel':
             raise ValueError('modelColumnName not found in markerChannelMap, please check')
         if 'gatormodels' in columnnames:
-            channelCol = 'gatormodels'
+            modelCol = 'gatormodels'
         else:
             raise ValueError('modelColumnName not found in markerChannelMap, please check')
     else:
         modelCol = modelColumnName
 
     # remove rowa that have nans in modelCol
     runMenu = maper.dropna(subset=[modelCol], inplace=False)[[channelCol,markerCol,modelCol]]
 
     # shortcuts
     numMarkers = len(runMenu)
-    len(runMenu.columns)
 
     I = skio.imread(imagePath, img_num=0, plugin='tifffile')
 
 
     probPath = pathlib.Path(projectDir + '/GATOR/gatorPredict/')
     modelPath = pathlib.Path(gatorModelPath)
 
@@ -174,22 +182,22 @@
         os.makedirs(probPath,exist_ok=True)
 
 
     def data(runMenu, 
              imagePath, 
              modelPath, 
              projectDir, 
-             dsFactor=1, 
-             GPU=0):
+             dsFactor=dsFactor, 
+             GPU=GPU):
         
         # Loop through the rows of the DataFrame
         for index, row in runMenu.iterrows():
-            channel = row[channelColumnName]
-            markerName = row[markerColumnName]
-            gatormodel = row[modelColumnName]
+            channel = row[channelCol]
+            markerName = row[markerCol]
+            gatormodel = row[modelCol]
             if verbose is True:
                 print('Running gator model ' + str(gatormodel) + ' on channel ' + str(channel) + ' corresponding to marker ' + str(markerName) )
 
 
             tf.reset_default_graph()
             UNet2D.singleImageInferenceSetup(pathlib.Path(modelPath / gatormodel), GPU, -1, -1)
 
@@ -223,16 +231,16 @@
                 'append': False,
             }
 
             PM = np.uint8(255 * UNet2D.singleImageInference(I, 'accumulate',1))
             PM = resize(PM, (rawVert, rawHorz))
             yield np.uint8(255 * PM)
 
-    with tifffile.TiffWriter(probPath / (fileName + '_gatorPredict.ome.tif'),bigtiff=True) as tiff:
-        tiff.write(data(runMenu, imagePath, modelPath, probPath, dsFactor=dsFactor, GPU=0), shape=(numMarkers,I.shape[0],I.shape[1]), dtype='uint8', metadata={'Channel': {'Name': runMenu.marker.tolist()}, 'axes': 'CYX'})
+    with tifffile.TiffWriter(probPath / (fileName + '_gatorPredict.ome.tif'), bigtiff=True) as tiff:
+        tiff.write(data(runMenu, imagePath, modelPath, probPath, dsFactor=dsFactor, GPU=GPU), shape=(numMarkers,I.shape[0],I.shape[1]), dtype='uint8', metadata={'Channel': {'Name': runMenu[markerCol].tolist()}, 'axes': 'CYX'})
         UNet2D.singleImageInferenceCleanup()
 
 
 # =============================================================================
 #     logPath = ''
 #     scriptPath = os.path.dirname(os.path.realpath(__file__))
 #
```

### Comparing `gatorpy-0.1.8/gatorpy/gatorTrain.py` & `gatorpy-0.1.9/gatorpy/gatorTrain.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/generateGatorScore.py` & `gatorpy-0.1.9/gatorpy/generateGatorScore.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/generateThumbnails.py` & `gatorpy-0.1.9/gatorpy/generateThumbnails.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/generateTrainTestSplit.py` & `gatorpy-0.1.9/gatorpy/generateTrainTestSplit.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/mergeGatorObject.py` & `gatorpy-0.1.9/gatorpy/mergeGatorObject.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/scatterPlot.py` & `gatorpy-0.1.9/gatorpy/scatterPlot.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/toolbox/.DS_Store` & `gatorpy-0.1.9/gatorpy/toolbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/toolbox/GPUselect.py` & `gatorpy-0.1.9/gatorpy/toolbox/GPUselect.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/toolbox/PartitionOfImage.py` & `gatorpy-0.1.9/gatorpy/toolbox/PartitionOfImage.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/toolbox/__pycache__/GPUselect.cpython-39.pyc` & `gatorpy-0.1.9/gatorpy/toolbox/__pycache__/GPUselect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc` & `gatorpy-0.1.9/gatorpy/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/toolbox/__pycache__/ftools.cpython-39.pyc` & `gatorpy-0.1.9/gatorpy/toolbox/__pycache__/ftools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/toolbox/__pycache__/imtools.cpython-39.pyc` & `gatorpy-0.1.9/gatorpy/toolbox/__pycache__/imtools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/gatorpy/toolbox/imtools.py` & `gatorpy-0.1.9/gatorpy/toolbox/imtools.py`

 * *Files identical despite different names*

### Comparing `gatorpy-0.1.8/pyproject.toml` & `gatorpy-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gatorpy"
-version = "0.1.8"
+version = "0.1.9"
 description = "GATOR: A scalable framework for automated processing of highly multiplexed tissue images"
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 readme = "README.md"
 
 keywords = ["image analysis","multiplex imaging","single cell analysis"]
 
 homepage = "https://pypi.org/project/gatorpy/"
```

### Comparing `gatorpy-0.1.8/setup.py` & `gatorpy-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'scikit-learn>=1.2.1,<2.0.0',
  'tensorflow<2.11',
  'tifffile>=2022.8.12,<2023.0.0',
  'zarr>=2.12.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'gatorpy',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'GATOR: A scalable framework for automated processing of highly multiplexed tissue images',
     'long_description': '# gatorpy\n GATOR: A scalable framework for automated processing of highly multiplexed tissue images\n',
     'author': 'Ajit Johnson Nirmal',
     'author_email': 'ajitjohnson.n@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/gatorpy/',
```

### Comparing `gatorpy-0.1.8/PKG-INFO` & `gatorpy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gatorpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: GATOR: A scalable framework for automated processing of highly multiplexed tissue images
 Home-page: https://pypi.org/project/gatorpy/
 Keywords: image analysis,multiplex imaging,single cell analysis
 Author: Ajit Johnson Nirmal
 Author-email: ajitjohnson.n@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
```

