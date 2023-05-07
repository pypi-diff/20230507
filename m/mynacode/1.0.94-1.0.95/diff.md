# Comparing `tmp/mynacode-1.0.94-py3-none-any.whl.zip` & `tmp/mynacode-1.0.95-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8815 bytes, number of entries: 9
+Zip file size: 8834 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Sep-11 20:53 mlauto/__init__.py
 -rw-rw-rw-  2.0 fat    13388 b- defN 23-Feb-02 06:52 mlauto/mlauto.py
 -rw-rw-rw-  2.0 fat      111 b- defN 23-Feb-24 03:08 mynacode/__init__.py
 -rw-rw-rw-  2.0 fat     8317 b- defN 23-Mar-20 01:11 mynacode/mynacode - Copy.py
--rw-rw-rw-  2.0 fat     5975 b- defN 23-Apr-29 21:40 mynacode/mynacode.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-29 21:40 mynacode-1.0.94.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 21:40 mynacode-1.0.94.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-29 21:40 mynacode-1.0.94.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-29 21:40 mynacode-1.0.94.dist-info/RECORD
-9 files, 29035 bytes uncompressed, 7635 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat     6017 b- defN 23-May-07 20:34 mynacode/mynacode.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-May-07 20:35 mynacode-1.0.95.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 20:35 mynacode-1.0.95.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-07 20:35 mynacode-1.0.95.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      689 b- defN 23-May-07 20:35 mynacode-1.0.95.dist-info/RECORD
+9 files, 29077 bytes uncompressed, 7654 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mynacode/mynacode - Copy.py
 Comment: 
 
 Filename: mynacode/mynacode.py
 Comment: 
 
-Filename: mynacode-1.0.94.dist-info/METADATA
+Filename: mynacode-1.0.95.dist-info/METADATA
 Comment: 
 
-Filename: mynacode-1.0.94.dist-info/WHEEL
+Filename: mynacode-1.0.95.dist-info/WHEEL
 Comment: 
 
-Filename: mynacode-1.0.94.dist-info/top_level.txt
+Filename: mynacode-1.0.95.dist-info/top_level.txt
 Comment: 
 
-Filename: mynacode-1.0.94.dist-info/RECORD
+Filename: mynacode-1.0.95.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mynacode/mynacode.py

```diff
@@ -2,20 +2,20 @@
 import os, sys
 import json, requests, ast
 import pkg_resources
 import GPUtil, platform, psutil
 from datetime import datetime
 from sklearn import metrics
 
-#protocol = 'https'
-protocol = 'http'
+protocol = 'https'
+#protocol = 'http'
 
 
-IP = '127.0.0.1:8000'
-#IP = 'mynacode.com'
+#IP = '127.0.0.1:8000'
+IP = 'mynacode.com'
 #prev_func_list = ['a1zqw_9_', 'b1zqw_9_']
 prev_func_list = []
 prev_node = -999
 username = ""
 key = ""
   
 
@@ -132,15 +132,15 @@
     y_predicted = np.count_nonzero(y_pred == 0)
    
     return float(y_correct/y_predicted)
 
 def get_roc_auc(y_true, y_pred):
     fpr, tpr, threshold = metrics.roc_curve(y_true, y_pred)
     roc_auc = metrics.auc(fpr, tpr)
-    gmeans = np.sqrt(tpr * (1 - fpr))
+    gmeans = np.sqrt(tpr * (1 - fpr)) #sensitivity * specificity (element-wise)
     index = np.argmax(gmeans) #Returns index of max value
     best_threshold = threshold[index]
    
     return fpr, tpr, roc_auc, gmeans, best_threshold, index
 
 def get_metrics(y_true, y_pred, threshold):
     y_pred_binary = (y_pred > threshold).astype('float')
```

## Comparing `mynacode-1.0.94.dist-info/RECORD` & `mynacode-1.0.95.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlauto/__init__.py,sha256=oF_0vCehmivw-qD8z2tkyGk12n7CIJK2WPKqtcGtK_Y,102
 mlauto/mlauto.py,sha256=Qx7vf9SoDjsM_xBhSwg6TSf8F3xjS63wxMYvsxlCFb0,13388
 mynacode/__init__.py,sha256=qzUS3oZUS9IMp1DFKSYsXkwCY9whoh9pSUicECIkFks,111
 mynacode/mynacode - Copy.py,sha256=6wRDTZ27gkfKlqucw2bTfbaHdQBEEsqsVacPd3Qnn2o,8317
-mynacode/mynacode.py,sha256=8eNjW-FAuxRsH_OTzFrSKQoad9qSQjWwhHiZDJ0Yl10,5975
-mynacode-1.0.94.dist-info/METADATA,sha256=M82_80qiKq6UqMsQLXWPNNF24dQ2nTul04FhRgeNCbc,352
-mynacode-1.0.94.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mynacode-1.0.94.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
-mynacode-1.0.94.dist-info/RECORD,,
+mynacode/mynacode.py,sha256=iXfMYBHQMyMpD8q7uXPL8XgraPMi-jsraSnE2iUML1A,6017
+mynacode-1.0.95.dist-info/METADATA,sha256=kogAAmO9Xc0PZ8-k2yfAodmzhJPqkhU5_iFPUd8dSbw,352
+mynacode-1.0.95.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mynacode-1.0.95.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
+mynacode-1.0.95.dist-info/RECORD,,
```

