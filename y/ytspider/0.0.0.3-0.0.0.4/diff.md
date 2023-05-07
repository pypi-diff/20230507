# Comparing `tmp/ytspider-0.0.0.3.tar.gz` & `tmp/ytspider-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytspider-0.0.0.3.tar", last modified: Tue May  2 17:37:29 2023, max compression
+gzip compressed data, was "ytspider-0.0.0.4.tar", last modified: Sun May  7 13:53:08 2023, max compression
```

## Comparing `ytspider-0.0.0.3.tar` & `ytspider-0.0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 17:37:29.650541 ytspider-0.0.0.3/
--rw-rw-rw-   0        0        0      377 2023-05-02 17:37:29.650541 ytspider-0.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-04-30 18:25:19.000000 ytspider-0.0.0.3/README.md
--rw-rw-rw-   0        0        0      115 2023-05-02 17:37:29.650541 ytspider-0.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-05-02 17:36:59.000000 ytspider-0.0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:37:29.555648 ytspider-0.0.0.3/src/
--rw-rw-rw-   0        0        0       45 2023-04-30 20:45:34.000000 ytspider-0.0.0.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:37:29.618361 ytspider-0.0.0.3/src/utils/
--rw-rw-rw-   0        0        0        0 2023-04-30 20:26:12.000000 ytspider-0.0.0.3/src/utils/__init__.py
--rw-rw-rw-   0        0        0     1969 2023-04-30 11:28:54.000000 ytspider-0.0.0.3/src/utils/client.py
--rw-rw-rw-   0        0        0     1670 2023-05-01 20:14:19.000000 ytspider-0.0.0.3/src/utils/context.py
--rw-rw-rw-   0        0        0     2938 2023-05-01 20:13:59.000000 ytspider-0.0.0.3/src/utils/decorator.py
--rw-rw-rw-   0        0        0     7605 2023-05-02 17:30:12.000000 ytspider-0.0.0.3/src/utils/handler.py
--rw-rw-rw-   0        0        0      707 2023-04-30 11:29:20.000000 ytspider-0.0.0.3/src/utils/playback_context.py
--rw-rw-rw-   0        0        0     2607 2023-05-02 00:21:25.000000 ytspider-0.0.0.3/src/utils/request.py
--rw-rw-rw-   0        0        0      951 2023-04-30 11:18:54.000000 ytspider-0.0.0.3/src/utils/signals_info.py
--rw-rw-rw-   0        0        0     6866 2023-05-02 16:57:42.000000 ytspider-0.0.0.3/src/ytspider.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:37:29.649735 ytspider-0.0.0.3/ytspider.egg-info/
--rw-rw-rw-   0        0        0      377 2023-05-02 17:37:29.000000 ytspider-0.0.0.3/ytspider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-05-02 17:37:29.000000 ytspider-0.0.0.3/ytspider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 17:37:29.000000 ytspider-0.0.0.3/ytspider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 17:37:29.000000 ytspider-0.0.0.3/ytspider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 17:37:29.000000 ytspider-0.0.0.3/ytspider.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 13:53:08.211298 ytspider-0.0.0.4/
+-rw-rw-rw-   0        0        0      377 2023-05-07 13:53:08.211298 ytspider-0.0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-04-30 18:25:19.000000 ytspider-0.0.0.4/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-07 13:53:08.212298 ytspider-0.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-05-07 13:52:59.000000 ytspider-0.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:53:08.158320 ytspider-0.0.0.4/src/
+-rw-rw-rw-   0        0        0       45 2023-04-30 20:45:34.000000 ytspider-0.0.0.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:53:08.194387 ytspider-0.0.0.4/src/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-30 20:26:12.000000 ytspider-0.0.0.4/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     1969 2023-04-30 11:28:54.000000 ytspider-0.0.0.4/src/utils/client.py
+-rw-rw-rw-   0        0        0     1670 2023-05-01 20:14:19.000000 ytspider-0.0.0.4/src/utils/context.py
+-rw-rw-rw-   0        0        0     2938 2023-05-01 20:13:59.000000 ytspider-0.0.0.4/src/utils/decorator.py
+-rw-rw-rw-   0        0        0     7942 2023-05-07 13:49:20.000000 ytspider-0.0.0.4/src/utils/handler.py
+-rw-rw-rw-   0        0        0      707 2023-04-30 11:29:20.000000 ytspider-0.0.0.4/src/utils/playback_context.py
+-rw-rw-rw-   0        0        0     2609 2023-05-07 13:23:21.000000 ytspider-0.0.0.4/src/utils/request.py
+-rw-rw-rw-   0        0        0      951 2023-04-30 11:18:54.000000 ytspider-0.0.0.4/src/utils/signals_info.py
+-rw-rw-rw-   0        0        0     7453 2023-05-07 13:52:15.000000 ytspider-0.0.0.4/src/ytspider.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:53:08.208758 ytspider-0.0.0.4/ytspider.egg-info/
+-rw-rw-rw-   0        0        0      377 2023-05-07 13:53:08.000000 ytspider-0.0.0.4/ytspider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-05-07 13:53:08.000000 ytspider-0.0.0.4/ytspider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 13:53:08.000000 ytspider-0.0.0.4/ytspider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-07 13:53:08.000000 ytspider-0.0.0.4/ytspider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-07 13:53:08.000000 ytspider-0.0.0.4/ytspider.egg-info/top_level.txt
```

### Comparing `ytspider-0.0.0.3/README.md` & `ytspider-0.0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.3/setup.py` & `ytspider-0.0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='ytspider',
     description="YouTube scraper, videos, channels, playlists, comments and transcriptions",
