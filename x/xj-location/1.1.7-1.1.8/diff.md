# Comparing `tmp/xj_location-1.1.7.tar.gz` & `tmp/xj_location-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_location-1.1.7.tar", last modified: Wed Dec  7 02:05:30 2022, max compression
+gzip compressed data, was "dist\xj_location-1.1.8.tar", last modified: Sun May  7 06:13:41 2023, max compression
```

## Comparing `xj_location-1.1.7.tar` & `xj_location-1.1.8.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2022-12-07 02:05:30.000000 xj_location-1.1.7/
--rw-rw-rw-   0        0        0     3830 2022-12-07 02:05:30.000000 xj_location-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3014 2022-08-08 01:31:17.000000 xj_location-1.1.7/README.md
--rw-rw-rw-   0        0        0       42 2022-12-07 02:05:30.000000 xj_location-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      894 2022-12-07 02:05:20.000000 xj_location-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-07 02:05:30.000000 xj_location-1.1.7/xj_location/
--rw-rw-rw-   0        0        0        0 2022-08-08 01:31:17.000000 xj_location-1.1.7/xj_location/__init__.py
--rw-rw-rw-   0        0        0      695 2022-12-07 01:41:08.000000 xj_location-1.1.7/xj_location/admin.py
-drwxrwxrwx   0        0        0        0 2022-12-07 02:05:30.000000 xj_location-1.1.7/xj_location/apis/
--rw-rw-rw-   0        0        0      158 2022-09-07 05:26:05.000000 xj_location-1.1.7/xj_location/apis/__init__.py
--rw-rw-rw-   0        0        0     2171 2022-09-07 06:35:32.000000 xj_location-1.1.7/xj_location/apis/boundary_api.py
--rw-rw-rw-   0        0        0      416 2022-09-07 07:10:10.000000 xj_location-1.1.7/xj_location/apis/group_api.py
--rw-rw-rw-   0        0        0     4214 2022-12-07 01:48:33.000000 xj_location-1.1.7/xj_location/apis/location_api.py
--rw-rw-rw-   0        0        0      212 2022-09-07 09:17:02.000000 xj_location-1.1.7/xj_location/apps.py
--rw-rw-rw-   0        0        0      489 2022-08-08 01:31:17.000000 xj_location-1.1.7/xj_location/config.py
--rw-rw-rw-   0        0        0     2544 2022-12-07 01:41:18.000000 xj_location-1.1.7/xj_location/models.py
-drwxrwxrwx   0        0        0        0 2022-12-07 02:05:30.000000 xj_location-1.1.7/xj_location/services/
--rw-rw-rw-   0        0        0      163 2022-08-08 01:31:17.000000 xj_location-1.1.7/xj_location/services/__init__.py
--rw-rw-rw-   0        0        0     3134 2022-09-07 07:30:10.000000 xj_location-1.1.7/xj_location/services/boundary_service.py
--rw-rw-rw-   0        0        0     3792 2022-12-07 02:04:26.000000 xj_location-1.1.7/xj_location/services/location_service.py
--rw-rw-rw-   0        0        0      949 2022-12-07 01:09:43.000000 xj_location-1.1.7/xj_location/urls.py
-drwxrwxrwx   0        0        0        0 2022-12-07 02:05:30.000000 xj_location-1.1.7/xj_location/utils/
--rw-rw-rw-   0        0        0        0 2022-08-08 01:31:17.000000 xj_location-1.1.7/xj_location/utils/__init__.py
--rw-rw-rw-   0        0        0      637 2022-08-08 01:31:17.000000 xj_location-1.1.7/xj_location/utils/custom_authentication_wrapper.py
--rw-rw-rw-   0        0        0     1526 2022-08-08 01:31:17.000000 xj_location-1.1.7/xj_location/utils/custom_authorization.py
--rw-rw-rw-   0        0        0     1551 2022-08-08 01:31:17.000000 xj_location-1.1.7/xj_location/utils/custom_exception.py
--rw-rw-rw-   0        0        0      881 2022-08-08 01:31:17.000000 xj_location-1.1.7/xj_location/utils/custom_pagination.py
--rw-rw-rw-   0        0        0     1453 2022-08-08 01:31:17.000000 xj_location-1.1.7/xj_location/utils/custom_response.py
--rw-rw-rw-   0        0        0     7806 2022-10-31 08:53:23.000000 xj_location-1.1.7/xj_location/utils/custom_tool.py
--rw-rw-rw-   0        0        0      429 2022-08-27 10:02:03.000000 xj_location-1.1.7/xj_location/utils/j_dict.py
--rw-rw-rw-   0        0        0     7024 2022-12-07 01:13:14.000000 xj_location-1.1.7/xj_location/utils/model_handle.py
--rw-rw-rw-   0        0        0     3885 2022-08-08 01:31:17.000000 xj_location-1.1.7/xj_location/utils/util.py
--rw-rw-rw-   0        0        0     1360 2022-08-08 01:31:17.000000 xj_location-1.1.7/xj_location/utils/validate.py
--rw-rw-rw-   0        0        0     1792 2022-08-08 01:31:17.000000 xj_location-1.1.7/xj_location/validate.py
--rw-rw-rw-   0        0        0     1347 2022-09-07 06:25:28.000000 xj_location-1.1.7/xj_location/view.py
-drwxrwxrwx   0        0        0        0 2022-12-07 02:05:30.000000 xj_location-1.1.7/xj_location.egg-info/
--rw-rw-rw-   0        0        0     3830 2022-12-07 02:05:30.000000 xj_location-1.1.7/xj_location.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2022-12-07 02:05:30.000000 xj_location-1.1.7/xj_location.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-07 02:05:30.000000 xj_location-1.1.7/xj_location.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-12-07 02:05:30.000000 xj_location-1.1.7/xj_location.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 06:13:41.000000 xj_location-1.1.8/
+-rw-rw-rw-   0        0        0     3830 2023-05-07 06:13:41.000000 xj_location-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3014 2022-08-08 01:31:17.000000 xj_location-1.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 06:13:41.000000 xj_location-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      894 2023-05-07 06:13:34.000000 xj_location-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:13:41.000000 xj_location-1.1.8/xj_location/
+-rw-rw-rw-   0        0        0        0 2022-08-08 01:31:17.000000 xj_location-1.1.8/xj_location/__init__.py
+-rw-rw-rw-   0        0        0      695 2022-12-07 01:41:08.000000 xj_location-1.1.8/xj_location/admin.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:13:41.000000 xj_location-1.1.8/xj_location/apis/
+-rw-rw-rw-   0        0        0      158 2022-09-07 05:26:05.000000 xj_location-1.1.8/xj_location/apis/__init__.py
+-rw-rw-rw-   0        0        0     2170 2023-05-06 01:57:31.000000 xj_location-1.1.8/xj_location/apis/boundary_api.py
+-rw-rw-rw-   0        0        0      688 2023-05-07 02:37:27.000000 xj_location-1.1.8/xj_location/apis/group_api.py
+-rw-rw-rw-   0        0        0     5809 2023-05-07 06:12:16.000000 xj_location-1.1.8/xj_location/apis/location_api.py
+-rw-rw-rw-   0        0        0      212 2022-09-07 09:17:02.000000 xj_location-1.1.8/xj_location/apps.py
+-rw-rw-rw-   0        0        0      489 2022-08-08 01:31:17.000000 xj_location-1.1.8/xj_location/config.py
+-rw-rw-rw-   0        0        0     2544 2023-05-05 08:01:05.000000 xj_location-1.1.8/xj_location/models.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:13:41.000000 xj_location-1.1.8/xj_location/services/
+-rw-rw-rw-   0        0        0      163 2022-08-08 01:31:17.000000 xj_location-1.1.8/xj_location/services/__init__.py
+-rw-rw-rw-   0        0        0     3133 2023-05-06 01:57:11.000000 xj_location-1.1.8/xj_location/services/boundary_service.py
+-rw-rw-rw-   0        0        0     1550 2023-05-06 02:14:23.000000 xj_location-1.1.8/xj_location/services/location_group_services.py
+-rw-rw-rw-   0        0        0     6815 2023-05-07 06:11:47.000000 xj_location-1.1.8/xj_location/services/location_service.py
+-rw-rw-rw-   0        0        0      949 2022-12-07 01:09:43.000000 xj_location-1.1.8/xj_location/urls.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:13:41.000000 xj_location-1.1.8/xj_location/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-08 01:31:17.000000 xj_location-1.1.8/xj_location/utils/__init__.py
+-rw-rw-rw-   0        0        0      637 2022-08-08 01:31:17.000000 xj_location-1.1.8/xj_location/utils/custom_authentication_wrapper.py
+-rw-rw-rw-   0        0        0     1526 2022-08-08 01:31:17.000000 xj_location-1.1.8/xj_location/utils/custom_authorization.py
+-rw-rw-rw-   0        0        0     1551 2022-08-08 01:31:17.000000 xj_location-1.1.8/xj_location/utils/custom_exception.py
+-rw-rw-rw-   0        0        0      881 2022-08-08 01:31:17.000000 xj_location-1.1.8/xj_location/utils/custom_pagination.py
+-rw-rw-rw-   0        0        0     1453 2022-08-08 01:31:17.000000 xj_location-1.1.8/xj_location/utils/custom_response.py
+-rw-rw-rw-   0        0        0    27342 2023-05-06 07:09:02.000000 xj_location-1.1.8/xj_location/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      429 2022-08-27 10:02:03.000000 xj_location-1.1.8/xj_location/utils/j_dict.py
+-rw-rw-rw-   0        0        0      660 2022-11-29 06:32:59.000000 xj_location-1.1.8/xj_location/utils/join_list.py
+-rw-rw-rw-   0        0        0     3885 2022-08-08 01:31:17.000000 xj_location-1.1.8/xj_location/utils/util.py
+-rw-rw-rw-   0        0        0     1360 2022-08-08 01:31:17.000000 xj_location-1.1.8/xj_location/utils/validate.py
+-rw-rw-rw-   0        0        0     1792 2022-08-08 01:31:17.000000 xj_location-1.1.8/xj_location/validate.py
+-rw-rw-rw-   0        0        0     1347 2022-09-07 06:25:28.000000 xj_location-1.1.8/xj_location/view.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:13:41.000000 xj_location-1.1.8/xj_location.egg-info/
+-rw-rw-rw-   0        0        0     3830 2023-05-07 06:13:41.000000 xj_location-1.1.8/xj_location.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2023-05-07 06:13:41.000000 xj_location-1.1.8/xj_location.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 06:13:41.000000 xj_location-1.1.8/xj_location.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-07 06:13:41.000000 xj_location-1.1.8/xj_location.egg-info/top_level.txt
```

### Comparing `xj_location-1.1.7/PKG-INFO` & `xj_location-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_location
-Version: 1.1.7
+Version: 1.1.8
 Summary: 定位模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: 孙楷炎
 Maintainer-email: sky4834@163.com
 License: apache 3.0
