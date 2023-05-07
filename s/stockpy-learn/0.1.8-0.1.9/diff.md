# Comparing `tmp/stockpy-learn-0.1.8.tar.gz` & `tmp/stockpy-learn-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockpy-learn-0.1.8.tar", last modified: Sat Mar 25 11:34:22 2023, max compression
+gzip compressed data, was "stockpy-learn-0.1.9.tar", last modified: Sat Mar 25 11:36:42 2023, max compression
```

## Comparing `stockpy-learn-0.1.8.tar` & `stockpy-learn-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:34:22.776512 stockpy-learn-0.1.8/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     1076 2023-02-15 15:14:44.000000 stockpy-learn-0.1.8/LICENSE
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     1092 2023-03-25 11:34:22.776512 stockpy-learn-0.1.8/PKG-INFO
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     6457 2023-03-25 11:30:57.000000 stockpy-learn-0.1.8/README.md
--rw-rw-r--   0 silvio    (1000) silvio    (1000)      140 2023-03-24 10:58:06.000000 stockpy-learn-0.1.8/pyproject.toml
--rw-rw-r--   0 silvio    (1000) silvio    (1000)       38 2023-03-25 11:34:22.776512 stockpy-learn-0.1.8/setup.cfg
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     1369 2023-03-25 09:59:09.000000 stockpy-learn-0.1.8/setup.py
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:34:22.772512 stockpy-learn-0.1.8/stockpy/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)       80 2023-03-24 12:12:27.000000 stockpy-learn-0.1.8/stockpy/__init__.py
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:34:22.772512 stockpy-learn-0.1.8/stockpy/neural_network/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)      122 2023-03-24 12:12:44.000000 stockpy-learn-0.1.8/stockpy/neural_network/__init__.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    24214 2023-03-25 11:26:50.000000 stockpy-learn-0.1.8/stockpy/neural_network/_bigru.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    21790 2023-03-25 11:26:55.000000 stockpy-learn-0.1.8/stockpy/neural_network/_bilstm.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    21831 2023-03-25 11:26:59.000000 stockpy-learn-0.1.8/stockpy/neural_network/_gru.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    21892 2023-03-25 11:26:53.000000 stockpy-learn-0.1.8/stockpy/neural_network/_lstm.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    21005 2023-03-25 11:26:57.000000 stockpy-learn-0.1.8/stockpy/neural_network/_mlp.py
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:34:22.772512 stockpy-learn-0.1.8/stockpy/probabilistic/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)       94 2023-03-24 12:13:22.000000 stockpy-learn-0.1.8/stockpy/probabilistic/__init__.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    24308 2023-03-25 11:02:45.000000 stockpy-learn-0.1.8/stockpy/probabilistic/_bnn.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    34370 2023-03-25 11:10:39.000000 stockpy-learn-0.1.8/stockpy/probabilistic/_dmm.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    31088 2023-03-25 11:12:34.000000 stockpy-learn-0.1.8/stockpy/probabilistic/_ghmm.py
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:34:22.772512 stockpy-learn-0.1.8/stockpy/utils/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)       67 2023-03-24 12:15:21.000000 stockpy-learn-0.1.8/stockpy/utils/__init__.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)    11547 2023-03-24 15:37:54.000000 stockpy-learn-0.1.8/stockpy/utils/_dataset.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     3090 2022-12-14 15:08:27.000000 stockpy-learn-0.1.8/stockpy/utils/_disk.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)      607 2022-09-30 12:25:40.000000 stockpy-learn-0.1.8/stockpy/utils/_logconf.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     6018 2023-01-05 12:00:39.000000 stockpy-learn-0.1.8/stockpy/utils/_utils.py
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:34:22.772512 stockpy-learn-0.1.8/stockpy/utils/prompt/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)        0 2022-12-29 19:04:34.000000 stockpy-learn-0.1.8/stockpy/utils/prompt/__init__.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     3664 2023-01-02 10:46:39.000000 stockpy-learn-0.1.8/stockpy/utils/prompt/data.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     3850 2023-01-05 16:33:37.000000 stockpy-learn-0.1.8/stockpy/utils/prompt/ghmm.py
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     3570 2023-01-02 11:36:50.000000 stockpy-learn-0.1.8/stockpy/utils/prompt/lstm.py
-drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:34:22.772512 stockpy-learn-0.1.8/stockpy_learn.egg-info/
--rw-rw-r--   0 silvio    (1000) silvio    (1000)     1092 2023-03-25 11:34:22.000000 stockpy-learn-0.1.8/stockpy_learn.egg-info/PKG-INFO
--rw-rw-r--   0 silvio    (1000) silvio    (1000)      811 2023-03-25 11:34:22.000000 stockpy-learn-0.1.8/stockpy_learn.egg-info/SOURCES.txt
--rw-rw-r--   0 silvio    (1000) silvio    (1000)        1 2023-03-25 11:34:22.000000 stockpy-learn-0.1.8/stockpy_learn.egg-info/dependency_links.txt
--rw-rw-r--   0 silvio    (1000) silvio    (1000)       43 2023-03-25 11:34:22.000000 stockpy-learn-0.1.8/stockpy_learn.egg-info/requires.txt
--rw-rw-r--   0 silvio    (1000) silvio    (1000)        8 2023-03-25 11:34:22.000000 stockpy-learn-0.1.8/stockpy_learn.egg-info/top_level.txt
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.561681 stockpy-learn-0.1.9/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     1076 2023-02-15 15:14:44.000000 stockpy-learn-0.1.9/LICENSE
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     7083 2023-03-25 11:36:42.561681 stockpy-learn-0.1.9/PKG-INFO
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     6457 2023-03-25 11:30:57.000000 stockpy-learn-0.1.9/README.md
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)      140 2023-03-24 10:58:06.000000 stockpy-learn-0.1.9/pyproject.toml
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)       38 2023-03-25 11:36:42.561681 stockpy-learn-0.1.9/setup.cfg
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     7360 2023-03-25 11:36:37.000000 stockpy-learn-0.1.9/setup.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.557681 stockpy-learn-0.1.9/stockpy/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)       80 2023-03-24 12:12:27.000000 stockpy-learn-0.1.9/stockpy/__init__.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.557681 stockpy-learn-0.1.9/stockpy/neural_network/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)      122 2023-03-24 12:12:44.000000 stockpy-learn-0.1.9/stockpy/neural_network/__init__.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    24214 2023-03-25 11:26:50.000000 stockpy-learn-0.1.9/stockpy/neural_network/_bigru.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    21790 2023-03-25 11:26:55.000000 stockpy-learn-0.1.9/stockpy/neural_network/_bilstm.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    21831 2023-03-25 11:26:59.000000 stockpy-learn-0.1.9/stockpy/neural_network/_gru.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    21892 2023-03-25 11:26:53.000000 stockpy-learn-0.1.9/stockpy/neural_network/_lstm.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    21005 2023-03-25 11:26:57.000000 stockpy-learn-0.1.9/stockpy/neural_network/_mlp.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.557681 stockpy-learn-0.1.9/stockpy/probabilistic/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)       94 2023-03-24 12:13:22.000000 stockpy-learn-0.1.9/stockpy/probabilistic/__init__.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    24308 2023-03-25 11:02:45.000000 stockpy-learn-0.1.9/stockpy/probabilistic/_bnn.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    34370 2023-03-25 11:10:39.000000 stockpy-learn-0.1.9/stockpy/probabilistic/_dmm.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    31088 2023-03-25 11:12:34.000000 stockpy-learn-0.1.9/stockpy/probabilistic/_ghmm.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.557681 stockpy-learn-0.1.9/stockpy/utils/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)       67 2023-03-24 12:15:21.000000 stockpy-learn-0.1.9/stockpy/utils/__init__.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)    11547 2023-03-24 15:37:54.000000 stockpy-learn-0.1.9/stockpy/utils/_dataset.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     3090 2022-12-14 15:08:27.000000 stockpy-learn-0.1.9/stockpy/utils/_disk.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)      607 2022-09-30 12:25:40.000000 stockpy-learn-0.1.9/stockpy/utils/_logconf.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     6018 2023-01-05 12:00:39.000000 stockpy-learn-0.1.9/stockpy/utils/_utils.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.561681 stockpy-learn-0.1.9/stockpy/utils/prompt/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)        0 2022-12-29 19:04:34.000000 stockpy-learn-0.1.9/stockpy/utils/prompt/__init__.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     3664 2023-01-02 10:46:39.000000 stockpy-learn-0.1.9/stockpy/utils/prompt/data.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     3850 2023-01-05 16:33:37.000000 stockpy-learn-0.1.9/stockpy/utils/prompt/ghmm.py
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     3570 2023-01-02 11:36:50.000000 stockpy-learn-0.1.9/stockpy/utils/prompt/lstm.py
+drwxrwxr-x   0 silvio    (1000) silvio    (1000)        0 2023-03-25 11:36:42.561681 stockpy-learn-0.1.9/stockpy_learn.egg-info/
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)     7083 2023-03-25 11:36:42.000000 stockpy-learn-0.1.9/stockpy_learn.egg-info/PKG-INFO
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)      811 2023-03-25 11:36:42.000000 stockpy-learn-0.1.9/stockpy_learn.egg-info/SOURCES.txt
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)        1 2023-03-25 11:36:42.000000 stockpy-learn-0.1.9/stockpy_learn.egg-info/dependency_links.txt
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)       43 2023-03-25 11:36:42.000000 stockpy-learn-0.1.9/stockpy_learn.egg-info/requires.txt
+-rw-rw-r--   0 silvio    (1000) silvio    (1000)        8 2023-03-25 11:36:42.000000 stockpy-learn-0.1.9/stockpy_learn.egg-info/top_level.txt
```

### Comparing `stockpy-learn-0.1.8/LICENSE` & `stockpy-learn-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/README.md` & `stockpy-learn-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/neural_network/_bigru.py` & `stockpy-learn-0.1.9/stockpy/neural_network/_bigru.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/neural_network/_bilstm.py` & `stockpy-learn-0.1.9/stockpy/neural_network/_bilstm.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/neural_network/_gru.py` & `stockpy-learn-0.1.9/stockpy/neural_network/_gru.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/neural_network/_lstm.py` & `stockpy-learn-0.1.9/stockpy/neural_network/_lstm.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/neural_network/_mlp.py` & `stockpy-learn-0.1.9/stockpy/neural_network/_mlp.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/probabilistic/_bnn.py` & `stockpy-learn-0.1.9/stockpy/probabilistic/_bnn.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/probabilistic/_dmm.py` & `stockpy-learn-0.1.9/stockpy/probabilistic/_dmm.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/probabilistic/_ghmm.py` & `stockpy-learn-0.1.9/stockpy/probabilistic/_ghmm.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/utils/_dataset.py` & `stockpy-learn-0.1.9/stockpy/utils/_dataset.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/utils/_disk.py` & `stockpy-learn-0.1.9/stockpy/utils/_disk.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/utils/_logconf.py` & `stockpy-learn-0.1.9/stockpy/utils/_logconf.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/utils/_utils.py` & `stockpy-learn-0.1.9/stockpy/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/utils/prompt/data.py` & `stockpy-learn-0.1.9/stockpy/utils/prompt/data.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/utils/prompt/ghmm.py` & `stockpy-learn-0.1.9/stockpy/utils/prompt/ghmm.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy/utils/prompt/lstm.py` & `stockpy-learn-0.1.9/stockpy/utils/prompt/lstm.py`

 * *Files identical despite different names*

### Comparing `stockpy-learn-0.1.8/stockpy_learn.egg-info/SOURCES.txt` & `stockpy-learn-0.1.9/stockpy_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

