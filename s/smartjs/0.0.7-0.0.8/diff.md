# Comparing `tmp/smartjs-0.0.7.tar.gz` & `tmp/smartjs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartjs-0.0.7.tar", max compression
+gzip compressed data, was "smartjs-0.0.8.tar", max compression
```

## Comparing `smartjs-0.0.7.tar` & `smartjs-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      302 2023-05-07 01:38:04.683465 smartjs-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      183 2023-05-05 14:06:40.683599 smartjs-0.0.7/smartjs/__init__.py
--rw-r--r--   0        0        0    13079 2023-05-06 23:09:29.043999 smartjs-0.0.7/smartjs/base.py
--rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.0.7/smartjs/constants.py
--rw-r--r--   0        0        0     4576 2023-05-06 23:09:29.046930 smartjs-0.0.7/smartjs/elements.py
--rw-r--r--   0        0        0     5805 2023-05-06 22:41:19.600790 smartjs-0.0.7/smartjs/functions.py
--rw-r--r--   0        0        0    11888 2023-05-06 23:09:29.039937 smartjs-0.0.7/smartjs/javascript.py
--rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.0.7/smartjs/page.py
--rw-r--r--   0        0        0      994 2023-05-07 01:38:04.688449 smartjs-0.0.7/smartjs/path.py
--rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.0.7/smartjs/style.py
--rw-r--r--   0        0        0      584 2023-05-07 01:38:12.061426 smartjs-0.0.7/setup.py
--rw-r--r--   0        0        0      333 2023-05-07 01:38:12.061650 smartjs-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      302 2023-05-07 13:14:18.311682 smartjs-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-05-05 14:06:40.683599 smartjs-0.0.8/smartjs/__init__.py
+-rw-r--r--   0        0        0    13214 2023-05-07 13:14:18.303555 smartjs-0.0.8/smartjs/base.py
+-rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.0.8/smartjs/constants.py
+-rw-r--r--   0        0        0     4879 2023-05-07 13:14:18.308482 smartjs-0.0.8/smartjs/elements.py
+-rw-r--r--   0        0        0     5805 2023-05-06 22:41:19.600790 smartjs-0.0.8/smartjs/functions.py
+-rw-r--r--   0        0        0    11888 2023-05-06 23:09:29.039937 smartjs-0.0.8/smartjs/javascript.py
+-rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.0.8/smartjs/page.py
+-rw-r--r--   0        0        0      994 2023-05-07 01:38:04.688449 smartjs-0.0.8/smartjs/path.py
+-rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.0.8/smartjs/style.py
+-rw-r--r--   0        0        0      584 2023-05-07 13:14:24.218109 smartjs-0.0.8/setup.py
+-rw-r--r--   0        0        0      333 2023-05-07 13:14:24.218325 smartjs-0.0.8/PKG-INFO
```

### Comparing `smartjs-0.0.7/smartjs/base.py` & `smartjs-0.0.8/smartjs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,20 @@
     def bootstrap(self):
         if self.is_form_field:
             if self.value == 'select':
                 return 'form-select'
             elif self.value == 'textarea':
                 return 'form-control'
         return None
+    
+    @property
+    def label_bootstrap(self):
+        if self.value == 'select':
+            return ''
+        return 'form-label'
 
 
 class InputType(Enum):
     _ignore_ = 'InputType i'
     InputType = vars()
     for i in INPUT_TYPES:
         InputType[f'{i}'.upper().replace("-", "_")] = i
```

### Comparing `smartjs-0.0.7/smartjs/constants.py` & `smartjs-0.0.8/smartjs/constants.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.7/smartjs/elements.py` & `smartjs-0.0.8/smartjs/elements.py`

 * *Files 9% similar despite different names*

```diff
@@ -193,15 +193,25 @@
 
 
 class Form(BaseElement):
 	KLASS = 'form-control'
 
 
 class Option(BaseElement):
-	pass
+	def __init__(self, value: str = None, id: str = None, text: str = None, default: bool = False):
+		args = []
+		if value:
+			args.append(Kwarg('value', value))
+		if id:
+			args.append(Kwarg('id', id))
+		if text:
+			args.append(Text(text))
+		if default:
+			args.append(Arg('checked'))
+		super().__init__(*args)
 
 
 class BaseUniqueElement(BaseElement):
 	@property
 	def post_init_kwargs(self):
 		return dict(id=type(self).__name__.lower())
```

### Comparing `smartjs-0.0.7/smartjs/functions.py` & `smartjs-0.0.8/smartjs/functions.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.7/smartjs/javascript.py` & `smartjs-0.0.8/smartjs/javascript.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.7/smartjs/page.py` & `smartjs-0.0.8/smartjs/page.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.7/smartjs/path.py` & `smartjs-0.0.8/smartjs/path.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.7/smartjs/style.py` & `smartjs-0.0.8/smartjs/style.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.7/setup.py` & `smartjs-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'smartjs',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': '',
     'long_description': None,
     'author': 'Daniel Victor',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

