# Comparing `tmp/gdshoplib-1.8.0.tar.gz` & `tmp/gdshoplib-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdshoplib-1.8.0.tar", max compression
+gzip compressed data, was "gdshoplib-1.9.0.tar", max compression
```

## Comparing `gdshoplib-1.8.0.tar` & `gdshoplib-1.9.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1855 2023-01-02 14:26:10.856806 gdshoplib-1.8.0/README.md
--rw-r--r--   0        0        0      195 2023-01-03 20:09:44.498187 gdshoplib-1.8.0/gdshoplib/__init__.py
--rw-r--r--   0        0        0       80 2023-01-03 20:04:30.238472 gdshoplib-1.8.0/gdshoplib/__main__.py
--rw-r--r--   0        0        0        0 2023-01-01 19:36:37.507364 gdshoplib-1.8.0/gdshoplib/apps/__init__.py
--rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003805 gdshoplib-1.8.0/gdshoplib/apps/finance/__init__.py
--rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003925 gdshoplib-1.8.0/gdshoplib/apps/marketing/__init__.py
--rw-r--r--   0        0        0     1234 2023-01-03 19:49:37.886499 gdshoplib-1.8.0/gdshoplib/apps/platform.py
--rw-r--r--   0        0        0      378 2023-01-01 19:36:37.510481 gdshoplib-1.8.0/gdshoplib/apps/platforms/README.md
--rw-r--r--   0        0        0      435 2023-01-01 19:36:37.511353 gdshoplib-1.8.0/gdshoplib/apps/platforms/__init__.py
--rw-r--r--   0        0        0     1573 2023-01-06 17:56:48.286983 gdshoplib-1.8.0/gdshoplib/apps/platforms/avito.py
--rw-r--r--   0        0        0      388 2023-01-01 19:36:37.513182 gdshoplib-1.8.0/gdshoplib/apps/platforms/base.py
--rw-r--r--   0        0        0      221 2023-01-01 19:36:37.513924 gdshoplib-1.8.0/gdshoplib/apps/platforms/instagram.py
--rw-r--r--   0        0        0      164 2023-01-01 19:36:37.514817 gdshoplib-1.8.0/gdshoplib/apps/platforms/ok.py
--rw-r--r--   0        0        0      164 2023-01-01 19:36:37.515587 gdshoplib-1.8.0/gdshoplib/apps/platforms/tg.py
--rw-r--r--   0        0        0      924 2023-01-01 19:36:37.516436 gdshoplib-1.8.0/gdshoplib/apps/platforms/ula.py
--rw-r--r--   0        0        0      200 2023-01-01 19:36:37.517154 gdshoplib-1.8.0/gdshoplib/apps/platforms/vk.py
--rw-r--r--   0        0        0      174 2023-01-01 19:36:37.517919 gdshoplib-1.8.0/gdshoplib/apps/platforms/yam.py
--rw-r--r--   0        0        0     3702 2023-01-08 13:59:30.357413 gdshoplib-1.8.0/gdshoplib/apps/product.py
--rw-r--r--   0        0        0      187 2023-01-01 19:36:37.519008 gdshoplib-1.8.0/gdshoplib/apps/products/README.md
--rw-r--r--   0        0        0        0 2022-11-29 21:45:29.004030 gdshoplib-1.8.0/gdshoplib/apps/products/__init__.py
--rw-r--r--   0        0        0     1931 2023-01-01 19:36:37.520803 gdshoplib-1.8.0/gdshoplib/apps/products/description.py
--rw-r--r--   0        0        0     2160 2023-01-01 20:08:35.653603 gdshoplib-1.8.0/gdshoplib/apps/products/media.py
--rw-r--r--   0        0        0     3216 2023-01-09 20:21:50.113611 gdshoplib-1.8.0/gdshoplib/apps/products/price.py
--rw-r--r--   0        0        0     8711 2023-01-09 19:33:42.810839 gdshoplib-1.8.0/gdshoplib/cli/application.py
--rw-r--r--   0        0        0     3292 2023-01-08 18:33:34.056846 gdshoplib-1.8.0/gdshoplib/core/settings.py
--rw-r--r--   0        0        0        0 2023-01-01 19:36:37.525746 gdshoplib-1.8.0/gdshoplib/packages/__init__.py
--rw-r--r--   0        0        0     3063 2023-01-09 20:19:16.166687 gdshoplib-1.8.0/gdshoplib/packages/cache.py
--rw-r--r--   0        0        0     2822 2023-01-06 17:56:22.155056 gdshoplib-1.8.0/gdshoplib/packages/feed.py
--rw-r--r--   0        0        0      774 2023-01-01 19:36:37.530383 gdshoplib-1.8.0/gdshoplib/packages/lang.py
--rw-r--r--   0        0        0     1820 2023-01-01 23:04:08.211299 gdshoplib-1.8.0/gdshoplib/packages/s3.py
--rw-r--r--   0        0        0        0 2023-01-01 19:36:37.533334 gdshoplib-1.8.0/gdshoplib/services/__init__.py
--rw-r--r--   0        0        0     2821 2022-11-29 21:45:29.006810 gdshoplib-1.8.0/gdshoplib/services/notion/README.md
--rw-r--r--   0        0        0       50 2023-01-01 19:36:37.534464 gdshoplib-1.8.0/gdshoplib/services/notion/__init__.py
--rw-r--r--   0        0        0     1729 2023-01-08 13:59:30.361038 gdshoplib-1.8.0/gdshoplib/services/notion/base.py
--rw-r--r--   0        0        0      655 2023-01-08 13:59:30.361846 gdshoplib-1.8.0/gdshoplib/services/notion/block.py
--rw-r--r--   0        0        0     1174 2023-01-08 13:59:30.362864 gdshoplib-1.8.0/gdshoplib/services/notion/database.py
--rw-r--r--   0        0        0     1296 2023-01-08 13:59:30.363533 gdshoplib-1.8.0/gdshoplib/services/notion/manager.py
--rw-r--r--   0        0        0     2981 2023-01-08 13:59:30.364304 gdshoplib-1.8.0/gdshoplib/services/notion/notion.py
--rw-r--r--   0        0        0     6733 2023-01-09 20:47:30.564612 gdshoplib-1.8.0/gdshoplib/services/notion/page.py
--rw-r--r--   0        0        0      811 2023-01-09 19:33:42.813057 gdshoplib-1.8.0/gdshoplib/services/vk/market.py
--rw-r--r--   0        0        0     2318 2023-01-08 18:33:35.656110 gdshoplib-1.8.0/gdshoplib/services/vk/vk.py
--rw-r--r--   0        0        0     1046 2023-01-08 13:59:30.366542 gdshoplib-1.8.0/gdshoplib/templates/basic.txt
--rw-r--r--   0        0        0      446 2023-01-06 19:31:05.484065 gdshoplib-1.8.0/gdshoplib/templates/instagram.txt
--rw-r--r--   0        0        0     1045 2023-01-08 13:59:30.367558 gdshoplib-1.8.0/gdshoplib/templates/ula.txt
--rw-r--r--   0        0        0     1108 2023-01-08 13:59:30.368645 gdshoplib-1.8.0/gdshoplib/templates/vk.txt
--rw-r--r--   0        0        0     1426 2023-01-09 20:22:22.086814 gdshoplib-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 gdshoplib-1.8.0/setup.py
--rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 gdshoplib-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-01-02 14:26:10.856806 gdshoplib-1.9.0/README.md
+-rw-r--r--   0        0        0      195 2023-01-03 20:09:44.498187 gdshoplib-1.9.0/gdshoplib/__init__.py
+-rw-r--r--   0        0        0       80 2023-01-03 20:04:30.238472 gdshoplib-1.9.0/gdshoplib/__main__.py
+-rw-r--r--   0        0        0        0 2023-01-01 19:36:37.507364 gdshoplib-1.9.0/gdshoplib/apps/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003805 gdshoplib-1.9.0/gdshoplib/apps/finance/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003925 gdshoplib-1.9.0/gdshoplib/apps/marketing/__init__.py
+-rw-r--r--   0        0        0     1234 2023-01-03 19:49:37.886499 gdshoplib-1.9.0/gdshoplib/apps/platform.py
+-rw-r--r--   0        0        0      378 2023-01-01 19:36:37.510481 gdshoplib-1.9.0/gdshoplib/apps/platforms/README.md
+-rw-r--r--   0        0        0      435 2023-01-01 19:36:37.511353 gdshoplib-1.9.0/gdshoplib/apps/platforms/__init__.py
+-rw-r--r--   0        0        0     1573 2023-01-06 17:56:48.286983 gdshoplib-1.9.0/gdshoplib/apps/platforms/avito.py
+-rw-r--r--   0        0        0      388 2023-01-01 19:36:37.513182 gdshoplib-1.9.0/gdshoplib/apps/platforms/base.py
+-rw-r--r--   0        0        0      221 2023-01-01 19:36:37.513924 gdshoplib-1.9.0/gdshoplib/apps/platforms/instagram.py
+-rw-r--r--   0        0        0      164 2023-01-01 19:36:37.514817 gdshoplib-1.9.0/gdshoplib/apps/platforms/ok.py
+-rw-r--r--   0        0        0      164 2023-01-01 19:36:37.515587 gdshoplib-1.9.0/gdshoplib/apps/platforms/tg.py
+-rw-r--r--   0        0        0      924 2023-01-01 19:36:37.516436 gdshoplib-1.9.0/gdshoplib/apps/platforms/ula.py
+-rw-r--r--   0        0        0      200 2023-01-01 19:36:37.517154 gdshoplib-1.9.0/gdshoplib/apps/platforms/vk.py
+-rw-r--r--   0        0        0      174 2023-01-01 19:36:37.517919 gdshoplib-1.9.0/gdshoplib/apps/platforms/yam.py
+-rw-r--r--   0        0        0     4849 2023-01-12 18:21:47.686707 gdshoplib-1.9.0/gdshoplib/apps/product.py
+-rw-r--r--   0        0        0      187 2023-01-01 19:36:37.519008 gdshoplib-1.9.0/gdshoplib/apps/products/README.md
+-rw-r--r--   0        0        0        0 2022-11-29 21:45:29.004030 gdshoplib-1.9.0/gdshoplib/apps/products/__init__.py
+-rw-r--r--   0        0        0     1931 2023-01-01 19:36:37.520803 gdshoplib-1.9.0/gdshoplib/apps/products/description.py
+-rw-r--r--   0        0        0     2160 2023-01-01 20:08:35.653603 gdshoplib-1.9.0/gdshoplib/apps/products/media.py
+-rw-r--r--   0        0        0     3730 2023-01-12 19:28:36.751691 gdshoplib-1.9.0/gdshoplib/apps/products/price.py
+-rw-r--r--   0        0        0     9381 2023-01-12 18:21:47.691820 gdshoplib-1.9.0/gdshoplib/cli/application.py
+-rw-r--r--   0        0        0     3401 2023-01-12 18:21:47.694016 gdshoplib-1.9.0/gdshoplib/core/settings.py
+-rw-r--r--   0        0        0        0 2023-01-01 19:36:37.525746 gdshoplib-1.9.0/gdshoplib/packages/__init__.py
+-rw-r--r--   0        0        0     3063 2023-01-09 20:19:16.166687 gdshoplib-1.9.0/gdshoplib/packages/cache.py
+-rw-r--r--   0        0        0     2822 2023-01-06 17:56:22.155056 gdshoplib-1.9.0/gdshoplib/packages/feed.py
+-rw-r--r--   0        0        0      774 2023-01-01 19:36:37.530383 gdshoplib-1.9.0/gdshoplib/packages/lang.py
+-rw-r--r--   0        0        0     1820 2023-01-01 23:04:08.211299 gdshoplib-1.9.0/gdshoplib/packages/s3.py
+-rw-r--r--   0        0        0        0 2023-01-01 19:36:37.533334 gdshoplib-1.9.0/gdshoplib/services/__init__.py
+-rw-r--r--   0        0        0     2821 2022-11-29 21:45:29.006810 gdshoplib-1.9.0/gdshoplib/services/notion/README.md
+-rw-r--r--   0        0        0       50 2023-01-01 19:36:37.534464 gdshoplib-1.9.0/gdshoplib/services/notion/__init__.py
+-rw-r--r--   0        0        0     1729 2023-01-08 13:59:30.361038 gdshoplib-1.9.0/gdshoplib/services/notion/base.py
+-rw-r--r--   0        0        0      655 2023-01-08 13:59:30.361846 gdshoplib-1.9.0/gdshoplib/services/notion/block.py
+-rw-r--r--   0        0        0     1174 2023-01-08 13:59:30.362864 gdshoplib-1.9.0/gdshoplib/services/notion/database.py
+-rw-r--r--   0        0        0     1296 2023-01-08 13:59:30.363533 gdshoplib-1.9.0/gdshoplib/services/notion/manager.py
+-rw-r--r--   0        0        0     2981 2023-01-08 13:59:30.364304 gdshoplib-1.9.0/gdshoplib/services/notion/notion.py
+-rw-r--r--   0        0        0     7375 2023-01-12 19:28:36.931278 gdshoplib-1.9.0/gdshoplib/services/notion/page.py
+-rw-r--r--   0        0        0      811 2023-01-09 19:33:42.813057 gdshoplib-1.9.0/gdshoplib/services/vk/market.py
+-rw-r--r--   0        0        0     2318 2023-01-08 18:33:35.656110 gdshoplib-1.9.0/gdshoplib/services/vk/vk.py
+-rw-r--r--   0        0        0     1046 2023-01-08 13:59:30.366542 gdshoplib-1.9.0/gdshoplib/templates/basic.txt
+-rw-r--r--   0        0        0      446 2023-01-06 19:31:05.484065 gdshoplib-1.9.0/gdshoplib/templates/instagram.txt
+-rw-r--r--   0        0        0     1045 2023-01-08 13:59:30.367558 gdshoplib-1.9.0/gdshoplib/templates/ula.txt
+-rw-r--r--   0        0        0     1108 2023-01-08 13:59:30.368645 gdshoplib-1.9.0/gdshoplib/templates/vk.txt
+-rw-r--r--   0        0        0     1426 2023-01-12 19:28:29.421278 gdshoplib-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 gdshoplib-1.9.0/setup.py
+-rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 gdshoplib-1.9.0/PKG-INFO
```

### Comparing `gdshoplib-1.8.0/README.md` & `gdshoplib-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/apps/platform.py` & `gdshoplib-1.9.0/gdshoplib/apps/platform.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/apps/platforms/avito.py` & `gdshoplib-1.9.0/gdshoplib/apps/platforms/avito.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/apps/platforms/ula.py` & `gdshoplib-1.9.0/gdshoplib/apps/platforms/ula.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/apps/product.py` & `gdshoplib-1.9.0/gdshoplib/apps/product.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,18 +14,42 @@
 
     def __init__(self, *args, **kwargs):
         self._images = None
         self._videos = None
         self._price = None
         self._description = None
         self._kit = None
