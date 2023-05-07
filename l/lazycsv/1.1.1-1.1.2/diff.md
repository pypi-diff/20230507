# Comparing `tmp/lazycsv-1.1.1.tar.gz` & `tmp/lazycsv-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazycsv-1.1.1.tar", last modified: Wed May  3 00:55:57 2023, max compression
+gzip compressed data, was "lazycsv-1.1.2.tar", last modified: Sun May  7 19:56:48 2023, max compression
```

## Comparing `lazycsv-1.1.1.tar` & `lazycsv-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-03 00:55:57.318527 lazycsv-1.1.1/
--rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.1.1/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     9415 2023-05-03 00:55:57.318527 lazycsv-1.1.1/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     8364 2023-05-02 14:38:28.000000 lazycsv-1.1.1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-03 00:55:57.318527 lazycsv-1.1.1/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     2400 2023-05-03 00:55:38.000000 lazycsv-1.1.1/setup.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-03 00:55:57.318527 lazycsv-1.1.1/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-03 00:55:57.318527 lazycsv-1.1.1/src/lazycsv/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.1.1/src/lazycsv/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    39385 2023-05-02 14:43:37.000000 lazycsv-1.1.1/src/lazycsv/lazycsv.c
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-03 00:55:57.318527 lazycsv-1.1.1/src/lazycsv.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     9415 2023-05-03 00:55:57.000000 lazycsv-1.1.1/src/lazycsv.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-05-03 00:55:57.000000 lazycsv-1.1.1/src/lazycsv.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-03 00:55:57.000000 lazycsv-1.1.1/src/lazycsv.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       66 2023-05-03 00:55:57.000000 lazycsv-1.1.1/src/lazycsv.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-03 00:55:57.000000 lazycsv-1.1.1/src/lazycsv.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-03 00:55:57.318527 lazycsv-1.1.1/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)    23737 2023-05-02 15:32:03.000000 lazycsv-1.1.1/tests/test_lazycsv.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-07 19:56:48.041865 lazycsv-1.1.2/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.1.2/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     9408 2023-05-07 19:56:48.041865 lazycsv-1.1.2/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     8357 2023-05-07 19:55:27.000000 lazycsv-1.1.2/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-07 19:56:48.041865 lazycsv-1.1.2/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     2400 2023-05-07 19:56:34.000000 lazycsv-1.1.2/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-07 19:56:48.041865 lazycsv-1.1.2/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-07 19:56:48.041865 lazycsv-1.1.2/src/lazycsv/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.1.2/src/lazycsv/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    39603 2023-05-07 19:55:27.000000 lazycsv-1.1.2/src/lazycsv/lazycsv.c
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-07 19:56:48.041865 lazycsv-1.1.2/src/lazycsv.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     9408 2023-05-07 19:56:48.000000 lazycsv-1.1.2/src/lazycsv.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-05-07 19:56:48.000000 lazycsv-1.1.2/src/lazycsv.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-07 19:56:48.000000 lazycsv-1.1.2/src/lazycsv.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       66 2023-05-07 19:56:48.000000 lazycsv-1.1.2/src/lazycsv.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-07 19:56:48.000000 lazycsv-1.1.2/src/lazycsv.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-07 19:56:48.041865 lazycsv-1.1.2/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)    23765 2023-05-03 15:13:07.000000 lazycsv-1.1.2/tests/test_lazycsv.py
```

### Comparing `lazycsv-1.1.1/LICENSE` & `lazycsv-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lazycsv-1.1.1/PKG-INFO` & `lazycsv-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.1.1
+Version: 1.1.2
 Summary: an fast, memory efficient csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -201,17 +201,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 0.134gb
 cols=10000
 rows=10000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 0.4746863649925217
-parsing cols... time to parse: 1.5940959230065346
-total time: 2.0687822879990563
+indexing lazy... time to index: 0.450414217018988
+parsing cols... time to parse: 1.5233540059998631
+total time: 1.9737682230188511
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 0.40828132900060154
 parsing cols... time to parse: 3.810204313998838
 total time: 4.21848564299944
 
@@ -225,17 +225,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 1.387gb
 cols=10000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 4.287910053972155
-parsing cols... time to parse: 20.004111379006645
-total time: 24.2920214329788
+indexing lazy... time to index: 4.298127760004718
+parsing cols... time to parse: 18.591125406033825
+total time: 22.889253166038543
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 2.4456441220027045
 parsing cols... time to parse: 37.424315700998704
 total time: 39.86995982300141
 
@@ -248,17 +248,17 @@
 ```
 filesize: 14.333gb
 cols=100000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 61.56681043098797
-parsing cols... time to parse: 553.8464674730203
-total time: 615.4132779040083
+indexing lazy... time to index: 55.42112316700002
+parsing cols... time to parse: 362.268973717
+total time: 417.690096884
 
 benchmarking datatable:
  58% |█████████████████████████████▍                    | Reading data Killed
 
 benchmarking polars (read):
 Killed
 ```
