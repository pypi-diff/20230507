# Comparing `tmp/mynacode-1.0.95-py3-none-any.whl.zip` & `tmp/mynacode-1.0.96-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8834 bytes, number of entries: 9
+Zip file size: 8887 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Sep-11 20:53 mlauto/__init__.py
 -rw-rw-rw-  2.0 fat    13388 b- defN 23-Feb-02 06:52 mlauto/mlauto.py
 -rw-rw-rw-  2.0 fat      111 b- defN 23-Feb-24 03:08 mynacode/__init__.py
 -rw-rw-rw-  2.0 fat     8317 b- defN 23-Mar-20 01:11 mynacode/mynacode - Copy.py
--rw-rw-rw-  2.0 fat     6017 b- defN 23-May-07 20:34 mynacode/mynacode.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-May-07 20:35 mynacode-1.0.95.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 20:35 mynacode-1.0.95.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-07 20:35 mynacode-1.0.95.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      689 b- defN 23-May-07 20:35 mynacode-1.0.95.dist-info/RECORD
-9 files, 29077 bytes uncompressed, 7654 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat     6308 b- defN 23-May-07 21:30 mynacode/mynacode.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-May-07 21:30 mynacode-1.0.96.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 21:30 mynacode-1.0.96.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-07 21:30 mynacode-1.0.96.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      689 b- defN 23-May-07 21:30 mynacode-1.0.96.dist-info/RECORD
+9 files, 29368 bytes uncompressed, 7707 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mynacode/mynacode - Copy.py
 Comment: 
 
 Filename: mynacode/mynacode.py
 Comment: 
 
-Filename: mynacode-1.0.95.dist-info/METADATA
+Filename: mynacode-1.0.96.dist-info/METADATA
 Comment: 
 
-Filename: mynacode-1.0.95.dist-info/WHEEL
+Filename: mynacode-1.0.96.dist-info/WHEEL
 Comment: 
 
-Filename: mynacode-1.0.95.dist-info/top_level.txt
+Filename: mynacode-1.0.96.dist-info/top_level.txt
 Comment: 
 
-Filename: mynacode-1.0.95.dist-info/RECORD
+Filename: mynacode-1.0.96.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mynacode/mynacode.py

```diff
@@ -79,20 +79,19 @@
 
 def datasets(train, test, val, run_id):
 
   train = np.array(train)
   test = np.array(test)
   val = np.array(val)
 
-  train_shape = train.shape
-  test_shape = test.shape
-  val_shape = val.shape
-
-
-  data = {'run_id': run_id, 'train_shape' : train_shape, 'test_shape': test_shape, 'val_shape': val_shape,
+  data = {'run_id': run_id, 'train_shape' : train.shape, 'test_shape': test.shape, 'val_shape': val.shape,
+          'train_mean': np.mean(train), 'test_mean': np.mean(test), 'val_mean': np.mean(val),
+          'train_median': np.median(train), 'test_mean': np.median(test), 'val_mean': np.median(val),
+          'train_min': np.min(train), 'test_min': np.min(test), 'val_min': np.min(val),
+          'train_max': np.max(train), 'test_max': np.max(test), 'val_max': np.max(val),
           'username': username, 'key': key}
   
   response = requests.post(protocol+'://'+IP+'/api/add_datasets', data=data)
   
   if response.text == '0':
     print("Authentication failed")
   else:
```

## Comparing `mynacode-1.0.95.dist-info/RECORD` & `mynacode-1.0.96.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlauto/__init__.py,sha256=oF_0vCehmivw-qD8z2tkyGk12n7CIJK2WPKqtcGtK_Y,102
 mlauto/mlauto.py,sha256=Qx7vf9SoDjsM_xBhSwg6TSf8F3xjS63wxMYvsxlCFb0,13388
 mynacode/__init__.py,sha256=qzUS3oZUS9IMp1DFKSYsXkwCY9whoh9pSUicECIkFks,111
 mynacode/mynacode - Copy.py,sha256=6wRDTZ27gkfKlqucw2bTfbaHdQBEEsqsVacPd3Qnn2o,8317
-mynacode/mynacode.py,sha256=iXfMYBHQMyMpD8q7uXPL8XgraPMi-jsraSnE2iUML1A,6017
-mynacode-1.0.95.dist-info/METADATA,sha256=kogAAmO9Xc0PZ8-k2yfAodmzhJPqkhU5_iFPUd8dSbw,352
-mynacode-1.0.95.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mynacode-1.0.95.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
-mynacode-1.0.95.dist-info/RECORD,,
+mynacode/mynacode.py,sha256=HRXkX2PrxAGVRgHCRoGZDi4ZxIgP21VX4NPyTxyscF4,6308
+mynacode-1.0.96.dist-info/METADATA,sha256=3X5b4otD73hUW4B2prwvqR9T0vcmiu3JhgUX0deYkN8,352
+mynacode-1.0.96.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mynacode-1.0.96.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
+mynacode-1.0.96.dist-info/RECORD,,
```