-    version='0.0.0.3',
+    version='0.0.0.4',
     license='MIT',
     author="Zeyad Khalid",
     maintainer_email='zeyad.khalid@must.edu.eg',
     author_email='zeyadpro99@gmail.com',
     package_dir={"ytspider":"src"},
     packages=find_packages(),#["ytspider","ytspider.utils"],
     py_modules=["ytspider.py"],
```

### Comparing `ytspider-0.0.0.3/src/utils/client.py` & `ytspider-0.0.0.4/src/utils/client.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.3/src/utils/context.py` & `ytspider-0.0.0.4/src/utils/context.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.3/src/utils/decorator.py` & `ytspider-0.0.0.4/src/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.3/src/utils/handler.py` & `ytspider-0.0.0.4/src/utils/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,28 +49,34 @@
                     firstTime = False
                 # Couldn't get token for comment retrieval
                 except Exception as e:
                     token = None
             else:
                 # Try get comments
                 try:
-                    comments = result["onResponseReceivedEndpoints"][-1]["reloadContinuationItemsCommand"]["continuationItems"][:-1]
-                
+
+                    commentsContainer = result["onResponseReceivedEndpoints"][-1]["reloadContinuationItemsCommand"]["continuationItems"]
+                    
+                    # If it's only one comment on the video, get it
+                    if len(commentsContainer) == 1:
+                        comments = [commentsContainer[0]]
+                    # +2 comments, grab all but the last item (token)
+                    else:
+                        comments = commentsContainer[:-1]
                 # There are no comments at all (not a single one!)
                 except Exception as e:
-                    comments = []
+                    pass
                 
                 # Try get token, but if comments are < 20, there is no 'continuation' token because there're no more comments
                 try:
                     token = result["onResponseReceivedEndpoints"][-1]["reloadContinuationItemsCommand"]["continuationItems"][-1]["commentThreadRenderer"]["continuationEndpoint"]["continuationCommand"]["token"]
                 
                 # No more comments
                 except Exception as e:
                     token = None
-
                 for i in range(len(comments)):
                     comment_texts = comments[i]["commentThreadRenderer"]["comment"]["commentRenderer"]["contentText"]['runs']
                     comment = " ".join(
                         list(map(lambda c: c["text"], comment_texts)))
                     all_comments.append(comment)
         return all_comments
```

### Comparing `ytspider-0.0.0.3/src/utils/playback_context.py` & `ytspider-0.0.0.4/src/utils/playback_context.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.3/src/utils/request.py` & `ytspider-0.0.0.4/src/utils/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,11 +72,11 @@
 
         if response.status_code == 200:
             if method.upper() == "GET":
                 return response
             elif method.upper() == "POST":
                 return response.json()
         else:
-            print(response.content)
+            # print(response.content)
             raise RuntimeError(f"Request failed ({response.status_code})")
         return None
```

### Comparing `ytspider-0.0.0.3/src/utils/signals_info.py` & `ytspider-0.0.0.4/src/utils/signals_info.py`

 * *Files identical despite different names*

### Comparing `ytspider-0.0.0.3/src/ytspider.py` & `ytspider-0.0.0.4/src/ytspider.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     def __init__(self):
         self.Request = Request()
         self.__Response = {}
         self.__Context = Context()
         self.handlers = {}
         self.defaultHandlers = {}
+        self.itemId = []
 
     def attachHandler(self, handler):
         if not isinstance(handler, BaseHandler):
             raise ValueError(
                 "Argument (handler) must be a subclass of BaseHandler")
         if not handler.name in self.defaultHandlers:
             self.defaultHandlers[handler.name] = handler
