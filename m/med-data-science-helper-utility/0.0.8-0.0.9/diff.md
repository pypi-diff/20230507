# Comparing `tmp/med-data-science-helper-utility-0.0.8.tar.gz` & `tmp/med-data-science-helper-utility-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\med-data-science-helper-utility-0.0.8.tar", last modified: Mon May 16 05:38:24 2022, max compression
+gzip compressed data, was "dist\med-data-science-helper-utility-0.0.9.tar", last modified: Mon May 16 15:18:54 2022, max compression
```

## Comparing `med-data-science-helper-utility-0.0.8.tar` & `med-data-science-helper-utility-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-05-16 05:38:24.000000 med-data-science-helper-utility-0.0.8/
--rw-rw-rw-   0        0        0      684 2022-05-16 05:38:24.000000 med-data-science-helper-utility-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       21 2022-04-16 22:53:16.000000 med-data-science-helper-utility-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-05-16 05:38:24.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper/
--rw-rw-rw-   0        0        0        0 2022-03-18 15:45:43.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper/__init__.py
--rw-rw-rw-   0        0        0    34330 2022-05-15 19:28:56.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper/helper_acces_db.py
--rw-rw-rw-   0        0        0     4962 2022-05-06 22:07:36.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper/helper_integracion.py
--rw-rw-rw-   0        0        0    66318 2022-05-15 19:31:19.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper/helper_siagie_kpi.py
--rw-rw-rw-   0        0        0    36762 2022-05-04 04:24:08.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper/helper_siagie_kpi_old.py
--rw-rw-rw-   0        0        0     7324 2022-05-15 20:24:13.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper/helper_terceros_kpi.py
-drwxrwxrwx   0        0        0        0 2022-05-16 05:38:24.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper_utility.egg-info/
--rw-rw-rw-   0        0        0      684 2022-05-16 05:38:24.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper_utility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2022-05-16 05:38:24.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper_utility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-16 05:38:24.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper_utility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2022-05-16 05:38:24.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper_utility.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2022-05-16 05:38:24.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper_utility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2022-05-16 05:38:24.000000 med-data-science-helper-utility-0.0.8/med_data_science_helper_utility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-16 05:38:24.000000 med-data-science-helper-utility-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     4461 2022-05-16 05:38:07.000000 med-data-science-helper-utility-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-16 05:38:24.000000 med-data-science-helper-utility-0.0.8/test/
--rw-rw-rw-   0        0        0      562 2022-05-06 22:08:03.000000 med-data-science-helper-utility-0.0.8/test/test_helper_acces_db.py
--rw-rw-rw-   0        0        0      319 2022-05-06 22:07:36.000000 med-data-science-helper-utility-0.0.8/test/test_import.py
+drwxrwxrwx   0        0        0        0 2022-05-16 15:18:54.000000 med-data-science-helper-utility-0.0.9/
+-rw-rw-rw-   0        0        0      684 2022-05-16 15:18:54.000000 med-data-science-helper-utility-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2022-04-16 22:53:16.000000 med-data-science-helper-utility-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-05-16 15:18:54.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper/
+-rw-rw-rw-   0        0        0        0 2022-03-18 15:45:43.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper/__init__.py
+-rw-rw-rw-   0        0        0    35138 2022-05-16 15:08:03.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper/helper_acces_db.py
+-rw-rw-rw-   0        0        0     4962 2022-05-06 22:07:36.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper/helper_integracion.py
+-rw-rw-rw-   0        0        0    66318 2022-05-15 19:31:19.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper/helper_siagie_kpi.py
+-rw-rw-rw-   0        0        0    36762 2022-05-04 04:24:08.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper/helper_siagie_kpi_old.py
+-rw-rw-rw-   0        0        0     7324 2022-05-15 20:24:13.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper/helper_terceros_kpi.py
+drwxrwxrwx   0        0        0        0 2022-05-16 15:18:54.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper_utility.egg-info/
+-rw-rw-rw-   0        0        0      684 2022-05-16 15:18:53.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper_utility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2022-05-16 15:18:53.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper_utility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-16 15:18:53.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper_utility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2022-05-16 15:18:53.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper_utility.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2022-05-16 15:18:53.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper_utility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2022-05-16 15:18:53.000000 med-data-science-helper-utility-0.0.9/med_data_science_helper_utility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-05-16 15:18:54.000000 med-data-science-helper-utility-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     4461 2022-05-16 15:18:11.000000 med-data-science-helper-utility-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-16 15:18:54.000000 med-data-science-helper-utility-0.0.9/test/
+-rw-rw-rw-   0        0        0      629 2022-05-16 15:15:25.000000 med-data-science-helper-utility-0.0.9/test/test_helper_acces_db.py
+-rw-rw-rw-   0        0        0      319 2022-05-06 22:07:36.000000 med-data-science-helper-utility-0.0.9/test/test_import.py
```

### Comparing `med-data-science-helper-utility-0.0.8/PKG-INFO` & `med-data-science-helper-utility-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: med-data-science-helper-utility
-Version: 0.0.8
+Version: 0.0.9
 Summary: med-data-science-helper-utility de proyectos de analitica avanzada
 Download-URL: https://URL_PAQUETE/med-data-science-helper-utility/-/archive/master/med-data-science-helper-utility-master.tar
 Author: Analitica Avanzada
 Author-email: analitica.avanzada.talento@gmail.com
 License: NOTFOUND
 Keywords: med-data-science-helper-utility,paquete,package
 Platform: UNKNOWN
