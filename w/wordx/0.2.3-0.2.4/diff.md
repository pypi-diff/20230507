# Comparing `tmp/wordx-0.2.3.tar.gz` & `tmp/wordx-0.2.4.tar.gz`

## Comparing `wordx-0.2.3.tar` & `wordx-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wordx-0.2.3/src/wordx/__init__.py
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 wordx-0.2.3/src/wordx/fake_zip.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 wordx-0.2.3/src/wordx/sheet.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 wordx-0.2.3/src/wordx/utility.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 wordx-0.2.3/src/wordx/word_file.py
--rw-r--r--   0        0        0    25045 2020-02-02 00:00:00.000000 wordx-0.2.3/tests/1.png
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 wordx-0.2.3/tests/1.py
--rw-r--r--   0        0        0   241198 2020-02-02 00:00:00.000000 wordx-0.2.3/tests/123.docx
--rw-r--r--   0        0        0    12116 2020-02-02 00:00:00.000000 wordx-0.2.3/tests/2.docx
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 wordx-0.2.3/tests/3.docx
--rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 wordx-0.2.3/tests/footer.docx
--rw-r--r--   0        0        0    12201 2020-02-02 00:00:00.000000 wordx-0.2.3/tests/footer.xml
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 wordx-0.2.3/tests/haha.xml
--rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 wordx-0.2.3/tests/文档合并/123.docx
--rw-r--r--   0        0        0    14199 2020-02-02 00:00:00.000000 wordx-0.2.3/tests/文档合并/456.docx
--rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 wordx-0.2.3/tests/文档合并/merge.docx
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wordx-0.2.3/tests/文档合并/merge.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 wordx-0.2.3/LICENSE
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 wordx-0.2.3/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 wordx-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 wordx-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wordx-0.2.4/src/wordx/__init__.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 wordx-0.2.4/src/wordx/fake_zip.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 wordx-0.2.4/src/wordx/sheet.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 wordx-0.2.4/src/wordx/utility.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 wordx-0.2.4/src/wordx/word_file.py
+-rw-r--r--   0        0        0    25045 2020-02-02 00:00:00.000000 wordx-0.2.4/tests/1.png
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 wordx-0.2.4/tests/1.py
+-rw-r--r--   0        0        0   241198 2020-02-02 00:00:00.000000 wordx-0.2.4/tests/123.docx
+-rw-r--r--   0        0        0    12116 2020-02-02 00:00:00.000000 wordx-0.2.4/tests/2.docx
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 wordx-0.2.4/tests/3.docx
+-rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 wordx-0.2.4/tests/footer.docx
+-rw-r--r--   0        0        0    12201 2020-02-02 00:00:00.000000 wordx-0.2.4/tests/footer.xml
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 wordx-0.2.4/tests/haha.xml
+-rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 wordx-0.2.4/tests/文档合并/123.docx
+-rw-r--r--   0        0        0    14199 2020-02-02 00:00:00.000000 wordx-0.2.4/tests/文档合并/456.docx
+-rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 wordx-0.2.4/tests/文档合并/merge.docx
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wordx-0.2.4/tests/文档合并/merge.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 wordx-0.2.4/LICENSE
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 wordx-0.2.4/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 wordx-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 wordx-0.2.4/PKG-INFO
```

### Comparing `wordx-0.2.3/src/wordx/sheet.py` & `wordx-0.2.4/src/wordx/sheet.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,35 +16,35 @@
             'tuple': tuple,
             'list': list
         }
         return Template(tpl).render(**data, **lib)
 
     def render_header(self, data):
         """页眉渲染"""
-        header_xml = self.render_template(self.get_resource_as_str('header.xml'), data)
-        self.replace('word/header.xml', header_xml)
+        header_xml = self.retrieve(f'word/header.xml')
+        self['word/header.xml'] = self.render_template(header_xml, data)
 
     def render_footer(self, data):
-        """页脚渲染"""
-        footer_xml = self.render_template(self.get_resource_as_str('footer.xml'), data)
-        self.replace('word/footer.xml', footer_xml)
+        """页脚渲染""" 
+        footer_xml = self.retrieve(f'word/footer.xml')
+        self['word/footer.xml'] = self.render_template(footer_xml, data)
 
     def render_document(self, data):
         """文档渲染"""
-        document_xml = self.render_template(self.get_resource_as_str('document.xml'), data)
-        self.replace('word/document.xml', document_xml)
+        document_xml = self.retrieve(f'word/document.xml')
+        self['word/document.xml'] = self.render_template(document_xml, data)
 
     def render_and_add_header(self, data):
         """添加页眉"""
-        header_xml_data = self.render_template(self.get_resource_as_str('header.xml'), data)
+        header_xml_data = self.render_template(self.retrieve(f'word/header.xml'), data)
         return self.add_header(header_xml_data)
 
     def render_and_add_footer(self, data):
         """添加页脚"""
-        footer_xml_data = self.render_template(self.get_resource_as_str('footer.xml'), data)
+        footer_xml_data = self.render_template(self.retrieve(f'word/footer.xml'), data)
         return self.add_footer(footer_xml_data)
 
     def render(self, data):
         self.render_header(data)
         self.render_footer(data)
         self.render_document(data)
         return self
```

### Comparing `wordx-0.2.3/src/wordx/utility.py` & `wordx-0.2.4/src/wordx/utility.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 from lxml import etree
 from lxml.builder import E
 import random
 
 
 class ResourceUtility:
-    def get_resource(self, res_path):
-        return self.get(f'word/{res_path}')
-
     def get_resource_as_str(self, res_path):
-        return self.get_resource(res_path).decode()
+        return self[f'word/{res_path}'].decode()
 
     def add_resource(res_path, file_bytes):
