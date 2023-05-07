# Comparing `tmp/evina-1.0.3.tar.gz` & `tmp/evina-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\evina-1.0.3.tar", last modified: Sun May  7 15:23:13 2023, max compression
+gzip compressed data, was "dist\evina-1.0.4.tar", last modified: Sun May  7 15:33:05 2023, max compression
```

## Comparing `evina-1.0.3.tar` & `evina-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 15:23:13.886379 evina-1.0.3/
--rw-rw-rw-   0        0        0     1083 2023-05-02 16:19:36.000000 evina-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       47 2023-05-07 06:53:08.000000 evina-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0       90 2023-05-07 15:23:13.885374 evina-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2023-05-02 16:19:36.000000 evina-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 15:23:13.866426 evina-1.0.3/evina/
--rw-rw-rw-   0        0        0       90 2023-05-07 06:53:08.000000 evina-1.0.3/evina/__init__.py
--rw-rw-rw-   0        0        0      720 2023-05-07 06:53:08.000000 evina-1.0.3/evina/alipan.py
--rw-rw-rw-   0        0        0     4987 2023-05-07 15:06:11.000000 evina-1.0.3/evina/config.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:23:13.882382 evina-1.0.3/evina/disposition/
--rw-rw-rw-   0        0        0        0 2023-05-07 06:53:08.000000 evina-1.0.3/evina/disposition/__init__.py
--rw-rw-rw-   0        0        0     1135 2023-05-07 13:48:35.000000 evina-1.0.3/evina/disposition/config.conf
--rw-rw-rw-   0        0        0      101 2023-05-07 06:53:08.000000 evina-1.0.3/evina/disposition/evina.conf
--rw-rw-rw-   0        0        0    14649 2023-05-07 15:17:12.000000 evina-1.0.3/evina/douyin.py
--rw-rw-rw-   0        0        0    10173 2023-05-07 15:21:43.000000 evina-1.0.3/evina/douyu.py
--rw-rw-rw-   0        0        0     1687 2023-05-07 15:14:15.000000 evina-1.0.3/evina/evina.py
--rw-rw-rw-   0        0        0      955 2023-05-05 16:33:43.000000 evina-1.0.3/evina/replacement.py
--rw-rw-rw-   0        0        0     1342 2023-05-07 06:53:08.000000 evina-1.0.3/evina/ssh.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:23:13.878393 evina-1.0.3/evina.egg-info/
--rw-rw-rw-   0        0        0       90 2023-05-07 15:23:13.000000 evina-1.0.3/evina.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-05-07 15:23:13.000000 evina-1.0.3/evina.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 15:23:13.000000 evina-1.0.3/evina.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-07 15:23:13.000000 evina-1.0.3/evina.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-05-07 15:23:13.000000 evina-1.0.3/evina.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-07 15:23:13.000000 evina-1.0.3/evina.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 15:23:13.886379 evina-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-05-07 15:22:44.000000 evina-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:33:05.609373 evina-1.0.4/
+-rw-rw-rw-   0        0        0     1083 2023-05-02 16:19:36.000000 evina-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       47 2023-05-07 06:53:08.000000 evina-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0       90 2023-05-07 15:33:05.608398 evina-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2023-05-02 16:19:36.000000 evina-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 15:33:05.559391 evina-1.0.4/evina/
+-rw-rw-rw-   0        0        0       90 2023-05-07 06:53:08.000000 evina-1.0.4/evina/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-05-07 06:53:08.000000 evina-1.0.4/evina/alipan.py
+-rw-rw-rw-   0        0        0     4987 2023-05-07 15:06:11.000000 evina-1.0.4/evina/config.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:33:05.606380 evina-1.0.4/evina/disposition/
+-rw-rw-rw-   0        0        0        0 2023-05-07 06:53:08.000000 evina-1.0.4/evina/disposition/__init__.py
+-rw-rw-rw-   0        0        0     1135 2023-05-07 13:48:35.000000 evina-1.0.4/evina/disposition/config.conf
+-rw-rw-rw-   0        0        0      101 2023-05-07 06:53:08.000000 evina-1.0.4/evina/disposition/evina.conf
+-rw-rw-rw-   0        0        0    14673 2023-05-07 15:32:16.000000 evina-1.0.4/evina/douyin.py
+-rw-rw-rw-   0        0        0    10221 2023-05-07 15:32:44.000000 evina-1.0.4/evina/douyu.py
+-rw-rw-rw-   0        0        0     1687 2023-05-07 15:14:15.000000 evina-1.0.4/evina/evina.py
+-rw-rw-rw-   0        0        0      955 2023-05-05 16:33:43.000000 evina-1.0.4/evina/replacement.py
+-rw-rw-rw-   0        0        0     1342 2023-05-07 06:53:08.000000 evina-1.0.4/evina/ssh.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:33:05.598402 evina-1.0.4/evina.egg-info/
+-rw-rw-rw-   0        0        0       90 2023-05-07 15:33:05.000000 evina-1.0.4/evina.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-05-07 15:33:05.000000 evina-1.0.4/evina.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 15:33:05.000000 evina-1.0.4/evina.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-07 15:33:05.000000 evina-1.0.4/evina.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-05-07 15:33:05.000000 evina-1.0.4/evina.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-07 15:33:05.000000 evina-1.0.4/evina.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 15:33:05.609373 evina-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-05-07 15:32:52.000000 evina-1.0.4/setup.py
```

### Comparing `evina-1.0.3/LICENSE` & `evina-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `evina-1.0.3/README.md` & `evina-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `evina-1.0.3/evina/alipan.py` & `evina-1.0.4/evina/alipan.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.3/evina/config.py` & `evina-1.0.4/evina/config.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.3/evina/disposition/config.conf` & `evina-1.0.4/evina/disposition/config.conf`

 * *Files identical despite different names*

### Comparing `evina-1.0.3/evina/douyin.py` & `evina-1.0.4/evina/douyin.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,16 @@
             for key, value in flv_pull_url.items():
                 flv_list.append(value)
             hls_pull_url_map = stream_url['hls_pull_url_map']
             for key, value in hls_pull_url_map.items():
                 m3u8_list.append(value)
             list = flv_list + m3u8_list
             time = datetime.datetime.now().ctime().replace(':', '-')
