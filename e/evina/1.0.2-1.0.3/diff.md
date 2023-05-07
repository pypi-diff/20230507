# Comparing `tmp/evina-1.0.2.tar.gz` & `tmp/evina-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\evina-1.0.2.tar", last modified: Fri May  5 16:39:18 2023, max compression
+gzip compressed data, was "dist\evina-1.0.3.tar", last modified: Sun May  7 15:23:13 2023, max compression
```

## Comparing `evina-1.0.2.tar` & `evina-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 16:39:18.332053 evina-1.0.2/
--rw-rw-rw-   0        0        0     1083 2023-05-02 16:19:36.000000 evina-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       47 2023-05-05 16:32:20.000000 evina-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0       90 2023-05-05 16:39:18.331054 evina-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2023-05-02 16:19:36.000000 evina-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 16:39:18.309112 evina-1.0.2/evina/
--rw-rw-rw-   0        0        0       90 2023-05-05 16:32:20.000000 evina-1.0.2/evina/__init__.py
--rw-rw-rw-   0        0        0      720 2023-05-05 16:32:20.000000 evina-1.0.2/evina/alipan.py
--rw-rw-rw-   0        0        0     4757 2023-05-05 16:33:18.000000 evina-1.0.2/evina/config.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:39:18.327065 evina-1.0.2/evina/disposition/
--rw-rw-rw-   0        0        0        0 2023-05-05 16:32:20.000000 evina-1.0.2/evina/disposition/__init__.py
--rw-rw-rw-   0        0        0     1135 2023-05-05 16:34:25.000000 evina-1.0.2/evina/disposition/config.conf
--rw-rw-rw-   0        0        0      101 2023-05-05 16:32:20.000000 evina-1.0.2/evina/disposition/evina.conf
--rw-rw-rw-   0        0        0    14557 2023-05-05 16:32:20.000000 evina-1.0.2/evina/douyin.py
--rw-rw-rw-   0        0        0     9388 2023-05-05 16:32:20.000000 evina-1.0.2/evina/douyu.py
--rw-rw-rw-   0        0        0     1559 2023-05-05 16:32:20.000000 evina-1.0.2/evina/evina.py
--rw-rw-rw-   0        0        0      955 2023-05-05 16:33:43.000000 evina-1.0.2/evina/replacement.py
--rw-rw-rw-   0        0        0     1342 2023-05-05 16:32:20.000000 evina-1.0.2/evina/ssh.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:39:18.322078 evina-1.0.2/evina.egg-info/
--rw-rw-rw-   0        0        0       90 2023-05-05 16:39:18.000000 evina-1.0.2/evina.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-05-05 16:39:18.000000 evina-1.0.2/evina.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 16:39:18.000000 evina-1.0.2/evina.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-05 16:39:18.000000 evina-1.0.2/evina.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-05-05 16:39:18.000000 evina-1.0.2/evina.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-05 16:39:18.000000 evina-1.0.2/evina.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 16:39:18.333050 evina-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-05-05 16:35:33.000000 evina-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:23:13.886379 evina-1.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-05-02 16:19:36.000000 evina-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       47 2023-05-07 06:53:08.000000 evina-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0       90 2023-05-07 15:23:13.885374 evina-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2023-05-02 16:19:36.000000 evina-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 15:23:13.866426 evina-1.0.3/evina/
+-rw-rw-rw-   0        0        0       90 2023-05-07 06:53:08.000000 evina-1.0.3/evina/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-05-07 06:53:08.000000 evina-1.0.3/evina/alipan.py
+-rw-rw-rw-   0        0        0     4987 2023-05-07 15:06:11.000000 evina-1.0.3/evina/config.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:23:13.882382 evina-1.0.3/evina/disposition/
+-rw-rw-rw-   0        0        0        0 2023-05-07 06:53:08.000000 evina-1.0.3/evina/disposition/__init__.py
+-rw-rw-rw-   0        0        0     1135 2023-05-07 13:48:35.000000 evina-1.0.3/evina/disposition/config.conf
+-rw-rw-rw-   0        0        0      101 2023-05-07 06:53:08.000000 evina-1.0.3/evina/disposition/evina.conf
+-rw-rw-rw-   0        0        0    14649 2023-05-07 15:17:12.000000 evina-1.0.3/evina/douyin.py
+-rw-rw-rw-   0        0        0    10173 2023-05-07 15:21:43.000000 evina-1.0.3/evina/douyu.py
+-rw-rw-rw-   0        0        0     1687 2023-05-07 15:14:15.000000 evina-1.0.3/evina/evina.py
+-rw-rw-rw-   0        0        0      955 2023-05-05 16:33:43.000000 evina-1.0.3/evina/replacement.py
+-rw-rw-rw-   0        0        0     1342 2023-05-07 06:53:08.000000 evina-1.0.3/evina/ssh.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:23:13.878393 evina-1.0.3/evina.egg-info/
+-rw-rw-rw-   0        0        0       90 2023-05-07 15:23:13.000000 evina-1.0.3/evina.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-05-07 15:23:13.000000 evina-1.0.3/evina.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 15:23:13.000000 evina-1.0.3/evina.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-07 15:23:13.000000 evina-1.0.3/evina.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-05-07 15:23:13.000000 evina-1.0.3/evina.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-07 15:23:13.000000 evina-1.0.3/evina.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 15:23:13.886379 evina-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-05-07 15:22:44.000000 evina-1.0.3/setup.py
```

### Comparing `evina-1.0.2/LICENSE` & `evina-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `evina-1.0.2/README.md` & `evina-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `evina-1.0.2/evina/alipan.py` & `evina-1.0.3/evina/alipan.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.2/evina/config.py` & `evina-1.0.3/evina/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,19 @@
 
         parse = argparse.ArgumentParser()
         parse.add_argument('--start', '-s', nargs=1, help='选择需要录制的平台。')
         parse.add_argument('--url', '-u', nargs='*', help='需要录制的直播间URL/ID。')
         parse.add_argument('--name', '-n', nargs='*', help='自定义文件夹名称')
         self.arg = parse.parse_args()
 
