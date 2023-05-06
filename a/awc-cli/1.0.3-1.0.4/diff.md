# Comparing `tmp/awc_cli-1.0.3-py2.py3-none-any.whl.zip` & `tmp/awc_cli-1.0.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21827 bytes, number of entries: 18
--rw-r--r--  2.0 unx      122 b- defN 23-Apr-29 18:40 awc_cli/__init__.py
+Zip file size: 22074 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      122 b- defN 23-May-06 23:26 awc_cli/__init__.py
 -rw-r--r--  2.0 unx      508 b- defN 23-Apr-15 23:24 awc_cli/__main__.py
 -rw-r--r--  2.0 unx      423 b- defN 23-Apr-15 23:09 awc_cli/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 17:08 awc_cli/py.typed
 -rw-r--r--  2.0 unx     2799 b- defN 23-Apr-29 18:40 awc_cli/repl.py
 -rw-r--r--  2.0 unx     1790 b- defN 23-Apr-15 23:14 awc_cli/util.py
 -rw-r--r--  2.0 unx      490 b- defN 23-Apr-15 21:10 awc_cli/cmd/__init__.py
--rw-r--r--  2.0 unx     4004 b- defN 23-Apr-16 00:42 awc_cli/cmd/admin_cmds.py
+-rw-r--r--  2.0 unx     4811 b- defN 23-May-06 23:23 awc_cli/cmd/admin_cmds.py
 -rw-r--r--  2.0 unx      290 b- defN 23-Apr-15 23:23 awc_cli/cmd/cmds.py
 -rw-r--r--  2.0 unx     3326 b- defN 23-Apr-15 23:23 awc_cli/cmd/mgr.py
--rw-r--r--  2.0 unx     2335 b- defN 23-Apr-15 23:15 awc_cli/cmd/user_cmds.py
--rw-------  2.0 unx    35115 b- defN 23-Apr-29 18:41 awc_cli-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1092 b- defN 23-Apr-29 18:41 awc_cli-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-29 18:41 awc_cli-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Apr-29 18:41 awc_cli-1.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-29 18:41 awc_cli-1.0.3.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-15 23:07 awc_cli-1.0.3.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1397 b- defN 23-Apr-29 18:41 awc_cli-1.0.3.dist-info/RECORD
-18 files, 53856 bytes uncompressed, 19555 bytes compressed:  63.7%
+-rw-r--r--  2.0 unx     2573 b- defN 23-May-06 23:28 awc_cli/cmd/user_cmds.py
+-rw-------  2.0 unx    35115 b- defN 23-May-06 23:30 awc_cli-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1271 b- defN 23-May-06 23:30 awc_cli-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-06 23:30 awc_cli-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-May-06 23:30 awc_cli-1.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-06 23:30 awc_cli-1.0.4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-15 23:07 awc_cli-1.0.4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1397 b- defN 23-May-06 23:30 awc_cli-1.0.4.dist-info/RECORD
+18 files, 55080 bytes uncompressed, 19802 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -27,29 +27,29 @@
 
 Filename: awc_cli/cmd/mgr.py
 Comment: 
 
 Filename: awc_cli/cmd/user_cmds.py
 Comment: 
 
-Filename: awc_cli-1.0.3.dist-info/LICENSE
+Filename: awc_cli-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: awc_cli-1.0.3.dist-info/METADATA
+Filename: awc_cli-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: awc_cli-1.0.3.dist-info/WHEEL
+Filename: awc_cli-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: awc_cli-1.0.3.dist-info/entry_points.txt
+Filename: awc_cli-1.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: awc_cli-1.0.3.dist-info/top_level.txt
+Filename: awc_cli-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: awc_cli-1.0.3.dist-info/zip-safe
+Filename: awc_cli-1.0.4.dist-info/zip-safe
 Comment: 
 
-Filename: awc_cli-1.0.3.dist-info/RECORD
+Filename: awc_cli-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awc_cli/__init__.py

```diff
@@ -1,7 +1,7 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """awc_cli"""
 
 from typing import Final
 
-__version__: Final[str] = "1.0.3"
+__version__: Final[str] = "1.0.4"
```

## awc_cli/cmd/admin_cmds.py

```diff
@@ -178,7 +178,47 @@
             )
         ],
     )
 
     print(f"edited #{cid}")
 
     return 0
+
+
+@ADMIN_CMDS.new
+def getanon(api: awc.Awc, *_: typing.Any) -> int:
+    """get anonymous messages
+    usage : getanon"""
+
+    for row in awc.api.sql(api, awc.sql.sql(awc.sql.AnonMsg.all()))[0]:
+        print(
+            f"""id : {row[0]}
+content : {row[1]}
+"""
+        )
+
+    return 0
+
+
+@ADMIN_CMDS.new
+@ADMIN_CMDS.nonempty
+def delanon(api: awc.Awc, cmd: Command) -> int:
+    """delete anonymous message
+    usage : delanon <id>"""
+
+    try:
+        cid: int = int(cmd.next() or "")
+    except ValueError:
+        return err("not a valid content ID")
+
+    awc.api.sql(
+        api,
+        awc.sql.sql(
+            awc.sql.delete(
+                awc.sql.AnonMsg.query(awc.sql.AnonMsg.cid == cid)  # type: ignore
+            )
+        ),
+    )
+
+    print(f"deleted anonymous message #{cid}")
+
+    return 0
```

