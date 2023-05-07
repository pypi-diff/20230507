# Comparing `tmp/nonebot_plugin_watermarker-0.1.3.tar.gz` & `tmp/nonebot_plugin_watermarker-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_watermarker-0.1.3.tar", last modified: Mon May  1 23:54:19 2023, max compression
+gzip compressed data, was "nonebot_plugin_watermarker-0.1.4.tar", last modified: Sun May  7 02:48:42 2023, max compression
```

## Comparing `nonebot_plugin_watermarker-0.1.3.tar` & `nonebot_plugin_watermarker-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 23:54:19.730735 nonebot_plugin_watermarker-0.1.3/
--rw-rw-rw-   0        0        0     1087 2023-05-01 12:04:12.000000 nonebot_plugin_watermarker-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     4000 2023-05-01 23:54:19.729765 nonebot_plugin_watermarker-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3644 2023-05-01 12:31:50.000000 nonebot_plugin_watermarker-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 23:54:19.720766 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/
--rw-rw-rw-   0        0        0     2081 2023-05-01 23:54:10.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/__init__.py
--rw-rw-rw-   0        0        0      842 2023-05-01 09:25:17.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/config.py
--rw-rw-rw-   0        0        0     2009 2023-05-01 08:46:06.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/fuctions.py
-drwxrwxrwx   0        0        0        0 2023-05-01 23:54:19.728739 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/
--rw-rw-rw-   0        0        0     4000 2023-05-01 23:54:19.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-05-01 23:54:19.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 23:54:19.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-01 23:54:19.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-01 23:54:19.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 23:54:19.730735 nonebot_plugin_watermarker-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     4208 2023-05-01 23:53:54.000000 nonebot_plugin_watermarker-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 02:48:42.627277 nonebot_plugin_watermarker-0.1.4/
+-rw-rw-rw-   0        0        0     1087 2023-05-01 12:04:12.000000 nonebot_plugin_watermarker-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     4000 2023-05-07 02:48:42.626282 nonebot_plugin_watermarker-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3644 2023-05-02 00:05:20.000000 nonebot_plugin_watermarker-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 02:48:42.613314 nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker/
+-rw-rw-rw-   0        0        0     2081 2023-05-01 23:54:10.000000 nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-05-01 09:25:17.000000 nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker/config.py
+-rw-rw-rw-   0        0        0     2365 2023-05-07 02:46:45.000000 nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker/fuctions.py
+drwxrwxrwx   0        0        0        0 2023-05-07 02:48:42.625283 nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker.egg-info/
+-rw-rw-rw-   0        0        0     4000 2023-05-07 02:48:42.000000 nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-05-07 02:48:42.000000 nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 02:48:42.000000 nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-07 02:48:42.000000 nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-07 02:48:42.000000 nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 02:48:42.627277 nonebot_plugin_watermarker-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     4208 2023-05-07 02:48:05.000000 nonebot_plugin_watermarker-0.1.4/setup.py
```

### Comparing `nonebot_plugin_watermarker-0.1.3/LICENSE` & `nonebot_plugin_watermarker-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_watermarker-0.1.3/PKG-INFO` & `nonebot_plugin_watermarker-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_watermarker
-Version: 0.1.3
+Version: 0.1.4
 Summary: 为nonebot机器人发送的图片加上水印
 Home-page: https://github.com/X-Skirt-X/nonebot-plugin-watermarker
 Author: XU
 Author-email: Woyerpa@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_watermarker Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_watermarker Version: 0.1.4 Summary:
 ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å° Home-page: https://github.com/X-
 Skirt-X/nonebot-plugin-watermarker Author: XU Author-email: Woyerpa@outlook.com
 License: MIT License Platform: UNKNOWN Description-Content-Type: text/markdown
 License-File: LICENSE
                             [PoweredByNonebotLogo]
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

### Comparing `nonebot_plugin_watermarker-0.1.3/README.md` & `nonebot_plugin_watermarker-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,27 +38,27 @@
 ## 💿安装方法
 ### ```nb脚手架```
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
 ```cmd
-nb plugin install nonebot_piugin_watermarker
+nb plugin install nonebot-piugin-watermarker
 ```
 
 </details>
 
 ### ```pip```
 <details>
 <summary>pip安装</summary>
 
 命令行输入以下命令
 
 ```cmd
-pip install nonebot_plugin_watermarker
+pip install nonebot-plugin-watermarker
 ```
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot_plugin_rename"]
 
 ```
```

#### html2text {}

```diff
@@ -7,16 +7,16 @@
 [âï¸æä»¶éç½®é¡¹](#æä»¶éç½®é¡¹) * [ðç®åå·²å®ç°çåè½]
 (#ç®åå·²å®ç°çåè½) * [ð¡å¾å®ç°çåè½](#å¾å®ç°çåè½) *
 [ð£å·²ç¥bug](#å·²ç¥bug) * [ð¥é¸£è°¢](#é¸£è°¢) * [ð¦å¶ä»](#å¶ä»)  ##
 ðç®ä» ä¸ºbotååºçææå¾çé½å ä¸æ°´å°
 (æçæ¶åæ°´å°å¾ç¦,ä½æ¯å¸æ°çæ°´å°è½å¢å å¾ççç¾æ,ä¸æ¯å?)
 ## ð¿å®è£æ¹æ³ ### ```nbèææ¶```  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```cmd nb
