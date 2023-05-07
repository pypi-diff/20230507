# Comparing `tmp/django_tsp-3.14.1-py3-none-any.whl.zip` & `tmp/django_tsp-3.14.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,17 @@
-Zip file size: 4457 bytes, number of entries: 11
+Zip file size: 6219 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-09 10:17 django_tsp/__init__.py
+-rw-r--r--  2.0 unx     1766 b- defN 23-May-07 17:51 django_tsp/apis.py
 -rw-r--r--  2.0 unx      429 b- defN 23-Apr-28 14:31 django_tsp/apps.py
--rw-r--r--  2.0 unx     1179 b- defN 23-Apr-28 13:38 django_tsp/checks.py
--rw-r--r--  2.0 unx      446 b- defN 23-Apr-28 13:36 django_tsp/conf.py
--rw-r--r--  2.0 unx      137 b- defN 23-Apr-28 13:30 django_tsp/defaults.py
--rw-r--r--  2.0 unx      328 b- defN 23-Apr-28 13:37 django_tsp/utils.py
--rw-r--r--  2.0 unx     1078 b- defN 23-Apr-28 14:35 django_tsp-3.14.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1492 b- defN 23-Apr-28 14:35 django_tsp-3.14.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 14:35 django_tsp-3.14.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-28 14:35 django_tsp-3.14.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      860 b- defN 23-Apr-28 14:35 django_tsp-3.14.1.dist-info/RECORD
-11 files, 6052 bytes uncompressed, 3003 bytes compressed:  50.4%
+-rw-r--r--  2.0 unx     1141 b- defN 23-May-07 17:51 django_tsp/checks.py
+-rw-r--r--  2.0 unx      494 b- defN 23-May-07 17:51 django_tsp/conf.py
+-rw-r--r--  2.0 unx      590 b- defN 23-May-07 17:51 django_tsp/consumer.py
+-rw-r--r--  2.0 unx      132 b- defN 23-May-07 17:51 django_tsp/routing.py
+-rw-r--r--  2.0 unx      212 b- defN 23-May-07 17:51 django_tsp/serializers.py
+-rw-r--r--  2.0 unx      648 b- defN 23-May-07 17:51 django_tsp/services.py
+-rw-r--r--  2.0 unx      102 b- defN 23-May-07 17:51 django_tsp/views.py
+-rw-r--r--  2.0 unx     1078 b- defN 23-May-07 17:52 django_tsp-3.14.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1492 b- defN 23-May-07 17:52 django_tsp-3.14.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-07 17:52 django_tsp-3.14.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-07 17:52 django_tsp-3.14.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1171 b- defN 23-May-07 17:52 django_tsp-3.14.2.dist-info/RECORD
+15 files, 9358 bytes uncompressed, 4289 bytes compressed:  54.2%
```

## zipnote {}

```diff
@@ -1,34 +1,46 @@
 Filename: django_tsp/__init__.py
 Comment: 
 
+Filename: django_tsp/apis.py
+Comment: 
+
 Filename: django_tsp/apps.py
 Comment: 
 
 Filename: django_tsp/checks.py
 Comment: 
 
 Filename: django_tsp/conf.py
 Comment: 
 
-Filename: django_tsp/defaults.py
+Filename: django_tsp/consumer.py
+Comment: 
+
+Filename: django_tsp/routing.py
+Comment: 
+
+Filename: django_tsp/serializers.py
+Comment: 
+
+Filename: django_tsp/services.py
 Comment: 
 
-Filename: django_tsp/utils.py
+Filename: django_tsp/views.py
 Comment: 
 
-Filename: django_tsp-3.14.1.dist-info/LICENSE
+Filename: django_tsp-3.14.2.dist-info/LICENSE
 Comment: 
 
-Filename: django_tsp-3.14.1.dist-info/METADATA
+Filename: django_tsp-3.14.2.dist-info/METADATA
 Comment: 
 
-Filename: django_tsp-3.14.1.dist-info/WHEEL
+Filename: django_tsp-3.14.2.dist-info/WHEEL
 Comment: 
 
-Filename: django_tsp-3.14.1.dist-info/top_level.txt
+Filename: django_tsp-3.14.2.dist-info/top_level.txt
 Comment: 
 
-Filename: django_tsp-3.14.1.dist-info/RECORD
+Filename: django_tsp-3.14.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_tsp/checks.py

```diff
@@ -7,32 +7,30 @@
 
 from django_tsp.conf import conf
 
 
 def check_settings(**kwargs: Any) -> list[CheckMessage]:
     errors: list[CheckMessage] = []
 
-    if not is_sequence(conf.NAME_LIST, str):
+    if not isinstance(conf.TSP_BROKER_URL, str):
         errors.append(
-            Error(
-                "NAME_LIST should be a sequence of strings.",
-                id="django_tsp.E001",
-            )
+            Error("TSP_BROKER_URL should be a string.", id="django_tsp.E009")
         )
 
-    if not isinstance(conf.COMPANY_NAME, str):
+    if not isinstance(conf.TSP_HOOK_URL, str):
         errors.append(
-            Error("COMPANY_NAME should be a string.", id="django_tsp.E009")
+            Error("TSP_HOOK_URL should be a string.", id="django_tsp.E009")
         )
 
-    if hasattr(settings, "REQ_NAME"):
+
+    if not hasattr(settings, "TSP_HOOK_URL"):
         errors.append(
             Error(
                 (
-                    "The REQ_NAME setting has been removed"
+                    "The TSP_HOOK_URL setting has been removed"
                     + " - see django_tsp' CHANGELOG."
                 ),
                 id="django_tsp.E013",
             )
         )
 
     return errors
```

