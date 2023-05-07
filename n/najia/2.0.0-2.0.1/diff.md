# Comparing `tmp/najia-2.0.0.tar.gz` & `tmp/najia-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "najia-2.0.0.tar", max compression
+gzip compressed data, was "najia-2.0.1.tar", max compression
```

## Comparing `najia-2.0.0.tar` & `najia-2.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      186 2023-05-07 07:23:26.496981 najia-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2023-05-06 14:18:26.541562 najia-2.0.0/LICENSE
--rw-r--r--   0        0        0     1849 2023-05-07 02:41:59.512204 najia-2.0.0/README.md
--rw-r--r--   0        0        0      104 2023-05-07 07:23:26.516038 najia-2.0.0/najia/__init__.py
--rw-r--r--   0        0        0     1334 2023-05-07 07:07:54.049233 najia-2.0.0/najia/__main__.py
--rw-r--r--   0        0        0     4666 2023-05-07 02:41:59.512624 najia-2.0.0/najia/const.py
--rw-r--r--   0        0        0   116617 2023-05-06 14:18:26.544328 najia-2.0.0/najia/data/dd.json
--rw-r--r--   0        0        0     1268 2023-05-07 07:07:54.049455 najia-2.0.0/najia/data/standard.tpl
--rw-r--r--   0        0        0     8958 2023-05-07 07:07:54.049701 najia-2.0.0/najia/najia.py
--rw-r--r--   0        0        0     5790 2023-05-07 07:07:54.049939 najia-2.0.0/najia/utils.py
--rw-r--r--   0        0        0     1082 2023-05-07 07:23:26.528502 najia-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2539 1970-01-01 00:00:00.000000 najia-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      256 2023-05-07 07:59:00.829133 najia-2.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2023-05-06 14:18:26.541562 najia-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1849 2023-05-07 02:41:59.512204 najia-2.0.1/README.md
+-rw-r--r--   0        0        0      104 2023-05-07 07:59:00.848581 najia-2.0.1/najia/__init__.py
+-rw-r--r--   0        0        0     1334 2023-05-07 07:07:54.049233 najia-2.0.1/najia/__main__.py
+-rw-r--r--   0        0        0     4666 2023-05-07 02:41:59.512624 najia-2.0.1/najia/const.py
+-rw-r--r--   0        0        0    58212 2023-05-07 07:55:58.000918 najia-2.0.1/najia/data/guaci.pkl
+-rw-r--r--   0        0        0     1268 2023-05-07 07:07:54.049455 najia-2.0.1/najia/data/standard.tpl
+-rw-r--r--   0        0        0     9063 2023-05-07 07:57:17.519268 najia-2.0.1/najia/najia.py
+-rw-r--r--   0        0        0     6105 2023-05-07 07:56:41.876988 najia-2.0.1/najia/utils.py
+-rw-r--r--   0        0        0     1082 2023-05-07 07:59:00.861621 najia-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2539 1970-01-01 00:00:00.000000 najia-2.0.1/PKG-INFO
```

### Comparing `najia-2.0.0/LICENSE` & `najia-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `najia-2.0.0/README.md` & `najia-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `najia-2.0.0/najia/__main__.py` & `najia-2.0.1/najia/__main__.py`

 * *Files identical despite different names*

### Comparing `najia-2.0.0/najia/const.py` & `najia-2.0.1/najia/const.py`

 * *Files identical despite different names*

### Comparing `najia-2.0.0/najia/data/standard.tpl` & `najia-2.0.1/najia/data/standard.tpl`

 * *Files identical despite different names*

### Comparing `najia-2.0.0/najia/najia.py` & `najia-2.0.1/najia/najia.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 from .const import GUA64
 from .const import GUAS
 from .const import SYMBOL
 from .const import XING5
 from .const import YAOS
 from .const import ZHI5
 from .const import ZHIS
+from .utils import get_god6
+from .utils import get_guaci
 from .utils import get_najia
+from .utils import get_qin6
 from .utils import get_type
-from .utils import god6
-from .utils import gz5_x
+from .utils import GZ5X
 from .utils import palace
-from .utils import qin6
 from .utils import set_shi_yao
 
 logging.basicConfig(level='INFO')
 logger = logging.getLogger(__name__)
 
 
 class Najia(object):
@@ -111,18 +112,18 @@
 
         if len(set(qins)) < 5:
             mark = YAOS[gong] * 2
 
             logger.debug(mark)
 
             # 六亲
-            qin6 = [(qin6(XING5[int(GUA5[gong])], ZHI5[ZHIS.index(x[1])])) for x in get_najia(mark)]
+            qin6 = [(get_qin6(XING5[int(GUA5[gong])], ZHI5[ZHIS.index(x[1])])) for x in get_najia(mark)]
 
             # 干支五行
