# Comparing `tmp/ZaidPP-0.3.1.tar.gz` & `tmp/ZaidPP-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZaidPP-0.3.1.tar", last modified: Sat May  6 17:31:00 2023, max compression
+gzip compressed data, was "ZaidPP-0.4.1.tar", last modified: Sun May  7 18:14:20 2023, max compression
```

## Comparing `ZaidPP-0.3.1.tar` & `ZaidPP-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 17:31:00.710495 ZaidPP-0.3.1/
--rw-rw-rw-   0        0        0       32 2023-04-19 17:51:40.000000 ZaidPP-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0      842 2023-05-06 17:31:00.709510 ZaidPP-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-04-21 20:51:26.000000 ZaidPP-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 17:31:00.711493 ZaidPP-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      956 2023-05-06 17:21:29.000000 ZaidPP-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:31:00.669516 ZaidPP-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 17:31:00.684507 ZaidPP-0.3.1/src/ZaidPP/
--rw-rw-rw-   0        0        0    13721 2023-05-06 17:28:03.000000 ZaidPP-0.3.1/src/ZaidPP/ZaidPP.py
--rw-rw-rw-   0        0        0       24 2023-04-22 22:35:06.000000 ZaidPP-0.3.1/src/ZaidPP/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:31:00.706511 ZaidPP-0.3.1/src/ZaidPP.egg-info/
--rw-rw-rw-   0        0        0      842 2023-05-06 17:31:00.000000 ZaidPP-0.3.1/src/ZaidPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-05-06 17:31:00.000000 ZaidPP-0.3.1/src/ZaidPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 17:31:00.000000 ZaidPP-0.3.1/src/ZaidPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 17:31:00.000000 ZaidPP-0.3.1/src/ZaidPP.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 18:14:20.922875 ZaidPP-0.4.1/
+-rw-rw-rw-   0        0        0       32 2023-04-19 17:51:40.000000 ZaidPP-0.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      842 2023-05-07 18:14:20.922875 ZaidPP-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-04-21 20:51:26.000000 ZaidPP-0.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 18:14:20.922875 ZaidPP-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      956 2023-05-07 18:13:11.000000 ZaidPP-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 18:14:20.898267 ZaidPP-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 18:14:20.909491 ZaidPP-0.4.1/src/ZaidPP/
+-rw-rw-rw-   0        0        0    14578 2023-05-07 18:10:29.000000 ZaidPP-0.4.1/src/ZaidPP/ZaidPP.py
+-rw-rw-rw-   0        0        0       24 2023-04-22 22:35:06.000000 ZaidPP-0.4.1/src/ZaidPP/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 18:14:20.922875 ZaidPP-0.4.1/src/ZaidPP.egg-info/
+-rw-rw-rw-   0        0        0      842 2023-05-07 18:14:20.000000 ZaidPP-0.4.1/src/ZaidPP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-05-07 18:14:20.000000 ZaidPP-0.4.1/src/ZaidPP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 18:14:20.000000 ZaidPP-0.4.1/src/ZaidPP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 18:14:20.000000 ZaidPP-0.4.1/src/ZaidPP.egg-info/top_level.txt
```

### Comparing `ZaidPP-0.3.1/PKG-INFO` & `ZaidPP-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZaidPP
-Version: 0.3.1
+Version: 0.4.1
 Summary: • Scrape Instagram Profile and login Instagram
 Home-page: 
 Author: Zaid
 Author-email: www710700@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ZaidPP-0.3.1/setup.py` & `ZaidPP-0.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 f.write('instaloder\nuser_agent\nrequests\nuuid')
 
 fr = open("requirements.txt",'r')
 requires = fr.read().split('\n')
     
 setuptools.setup(
     name="ZaidPP",
-    version="0.3.1",
+    version="0.4.1",
     author="Zaid",
     author_email="www710700@gmail.com",
     description="• Scrape Instagram Profile and login Instagram",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={
```

### Comparing `ZaidPP-0.3.1/src/ZaidPP/ZaidPP.py` & `ZaidPP-0.4.1/src/ZaidPP/ZaidPP.py`

 * *Files 7% similar despite different names*

```diff
@@ -109,15 +109,17 @@
 		    }, cookies = {
 		        'cookie'                    : cookies
 		    })
 		    
 		    
 		
 		    find_token = re.search('(EAAG\w+)', data.text)
+		    #print(find_token)
 		    results    = '\n* Fail : maybe your cookie invalid !!' if (find_token is None) else find_token.group(1)
+		    #print(results)
 		except requests.exceptions.ConnectionError:
 		    results    = '\n* Fail : no connection here !!'
 		except:
 		    results    = '\n* Fail : unknown errors, please try again !!'
 		
 		return results
 
@@ -196,8 +198,42 @@
 'x-requested-with': 'XMLHttpRequest',}
 
 		try:
 			rr = requests.get(f'https://www.instagram.com/api/v1/users/web_profile_info/?username={user}',headers=he).json();user=user;id = rr['data']['user']['id'];name=rr['data']['user']['full_name'];bio = rr['data']['user']['biography'];flos = rr['data']['user']['edge_followed_by']['count'];flog = rr['data']['user']['edge_follow']['count'];pr=rr['data']['user']['is_private'];re = requests.get(f"https://o7aa.pythonanywhere.com/?id={id}").json();da = re['date']
 			resp = {"user":user,"name":name,"id":id,"private":pr,"date":da,"following":flog,"followers":flos,"bio":bio}
 			return resp
 		except:
-			return {"status":"Error","Username":"Unavailable"}
+			return {"status":"Error","Username":"Unavailable"}
+
+
+	def store_add(text):
+		try:
+			te = text.split(':')[0]
+			te1 = text.split(':')[1]
+			rr = requests.get(f'https://store-mktbh.zaidbot.repl.co/1/text={te}:add:{te1}').text
+			return rr
+		except:
+			return {"Error":"Type-Enter"}
+
+	def store_dde(text):
+		try:
+			te = text.split(':')[0]
+			te1 = text.split(':')[1]
+			rr = requests.get(f'https://store-mktbh.zaidbot.repl.co/1/text={te}:dde:{te1}').text
+			return rr
+		except:
+			return {"Error":"Type-Enter"}
+			
+	def store_open(text):
+		try:
+			rr = requests.get(f'https://store-mktbh.zaidbot.repl.co/1/text={text}:ok:').text
+			return rr
+		except:
+			return {"Error":"Type-Enter"}
+		
+	def store_exit(text):
+		try:
+			rr = requests.get(f'https://store-mktbh.zaidbot.repl.co/1/text={text}:all:').text
+			return rr
+		except:
+			return {"Error":"Type-Enter"}
+
```

### Comparing `ZaidPP-0.3.1/src/ZaidPP.egg-info/PKG-INFO` & `ZaidPP-0.4.1/src/ZaidPP.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZaidPP
-Version: 0.3.1
+Version: 0.4.1
 Summary: • Scrape Instagram Profile and login Instagram
 Home-page: 
 Author: Zaid
 Author-email: www710700@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