## awc_cli/cmd/user_cmds.py

```diff
@@ -102,7 +102,17 @@
 @USER_CMDS.new
 def apikey(api: awc.Awc, cmd: Command) -> int:
     """set the api key ( or unset it )
     usage : apikey [api key]"""
 
     api.api_key = cmd.cmd or None
     return 0
+
+
+@USER_CMDS.new
+@USER_CMDS.nonempty
+def anon(api: awc.Awc, cmd: Command) -> int:
+    """post an anonymous message
+    usage : anon <message>"""
+
+    print("posted anonymous message with id", awc.api.anon(api, cmd.cmd).text)
+    return 0
```

## Comparing `awc_cli-1.0.3.dist-info/LICENSE` & `awc_cli-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awc_cli-1.0.3.dist-info/METADATA` & `awc_cli-1.0.4.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awc-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: cli for https://server.ari-web.xyz/
 Home-page: https://ari-web.xyz/gh/awc-cli
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,comments,api,https,awc
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,13 +18,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: awc (>=1.2.4)
+Requires-Dist: awc (>=1.3.0)
 Requires-Dist: sqlparse
 
 # awc-cli
 
 > cli for https://server.ari-web.xyz/ using https://ari-web.xyz/gh/awc
+
+# configuration
+
+config is done through environement variables :
+
+-   `INSTANCE` -- the server instance
+-   `KEY` -- the server instance key
+-   `ADMIN_CLR` -- admin ANSI colour
```

## Comparing `awc_cli-1.0.3.dist-info/RECORD` & `awc_cli-1.0.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-awc_cli/__init__.py,sha256=EFfETku-Xl2gUIrozi9FooRnx9-4fqxw-1vyPvoxx74,122
+awc_cli/__init__.py,sha256=uYTrCYRxI3zhirwxPnn6eF5MEfmy5COl9K4xSp69jKc,122
 awc_cli/__main__.py,sha256=4yHZMkIHuTIIDs61cc1graPrMLDf52djTpUrIydnBHI,508
 awc_cli/config.py,sha256=LOb3rgb14ui92pGUmnk63JEiOoTO3VOxF9xFtvzN-Ic,423
 awc_cli/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awc_cli/repl.py,sha256=PXZZfqVa9x9Y6DTkIcPNqm1cKAWVQA34JMeu99LntP8,2799
 awc_cli/util.py,sha256=vxJ0DwU9Bwk87H4MfgBg7rkhMWd-aO_xskib4Uxq7To,1790
 awc_cli/cmd/__init__.py,sha256=jwBEdqk3lhwYnMuhY8Srkoo__3FYKd3q9DEv8BpEmeA,490
-awc_cli/cmd/admin_cmds.py,sha256=3QifXHPwg0aU_ynpyL2w-0gxpm3EchP4aVjXGx8QH9k,4004
+awc_cli/cmd/admin_cmds.py,sha256=Ybut8rj4hrpOvF4d4Mc1di6HGeTywOtEGAyxiS3VuOs,4811
 awc_cli/cmd/cmds.py,sha256=dn2mhqcABK0qrdvNNz5PRQ9F5wNXW52nia2Ju6_n9Cw,290
 awc_cli/cmd/mgr.py,sha256=FUA5hl2UqKqoR6bKYwZCJTRg6_9163Lh3n17Rol2w7E,3326
-awc_cli/cmd/user_cmds.py,sha256=iytxNKB7aui4diTDybPnVUWF4ygltr2clqePR2K8v8A,2335
-awc_cli-1.0.3.dist-info/LICENSE,sha256=oo1Q3PR860k723dU4IFQHEp-dmJy49c3F_OdbhlHj88,35115
-awc_cli-1.0.3.dist-info/METADATA,sha256=WIa_q0qlJW4bSGqO2lzs71eqjvRdxqXkexMCym_80sE,1092
-awc_cli-1.0.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-awc_cli-1.0.3.dist-info/entry_points.txt,sha256=Bpjz7jmU8iLTFkxixEbvx_03RogoHocK_zDoVsGR8R0,46
-awc_cli-1.0.3.dist-info/top_level.txt,sha256=4NIrO2nFlQFYzCa0gD1_twziYc8me452Za3vtcFWans,8
-awc_cli-1.0.3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-awc_cli-1.0.3.dist-info/RECORD,,
+awc_cli/cmd/user_cmds.py,sha256=c984BNFP_a8vUuyP8ic4oaLk7tegXP8Hp8JKtmMIauI,2573
+awc_cli-1.0.4.dist-info/LICENSE,sha256=oo1Q3PR860k723dU4IFQHEp-dmJy49c3F_OdbhlHj88,35115
+awc_cli-1.0.4.dist-info/METADATA,sha256=lAWCpHNtF4ZB4y7hoxkAOI-RDV7_iwbe2QwXRmuDIq8,1271
+awc_cli-1.0.4.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+awc_cli-1.0.4.dist-info/entry_points.txt,sha256=Bpjz7jmU8iLTFkxixEbvx_03RogoHocK_zDoVsGR8R0,46
+awc_cli-1.0.4.dist-info/top_level.txt,sha256=4NIrO2nFlQFYzCa0gD1_twziYc8me452Za3vtcFWans,8
+awc_cli-1.0.4.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+awc_cli-1.0.4.dist-info/RECORD,,
```

