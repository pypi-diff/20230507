# Comparing `tmp/agspiel-python-api-0.5.4.tar.gz` & `tmp/agspiel-python-api-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agspiel-python-api-0.5.4.tar", last modified: Mon Mar 27 23:04:39 2023, max compression
+gzip compressed data, was "agspiel-python-api-0.5.5.tar", last modified: Sun May  7 12:10:49 2023, max compression
```

## Comparing `agspiel-python-api-0.5.4.tar` & `agspiel-python-api-0.5.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 kevinbaier   (501) staff       (20)        0 2023-03-27 23:04:39.004719 agspiel-python-api-0.5.4/
--rw-r--r--   0 kevinbaier   (501) staff       (20)     1068 2020-08-08 11:42:25.000000 agspiel-python-api-0.5.4/LICENSE
--rw-r--r--   0 kevinbaier   (501) staff       (20)     2683 2023-03-27 23:04:39.004319 agspiel-python-api-0.5.4/PKG-INFO
--rw-r--r--   0 kevinbaier   (501) staff       (20)     2197 2020-08-20 13:25:22.000000 agspiel-python-api-0.5.4/README.md
-drwxr-xr-x   0 kevinbaier   (501) staff       (20)        0 2023-03-27 23:04:38.986260 agspiel-python-api-0.5.4/agspiel/
--rw-r--r--   0 kevinbaier   (501) staff       (20)      101 2020-08-09 08:30:46.000000 agspiel-python-api-0.5.4/agspiel/__init__.py
-drwxr-xr-x   0 kevinbaier   (501) staff       (20)        0 2023-03-27 23:04:38.994951 agspiel-python-api-0.5.4/agspiel/api/
--rw-r--r--   0 kevinbaier   (501) staff       (20)       90 2020-08-09 09:21:56.000000 agspiel-python-api-0.5.4/agspiel/api/__init__.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)    15818 2023-03-27 23:01:09.000000 agspiel-python-api-0.5.4/agspiel/api/ag.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)      620 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.4/agspiel/api/aktie.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)     1648 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.4/agspiel/api/anleihe.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)     3594 2021-07-24 17:27:21.000000 agspiel-python-api-0.5.4/agspiel/api/api.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)      857 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.4/agspiel/api/ceo.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)     1251 2021-07-23 10:04:19.000000 agspiel-python-api-0.5.4/agspiel/api/data.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)     5035 2023-03-10 14:48:28.000000 agspiel-python-api-0.5.4/agspiel/api/historic_ag.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)      774 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.4/agspiel/api/index.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)     1080 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.4/agspiel/api/kapitalmassnahme.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)     2777 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.4/agspiel/api/markt.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)     1425 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.4/agspiel/api/order.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)     1180 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.4/agspiel/api/zertifikat.py
-drwxr-xr-x   0 kevinbaier   (501) staff       (20)        0 2023-03-27 23:04:38.997656 agspiel-python-api-0.5.4/agspiel/utils/
--rw-r--r--   0 kevinbaier   (501) staff       (20)       90 2021-07-08 16:19:59.000000 agspiel-python-api-0.5.4/agspiel/utils/__init__.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)     3948 2021-07-24 17:27:21.000000 agspiel-python-api-0.5.4/agspiel/utils/controller.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)      194 2021-07-24 17:27:21.000000 agspiel-python-api-0.5.4/agspiel/utils/errors.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)     1091 2021-05-19 19:54:15.000000 agspiel-python-api-0.5.4/agspiel/utils/main.py
-drwxr-xr-x   0 kevinbaier   (501) staff       (20)        0 2023-03-27 23:04:39.001074 agspiel-python-api-0.5.4/agspiel_python_api.egg-info/
--rw-r--r--   0 kevinbaier   (501) staff       (20)     2683 2023-03-27 23:04:38.000000 agspiel-python-api-0.5.4/agspiel_python_api.egg-info/PKG-INFO
--rw-r--r--   0 kevinbaier   (501) staff       (20)      746 2023-03-27 23:04:38.000000 agspiel-python-api-0.5.4/agspiel_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 kevinbaier   (501) staff       (20)        1 2023-03-27 23:04:38.000000 agspiel-python-api-0.5.4/agspiel_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 kevinbaier   (501) staff       (20)       39 2023-03-27 23:04:38.000000 agspiel-python-api-0.5.4/agspiel_python_api.egg-info/requires.txt
--rw-r--r--   0 kevinbaier   (501) staff       (20)       14 2023-03-27 23:04:38.000000 agspiel-python-api-0.5.4/agspiel_python_api.egg-info/top_level.txt
--rw-r--r--   0 kevinbaier   (501) staff       (20)       38 2023-03-27 23:04:39.004871 agspiel-python-api-0.5.4/setup.cfg
--rw-r--r--   0 kevinbaier   (501) staff       (20)      830 2023-03-27 23:03:55.000000 agspiel-python-api-0.5.4/setup.py
-drwxr-xr-x   0 kevinbaier   (501) staff       (20)        0 2023-03-27 23:04:39.003647 agspiel-python-api-0.5.4/tests/
--rw-r--r--   0 kevinbaier   (501) staff       (20)        0 2020-08-09 09:23:53.000000 agspiel-python-api-0.5.4/tests/__init__.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)    16801 2023-03-27 22:58:06.000000 agspiel-python-api-0.5.4/tests/test_ag.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)      403 2020-08-13 13:41:55.000000 agspiel-python-api-0.5.4/tests/test_api.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)     5701 2023-03-10 14:49:14.000000 agspiel-python-api-0.5.4/tests/test_historic_ag.py
--rw-r--r--   0 kevinbaier   (501) staff       (20)     1752 2020-08-23 11:52:48.000000 agspiel-python-api-0.5.4/tests/test_markt.py
+drwxr-xr-x   0 kevinbaier   (501) staff       (20)        0 2023-05-07 12:10:49.514073 agspiel-python-api-0.5.5/
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     1068 2020-08-08 11:42:25.000000 agspiel-python-api-0.5.5/LICENSE
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     2683 2023-05-07 12:10:49.513704 agspiel-python-api-0.5.5/PKG-INFO
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     2197 2020-08-20 13:25:22.000000 agspiel-python-api-0.5.5/README.md
+drwxr-xr-x   0 kevinbaier   (501) staff       (20)        0 2023-05-07 12:10:49.495186 agspiel-python-api-0.5.5/agspiel/
+-rw-r--r--   0 kevinbaier   (501) staff       (20)      101 2020-08-09 08:30:46.000000 agspiel-python-api-0.5.5/agspiel/__init__.py
+drwxr-xr-x   0 kevinbaier   (501) staff       (20)        0 2023-05-07 12:10:49.503389 agspiel-python-api-0.5.5/agspiel/api/
+-rw-r--r--   0 kevinbaier   (501) staff       (20)       90 2020-08-09 09:21:56.000000 agspiel-python-api-0.5.5/agspiel/api/__init__.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)    15225 2023-05-07 11:38:27.000000 agspiel-python-api-0.5.5/agspiel/api/ag.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)      620 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.5/agspiel/api/aktie.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     1648 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.5/agspiel/api/anleihe.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     3594 2021-07-24 17:27:21.000000 agspiel-python-api-0.5.5/agspiel/api/api.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)      985 2023-05-07 11:37:51.000000 agspiel-python-api-0.5.5/agspiel/api/ceo.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     1251 2021-07-23 10:04:19.000000 agspiel-python-api-0.5.5/agspiel/api/data.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     5035 2023-03-10 14:48:28.000000 agspiel-python-api-0.5.5/agspiel/api/historic_ag.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)      774 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.5/agspiel/api/index.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     1080 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.5/agspiel/api/kapitalmassnahme.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     2777 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.5/agspiel/api/markt.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     1425 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.5/agspiel/api/order.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     1180 2021-04-19 19:32:36.000000 agspiel-python-api-0.5.5/agspiel/api/zertifikat.py
+drwxr-xr-x   0 kevinbaier   (501) staff       (20)        0 2023-05-07 12:10:49.506936 agspiel-python-api-0.5.5/agspiel/utils/
+-rw-r--r--   0 kevinbaier   (501) staff       (20)       90 2021-07-08 16:19:59.000000 agspiel-python-api-0.5.5/agspiel/utils/__init__.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     3948 2021-07-24 17:27:21.000000 agspiel-python-api-0.5.5/agspiel/utils/controller.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)      194 2021-07-24 17:27:21.000000 agspiel-python-api-0.5.5/agspiel/utils/errors.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     1091 2021-05-19 19:54:15.000000 agspiel-python-api-0.5.5/agspiel/utils/main.py
+drwxr-xr-x   0 kevinbaier   (501) staff       (20)        0 2023-05-07 12:10:49.509355 agspiel-python-api-0.5.5/agspiel_python_api.egg-info/
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     2683 2023-05-07 12:10:49.000000 agspiel-python-api-0.5.5/agspiel_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 kevinbaier   (501) staff       (20)      746 2023-05-07 12:10:49.000000 agspiel-python-api-0.5.5/agspiel_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinbaier   (501) staff       (20)        1 2023-05-07 12:10:49.000000 agspiel-python-api-0.5.5/agspiel_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinbaier   (501) staff       (20)       39 2023-05-07 12:10:49.000000 agspiel-python-api-0.5.5/agspiel_python_api.egg-info/requires.txt
+-rw-r--r--   0 kevinbaier   (501) staff       (20)       14 2023-05-07 12:10:49.000000 agspiel-python-api-0.5.5/agspiel_python_api.egg-info/top_level.txt
+-rw-r--r--   0 kevinbaier   (501) staff       (20)       38 2023-05-07 12:10:49.514248 agspiel-python-api-0.5.5/setup.cfg
+-rw-r--r--   0 kevinbaier   (501) staff       (20)      830 2023-05-07 11:52:39.000000 agspiel-python-api-0.5.5/setup.py
+drwxr-xr-x   0 kevinbaier   (501) staff       (20)        0 2023-05-07 12:10:49.512778 agspiel-python-api-0.5.5/tests/
+-rw-r--r--   0 kevinbaier   (501) staff       (20)        0 2020-08-09 09:23:53.000000 agspiel-python-api-0.5.5/tests/__init__.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)    17079 2023-05-07 11:41:23.000000 agspiel-python-api-0.5.5/tests/test_ag.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)      403 2020-08-13 13:41:55.000000 agspiel-python-api-0.5.5/tests/test_api.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     5701 2023-03-10 14:49:14.000000 agspiel-python-api-0.5.5/tests/test_historic_ag.py
+-rw-r--r--   0 kevinbaier   (501) staff       (20)     1752 2020-08-23 11:52:48.000000 agspiel-python-api-0.5.5/tests/test_markt.py
```

### Comparing `agspiel-python-api-0.5.4/LICENSE` & `agspiel-python-api-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/PKG-INFO` & `agspiel-python-api-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agspiel-python-api
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python API für das AG-Spiel
 Home-page: https://github.com/KingKevin23/agspiel-python-api
 Author: KingKevin23
 Author-email: code@kingkevin.de
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `agspiel-python-api-0.5.4/README.md` & `agspiel-python-api-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel/api/ag.py` & `agspiel-python-api-0.5.5/agspiel/api/ag.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     @property
     def in_liquidation(self) -> bool:
         return self._ag_data().get("in_liquidation")
 
     @property
     def in_kapitalerhoehung(self) -> bool:
-        return "Diese AG befindet sich in einer Kapitalerhöhung" in str(self._web_data())
+        return self._ag_data().get("laufende_ke")
 
     @property
     def kurs(self) -> float:
         return float(self._ag_data().get("kurs"))
 
     @property
     def brief(self) -> float:
@@ -172,17 +172,18 @@
                           gruendung_datum=index_gruendung)
         except TypeError:  # Wenn Spieler in keinem Index
             index = None
 
         registrierung_datum = datetime.strptime(self._ag_data().get("ceo").get("registrierung_datum"),
                                                 "%Y-%m-%d %H:%M:%S")
         gesperrt = self._ag_data().get("ceo").get("gesperrt")
+        premium = self._ag_data().get("ceo").get("premium")
         userprojekt = self._ag_data().get("ceo").get("ist_userprojekt_account")
         return Ceo(name=name, index=index, registrierung_datum=registrierung_datum, gesperrt=gesperrt,
-                   userprojekt=userprojekt)
+                   premium=premium, userprojekt=userprojekt)
 
     @property
     def aktien(self) -> list:
         aktien = []
         for i in self._ag_data().get("aktien"):
             temp = Aktie(wkn=int(i.get("wkn")), stueckzahl=int(i.get("stueckzahl")))
             aktien.append(temp)
@@ -289,41 +290,27 @@
                         gesamt = float(cols[3].text.replace(".", "").replace(",", ".").replace("€", "").strip())
                     khs.append(Kapitalherabsetzung(datum, anzahl, preis, gesamt))
 
         return khs
 
     @property
     def dividende(self) -> float:
-        table_data = {}
-        rows = self._web_data().find('table', attrs={'class': 'padding5'}).find_all('tr')
-        for row in rows:
-            cols = row.find_all("td")
-            table_data[cols[0].text] = cols[1].text
-
-        return float(re.compile("(0\.?\d{0,2})%").findall(table_data.get("Dividende"))[0])
+        return float(self._ag_data().get("dividende"))
 
     @property
     def max_zertis(self) -> int:
-        table_data = {}
-        rows = self._web_data().find('table', attrs={'class': 'padding5'}).find_all('tr')
-        for row in rows:
-            cols = row.find_all("td")
-            table_data[cols[0].text] = cols[1].text
+        return int(float(self._ag_data().get("max_zertifikate_anteil")) * 100)
 
-        return int(re.compile("(\d{1,2})%").findall(table_data.get("Max. Zertifikatevol."))[0])
+    @property
+    def max_zertis_aenderbar(self) -> bool:
+        return self._ag_data().get("max_zertifikate_anteil_aenderbar")
 
     @property
     def uebernahmeschutz(self) -> bool:
-        table_data = {}
-        rows = self._web_data().find('table', attrs={'class': 'padding5'}).find_all('tr')
-        for row in rows:
-            cols = row.find_all("td")
-            table_data[cols[0].text] = cols[1].text
-
-        return table_data.get("Hat Übernahmeschutz?").strip() == "ja"
+        return self._ag_data().get("uebernahmeschutz")
 
     @property
     def tages_hoch(self) -> float:
         table_data = {}
         rows = self._web_data().find('table', attrs={'class': 'padding5'}).find_all('tr')
         for row in rows:
             cols = row.find_all("td")
```