+        self._badges = None
 
         super(Product, self).__init__(*args, **kwargs)
 
     @classmethod
+    def get(cls, sku):
+        page = [
+            page
+            for page in Database(cls.SETTINGS.PRODUCT_DB).pages(
+                params={
+                    "filter": {
+                        "property": "Наш SKU",
+                        "rich_text": {
+                            "equals": sku,
+                        },
+                    }
+                }
+            )
+        ]
+        if not page:
+            return
+        if len(page) > 1:
+            raise SKUDuplicate
+        page = page[0]
+
+        return cls(page["id"], notion=page.notion, parent=page.parent)
+
+    @classmethod
     def query(cls, filter=None, params=None, notion=None):
         for page in Database(cls.SETTINGS.PRODUCT_DB, notion=notion).pages(
             filter=filter, params=params
         ):
             yield cls(page["id"], notion=page.notion, parent=page.parent)
 
     @property
@@ -104,14 +128,28 @@
             for page in self.kit_field:
                 if self.id != page.id:
                     self._kit.append(
                         Product(page.id, notion=self.notion, parent=self.parent)
                     )
         return self._kit
 
+    @property
+    def badges(self):
+        if not self.badge_field:
+            return
+
+        if not self._badges:
+            self._badges = []
+            for page in self.badge_field:
+                if self.id != page.id:
+                    self._badges.append(
+                        Page(page.id, notion=self.notion, parent=self.parent)
+                    )
+        return self._badges
+
     def available(self):
         return bool(self.quantity)
 
     def generate_sku(self):
         # Сгенерировать SKU на основе продукта
         # Категория.Бренд.Цена_покупки.месяц_добавления.год_добавления.случайные_4_числа
 
