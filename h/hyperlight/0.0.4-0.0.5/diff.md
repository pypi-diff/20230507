# Comparing `tmp/hyperlight-0.0.4.tar.gz` & `tmp/hyperlight-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperlight-0.0.4.tar", max compression
+gzip compressed data, was "hyperlight-0.0.5.tar", max compression
```

## Comparing `hyperlight-0.0.4.tar` & `hyperlight-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    10173 2023-04-30 17:07:30.205256 hyperlight-0.0.4/LICENSE
--rw-r--r--   0        0        0    13145 2023-05-06 20:41:23.110335 hyperlight-0.0.4/README.md
--rw-r--r--   0        0        0      180 2023-05-06 20:42:46.131398 hyperlight-0.0.4/hyperlight/__init__.py
--rw-r--r--   0        0        0     6320 2023-04-30 17:16:14.247970 hyperlight-0.0.4/hyperlight/convert.py
--rw-r--r--   0        0        0     4101 2023-05-01 13:50:40.802147 hyperlight-0.0.4/hyperlight/find.py
--rw-r--r--   0        0        0       43 2023-04-30 17:07:30.229256 hyperlight-0.0.4/hyperlight/hypernet/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-30 17:07:30.233256 hyperlight-0.0.4/hyperlight/hypernet/encoding.py
--rw-r--r--   0        0        0     3624 2023-04-30 17:07:30.237256 hyperlight-0.0.4/hyperlight/hypernet/initialization.py
--rw-r--r--   0        0        0    15628 2023-05-06 20:41:05.214106 hyperlight-0.0.4/hyperlight/hypernet/model.py
--rw-r--r--   0        0        0      141 2023-04-30 17:07:30.241256 hyperlight-0.0.4/hyperlight/nn/__init__.py
--rw-r--r--   0        0        0      566 2023-04-30 17:07:30.245257 hyperlight-0.0.4/hyperlight/nn/container.py
--rw-r--r--   0        0        0     3888 2023-04-30 17:07:30.245257 hyperlight-0.0.4/hyperlight/nn/layers.py
--rw-r--r--   0        0        0     9494 2023-05-01 15:35:13.143976 hyperlight-0.0.4/hyperlight/nn/module.py
--rw-r--r--   0        0        0     4446 2023-04-30 17:07:30.253257 hyperlight-0.0.4/hyperlight/nn/xparam.py
--rw-r--r--   0        0        0     1442 2023-05-06 20:42:46.127397 hyperlight-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    13904 1970-01-01 00:00:00.000000 hyperlight-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-04-30 17:07:30.205256 hyperlight-0.0.5/LICENSE
+-rw-r--r--   0        0        0    13145 2023-05-06 20:41:23.110335 hyperlight-0.0.5/README.md
+-rw-r--r--   0        0        0      180 2023-05-07 00:15:30.508417 hyperlight-0.0.5/hyperlight/__init__.py
+-rw-r--r--   0        0        0     6320 2023-04-30 17:16:14.247970 hyperlight-0.0.5/hyperlight/convert.py
+-rw-r--r--   0        0        0     4101 2023-05-01 13:50:40.802147 hyperlight-0.0.5/hyperlight/find.py
+-rw-r--r--   0        0        0       43 2023-04-30 17:07:30.229256 hyperlight-0.0.5/hyperlight/hypernet/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-30 17:07:30.233256 hyperlight-0.0.5/hyperlight/hypernet/encoding.py
+-rw-r--r--   0        0        0     3624 2023-04-30 17:07:30.237256 hyperlight-0.0.5/hyperlight/hypernet/initialization.py
+-rw-r--r--   0        0        0    15643 2023-05-07 00:14:18.631510 hyperlight-0.0.5/hyperlight/hypernet/model.py
+-rw-r--r--   0        0        0      141 2023-04-30 17:07:30.241256 hyperlight-0.0.5/hyperlight/nn/__init__.py
+-rw-r--r--   0        0        0      566 2023-04-30 17:07:30.245257 hyperlight-0.0.5/hyperlight/nn/container.py
+-rw-r--r--   0        0        0     3888 2023-04-30 17:07:30.245257 hyperlight-0.0.5/hyperlight/nn/layers.py
+-rw-r--r--   0        0        0     9494 2023-05-01 15:35:13.143976 hyperlight-0.0.5/hyperlight/nn/module.py
+-rw-r--r--   0        0        0     4446 2023-04-30 17:07:30.253257 hyperlight-0.0.5/hyperlight/nn/xparam.py
+-rw-r--r--   0        0        0     1442 2023-05-07 00:15:30.504417 hyperlight-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    13904 1970-01-01 00:00:00.000000 hyperlight-0.0.5/PKG-INFO
```

### Comparing `hyperlight-0.0.4/LICENSE` & `hyperlight-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.4/README.md` & `hyperlight-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.4/hyperlight/convert.py` & `hyperlight-0.0.5/hyperlight/convert.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.4/hyperlight/find.py` & `hyperlight-0.0.5/hyperlight/find.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.4/hyperlight/hypernet/encoding.py` & `hyperlight-0.0.5/hyperlight/hypernet/encoding.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.4/hyperlight/hypernet/initialization.py` & `hyperlight-0.0.5/hyperlight/hypernet/initialization.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.4/hyperlight/hypernet/model.py` & `hyperlight-0.0.5/hyperlight/hypernet/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
                 shape = (batch_dim, *shape)
             outputs[name] = flat_output.narrow(1, *self._output_offsets[name]).view(
                 shape
             )
         return outputs
 
 
