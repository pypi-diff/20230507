# Comparing `tmp/EdgeGPT-0.3.5.tar.gz` & `tmp/EdgeGPT-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.3.5.tar", last modified: Wed May  3 10:12:11 2023, max compression
+gzip compressed data, was "EdgeGPT-0.3.6.tar", last modified: Sun May  7 09:45:55 2023, max compression
```

## Comparing `EdgeGPT-0.3.5.tar` & `EdgeGPT-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:12:11.122613 EdgeGPT-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 10:11:41.000000 EdgeGPT-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-03 10:12:11.122613 EdgeGPT-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-03 10:12:10.000000 EdgeGPT-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 10:12:11.122613 EdgeGPT-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-03 10:11:41.000000 EdgeGPT-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:12:11.122613 EdgeGPT-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:12:11.122613 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-03 10:12:11.000000 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-03 10:12:11.000000 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:12:11.000000 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 10:12:11.000000 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 10:12:11.000000 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 10:12:11.000000 EdgeGPT-0.3.5/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29462 2023-05-03 10:11:41.000000 EdgeGPT-0.3.5/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-03 10:11:41.000000 EdgeGPT-0.3.5/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:45:55.828800 EdgeGPT-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-07 09:45:25.000000 EdgeGPT-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-07 09:45:55.828800 EdgeGPT-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 09:45:55.832800 EdgeGPT-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-07 09:45:25.000000 EdgeGPT-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:45:55.828800 EdgeGPT-0.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:45:55.828800 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 09:45:55.000000 EdgeGPT-0.3.6/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29532 2023-05-07 09:45:25.000000 EdgeGPT-0.3.6/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-07 09:45:25.000000 EdgeGPT-0.3.6/src/ImageGen.py
```

### Comparing `EdgeGPT-0.3.5/LICENSE` & `EdgeGPT-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.5/PKG-INFO` & `EdgeGPT-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.5
+Version: 0.3.6
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.5 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.6 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.3.5/README.md` & `EdgeGPT-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.5/setup.py` & `EdgeGPT-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.3.5",
+    version="0.3.6",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.3.5/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.3.6/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.5
+Version: 0.3.6
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.5 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.6 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.3.5/src/EdgeGPT.py` & `EdgeGPT-0.3.6/src/EdgeGPT.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 
     def update(
         self,
         prompt: str,
         conversation_style: CONVERSATION_STYLE_TYPE,
         options: list | None = None,
         webpage_context: str | None = None,
-        search_result: bool = False 
+        search_result: bool = False
     ) -> None:
         """
         Updates request object
         """
         if options is None:
             options = [
                 "deepleo",
@@ -338,15 +338,15 @@
         if self.struct["result"]["value"] == "UnauthorizedRequest":
             raise NotAllowedToAccess(self.struct["result"]["message"])
 
     @staticmethod
     async def create(
         cookies: dict,
         proxy: str | None = None,
-    ) -> None:
+    ) -> _Conversation:
         self = _Conversation(async_mode=True)
         self.struct = {
             "conversationId": None,
             "clientId": None,
             "conversationSignature": None,
             "result": {"value": "Success", "message": None},
         }
@@ -488,59 +488,57 @@
                     continue
                 response = json.loads(obj)
                 if response.get("type") != 2 and raw:
                     yield False, response
                 elif response.get("type") == 1 and response["arguments"][0].get(
                     "messages",
                 ):
-                    try:
-                        if not draw:
-                            if (
-                                response["arguments"][0]["messages"][0]["contentOrigin"]
-                                != "Apology"
-                            ):
+                    if not draw:
+                        if(response["arguments"][0]["messages"][0].get("messageType") == "GenerateContentQuery"):
+                            for item in cookies:
+                                if item["name"] == "_U":
+                                    U = item["value"]
+                            async with ImageGenAsync(U, True) as image_generator:
+                                images = await image_generator.get_images(
+                                    response["arguments"][0]["messages"][0]["text"],
+                                )
+                            cache = resp_txt
+                            resp_txt = (
+                                cache
+                                + "\n![image0]("
+                                + images[0]
+                                + ")\n![image1]("
+                                + images[1]
+                                + ")\n![image0]("
+                                + images[2]
+                                + ")\n![image3]("
+                                + images[3]
+                                + ")"
+                            )
+                            draw = True
+                        if (
+                            response["arguments"][0]["messages"][0]["contentOrigin"]
+                            != "Apology"
+                        ):
+                            if not draw:
                                 resp_txt = result_text+response["arguments"][0]["messages"][0][
                                     "adaptiveCards"
                                 ][0]["body"][0].get("text", "")
                                 resp_txt_no_link = result_text+response["arguments"][0]["messages"][
                                     0
                                 ].get("text", "")
                                 if(response["arguments"][0]["messages"][0].get("messageType")):
                                     resp_txt = resp_txt+response["arguments"][0]["messages"][0][
-                                    "adaptiveCards"
+                                        "adaptiveCards"
                                     ][0]["body"][0]["inlines"][0].get("text")+"\n"
                                     result_text = result_text+response["arguments"][0]["messages"][0][
-                                    "adaptiveCards"
+                                        "adaptiveCards"
                                     ][0]["body"][0]["inlines"][0].get("text")+"\n"
                         yield False, resp_txt
-                    except Exception as exc:
-                        print(exc)
-                        if not draw:
-                            continue
-                        for item in cookies:
-                            if item["name"] == "_U":
-                                U = item["value"]
-                        async with ImageGenAsync(U, True) as image_generator:
-                            images = await image_generator.get_images(
-                                response["arguments"][0]["messages"][0]["text"],
-                            )
-                        cache = resp_txt
-                        resp_txt = (
-                            cache
-                            + "\n![image0]("
-                            + images[0]
-                            + ")\n![image1]("
-                            + images[1]
-                            + ")\n![image0]("
-                            + images[2]
-                            + ")\n![image3]("
-                            + images[3]
-                            + ")"
-                        )
-                        yield False, resp_txt
+                        
                 elif response.get("type") == 2:
                     if draw:
                         cache = response["item"]["messages"][1]["adaptiveCards"][0][
                             "body"
                         ][0]["text"]
                         response["item"]["messages"][1]["adaptiveCards"][0]["body"][0][
                             "text"
@@ -640,25 +638,25 @@
             cookies=self.cookies,
             webpage_context=webpage_context,
             search_result=search_result
         ):
             if final:
                 return response
         await self.chat_hub.wss.close()
-        return None
+        return {}
 
     async def ask_stream(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
         webpage_context: str | None = None,
-        search_result: str = False
+        search_result: bool = False
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         async for response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
```

