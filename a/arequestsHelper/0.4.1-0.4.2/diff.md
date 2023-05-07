# Comparing `tmp/arequestsHelper-0.4.1.tar.gz` & `tmp/arequestsHelper-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arequestsHelper-0.4.1.tar", last modified: Mon Mar  6 18:00:55 2023, max compression
+gzip compressed data, was "arequestsHelper-0.4.2.tar", last modified: Sun May  7 16:42:22 2023, max compression
```

## Comparing `arequestsHelper-0.4.1.tar` & `arequestsHelper-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-03-06 18:00:55.248621 arequestsHelper-0.4.1/
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     1074 2022-11-13 00:46:48.000000 arequestsHelper-0.4.1/LICENSE
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      792 2023-03-06 18:00:55.248621 arequestsHelper-0.4.1/PKG-INFO
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       62 2022-11-13 01:00:48.000000 arequestsHelper-0.4.1/README.md
-drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-03-06 18:00:55.247621 arequestsHelper-0.4.1/arequestsHelper/
--rwxrwxrwx   0 kaixenix  (1000) kaixenix  (1000)       61 2022-11-14 20:03:06.000000 arequestsHelper-0.4.1/arequestsHelper/__init__.py
--rwxrwxrwx   0 kaixenix  (1000) kaixenix  (1000)     5675 2023-03-06 18:00:18.000000 arequestsHelper-0.4.1/arequestsHelper/arequestsHelper.py
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      149 2022-11-14 22:37:14.000000 arequestsHelper-0.4.1/arequestsHelper/errors.py
-drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-03-06 18:00:55.248621 arequestsHelper-0.4.1/arequestsHelper.egg-info/
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      792 2023-03-06 18:00:55.000000 arequestsHelper-0.4.1/arequestsHelper.egg-info/PKG-INFO
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      319 2023-03-06 18:00:55.000000 arequestsHelper-0.4.1/arequestsHelper.egg-info/SOURCES.txt
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)        1 2023-03-06 18:00:55.000000 arequestsHelper-0.4.1/arequestsHelper.egg-info/dependency_links.txt
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       17 2023-03-06 18:00:55.000000 arequestsHelper-0.4.1/arequestsHelper.egg-info/requires.txt
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       16 2023-03-06 18:00:55.000000 arequestsHelper-0.4.1/arequestsHelper.egg-info/top_level.txt
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       79 2023-03-06 18:00:55.249621 arequestsHelper-0.4.1/setup.cfg
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     1761 2023-03-06 17:49:54.000000 arequestsHelper-0.4.1/setup.py
+drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-07 16:42:22.803092 arequestsHelper-0.4.2/
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     1074 2023-05-07 16:38:56.000000 arequestsHelper-0.4.2/LICENSE
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      789 2023-05-07 16:42:22.803092 arequestsHelper-0.4.2/PKG-INFO
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      365 2023-05-07 16:38:56.000000 arequestsHelper-0.4.2/README.md
+drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-07 16:42:22.802092 arequestsHelper-0.4.2/arequestsHelper/
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       61 2023-05-07 16:38:56.000000 arequestsHelper-0.4.2/arequestsHelper/__init__.py
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     4578 2023-05-07 16:40:12.000000 arequestsHelper-0.4.2/arequestsHelper/arequestsHelper.py
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      149 2023-05-07 16:38:56.000000 arequestsHelper-0.4.2/arequestsHelper/errors.py
+drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-07 16:42:22.803092 arequestsHelper-0.4.2/arequestsHelper.egg-info/
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      789 2023-05-07 16:42:22.000000 arequestsHelper-0.4.2/arequestsHelper.egg-info/PKG-INFO
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      319 2023-05-07 16:42:22.000000 arequestsHelper-0.4.2/arequestsHelper.egg-info/SOURCES.txt
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)        1 2023-05-07 16:42:22.000000 arequestsHelper-0.4.2/arequestsHelper.egg-info/dependency_links.txt
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       17 2023-05-07 16:42:22.000000 arequestsHelper-0.4.2/arequestsHelper.egg-info/requires.txt
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       16 2023-05-07 16:42:22.000000 arequestsHelper-0.4.2/arequestsHelper.egg-info/top_level.txt
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       79 2023-05-07 16:42:22.803092 arequestsHelper-0.4.2/setup.cfg
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     1757 2023-05-07 16:42:06.000000 arequestsHelper-0.4.2/setup.py
```

### Comparing `arequestsHelper-0.4.1/LICENSE` & `arequestsHelper-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arequestsHelper-0.4.1/PKG-INFO` & `arequestsHelper-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: arequestsHelper
-Version: 0.4.1
+Version: 0.4.2
 Summary: This pakage helps to work with aiohttp requests in many threads
 Home-page: https://github.com/Harukvitalii