-            if 'FILE' in self.settings.keys() and self.settings.file != '':
-                file = os.path.join(self.settings.file, 'download', '抖音录播',
+            if 'FILE' in self.default_settings.keys() and self.default_settings.file != '':
+                file = os.path.join(self.default_settings.file, 'download', '抖音录播',
                                     name, time)
             else:
                 file = os.path.join(os.getcwd(), 'download', '抖音录播', name,
                                     time)
             ali_file = os.path.join('录播', '抖音录播', name,
                                     time).replace('\\', '/')
             if not os.path.exists(file):
```

### Comparing `evina-1.0.3/evina/douyu.py` & `evina-1.0.4/evina/douyu.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
         if self.response['state'] == 'SUCCESS':
             if self.name == None:
                 filename = self.response['Rendata']['data']['nickname']
             else:
                 filename = self.name
             # time = str(datetime.datetime.now().strftime('%Y-%m-%d-%H-%M-%S'))
             time = datetime.datetime.now().ctime().replace(':', '-')
-            if 'FILE' in self.settings.keys() and self.settings.file != '':
-                file = os.path.join(self.settings.file, 'download', '斗鱼录播',
+            if 'FILE' in self.default_settings.keys() and self.default_settings.file != '':
+                file = os.path.join(self.default_settings.file, 'download', '斗鱼录播',
                                     filename, time)
             else:
                 file = os.path.join(os.getcwd(), 'download', '斗鱼录播', filename,
                                     time)
             ali_file = os.path.join('录播', '斗鱼录播', filename,
                                     time).replace('\\', '/')
             if not os.path.exists(file):
@@ -165,16 +165,16 @@
         rea_rid = rtmp_live.split('?')[0]
         http = os.path.join(random.choice(['http://hdltc1.douyucdn.cn/live', 'http://hw-tct.douyucdn.cn/live']))  \
             + '/' + rea_rid
         if self.name == None:
             name = self.get_name()
         else:
             name = self.name
-        if 'FILE' in self.settings.keys() and self.settings.file != '':
-            file = os.path.join(self.settings.file, 'download', '斗鱼录播', name,
+        if 'FILE' in self.default_settings.keys() and self.default_settings.file != '':
+            file = os.path.join(self.default_settings.file, 'download', '斗鱼录播', name,
                                 time)
         else:
             file = os.path.join(os.getcwd(), 'download', '斗鱼录播', name, time)
         ali_file = os.path.join('录播', '斗鱼录播', name, time).replace('\\', '/')
         if not os.path.exists(file):
             os.makedirs(file)
         f = open(file=os.path.join(file, '直播源.txt'), mode='w', encoding='utf8')
```

### Comparing `evina-1.0.3/evina/evina.py` & `evina-1.0.4/evina/evina.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.3/evina/replacement.py` & `evina-1.0.4/evina/replacement.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.3/evina/ssh.py` & `evina-1.0.4/evina/ssh.py`

 * *Files identical despite different names*