```

### Comparing `lazycsv-1.1.1/README.md` & `lazycsv-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -174,17 +174,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 0.134gb
 cols=10000
 rows=10000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 0.4746863649925217
-parsing cols... time to parse: 1.5940959230065346
-total time: 2.0687822879990563
+indexing lazy... time to index: 0.450414217018988
+parsing cols... time to parse: 1.5233540059998631
+total time: 1.9737682230188511
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 0.40828132900060154
 parsing cols... time to parse: 3.810204313998838
 total time: 4.21848564299944
 
@@ -198,17 +198,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 1.387gb
 cols=10000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 4.287910053972155
-parsing cols... time to parse: 20.004111379006645
-total time: 24.2920214329788
+indexing lazy... time to index: 4.298127760004718
+parsing cols... time to parse: 18.591125406033825
+total time: 22.889253166038543
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 2.4456441220027045
 parsing cols... time to parse: 37.424315700998704
 total time: 39.86995982300141
 
@@ -221,17 +221,17 @@
 ```
 filesize: 14.333gb
 cols=100000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 61.56681043098797
-parsing cols... time to parse: 553.8464674730203
-total time: 615.4132779040083
+indexing lazy... time to index: 55.42112316700002
+parsing cols... time to parse: 362.268973717
+total time: 417.690096884
 
 benchmarking datatable:
  58% |█████████████████████████████▍                    | Reading data Killed
 
 benchmarking polars (read):
 Killed
 ```
