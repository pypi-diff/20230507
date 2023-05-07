# Comparing `tmp/compel-1.1.4.tar.gz` & `tmp/compel-1.1.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-boqrvlq6/compel-1.1.4.tar", last modified: Sun May  7 08:39:05 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-t3ns2776/compel-1.1.4.dev0.tar", last modified: Sun May  7 07:43:38 2023, max compression
```

## Comparing `compel-1.1.4.tar` & `compel-1.1.4.dev0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 08:39:05.000000 compel-1.1.4/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.4/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)     7201 2023-05-07 08:39:05.000000 compel-1.1.4/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)     6623 2023-05-07 08:37:30.000000 compel-1.1.4/README.md
--rw-r--r--   0 damian     (501) staff       (20)      761 2023-05-07 08:35:46.000000 compel-1.1.4/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-05-07 08:39:05.000000 compel-1.1.4/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 08:39:05.000000 compel-1.1.4/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 08:39:05.000000 compel-1.1.4/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.4/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    14678 2023-05-07 07:42:07.000000 compel-1.1.4/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.4/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.4/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)    25187 2023-05-07 07:42:07.000000 compel-1.1.4/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    29539 2023-05-07 08:38:07.000000 compel-1.1.4/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 08:39:05.000000 compel-1.1.4/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)     7201 2023-05-07 08:39:05.000000 compel-1.1.4/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      462 2023-05-07 08:39:05.000000 compel-1.1.4/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-05-07 08:39:05.000000 compel-1.1.4/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-05-07 08:39:05.000000 compel-1.1.4/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-05-07 08:39:05.000000 compel-1.1.4/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 08:39:05.000000 compel-1.1.4/test/
--rw-r--r--   0 damian     (501) staff       (20)    14454 2023-05-07 07:40:27.000000 compel-1.1.4/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    21072 2023-04-30 12:11:27.000000 compel-1.1.4/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47126 2023-05-07 07:40:27.000000 compel-1.1.4/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.4.dev0/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)     7101 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)     6518 2023-04-30 12:11:27.000000 compel-1.1.4.dev0/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      767 2023-05-07 07:43:20.000000 compel-1.1.4.dev0/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.4.dev0/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    14678 2023-05-07 07:42:07.000000 compel-1.1.4.dev0/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.4.dev0/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.4.dev0/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)    25187 2023-05-07 07:42:07.000000 compel-1.1.4.dev0/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    29533 2023-05-07 07:42:03.000000 compel-1.1.4.dev0/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)     7101 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      462 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/test/
+-rw-r--r--   0 damian     (501) staff       (20)    14454 2023-05-07 07:40:27.000000 compel-1.1.4.dev0/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    21072 2023-04-30 12:11:27.000000 compel-1.1.4.dev0/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47126 2023-05-07 07:40:27.000000 compel-1.1.4.dev0/test/test_prompt_parser.py
```

### Comparing `compel-1.1.4/LICENSE` & `compel-1.1.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-1.1.4/PKG-INFO` & `compel-1.1.4.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.4
+Version: 1.1.4.dev0
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -73,16 +73,14 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
-#### 1.1.4 - fixes for #23 (sequential offload) and InvokeAI issue #3442 (allow hyphens in LoRA names) 
-
 #### 1.1.3 - enable fetching the penultimate CLIP hidden layer (aka "clip skip")
 
 To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance. Note that there's no need to pass this flag for SD2.0/SD2.1 because diffusers already throws away the last hidden layer when loading the SD2.0+ text encoder.
 
 #### 1.1.2 - fix for #21 (crash when parsing long prompts with truncation enabled if there is weighted fragments beyond the truncation boundary)
 
 #### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
```

### Comparing `compel-1.1.4/README.md` & `compel-1.1.4.dev0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,14 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
-#### 1.1.4 - fixes for #23 (sequential offload) and InvokeAI issue #3442 (allow hyphens in LoRA names) 
-
 #### 1.1.3 - enable fetching the penultimate CLIP hidden layer (aka "clip skip")
 
 To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance. Note that there's no need to pass this flag for SD2.0/SD2.1 because diffusers already throws away the last hidden layer when loading the SD2.0+ text encoder.
 
 #### 1.1.2 - fix for #21 (crash when parsing long prompts with truncation enabled if there is weighted fragments beyond the truncation boundary)
 
 #### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
```

### Comparing `compel-1.1.4/pyproject.toml` & `compel-1.1.4.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "1.1.4"
+version = "1.1.4-dev.0"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-1.1.4/src/compel/compel.py` & `compel-1.1.4.dev0/src/compel/compel.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.4/src/compel/conditioning_scheduler.py` & `compel-1.1.4.dev0/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.4/src/compel/cross_attention_control.py` & `compel-1.1.4.dev0/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.4/src/compel/embeddings_provider.py` & `compel-1.1.4.dev0/src/compel/embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.4/src/compel/prompt_parser.py` & `compel-1.1.4.dev0/src/compel/prompt_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,15 +502,15 @@
     syntactic_chars = "".join(syntactic_symbols.keys())
 
     # accepts int or float notation, always maps to float
     number = pp.pyparsing_common.real | \
              pp.Combine(pp.Optional("-")+pp.Word(pp.nums)).set_parse_action(pp.token_map(float))
 
     # for options
-    keyword = pp.Word(pp.alphanums + '_' + '-')
+    keyword = pp.Word(pp.alphanums + '_')
 
     # a word that absolutely does not contain any meaningful syntax
     non_syntax_word = pp.Combine(pp.OneOrMore(pp.MatchFirst([
             pp.Or(syntactic_symbols.values()), # escaped syntactic symbols
             pp.one_of(['-', '+']) + pp.NotAny(pp.White() | pp.Char(syntactic_chars) | pp.StringEnd()),
             number,
             # build character-by-character
```

### Comparing `compel-1.1.4/src/compel.egg-info/PKG-INFO` & `compel-1.1.4.dev0/src/compel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.4
+Version: 1.1.4.dev0
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -73,16 +73,14 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
-#### 1.1.4 - fixes for #23 (sequential offload) and InvokeAI issue #3442 (allow hyphens in LoRA names) 
-
 #### 1.1.3 - enable fetching the penultimate CLIP hidden layer (aka "clip skip")
 
 To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance. Note that there's no need to pass this flag for SD2.0/SD2.1 because diffusers already throws away the last hidden layer when loading the SD2.0+ text encoder.
 
 #### 1.1.2 - fix for #21 (crash when parsing long prompts with truncation enabled if there is weighted fragments beyond the truncation boundary)
 
 #### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
```

### Comparing `compel-1.1.4/test/test_compel.py` & `compel-1.1.4.dev0/test/test_compel.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.4/test/test_embeddings_provider.py` & `compel-1.1.4.dev0/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.4/test/test_prompt_parser.py` & `compel-1.1.4.dev0/test/test_prompt_parser.py`

 * *Files identical despite different names*

