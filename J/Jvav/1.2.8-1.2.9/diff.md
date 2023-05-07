# Comparing `tmp/Jvav-1.2.8.tar.gz` & `tmp/Jvav-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\akyna\Codes\jvav\dist\.tmp-m7htmn5o\Jvav-1.2.8.tar", last modified: Fri Mar 17 05:54:39 2023, max compression
+gzip compressed data, was "C:\Users\akyna\Codes\jvav\dist\.tmp-5wtz56n7\Jvav-1.2.9.tar", last modified: Sat Mar 18 11:48:36 2023, max compression
```

## Comparing `Jvav-1.2.8.tar` & `Jvav-1.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 05:54:39.000000 Jvav-1.2.8/
-drwxrwxrwx   0        0        0        0 2023-03-17 05:54:39.000000 Jvav-1.2.8/Jvav.egg-info/
--rw-rw-rw-   0        0        0     2229 2023-03-17 05:54:39.000000 Jvav-1.2.8/Jvav.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-03-17 05:54:39.000000 Jvav-1.2.8/Jvav.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 05:54:39.000000 Jvav-1.2.8/Jvav.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-03-17 05:54:39.000000 Jvav-1.2.8/Jvav.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-16 05:58:00.000000 Jvav-1.2.8/Jvav.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      138 2023-03-17 05:54:39.000000 Jvav-1.2.8/Jvav.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-17 05:54:39.000000 Jvav-1.2.8/Jvav.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2023-03-16 05:23:06.000000 Jvav-1.2.8/LICENSE
--rw-rw-rw-   0        0        0      108 2023-03-16 05:23:06.000000 Jvav-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2229 2023-03-17 05:54:39.000000 Jvav-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1424 2023-03-16 05:23:06.000000 Jvav-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-17 05:54:39.000000 Jvav-1.2.8/jvav/
--rw-rw-rw-   0        0        0      312 2023-03-16 05:23:06.000000 Jvav-1.2.8/jvav/__init__.py
--rw-rw-rw-   0        0        0     5228 2023-03-16 13:11:07.000000 Jvav-1.2.8/jvav/cmd.py
--rw-rw-rw-   0        0        0    36525 2023-03-17 05:54:08.000000 Jvav-1.2.8/jvav/utils.py
--rw-rw-rw-   0        0        0      145 2023-03-16 06:07:30.000000 Jvav-1.2.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-17 05:54:39.000000 Jvav-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1395 2023-03-17 05:54:17.000000 Jvav-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-18 11:48:36.000000 Jvav-1.2.9/
+drwxrwxrwx   0        0        0        0 2023-03-18 11:48:36.000000 Jvav-1.2.9/Jvav.egg-info/
+-rw-rw-rw-   0        0        0     2229 2023-03-18 11:48:36.000000 Jvav-1.2.9/Jvav.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-03-18 11:48:36.000000 Jvav-1.2.9/Jvav.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-18 11:48:36.000000 Jvav-1.2.9/Jvav.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-03-18 11:48:36.000000 Jvav-1.2.9/Jvav.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-03-16 05:58:00.000000 Jvav-1.2.9/Jvav.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      138 2023-03-18 11:48:36.000000 Jvav-1.2.9/Jvav.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-03-18 11:48:36.000000 Jvav-1.2.9/Jvav.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2023-03-16 05:23:06.000000 Jvav-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0      108 2023-03-16 05:23:06.000000 Jvav-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2229 2023-03-18 11:48:36.000000 Jvav-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1424 2023-03-16 05:23:06.000000 Jvav-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-18 11:48:36.000000 Jvav-1.2.9/jvav/
+-rw-rw-rw-   0        0        0      312 2023-03-16 05:23:06.000000 Jvav-1.2.9/jvav/__init__.py
+-rw-rw-rw-   0        0        0     5228 2023-03-16 13:11:07.000000 Jvav-1.2.9/jvav/cmd.py
+-rw-rw-rw-   0        0        0    38338 2023-03-18 11:46:09.000000 Jvav-1.2.9/jvav/utils.py
+-rw-rw-rw-   0        0        0      145 2023-03-16 06:07:30.000000 Jvav-1.2.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-03-18 11:48:36.000000 Jvav-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1395 2023-03-18 11:48:24.000000 Jvav-1.2.9/setup.py
```

### Comparing `Jvav-1.2.8/Jvav.egg-info/PKG-INFO` & `Jvav-1.2.9/Jvav.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.2.8
+Version: 1.2.9
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
```

### Comparing `Jvav-1.2.8/LICENSE` & `Jvav-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Jvav-1.2.8/PKG-INFO` & `Jvav-1.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.2.8
+Version: 1.2.9
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
```

### Comparing `Jvav-1.2.8/README.md` & `Jvav-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `Jvav-1.2.8/jvav/cmd.py` & `Jvav-1.2.9/jvav/cmd.py`

 * *Files identical despite different names*