@@ -124,7 +162,12 @@
         return re.sub(r"\W", "", sku)
 
     def __str__(self) -> str:
         return f"{self.__class__}: {self.sku}"
 
     def __repr__(self) -> str:
         return f"{self.__class__}: {self.sku}"
+
+
+class SKUDuplicate(Exception):
+    # Если найден товар с одинаковым SKU
+    ...
```

### Comparing `gdshoplib-1.8.0/gdshoplib/apps/products/description.py` & `gdshoplib-1.9.0/gdshoplib/apps/products/description.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/apps/products/media.py` & `gdshoplib-1.9.0/gdshoplib/apps/products/media.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/apps/products/price.py` & `gdshoplib-1.9.0/gdshoplib/apps/products/price.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,55 +12,58 @@
     def __init__(self, product):
         self.product = product
 
     def get_score(self):
         # Получить текущий % наценки
         return (self.allowance_score or 0) + -(self.time_discount or 0)
 
-    @property
-    def kit(self):
-        result = self.now if self.product.quantity else 0
+    def get_kit_price(self, base_price="now"):
+        if not self.product.kit:
+            return None
+
+        result = self[base_price] if self.product.quantity else 0
         for product in self.product.kit:
             if product.quantity:
-                result += product.price.now
+                result += product.price[base_price]
         return result
 
     @property
     def allowance_score(self):