```

### Comparing `med-data-science-helper-utility-0.0.8/med_data_science_helper/helper_acces_db.py` & `med-data-science-helper-utility-0.0.9/med_data_science_helper/helper_acces_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,40 +94,64 @@
         
     df = get_juntos(anio=anio, cache=cache)
     
     df_ = df.groupby(["TIPODOC_MO",'DNI_MO'])[['RESULTADO_HOGAR']].agg('count').reset_index()   
         
     return df_
 
+'''
+url_template = get_path_BD()+'\\07.Nexus\\_data_\\{}'     
+url_nexus = url_template.format('nexus_2018_2019.xlsb')    
+anio = 2019
+df_nexus = pd.read_excel(url_nexus, engine='pyxlsb',sheet_name=str(anio))   
+print(df_nexus.columns)
+print(df_nexus.SITUACION.value_counts()) 
 
-    
+SITUACION
+'''
 def get_nexus(anio=2020,subtipo_trabajador=["DOCENTE"], estado_plaza=["Activo","Encargatura"], cache=False):  
 
     if anio in [2015,2016,2017,2020,2021] :
         filename = 'nexus_2015_2016_2017_2020_2021.xlsb'
     elif anio in [2018,2019]:
         filename = 'nexus_2018_2019.xlsb'
     else :
         return None
-      
+
+    if(subtipo_trabajador is None):
+        subtipo_trabajador = []
+        
+    if(estado_plaza is None):
+        estado_plaza = []
+
+    params = subtipo_trabajador+estado_plaza
+    params_str = '_'.join(params)
+    
     df_nexus_group = None
-    key_cache = hc.get_key_cache([anio])
+    key_cache = hc.get_key_cache([anio,params_str])
     print(key_cache)
     if cache:
         df_nexus_group = hc.get_cache(filename,key_cache)
         
     if df_nexus_group is not None:
         return df_nexus_group
 
     
     url_template = get_path_BD()+'\\07.Nexus\\_data_\\{}'     
     url_nexus = url_template.format(filename)    
     
     df_nexus = pd.read_excel(url_nexus, engine='pyxlsb',sheet_name=str(anio))       
     
