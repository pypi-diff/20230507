# Comparing `tmp/qtex-0.0.4.tar.gz` & `tmp/qtex-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtex-0.0.4.tar", last modified: Wed May  3 01:05:27 2023, max compression
+gzip compressed data, was "qtex-0.0.5.tar", last modified: Sun May  7 02:20:18 2023, max compression
```

## Comparing `qtex-0.0.4.tar` & `qtex-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-03 01:05:27.781033 qtex-0.0.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:03:44.000000 qtex-0.0.4/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-05-03 01:05:27.781033 qtex-0.0.4/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-03 01:05:27.777033 qtex-0.0.4/qtex/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:19:14.000000 qtex-0.0.4/qtex/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-03 01:05:27.781033 qtex-0.0.4/qtex/jq/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:19:37.000000 qtex-0.0.4/qtex/jq/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-03 01:05:27.781033 qtex-0.0.4/qtex/jq/etl/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:54:50.000000 qtex-0.0.4/qtex/jq/etl/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-05-03 01:04:46.000000 qtex-0.0.4/qtex/jq/etl/factor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1899 2023-05-02 01:56:55.000000 qtex-0.0.4/qtex/jq/persist_ext.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-03 01:05:27.781033 qtex-0.0.4/qtex/jq/sync/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:58:58.000000 qtex-0.0.4/qtex/jq/sync/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1221 2023-05-03 01:04:37.000000 qtex-0.0.4/qtex/jq/sync/position.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2524 2023-05-03 01:04:18.000000 qtex-0.0.4/qtex/jq/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-03 01:05:27.000000 qtex-0.0.4/qtex/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-03 01:05:27.781033 qtex-0.0.4/qtex.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-05-03 01:05:27.000000 qtex-0.0.4/qtex.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      375 2023-05-03 01:05:27.000000 qtex-0.0.4/qtex.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-03 01:05:27.000000 qtex-0.0.4/qtex.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-02 02:06:42.000000 qtex-0.0.4/qtex.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-05-03 01:05:27.000000 qtex-0.0.4/qtex.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-03 01:05:27.000000 qtex-0.0.4/qtex.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-03 01:05:27.781033 qtex-0.0.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      698 2023-05-02 02:07:22.000000 qtex-0.0.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.117449 qtex-0.0.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:03:44.000000 qtex-0.0.5/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-05-07 02:20:18.117449 qtex-0.0.5/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.113449 qtex-0.0.5/qtex/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:19:14.000000 qtex-0.0.5/qtex/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.117449 qtex-0.0.5/qtex/app/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 03:52:06.000000 qtex-0.0.5/qtex/app/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9965 2023-05-04 04:14:21.000000 qtex-0.0.5/qtex/app/persist_universe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      374 2023-04-28 21:57:05.000000 qtex-0.0.5/qtex/env_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.117449 qtex-0.0.5/qtex/jq/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:19:37.000000 qtex-0.0.5/qtex/jq/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.117449 qtex-0.0.5/qtex/jq/etl/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:54:50.000000 qtex-0.0.5/qtex/jq/etl/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4462 2023-05-07 01:58:29.000000 qtex-0.0.5/qtex/jq/etl/factor_info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6254 2023-05-07 02:16:55.000000 qtex-0.0.5/qtex/jq/etl/factor_values.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1899 2023-05-02 01:56:55.000000 qtex-0.0.5/qtex/jq/persist_ext.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.117449 qtex-0.0.5/qtex/jq/sync/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:58:58.000000 qtex-0.0.5/qtex/jq/sync/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1224 2023-05-06 02:37:06.000000 qtex-0.0.5/qtex/jq/sync/position.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1928 2023-05-04 00:04:51.000000 qtex-0.0.5/qtex/jq/univ.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2849 2023-05-07 01:58:58.000000 qtex-0.0.5/qtex/jq/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-05-07 02:20:02.000000 qtex-0.0.5/qtex/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.117449 qtex-0.0.5/qtex.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-05-07 02:20:18.000000 qtex-0.0.5/qtex.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      494 2023-05-07 02:20:18.000000 qtex-0.0.5/qtex.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-07 02:20:18.000000 qtex-0.0.5/qtex.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-02 02:06:42.000000 qtex-0.0.5/qtex.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-05-07 02:20:18.000000 qtex-0.0.5/qtex.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-07 02:20:18.000000 qtex-0.0.5/qtex.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-07 02:20:18.117449 qtex-0.0.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      698 2023-05-02 02:07:22.000000 qtex-0.0.5/setup.py
```

### Comparing `qtex-0.0.4/qtex/jq/etl/factor.py` & `qtex-0.0.5/qtex/jq/persist_ext.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 import pandas as pd
-import qtc.utils.datetime_utils as dtu
+import jqfactor as jqf
+import qtc.utils.cipher_utils as cu
 import qtc.utils.misc_utils as mu