-Download-URL: https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.1.tar.gz
+Download-URL: https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.2.zip
 Author: Vitalii Haruk
 Author-email: garuk1vitalik@gmail.com
 License: MIT
 Keywords: aiohttp,requests,threads
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `arequestsHelper-0.4.1/arequestsHelper/arequestsHelper.py` & `arequestsHelper-0.4.2/arequestsHelper/arequestsHelper.py`

 * *Files 26% similar despite different names*

```diff
@@ -31,23 +31,14 @@
     async def get_json_get(self,client: aiohttp.ClientSession, url: str,proxy,force_json = False) -> dict:
         if proxy == None: 
             async with client.request('GET', url,ssl=False,timeout=30) as response:
                 return await self.errors_catcher(response, force_json)
         else: 
             async with client.request('GET', url,proxy=proxy[0], proxy_auth=proxy[1],ssl=False,timeout=30) as response:
                 return await self.errors_catcher(response, force_json)
-            
-    async def get_json_patch(self,client: aiohttp.ClientSession, url: str, data ,proxy,force_json = False) -> dict:
-        if proxy == None: 
-            async with client.request('PATCH', url, json = data, ssl=False,timeout=30) as response:
-                return await self.errors_catcher(response, force_json)
-        else: 
-            async with client.request('PATCH', url, json = data, proxy=proxy[0], proxy_auth=proxy[1],ssl=False,timeout=30) as response:
-                return await self.errors_catcher(response, force_json)
-    
         
 
     async def errors_catcher(self,response, force_json = False): 
         content_type = response.headers['Content-Type']
         # print(response)
         try: 
             resp = await response.json(content_type=None)
@@ -98,31 +89,22 @@
         r = requests.get(url = URL, params = PARAMS,verify=False)
         return r
     
     
     def run_function_with_exception(self, func, start_abr_for_notification: str, func_args = (),  tries: int = 10,attempt = 1, otladka: bool = False):
         if otladka:
             asyncio.run(func(func_args))
-            print('test Run successfully')
+            print('done Success')
             exit()
             
             
-        while attempt != tries:
+        while True:
             try: 
                 asyncio.run(func(func_args))
-
-            except KeyError:
-                print('Login Please') 
-                self.bot_notify_normal(f'{start_abr_for_notification} ERROR Login Please')
-
-            except aiohttp.client_exceptions.ClientOSError:
-                print(errs['System ERROR'])
-                time.sleep(10)
-                self.run_function_with_exception(func,start_abr_for_notification,attempt=attempt+1)
-                self.bot_notify_normal(f'{start_abr_for_notification} ERROR Winodws closed connection\nAttempt {attempt+1}')
+                
             except Exception as e:
                 print(e)
                 # print(errs['ERROR'])
                 exc_type, exc_obj, exc_tb = sys.exc_info()
                 fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
                 print(exc_type, fname, exc_tb.tb_lineno)
                 time.sleep(10)
```

### Comparing `arequestsHelper-0.4.1/arequestsHelper.egg-info/PKG-INFO` & `arequestsHelper-0.4.2/arequestsHelper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: arequestsHelper
-Version: 0.4.1
+Version: 0.4.2
 Summary: This pakage helps to work with aiohttp requests in many threads
 Home-page: https://github.com/Harukvitalii
-Download-URL: https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.1.tar.gz
+Download-URL: https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.2.zip
 Author: Vitalii Haruk
 Author-email: garuk1vitalik@gmail.com
 License: MIT
 Keywords: aiohttp,requests,threads
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `arequestsHelper-0.4.1/setup.py` & `arequestsHelper-0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'arequestsHelper',         # How you named your package folder (MyLib)
   packages = ['arequestsHelper'],   # Chose the same as "name"
-  version = '0.4.1',      # Start with a small number and increase it with every change you make
+  version = '0.4.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = "This pakage helps to work with aiohttp requests in many threads",   # Give a short description about your library
   author = 'Vitalii Haruk',                   # Type in your name
   author_email = "garuk1vitalik@gmail.com",      # Type in your E-Mail
   url = "https://github.com/Harukvitalii",   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.2.zip',    # I explain this later on
   keywords = ['aiohttp', 'requests', 'threads'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests',
           'aiohttp',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
@@ -23,8 +23,8 @@
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
   ],
 )
 
 # python setup.py sdist
-# twine upload dist/*
+#twine upload dist/*
```