-        # Наценка бренда
+        # Наценка категорий
         categories_score = 0
         for category in self.product.categories:
             categories_score += category.price_coefficient
-        brand_score = self.product.brand.price_coefficient if self.product.brand else 0
-        # Наценка категорий
 
+        # Наценка бренда
+        brand_score = self.product.brand.price_coefficient if self.product.brand else 0
         return sum([self.product.price_coefficient, brand_score, categories_score])
 
     @property
     def current_discount(self):
         # Получить текущую скидку
         if self.now >= self.profit:
             return 0
         return 100 - round(self.now / self.profit * 100)
 
     @property
     def time_discount(self):
+        created_time = self.product.discount_from_date or self.product.created_time
         created_time = (
-            parse(self.product.created_time)
-            if isinstance(self.product.created_time, str)
-            else self.product.created_time
+            parse(created_time).date()
+            if isinstance(created_time, str)
+            else created_time
         )
-        created_at = (datetime.date.today() - created_time.date()).days
+        created_at = (datetime.date.today() - created_time).days
+
         if created_at > 60:
             return 15
-
-        if created_at > 30:
+        elif created_at > 30:
             return 10
 
-        return
+        return 0
 
     def handle_ratio(*rations):
         def decor(func):
             @functools.wraps(func)
             def wrap(self, *args, **kwargs):
                 ration = sum([1, *rations])
                 return func(self, *args, **kwargs) * ration
