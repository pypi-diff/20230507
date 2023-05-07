# Comparing `tmp/Omar_Style_sel-0.5.tar.gz` & `tmp/Omar_Style_sel-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Omar_Style_sel-0.5.tar", last modified: Fri May  5 19:21:28 2023, max compression
+gzip compressed data, was "Omar_Style_sel-0.6.tar", last modified: Sun May  7 17:15:38 2023, max compression
```

## Comparing `Omar_Style_sel-0.5.tar` & `Omar_Style_sel-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:21:28.675215 Omar_Style_sel-0.5/
--rw-rw-rw-   0        0        0       36 2023-04-01 18:28:23.000000 Omar_Style_sel-0.5/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-05 19:21:28.617338 Omar_Style_sel-0.5/Omar_Style_sel/
--rw-rw-rw-   0        0        0     5266 2023-05-05 19:19:58.000000 Omar_Style_sel-0.5/Omar_Style_sel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:21:28.666215 Omar_Style_sel-0.5/Omar_Style_sel.egg-info/
--rw-rw-rw-   0        0        0     1833 2023-05-05 19:21:28.000000 Omar_Style_sel-0.5/Omar_Style_sel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-05 19:21:28.000000 Omar_Style_sel-0.5/Omar_Style_sel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:21:28.000000 Omar_Style_sel-0.5/Omar_Style_sel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-05 19:21:28.000000 Omar_Style_sel-0.5/Omar_Style_sel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-05 19:21:28.000000 Omar_Style_sel-0.5/Omar_Style_sel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1833 2023-05-05 19:21:28.670215 Omar_Style_sel-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1253 2023-04-25 18:53:37.000000 Omar_Style_sel-0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 19:21:28.676215 Omar_Style_sel-0.5/setup.cfg
--rw-rw-rw-   0        0        0      921 2023-05-05 19:21:07.000000 Omar_Style_sel-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:15:38.249830 Omar_Style_sel-0.6/
+-rw-rw-rw-   0        0        0       36 2023-04-01 18:28:23.000000 Omar_Style_sel-0.6/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-07 17:15:38.162823 Omar_Style_sel-0.6/Omar_Style_sel/
+-rw-rw-rw-   0        0        0     5870 2023-05-07 17:14:20.000000 Omar_Style_sel-0.6/Omar_Style_sel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:15:38.234827 Omar_Style_sel-0.6/Omar_Style_sel.egg-info/
+-rw-rw-rw-   0        0        0     2210 2023-05-07 17:15:37.000000 Omar_Style_sel-0.6/Omar_Style_sel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-07 17:15:37.000000 Omar_Style_sel-0.6/Omar_Style_sel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 17:15:37.000000 Omar_Style_sel-0.6/Omar_Style_sel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-07 17:15:37.000000 Omar_Style_sel-0.6/Omar_Style_sel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-07 17:15:37.000000 Omar_Style_sel-0.6/Omar_Style_sel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2210 2023-05-07 17:15:38.236827 Omar_Style_sel-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1630 2023-05-07 17:09:10.000000 Omar_Style_sel-0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 17:15:38.251829 Omar_Style_sel-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      921 2023-05-07 17:11:28.000000 Omar_Style_sel-0.6/setup.py
```

### Comparing `Omar_Style_sel-0.5/Omar_Style_sel/__init__.py` & `Omar_Style_sel-0.6/Omar_Style_sel/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,22 +38,24 @@
         firefox_profile.set_preference("network.proxy.ssl", proxy_host)
         firefox_profile.set_preference("network.proxy.ssl_port", int(proxy_port))
 
         driver = webdriver.Firefox(firefox_profile=firefox_profile)
         driver.get(firr)
         return driver
 
-    def proxy_chrome(self,proxy_address,Link,driver_path=None):
+    def proxy_chrome(self,proxy_address,Link,user,driver_path=None):
         options = Options()
         # options.add_argument("window-size=1400,600")
         from fake_useragent import UserAgent
         ua = UserAgent()
         user_agent = ua.random