+        self.default = Dynaconf(envvar_prefix='evina',
+                                load_dotenv=True,
+                                dotenv_path=conf_file,
+                                dotenv_override=False)
+
         self.conf = Dynaconf(envvar_prefix='evina',
                              load_dotenv=True,
                              dotenv_path=conf_file,
                              dotenv_override=True)
 
         self.evina_douyu = Dynaconf(envvar_prefix='douyu',
                                     load_dotenv=True,
@@ -44,20 +49,20 @@
                                     dotenv_override=True)
 
         self.evina_douyin = Dynaconf(envvar_prefix='douyin',
                                      load_dotenv=True,
                                      dotenv_path=evina_file,
                                      dotenv_override=True)
 
-        replacement.Auth._EMAIL_USER = self.conf.settings.email_user
-        replacement.Auth._EMAIL_PASSWORD = self.conf.settings.email_password
+        replacement.Auth._EMAIL_USER = self.default.settings.email_user
+        replacement.Auth._EMAIL_PASSWORD = self.default.settings.email_password
         email_host = replacement.Auth._EMAIL_USER.split('@')[1].split('.')
         replacement.Auth._EMAIL_HOST = 'smtp.{}.{}'.format(
             email_host[0], email_host[1])
-        Aligo(email=(self.conf.settings.email_user, '阿里云盘登录二维码验证'))
+        Aligo(email=(self.default.settings.email_user, '阿里云盘登录二维码验证'))
 
 
 class Arg(Conf):
     def __init__(self) -> None:
         super().__init__()
         if self.arg.start != None:
             self.start = self.arg.start[0]
```

### Comparing `evina-1.0.2/evina/disposition/config.conf` & `evina-1.0.3/evina/disposition/config.conf`

 * *Files identical despite different names*

### Comparing `evina-1.0.2/evina/douyin.py` & `evina-1.0.3/evina/douyin.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 import requests
 from evina import ssh
 from faker import Faker
 from loguru import logger
 
 
 class Douyin:
-    def __init__(self, name, settings, uid=None):
+    def __init__(self, name, settings, default_settings, uid=None):
         logger.info('线程创建成功 | 线程名 - {} | PID - {}'.format(
             threading.current_thread().name,
             threading.current_thread().ident))
         self.name = name
         self.settings = settings
-        self.open = self.settings.open
+        self.default_settings = default_settings
+        self.open = self.default_settings.open
         self.ua = Faker(locale="zh_CN").user_agent()
 
         if uid == None:
             sys.exit()
         if uid.endswith('/'):
             uid = uid.rsplit('/', 1)[0]
         uid = uid.rsplit('/', 1)
@@ -111,25 +112,25 @@
                 logger.info('抖音直播间 - {} - {} | 已成功保存直播源地址到文件'.format(
                     name,
                     url.rsplit('/', 1)[1]))
             if self.open:
                 logger.info('抖音直播间 - {} - {} 开始录制'.format(
                     name,
                     url.rsplit('/', 1)[1]))
