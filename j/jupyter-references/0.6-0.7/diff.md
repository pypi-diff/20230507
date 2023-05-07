# Comparing `tmp/jupyter-references-0.6.tar.gz` & `tmp/jupyter-references-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-references-0.6.tar", last modified: Sat May  6 09:14:43 2023, max compression
+gzip compressed data, was "jupyter-references-0.7.tar", last modified: Sun May  7 07:23:08 2023, max compression
```

## Comparing `jupyter-references-0.6.tar` & `jupyter-references-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-06 09:14:43.446964 jupyter-references-0.6/
--rw-r--r--   0 kmt        (501) staff       (20)     1069 2023-05-05 17:02:48.000000 jupyter-references-0.6/LICENSE
--rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-06 09:14:43.446724 jupyter-references-0.6/PKG-INFO
--rw-r--r--   0 kmt        (501) staff       (20)     1711 2023-05-05 17:02:48.000000 jupyter-references-0.6/README.md
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-06 09:14:43.443013 jupyter-references-0.6/jupyter_references/
--rw-r--r--   0 kmt        (501) staff       (20)     3904 2023-05-06 09:11:24.000000 jupyter-references-0.6/jupyter_references/__init__.py
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-06 09:14:43.446183 jupyter-references-0.6/jupyter_references.egg-info/
--rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-06 09:14:43.000000 jupyter-references-0.6/jupyter_references.egg-info/PKG-INFO
--rw-r--r--   0 kmt        (501) staff       (20)      266 2023-05-06 09:14:43.000000 jupyter-references-0.6/jupyter_references.egg-info/SOURCES.txt
--rw-r--r--   0 kmt        (501) staff       (20)        1 2023-05-06 09:14:43.000000 jupyter-references-0.6/jupyter_references.egg-info/dependency_links.txt
--rw-r--r--   0 kmt        (501) staff       (20)       26 2023-05-06 09:14:43.000000 jupyter-references-0.6/jupyter_references.egg-info/requires.txt
--rw-r--r--   0 kmt        (501) staff       (20)       19 2023-05-06 09:14:43.000000 jupyter-references-0.6/jupyter_references.egg-info/top_level.txt
--rw-r--r--   0 kmt        (501) staff       (20)       38 2023-05-06 09:14:43.447019 jupyter-references-0.6/setup.cfg
--rw-r--r--   0 kmt        (501) staff       (20)     1114 2023-05-06 09:10:58.000000 jupyter-references-0.6/setup.py
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-07 07:23:08.220586 jupyter-references-0.7/
+-rw-r--r--   0 kmt        (501) staff       (20)     1069 2023-05-05 17:02:48.000000 jupyter-references-0.7/LICENSE
+-rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-07 07:23:08.218812 jupyter-references-0.7/PKG-INFO
+-rw-r--r--   0 kmt        (501) staff       (20)     1711 2023-05-05 17:02:48.000000 jupyter-references-0.7/README.md
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-07 07:23:08.206473 jupyter-references-0.7/jupyter_references/
+-rw-r--r--   0 kmt        (501) staff       (20)     4203 2023-05-07 07:15:35.000000 jupyter-references-0.7/jupyter_references/__init__.py
+drwxr-xr-x   0 kmt        (501) staff       (20)        0 2023-05-07 07:23:08.217014 jupyter-references-0.7/jupyter_references.egg-info/
+-rw-r--r--   0 kmt        (501) staff       (20)     2062 2023-05-07 07:23:08.000000 jupyter-references-0.7/jupyter_references.egg-info/PKG-INFO
+-rw-r--r--   0 kmt        (501) staff       (20)      266 2023-05-07 07:23:08.000000 jupyter-references-0.7/jupyter_references.egg-info/SOURCES.txt
+-rw-r--r--   0 kmt        (501) staff       (20)        1 2023-05-07 07:23:08.000000 jupyter-references-0.7/jupyter_references.egg-info/dependency_links.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       26 2023-05-07 07:23:08.000000 jupyter-references-0.7/jupyter_references.egg-info/requires.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       19 2023-05-07 07:23:08.000000 jupyter-references-0.7/jupyter_references.egg-info/top_level.txt
+-rw-r--r--   0 kmt        (501) staff       (20)       38 2023-05-07 07:23:08.220656 jupyter-references-0.7/setup.cfg
+-rw-r--r--   0 kmt        (501) staff       (20)     1114 2023-05-07 07:16:03.000000 jupyter-references-0.7/setup.py
```

### Comparing `jupyter-references-0.6/LICENSE` & `jupyter-references-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-references-0.6/PKG-INFO` & `jupyter-references-0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-references
-Version: 0.6
+Version: 0.7
 Summary: Lightweight system for citing papers and making a reference list in jupyter
 Home-page: https://github.com/kaspermunch/jupyter-references
 Author: Kasper Munch
 Author-email: kaspermunch@birc.au.dk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyter-references-0.6/README.md` & `jupyter-references-0.7/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-references-0.6/jupyter_references/__init__.py` & `jupyter-references-0.7/jupyter_references/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import sys
 import ipynbname
 import json
 import re
 from IPython.lib import clipboard
 from IPython.core.magic import Magics, magics_class, line_magic
 
