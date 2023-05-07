# Comparing `tmp/custodes-0.0.8.tar.gz` & `tmp/custodes-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodes-0.0.8.tar", max compression
+gzip compressed data, was "custodes-0.0.9.tar", max compression
```

## Comparing `custodes-0.0.8.tar` & `custodes-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      472 2023-05-05 04:33:11.034987 custodes-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-05-04 13:19:56.214387 custodes-0.0.8/custodes/__init__.py
--rw-r--r--   0        0        0      893 2023-05-05 03:02:32.934998 custodes-0.0.8/custodes/auth.py
--rw-r--r--   0        0        0     2910 2023-05-05 12:41:23.798709 custodes-0.0.8/custodes/client.py
--rw-r--r--   0        0        0       16 2023-05-04 16:18:32.000000 custodes-0.0.8/custodes/config.py
--rw-r--r--   0        0        0     2000 2023-05-05 04:38:59.117136 custodes-0.0.8/custodes/server.py
--rw-r--r--   0        0        0      375 2023-05-05 12:51:19.345723 custodes-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 custodes-0.0.8/setup.py
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 custodes-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      472 2023-05-05 04:33:11.000000 custodes-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 13:19:56.000000 custodes-0.0.9/custodes/__init__.py
+-rw-r--r--   0        0        0      893 2023-05-05 03:02:32.000000 custodes-0.0.9/custodes/auth.py
+-rw-r--r--   0        0        0     3189 2023-05-05 14:41:39.967443 custodes-0.0.9/custodes/client.py
+-rw-r--r--   0        0        0       16 2023-05-04 16:18:32.541207 custodes-0.0.9/custodes/config.py
+-rw-r--r--   0        0        0     2000 2023-05-05 04:38:59.000000 custodes-0.0.9/custodes/server.py
+-rw-r--r--   0        0        0      375 2023-05-05 14:43:14.832079 custodes-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1198 2023-05-05 14:43:38.996575 custodes-0.0.9/setup.py
+-rw-r--r--   0        0        0     1085 2023-05-05 14:43:38.997073 custodes-0.0.9/PKG-INFO
```

### Comparing `custodes-0.0.8/custodes/auth.py` & `custodes-0.0.9/custodes/auth.py`

 * *Files identical despite different names*

### Comparing `custodes-0.0.8/custodes/client.py` & `custodes-0.0.9/custodes/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,16 +9,25 @@
 from rich import print
 
 POSTER = '/tmp/cusposter'
 
 
 # —--------------------------------------------
 async def _parse_ip(js: Dict) -> str:
-    masked_ip = '.'.join(js['ip'].split('.')[-2:])
-    return f"{js['country']} {js['region']} {js['city']} *.*.{masked_ip}"
+    try:
+        masked_ip = '.'.join(js['ip'].split('.')[-2:])
+        return f"{js['country']} {js['region']} {js['city']} *.*.{masked_ip}"
+    except Exception as e:
+        import traceback
+        cf.error({
+            'error': 'parse ip failed',
+            'exception': str(e),
+            'traceback': traceback.format_exc(),
+        })
+        return ''
 
 
 async def init_poster():
     if not cf.io.exists(POSTER):
         async with aiohttp.ClientSession() as session:
             async with session.get(
                 cf.b64decode(
@@ -32,16 +41,18 @@
                         f.write(chunk)
     return cf.shell(f'chmod 755 {POSTER}')
 
 
 async def ipinfo() -> str:
     fp = '/tmp/ipinfo.json'
     if cf.io.exists(fp):
-        js = cf.js(fp)
-        return await _parse_ip(js)
+        ip = await _parse_ip(cf.js(fp))
+        if ip:
+            return ip
+        cf.io.rm(fp)
     else:
         async with aiohttp.ClientSession() as session:
             async with session.get(f'https://ipinfo.io/json') as resp:
                 js = await resp.json()
                 cf.js.write(js, fp)
                 return await _parse_ip(js)
```

### Comparing `custodes-0.0.8/custodes/server.py` & `custodes-0.0.9/custodes/server.py`

 * *Files identical despite different names*

### Comparing `custodes-0.0.8/setup.py` & `custodes-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,22 @@
  'codefast>=23.4.18.13,<24.0.0.0',
  'rich>=13.3.5,<14.0.0',
  'simauth==0.0.9',
  'urllib3==1.26.15']
 
 setup_kwargs = {
     'name': 'custodes',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': '',
     'long_description': "\nApp guardians.\n\n# Usage\n```python\nimport asyncio\nfrom typing import Any, Dict\n\nfrom codefast.asyncio.rabbitmq import consume\nfrom rich import print\n\nfrom custodes.server import get\nfrom custodes.client import post\n\nasync def main():\n    return await asyncio.gather(\n        post('custodes server', {'code': 0, 'message': 'OK'}, loop=True, expire=120),\n        get()\n    )\n\nif __name__ == '__main__':\n    cf.info('custodes server started...')\n    asyncio.run(main())\n\n```\n",
     'author': 'tompz',
     'author_email': 'tompz@tompz.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
+    'maintainer': None,
+    'maintainer_email': None,
+    'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `custodes-0.0.8/PKG-INFO` & `custodes-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: custodes
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: tompz
 Author-email: tompz@tompz.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aio-pika (>=9.0.5,<10.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: codefast (>=23.4.18.13,<24.0.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: simauth (==0.0.9)
 Requires-Dist: urllib3 (==1.26.15)
 Description-Content-Type: text/markdown
```