+import qtc.utils.datetime_utils as dtu
+
+import qtex.jq.utils
 import qtex.jq.utils as jqu
 import logging
 logger = logging.getLogger()
 
 
-DATA_TYPE_CONFIG = dict()
+# DB_CONFIG = {
+#     'HOST': '124.222.142.29',
+#     'PORT': 7423,
+#     'USER': 's_heimdal_etl',
+#     'PASSWORD': '390f1c1c05140241445767',
+#     'DATABASE': 'CN-EQUITY-VENDOR'
+# }
 
-def persist_cne5(dateid, securities=None,
-                 **db_config):
-    global DATA_TYPE_CONFIG
-
-    datestr = dtu.dateid_to_datestr(dateid=dateid)
-    if securities is None:
-        securities = get_all_securities(types=['stock'], date=datestr)
-        securities = securities.index.to_list()
-    else:
-        securities = list(mu.iterable_to_tuple(securities, raw_type='str'))
 
-    if len(securities) == 0:
+def persist_target_positions(dateid, target_positions,
+                             **kwargs):
+    if target_positions is None or len(target_positions)==0:
         return None
 
-    factor_names = ['size', 'beta', 'momentum', 'residual_volatility', 'non_linear_size',
-                    'book_to_price_ratio', 'liquidity', 'earnings_yield', 'growth', 'leverage']
-
-    import jqfactor as jqf
-    factor_data = jqf.get_factor_values(
-        securities=securities,
-        factors=factor_names,
-        start_date=datestr, end_date=datestr
-    )
-
-    data = pd.concat([factor_data[fn].unstack().to_frame(fn) for fn in factor_data.keys()], axis=1)
-    data.index.names = ['ts_code', 'trade_date']
-    data.reset_index(inplace=True)
-    data['trade_date'] = data['trade_date'].dt.strftime('%Y%m%d').astype(int)
-    data['ts_code'] = data['ts_code'].apply(lambda x: x.replace('.XSHE', '.SZ').replace('.XSHG', 'SH'))
-    logger.info(f'data.shape={data.shape}. Examples:\n{data.head()}')
-
-    conn, database = jqu.get_conn_data_type(data_type='CNE5',
-                                            **db_config)
-    schema = 'joinquant'
-    table_name = 'CNE5'
+    cols =['AccountId', 'StrategyId', 'DateId', 'SecurityCode', 'SideId',
+           'Signal', 'Quantity', 'MV', 'Weight']
+    cols = [col for col in cols if col in target_positions.columns]
+    data = target_positions[cols]
+
+    user_d, password_d, database_d = \
+        qtex.jq.utils.DATA_TYPE_CONFIG.get('TARGET_POSITION',
+                                           ('s_heimdal_trading', '390f1c1c05140241445767', 'TRADING'))
+    if 'user' not in kwargs:
+        user = user_d
+    if 'password' not in kwargs:
+        password = password_d
+    if 'database' not in kwargs:
+        database = database_d
+
+    conn = jqu.get_conn(user=user, password=password, database=database)
+    schema = 'signal'
+    table_name = 'TargetPosition'
     # upsert_method = dbu.create_upsert_method(db_code=database, schema=schema,
     #                                          extra_update_fields={'UpdateDateTime': "NOW()"})
 
-    # conn.execute(f'DELETE FROM "{schema}"."{table_name}" WHERE "DateId"={dateid}')
     num_rows = data.to_sql(table_name,
                            con=conn, schema=schema,
                            if_exists='append', index=False)
 
     logger.info(f'{table_name} with shape {data.shape} on dateid={dateid} '
                 f'persisted into "{database}"."{schema}"."{table_name}" .')
 