-        self.add(f'word/{res_path}', file_bytes)
-
-    def add_media(self, filename, file_bytes):
-        self.add_resource(f'media/{filename}', file_bytes)
+        self[f'word/{res_path}'] = file_bytes
 
     def get_document(self):
-        return self.get_resource('document.xml')
+        return self[f'word/document.xml']
 
     def extract_resource(self, res_path, file_path):
-        data = self.get_resource(res_path)
+        data = self[f'word/{res_path}']
         with open(file_path, 'wb') as f:
             f.write(data)
 
 
 class RelationUtility:
     def get_relations(self, xml_file):
-        return self.get(f'word/_rels/{xml_file}.rels') 
+        return self[f'word/_rels/{xml_file}.rels']
 
     def get_document_relations(self):
         return self.get_relations('document.xml')
 
     def save_relations(self, xml_file, relations):
-        relations_path = f'word/_rels/{xml_file}.rels'
-        self.replace(relations_path, relations)
+        self[f'word/_rels/{xml_file}.rels'] = relations
 
     def merge_relations(self, relations_a, relations_b):
         relation_tree = etree.fromstring(relations_a)
         for relation in relations_b:
             relation_id = relation['id']
             relation_type = relation['type']
             relation_target = relation['target']
```

### Comparing `wordx-0.2.3/src/wordx/word_file.py` & `wordx-0.2.4/src/wordx/word_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 class WordFile(FakeZip, ResourceUtility, RelationUtility):
     def __init__(self, file_path):
         super().__init__(file_path)
 
     def add_footer(self, footer):
         footer_relation_id, footer_file = self.add_footer_relation()
-        self.add(f'word/{footer_file}', footer)
+        self[f'word/{footer_file}'] = footer
         self.register_xml({'path': f'/word/{footer_file}','type': 'footer'})
         return footer_relation_id
 
     def add_header(self, header):
         header_relation_id, header_file = self.add_header_relation()
-        self.add(f'word/{header_file}', header)
+        self[f'word/{header_file}'] = header
         self.register_xml({'path': f'/word/{header_file}','type': 'header'})
         return header_relation_id
 
     def register_xml(self, xml_data):
         xml_path = xml_data['path']
         xml_type = xml_data['type']
-        content_type_xml = self.get('[Content_Types].xml')
+        content_type_xml = self['[Content_Types].xml']
         content_type_tree = etree.fromstring(content_type_xml)
         content_type = f'application/vnd.openxmlformats-officedocument.wordprocessingml.{xml_type}+xml'
         content_type_new_element = E.Override(PartName = xml_path, ContentType = content_type)
         content_type_tree.append(content_type_new_element)
         content_type_xml = etree.tostring(content_type_tree)
-        self.replace('[Content_Types].xml', content_type_xml)
+        self['[Content_Types].xml'] = content_type_xml
         return self
 
     def mask_relations(self, xml_file):
         relations = self.get_relations(xml_file)
         relation_tree = etree.fromstring(relations)
         tmp = []
         for relation_element in relation_tree:
@@ -62,17 +62,17 @@
         return tmp
 
     def merge(self, wf):
         # 合并文件
         wf_relations = wf.mask_relations('document.xml')
         for wf_relation in wf_relations:
             filename = 'word/' + wf_relation['target']
-            content = wf.get(filename)
+            content = wf[filename]
             filename_ = 'word/' + wf_relation['target_']
-            self.add(filename_, content)
+            self[filename_] = content
         # 合并映射
         document_relations = self.get_document_relations()
         document_relations_ = self.merge_relations(document_relations, wf_relations)
         self.save_relations('document.xml', document_relations_)
 
 
         document = self.get_document().decode()
@@ -86,9 +86,9 @@
         etree2 = etree.fromstring(document2)
         etree1_body = etree1[0]
         etree2_body = etree2[0]
         sect_pr = etree1_body[-1]
         etree1_body.remove(sect_pr)
         for element in etree2_body:
             etree1_body.append(element)
-        self.replace('word/document.xml', etree.tostring(etree1).decode())
+        self['word/document.xml'] = etree.tostring(etree1).decode()
        	self.save('merge.docx')
```

### Comparing `wordx-0.2.3/tests/1.png` & `wordx-0.2.4/tests/1.png`

 * *Files identical despite different names*

### Comparing `wordx-0.2.3/tests/1.py` & `wordx-0.2.4/tests/1.py`

 * *Files identical despite different names*

### Comparing `wordx-0.2.3/tests/123.docx` & `wordx-0.2.4/tests/123.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.3/tests/2.docx` & `wordx-0.2.4/tests/2.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.3/tests/3.docx` & `wordx-0.2.4/tests/3.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.3/tests/footer.docx` & `wordx-0.2.4/tests/footer.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.3/tests/footer.xml` & `wordx-0.2.4/tests/footer.xml`

 * *Files identical despite different names*

### Comparing `wordx-0.2.3/tests/haha.xml` & `wordx-0.2.4/tests/haha.xml`

 * *Files identical despite different names*

### Comparing `wordx-0.2.3/tests/文档合并/123.docx` & `wordx-0.2.4/tests/文档合并/123.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.3/tests/文档合并/456.docx` & `wordx-0.2.4/tests/文档合并/456.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.3/tests/文档合并/merge.docx` & `wordx-0.2.4/tests/文档合并/merge.docx`

 * *Files identical despite different names*

### Comparing `wordx-0.2.3/LICENSE` & `wordx-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wordx-0.2.3/pyproject.toml` & `wordx-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wordx"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "generate word documents in a sexy way"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
-  "jinja2",
-  "lxml",
+  "jinja2==3.1.2",
+  "lxml==4.9.2",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