## django_tsp/conf.py

```diff
@@ -1,18 +1,18 @@
 from django.conf import settings
 from typing import Sequence
 from django_tsp.defaults import default_names
-
+from tsp_wrapper import BROKER_URL
 
 class Settings:
     """
     Shadow Django's settings with a little logic
     """
     @property
-    def NAME_LIST(self) -> Sequence[str]:
-        return getattr(settings, "NAME_LIST", default_names)
+    def TSP_BROKER_URL(self) -> str:
+        return getattr(settings, "TSP_BROKER_URL", BROKER_URL)
 
     @property
-    def COMPANY_NAME(self) -> str:
-        return getattr(settings, "CORS_PREFLIGHT_MAX_AGE", "CoolBlue")
+    def TSP_HOOK_URL(self) -> str:
+        return getattr(settings, "TSP_HOOK_URL", "http://localhost:8000/api/tsp/hook/")
 
 conf = Settings()
```

## Comparing `django_tsp-3.14.1.dist-info/LICENSE` & `django_tsp-3.14.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_tsp-3.14.1.dist-info/METADATA` & `django_tsp-3.14.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tsp
-Version: 3.14.1
+Version: 3.14.2
 Summary: django-tsp is a django travel salesman problem.
 Home-page: https://github.com/TravelSalesmanProblem/django_tsp
 Author: AmirBahador Bahadori
 Author-email: amirbahador.pv@gmail.com
 Maintainer: AmirBahador Bahadori
 Maintainer-email: amirbahador.pv@gmail.com
 License: MIT
```

## Comparing `django_tsp-3.14.1.dist-info/RECORD` & `django_tsp-3.14.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 django_tsp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+django_tsp/apis.py,sha256=YbCOyQTaGpEZ8_TaTMdHxP1tSyodcaq85TydLi5DDpY,1766
 django_tsp/apps.py,sha256=atpRGfJjp09ZsdPUSrx4lFFvrGyO3zRC_WNm23HEEu8,429
-django_tsp/checks.py,sha256=_YnWdSqB-dUCGxQXGBM-B2SZqGEZW-vSYpdE6HseZe4,1179
-django_tsp/conf.py,sha256=KH0iQSUV_z1Jrj9SNRE8AHbZ52ETf1AiYCVO7ImPUGQ,446
-django_tsp/defaults.py,sha256=YuOuYh5lYLPfVasM1qEXXpZRaQO-i5XDNJnai2XZ1PE,137
-django_tsp/utils.py,sha256=bRYIC0JwnDfmDu0K2GzCijzwVfIEE1cgSG9oQo4b-r8,328
-django_tsp-3.14.1.dist-info/LICENSE,sha256=OlcFwcrl0vK6seF27WoEsrMyD4iee-HclD2eH3Y6ncw,1078
-django_tsp-3.14.1.dist-info/METADATA,sha256=1vaGnScjwJ9D27pzAkiT2TcxClWwoBZZL_6nLoz0yf0,1492
-django_tsp-3.14.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-django_tsp-3.14.1.dist-info/top_level.txt,sha256=SccQRSWrs0c7FKxZlap4DQ9HZMk1h3wbDMgGxDRreBs,11
-django_tsp-3.14.1.dist-info/RECORD,,
+django_tsp/checks.py,sha256=kpUsVhiXj_pMS1LfZaQyGAP4fFOtc6RgC_dI7voFME0,1141
+django_tsp/conf.py,sha256=HJvqoN1TwYz4ib4EsSA7HCph4AIOBQXAUW8pYxgu3tw,494
+django_tsp/consumer.py,sha256=UOdhqTzGN-2ziNdS5IIp3S4pRUccYApRCoAZzC6DWvY,590
+django_tsp/routing.py,sha256=i7HdR5oBMSw0TlHsfuYK6QSqHVmIFEv19myJGNGKe5I,132
+django_tsp/serializers.py,sha256=Wm2KtSRluB7VmnWRAocG8ZAuZwVqe1d0pVg3EOtp6tA,212
+django_tsp/services.py,sha256=1v7XydFXJmE6VWBy56dh5vgZv__sGKO_WUo_fPikdHI,648
+django_tsp/views.py,sha256=gvTbnLWevATVfUn78eCXjHEQwKTXfWTkFQ3PYOmi5Cg,102
+django_tsp-3.14.2.dist-info/LICENSE,sha256=OlcFwcrl0vK6seF27WoEsrMyD4iee-HclD2eH3Y6ncw,1078
+django_tsp-3.14.2.dist-info/METADATA,sha256=F54yYBHpOOXuXX4qJM6K9kRF0XzF1D5Gw2xeAPx6984,1492
+django_tsp-3.14.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+django_tsp-3.14.2.dist-info/top_level.txt,sha256=SccQRSWrs0c7FKxZlap4DQ9HZMk1h3wbDMgGxDRreBs,11
+django_tsp-3.14.2.dist-info/RECORD,,
```