+#    if filename == "nexus_2015_2016_2017_2020_2021.xlsb":
+#        df_nexus.rename(columns={"MODULAR IE": "codmod"},inplace=True)
+        
+    if filename == "nexus_2018_2019.xlsb":
+        df_nexus.rename(columns={"SITUACION": "SITUACION LAB"},inplace=True)
+        
+    
     df_nexus['MODULAR IE'] = df_nexus['MODULAR IE'].str.strip()
     df_nexus['SITUACION LAB'] = df_nexus['SITUACION LAB'].str.strip()
     df_nexus['ESTADO PLAZA'] = df_nexus['ESTADO PLAZA'].str.strip()
     df_nexus['SUBTIPO TRABAJADOR'] = df_nexus['SUBTIPO TRABAJADOR'].str.strip()
     df_nexus['NIVEL EDUCATIVO'] = df_nexus['NIVEL EDUCATIVO'].str.strip()    
 
     df_nexus.rename(columns={"MODULAR IE": "codmod"},inplace=True)
```

### Comparing `med-data-science-helper-utility-0.0.8/med_data_science_helper/helper_integracion.py` & `med-data-science-helper-utility-0.0.9/med_data_science_helper/helper_integracion.py`

 * *Files identical despite different names*

### Comparing `med-data-science-helper-utility-0.0.8/med_data_science_helper/helper_siagie_kpi.py` & `med-data-science-helper-utility-0.0.9/med_data_science_helper/helper_siagie_kpi.py`

 * *Files identical despite different names*

### Comparing `med-data-science-helper-utility-0.0.8/med_data_science_helper/helper_siagie_kpi_old.py` & `med-data-science-helper-utility-0.0.9/med_data_science_helper/helper_siagie_kpi_old.py`

 * *Files identical despite different names*

### Comparing `med-data-science-helper-utility-0.0.8/med_data_science_helper/helper_terceros_kpi.py` & `med-data-science-helper-utility-0.0.9/med_data_science_helper/helper_terceros_kpi.py`

 * *Files identical despite different names*

### Comparing `med-data-science-helper-utility-0.0.8/med_data_science_helper_utility.egg-info/PKG-INFO` & `med-data-science-helper-utility-0.0.9/med_data_science_helper_utility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: med-data-science-helper-utility
-Version: 0.0.8
+Version: 0.0.9
 Summary: med-data-science-helper-utility de proyectos de analitica avanzada
 Download-URL: https://URL_PAQUETE/med-data-science-helper-utility/-/archive/master/med-data-science-helper-utility-master.tar
 Author: Analitica Avanzada
 Author-email: analitica.avanzada.talento@gmail.com
 License: NOTFOUND
 Keywords: med-data-science-helper-utility,paquete,package
 Platform: UNKNOWN
```

### Comparing `med-data-science-helper-utility-0.0.8/med_data_science_helper_utility.egg-info/SOURCES.txt` & `med-data-science-helper-utility-0.0.9/med_data_science_helper_utility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `med-data-science-helper-utility-0.0.8/setup.py` & `med-data-science-helper-utility-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 import json
 from os import path
 from setuptools import setup, find_packages
 from sys import version_info
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 CURR_PATH = "{}{}".format(path.abspath(path.dirname(__file__)), '/')
 
 
 
 
 def path_format(file_path=None, file_name=None, is_abspath=False,
                 ignore_raises=False):
```

### Comparing `med-data-science-helper-utility-0.0.8/test/test_helper_acces_db.py` & `med-data-science-helper-utility-0.0.9/test/test_helper_acces_db.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 
 import med_data_science_helper.helper_acces_db as hadb
 
 
 print(hadb.get_path_BD())
 
+df = hadb.get_nexus(anio=2015,cache=True,subtipo_trabajador=None)
 
 df = hadb.get_ECE_2P()
 df = hadb.get_ECE_4P()
 df = hadb.get_ECE_2S()
 df = hadb.get_ECE()
 
 df = hadb.get_Censo_Educativo(anio=2019)
```