```

### Comparing `xj_location-1.1.7/README.md` & `xj_location-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `xj_location-1.1.7/setup.py` & `xj_location-1.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_location',  # 模块名称
-    version='1.1.7',  # 模块版本
+    version='1.1.8',  # 模块版本
     description='定位模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     author='赵向明',  # 作者
     author_email='sieyoo@163.com',  # 作者邮箱
     maintainer="孙楷炎",  # 维护者
     maintainer_email="sky4834@163.com",  # 维护者的邮箱地址
```

### Comparing `xj_location-1.1.7/xj_location/admin.py` & `xj_location-1.1.8/xj_location/admin.py`

 * *Files identical despite different names*

### Comparing `xj_location-1.1.7/xj_location/apis/boundary_api.py` & `xj_location-1.1.8/xj_location/apis/boundary_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @synopsis: 边界API
 @created_time: 2022/9/7 14:06
 """
 from rest_framework.views import APIView
 
 from ..services.boundary_service import BoundaryService
 from ..utils.custom_response import util_response
-from ..utils.model_handle import parse_data
+from ..utils.custom_tool import parse_data
 
 
 class BoundaryAPI(APIView):
     def list(self, **kwargs):
         # 用户组 列表接口
         params = parse_data(self)
         data, err = BoundaryService.boundary_list(params)
```

### Comparing `xj_location-1.1.7/xj_location/models.py` & `xj_location-1.1.8/xj_location/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 from django.db import models
 from django.utils import timezone
 
 
 class Location(models.Model):
     id = models.AutoField(primary_key=True)
-    region_code = models.BigIntegerField('行政ID', null=False, default=0)
+    name = models.CharField('名称', null=False, default="", max_length=50)
+    group_id = models.IntegerField('分组ID', null=False, default=0)
+    user_id = models.IntegerField('用户ID', null=False, default=0)
+    by_user_id = models.IntegerField('创建者ID', null=False, default=0)
     thread_id = models.IntegerField('信息ID', null=False, default=0)
     category_id = models.IntegerField('类别ID', null=False, default=0)
     classify_id = models.IntegerField('分类ID', null=False, default=0)
-    name = models.CharField('名称', null=False, default="", max_length=50)
+    region_code = models.BigIntegerField('行政ID', null=False, default=0)
     address = models.CharField('详细地址', null=False, default="", max_length=255)
-    coordinate_type = models.IntegerField('定位类型', null=False, default=84)
     longitude = models.DecimalField('经度', null=False, max_digits=10, decimal_places=6)
-    latitude = models.DecimalField('维度', null=False, max_digits=10, decimal_places=6)
+    latitude = models.DecimalField('纬度', null=False, max_digits=10, decimal_places=6)
     altitude = models.DecimalField('海拔', null=False, max_digits=10, decimal_places=6)
-    user_id = models.IntegerField('用户ID', null=False, default=0)
-    by_user_id = models.IntegerField('创建者ID', null=False, default=0)
-    group_id = models.IntegerField('分组ID', null=False, default=0)
+    coordinate_type = models.IntegerField('定位类型', null=False, default=84)
     created_time = models.DateTimeField('创建时间', default=timezone.now)
 
     class Meta:
         managed = False
         db_table = "location_location"
         verbose_name = "定位信息表"
         verbose_name_plural = verbose_name
```

### Comparing `xj_location-1.1.7/xj_location/services/boundary_service.py` & `xj_location-1.1.8/xj_location/services/boundary_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 import json
 
 from django.core.paginator import Paginator
 from matplotlib.path import Path
 
 from ..models import Boundary, Location
-from ..utils.model_handle import format_params_handle
+from ..utils.custom_tool import format_params_handle
 
 
 class BoundaryService:
     @staticmethod
     def boundary_list(params):
         params = format_params_handle(
             param_dict=params,
```

### Comparing `xj_location-1.1.7/xj_location/urls.py` & `xj_location-1.1.8/xj_location/urls.py`

 * *Files identical despite different names*

### Comparing `xj_location-1.1.7/xj_location/utils/custom_authentication_wrapper.py` & `xj_location-1.1.8/xj_location/utils/custom_authentication_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_location-1.1.7/xj_location/utils/custom_authorization.py` & `xj_location-1.1.8/xj_location/utils/custom_authorization.py`

 * *Files identical despite different names*

### Comparing `xj_location-1.1.7/xj_location/utils/custom_exception.py` & `xj_location-1.1.8/xj_location/utils/custom_exception.py`

 * *Files identical despite different names*

### Comparing `xj_location-1.1.7/xj_location/utils/custom_pagination.py` & `xj_location-1.1.8/xj_location/utils/custom_pagination.py`

 * *Files identical despite different names*

### Comparing `xj_location-1.1.7/xj_location/utils/custom_response.py` & `xj_location-1.1.8/xj_location/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_location-1.1.7/xj_location/utils/util.py` & `xj_location-1.1.8/xj_location/utils/util.py`

 * *Files identical despite different names*

### Comparing `xj_location-1.1.7/xj_location/utils/validate.py` & `xj_location-1.1.8/xj_location/utils/validate.py`

 * *Files identical despite different names*

### Comparing `xj_location-1.1.7/xj_location/validate.py` & `xj_location-1.1.8/xj_location/validate.py`

 * *Files identical despite different names*

### Comparing `xj_location-1.1.7/xj_location/view.py` & `xj_location-1.1.8/xj_location/view.py`

 * *Files identical despite different names*

### Comparing `xj_location-1.1.7/xj_location.egg-info/PKG-INFO` & `xj_location-1.1.8/xj_location.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-location
-Version: 1.1.7
+Version: 1.1.8
 Summary: 定位模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: 孙楷炎
 Maintainer-email: sky4834@163.com
 License: apache 3.0
```

### Comparing `xj_location-1.1.7/xj_location.egg-info/SOURCES.txt` & `xj_location-1.1.8/xj_location.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 xj_location.egg-info/top_level.txt
 xj_location/apis/__init__.py
 xj_location/apis/boundary_api.py
 xj_location/apis/group_api.py
 xj_location/apis/location_api.py
 xj_location/services/__init__.py
 xj_location/services/boundary_service.py
+xj_location/services/location_group_services.py
 xj_location/services/location_service.py
 xj_location/utils/__init__.py
 xj_location/utils/custom_authentication_wrapper.py
 xj_location/utils/custom_authorization.py
 xj_location/utils/custom_exception.py
 xj_location/utils/custom_pagination.py
 xj_location/utils/custom_response.py
 xj_location/utils/custom_tool.py
 xj_location/utils/j_dict.py
-xj_location/utils/model_handle.py
+xj_location/utils/join_list.py
 xj_location/utils/util.py
 xj_location/utils/validate.py
```

