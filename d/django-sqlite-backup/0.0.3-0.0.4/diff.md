# Comparing `tmp/django_sqlite_backup-0.0.3-py3-none-any.whl.zip` & `tmp/django_sqlite_backup-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,14 @@
-Zip file size: 7406 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-May-06 10:15 django_sqlite_backup/__init__.py
--rw-r--r--  2.0 unx      450 b- defN 23-May-06 10:15 django_sqlite_backup/apps.py
--rw-r--r--  2.0 unx     1537 b- defN 23-May-06 10:15 django_sqlite_backup/aws.py
--rw-r--r--  2.0 unx      779 b- defN 23-May-06 10:15 django_sqlite_backup/backup.py
--rw-r--r--  2.0 unx      496 b- defN 23-May-06 10:15 django_sqlite_backup/decorators.py
--rw-r--r--  2.0 unx      740 b- defN 23-May-06 10:15 django_sqlite_backup/restore.py
--rw-r--r--  2.0 unx      150 b- defN 23-May-06 10:15 django_sqlite_backup/urls.py
--rw-r--r--  2.0 unx      403 b- defN 23-May-06 10:15 django_sqlite_backup/views.py
--rw-r--r--  2.0 unx     1070 b- defN 23-May-06 10:15 django_sqlite_backup-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4621 b- defN 23-May-06 10:15 django_sqlite_backup-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-06 10:15 django_sqlite_backup-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-May-06 10:15 django_sqlite_backup-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1137 b- defN 23-May-06 10:15 django_sqlite_backup-0.0.3.dist-info/RECORD
-13 files, 11496 bytes uncompressed, 5470 bytes compressed:  52.4%
+Zip file size: 7057 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-May-07 17:07 django_sqlite_backup/__init__.py
+-rw-r--r--  2.0 unx      450 b- defN 23-May-07 17:07 django_sqlite_backup/apps.py
+-rw-r--r--  2.0 unx     1535 b- defN 23-May-07 17:07 django_sqlite_backup/aws.py
+-rw-r--r--  2.0 unx      779 b- defN 23-May-07 17:07 django_sqlite_backup/backup.py
+-rw-r--r--  2.0 unx      740 b- defN 23-May-07 17:07 django_sqlite_backup/restore.py
+-rw-r--r--  2.0 unx      150 b- defN 23-May-07 17:07 django_sqlite_backup/urls.py
+-rw-r--r--  2.0 unx      234 b- defN 23-May-07 17:07 django_sqlite_backup/views.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-07 17:07 django_sqlite_backup-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4939 b- defN 23-May-07 17:07 django_sqlite_backup-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-07 17:07 django_sqlite_backup-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-07 17:07 django_sqlite_backup-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1047 b- defN 23-May-07 17:07 django_sqlite_backup-0.0.4.dist-info/RECORD
+12 files, 11057 bytes uncompressed, 5265 bytes compressed:  52.4%
```

## zipnote {}

```diff
@@ -6,35 +6,32 @@
 
 Filename: django_sqlite_backup/aws.py
 Comment: 
 
 Filename: django_sqlite_backup/backup.py
 Comment: 
 
-Filename: django_sqlite_backup/decorators.py
-Comment: 
-
 Filename: django_sqlite_backup/restore.py
 Comment: 
 
 Filename: django_sqlite_backup/urls.py
 Comment: 
 
 Filename: django_sqlite_backup/views.py
 Comment: 
 
-Filename: django_sqlite_backup-0.0.3.dist-info/LICENSE
+Filename: django_sqlite_backup-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: django_sqlite_backup-0.0.3.dist-info/METADATA
+Filename: django_sqlite_backup-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: django_sqlite_backup-0.0.3.dist-info/WHEEL
+Filename: django_sqlite_backup-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: django_sqlite_backup-0.0.3.dist-info/top_level.txt
+Filename: django_sqlite_backup-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: django_sqlite_backup-0.0.3.dist-info/RECORD
+Filename: django_sqlite_backup-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_sqlite_backup/aws.py

```diff
@@ -17,15 +17,15 @@
 
 def get_database_name() -> str:
     return str(settings.DATABASES["default"]["NAME"])
 
 
 class AwsSqliteBackup:
     def _read_db(self) -> Any:
-        with open(get_database_name()) as f:
+        with open(get_database_name(), "rb") as f:
             return f.read()
 
     def backup_db(self) -> None:
         bucket_name = settings.SQLITE_BACKUP.get("BUCKET_NAME")
         db_name = get_database_name().split("/")[-1]
 
         if bucket_name is None:
@@ -51,9 +51,9 @@
         key = f"sqlite_backup/{date_str}/{db_name}"
 
         response = s3().get_object(
             Bucket=bucket_name,
             Key=key,
         )
 
-        with open(db_name, "w") as f:
-            f.write(response.get("Body").read().decode())
+        with open(db_name, "wb") as f:
+            f.write(response.get("Body").read())
```

## django_sqlite_backup/views.py

```diff
@@ -1,13 +1,9 @@
 from django.http import HttpRequest
 from django.http import JsonResponse
-from django.views.decorators.http import require_http_methods
 
 from django_sqlite_backup import backup
-from django_sqlite_backup.decorators import login_required
 
 
-@login_required
-@require_http_methods(["POST"])
 def backup_view(request: HttpRequest) -> JsonResponse:
     backup.do_backup()
     return JsonResponse({}, status=204)
```