### Comparing `agspiel-python-api-0.5.4/agspiel/api/aktie.py` & `agspiel-python-api-0.5.5/agspiel/api/aktie.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel/api/anleihe.py` & `agspiel-python-api-0.5.5/agspiel/api/anleihe.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel/api/api.py` & `agspiel-python-api-0.5.5/agspiel/api/api.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel/api/ceo.py` & `agspiel-python-api-0.5.5/agspiel/api/ceo.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 from datetime import datetime
 
 from .index import Index
 
 
 class Ceo:
-    def __init__(self, name: str, index: Index, registrierung_datum: datetime, gesperrt: bool, userprojekt: bool):
+    def __init__(self, name: str, index: Index, registrierung_datum: datetime, gesperrt: bool, premium: bool, userprojekt: bool):
         self._name: str = name
         self._index: Index = index
         self._registrierung_datum: datetime = registrierung_datum
         self._gesperrt: bool = gesperrt
+        self._premium: bool = premium
         self._userprojekt: bool = userprojekt
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
@@ -26,9 +27,13 @@
         return self._registrierung_datum
 
     @property
     def gesperrt(self) -> bool:
         return self._gesperrt
 
     @property
+    def premium(self) -> bool:
+        return self._premium
+
+    @property
     def userprojekt(self) -> bool:
         return self._userprojekt