@@ -90,35 +93,45 @@
                 return self.neitral
             return _now
 
         return self.profit
 
     @property
     def eur(self):
+        # Цена в EUR
         return self.product.price_eur
 
     @property
     @round
     def net(self):
+        # Цена в рублях
         return self.eur * price_settings.EURO_PRICE
 
     @property
     @round
     @handle_ratio(price_settings.PRICE_VAT_RATIO)
     def gross(self):
+        # Цена с учетом расходов и налогов на закупку
         return self.net
 
     @property
     @round
     @handle_ratio(price_settings.PRICE_VAT_RATIO, price_settings.PRICE_NEITRAL_RATIO)
     def neitral(self):
+        # Цена безубыточности
         return self.net
 
     @property
     @round
     @handle_ratio(
         price_settings.PRICE_VAT_RATIO,
         price_settings.PRICE_NEITRAL_RATIO,
         price_settings.PRICE_PROFIT_RATIO,
     )
     def profit(self):
         return self.net
+
+    def __getitem__(self, key):
+        try:
+            return super(Price, self).__getattribute__(key)
+        except AttributeError:
+            return self.__getattr__(key)
```

### Comparing `gdshoplib-1.8.0/gdshoplib/cli/application.py` & `gdshoplib-1.9.0/gdshoplib/cli/application.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from multiprocessing import Pool
+from typing import Optional
 
 import typer
 from rich import print
 
 from gdshoplib import Platform, Product
 from gdshoplib.apps.platforms.base import BasePlatformManager
 from gdshoplib.packages.cache import KeyDBCache
@@ -32,38 +33,49 @@
 
         page.notion.update_prop(
             page.id, params={"properties": {"Наш SKU": [{"text": {"content": sku}}]}}
         )
         print(Product(page.id).sku)
 
 
-@app.command()
-def price_update():
-    for product in Product.query():
-        price = product.price.now
-        product.notion.update_prop(
-            product.id, params={"properties": {"Текущая цена": {"number": price}}}
-        )
-        if product.kit:
-            product.notion.update_prop(
-                product.id,
-                params={
-                    "properties": {"Цена комплекта": {"number": product.price.kit}}
-                },
-            )
+def price_update_action(id):
+    product = Product(id)
+    props_map = {
+        "Текущая Цена": product.price.now,
+        "Цена комплекта": product.price.get_kit_price(),
+        "Безубыточность": product.price.neitral,
+        "Текущая Скидка": product.price.current_discount,
+        "Агентская Цена": product.price.neitral,
+        "Агентский комплект": product.price.get_kit_price(base_price="neitral"),
+    }
+
+    for k, v in props_map.items():
         product.notion.update_prop(
-            product.id,
-            params={
-                "properties": {
-                    "Текущая скидка": {"number": product.price.current_discount}
-                }
-            },
+            product.id, params={"properties": {k: {"number": v}}}
         )
 