-plugin install nonebot_piugin_watermarker ```  ### ```pip```  pipå®è£
-å½ä»¤è¡è¾å¥ä»¥ä¸å½ä»¤ ```cmd pip install nonebot_plugin_watermarker ```
+plugin install nonebot-piugin-watermarker ```  ### ```pip```  pipå®è£
+å½ä»¤è¡è¾å¥ä»¥ä¸å½ä»¤ ```cmd pip install nonebot-plugin-watermarker ```
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_rename"] ```
 [tool.nonebot] plugins = [] plugin_dirs = ["src/plugins"] ```  ##
 âæä»¶éç½®é¡¹ | åéå | åéç±»å | åéæ¦è¿° | |------------|--
 --------------------------------|----------------| | ```watermark_image_path```
 |```str```|æ°´å°å¾çå­æ¾ç®å½,ç®å½ä¸çæææ°´å°å¾çä¼è¢«éæºéå|
 | ```watermark_image_size``` |```float```|æ°´å°ç¸å¯¹å¾ççå¤§å°
```

### Comparing `nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/__init__.py` & `nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/config.py` & `nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/fuctions.py` & `nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker/fuctions.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,36 +5,44 @@
 import urllib.request
 import PIL.Image as Image
 
 from pathlib import Path
 from typing import Union, List, Tuple
 
 
-def str2img(string: str) -> Union[Image.Image, None]:
+async def str2img(string: str) -> Union[Image.Image, None]:
     """传入的MessageSegment中的file的字符串转换为PIL图片对象
 
     Args:
         string (str): _description_
 
     Returns:
         Union[Image.Image, None]: _description_
     """
     base64_pattern = r"base64://[a-zA-Z0-9+/]+"
-    other_pattern = r"(?:file|http|https)://[a-zA-Z0-9+/]+"
+    other_pattern = r"(?:http|https)://\S+"
+    file_pattern = r"file:///\S+"
     image1 = None
+    breakpoint()
     if matcher := re.search(base64_pattern, string):
         string = matcher.group()
         string = string.replace("base64://", "")
-        bytes = base64.b64decode(string)
-        image_stream = io.BytesIO(bytes)
+        image_bytes = base64.b64decode(string)
+        image_stream = io.BytesIO(image_bytes)
         image1 = Image.open(image_stream)
     elif matcher := re.search(other_pattern, string):
         string = matcher.group()
-        bytes = urllib.request.urlopen(string).read()
-        image1 = Image.open(bytes)
+        image_bytes = urllib.request.urlopen(string).read()
+        image_stream = io.BytesIO(image_bytes)
+        image1 = Image.open(image_stream)
+    elif matcher := re.search(file_pattern, string):
+        string = matcher.group()
+        image_bytes = urllib.request.urlopen(string).read()
+        image_stream = io.BytesIO(image_bytes)
+        image1 = Image.open(image_stream)
 
     return image1
 
 
 def get_image_dirs(path: Union[str, Path]) -> List[str]:
     """获得传入目录下的所有图片(AI写的,错了不怪我())
```

### Comparing `nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/PKG-INFO` & `nonebot_plugin_watermarker-0.1.4/nonebot_plugin_watermarker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-watermarker
-Version: 0.1.3
+Version: 0.1.4
 Summary: 为nonebot机器人发送的图片加上水印
 Home-page: https://github.com/X-Skirt-X/nonebot-plugin-watermarker
 Author: XU
 Author-email: Woyerpa@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-watermarker Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-watermarker Version: 0.1.4 Summary:
 ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å° Home-page: https://github.com/X-
 Skirt-X/nonebot-plugin-watermarker Author: XU Author-email: Woyerpa@outlook.com
 License: MIT License Platform: UNKNOWN Description-Content-Type: text/markdown
 License-File: LICENSE
                             [PoweredByNonebotLogo]
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

### Comparing `nonebot_plugin_watermarker-0.1.3/setup.py` & `nonebot_plugin_watermarker-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
     
 setup(
     name='nonebot_plugin_watermarker',
 
-    version="0.1.3",
+    version="0.1.4",
     description=(
         '为nonebot机器人发送的图片加上水印'
 
     ),
     long_description="""<div align="center">
   <p><img src="https://user-images.githubusercontent.com/91937041/235443858-85949be1-08d6-4d7a-b132-b1aed71ab943.png" width="560" alt="PoweredByNonebotLogo"></p>
   <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages setup
-( name='nonebot_plugin_watermarker', version="0.1.3", description=
+( name='nonebot_plugin_watermarker', version="0.1.4", description=
 ( 'ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å°' ), long_description="""
                             [PoweredByNonebotLogo]
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot-plugin-watermarker _â¨ ä¸ºä½ çbotååºçå¾çæ·»å æ°´å°! â¨_
                            [license] [pypi] [python]
  * [ðç®ä»](#ç®ä») * [ð¿ å®è£æ¹æ³](#å®è£æ¹æ³) *
```