```

### Comparing `lazycsv-1.1.1/setup.py` & `lazycsv-1.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ]
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="lazycsv",
-    version="1.1.1",
+    version="1.1.2",
     author="Michael Green, Chris Perkins",
     author_email="dev@crunch.io",
     description="an fast, memory efficient csv parser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src"),
     extras_require={
```

### Comparing `lazycsv-1.1.1/src/lazycsv/lazycsv.c` & `lazycsv-1.1.2/src/lazycsv/lazycsv.c`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,16 @@
 typedef struct {
     PyObject* empty;
     PyObject** items;
 } LazyCSV_Cache;
 
 
 typedef struct {
-    size_t value;
     size_t col;
+    size_t value;
 } LazyCSV_AnchorPoint;
 
 
 typedef struct {
     size_t index;
     size_t count;
 } LazyCSV_RowIndex;
@@ -107,15 +107,15 @@
     char _newline;
     LazyCSV_Index* _index;
     LazyCSV_File* _data;
     LazyCSV_Cache* _cache;
 } LazyCSV;
 
 
-typedef struct lazycsv_iter {
+typedef struct {
     PyObject_HEAD
     PyObject* lazy;
     size_t row;
     size_t col;
     size_t position;
     size_t stop;
     size_t step;
@@ -172,56 +172,54 @@
 
     INDEX_DTYPE item = target;
 
     _BufferWrite(cfile, cbuf, &item, sizeof(INDEX_DTYPE));
 }
 
 
-static inline size_t _AnchorValue_FromValue(size_t value, char *amap,
+static inline size_t _AnchorValue_FromValue(size_t value,
+                                            LazyCSV_AnchorPoint *amap,
                                             LazyCSV_RowIndex *ridx) {
 
-    LazyCSV_AnchorPoint apnt, apntp1;
+    LazyCSV_AnchorPoint *apnt = amap + ridx->count - 1;
 
-    apnt = *(LazyCSV_AnchorPoint *)(amap + ((ridx->count - 1) *
-                                            sizeof(LazyCSV_AnchorPoint)));
-    if (value >= apnt.col) {
-        return apnt.value;
+    if (value >= apnt->col) {
+        // we hit this if there is only one anchor point, or we're iterating
+        // over the last anchor point.
+        return apnt->value;
     }
 
+    LazyCSV_AnchorPoint* apntp1;
     size_t L = 0, R = ridx->count-1;
 
-    size_t asize = sizeof(LazyCSV_AnchorPoint);
-
     while (L <= R) {
         size_t M = (L + R) / 2;
-        apnt = *(LazyCSV_AnchorPoint *)(amap + (asize * M));
-        apntp1 = *(LazyCSV_AnchorPoint *)(amap + (asize * (M + 1)));
-        if (value > apntp1.col) {
+        apnt = amap + M;
+        apntp1 = apnt + 1;
+        if (value > apntp1->col) {
             L = M + 1;
         }
-        else if (value < apnt.col) {
+        else if (value < apnt->col) {
             R = M - 1;
         }
-        else if (value == apntp1.col) {
-            return apntp1.value;
+        else if (value == apntp1->col) {
+            return apntp1->value;
         }
         else {
-            // apnt.col <= value && value < apntp1.col
-            return apnt.value;
+            return apnt->value;
         }
     }
     return SIZE_MAX;
 }
 
-
 static inline size_t _Value_FromIndex(size_t value, LazyCSV_RowIndex *ridx,
                                       char *cmap, char *amap) {
 
     size_t cval = *(INDEX_DTYPE*)(cmap+(value*sizeof(INDEX_DTYPE)));
-    size_t aval = _AnchorValue_FromValue(value, amap, ridx);
+    size_t aval = _AnchorValue_FromValue(value, (LazyCSV_AnchorPoint*)amap, ridx);
     return aval == SIZE_MAX ? aval : cval + aval;
 }
 
 
 static inline void LazyCSV_IterCol(LazyCSV_Iter *iter, size_t *offset,
                                    size_t *len) {
     LazyCSV *lazy = (LazyCSV *)iter->lazy;
@@ -252,14 +250,15 @@
         *offset = cs;
     }
 }
 
 
 static inline void LazyCSV_IterRow(LazyCSV_Iter *iter, size_t *offset,
                                    size_t *len) {
+
     LazyCSV *lazy = (LazyCSV *)iter->lazy;
 
     if (iter->position < iter->stop) {
         size_t position =
             iter->reversed ? lazy->cols - iter->position - 1 : iter->position;
 
         iter->position += iter->step;
@@ -270,26 +269,25 @@
 
         size_t row = iter->row + !lazy->_skip_headers;
 
         LazyCSV_RowIndex* ridx =
             (LazyCSV_RowIndex*)
             (newlines + row*sizeof(LazyCSV_RowIndex));
 
-        char* aidx = anchors+ridx->index;
-        char* cidx = commas+((lazy->cols+1)*row*sizeof(INDEX_DTYPE));
+        char *aidx = anchors + ridx->index;
+        char *cidx = commas + ((lazy->cols + 1) * row * sizeof(INDEX_DTYPE));
 
         size_t cs = _Value_FromIndex(position, ridx, cidx, aidx);
         size_t ce = _Value_FromIndex(position + 1, ridx, cidx, aidx);
 
         *len = ce - cs - 1;
         *offset = cs;
     }
 }
 
-
 static inline PyObject *PyBytes_FromOffsetAndLen(LazyCSV *lazy, size_t offset,
                                                  size_t len) {
 
     PyObject* result;
     char* addr;
 
     switch (len) {
@@ -327,23 +325,22 @@
 
 static PyObject* LazyCSV_IterNext(PyObject* self) {
     LazyCSV_Iter* iter = (LazyCSV_Iter*)self;
     LazyCSV *lazy = (LazyCSV *)iter->lazy;
 
     size_t offset = SIZE_MAX, len;
 
-    if (iter->col != SIZE_MAX) {
-        LazyCSV_IterCol(iter, &offset, &len);
-    }
-
-    else if (iter->row != SIZE_MAX) {
+    switch ((iter->row == SIZE_MAX) - (iter->col == SIZE_MAX)) {
+    case -1:
         LazyCSV_IterRow(iter, &offset, &len);
-    }
-
-    else {
+        break;
+    case +1:
+        LazyCSV_IterCol(iter, &offset, &len);
+        break;
+    default:
         PyErr_SetString(
             PyExc_RuntimeError,
             "could not determine axis for materialization"
         );
         return NULL;
     }
 
@@ -355,63 +352,67 @@
     return PyBytes_FromOffsetAndLen(lazy, offset, len);
 }
 
 
 static PyObject* LazyCSV_IterAsList(PyObject* self) {
     LazyCSV_Iter* iter = (LazyCSV_Iter*)self;
     LazyCSV* lazy = (LazyCSV*)iter->lazy;
-    void (*fn)(LazyCSV_Iter*, size_t*, size_t*);
 
     size_t size;
+    size_t iter_col = iter->col;
+    size_t iter_row = iter->row;
 
-    if (iter->col != SIZE_MAX) {
-        size = lazy->rows - iter->position;
-        fn = LazyCSV_IterCol;
-    }
-    else if (iter->row != SIZE_MAX) {
+    if (iter_col == SIZE_MAX) {
         size = lazy->cols - iter->position;
-        fn = LazyCSV_IterRow;
+    }
+    else if (iter_row == SIZE_MAX) {
+        size = lazy->rows - iter->position;
     }
     else {
         PyErr_SetString(
             PyExc_RuntimeError,
             "could not determine axis for materialization"
         );
         return NULL;
     }
 
     PyObject* result = PyList_New(size);
-    size_t offset, len;
+    size_t offset=SIZE_MAX, len=0;
 
     PyObject* item;
     for (size_t i = 0; i < size; i++) {
-        fn(iter, &offset, &len);
+        switch (iter_col) {
+        case SIZE_MAX:
+            LazyCSV_IterRow(iter, &offset, &len);
+            break;
+        default:
+            LazyCSV_IterCol(iter, &offset, &len);
+        }
         item = PyBytes_FromOffsetAndLen(lazy, offset, len);
         PyList_SET_ITEM(result, i, item);
     }
 
     return result;
 }
 
 
 #if INCLUDE_NUMPY
 static PyObject* LazyCSV_IterAsNumpy(PyObject* self) {
     LazyCSV_Iter* iter = (LazyCSV_Iter*)self;
     LazyCSV* lazy = (LazyCSV*)iter->lazy;
 
     size_t size;
-    void (*fn)(LazyCSV_Iter*, size_t*, size_t*);
+    size_t iter_col = iter->col;
+    size_t iter_row = iter->row;
 
-    if (iter->col != SIZE_MAX) {
+    if (iter_col != SIZE_MAX) {
         size = lazy->rows - iter->position;
-        fn = LazyCSV_IterCol;
     }
-    else if (iter->row != SIZE_MAX) {
+    else if (iter_row != SIZE_MAX) {
         size = lazy->cols - iter->position;
-        fn = LazyCSV_IterRow;
     }
     else {
         PyErr_SetString(
             PyExc_RuntimeError,
             "could not determine axis for materialization"
         );
         return NULL;
@@ -420,16 +421,23 @@
     size_t buffer_capacity = 65536; // 2**16
     LazyCSV_Buffer buffer = {.data = malloc(buffer_capacity),
                              .size = 0,
                              .capacity = buffer_capacity};
 
     size_t offset, len=0, max_len=0;
     char* addr;
+
     for (size_t i=0; i < size; i++) {
-        fn(iter, &offset, &len);
+        switch (iter_col) {
+        case SIZE_MAX:
+            LazyCSV_IterRow(iter, &offset, &len);
+            break;
+        default:
+            LazyCSV_IterCol(iter, &offset, &len);
+        }
         addr = lazy->_data->data + offset;
         _BufferCache(&buffer, &len, sizeof(size_t));
         _BufferCache(&buffer, addr, len);
         max_len = len > max_len ? len : max_len;
     }
 
     npy_intp const dimensions[1] = {size, };
```

### Comparing `lazycsv-1.1.1/src/lazycsv.egg-info/PKG-INFO` & `lazycsv-1.1.2/src/lazycsv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.1.1
+Version: 1.1.2
 Summary: an fast, memory efficient csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -201,17 +201,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 0.134gb
 cols=10000
 rows=10000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 0.4746863649925217
-parsing cols... time to parse: 1.5940959230065346
-total time: 2.0687822879990563
+indexing lazy... time to index: 0.450414217018988
+parsing cols... time to parse: 1.5233540059998631
+total time: 1.9737682230188511
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 0.40828132900060154
 parsing cols... time to parse: 3.810204313998838
 total time: 4.21848564299944
 
@@ -225,17 +225,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 1.387gb
 cols=10000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 4.287910053972155
-parsing cols... time to parse: 20.004111379006645
-total time: 24.2920214329788
+indexing lazy... time to index: 4.298127760004718
+parsing cols... time to parse: 18.591125406033825
+total time: 22.889253166038543
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 2.4456441220027045
 parsing cols... time to parse: 37.424315700998704
 total time: 39.86995982300141
 
@@ -248,17 +248,17 @@
 ```
 filesize: 14.333gb
 cols=100000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 61.56681043098797
-parsing cols... time to parse: 553.8464674730203
-total time: 615.4132779040083
+indexing lazy... time to index: 55.42112316700002
+parsing cols... time to parse: 362.268973717
+total time: 417.690096884
 
 benchmarking datatable:
  58% |█████████████████████████████▍                    | Reading data Killed
 
 benchmarking polars (read):
 Killed
 ```
```

### Comparing `lazycsv-1.1.1/tests/test_lazycsv.py` & `lazycsv-1.1.2/tests/test_lazycsv.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,15 +524,16 @@
         -179769313486000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
         """
         data = textwrap.dedent(data)
         data = data.encode()
         with prepped_file(data) as tempf:
             lazy = lazycsv.LazyCSV(tempf.name, skip_headers=True)
             actual = list(list(lazy.sequence(col=i)) for i in range(lazy.cols))
-        assert actual == [data.split()]
+        expected = [data.split()]
+        assert actual == expected
 
     def test_encoded_headers(self):
         data = '"Göteborg","Sverige",Umeå,Köln,東京,deltaΔdelta\nc1,c2,c3,c4,c5,c6\n'
         data = data.encode()
         with prepped_file(data) as tempf:
             lazy = lazycsv.LazyCSV(tempf.name)
             assert lazy.headers == (
```