-class HyperNet(nn.Module):
+class HyperNet(nn.Module, HyperNetMixin):
     """A hypernetwork that generates weights for a target network. Shape is Dict[str, Tuple[int, ...]]
 
     Args:
         input_shapes (Dict[str, Shape]): The shapes of the inputs that the hypernetwork takes
         output_shapes (Dict[str, Shape]): The shapes of the primary network weights being predicted,
         hidden_sizes (List[int]): The sizes of the hidden layers of the hypernetwork.
         encoding (InputMode, optional): The input encoding mode. Defaults to "cos|sin".
```

### Comparing `hyperlight-0.0.4/hyperlight/nn/container.py` & `hyperlight-0.0.5/hyperlight/nn/container.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.4/hyperlight/nn/layers.py` & `hyperlight-0.0.5/hyperlight/nn/layers.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.4/hyperlight/nn/module.py` & `hyperlight-0.0.5/hyperlight/nn/module.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.4/hyperlight/nn/xparam.py` & `hyperlight-0.0.5/hyperlight/nn/xparam.py`

 * *Files identical despite different names*

### Comparing `hyperlight-0.0.4/pyproject.toml` & `hyperlight-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hyperlight"
 homepage = "https://github.com/JJGO/hyperlight"
 documentation = "https://github.com/JJGO/hyperlight"
-version = "0.0.4"
+version = "0.0.5"
 description = "Hyperlight is a Pytorch hypernetwork framework with a streamlined API"
 authors = ["Jose Javier Gonzalez Ortiz <josejg@mit.edu>"]
 license = "Apache-2.0"
 readme = "README.md"
 classifiers=[
     'Intended Audience :: Science/Research',
     'Intended Audience :: Developers',
@@ -35,15 +35,15 @@
 pyright = "^1.2.0"
 pre-commit = "^2.17.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.0.4"
+current_version = "0.0.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `hyperlight-0.0.4/PKG-INFO` & `hyperlight-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperlight
-Version: 0.0.4
+Version: 0.0.5
 Summary: Hyperlight is a Pytorch hypernetwork framework with a streamlined API
 Home-page: https://github.com/JJGO/hyperlight
 License: Apache-2.0
 Keywords: hyperlight,pytorch,hypernetworks,deep learning
 Author: Jose Javier Gonzalez Ortiz
 Author-email: josejg@mit.edu
 Requires-Python: >=3.7,<4.0
```