-        print(user_agent)
-        options.add_argument(f'user-agent={user_agent}')
+        # print(user_agent)
+        if user:
+            options.add_argument(f'user-agent={user_agent}')
+            
         
         # driver = webdriver.Chrome(chrome_options=options)
         # driver.get('https://whoer.net/')
         # driver.quit()
 
         """
 
@@ -68,17 +70,17 @@
         except ValueError:
             raise ValueError("Please enter the proxy correctly. Example: 95.56.254.139:3128")
 
         chrome_options = webdriver.ChromeOptions()
         chrome_options.add_argument(f'--proxy-server={proxy_host}:{proxy_port}')
 
         if driver_path is None:
-            driver = webdriver.Chrome(options=chrome_options,chrome_options=options)
+            driver = webdriver.Chrome(options=chrome_options)
         else:
-            driver = webdriver.Chrome(driver_path, options=chrome_options,chrome_options=options)
+            driver = webdriver.Chrome(driver_path, options=chrome_options)
         driver.get(Link)
         return driver
 
 
 
 class Browsers:
     def firefox_b(url):
@@ -124,17 +126,26 @@
                     break
                 except:
                     print(error_message)
                     sleep(1)
                     continue
     
 
+# from Omar_Style_sel import BrowsersProxy as Br
+
+# pr = BrowsersProxy()
+# # driver = pr.proxy_firefox("74.249.8.183:3128", "http://whatismyipaddress.com")
 
+# driver = pr.proxy_chrome("103.168.44.41:9191","https://youtu.be/hCtg283iJKg",False)
+# sleep(1000)
 
+# dd = Browsers.chrome_b ("https://youtu.be/Qq5bVHRQ7zQ")
+# dd.get("https://accounts.google.com/InteractiveLogin/identifier?continue=https%3A%2F%2Fwww.google.com%2F%3Fhl%3Den-US&ec=GAZAmgQ&hl=en&passive=true&ifkv=Af_xneFkB3tG1PGehWiTNPJ0nlCIMbZbRppbIXYIEkdJU-FhTAbL__UJYdBZQn7UOhNhtNJL-lei&flowName=GlifWebSignIn&flowEntry=ServiceLogin")
 
+   
 # dd = Browsers.chrome_b("https://youtu.be/Qq5bVHRQ7zQ")
 # # print(dd)
 # # Browsers.input_a(dd,By.XPATH,'//*[@id="APjFqb"]',"python","SSSS","Eeee")
 # Browsers.click_a(dd, By.XPATH, '//*[@id="segmented-like-button"]/ytd-toggle-button-renderer/yt-button-shape/button/yt-touch-feedback-shape/div/div[2]', "SSS", "EEEE")
 
 # # Browsers.click_a(dd,By.XPATH,'//*[@id="segmented-like-button"]/ytd-toggle-button-renderer/yt-button-shape/button/yt-touch-feedback-shape/div/div[2]',"SSS","EEEE")
 # # pr = BrowsersProxy()
```

### Comparing `Omar_Style_sel-0.5/Omar_Style_sel.egg-info/PKG-INFO` & `Omar_Style_sel-0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Omar-Style-sel
-Version: 0.5
+Name: Omar_Style_sel
+Version: 0.6
 Summary: Omar_Style _ 〄🇵🇸
 Home-page: https://github.com/Omarail1/omarpoop.git
 Author: omar Style
 Author-email: omarllStyle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -44,32 +44,46 @@
 
 ___
 
 ## Library use:
 
 Here I use Firefox and Google Chrome browsers only
 
+##### The library has been updated and new features have been added such as :: => user_agent    
+
+
+If you want to use this feature, all you have to do is write it  ===> True 
+
+```python 
+ from Omar_Style_sel import BrowsersProxy as Br
+
+    pr = Br()
+
+    driver = pr.proxy_chrome("103.168.44.41:9191","https://youtu.be/hCtg283iJKg",False)
+```
+---
 
 ``` python
    
    from Omar_Style_sel import BrowsersProxy as Br
 
     pr = Br()
     driver = pr.proxy_firefox("74.249.8.183:3128", "http://whatismyipaddress.com")
 
-    driver = pr.proxy_chrome("95.56.254.139:3128","http://whatismyipaddress.com")
+   
+    driver = pr.proxy_chrome("103.168.44.41:9191","https://youtu.be/hCtg283iJKg",False)
 
 ```
 ____
 #### Here you can only use Google Chrome, but you have to download it to your computer and then use it :
 
 ##This is the example to illustrate
 
 ``` python 
-driver = pr.proxy_chrome("95.56.254.139:3128","http://whatismyipaddress.com", driver_path='E:\\chroo\\chromedriver.exe')
+driver = pr.proxy_chrome("95.56.254.139:3128","http://whatismyipaddress.com",False, driver_path='E:\\chroo\\chromedriver.exe')
 ```
 ____
 
 
 ## Any problem contact us
 [Telegram](https://t.me/OmarStyle1)
```

### Comparing `Omar_Style_sel-0.5/PKG-INFO` & `Omar_Style_sel-0.6/Omar_Style_sel.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Omar_Style_sel
-Version: 0.5
+Name: Omar-Style-sel
+Version: 0.6
 Summary: Omar_Style _ 〄🇵🇸
 Home-page: https://github.com/Omarail1/omarpoop.git
 Author: omar Style
 Author-email: omarllStyle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -44,32 +44,46 @@
 
 ___
 
 ## Library use:
 
 Here I use Firefox and Google Chrome browsers only
 
+##### The library has been updated and new features have been added such as :: => user_agent    
+
+
+If you want to use this feature, all you have to do is write it  ===> True 
+
+```python 
+ from Omar_Style_sel import BrowsersProxy as Br
+
+    pr = Br()
+
+    driver = pr.proxy_chrome("103.168.44.41:9191","https://youtu.be/hCtg283iJKg",False)
+```
+---
 
 ``` python
    
    from Omar_Style_sel import BrowsersProxy as Br
 
     pr = Br()
     driver = pr.proxy_firefox("74.249.8.183:3128", "http://whatismyipaddress.com")
 
-    driver = pr.proxy_chrome("95.56.254.139:3128","http://whatismyipaddress.com")
+   
+    driver = pr.proxy_chrome("103.168.44.41:9191","https://youtu.be/hCtg283iJKg",False)
 
 ```
 ____
 #### Here you can only use Google Chrome, but you have to download it to your computer and then use it :
 
 ##This is the example to illustrate
 
 ``` python 
-driver = pr.proxy_chrome("95.56.254.139:3128","http://whatismyipaddress.com", driver_path='E:\\chroo\\chromedriver.exe')
+driver = pr.proxy_chrome("95.56.254.139:3128","http://whatismyipaddress.com",False, driver_path='E:\\chroo\\chromedriver.exe')
 ```
 ____
 
 
 ## Any problem contact us
 [Telegram](https://t.me/OmarStyle1)
```

### Comparing `Omar_Style_sel-0.5/README.md` & `Omar_Style_sel-0.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -28,32 +28,46 @@
 
 ___
 
 ## Library use:
 
 Here I use Firefox and Google Chrome browsers only
 
+##### The library has been updated and new features have been added such as :: => user_agent    
+
+
+If you want to use this feature, all you have to do is write it  ===> True 
+
+```python 
+ from Omar_Style_sel import BrowsersProxy as Br
+
+    pr = Br()
+
+    driver = pr.proxy_chrome("103.168.44.41:9191","https://youtu.be/hCtg283iJKg",False)
+```
+---
 
 ``` python
    
    from Omar_Style_sel import BrowsersProxy as Br
 
     pr = Br()
     driver = pr.proxy_firefox("74.249.8.183:3128", "http://whatismyipaddress.com")
 
-    driver = pr.proxy_chrome("95.56.254.139:3128","http://whatismyipaddress.com")
+   
+    driver = pr.proxy_chrome("103.168.44.41:9191","https://youtu.be/hCtg283iJKg",False)
 
 ```
 ____
 #### Here you can only use Google Chrome, but you have to download it to your computer and then use it :
 
 ##This is the example to illustrate
 
 ``` python 
-driver = pr.proxy_chrome("95.56.254.139:3128","http://whatismyipaddress.com", driver_path='E:\\chroo\\chromedriver.exe')
+driver = pr.proxy_chrome("95.56.254.139:3128","http://whatismyipaddress.com",False, driver_path='E:\\chroo\\chromedriver.exe')
 ```
 ____
 
 
 ## Any problem contact us
 [Telegram](https://t.me/OmarStyle1)
```

### Comparing `Omar_Style_sel-0.5/setup.py` & `Omar_Style_sel-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 # with open('requirements.txt','r') as fr:
 #     requires = fr.read().split('\n')
 
 setuptools.setup(
     name='Omar_Style_sel',
-    version="0.5",
+    version="0.6",
     author='omar Style',
     author_email='omarllStyle@gmail.com',
     description='Omar_Style _ 〄🇵🇸',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Omarail1/omarpoop.git',
     packages=['Omar_Style_sel'],
```

