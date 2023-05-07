# Comparing `tmp/audit_flask-0.24-py3-none-any.whl.zip` & `tmp/audit_flask-0.25-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 7478 bytes, number of entries: 18
+Zip file size: 7503 bytes, number of entries: 18
 -rw-r--r--  2.0 unx       49 b- defN 23-May-07 16:32 audit_flask/__init__.py
 -rw-r--r--  2.0 unx      489 b- defN 23-May-07 17:11 audit_flask/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-07 16:39 audit_flask/main.py
 -rw-r--r--  2.0 unx       79 b- defN 23-May-07 17:10 audit_flask/audit/__init__.py
 -rw-r--r--  2.0 unx      233 b- defN 23-May-07 17:20 audit_flask/audit/kwargs.py
 -rw-r--r--  2.0 unx     2167 b- defN 23-May-07 17:21 audit_flask/audit/mongoengine.py
--rw-r--r--  2.0 unx     1787 b- defN 23-May-07 17:21 audit_flask/audit/sqlalchemy.py
+-rw-r--r--  2.0 unx     1899 b- defN 23-May-07 19:19 audit_flask/audit/sqlalchemy.py
 -rw-r--r--  2.0 unx        1 b- defN 23-May-07 17:19 audit_flask/utils/__init__.py
 -rw-r--r--  2.0 unx      788 b- defN 23-May-07 17:35 audit_flask/utils/flask.py
 -rw-r--r--  2.0 unx      558 b- defN 23-May-07 17:13 audit_flask/utils/json.py
 -rw-r--r--  2.0 unx       45 b- defN 23-May-07 16:58 test/__init__.py
 -rw-r--r--  2.0 unx      217 b- defN 23-May-07 17:00 test/config.py
 -rw-r--r--  2.0 unx     1433 b- defN 23-May-07 17:23 test/test_mongoengine.py
 -rw-r--r--  2.0 unx     1990 b- defN 23-May-07 17:10 test/test_sqlalchemy.py
--rw-r--r--  2.0 unx      394 b- defN 23-May-07 17:58 audit_flask-0.24.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-07 17:58 audit_flask-0.24.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-07 17:58 audit_flask-0.24.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1429 b- defN 23-May-07 17:58 audit_flask-0.24.dist-info/RECORD
-18 files, 11768 bytes uncompressed, 5130 bytes compressed:  56.4%
+-rw-r--r--  2.0 unx      394 b- defN 23-May-07 19:21 audit_flask-0.25.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-07 19:21 audit_flask-0.25.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-07 19:21 audit_flask-0.25.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1429 b- defN 23-May-07 19:21 audit_flask-0.25.dist-info/RECORD
+18 files, 11880 bytes uncompressed, 5155 bytes compressed:  56.6%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: test/test_mongoengine.py
 Comment: 
 
 Filename: test/test_sqlalchemy.py
 Comment: 
 
-Filename: audit_flask-0.24.dist-info/METADATA
+Filename: audit_flask-0.25.dist-info/METADATA
 Comment: 
 
-Filename: audit_flask-0.24.dist-info/WHEEL
+Filename: audit_flask-0.25.dist-info/WHEEL
 Comment: 
 
-Filename: audit_flask-0.24.dist-info/top_level.txt
+Filename: audit_flask-0.25.dist-info/top_level.txt
 Comment: 
 
-Filename: audit_flask-0.24.dist-info/RECORD
+Filename: audit_flask-0.25.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## audit_flask/audit/sqlalchemy.py

```diff
@@ -20,15 +20,18 @@
         state = inspect(target)
         changes = {}
         object_before_changed = {}
 
         for attr in state.attrs:
             hist = attr.load_history()
             hist_attr = hist.deleted or hist.unchanged
-            object_before_changed[attr.key] = hist_attr[0]
+            if len(hist_attr) > 0:
+                object_before_changed[attr.key] = hist_attr[0]
+            else:
+                object_before_changed[attr.key] = None
             if not hist.has_changes():
                 continue
             changes[attr.key] = hist.added
         __audit((cls, target), 'update', changes, object_before_changed)
 
     @event.listens_for(cls, 'after_delete')
     def after_delete(mapper, connection, target):
```

## Comparing `audit_flask-0.24.dist-info/RECORD` & `audit_flask-0.25.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 audit_flask/__init__.py,sha256=gXThpjrk5OnqdQRuSRD0l3DyOn66eEuF0kQPePaF4sQ,49
 audit_flask/config.py,sha256=94KYLsr8p--fTi-Egm_8cRpJMtytFybHEmcS_-wIeqw,489
 audit_flask/main.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 audit_flask/audit/__init__.py,sha256=aNCr6aPAmOKm1hASiH-qnAG8726WKHYmXamTRkp3mDY,79
 audit_flask/audit/kwargs.py,sha256=Lv_5vafyyi-zDkvfEv-bsY7hWPejNJIz24drsTHhQj8,233
 audit_flask/audit/mongoengine.py,sha256=8H-CRe22WezP-WnlnZuE0aNl88WeXVwk8WfRXsM5mng,2167
-audit_flask/audit/sqlalchemy.py,sha256=MG8mGWRwb-ufaGB23pM-eBvLtVWSqGR-lPHGSYta_JQ,1787
+audit_flask/audit/sqlalchemy.py,sha256=dgbQHBHpslX45FIr_UKT00GzwFFz305wr2j3XwpTevo,1899
 audit_flask/utils/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 audit_flask/utils/flask.py,sha256=VMFKl0Cj9x06KnYU_owteST7qcYF8nWJGCKSrXNqkWQ,788
 audit_flask/utils/json.py,sha256=DX2KiAD4xI5FKxA15SXaagaFTzil8uqwkwMcVgavwRw,558
 test/__init__.py,sha256=rietiseBKDBp2H2-xOZviKdWmnacQnEqzQQ0Y6Ej8CY,45
 test/config.py,sha256=vP45_qCTy55AjqPx_M-o6qZBRHq2QcST1bDghZwPxXI,217
 test/test_mongoengine.py,sha256=72Yz5OfX7zDuFZucuTW2xmvt5yGf1w7GNtRV_3dIWw4,1433
 test/test_sqlalchemy.py,sha256=OGMkHKbqgv8BBtNbSOh-Jey77ljxKkOF2S9zlZM98-A,1990
-audit_flask-0.24.dist-info/METADATA,sha256=-AoihEKZX7JRdTFr233OJnfZAubs1ARZZve7gMXzvG8,394
-audit_flask-0.24.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-audit_flask-0.24.dist-info/top_level.txt,sha256=vnGYiKEEfaT1zXkdI7u5w5e93ymHk2o0gj35p8UKU8Q,17
-audit_flask-0.24.dist-info/RECORD,,
+audit_flask-0.25.dist-info/METADATA,sha256=xlDwvyRwHIytGY89WNILDoIF7QvOkpib9-XraLVstC0,394
+audit_flask-0.25.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+audit_flask-0.25.dist-info/top_level.txt,sha256=vnGYiKEEfaT1zXkdI7u5w5e93ymHk2o0gj35p8UKU8Q,17
+audit_flask-0.25.dist-info/RECORD,,
```