-        print(product.sku)
+    print(product.sku)
+
+
+@app.command()
+def price_update(
+    sku: Optional[str] = typer.Option(None), single: bool = typer.Option(False)
+):
+    if sku:
+        price_update_action(Product.get(sku).id)
+
+    if single:
+        for product in Database(Product.SETTINGS.PRODUCT_DB).pages():
+            price_update_action(product["id"])
+    else:
+        with Pool(3) as p:
+            for product in Database(Product.SETTINGS.PRODUCT_DB).pages():
+                p.apply_async(price_update_action, (product["id"],))
+            p.close()
+            p.join()
 
 
 def generate_description(id):
     product = Product(id)
     product.description.warm_description_blocks()
     for platform, block in product.description.description_blocks.items():
         key = platform.split(":")[-1]
@@ -104,15 +116,16 @@
         for product in Database(Product.SETTINGS.PRODUCT_DB).pages():
             p.apply_async(description_check_action, (product["id"],))
         p.close()
         p.join()
 
 
 @app.command()
-def cache_clean():
+def cache_clean(id: Optional[str] = typer.Option(None)):
+    # TODO: сделать удаление по ID
     KeyDBCache().clean(r"[blocks|pages|databases]*")
 
 
 def cache_warm_func(id):
     product = Product(id)
     product.price.now
     product.kit
@@ -127,15 +140,20 @@
 
 
 @app.command()
 def cache_warm(
     only_exists: bool = typer.Option(False),
     single: bool = typer.Option(False),
     only_edited: bool = typer.Option(True),
+    sku: Optional[str] = typer.Option(None),
 ):
+    if sku:
+        cache_warm_func(Product.get(sku).id)
+        return
+
     if single:
         with Database(
             Product.SETTINGS.PRODUCT_DB, notion=Notion(caching=True)
         ) as database:
             params = {}
             if only_edited and database.get_update_time():
                 print(f"Фильтрация от даты: {database.get_update_time()}")
```

### Comparing `gdshoplib-1.8.0/gdshoplib/core/settings.py` & `gdshoplib-1.9.0/gdshoplib/core/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 class PriceSettins(BaseSettings):
     # Базовые коэфиценты цены
     PRICE_VAT_RATIO: float = 0.16
     PRICE_NEITRAL_RATIO: float = 0.40
     PRICE_PROFIT_RATIO: float = 0.60
-    EURO_PRICE: int = 75
+    EURO_PRICE: int = 72
 
 
 class RecurrentCommonExpenseSettings(BaseSettings):
     # Общие месячные расходы
     CLOUD_HOSTING_MONTH: int = 2400
     PLATFORMS_MONTH: int = 2000
     AD_MONTH: int = 3000  # Рассход на общие рекламные компании
@@ -98,7 +98,12 @@
     VK_BASEPATH: str = "https://api.vk.com/method/"
     VK_API_VERSION: str = "5.131"
     VK_GROUP_ID: str = "215870481"
     VK_CLIENT_ID: str = "51521300"
     VK_USER_SCOPE: str = "notify,friends,photos,audio,video,stories,pages,status,notes,wall,ads,offline,docs,groups,notifications,stats,email,market"
     VK_SECRET_KEY: Optional[str]
     VK_USER_ACCESS_TOKEN: Optional[str]