```

### Comparing `agspiel-python-api-0.5.4/agspiel/api/data.py` & `agspiel-python-api-0.5.5/agspiel/api/data.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel/api/historic_ag.py` & `agspiel-python-api-0.5.5/agspiel/api/historic_ag.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel/api/index.py` & `agspiel-python-api-0.5.5/agspiel/api/index.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel/api/kapitalmassnahme.py` & `agspiel-python-api-0.5.5/agspiel/api/kapitalmassnahme.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel/api/markt.py` & `agspiel-python-api-0.5.5/agspiel/api/markt.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel/api/order.py` & `agspiel-python-api-0.5.5/agspiel/api/order.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel/api/zertifikat.py` & `agspiel-python-api-0.5.5/agspiel/api/zertifikat.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel/utils/controller.py` & `agspiel-python-api-0.5.5/agspiel/utils/controller.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel/utils/main.py` & `agspiel-python-api-0.5.5/agspiel/utils/main.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/agspiel_python_api.egg-info/PKG-INFO` & `agspiel-python-api-0.5.5/agspiel_python_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agspiel-python-api
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python API für das AG-Spiel
 Home-page: https://github.com/KingKevin23/agspiel-python-api
 Author: KingKevin23
 Author-email: code@kingkevin.de
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `agspiel-python-api-0.5.4/agspiel_python_api.egg-info/SOURCES.txt` & `agspiel-python-api-0.5.5/agspiel_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/setup.py` & `agspiel-python-api-0.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="agspiel-python-api",
-    version="0.5.4",
+    version="0.5.5",
     author="KingKevin23",
     author_email="code@kingkevin.de",
     description="Python API für das AG-Spiel",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT License",
     url="https://github.com/KingKevin23/agspiel-python-api",
```