-                if self.settings.docker == False:
+                if self.default_settings.docker == False:
                     subout = subprocess.run(
                         "ffmpeg -i " + '"{}"'.format(list[0]) +
                         " -c:a copy -c:v copy -bsf:a aac_adtstoasc -threads {} -preset {} -f {}  -f segment -segment_time {} -strftime 1 "
                         .format(str(self.settings.thread),
                                 self.settings.preset, self.settings.scheme,
                                 str(self.settings.time)) +
                         '"{}"'.format(
                             os.path.join(file, '%Y-%m-%d-%H-%M-%S.ts')))
                     logger.info(subout)
-                if self.settings.docker == True:
+                if self.default_settings.docker == True:
                     ssh.Ssh(list[0], os.path.join(file,
                                                   '%Y-%m-%d-%H-%M-%S.ts'),
                             self.settings)
                     alipan.Backup(local_file=file, ali_file=ali_file)
                     shutil.rmtree(
                         os.path.join(
                             os.path.abspath(
```

### Comparing `evina-1.0.2/evina/douyu.py` & `evina-1.0.3/evina/douyu.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,29 @@
 import re
 import shutil
 import subprocess
 import sys
 import threading
 import time
 
-from evina import alipan
 import requests
-from evina import ssh
 from faker import Faker
 from loguru import logger
 
+from evina import alipan, ssh
+
 
 class Douyu:
-    def __init__(self, rid, name, settings):
+    def __init__(self, rid, name, settings, default_settings):
         logger.info('线程创建成功 | 线程名 - {} | PID - {}'.format(
             threading.current_thread().name,
             threading.current_thread().ident))
         self.settings = settings
-        self.open = self.settings.open
+        self.default_settings = default_settings
+        self.open = self.default_settings.open
         self.name = name
         self.rid = rid
         self.ua = Faker(locale="zh_CN").user_agent()
         try:
             self.api()
         except:
             self.data = self.js()
@@ -70,25 +71,25 @@
             logger.info('斗鱼直播间 - {} | 源地址为 - {}'.format(self.rid, link))
             if self.open == False:
                 logger.info('斗鱼直播间 - {} - {} | 已成功保存直播源地址到文件'.format(
                     filename, self.rid))
 
             if self.open:
                 logger.info('斗鱼直播间 - {} - {} 开始录制'.format(filename, self.rid))
-                if self.settings.docker == False:
+                if self.default_settings.docker == False:
                     subout = subprocess.run(
                         "ffmpeg -i " + '"{}"'.format(link) +
                         " -c:a copy -c:v copy -bsf:a aac_adtstoasc -threads {} -preset {} -f {}  -f segment -segment_time {} -strftime 1 "
                         .format(str(self.settings.thread),
                                 self.settings.preset, self.settings.scheme,
                                 str(self.settings.time)) +
                         '"{}"'.format(
                             os.path.join(file, '%Y-%m-%d-%H-%M-%S.ts')))
                     logger.info(subout)
-                if self.settings.docker == True:
+                if self.default_settings.docker == True:
                     ssh.Ssh(link, os.path.join(file, '%Y-%m-%d-%H-%M-%S.ts'),
                             self.settings)
                     alipan.Backup(local_file=file, ali_file=ali_file)
                     shutil.rmtree(
                         os.path.join(
                             os.path.abspath(
                                 os.path.join(os.path.dirname(__file__), '..')),
@@ -98,16 +99,20 @@
         file = os.path.join(
             os.path.dirname(__file__),
             str(datetime.datetime.now()).replace(':', '-') + '.js')
         jstime = str(int(time.time()))
         did = '10000000000000000000000000001501'
         url = 'https://www.douyu.com/{}'.format(self.rid)
         response = requests.get(url=url)
-        try:self.rid = re.findall(r'ROOM.room_id =(\d+)', response.text, re.S)[0]
-        except:self.rid = re.findall(r'ROOM.room_id = (\d+)', response.text, re.S)[0]
+        try:
+            self.rid = re.findall(r'ROOM.room_id =(\d+)', response.text,
+                                  re.S)[0]
+        except:
+            self.rid = re.findall(r'ROOM.room_id = (\d+)', response.text,
+                                  re.S)[0]
         jsdate = re.findall(
             r'<script type="text/javascript">.*?var vdwdae325w_64we = .*?;(.*?)</script>',
             response.text, re.S)[0]
         # js = 'module.paths.push("D:/node/node_modules");const CryptoJS = require("crypto-js");' + jsdate + \
         #     "let arguments=process.argv.splice(2).join('').split(',');for(var i = 0; i < arguments.length; i++) {}console.log(ub98484234(arguments[0],arguments[1],arguments[2]))"
         js = 'module.paths.push("{}");const CryptoJS = require("crypto-js");'.format(self.settings.node_modules) + jsdate + \
             "let arguments=process.argv.splice(2).join('').split(',');for(var i = 0; i < arguments.length; i++) {}console.log(ub98484234(arguments[0],arguments[1],arguments[2]))"
@@ -148,15 +153,17 @@
             self.ua
         }
         response = requests.post(url=url, headers=headers, data=self.data)
         if response.status_code != 200:
             logger.info('斗鱼直播间 - {} | 暂未开播'.format(self.rid))
             sys.exit()
         data = json.loads(response.text)
-        if '房间未开播' in data.values():logger.info('斗鱼直播间 - {} | 暂未开播'.format(self.rid));sys.exit()
+        if '房间未开播' in data.values():
+            logger.info('斗鱼直播间 - {} | 暂未开播'.format(self.rid))
+            sys.exit()
         rtmp_url = data['data']['rtmp_url']
         rtmp_live = data['data']['rtmp_live']
         rea_rid = rtmp_live.split('?')[0]
         http = os.path.join(random.choice(['http://hdltc1.douyucdn.cn/live', 'http://hw-tct.douyucdn.cn/live']))  \
             + '/' + rea_rid
         if self.name == None:
             name = self.get_name()
@@ -174,22 +181,31 @@
         f.write(http)
         f.close()
         logger.info('斗鱼直播间 - {} - {} | 源地址为 - {}'.format(name, self.rid, http))
         if self.open == False:
             logger.info('已成功保存直播源地址到文件')
         if self.open:
             logger.info('斗鱼直播间 - {} - {} 开始录制'.format(name, self.rid))
-            # os.system('ffmpeg -i "{}" -c:v copy -c:a copy "{}"'.format(link, file))
-            ssh.Ssh(http, os.path.join(file, '%Y-%m-%d-%H-%M-%S.ts'), self.settings)
-            alipan.Backup(local_file=file, ali_file=ali_file)
-            shutil.rmtree(
-                os.path.join(
-                    os.path.abspath(
-                        os.path.join(os.path.dirname(__file__), '..')),
-                    'download', '斗鱼录播', name))
+            if self.default_settings.docker == False:
+                subout = subprocess.run(
+                    "ffmpeg -i " + '"{}"'.format(http) +
+                    " -c:a copy -c:v copy -bsf:a aac_adtstoasc -threads {} -preset {} -f {}  -f segment -segment_time {} -strftime 1 "
+                    .format(str(self.settings.thread), self.settings.preset,
+                            self.settings.scheme, str(self.settings.time)) +
+                    '"{}"'.format(os.path.join(file, '%Y-%m-%d-%H-%M-%S.ts')))
+                logger.info(subout)
+            if self.default_settings.docker == True:
+                ssh.Ssh(http, os.path.join(file, '%Y-%m-%d-%H-%M-%S.ts'),
+                        self.settings)
+                alipan.Backup(local_file=file, ali_file=ali_file)
+                shutil.rmtree(
+                    os.path.join(
+                        os.path.abspath(
+                            os.path.join(os.path.dirname(__file__), '..')),
+                        'download', '斗鱼录播', name))
 
     def get_name(self):
         url = 'https://www.douyu.com/betard/{}'.format(self.rid)
         headers = {
             'accept':
             'application/json, text/plain, */*',
             'accept-language':
```

### Comparing `evina-1.0.2/evina/evina.py` & `evina-1.0.3/evina/evina.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,36 +22,31 @@
         for start in self.dict:
             if start == 'douyu':
                 for url, name in self.dict[start].items():
                     if 'http' in url and not url.endswith('/'):
                         url = url.rsplit('/', 1)[1]
                     if not self.check(url):
                         threading.Thread(target=douyu.Douyu,
-                                         args=(url, name, self.conf.settings),
+                                         args=(url, name, self.conf.settings,
+                                               self.default.settings),
                                          name=url).start()
             if start == 'douyin':
                 for url, name in self.dict[start].items():
                     if not self.check(str(url)):
                         threading.Thread(target=douyin.Douyin,
-                                         args=(name, self.conf.settings, url),
+                                         args=(name, self.conf.settings,
+                                               self.default.settings, url),
                                          name=url).start()
 
     def check(self, name):
         for thread in threading.enumerate():
             if name == thread.name:
                 return True
         return False
 
+
 def start():
     while True:
         sleep = config.Conf().conf.settings.sleep
         print(config.Conf().evina_douyu.url)
         Evina()
         time.sleep(sleep)
-
-
-
-
-
-
-
-
```

### Comparing `evina-1.0.2/evina/replacement.py` & `evina-1.0.3/evina/replacement.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.2/evina/ssh.py` & `evina-1.0.3/evina/ssh.py`

 * *Files identical despite different names*