-            qinx = [gz5_x(x) for x in get_najia(mark)]
+            qinx = [GZ5X(x) for x in get_najia(mark)]
             seat = [qin6.index(x) for x in list(set(qin6).difference(set(qins)))]
 
             return {
                 'name': GUA64.get(mark),
                 'mark': mark,
                 'qin6': qin6,
                 'qinx': qinx,
@@ -147,16 +148,16 @@
             params = [x for x in params]
 
         if len(params) < 6:
             raise Exception('')
 
         if 3 in params or 4 in params:
             mark = ''.join(['1' if v in [1, 4] else '0' for v in params])
-            qin6 = [(qin6(XING5[int(GUA5[gong])], ZHI5[ZHIS.index(x[1])])) for x in get_najia(mark)]
-            qinx = [gz5_x(x) for x in get_najia(mark)]
+            qin6 = [(get_qin6(XING5[int(GUA5[gong])], ZHI5[ZHIS.index(x[1])])) for x in get_najia(mark)]
+            qinx = [GZ5X(x) for x in get_najia(mark)]
 
             return {
                 'name': GUA64.get(mark),
                 'mark': mark,
                 'qin6': qin6,
                 'qinx': qinx,
                 'gong': GUAS[palace(mark, set_shi_yao(mark)[0])],
@@ -191,22 +192,22 @@
         # 卦宫
         gong = palace(mark, shiy[0])  # 卦宫
 
         # 卦名
         name = GUA64[mark]
 
         # 六亲
-        qin6 = [(qin6(XING5[int(GUA5[gong])], ZHI5[ZHIS.index(x[1])])) for x in get_najia(mark)]
-        qinx = [gz5_x(x) for x in get_najia(mark)]
+        qin6 = [(get_qin6(XING5[int(GUA5[gong])], ZHI5[ZHIS.index(x[1])])) for x in get_najia(mark)]
+        qinx = [GZ5X(x) for x in get_najia(mark)]
 
         # logger.debug(qin6)
 
         # 六神
         # god6 = God6(''.join([GANS[lunar['day'].tg], ZHIS[lunar['day'].dz]]))
-        god6 = god6(lunar['gz']['day'])
+        god6 = get_god6(lunar['gz']['day'])
 
         # 动爻位置
         dong = [i for i, x in enumerate(params) if x > 2]
         # logger.debug(dong)
 
         # 伏神
         hide = self._hidden(gong, qin6)
@@ -300,16 +301,17 @@
                 shiy.append('应')
             else:
                 shiy.append('  ')
 
         rows['shiy'] = shiy
 
         if self.data['guaci']:
-            rows['guaci'] = json.load(open(os.path.join(os.path.dirname(__file__), 'data/dd.json'))).get(rows['name'])
-            rows['guaci'] = rows.get('guaci', '').replace('********************', '').replace('　象曰：', '象曰：')
+            rows['guaci'] = get_guaci(rows['name'])
+            # rows['guaci'] = json.load(open(os.path.join(os.path.dirname(__file__), 'data/dd.json'))).get(rows['name'])
+            # rows['guaci'] = rows.get('guaci', '').replace('********************', '').replace('　象曰：', '象曰：')
 
         template = Template(tpl)
         return template.render(**rows)
 
     def export(self):
         solar, params = self.data
         return solar, params
```

### Comparing `najia-2.0.0/najia/utils.py` & `najia-2.0.1/najia/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 import math
+from pathlib import Path
 
 from . import const
 
 logging.basicConfig(level='INFO')
 logger = logging.getLogger(__name__)
 
 
-def gz5_x(gz=''):
+def GZ5X(gz=''):
     """
     干支五行
     :param gz:
     :return:
     """
     _, z = [i for i in gz]
     zm = const.ZHIS.index(z)
@@ -50,15 +51,15 @@
         zm += 12
 
     xk = int((zm - gm) / 2) - 1
 
     return const.KONG[xk]
 
 
-def god6(gz=None):
+def get_god6(gz=None):
     """
     # 六神, 根据日干五行配对六神五行
 
     :param gz: 日干支
     :return:
     """
 
@@ -262,15 +263,15 @@
 
     gan = const.NAJIA[wai][1][0]
     wgz = [f'{gan}{zhi}' for zhi in const.NAJIA[wai][1][1:]]  # 排干支
 
     return ngz + wgz
 
 
-def qin6(w1, w2):
+def get_qin6(w1, w2):
     """
     两个五行判断六亲
     水1 # 木2 # 金3 # 火4 # 土5
 
     :param w1:
     :param w2:
     :return:
@@ -282,7 +283,20 @@
     ws = ws + 5 if ws < 0 else ws
     q6 = const.QING6[ws]
 
     logger.debug(ws)
     logger.debug(q6)
 
     return q6
+
+
+def get_guaci(name=None):
+    import pickle
+
+    try:
+        result = Path(__file__).parent / 'data' / 'guaci.pkl'
+        result = pickle.loads(result.read_bytes())
+        result = result.get(name)
+
+        return result
+    except Exception as ex:
+        logger.exception(ex)
```

### Comparing `najia-2.0.0/pyproject.toml` & `najia-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "najia"
-version = "2.0.0"
+version = "2.0.1"
 description = ""
 authors = ["bopo <ibopo@126.com>"]
 readme = "README.md"
 include = ["CHANGELOG.md"]
 repository = "https://github.com/bopo/najia"
 homepage = "https://github.com/bopo/najia"
 license = "MIT"
@@ -43,15 +43,15 @@
 testpaths = "tests"
 addopts = "-p no:warnings"
 log_cli = 0
 log_cli_level = "DEBUG"
 
 
 [tool.commitizen]
-version = "2.0.0"
+version = "2.0.1"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_file = "CHANGELOG.md"
 annotated_tag = true
 version_files = [
     "najia/__init__.py:__version__",
     "pyproject.toml:version",
```

### Comparing `najia-2.0.0/PKG-INFO` & `najia-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: najia
-Version: 2.0.0
+Version: 2.0.1
 Summary: 
 Home-page: https://github.com/bopo/najia
 License: MIT
 Author: bopo
 Author-email: ibopo@126.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