### Comparing `agspiel-python-api-0.5.4/tests/test_ag.py` & `agspiel-python-api-0.5.5/tests/test_ag.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,16 @@
         self.assertEqual(self.ag.ceo.index.gruendung_datum, datetime(year=2019, month=11, day=19, hour=0, minute=10, second=12))
         self.assertIsInstance(self.ag.ceo.index.gruendung_datum, datetime)
 
         self.assertEqual(self.ag.ceo.registrierung_datum, datetime(year=2020, month=2, day=4, hour=16, minute=24))
         self.assertIsInstance(self.ag.ceo.registrierung_datum, datetime)
         self.assertEqual(self.ag.ceo.gesperrt, False)
         self.assertIsInstance(self.ag.ceo.gesperrt, bool)
+        self.assertEqual(self.ag.ceo.premium, True)
+        self.assertIsInstance(self.ag.ceo.premium, bool)
         self.assertEqual(self.ag.ceo.userprojekt, True)
         self.assertIsInstance(self.ag.ceo.userprojekt, bool)
 
     def test_aktien(self):
         for i in self.ag.aktien:
             self.assertIsInstance(i, Aktie)
         self.assertEqual(self.ag.aktien[0].wkn, 146244)
@@ -330,14 +332,18 @@
         self.assertEqual(self.ag.dividende, 0)
         self.assertIsInstance(self.ag.dividende, float)
 
     def test_max_zertis(self):
         self.assertEqual(self.ag.max_zertis, 5)
         self.assertIsInstance(self.ag.max_zertis, int)
 
+    def test_max_zertis_aenderbar(self):
+        self.assertEqual(self.ag.max_zertis_aenderbar, True)
+        self.assertIsInstance(self.ag.max_zertis_aenderbar, bool)
+
     def test_uebernahmeschutz(self):
         self.assertEqual(self.ag.uebernahmeschutz, False)
         self.assertIsInstance(self.ag.uebernahmeschutz, bool)
 
     def test_tages_hoch(self):
         self.assertEqual(self.ag.tages_hoch, 423.35)
         self.assertIsInstance(self.ag.tages_hoch, float)
```

### Comparing `agspiel-python-api-0.5.4/tests/test_historic_ag.py` & `agspiel-python-api-0.5.5/tests/test_historic_ag.py`

 * *Files identical despite different names*

### Comparing `agspiel-python-api-0.5.4/tests/test_markt.py` & `agspiel-python-api-0.5.5/tests/test_markt.py`

 * *Files identical despite different names*