-    return data
+    return data
```

### Comparing `qtex-0.0.4/qtex/jq/sync/position.py` & `qtex-0.0.5/qtex/jq/sync/position.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import qtex.jq.utils as jqu
 import logging
 logger = logging.getLogger()
 
 
-DATA_TYPE_CONFIG = dict()
+DATA_TYPE_DB_CONFIG = dict()
 
 def persist_target_positions(dateid, target_positions,
                              **db_config):
     if target_positions is None or len(target_positions)==0:
         return None
 
     cols =['AccountId', 'StrategyId', 'DateId', 'SecurityCode', 'SideId',
```

### Comparing `qtex-0.0.4/qtex/jq/utils.py` & `qtex-0.0.5/qtex/jq/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 import os
 import pandas as pd
 import qtc.utils.db_utils as dbu
 import qtc.utils.cipher_utils as cu
 
 
-# def get_conn(host='124.222.142.29',
-#              port=7423,
-#              user=None,
-#              password=None,
-#              database=None):
 def get_conn(**db_config):
     db_type = db_config.get('db_type', 'POSTGRES')
     host = db_config.get('host', os.getenv('DB_HOST', None))
     port = db_config.get('port', os.getenv('DB_PORT', None))
     user = db_config.get('user', os.getenv('DB_USER', None))
     password = db_config.get('password', os.getenv('DB_PASSWORD', None))
     database = db_config.get('database', os.getenv('DB_DATABASE', None))
@@ -26,27 +21,31 @@
         database=database
     )
 
     return conn
 
 
 def get_conn_data_type(data_type, **db_config):
-    import qtex.jq.etl.factor as etlf
+    import qtex.jq.etl.factor_info as etlfi
+    import qtex.jq.etl.factor_values as etlfv
     import qtex.jq.sync.position as syncp
 
-    DATA_TYPE_CONFIG_MAP = {
-        'CNE5': etlf.DATA_TYPE_CONFIG,
-        'TARGET_POSITION': syncp.DATA_TYPE_CONFIG
+    DATA_TYPE_DB_CONFIG_MAP = {
+        'FACTOR_GROUP': etlfi.DATA_TYPE_DB_CONFIG,
+        'FACTOR_INFO': etlfi.DATA_TYPE_DB_CONFIG,
+        'CNE5': etlfv.DATA_TYPE_DB_CONFIG,
+        'FACTOR_VALUE': etlfv.DATA_TYPE_DB_CONFIG,
+        'TARGET_POSITION': syncp.DATA_TYPE_DB_CONFIG
     }
 
-    data_type_config = DATA_TYPE_CONFIG_MAP[data_type]
+    data_type_db_config = DATA_TYPE_DB_CONFIG_MAP.get(data_type, dict())
 
     db_type_d, host_d, port_d, user_d, password_d, database_d = \
-        data_type_config.get(data_type,
-                             ('POSTGRES', None, None, None, None, None))
+        data_type_db_config.get(data_type,
+                                ('POSTGRES', None, None, None, None, None))
 
     db_type = db_config.get('db_type', db_type_d)
     host = db_config.get('host', host_d)
     port = db_config.get('port', port_d)
     user = db_config.get('user', user_d)
     password = db_config.get('password', password_d)
     database = db_config.get('database', database_d)
@@ -72,13 +71,21 @@
         factors=factors,
         start_date=start_date, end_date=end_date, count=count
     )
 
     scores = pd.concat(scores)
     scores.index.names = ['factor_code', 'trade_date']
 
-    if count==1 and transpose:
-#         scores = scores.droplevel(level='Date').T
-        scores.index = scores.index.droplevel(level='Date')
-        scores = scores.T
+    if count==1:
+        if transpose:
+    #         scores = scores.droplevel(level='Date').T
+            scores.index = scores.index.droplevel(level='trade_date')
+            scores = scores.T
+    else:
+        if transpose:
+            scores = scores.T.stack()
 
-    return scores
+    return scores
+
+
+def produce_factor_id(source_id, factor_code):
+    return int(int(str(source_id).ljust(3, '0')) * 1e6 + hash(factor_code) % (1e6))
```

### Comparing `qtex-0.0.4/setup.py` & `qtex-0.0.5/setup.py`

 * *Files identical despite different names*

