# Comparing `tmp/quick-csv-0.0.5.tar.gz` & `tmp/quick-csv-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick-csv-0.0.5.tar", last modified: Tue Aug 30 09:57:30 2022, max compression
+gzip compressed data, was "quick-csv-0.0.6a0.tar", last modified: Sun May  7 00:49:31 2023, max compression
```

## Comparing `quick-csv-0.0.5.tar` & `quick-csv-0.0.6a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-08-30 09:57:30.390172 quick-csv-0.0.5/
--rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 quick-csv-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      252 2022-01-22 19:50:32.000000 quick-csv-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3864 2022-08-30 09:57:30.391168 quick-csv-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2649 2022-05-08 15:40:33.000000 quick-csv-0.0.5/README.md
--rw-rw-rw-   0        0        0       81 2022-08-30 09:57:30.392165 quick-csv-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     8499 2022-08-30 09:57:00.000000 quick-csv-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-30 09:57:30.350129 quick-csv-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2022-08-30 09:57:30.359105 quick-csv-0.0.5/src/quick_csv.egg-info/
--rw-rw-rw-   0        0        0     3864 2022-08-30 09:57:29.000000 quick-csv-0.0.5/src/quick_csv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2022-08-30 09:57:30.000000 quick-csv-0.0.5/src/quick_csv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-30 09:57:29.000000 quick-csv-0.0.5/src/quick_csv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2022-08-30 09:57:29.000000 quick-csv-0.0.5/src/quick_csv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-30 09:57:29.000000 quick-csv-0.0.5/src/quick_csv.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-30 09:57:30.360132 quick-csv-0.0.5/src/quickcsv/
--rw-rw-rw-   0        0        0       27 2022-08-30 09:57:00.000000 quick-csv-0.0.5/src/quickcsv/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-30 09:57:30.385035 quick-csv-0.0.5/src/quickcsv/__pycache__/
--rw-rw-rw-   0        0        0      163 2022-01-22 20:11:01.000000 quick-csv-0.0.5/src/quickcsv/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      231 2022-05-08 15:40:34.000000 quick-csv-0.0.5/src/quickcsv/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2171 2022-01-22 20:14:44.000000 quick-csv-0.0.5/src/quickcsv/__pycache__/file.cpython-36.pyc
--rw-rw-rw-   0        0        0     4118 2022-05-08 15:27:05.000000 quick-csv-0.0.5/src/quickcsv/__pycache__/file.cpython-39.pyc
--rw-rw-rw-   0        0        0     2174 2022-05-08 15:40:34.000000 quick-csv-0.0.5/src/quickcsv/__pycache__/largefile.cpython-39.pyc
--rw-rw-rw-   0        0        0     4682 2022-08-30 09:57:00.000000 quick-csv-0.0.5/src/quickcsv/file.py
--rw-rw-rw-   0        0        0     3263 2022-05-08 15:31:51.000000 quick-csv-0.0.5/src/quickcsv/largefile.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:49:31.082198 quick-csv-0.0.6a0/
+-rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 quick-csv-0.0.6a0/LICENSE
+-rw-rw-rw-   0        0        0      252 2022-01-22 19:50:32.000000 quick-csv-0.0.6a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4708 2023-05-07 00:49:31.082198 quick-csv-0.0.6a0/PKG-INFO
+-rw-rw-rw-   0        0        0     2649 2022-05-08 15:40:33.000000 quick-csv-0.0.6a0/README.md
+-rw-rw-rw-   0        0        0       81 2023-05-07 00:49:31.082198 quick-csv-0.0.6a0/setup.cfg
+-rw-rw-rw-   0        0        0     8516 2023-05-06 23:10:56.000000 quick-csv-0.0.6a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:49:31.050977 quick-csv-0.0.6a0/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 00:49:31.082198 quick-csv-0.0.6a0/src/quick_csv.egg-info/
+-rw-rw-rw-   0        0        0     4708 2023-05-07 00:49:30.000000 quick-csv-0.0.6a0/src/quick_csv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-05-07 00:49:30.000000 quick-csv-0.0.6a0/src/quick_csv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 00:49:30.000000 quick-csv-0.0.6a0/src/quick_csv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-07 00:49:30.000000 quick-csv-0.0.6a0/src/quick_csv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 00:49:30.000000 quick-csv-0.0.6a0/src/quick_csv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 00:49:31.082198 quick-csv-0.0.6a0/src/quickcsv/
+-rw-rw-rw-   0        0        0       27 2022-08-30 09:57:00.000000 quick-csv-0.0.6a0/src/quickcsv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:49:31.082198 quick-csv-0.0.6a0/src/quickcsv/__pycache__/
+-rw-rw-rw-   0        0        0      163 2022-01-22 20:11:01.000000 quick-csv-0.0.6a0/src/quickcsv/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      201 2023-05-07 00:37:51.000000 quick-csv-0.0.6a0/src/quickcsv/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2171 2022-01-22 20:14:44.000000 quick-csv-0.0.6a0/src/quickcsv/__pycache__/file.cpython-36.pyc
+-rw-rw-rw-   0        0        0     5447 2023-05-07 00:41:18.000000 quick-csv-0.0.6a0/src/quickcsv/__pycache__/file.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2174 2022-05-08 15:40:34.000000 quick-csv-0.0.6a0/src/quickcsv/__pycache__/largefile.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6142 2023-05-07 00:49:19.000000 quick-csv-0.0.6a0/src/quickcsv/file.py
+-rw-rw-rw-   0        0        0     3261 2023-05-07 00:49:19.000000 quick-csv-0.0.6a0/src/quickcsv/largefile.py
```

### Comparing `quick-csv-0.0.5/LICENSE` & `quick-csv-0.0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `quick-csv-0.0.5/PKG-INFO` & `quick-csv-0.0.6a0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,125 @@
 Metadata-Version: 2.1
 Name: quick-csv
-Version: 0.0.5
+Version: 0.0.6a0
 Summary: Read and write CSV or TXT files in a simple manner
 Home-page: https://github.com/dhchenx/quick-csv
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/quick-csv/issues
 Project-URL: Source, https://github.com/dhchenx/quick-csv
+Description: ## Quick CSV
+        
+        Read and write small or large CSV/TXT files in a simple manner
+        
+        ### Installation
+        ```pip
+        pip install quick-csv
+        ```
+        
+        ### Examples for small files
+        Example 1: read and write csv or txt files
+        ```python
+        from quickcsv.file import *
+        # read a csv file
+        list_model=read_csv('data/test.csv')
+        for idx,model in enumerate(list_model):
+            print(model)
+            list_model[idx]['id']=idx
+        # save a csv file
+        write_csv('data/test1.csv',list_model)
+        
+        # write a text file
+        write_text('data/text1.txt',"Hello World!")
+        # read a text file
+        print(read_text('data/text1.txt'))
+        ```
+        Example 2: create dataframe from a list of models
+        ```python
+        from quickcsv.file import *
+        # read a csv file
+        list_model=read_csv('data/test.csv')
+        # create a dataframe from list_model
+        df=create_df(list_model)
+        # print
+        print(df)
+        ```
+        
+        ### Examples for large files
+        Example 1: read large csv file
+        ```python
+        from quickcsv.largefile import *
+        if __name__=="__main__":
+            csv_path=r"umls_atui_rels.csv" # a large file (>500 MB)
+            total_count=0
+        
+            def process_partition(part_df,i):
+                print(f"Part {i}")
+        
+            def process_row(row,i):
+                global total_count
+                print(i)
+                total_count+=1
+        
+            list_results=read_large_csv(csv_file=csv_path,row_func=process_row,partition_func=process_partition)
+        
+            print("Return: ")
+            print(list_results)
+        
+            print("Total Record Num: ",total_count)
+        
+        ```
+        
+        Example 2: query from a large csv file
+        ```python
+        from quickcsv.largefile import *
+        
+        if __name__=="__main__":
+            csv_path=r"umls_sui_nodes.csv" # a large file (>500 MB)
+            total_count=0
+            # process each partition in the large file
+            def process_partition(part_df,i):
+                print(f"Part {i}")
+                print()
+            # process each row in a partition while reading
+            def process_row(row,i):
+                global total_count
+                print(row)
+                total_count+=1
+            # field is a field in the csv file, and value is the value you need to find within the csv file
+            list_results=read_large_csv(csv_file=csv_path, field="SUI",value="S0000004", append_row=True, row_func=process_row,partition_func=process_partition)
+        
+            print("Return: ")
+            print(list_results)
+        
+            print("Total Record Num: ",total_count)
+        ```
+        
+        Example 3: read top N records from the large csv file
+        ```python
+        from quickcsv.largefile import *
+        
+        if __name__=="__main__":
+            csv_path=r"umls_atui_rels.csv"
+            total_count=0
+            # return top 10 rows in the csv file
+            list_results=read_large_csv(csv_file=csv_path,head_num=10)
+        
+            print("Return: ")
+            print(list_results)
+        
+            print("Total Record Num: ",total_count)
+        ```
+        
+        ### License
+        
+        The `quick-csv` project is provided by [Donghua Chen](https://github.com/dhchenx). 
+        
+        
 Keywords: csv file,txt file,write,read,quick-csv,quickcsv
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,118 +128,7 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE
-
-## Quick CSV
-
-Read and write small or large CSV/TXT files in a simple manner
-
-### Installation
-```pip
-pip install quick-csv
-```
-
-### Examples for small files
-Example 1: read and write csv or txt files
-```python
-from quickcsv.file import *
-# read a csv file
-list_model=read_csv('data/test.csv')
-for idx,model in enumerate(list_model):
-    print(model)
-    list_model[idx]['id']=idx
-# save a csv file
-write_csv('data/test1.csv',list_model)
-
-# write a text file
-write_text('data/text1.txt',"Hello World!")
-# read a text file
-print(read_text('data/text1.txt'))
-```
-Example 2: create dataframe from a list of models
-```python
-from quickcsv.file import *
-# read a csv file
-list_model=read_csv('data/test.csv')
-# create a dataframe from list_model
-df=create_df(list_model)
-# print
-print(df)
-```
-
-### Examples for large files
-Example 1: read large csv file
-```python
-from quickcsv.largefile import *
-if __name__=="__main__":
-    csv_path=r"umls_atui_rels.csv" # a large file (>500 MB)
-    total_count=0
-
-    def process_partition(part_df,i):
-        print(f"Part {i}")
-
-    def process_row(row,i):
-        global total_count
-        print(i)
-        total_count+=1
-
-    list_results=read_large_csv(csv_file=csv_path,row_func=process_row,partition_func=process_partition)
-
-    print("Return: ")
-    print(list_results)
-
-    print("Total Record Num: ",total_count)
-
-```
-
-Example 2: query from a large csv file
-```python
-from quickcsv.largefile import *
-
-if __name__=="__main__":
-    csv_path=r"umls_sui_nodes.csv" # a large file (>500 MB)
-    total_count=0
-    # process each partition in the large file
-    def process_partition(part_df,i):
-        print(f"Part {i}")
-        print()
-    # process each row in a partition while reading
-    def process_row(row,i):
-        global total_count
-        print(row)
-        total_count+=1
-    # field is a field in the csv file, and value is the value you need to find within the csv file
-    list_results=read_large_csv(csv_file=csv_path, field="SUI",value="S0000004", append_row=True, row_func=process_row,partition_func=process_partition)
-
-    print("Return: ")
-    print(list_results)
-
-    print("Total Record Num: ",total_count)
-```
-
-Example 3: read top N records from the large csv file
-```python
-from quickcsv.largefile import *
-
-if __name__=="__main__":
-    csv_path=r"umls_atui_rels.csv"
-    total_count=0
-    # return top 10 rows in the csv file
-    list_results=read_large_csv(csv_file=csv_path,head_num=10)
-
-    print("Return: ")
-    print(list_results)
-
-    print("Total Record Num: ",total_count)
-```
-
-### License
-
-The `quick-csv` project is provided by [Donghua Chen](https://github.com/dhchenx). 
-
-
-
```