+
+
+class AVITOSettings(BaseSettings):
+    AVITO_CLIENT_ID: str = "PjsDDbv2OD294pmW1aak"
+    AVITO_SECRET: str
```

### Comparing `gdshoplib-1.8.0/gdshoplib/packages/cache.py` & `gdshoplib-1.9.0/gdshoplib/packages/cache.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/packages/feed.py` & `gdshoplib-1.9.0/gdshoplib/packages/feed.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/packages/lang.py` & `gdshoplib-1.9.0/gdshoplib/packages/lang.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/packages/s3.py` & `gdshoplib-1.9.0/gdshoplib/packages/s3.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/services/notion/README.md` & `gdshoplib-1.9.0/gdshoplib/services/notion/README.md`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/services/notion/base.py` & `gdshoplib-1.9.0/gdshoplib/services/notion/base.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/services/notion/block.py` & `gdshoplib-1.9.0/gdshoplib/services/notion/block.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/services/notion/database.py` & `gdshoplib-1.9.0/gdshoplib/services/notion/database.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/services/notion/manager.py` & `gdshoplib-1.9.0/gdshoplib/services/notion/manager.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/services/notion/notion.py` & `gdshoplib-1.9.0/gdshoplib/services/notion/notion.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/services/notion/page.py` & `gdshoplib-1.9.0/gdshoplib/services/notion/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dateutil import parser
+from dateutil.parser import parse
 
 from gdshoplib.services.notion.base import BasePage
 from gdshoplib.services.notion.block import Block
 from gdshoplib.services.notion.notion import Notion
 
 
 class Page(BasePage):
@@ -72,49 +72,67 @@
 
     def relation_list_handler(self, page_ids):
         result = []
         for _id in page_ids:
             result.append(Page(_id["id"]))
         return result
 
+    def date_handler(self, date):
+        if not date:
+            return
+        elif "start" in date:
+            return parse(date["start"]).date()
+
+        return parse(date).date()
+
     @property
     def properties_keys_map(self):
         return {
             "title": (dict(name="Name", id="title"),),
             "edited_by": (dict(name="Last edited by", id="~%7BrF"),),
-            "price_sale_10": (dict(name="Скидка, 10%", id="%7Bh%7D%7B"),),
-            "price_general": (dict(name="Ходовая", id="x%3A%5Ci"),),
-            "created_time": (dict(name="Created time", id="v%5Dsj"),),
+            "created_time": (
+                dict(name="Created time", id="v%5Dsj", handler=self.date_handler),
+            ),
             "short_description": (dict(name="Короткое описание", id="u_tU"),),
             "size": (dict(name="Размер", id="taW%3B"),),
             "notes_field": (dict(name="Примечания", id="sXND"),),
-            "price_buy": (dict(name="Закупочная", id="pyiW"),),
             "quantity": (dict(name="Кол-во", id="pXTy"),),
-            "price_neutral": (dict(name="Себестоимость", id="opcQ"),),
-            "edited_time": (dict(name="Last edited time", id="mVEw"),),
-            "price_sale_20": (dict(name="Скидка, 20%", id="cPu~"),),
+            "edited_time": (
+                dict(name="Last edited time", id="mVEw", handler=self.date_handler),
+            ),
             "collection": (dict(name="Коллекция", id="W%5BhI"),),
-            "price_base": (dict(name="Безубыточность", id="VmWm"),),
             "name": (dict(name="Название на русском", id="Tss%5D"),),
             "created_by": (dict(name="Created by", id="TbyK"),),
             "kit_field": (
                 dict(
                     name="Комплект", id="QV%5D%5D", handler=self.relation_list_handler
                 ),
             ),
             "tags_field": (dict(name="Теги", id="MqdC"),),
             "status_description": (dict(name="Описание", id="MUl%7C"),),
             "color": (dict(name="Цвет", id="Jvku"),),
-            "price_now": (dict(name="Текущая цена", id="Ddaz"),),
             "specifications_field": (
                 dict(name="Материалы / Характеристики", id="COmf"),
             ),
-            "status_publication": (dict(name="Публикация", id="BeEA"),),
+            "price_neitral": (dict(name="Безубыточность", id="VmWm"),),
+            "price_now": (dict(name="Текущая Цена", id="Ddaz"),),
+            "price_kit": (dict(name="Цена комплекта", id="Dwfs"),),
+            "price_current_discount": (dict(name="Текущая Скидка", id="syrp"),),
+            "price_agent": (dict(name="Агентская Цена", id="vC%5E%3D"),),
+            "price_agent_kit": (dict(name="Агентский комплект", id="M%60HY"),),
+            "discount_from_date": (
+                dict(name="Дата поставки", id="%60_a%3D", handler=self.date_handler),
+            ),
+            "badge_field": (
+                dict(name="🎖️ Бейджи", id="%3CU_H", handler=self.relation_list_handler),
+            ),
+            "file": (dict(name="Файл", id="uK%3CN"),),
+            "coordinates": (dict(name="Координаты", id="XU%7C%3F"),),
+            "transparency": (dict(name="Прозрачность", id="RHj%5B"),),
             "sku": (dict(name="Наш SKU", id="BKOs"),),
-            "price_sale_15": (dict(name="Скидка, 15%", id="BJPc"),),
             "sku_s": (dict(name="SKU поставщика", id="BHve"),),
             "price_eur": (dict(name="Цена (eur)", id="AyqD"),),
             "platforms": (
                 dict(name="Платформы", id="%40Q~A", handler=self.relation_list_handler),
             ),
             "brand": (
                 dict(name="Бренд", id="gk%40%3B", handler=self.relation_handler),
@@ -139,24 +157,24 @@
             "number": lambda data: data["number"] or 0,
             "title": lambda data: data["title"][0]["text"]["content"],
             "select": lambda data: data.get("select").get("name")
             if data.get("select")
             else None,
             "multi_select": lambda data: data,
             "status": lambda data: data["status"]["name"],
-            "date": lambda data: data,
+            "date": lambda data: data["date"],
             "formula": lambda data: data["formula"]["number"],
             "relation": lambda data: data["relation"],
             "rollup": lambda data: data,
             "people": lambda data: data,
             "files": lambda data: data,
             "checkbox": lambda data: data,
             "url": lambda data: data["url"],
             "email": lambda data: data,
             "phone_number": lambda data: data,
-            "created_time": lambda data: parser(data["created_time"]),
+            "created_time": lambda data: parse(data["created_time"]),
             "created_by": lambda data: str(data["created_by"]),
-            "last_edited_time": lambda data: parser(data["last_edited_time"]),
+            "last_edited_time": lambda data: parse(data["last_edited_time"]),
             "last_edited_by": lambda data: str(data["last_edited_by"]),
             "image": lambda data: data["image"]["file"]["url"],
             "video": lambda data: data["video"]["file"]["url"],
         }
```

