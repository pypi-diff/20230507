# Comparing `tmp/cmx-0.0.8-py3-none-any.whl.zip` & `tmp/cmx-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9770 bytes, number of entries: 13
+Zip file size: 9816 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      192 b- defN 20-Sep-12 03:43 cmx/__init__.py
 -rw-r--r--  2.0 unx      581 b- defN 20-Sep-12 03:53 cmx/data.py
 -rw-r--r--  2.0 unx     1461 b- defN 20-Sep-14 18:15 cmx/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Jul-26 20:46 cmx/backends/__init__.py
--rw-r--r--  2.0 unx    11185 b- defN 20-Sep-14 19:45 cmx/backends/components.py
+-rw-r--r--  2.0 unx    11421 b- defN 20-Sep-16 05:42 cmx/backends/components.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Jul-26 20:46 cmx/backends/html.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Jul-26 20:46 cmx/backends/latex.py
 -rw-r--r--  2.0 unx     7533 b- defN 20-Sep-14 21:58 cmx/backends/markdown.py
--rw-r--r--  2.0 unx     1063 b- defN 20-Sep-14 22:10 cmx-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1424 b- defN 20-Sep-14 22:10 cmx-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-Sep-14 22:10 cmx-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 20-Sep-14 22:10 cmx-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      964 b- defN 20-Sep-14 22:10 cmx-0.0.8.dist-info/RECORD
-13 files, 24499 bytes uncompressed, 8176 bytes compressed:  66.6%
+-rw-r--r--  2.0 unx     1063 b- defN 20-Sep-16 14:42 cmx-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1424 b- defN 20-Sep-16 14:42 cmx-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 20-Sep-16 14:42 cmx-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 20-Sep-16 14:42 cmx-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      964 b- defN 20-Sep-16 14:42 cmx-0.0.9.dist-info/RECORD
+13 files, 24735 bytes uncompressed, 8222 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: cmx/backends/latex.py
 Comment: 
 
 Filename: cmx/backends/markdown.py
 Comment: 
 
-Filename: cmx-0.0.8.dist-info/LICENSE
+Filename: cmx-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: cmx-0.0.8.dist-info/METADATA
+Filename: cmx-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: cmx-0.0.8.dist-info/WHEEL
+Filename: cmx-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: cmx-0.0.8.dist-info/top_level.txt
+Filename: cmx-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: cmx-0.0.8.dist-info/RECORD
+Filename: cmx-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmx/backends/components.py

```diff
@@ -309,35 +309,40 @@
     def __init__(self, header=None, n_cols=None, **kwargs):
         super().__init__(**kwargs)
         # self.header = header
         # todo: add fixed n_cols support
         self.n_cols = n_cols
         self.titles = []
         self.images = []
-        self.captions = []
+        self.footers = []
 
     def figure(self, image=None, src=None, title=None, caption=None, **kwargs):
         # todo: if image is Image/Video/Component
         self.titles.append(title if title is None else Bold(title))
-        self.captions.append(caption if caption is None else Span(caption))
+        self.footers.append(caption if caption is None else Span(caption))
         self.image(image=image, src=src, **kwargs)
 
     def video(self, frames=None, src=None, title=None, caption=None, **kwargs):
         self.titles.append(title if title is None else Bold(title))
-        self.captions.append(caption if caption is None else Span(caption))
+        self.footers.append(caption if caption is None else Span(caption))
         v = self.window.video(frames=frames, src=src, window=self.window, **kwargs)
         self.children.append(v)
 
+    def column(self, title=None, text=None, footer=None):
+        self.titles.append(title if title is None else Bold(title))
+        self.footers.append(footer if footer is None else Span(footer))
+        self.children.append(Text(text))
+
     # def image(self):
     #     raise RuntimeError('please use figure instead of image.')
 
     @property
     def rows(self):
         non_empty_rows = []
-        for r in [self.titles, self.children, self.captions]:
+        for r in [self.titles, self.children, self.footers]:
             for item in r:
                 if item is not None:
                     non_empty_rows.append(r)
                     break
         return non_empty_rows
```

## Comparing `cmx-0.0.8.dist-info/LICENSE` & `cmx-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cmx-0.0.8.dist-info/METADATA` & `cmx-0.0.9.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmx
-Version: 0.0.8
+Version: 0.0.9
 Summary: long_description
 Home-page: https://github.com/cmx/cmx-python
 Author: Ge Yang<ge.ike.yang@gmail.com>
 Author-email: ge.ike.yang@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Dist: gym
```

## Comparing `cmx-0.0.8.dist-info/RECORD` & `cmx-0.0.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cmx/__init__.py,sha256=bQXoRGBBmGuxssVdZzZR2-ga6gtiYM-ZGYcaQ1CGpn0,192
 cmx/data.py,sha256=VX44xxYnddBlMV3svgWjTDfvTriqlfqHxgaeNyqpSXw,581
 cmx/utils.py,sha256=EGeonGu14xh2aP5tAMqxgcmFyJCUwC68qmRCtUpEjxU,1461
 cmx/backends/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cmx/backends/components.py,sha256=36svGYy-VucLGq0XNEIje2QEuSb4rzsDvtjqUsf1Sso,11185
+cmx/backends/components.py,sha256=tcNKkFSVCAxT0_4R_TqtbCgVE_WPzq09mArd-MyKpwc,11421
 cmx/backends/html.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cmx/backends/latex.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cmx/backends/markdown.py,sha256=aSvrEAx4ZqjD0_1Yiub0IAJDAlMY-qUD6c1JpqDqWhY,7533
-cmx-0.0.8.dist-info/LICENSE,sha256=nOTfVshy6RJQfmi64dLiNesUqoMZueHWS7RbXTK5k-E,1063
-cmx-0.0.8.dist-info/METADATA,sha256=DgVRcozrFKuP4DZuLfzmGqLKDF4hEQm-A86BnIkFqjg,1424
-cmx-0.0.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-cmx-0.0.8.dist-info/top_level.txt,sha256=odDkeX_EhztoToQW8w858SHj6AgXmGOdiN1Wi0jTxSI,4
-cmx-0.0.8.dist-info/RECORD,,
+cmx-0.0.9.dist-info/LICENSE,sha256=nOTfVshy6RJQfmi64dLiNesUqoMZueHWS7RbXTK5k-E,1063
+cmx-0.0.9.dist-info/METADATA,sha256=xEh7ljeu145GwKo1q8loED5Jn68HacR0_5SsOA--8mQ,1424
+cmx-0.0.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+cmx-0.0.9.dist-info/top_level.txt,sha256=odDkeX_EhztoToQW8w858SHj6AgXmGOdiN1Wi0jTxSI,4
+cmx-0.0.9.dist-info/RECORD,,
```

