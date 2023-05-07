# Comparing `tmp/nakuru_project_idk-0.0.2.tar.gz` & `tmp/nakuru_project_idk-0.0.2.1.tar.gz`

## Comparing `nakuru_project_idk-0.0.2.tar` & `nakuru_project_idk-0.0.2.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0   280258 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/logo.png
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/setup.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/__init__.py
--rw-r--r--   0        0        0    14029 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/application.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/logger.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/misc.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/network.py
--rw-r--r--   0        0        0    30016 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/protocol.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/__init__.py
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/components.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/device.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/file.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/friend.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/group.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/guild.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/others.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/event/__init__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/event/builtins.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/event/enums.py
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/event/models.py
--rw-r--r--   0        0        0    51695 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/examples/src/1.jpg
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/examples/src/forward_message.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/LICENSE
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/README.md
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0   280258 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/logo.png
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/setup.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/__init__.py
+-rw-r--r--   0        0        0    14029 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/application.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/logger.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/misc.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/network.py
+-rw-r--r--   0        0        0    30016 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/protocol.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/entities/__init__.py
+-rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/entities/components.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/entities/device.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/entities/file.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/entities/friend.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/entities/group.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/entities/guild.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/entities/others.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/event/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/event/builtins.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/event/enums.py
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/event/models.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/examples/forward_message.py
+-rw-r--r--   0        0        0    51695 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/examples/src/1.jpg
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/nakuru/examples/src/forward_message.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/LICENSE
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2.1/PKG-INFO
```

### Comparing `nakuru_project_idk-0.0.2/logo.png` & `nakuru_project_idk-0.0.2.1/logo.png`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/setup.py` & `nakuru_project_idk-0.0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/application.py` & `nakuru_project_idk-0.0.2.1/nakuru/application.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/misc.py` & `nakuru_project_idk-0.0.2.1/nakuru/misc.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/network.py` & `nakuru_project_idk-0.0.2.1/nakuru/network.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/protocol.py` & `nakuru_project_idk-0.0.2.1/nakuru/protocol.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/entities/components.py` & `nakuru_project_idk-0.0.2.1/nakuru/entities/components.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/entities/file.py` & `nakuru_project_idk-0.0.2.1/nakuru/entities/file.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/entities/group.py` & `nakuru_project_idk-0.0.2.1/nakuru/entities/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
 class Anonymous(BaseModel):
     id: int
     name: str
     flag: str
 
 class Group(BaseModel):
-    group_id: int
-    group_name: str
-    group_memo: str
     group_create_time: int
+    group_id: int
     group_level: int
+    group_name: str
+    group_memo: Optional[str]
     member_count: int
-    max_member_count: int
+    max_member_count: Optional[int]
 
 class HonorListNode(BaseModel):
     user_id: int
     nickname: str
     avatar: str
     description: Optional[str]
     day_count: Optional[int]
```

### Comparing `nakuru_project_idk-0.0.2/nakuru/entities/guild.py` & `nakuru_project_idk-0.0.2.1/nakuru/entities/guild.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/entities/others.py` & `nakuru_project_idk-0.0.2.1/nakuru/entities/others.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/event/builtins.py` & `nakuru_project_idk-0.0.2.1/nakuru/event/builtins.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/event/enums.py` & `nakuru_project_idk-0.0.2.1/nakuru/event/enums.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/event/models.py` & `nakuru_project_idk-0.0.2.1/nakuru/event/models.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/examples/src/1.jpg` & `nakuru_project_idk-0.0.2.1/nakuru/examples/src/1.jpg`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/nakuru/examples/src/forward_message.py` & `nakuru_project_idk-0.0.2.1/nakuru/examples/src/forward_message.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/LICENSE` & `nakuru_project_idk-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.2/README.md` & `nakuru_project_idk-0.0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 <div align="center">
   <img width="256" src="./logo.png" alt="logo">
 
 # Nakuru Project
+
+> 这是由idoknow维护的分支
+
 一款为 [go-cqhttp](https://github.com/Mrs4s/go-cqhttp) 的正向 WebSocket 设计的 Python SDK，支持纯 CQ 码与消息链的转换处理
 
 在 [kuriyama](https://github.com/Lxns-Network/mirai-python-sdk) 的基础上改动
 
 项目名来源于藍月なくる，图标由[せら](https://www.pixiv.net/users/577968)绘制
 </div>
 
 ## 食用方法
-使用 `pip install git+https://github.com/Lxns-Network/nakuru-project.git` 安装。
+
+使用 `pip install nakuru-project-idk` 安装。
 
 需要将 go-cqhttp 的正向 WebSocket 与 HTTP 配置项开启。
 
 ## 示例
+
 没有文档，源码就是文档。
 
 ```python
 from nakuru import (
     CQHTTP,
     GroupMessage,
     Notify,
```

### Comparing `nakuru_project_idk-0.0.2/pyproject.toml` & `nakuru_project_idk-0.0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nakuru-project-idk"
-version = "0.0.2"
+version = "0.0.2.1"
 authors = [
   { name="Lxns-Network", email="joinchang1206@gmail.com" },
-  { name="RockChinQ", email="junyan_qin@qq.com"}
+  { name="RockChinQ", email="junyan_qin@qq.com" }
 ]
 description = "一款为 go-cqhttp 的正向 WebSocket 设计的 Python SDK，支持纯 CQ 码与消息链的转换处理"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `nakuru_project_idk-0.0.2/PKG-INFO` & `nakuru_project_idk-0.0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakuru-project-idk
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: 一款为 go-cqhttp 的正向 WebSocket 设计的 Python SDK，支持纯 CQ 码与消息链的转换处理
 Project-URL: Homepage, https://github.com/idoknow/nakuru-project-idk
 Project-URL: Bug Tracker, https://github.com/idoknow/nakuru-project-idk/issues
 Author-email: Lxns-Network <joinchang1206@gmail.com>, RockChinQ <junyan_qin@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,27 +16,32 @@
 Requires-Dist: pydantic
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img width="256" src="./logo.png" alt="logo">
 
 # Nakuru Project
+
+> 这是由idoknow维护的分支
+
 一款为 [go-cqhttp](https://github.com/Mrs4s/go-cqhttp) 的正向 WebSocket 设计的 Python SDK，支持纯 CQ 码与消息链的转换处理
 
 在 [kuriyama](https://github.com/Lxns-Network/mirai-python-sdk) 的基础上改动
 
 项目名来源于藍月なくる，图标由[せら](https://www.pixiv.net/users/577968)绘制
 </div>
 
 ## 食用方法
-使用 `pip install git+https://github.com/Lxns-Network/nakuru-project.git` 安装。
+
+使用 `pip install nakuru-project-idk` 安装。
 
 需要将 go-cqhttp 的正向 WebSocket 与 HTTP 配置项开启。
 
 ## 示例
+
 没有文档，源码就是文档。
 
 ```python
 from nakuru import (
     CQHTTP,
     GroupMessage,
     Notify,
```

