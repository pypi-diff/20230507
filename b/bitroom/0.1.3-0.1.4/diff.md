# Comparing `tmp/bitroom-0.1.3.tar.gz` & `tmp/bitroom-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitroom-0.1.3.tar", last modified: Fri May  5 09:24:15 2023, max compression
+gzip compressed data, was "bitroom-0.1.4.tar", last modified: Sun May  7 11:38:00 2023, max compression
```

## Comparing `bitroom-0.1.3.tar` & `bitroom-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     4160 2023-05-05 09:23:56.607045 bitroom-0.1.3/README.md
--rw-r--r--   0        0        0     1408 2023-05-05 09:24:15.211127 bitroom-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      100 2023-05-05 09:23:56.607045 bitroom-0.1.3/src/bitroom/__init__.py
--rw-r--r--   0        0        0       28 2023-05-05 09:23:56.607045 bitroom-0.1.3/src/bitroom/__main__.py
--rw-r--r--   0        0        0       43 2023-05-05 09:23:56.607045 bitroom-0.1.3/src/bitroom/auth/__init__.py
--rw-r--r--   0        0        0     2452 2023-05-05 09:23:56.607045 bitroom-0.1.3/src/bitroom/auth/auth.py
--rw-r--r--   0        0        0    18654 2023-05-05 09:23:56.607045 bitroom-0.1.3/src/bitroom/auth/encrypt_js.py
--rw-r--r--   0        0        0     2540 2023-05-05 09:23:56.607045 bitroom-0.1.3/src/bitroom/cli.py
--rw-r--r--   0        0        0     1642 2023-05-05 09:23:56.607045 bitroom-0.1.3/src/bitroom/config.py
--rw-r--r--   0        0        0    10055 2023-05-05 09:23:56.607045 bitroom-0.1.3/src/bitroom/room.py
--rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 bitroom-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-07 11:37:45.595288 bitroom-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4160 2023-05-07 11:37:45.595288 bitroom-0.1.4/README.md
+-rw-r--r--   0        0        0     1408 2023-05-07 11:38:00.619281 bitroom-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/__main__.py
+-rw-r--r--   0        0        0       43 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/auth/__init__.py
+-rw-r--r--   0        0        0     2452 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/auth/auth.py
+-rw-r--r--   0        0        0    18654 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/auth/encrypt_js.py
+-rw-r--r--   0        0        0     2540 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/cli.py
+-rw-r--r--   0        0        0     1642 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/config.py
+-rw-r--r--   0        0        0    10664 2023-05-07 11:37:45.595288 bitroom-0.1.4/src/bitroom/room.py
+-rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 bitroom-0.1.4/PKG-INFO
```

### Comparing `bitroom-0.1.3/README.md` & `bitroom-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.3/pyproject.toml` & `bitroom-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bitroom"
-version = "0.1.3"
+version = "0.1.4"
 description = "BIT 场地预约查询接口（bitroom）"
 authors = [
     { name = "Y.D.X.", email = "73375426+YDX-2147483647@users.noreply.github.com" },
 ]
 dependencies = [
     "PyExecJS>=1.5.1",
     "httpx>=0.24.0",
```

### Comparing `bitroom-0.1.3/src/bitroom/auth/auth.py` & `bitroom-0.1.4/src/bitroom/auth/auth.py`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.3/src/bitroom/auth/encrypt_js.py` & `bitroom-0.1.4/src/bitroom/auth/encrypt_js.py`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.3/src/bitroom/cli.py` & `bitroom-0.1.4/src/bitroom/cli.py`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.3/src/bitroom/config.py` & `bitroom-0.1.4/src/bitroom/config.py`

 * *Files identical despite different names*

### Comparing `bitroom-0.1.3/src/bitroom/room.py` & `bitroom-0.1.4/src/bitroom/room.py`

 * *Files 12% similar despite different names*

```diff
@@ -237,49 +237,67 @@
 
         data = await self._fetch_bookings_data(
             date, page=page, rooms_per_page=rooms_per_page
         )
         return list(self._parse_bookings_data(data, dates=dates))
 
     async def fetch_bookings(
-        self, date: datetime.date, *, rooms_per_page=3
+        self,
+        date: datetime.date,
+        *,
+        rooms_per_page=3,
+        n_weeks=2,
     ) -> list[Booking]:
         """获取可预约的时空区间
 
         :param date: 日期
         :param rooms_per_page: 访问 API 时每页房间数量
-        :yield: 相邻一周（周一–周日）可预约的时空区间
+        :param n_weeks: 获取的时间范围，1 代表只获取相邻一周，2 代表相邻一周和再下一周
+        :yield: 相邻几周可预约的时空区间
+
+        “相邻一周”指周一–周日。
+        例如假设5月1日为周一，查询 5月5日，则会返回5月1–7日的情况。
 
         # 玄学
 
         响应时间与 rooms_per_page 近似线性正相关。
 
         若不并发，rooms_per_page=10 时单位时间获取的房间最多。
         """
 
         # 首先试探，取得基本数据
         # 只获取一项响应更快
         sniff_data = await self._fetch_bookings_data(date, page=0, rooms_per_page=1)
 
         dates = [date.fromisoformat(it["WEEKDATE"]) for it in sniff_data["weekList"]]
-        """此次查询涉及的日期，周一–周日"""
+        """此次查询相邻一周的日期，周一–周日"""
 
         n_rooms = int(sniff_data["siteInfoList"][0]["totalCount"])
         n_pages = ceil(n_rooms / rooms_per_page)
 
         # 然后获取所有数据
-        # 每一页的结果
-        bookings_set = await gather(
-            *(
+        fetch_plans = []
+        # 每一周
+        for w in range(n_weeks):
+            shift = datetime.timedelta(weeks=w)
+            shifted_date = date + shift
+            shifted_dates = [d + shift for d in dates]
+
+            fetch_plans.extend(
                 self._fetch_bookings_page(
-                    page=p, date=date, rooms_per_page=rooms_per_page, dates=dates
+                    page=p,
+                    date=shifted_date,
+                    rooms_per_page=rooms_per_page,
+                    dates=shifted_dates,
                 )
                 for p in range(n_pages)
             )
-        )
+
+        # 每一页的结果
+        bookings_set = await gather(*fetch_plans)
 
         # Flatten
         return list(chain.from_iterable(bookings_set))
 
     async def book(
         self,
         booking: Booking | list[Booking],
```

### Comparing `bitroom-0.1.3/PKG-INFO` & `bitroom-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitroom
-Version: 0.1.3
+Version: 0.1.4
 Summary: BIT 场地预约查询接口（bitroom）
 Author-Email: Y.D.X. <73375426+YDX-2147483647@users.noreply.github.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

