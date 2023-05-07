# Comparing `tmp/evina-1.0.5.tar.gz` & `tmp/evina-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\evina-1.0.5.tar", last modified: Sun May  7 15:36:25 2023, max compression
+gzip compressed data, was "dist\evina-1.0.6.tar", last modified: Sun May  7 16:06:11 2023, max compression
```

## Comparing `evina-1.0.5.tar` & `evina-1.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 15:36:25.527125 evina-1.0.5/
--rw-rw-rw-   0        0        0     1083 2023-05-02 16:19:36.000000 evina-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       47 2023-05-07 06:53:08.000000 evina-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0       90 2023-05-07 15:36:25.526126 evina-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2023-05-02 16:19:36.000000 evina-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 15:36:25.468651 evina-1.0.5/evina/
--rw-rw-rw-   0        0        0       90 2023-05-07 06:53:08.000000 evina-1.0.5/evina/__init__.py
--rw-rw-rw-   0        0        0      720 2023-05-07 06:53:08.000000 evina-1.0.5/evina/alipan.py
--rw-rw-rw-   0        0        0     4987 2023-05-07 15:06:11.000000 evina-1.0.5/evina/config.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:36:25.523136 evina-1.0.5/evina/disposition/
--rw-rw-rw-   0        0        0        0 2023-05-07 06:53:08.000000 evina-1.0.5/evina/disposition/__init__.py
--rw-rw-rw-   0        0        0     1135 2023-05-07 13:48:35.000000 evina-1.0.5/evina/disposition/config.conf
--rw-rw-rw-   0        0        0      101 2023-05-07 06:53:08.000000 evina-1.0.5/evina/disposition/evina.conf
--rw-rw-rw-   0        0        0    14673 2023-05-07 15:32:16.000000 evina-1.0.5/evina/douyin.py
--rw-rw-rw-   0        0        0    10237 2023-05-07 15:35:33.000000 evina-1.0.5/evina/douyu.py
--rw-rw-rw-   0        0        0     1687 2023-05-07 15:14:15.000000 evina-1.0.5/evina/evina.py
--rw-rw-rw-   0        0        0      955 2023-05-05 16:33:43.000000 evina-1.0.5/evina/replacement.py
--rw-rw-rw-   0        0        0     1342 2023-05-07 06:53:08.000000 evina-1.0.5/evina/ssh.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:36:25.517152 evina-1.0.5/evina.egg-info/
--rw-rw-rw-   0        0        0       90 2023-05-07 15:36:25.000000 evina-1.0.5/evina.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-05-07 15:36:25.000000 evina-1.0.5/evina.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 15:36:25.000000 evina-1.0.5/evina.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-07 15:36:25.000000 evina-1.0.5/evina.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-05-07 15:36:25.000000 evina-1.0.5/evina.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-07 15:36:25.000000 evina-1.0.5/evina.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 15:36:25.527125 evina-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-05-07 15:35:43.000000 evina-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:06:11.386566 evina-1.0.6/
+-rw-rw-rw-   0        0        0     1083 2023-05-02 16:19:36.000000 evina-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0       47 2023-05-07 06:53:08.000000 evina-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0       90 2023-05-07 16:06:11.384567 evina-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2023-05-02 16:19:36.000000 evina-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 16:06:11.251625 evina-1.0.6/evina/
+-rw-rw-rw-   0        0        0       90 2023-05-07 06:53:08.000000 evina-1.0.6/evina/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-05-07 06:53:08.000000 evina-1.0.6/evina/alipan.py
+-rw-rw-rw-   0        0        0     4991 2023-05-07 16:05:10.000000 evina-1.0.6/evina/config.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:06:11.381574 evina-1.0.6/evina/disposition/
+-rw-rw-rw-   0        0        0        0 2023-05-07 06:53:08.000000 evina-1.0.6/evina/disposition/__init__.py
+-rw-rw-rw-   0        0        0     1135 2023-05-07 13:48:35.000000 evina-1.0.6/evina/disposition/config.conf
+-rw-rw-rw-   0        0        0      101 2023-05-07 06:53:08.000000 evina-1.0.6/evina/disposition/evina.conf
+-rw-rw-rw-   0        0        0    14673 2023-05-07 15:32:16.000000 evina-1.0.6/evina/douyin.py
+-rw-rw-rw-   0        0        0    10237 2023-05-07 15:35:33.000000 evina-1.0.6/evina/douyu.py
+-rw-rw-rw-   0        0        0     1641 2023-05-07 15:59:50.000000 evina-1.0.6/evina/evina.py
+-rw-rw-rw-   0        0        0      955 2023-05-05 16:33:43.000000 evina-1.0.6/evina/replacement.py
+-rw-rw-rw-   0        0        0     1342 2023-05-07 06:53:08.000000 evina-1.0.6/evina/ssh.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:06:11.362649 evina-1.0.6/evina.egg-info/
+-rw-rw-rw-   0        0        0       90 2023-05-07 16:06:11.000000 evina-1.0.6/evina.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-05-07 16:06:11.000000 evina-1.0.6/evina.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 16:06:11.000000 evina-1.0.6/evina.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-07 16:06:11.000000 evina-1.0.6/evina.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-05-07 16:06:11.000000 evina-1.0.6/evina.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-07 16:06:11.000000 evina-1.0.6/evina.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 16:06:11.386566 evina-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-05-07 16:05:59.000000 evina-1.0.6/setup.py
```

### Comparing `evina-1.0.5/LICENSE` & `evina-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `evina-1.0.5/README.md` & `evina-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `evina-1.0.5/evina/alipan.py` & `evina-1.0.6/evina/alipan.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.5/evina/config.py` & `evina-1.0.6/evina/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self.evina_douyin = Dynaconf(envvar_prefix='douyin',
                                      load_dotenv=True,
                                      dotenv_path=evina_file,
                                      dotenv_override=True)
 
         replacement.Auth._EMAIL_USER = self.default.settings.email_user
         replacement.Auth._EMAIL_PASSWORD = self.default.settings.email_password
-        email_host = replacement.Auth._EMAIL_USER.split('@')[1].split('.')
+        email_host = self.default.settings.email_user.split('@')[1].split('.')
         replacement.Auth._EMAIL_HOST = 'smtp.{}.{}'.format(
             email_host[0], email_host[1])
         Aligo(email=(self.default.settings.email_user, '阿里云盘登录二维码验证'))
 
 
 class Arg(Conf):
     def __init__(self) -> None:
```

### Comparing `evina-1.0.5/evina/disposition/config.conf` & `evina-1.0.6/evina/disposition/config.conf`

 * *Files identical despite different names*

### Comparing `evina-1.0.5/evina/douyin.py` & `evina-1.0.6/evina/douyin.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.5/evina/douyu.py` & `evina-1.0.6/evina/douyu.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.5/evina/evina.py` & `evina-1.0.6/evina/evina.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,10 +43,9 @@
                 return True
         return False
 
 
 def start():
     while True:
         sleep = config.Conf().conf.settings.sleep
-        print(config.Conf().evina_douyu.url)
         Evina()
         time.sleep(sleep)
```

### Comparing `evina-1.0.5/evina/replacement.py` & `evina-1.0.6/evina/replacement.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.5/evina/ssh.py` & `evina-1.0.6/evina/ssh.py`

 * *Files identical despite different names*