### Comparing `gdshoplib-1.8.0/gdshoplib/services/vk/market.py` & `gdshoplib-1.9.0/gdshoplib/services/vk/market.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/services/vk/vk.py` & `gdshoplib-1.9.0/gdshoplib/services/vk/vk.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/templates/basic.txt` & `gdshoplib-1.9.0/gdshoplib/templates/basic.txt`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/templates/ula.txt` & `gdshoplib-1.9.0/gdshoplib/templates/ula.txt`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/gdshoplib/templates/vk.txt` & `gdshoplib-1.9.0/gdshoplib/templates/vk.txt`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.8.0/pyproject.toml` & `gdshoplib-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gdshoplib"
-version = "1.8.0"
+version = "1.9.0"
 description = ""
 authors = ["Nikolay Baryshnikov <root@k0d.ru>"]
 packages=[
     { include = "gdshoplib" },
 ]
 license="MIT"
 readme="README.md"
```

### Comparing `gdshoplib-1.8.0/setup.py` & `gdshoplib-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['gdshoplib = gdshoplib:application']}
 
 setup_kwargs = {
     'name': 'gdshoplib',
-    'version': '1.8.0',
+    'version': '1.9.0',
     'description': '',
     'long_description': '# Библиотека для управления магазином gdshop\n\nПользовательские объекты для высокоуровневой работы без привязки к слою данных. Предоставляет Python like интерфейс для работы с объектами\n\n## Finance\n\n- [ ] Информация о состоянии счетов\n- [ ] Операций с финансами\n- [ ] Статистика по финансам за периоды + Прогнозы\n- [ ] Расчет и контроль бюджетов\n- [ ] Сбор информации с площадок по финансам\n- [ ] Генерация отчетов\n- [x] Генерация цен по коэфицентам\n\n## Marketing\n\n- [ ] Статистика рекламных компаний\n- [ ] Управление рекламными компаниями\n- [ ] Статистика воронок\n- [ ] Выгрузка информации с площадок\n- [ ] Генерация отчетов\n- [ ] Статистика по товарам\n\n## Order\n- [ ] Получение информации о заказах\n\n## Product\n- [x] Получение информации о продукте\n- [ ] Обновление содержимого продукта\n- [x] Выгрузка информации о товаре в фид\n- [ ] Работа с закупками\n- [ ] Оценка материалов\n- [x] Работа с media\n- [x] Работа с description\n- [x] Выгрузка меда в S3\n\n## Platform\n- [x] Генерация товарных фидов\n\n\n# Полезные ссылки\n\n## Описание товарного фида\n\nhttps://yandex.ru/support/partnermarket/export/yml.html\nhttps://drive.google.com/file/d/1kkKa0KU7iNOszyC2oQSGmHNwp3sRGKFb/view',
     'author': 'Nikolay Baryshnikov',
     'author_email': 'root@k0d.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/p141592',
```

### Comparing `gdshoplib-1.8.0/PKG-INFO` & `gdshoplib-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdshoplib
-Version: 1.8.0
+Version: 1.9.0
 Summary: 
 Home-page: https://github.com/p141592
 License: MIT
 Author: Nikolay Baryshnikov
 Author-email: root@k0d.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