+import bibtexparser
+from thefuzz import fuzz, process
+
 @magics_class
 class MyMagics(Magics):
     
     @line_magic
     def replace_content(self, line):
         self.shell.set_next_input(line, replace=True)
         
@@ -24,22 +27,22 @@
     cite_list = []
     for i, entry in enumerate(bibtex_entries):
 
         match = re.search(r'@\w+{([^,]+).*year = {(\d+)}.*title = {{(.*)}}.*author = {([^,]+)', entry, re.DOTALL)
         if match:
             url, year, title, author = match.groups()
             if len(bibtex_entries) == 1:
-                cite_list.append(f'[({author} {year})](https://doi.org/{url} "{author} et al.\n{year}\n{title}\nDOI:{url}")')
+                cite_list.append(f'[({author} et al. {year})](https://doi.org/{url} "{title}")')
             else:
                 if i == 0:
-                    cite_list.append(f'[({author} {year},](https://doi.org/{url} "{author} et al.\n{year}\n{title}\nDOI:{url}")')
+                    cite_list.append(f'[({author} et al., {year},](https://doi.org/{url} "{title}")')
                 elif i+1 == len(bibtex_entries):
-                    cite_list.append(f'[{author} {year})](https://doi.org/{url} "{author} et al.\n{year}\n{title}\nDOI:{url}")')
+                    cite_list.append(f'[{author} et al. {year})](https://doi.org/{url} "{title}")')
                 else:
-                    cite_list.append(f'[{author} {year},](https://doi.org/{url} "{author} et al.\n{year}\n{title}\nDOI:{url}")')
+                    cite_list.append(f'[{author} et al. {year},](https://doi.org/{url} "{title}")')
     content = ' '.join(cite_list)
     if content:
         get_ipython().run_line_magic('replace_content', f"{content}") 
     else:
         print('clipboard is not bibtex:', cb)
         
 def incite(cb=None):
@@ -50,49 +53,73 @@
         print('clipboard has bibtex entries:', cb)
     else:
         match = re.search(r'@\w+{([^,]+).*year = {(\d+)}.*title = {{(.*)}}.*author = {([^,]+)',
             cb, re.DOTALL)
         if match:
             ref_list = {}
             url, year, title, author = match.groups()
-            content = f'{author} et al. [({year})](https://doi.org/{url} "{author} et al.\n{year}\n{title}\nDOI:{url}")'
+            content = f'{author} et al. [({year})](https://doi.org/{url} "{title}")'
             get_ipython().run_line_magic('replace_content', f"{content}") 
         else:
             print('clipboard is not bibtex:', cb)
         
 
 def ref_format_callback(i, ref):