@@ -59,59 +60,64 @@
 
     def scrape(self, itemId, continuation_token=None):
         self.__Response.clear()
         if type(itemId) == str:
             # self.itemId = itemId
             # self.__Response.update({itemId: self.scrapeSingle(itemId)})
             result = self.scrapeSingle(itemId)
-            key = self.itemId if hasattr(self, "itemId") else itemId
+            key =  self.itemId[0] if (len(self.itemId) > 0) else "undefined"
             self.__Response.update({key: result})
         elif type(itemId) == list:
             for i, id in enumerate(itemId):
                 if type(id) == str:
-                    # self.itemId = id
                     # self.__Response.update({id: self.scrapeSingle(id)})
                     result = self.scrapeSingle(id)
-                    key = self.itemId if hasattr(self, "itemId") else id
+                    key = self.itemId[i] if hasattr(self, "itemId") else id
                     self.__Response.update({key: result})
                 else:
                     raise ValueError(
                         f"Invalid data type at index {i}. Expected str")
         return self
 
     def scrapeSingle(self, itemId):
         result = {itemId: None}
         return result
 
     def get(self):
         for itemId in self.__Response.keys():
-            self.itemId = itemId
+            # self.itemId = itemId
             result = self.executeHandlers(itemId)
-
-            if itemId in self.__Response:
-                self.__Response[itemId].update(result)
-            else:
-                self.__Response[itemId] = result
+            # Set result in response item if and only if result contains data
+            if result is not None:
+                if itemId in self.__Response:
+                    # Sometimes, scraper has itemId, but no results (None)
+                    # in this case, just attach whatever the handler's got
+                    if self.__Response[itemId] is None:
+                        self.__Response[itemId] = result
+                    else:
+                        self.__Response[itemId].update(result)
+                else:
+                    self.__Response[itemId] = result
         self.restoreDefaultHandlers()
         return self.__Response
 
 
 
 class YTSVideo(YTSpider, CommentScraper, TranscriptScraper):
     def __init__(self, commentDefaultHandler=None, transcriptDefaultHandler=None):
         super(YTSVideo, self).__init__()
         CommentScraper.__init__(self, commentDefaultHandler)
         TranscriptScraper.__init__(self, transcriptDefaultHandler)
         self.url = "https://www.youtube.com/youtubei/v1/player?key=AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8&prettyPrint=false"
 
-        #
     def scrapeSingle(self, itemId):
         self.Request.updateContextState(itemId)
         result = self.Request.send(self.url, "POST")
         if "videoDetails" in result:
+            self.itemId.append(result["videoDetails"]["videoId"])
             return result["videoDetails"]
         return None
 
 class YTSChannel(YTSpider, VideosScraper):
     def __init__(self, videosDefaultHandler=None):
         super(YTSChannel, self).__init__()
         VideosScraper.__init__(self, videosDefaultHandler)
@@ -160,29 +166,28 @@
             for criteria in attributes:
                 for metaKey in attributes[criteria]:
                     tag = soup.find("meta", {criteria: metaKey})
                     if tag is not None:
                         tagInnerContent = tag['content']
                         data[metaKey] = tagInnerContent
         
-        # if "channelId" not in data:
-        #     channelId = 
-        # print(soup.find("meta", {"itemprop":"channelId"}))
-            # channelIds = re.findall(r'"browseId":"([a-zA-Z0-9 _ -]+)"', str(soup))
-            # if len(channelIds) > 0:
-            #     data["channelId"] = channelIds[0]
-        if "channelId" in data:
-            self.itemId = data["channelId"]
-            return data
+        # Sometimes, response does not include channelId in meta tags
+        # In this case -> brute-force extract channelId from embedded JS code
+        if "channelId" not in data:
+            channelIds = re.findall(r'"browseId":"([a-zA-Z0-9 _ -]+)"', str(soup))
+            if len(channelIds) > 0:
+                data["channelId"] = channelIds[0]
+                # print("ACTUATED CHANNEL " + channelIds[0])
+                self.itemId.append(data["channelId"])
+        
+        # channelId is found in HTML meta tags
         else:
-            return None
+            # print("SELF EXTRACTED " + data["channelId"])
+            self.itemId.append(data["channelId"])
+        return data
 
     def scrapeSingle(self, screenName):
         endpoint = self.prepareURL(screenName)
-        print("HHH")
-        print(endpoint)
         result = self.Request.send(endpoint)
         data = self.__postProcessResponse(result)
-        if not hasattr(self, "itemId"):
-            self.itemId = screenName
         return data
```