## Comparing `django_sqlite_backup-0.0.3.dist-info/LICENSE` & `django_sqlite_backup-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_sqlite_backup-0.0.3.dist-info/METADATA` & `django_sqlite_backup-0.0.4.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sqlite-backup
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Django app to easily backup your sqlite database through an endpoint.
 Author-email: Ferran Jovell <ferran.jovell+gh@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ferran Jovell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -81,29 +81,50 @@
 
 ```
     path("", include("django_sqlite_backup.urls")),
 ```
 
 This will create a route in your application to backup your sqlite database:
 
-`/backup/` which accepts only `POST` requests with authentication.
+```
+GET /backup/
+
+204: Successful backup
+```
+
+### Write your own view
+
+If you want to use a different method or want to add some sort of authentication or other kinds of logic with the backup call, you can write your own view importing the `do_backup` function:
+
+```
+# views.py
+from django.http import HttpRequest
+from django.http import JsonResponse
+
+from django_sqlite_backup import backup
+
 
-If the request succeeds it will return a `294`. Otherwise, a `403` if the request was not authenticated.
+def my_view(request: HttpRequest) -> JsonResponse:
+    do_backup()
+    return JsonResponse({}, status=204)
+```
 
 ### Settings
 
 You must define your settings in your `settings.py`:
 
 ```
+
 SQLITE_BACKUP = {
-    "BACKUP_CLASS": ...,
-    "RESTORE_CLASS": ...,
-    "BUCKET_NAME": ...,
-    "S3_ENDPOINT": ...,
+"BACKUP_CLASS": ...,
+"RESTORE_CLASS": ...,
+"BUCKET_NAME": ...,
+"S3_ENDPOINT": ...,
 }
+
 ```
 
 - `BACKUP_CLASS` must point to class which follows the [`SqliteBackup`](./django_sqlite_backup/backup.py) protocol.
 - `RESTORE_CLASS` must point to class which follows the [`SqliteRestore`](./django_sqlite_backup/restore.py) protocol.
 - `BUCKET_NAME` is the name of the bucket in S3 which can be written to.
 - `S3_ENDPOINT` S3 endpoint override. Leave this blank if you use AWS S3 directly.
```

## Comparing `django_sqlite_backup-0.0.3.dist-info/RECORD` & `django_sqlite_backup-0.0.4.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 django_sqlite_backup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_sqlite_backup/apps.py,sha256=hr_VWttIN8RVXzXXG2Vo-SjuNgCFDE5POwycNww-ixo,450
-django_sqlite_backup/aws.py,sha256=NvjSpndNvCTPAILKuH1EyZ5rZgPmsN5Oi8btC7gqSWM,1537
+django_sqlite_backup/aws.py,sha256=tpyJpF46JxUvR6PpThUgl_iWRnEj-Su4BacfpyjqrUo,1535
 django_sqlite_backup/backup.py,sha256=8-4QRYIWJOMYM0Deuub6P5nWiBKjW4w2Gvh-UjttcNg,779
-django_sqlite_backup/decorators.py,sha256=bXvyTazsw0xkkOJ3zNtt8tOv1GmXsmB1lbUMnzW9Mbg,496
 django_sqlite_backup/restore.py,sha256=BJTGqd0zqeTWRbk1c98OqNRweYNmOoDdUC1dsuCkKWc,740
 django_sqlite_backup/urls.py,sha256=ve4fRC0VSPi235hDc9_n973ii_jrIpeE4tPrJTBSNCA,150
-django_sqlite_backup/views.py,sha256=9evoRFbHv4dFHhMD0ntXQH4VyDfWFKNGTFUdTfoIK1Y,403
-django_sqlite_backup-0.0.3.dist-info/LICENSE,sha256=bwE4PTk0_zgY2rrrldsrBocfua-bkc_IUxH1pr1rCFA,1070
-django_sqlite_backup-0.0.3.dist-info/METADATA,sha256=hzdU3A3kYGC40s2jbhF2aSWHM8b1A6IwtJsuLQbKsNs,4621
-django_sqlite_backup-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-django_sqlite_backup-0.0.3.dist-info/top_level.txt,sha256=hpNLepZbcHqSqEC92LAtpsd7uaey2g64SD0C0NWEDqM,21
-django_sqlite_backup-0.0.3.dist-info/RECORD,,
+django_sqlite_backup/views.py,sha256=1UKV4iRhvdTub5WKT3KUh0CefYIh9QgOMo3N4Dik3DE,234
+django_sqlite_backup-0.0.4.dist-info/LICENSE,sha256=bwE4PTk0_zgY2rrrldsrBocfua-bkc_IUxH1pr1rCFA,1070
+django_sqlite_backup-0.0.4.dist-info/METADATA,sha256=8SogZWZjYS3EY1XJP2MGu4eIkq-1Gs7F0OE6w8sFLVg,4939
+django_sqlite_backup-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+django_sqlite_backup-0.0.4.dist-info/top_level.txt,sha256=hpNLepZbcHqSqEC92LAtpsd7uaey2g64SD0C0NWEDqM,21
+django_sqlite_backup-0.0.4.dist-info/RECORD,,
```