### Comparing `Jvav-1.2.8/jvav/utils.py` & `Jvav-1.2.9/jvav/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,14 +114,20 @@
         BASE_URL_MOST_WANTED_ALL,
     ]
     URLS_NEW = [
         BASE_URL_NEW_RELEASE_HAVE_COMMENT,
         BASE_URL_NEW_RELEASE_ALL,
         BASE_URL_NEW_ENTRIES,
     ]
+    # search
+    BASE_URL_SEARCH_AV = BASE_URL + "/cn/vl_searchbyid.php?keyword="
+    # comment
+    BASE_URL_COMMENT = BASE_URL + "/cn/videocomments.php?v="
+    # review 最佳评论
+    BASE_URL_REVIEW = BASE_URL + "/cn/videoreviews.php?v="
 
     def __init__(
         self,
         proxy_addr="",
         max_rank_page=25,
     ):
         """初始化
@@ -155,14 +161,52 @@
             ids = [tag.text for tag in tag_ids]
             if len(ids) > 0:
                 return 200, random.choice(ids)
         except Exception as e:
             self.log.error(f"JavLibUtil: 从排行榜随机获取番号: {e}")
             return 404, None
 
+    def get_comments_by_id(self, id: str, timeout=3) -> typing.Tuple[int, list]:
+        """根据番号获取评论 (最佳评论, 最多 5 条)
+
+        :param str id: 番号
+        :param int timeout: 超时时间(秒), 默认为 3
+        :return typing.Tuple[int, list]: 状态码和评论列表
+        """
+        url = JavLibUtil.BASE_URL_SEARCH_AV + id
+        code, resp = self.send_req(url=url, timeout=timeout)
+        if code != 200:
+            return code, None
+        javlib_av_id = ""
+        if resp.url == url:
+            try:
+                soup = self.get_soup(resp)
+                videos = soup.find_all(class_="video")
+                video_href = videos[0].a["href"]
+                javlib_av_id = video_href[video_href.find("v=") + 2 :]
+            except Exception as e:
+                self.log.error(f"JavLibUtil: 根据番号 {id} 获取评论失败: {e}")
+                return 404, None
+        else:
+            r_url = resp.url
+            javlib_av_id = r_url[r_url.find("v=") + 2 :]
+        comment_url = JavLibUtil.BASE_URL_REVIEW + javlib_av_id
+        code, resp = self.send_req(url=comment_url, timeout=timeout)
+        if code != 200:
+            return code, None
+        try:
+            soup = self.get_soup(resp)
+            comment_tags = soup.find_all(class_="t")
+            comments = []
+            for c in comment_tags:
+                comments.append(c.text)
+            return 200, comments[:5]
+        except Exception as e:
+            self.log.error(f"JavLibUtil: 根据番号 {id} 获取评论失败: {e}")
+
 
 class DmmUtil(BaseUtil):
     BASE_URL = "https://www.dmm.co.jp"
     BASE_URL_SEARCH_AV = BASE_URL + "/search/=/searchstr="
     BASE_URL_SEARCH_STAR = (
         BASE_URL + "/digital/videoa/-/list/search/=/device=tv/sort=ranking/?searchstr="
     )
```

### Comparing `Jvav-1.2.8/setup.py` & `Jvav-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("requirements.txt", encoding="utf-8") as r:
     requires = [i.strip() for i in r]
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(name="Jvav",
-      version='1.2.8',
+      version='1.2.9',
       description="Useful tools for Jav.",
       long_description=readme,
       long_description_content_type="text/markdown",
       url="https://github.com/akynazh/jvav",
       download_url="https://github.com/akynazh/jvav/releases/latest",
       author="akynazh",
       author_email="akynazh@gmail.com",
```