-    return f"{i}. {ref['author']}, {ref['year']}, _{ref['title']}_, [{ref['doi']}](https://doi.org/{ref['doi'].replace('DOI:', '')})"
+    #format authors
+    last_names, first_names = zip(*[token.split(', ') for token in refs['author'].split(' and ')])
+    if len(last_names) <= 3:
+        last_names = last_names[:3]
+    last_names = ', '.join(last_names[:-1]) + ' and ' + last_names[-1]
+    ref['author'] = last_names
+        
+    return f"{i}. " + "{author}, {year},\n**{title}**,\n{doi}".format(**ref)
+
 
-def reflist(file_base_name=None, format_fun=ref_format_callback):
-    regex = re.compile(r'\d+\s+"([^"]+)"')
-    references = {}
+def sort_fun(ref):
+    return ref['author']
+    
+    
+def reflist(file_base_name=None, format_fun=ref_format_callback, sort_fun=sort_fun):
+
+    with open('bibtex.bib') as bibtex_file:
+        db = bibtexparser.load(bibtex_file)
+        bib_database = {}
+        for entry in db.entries:
+            bib_database[entry['ID']] = entry
+
+    regex = re.compile(r'https://doi.org/(\S+)\s+"')
+    references = []
     if file_base_name is None:
         file_base_name = ipynbname.name()
     if type(file_base_name) is not list:
         file_base_names = [file_base_name]
     else:
         file_base_names = file_base_name
     for name in file_base_names:
         with open(os.path.abspath(name+'.ipynb')) as f:
             notebook_json = json.load(f)
         for cell in notebook_json['cells']:
             if cell['cell_type'] == 'markdown':
                 source = ''.join(cell['source'])
-                for ref in regex.findall(source):
-                    try:
-                        author, year, title, doi = ref.split('\n')
-                        references[ref] = dict(author=author.strip(),
-                                            year=year.strip(), 
-                                            title=title.strip(),
-                                            doi=doi.strip())
-                    except ValueError:
-                        print(f'Skipping invalid ref: {ref}', file=sys.stderr)
-
-    lst = []
-    for i, (key, ref) in enumerate(sorted(references.items())):
-        lst.append(format_fun(i+1, ref))
-    content = "\n".join(lst)
-    content = '## References\n\n' + content
+                for doi in regex.findall(source):
+                    ref = bib_database[doi]
+                    references.append(ref)
+
+    l = []
+    for ref in sorted(references, key=sort_fun):
+        if not l or ref['ID'] != l[-1]['ID']:
+            l.append(ref)
+    references = l
+
+    ref_list = []
+    for i, ref in enumerate(references):
+        try:
+            ref['title'] = ref['title'][1:-1]
+            ref_list.append(format_fun(i+1, ref))
+        except KeyError:
+            print(f'Skipping invalid ref: {ref}', file=sys.stderr)
+
+    content = "\n".join(ref_list)
     get_ipython().run_line_magic('replace_content', f"{content}") 
             
+
```

### Comparing `jupyter-references-0.6/jupyter_references.egg-info/PKG-INFO` & `jupyter-references-0.7/jupyter_references.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-references
-Version: 0.6
+Version: 0.7
 Summary: Lightweight system for citing papers and making a reference list in jupyter
 Home-page: https://github.com/kaspermunch/jupyter-references
 Author: Kasper Munch
 Author-email: kaspermunch@birc.au.dk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyter-references-0.6/setup.py` & `jupyter-references-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 # package name must be the git repository name
 package_name = path.basename(this_directory)
 
 setuptools.setup(
     name=package_name,
-    version="0.6",
+    version="0.7",
     author="Kasper Munch",
     author_email="kaspermunch@birc.au.dk",
     description="Lightweight system for citing papers and making a reference list in jupyter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f'https://github.com/kaspermunch/{package_name}',
     packages=setuptools.find_packages(),
```