### Comparing `quick-csv-0.0.5/README.md` & `quick-csv-0.0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `quick-csv-0.0.5/setup.py` & `quick-csv-0.0.6a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.5',  # Required
+    version='0.0.6a0',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Read and write CSV or TXT files in a simple manner',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -141,15 +141,15 @@
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=[
-
+        "dask",
     ],  # Optional
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
```

### Comparing `quick-csv-0.0.5/src/quick_csv.egg-info/PKG-INFO` & `quick-csv-0.0.6a0/src/quick_csv.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,125 @@
 Metadata-Version: 2.1
 Name: quick-csv
-Version: 0.0.5
+Version: 0.0.6a0
 Summary: Read and write CSV or TXT files in a simple manner
 Home-page: https://github.com/dhchenx/quick-csv
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/quick-csv/issues
 Project-URL: Source, https://github.com/dhchenx/quick-csv
+Description: ## Quick CSV
+        
+        Read and write small or large CSV/TXT files in a simple manner
+        
+        ### Installation
+        ```pip
+        pip install quick-csv
+        ```
+        
+        ### Examples for small files
+        Example 1: read and write csv or txt files
+        ```python
+        from quickcsv.file import *
+        # read a csv file
+        list_model=read_csv('data/test.csv')
+        for idx,model in enumerate(list_model):
+            print(model)
+            list_model[idx]['id']=idx
+        # save a csv file
+        write_csv('data/test1.csv',list_model)
+        
+        # write a text file
+        write_text('data/text1.txt',"Hello World!")
+        # read a text file
+        print(read_text('data/text1.txt'))
+        ```
+        Example 2: create dataframe from a list of models
+        ```python
+        from quickcsv.file import *
+        # read a csv file
+        list_model=read_csv('data/test.csv')
+        # create a dataframe from list_model
+        df=create_df(list_model)
+        # print
+        print(df)
+        ```
+        
+        ### Examples for large files
+        Example 1: read large csv file
+        ```python
+        from quickcsv.largefile import *
+        if __name__=="__main__":
+            csv_path=r"umls_atui_rels.csv" # a large file (>500 MB)
+            total_count=0
+        
+            def process_partition(part_df,i):
+                print(f"Part {i}")
+        
+            def process_row(row,i):
+                global total_count
+                print(i)
+                total_count+=1
+        
+            list_results=read_large_csv(csv_file=csv_path,row_func=process_row,partition_func=process_partition)
+        
+            print("Return: ")
+            print(list_results)
+        
+            print("Total Record Num: ",total_count)
+        
+        ```
+        
+        Example 2: query from a large csv file
+        ```python
+        from quickcsv.largefile import *
+        
+        if __name__=="__main__":
+            csv_path=r"umls_sui_nodes.csv" # a large file (>500 MB)
+            total_count=0
+            # process each partition in the large file
+            def process_partition(part_df,i):
+                print(f"Part {i}")
+                print()
+            # process each row in a partition while reading
+            def process_row(row,i):
+                global total_count
+                print(row)
+                total_count+=1
+            # field is a field in the csv file, and value is the value you need to find within the csv file
+            list_results=read_large_csv(csv_file=csv_path, field="SUI",value="S0000004", append_row=True, row_func=process_row,partition_func=process_partition)
+        
+            print("Return: ")
+            print(list_results)
+        
+            print("Total Record Num: ",total_count)
+        ```
+        
+        Example 3: read top N records from the large csv file
+        ```python
+        from quickcsv.largefile import *
+        
+        if __name__=="__main__":
+            csv_path=r"umls_atui_rels.csv"
+            total_count=0
+            # return top 10 rows in the csv file
+            list_results=read_large_csv(csv_file=csv_path,head_num=10)
+        
+            print("Return: ")
+            print(list_results)
+        
+            print("Total Record Num: ",total_count)
+        ```
+        
+        ### License
+        
+        The `quick-csv` project is provided by [Donghua Chen](https://github.com/dhchenx). 
+        
+        
 Keywords: csv file,txt file,write,read,quick-csv,quickcsv
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,118 +128,7 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE
-
-## Quick CSV
-
-Read and write small or large CSV/TXT files in a simple manner
-
-### Installation
-```pip
-pip install quick-csv
-```
-
-### Examples for small files
-Example 1: read and write csv or txt files
-```python
-from quickcsv.file import *
-# read a csv file
-list_model=read_csv('data/test.csv')
-for idx,model in enumerate(list_model):
-    print(model)
-    list_model[idx]['id']=idx
-# save a csv file
-write_csv('data/test1.csv',list_model)
-
-# write a text file
-write_text('data/text1.txt',"Hello World!")
-# read a text file
-print(read_text('data/text1.txt'))
-```
-Example 2: create dataframe from a list of models
-```python
-from quickcsv.file import *
-# read a csv file
-list_model=read_csv('data/test.csv')
-# create a dataframe from list_model
-df=create_df(list_model)
-# print
-print(df)
-```
-
-### Examples for large files
-Example 1: read large csv file
-```python
-from quickcsv.largefile import *
-if __name__=="__main__":
-    csv_path=r"umls_atui_rels.csv" # a large file (>500 MB)
-    total_count=0
-
-    def process_partition(part_df,i):
-        print(f"Part {i}")
-
-    def process_row(row,i):
-        global total_count
-        print(i)
-        total_count+=1
-
-    list_results=read_large_csv(csv_file=csv_path,row_func=process_row,partition_func=process_partition)
-
-    print("Return: ")
-    print(list_results)
-
-    print("Total Record Num: ",total_count)
-
-```
-
-Example 2: query from a large csv file
-```python
-from quickcsv.largefile import *
-
-if __name__=="__main__":
-    csv_path=r"umls_sui_nodes.csv" # a large file (>500 MB)
-    total_count=0
-    # process each partition in the large file
-    def process_partition(part_df,i):
-        print(f"Part {i}")
-        print()
-    # process each row in a partition while reading
-    def process_row(row,i):
-        global total_count
-        print(row)
-        total_count+=1
-    # field is a field in the csv file, and value is the value you need to find within the csv file
-    list_results=read_large_csv(csv_file=csv_path, field="SUI",value="S0000004", append_row=True, row_func=process_row,partition_func=process_partition)
-
-    print("Return: ")
-    print(list_results)
-
-    print("Total Record Num: ",total_count)
-```
-
-Example 3: read top N records from the large csv file
-```python
-from quickcsv.largefile import *
-
-if __name__=="__main__":
-    csv_path=r"umls_atui_rels.csv"
-    total_count=0
-    # return top 10 rows in the csv file
-    list_results=read_large_csv(csv_file=csv_path,head_num=10)
-
-    print("Return: ")
-    print(list_results)
-
-    print("Total Record Num: ",total_count)
-```
-
-### License
-
-The `quick-csv` project is provided by [Donghua Chen](https://github.com/dhchenx). 
-
-
-
```

### Comparing `quick-csv-0.0.5/src/quick_csv.egg-info/SOURCES.txt` & `quick-csv-0.0.6a0/src/quick_csv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quick-csv-0.0.5/src/quickcsv/__pycache__/file.cpython-36.pyc` & `quick-csv-0.0.6a0/src/quickcsv/__pycache__/file.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-csv-0.0.5/src/quickcsv/__pycache__/largefile.cpython-39.pyc` & `quick-csv-0.0.6a0/src/quickcsv/__pycache__/largefile.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-csv-0.0.5/src/quickcsv/file.py` & `quick-csv-0.0.6a0/src/quickcsv/file.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,26 @@
 
 def write_csv(save_path,list_rows=None,encoding='utf-8'):
     '''
         write csv file with a list of model dictionaries
     '''
     return qc_write(save_path=save_path,list_rows=list_rows,encoding=encoding)
 
+def read_csv_gbk(csv_path,fields=None,func_row=None,func_row_field=None):
+    '''
+        read csv file as a list of model dictionaries in GBK encoding
+    '''
+    return qc_read(csv_path=csv_path,fields=fields,func_row=func_row,func_row_field=func_row_field,encoding='gbk')
+
+def write_csv_gbk(save_path,list_rows=None):
+    '''
+        write csv file with a list of model dictionaries in GBK encoding
+    '''
+    return qc_write(save_path=save_path,list_rows=list_rows,encoding='gbk')
+
 def write_text(file_path,str,encoding='utf-8',mode='w'):
     '''
         write plain text content
     '''
     return qc_twrite(file_path=file_path,str=str,encoding=encoding,mode=mode)
 
 def read_text(file_path,encoding='utf-8',mode='r'):
@@ -119,15 +131,46 @@
             if k in dict_values:
                 dict_values[k].append(item[k])
             else:
                 dict_values[k]=[item[k]]
     df = pd.DataFrame(data=dict_values)
     return df
 
-
 def to_sorted_dict(dict,reverse=True):
     '''
     Convert a dict to ordered dict
     '''
     dict = OrderedDict(sorted(dict.items(), key=lambda obj: obj[1], reverse=reverse))
     return dict
 
+def quick_combine_csv(csv_path1,csv_path2,use_field=None,save_csv_path=None,remove_duplicate=True):
+    '''
+    Combine two csv files into a single CSV file according to settings.
+    '''
+    list_item1 = read_csv(csv_path1)
+    list_item2 = read_csv(csv_path2)
+
+    if use_field==None:
+        use_field=list(list_item1[0].keys())[0]
+
+    print(f"Combining two csv files according to [{use_field}]")
+
+    list_all = []
+    list_id = []
+    for item in list_item1:
+        url = item[use_field]
+        if remove_duplicate:
+            if url in list_id:
+                continue
+        list_all.append(item)
+        list_id.append(url)
+
+    for item in list_item2:
+        url = item[use_field]
+        if remove_duplicate:
+            if url in list_id:
+                continue
+        list_all.append(item)
+        list_id.append(url)
+    if save_csv_path!=None:
+        write_csv(save_csv_path, list_all)
+    return list_all
```

### Comparing `quick-csv-0.0.5/src/quickcsv/largefile.py` & `quick-csv-0.0.6a0/src/quickcsv/largefile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import time
-
 from dask import dataframe as dd
 
 def cols_from_large_csv(csv_file,encoding='utf-8',low_memeory=False,):
     dask_df = dd.read_csv(csv_file,  low_memory=low_memeory, encoding=encoding)
     cols = list(dask_df.columns.values)
     return cols
```

