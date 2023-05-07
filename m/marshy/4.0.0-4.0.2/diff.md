# Comparing `tmp/marshy-4.0.0.tar.gz` & `tmp/marshy-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/marshy-4.0.0.tar", last modified: Tue Apr 18 21:22:40 2023, max compression
+gzip compressed data, was "marshy-4.0.2.tar", last modified: Sun May  7 16:11:02 2023, max compression
```

## Comparing `marshy-4.0.0.tar` & `marshy-4.0.2.tar`

### file list

```diff
@@ -1,79 +1,49 @@
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/
--rw-r--r--   0 tofarr     (501) staff       (20)     1069 2021-09-27 22:36:51.000000 marshy-4.0.0/LICENSE
--rw-r--r--   0 tofarr     (501) staff       (20)     8717 2023-04-18 21:22:40.000000 marshy-4.0.0/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     8251 2022-11-30 22:13:29.000000 marshy-4.0.0/README.md
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/marshy/
--rw-r--r--   0 tofarr     (501) staff       (20)     1226 2021-11-14 22:08:58.000000 marshy-4.0.0/marshy/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-18 21:15:19.000000 marshy-4.0.0/marshy/__version__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       43 2021-09-25 17:26:10.000000 marshy-4.0.0/marshy/errors.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/marshy/factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2021-09-25 22:20:47.000000 marshy-4.0.0/marshy/factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4879 2022-11-30 22:09:24.000000 marshy-4.0.0/marshy/factory/dataclass_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      727 2021-09-28 02:53:11.000000 marshy-4.0.0/marshy/factory/enum_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      643 2021-11-05 23:12:05.000000 marshy-4.0.0/marshy/factory/factory_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1848 2022-08-11 16:57:36.000000 marshy-4.0.0/marshy/factory/impl_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1003 2022-11-30 21:49:19.000000 marshy-4.0.0/marshy/factory/list_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      774 2022-01-23 15:06:09.000000 marshy-4.0.0/marshy/factory/marshaller_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1220 2021-09-28 02:53:11.000000 marshy-4.0.0/marshy/factory/optional_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1241 2022-01-24 23:28:38.000000 marshy-4.0.0/marshy/factory/tuple_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1082 2021-09-28 02:53:11.000000 marshy-4.0.0/marshy/factory/union_marshaller_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/marshy/marshaller/
--rw-r--r--   0 tofarr     (501) staff       (20)      519 2021-11-03 13:37:59.000000 marshy-4.0.0/marshy/marshaller/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      452 2021-10-09 16:07:39.000000 marshy-4.0.0/marshy/marshaller/as_str_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      464 2022-02-06 00:41:38.000000 marshy-4.0.0/marshy/marshaller/bool_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      518 2021-11-03 13:39:03.000000 marshy-4.0.0/marshy/marshaller/datetime_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      734 2021-09-28 17:30:24.000000 marshy-4.0.0/marshy/marshaller/deferred_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1209 2023-04-18 21:16:33.000000 marshy-4.0.0/marshy/marshaller/enum_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      752 2022-01-24 23:12:00.000000 marshy-4.0.0/marshy/marshaller/iterable_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      518 2021-12-07 14:44:56.000000 marshy-4.0.0/marshy/marshaller/json_str_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      480 2022-02-06 00:41:38.000000 marshy-4.0.0/marshy/marshaller/marshaller_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      352 2021-09-28 02:53:11.000000 marshy-4.0.0/marshy/marshaller/no_op_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1825 2022-07-31 11:30:41.000000 marshy-4.0.0/marshy/marshaller/obj_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      761 2021-09-28 02:53:11.000000 marshy-4.0.0/marshy/marshaller/optional_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      453 2021-09-28 17:30:50.000000 marshy-4.0.0/marshy/marshaller/primitive_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1729 2022-07-31 11:31:15.000000 marshy-4.0.0/marshy/marshaller/property_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      913 2022-02-10 02:40:00.000000 marshy-4.0.0/marshy/marshaller/tuple_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1861 2021-11-17 23:59:03.000000 marshy-4.0.0/marshy/marshaller/type_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1539 2021-11-18 00:03:28.000000 marshy-4.0.0/marshy/marshaller/union_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2141 2022-07-26 13:23:28.000000 marshy-4.0.0/marshy/marshaller_context.py
--rw-r--r--   0 tofarr     (501) staff       (20)      199 2021-12-07 03:19:47.000000 marshy-4.0.0/marshy/types.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1009 2021-10-29 15:31:13.000000 marshy-4.0.0/marshy/utils.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/marshy.egg-info/
--rw-r--r--   0 tofarr     (501) staff       (20)     8717 2023-04-18 21:22:39.000000 marshy-4.0.0/marshy.egg-info/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     2192 2023-04-18 21:22:39.000000 marshy-4.0.0/marshy.egg-info/SOURCES.txt
--rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-04-18 21:22:39.000000 marshy-4.0.0/marshy.egg-info/dependency_links.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-18 21:22:39.000000 marshy-4.0.0/marshy.egg-info/requires.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       34 2023-04-18 21:22:39.000000 marshy-4.0.0/marshy.egg-info/top_level.txt
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/marshy_config_default/
--rw-r--r--   0 tofarr     (501) staff       (20)     1819 2022-01-24 23:05:39.000000 marshy-4.0.0/marshy_config_default/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-18 21:22:40.000000 marshy-4.0.0/setup.cfg
--rw-r--r--   0 tofarr     (501) staff       (20)      753 2021-09-28 02:54:22.000000 marshy-4.0.0/setup.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/test/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2021-09-26 14:52:20.000000 marshy-4.0.0/test/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/test/performance/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2021-10-09 15:23:45.000000 marshy-4.0.0/test/performance/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      716 2021-10-09 15:20:22.000000 marshy-4.0.0/test/performance/fixtures.py
--rw-r--r--   0 tofarr     (501) staff       (20)      316 2021-10-09 15:28:35.000000 marshy-4.0.0/test/performance/marshmallow_performance.py
--rw-r--r--   0 tofarr     (501) staff       (20)      252 2021-10-09 15:28:35.000000 marshy-4.0.0/test/performance/marshy_performance.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4118 2021-12-07 14:44:39.000000 marshy-4.0.0/test/test_custom_marshalling.py
--rw-r--r--   0 tofarr     (501) staff       (20)      625 2022-07-31 11:39:59.000000 marshy-4.0.0/test/test_customize_exclude_dumped_values.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1704 2022-01-23 15:06:09.000000 marshy-4.0.0/test/test_factory_ordering.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1752 2022-07-26 13:42:12.000000 marshy-4.0.0/test/test_futures.py
--rw-r--r--   0 tofarr     (501) staff       (20)      975 2022-01-24 23:31:34.000000 marshy-4.0.0/test/test_immutable.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1612 2022-08-11 16:59:14.000000 marshy-4.0.0/test/test_impl_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      703 2021-09-28 02:53:11.000000 marshy-4.0.0/test/test_marshall_bool.py
--rw-r--r--   0 tofarr     (501) staff       (20)      710 2021-11-03 13:45:28.000000 marshy-4.0.0/test/test_marshall_datetime.py
--rw-r--r--   0 tofarr     (501) staff       (20)      765 2021-09-28 02:53:11.000000 marshy-4.0.0/test/test_marshall_deferred.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1116 2023-04-18 21:21:34.000000 marshy-4.0.0/test/test_marshall_enum.py
--rw-r--r--   0 tofarr     (501) staff       (20)      474 2021-12-07 14:43:04.000000 marshy-4.0.0/test/test_marshall_freeform.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1053 2022-02-02 23:23:37.000000 marshy-4.0.0/test/test_marshall_iterable.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3799 2022-02-09 16:01:32.000000 marshy-4.0.0/test/test_marshall_obj.py
--rw-r--r--   0 tofarr     (501) staff       (20)      368 2021-09-28 02:53:11.000000 marshy-4.0.0/test/test_marshall_optional.py
--rw-r--r--   0 tofarr     (501) staff       (20)      542 2021-09-28 02:53:11.000000 marshy-4.0.0/test/test_marshall_primitive.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3023 2022-11-30 22:11:46.000000 marshy-4.0.0/test/test_marshall_properties.py
--rw-r--r--   0 tofarr     (501) staff       (20)      627 2022-02-10 02:49:32.000000 marshy-4.0.0/test/test_marshall_tuple.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1223 2021-11-18 00:01:20.000000 marshy-4.0.0/test/test_marshall_type.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1898 2021-11-18 00:13:22.000000 marshy-4.0.0/test/test_marshall_union.py
--rw-r--r--   0 tofarr     (501) staff       (20)      355 2021-10-29 15:33:04.000000 marshy-4.0.0/test/test_marshall_uuid.py
--rw-r--r--   0 tofarr     (501) staff       (20)      795 2021-10-09 15:50:08.000000 marshy-4.0.0/test/test_performance.py
--rw-r--r--   0 tofarr     (501) staff       (20)      975 2021-12-07 03:33:25.000000 marshy-4.0.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:11:02.670094 marshy-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-07 16:10:53.000000 marshy-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-07 16:10:53.000000 marshy-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-05-07 16:11:02.670094 marshy-4.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:11:02.666094 marshy-4.0.2/marshy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:11:02.666094 marshy-4.0.2/marshy/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/dataclass_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/enum_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/factory_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/impl_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/list_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/marshaller_factory_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/optional_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/tuple_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/union_marshaller_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:11:02.670094 marshy-4.0.2/marshy/marshaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/as_str_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/bool_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/datetime_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/deferred_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/enum_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/iterable_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/json_str_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/marshaller_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/no_op_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/obj_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/optional_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/primitive_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/property_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/tuple_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/type_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/union_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:11:02.666094 marshy-4.0.2/marshy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-05-07 16:11:02.000000 marshy-4.0.2/marshy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-07 16:11:02.000000 marshy-4.0.2/marshy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:11:02.000000 marshy-4.0.2/marshy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-07 16:11:02.000000 marshy-4.0.2/marshy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 16:11:02.000000 marshy-4.0.2/marshy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:11:02.670094 marshy-4.0.2/marshy_config_default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy_config_default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 16:11:02.670094 marshy-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-07 16:10:53.000000 marshy-4.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `marshy-4.0.0/LICENSE` & `marshy-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `marshy-4.0.0/PKG-INFO` & `marshy-4.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: marshy
-Version: 4.0.0
+Version: 4.0.2
 Summary: A convention over configuration approach to object marshalling.
 Home-page: https://github.com/tofarr/marshy
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Marshy - Better Marshalling for Python.
 
 This project is a general purpose externalizer for python objects.
 (Like Marshmallow or Pedantic) The guiding philosophy is convention
 over configuration, with the aim of still making customizations as
@@ -284,18 +284,25 @@
 python -m timeit -s "
 from test.performance.marshmallow_performance import run
 run(1000)
 "
 ```
 
 
-## Building The Project
+## Release Proceedure
+
+![status](https://github.com/tofarr/marshy/actions/workflows/quality.yml/badge.svg?branch=main)
+
+The typical process here is:
+* Create a PR with changes. Merge these to main (The `Quality` workflows make sure that styling, linting, and code
+  code coverage standards are met).
+* New releases created in github are automatically uploaded to pypi
+
 
 You need an account on pypi before this will work:
 
 ```
 pip install setuptools wheel
 python setup.py sdist bdist_wheel
 pip install twine
 python -m twine upload dist/*
 ```
-
```

### Comparing `marshy-4.0.0/README.md` & `marshy-4.0.2/marshy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: marshy
+Version: 4.0.2
+Summary: A convention over configuration approach to object marshalling.
+Home-page: https://github.com/tofarr/marshy
+Author: Tim O'Farrell
+Author-email: tofarr@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # Marshy - Better Marshalling for Python.
 
 This project is a general purpose externalizer for python objects.
 (Like Marshmallow or Pedantic) The guiding philosophy is convention
 over configuration, with the aim of still making customizations as
 pain free as possible, based on python type hints.
 
@@ -269,17 +284,25 @@
 python -m timeit -s "
 from test.performance.marshmallow_performance import run
 run(1000)
 "
 ```
 
 
-## Building The Project
+## Release Proceedure
+
+![status](https://github.com/tofarr/marshy/actions/workflows/quality.yml/badge.svg?branch=main)
+
+The typical process here is:
+* Create a PR with changes. Merge these to main (The `Quality` workflows make sure that styling, linting, and code
+  code coverage standards are met).
+* New releases created in github are automatically uploaded to pypi
+
 
 You need an account on pypi before this will work:
 
 ```
 pip install setuptools wheel
 python setup.py sdist bdist_wheel
 pip install twine
 python -m twine upload dist/*
-```
+```
```

### Comparing `marshy-4.0.0/marshy/__init__.py` & `marshy-4.0.2/marshy/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import pkgutil
 from typing import Type, Any, Optional, ForwardRef, TypeVar
 import importlib
 
 from marshy.types import ExternalType
 
 _default_context = None
-T = TypeVar('T')
-CONFIG_MODULE_PREFIX = 'marshy_config_'
+T = TypeVar("T")
+CONFIG_MODULE_PREFIX = "marshy_config_"
 
 
-def get_default_context() -> ForwardRef('marshy.marshaller_context.MarshallerContext'):
+# pylint: disable=W0603
+def get_default_context() -> ForwardRef("marshy.marshaller_context.MarshallerContext"):
     global _default_context
     if not _default_context:
         _default_context = new_default_context()
     return _default_context
 
 
-def new_default_context() -> ForwardRef('marshy.marshaller_context.MarshallerContext'):
+def new_default_context() -> ForwardRef("marshy.marshaller_context.MarshallerContext"):
+    # pylint: disable=C0415
     from marshy.marshaller_context import MarshallerContext
+
     default_context = MarshallerContext()
     # Set up context based on naming convention
-    module_info = (m for m in pkgutil.iter_modules() if m.name.startswith(CONFIG_MODULE_PREFIX))
+    module_info = (
+        m for m in pkgutil.iter_modules() if m.name.startswith(CONFIG_MODULE_PREFIX)
+    )
     modules = [importlib.import_module(m.name) for m in module_info]
     modules.sort(key=lambda m: m.priority, reverse=True)
     for m in modules:
-        getattr(m, 'configure')(default_context)
+        getattr(m, "configure")(default_context)
     return default_context
 
 
 def load(type_: Type[T], to_load: ExternalType) -> T:
     return get_default_context().load(type_, to_load)
```

### Comparing `marshy-4.0.0/marshy/factory/dataclass_marshaller_factory.py` & `marshy-4.0.2/marshy/factory/dataclass_marshaller_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,87 +14,117 @@
 
 
 @dataclasses.dataclass
 class DataclassMarshallerFactory(MarshallerFactoryABC):
     priority: int = 100
     exclude_dumped_values: Tuple = tuple()
 
-    def create(self,
-               context: marshaller_context.MarshallerContext,
-               type_: Type) -> Optional[marshaller_abc.MarshallerABC]:
+    def create(
+        self, context: marshaller_context.MarshallerContext, type_: Type
+    ) -> Optional[marshaller_abc.MarshallerABC]:
         if not dataclasses.is_dataclass(type_):
             return
-        return dataclass_marshaller(type_, context, exclude_dumped_values=self.exclude_dumped_values)
+        return dataclass_marshaller(
+            type_, context, exclude_dumped_values=self.exclude_dumped_values
+        )
 
 
-def get_property_configs_for_type(type_: Type,
-                                  context: MarshallerContext,
-                                  include: Optional[List[str]] = None,
-                                  exclude: Optional[List[str]] = None,
-                                  exclude_dumped_values: Tuple = DataclassMarshallerFactory.exclude_dumped_values):
+def get_property_configs_for_type(
+    type_: Type,
+    context: MarshallerContext,
+    include: Optional[List[str]] = None,
+    exclude: Optional[List[str]] = None,
+    exclude_dumped_values: Tuple = DataclassMarshallerFactory.exclude_dumped_values,
+):
     property_configs = []
     for p in inspect.getmembers(type_, lambda o: isinstance(o, property)):
         name = p[0]
         if skip(name, include, exclude):
             continue
         prop = p[1]
         type_hints = get_type_hints(prop.fget)
-        if 'return' not in type_hints:
-            raise MarshallError(f'UnannotatedProperty:{type_}:{name}')
-        prop_type = type_hints.get('return')
+        if "return" not in type_hints:
+            raise MarshallError(f"UnannotatedProperty:{type_}:{name}")
+        prop_type = type_hints.get("return")
 
         prop_type = resolve_forward_refs(prop_type)
         marshaller = DeferredMarshaller[prop_type](prop_type, context)
-        property_config = PropertyConfig(name, marshaller, prop, load=bool(prop.fset),
-                                         exclude_dumped_values=exclude_dumped_values)
+        property_config = PropertyConfig(
+            name,
+            marshaller,
+            prop,
+            load=bool(prop.fset),
+            exclude_dumped_values=exclude_dumped_values,
+        )
         property_configs.append(property_config)
     return property_configs
 
 
 def skip(name: str, include: Optional[List[str]], exclude: Optional[List[str]]) -> bool:
     if include is not None and name not in include:
         return True
     if exclude is not None and name in exclude:
         return True
     return False
 
 
-def get_attr_configs_for_type(type_: Type,
-                              context: marshaller_context.MarshallerContext,
-                              include: Optional[List[str]] = None,
-                              exclude: Optional[List[str]] = None,
-                              exclude_dumped_values: Tuple = (None,)):
+# pylint: disable=R0913
+def get_attr_configs_for_type(
+    type_: Type,
+    context: marshaller_context.MarshallerContext,
+    include: Optional[List[str]] = None,
+    exclude: Optional[List[str]] = None,
+    exclude_dumped_values: Tuple = (None,),
+):
     # noinspection PyDataclass
     fields: List[dataclasses.Field] = dataclasses.fields(type_)
     try:
         types = get_type_hints(type_, globalns=None, localns=None)
-        attr_configs = [attr_config(internal_name=f.name, marshaller=DeferredMarshaller(types[f.name], context),
-                                    exclude_dumped_values=exclude_dumped_values)
-                        for f in fields if not skip(f.name, include, exclude)]
+        attr_configs = [
+            attr_config(
+                internal_name=f.name,
+                marshaller=DeferredMarshaller(types[f.name], context),
+                exclude_dumped_values=exclude_dumped_values,
+            )
+            for f in fields
+            if not skip(f.name, include, exclude)
+        ]
     except NameError:
         # Still supporting old style forward refs without futures...
-        attr_configs = [attr_config(internal_name=f.name, marshaller=DeferredMarshaller(f.type, context),
-                                    exclude_dumped_values=exclude_dumped_values)
-                        for f in fields if not skip(f.name, include, exclude)]
+        attr_configs = [
+            attr_config(
+                internal_name=f.name,
+                marshaller=DeferredMarshaller(f.type, context),
+                exclude_dumped_values=exclude_dumped_values,
+            )
+            for f in fields
+            if not skip(f.name, include, exclude)
+        ]
     return attr_configs
 
 
-def dataclass_marshaller(type_: Type,
-                         context: marshaller_context.MarshallerContext,
-                         custom_attr_configs: Optional[List[AttrConfig]] = None,
-                         custom_property_configs: Optional[List[PropertyConfig]] = None,
-                         include: Optional[List[str]] = None,
-                         exclude: Optional[List[str]] = None,
-                         exclude_dumped_values: Tuple = (None,)):
+def dataclass_marshaller(
+    type_: Type,
+    context: marshaller_context.MarshallerContext,
+    custom_attr_configs: Optional[List[AttrConfig]] = None,
+    custom_property_configs: Optional[List[PropertyConfig]] = None,
+    include: Optional[List[str]] = None,
+    exclude: Optional[List[str]] = None,
+    exclude_dumped_values: Tuple = (None,),
+):
     exclude_list = exclude or []
     if custom_attr_configs:
         exclude_list.extend(a.external_name for a in custom_attr_configs)
     if custom_property_configs:
         exclude_list.extend(p.external_name for p in custom_property_configs)
-    attr_configs = get_attr_configs_for_type(type_, context, include, exclude, exclude_dumped_values)
-    property_configs = get_property_configs_for_type(type_, context, include, exclude_list, exclude_dumped_values)
+    attr_configs = get_attr_configs_for_type(
+        type_, context, include, exclude, exclude_dumped_values
+    )
+    property_configs = get_property_configs_for_type(
+        type_, context, include, exclude_list, exclude_dumped_values
+    )
     attr_configs.extend(custom_attr_configs or [])
     property_configs.extend(custom_property_configs or [])
     marshaller = ObjMarshaller[type_](type_, attr_configs)
     if property_configs:
         marshaller = PropertyMarshaller(marshaller, tuple(property_configs))
     return marshaller
```

### Comparing `marshy-4.0.0/marshy/factory/enum_marshaller_factory.py` & `marshy-4.0.2/marshy/factory/enum_marshaller_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 
 @dataclass
 class EnumMarshallerFactory(MarshallerFactoryABC):
     priority: int = 100
     allow_unknown: bool = False
 
-    def create(self,
-               context: marshaller_context.MarshallerContext,
-               type_: Type) -> Optional[marshaller_abc.MarshallerABC]:
+    def create(
+        self, context: marshaller_context.MarshallerContext, type_: Type
+    ) -> Optional[marshaller_abc.MarshallerABC]:
         if inspect.isclass(type_) and issubclass(type_, Enum):
             return EnumMarshaller[type_](type_, self.allow_unknown)
```

### Comparing `marshy-4.0.0/marshy/factory/factory_marshaller_factory.py` & `marshy-4.0.2/marshy/factory/factory_marshaller_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from dataclasses import dataclass
 from typing import Type, Optional
 
 from marshy import marshaller_context
 from marshy.factory.marshaller_factory_abc import MarshallerFactoryABC
 from marshy.marshaller import marshaller_abc
 
-MARSHALLER_FACTORY = '__marshaller_factory__'
+MARSHALLER_FACTORY = "__marshaller_factory__"
 
 
 @dataclass
 class FactoryMarshallerFactory(MarshallerFactoryABC):
     priority: int = 110
 
-    def create(self,
-               context: marshaller_context.MarshallerContext,
-               type_: Type) -> Optional[marshaller_abc.MarshallerABC]:
+    def create(
+        self, context: marshaller_context.MarshallerContext, type_: Type
+    ) -> Optional[marshaller_abc.MarshallerABC]:
         factory = getattr(type_, MARSHALLER_FACTORY, None)
         if factory is not None:
             return factory(context)
```

### Comparing `marshy-4.0.0/marshy/factory/impl_marshaller_factory.py` & `marshy-4.0.2/marshy/factory/impl_marshaller_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,45 +4,51 @@
 from marshy import marshaller_context, get_default_context
 from marshy.factory.marshaller_factory_abc import MarshallerFactoryABC
 from marshy.factory.union_marshaller_factory import name_for_type
 from marshy.marshaller import marshaller_abc
 from marshy.marshaller.deferred_marshaller import DeferredMarshaller
 from marshy.marshaller.union_marshaller import UnionMarshaller
 
-MARSHALLER_FACTORY = '__marshaller_factory__'
+MARSHALLER_FACTORY = "__marshaller_factory__"
 
 
 @dataclass
 class ImplMarshallerFactory(MarshallerFactoryABC):
     base: Type
     impls: Set[Type] = field(default_factory=set)
     priority: int = 110
 
-    def create(self,
-               context: marshaller_context.MarshallerContext,
-               type_: Type) -> Optional[marshaller_abc.MarshallerABC]:
+    def create(
+        self, context: marshaller_context.MarshallerContext, type_: Type
+    ) -> Optional[marshaller_abc.MarshallerABC]:
         if type_ is self.base:
-            marshallers = {name_for_type(t): DeferredMarshaller[t](t, context) for t in self.impls}
+            marshallers = {
+                name_for_type(t): DeferredMarshaller[t](t, context) for t in self.impls
+            }
             return UnionMarshaller[self.base](self.base, marshallers)
 
     def add_impl(self, impl):
         self.impls.add(impl)
 
 
-def register_impl(base, impl, context: Optional[marshaller_context.MarshallerContext] = None):
+def register_impl(
+    base, impl, context: Optional[marshaller_context.MarshallerContext] = None
+):
     if context is None:
         context = get_default_context()
     for factory in context.get_factories():
         if isinstance(factory, ImplMarshallerFactory) and factory.base == base:
             factory.add_impl(impl)
             return
     factory = ImplMarshallerFactory(base)
     factory.add_impl(impl)
     context.register_factory(factory)
 
 
-def get_impls(base: Type, context: Optional[marshaller_context.MarshallerContext] = None) -> Set[Type]:
+def get_impls(
+    base: Type, context: Optional[marshaller_context.MarshallerContext] = None
+) -> Set[Type]:
     if context is None:
         context = get_default_context()
     for factory in context.get_factories():
         if isinstance(factory, ImplMarshallerFactory) and factory.base == base:
             return set(factory.impls)
```

### Comparing `marshy-4.0.0/marshy/factory/list_marshaller_factory.py` & `marshy-4.0.2/marshy/factory/list_marshaller_factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from marshy.marshaller.deferred_marshaller import DeferredMarshaller
 from marshy.marshaller.iterable_marshaller import IterableMarshaller
 
 
 @dataclass
 class ListMarshallerFactory(MarshallerFactoryABC):
     priority: int = 100
-    type_name_attr: str = '__type__'
+    type_name_attr: str = "__type__"
 
-    def create(self,
-               context: marshaller_context.MarshallerContext,
-               type_: Type) -> Optional[marshaller_abc.MarshallerABC]:
+    def create(
+        self, context: marshaller_context.MarshallerContext, type_: Type
+    ) -> Optional[marshaller_abc.MarshallerABC]:
         origin = typing_inspect.get_origin(type_)
         if origin in (list, set, frozenset):
             item_type = typing_inspect.get_args(type_)[0]
             item_marshaller = DeferredMarshaller(item_type, context)
             marshaller = IterableMarshaller[item_type](type_, item_marshaller, origin)
             return marshaller
```

### Comparing `marshy-4.0.0/marshy/factory/optional_marshaller_factory.py` & `marshy-4.0.2/marshy/factory/optional_marshaller_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 from marshy.marshaller.optional_marshaller import OptionalMarshaller
 
 
 @dataclass
 class OptionalMarshallerFactory(MarshallerFactoryABC):
     priority: int = 100
 
-    def create(self,
-               context: marshaller_context.MarshallerContext,
-               type_: Type) -> Optional[marshaller_abc.MarshallerABC]:
+    def create(
+        self, context: marshaller_context.MarshallerContext, type_: Type
+    ) -> Optional[marshaller_abc.MarshallerABC]:
         origin = typing_inspect.get_origin(type_)
         if origin == Union:
             optional_type = get_optional_type(type_)
             if optional_type:
-                return OptionalMarshaller[optional_type](context.get_marshaller(optional_type))
+                return OptionalMarshaller[optional_type](
+                    context.get_marshaller(optional_type)
+                )
 
 
 def get_optional_type(type_: Type) -> Optional[Type]:
     origin = typing_inspect.get_origin(type_)
     if origin == Union:
         args = typing_inspect.get_args(type_)
         if len(args) != 2:
```

### Comparing `marshy-4.0.0/marshy/factory/union_marshaller_factory.py` & `marshy-4.0.2/marshy/factory/union_marshaller_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 from marshy.marshaller.union_marshaller import UnionMarshaller
 
 
 @dataclass
 class UnionMarshallerFactory(MarshallerFactoryABC):
     priority: int = 90
 
-    def create(self,
-               context: marshaller_context.MarshallerContext,
-               type_: Type) -> Optional[marshaller_abc.MarshallerABC]:
+    def create(
+        self, context: marshaller_context.MarshallerContext, type_: Type
+    ) -> Optional[marshaller_abc.MarshallerABC]:
         origin = typing_inspect.get_origin(type_)
         if origin == Union:
-            marshallers = {name_for_type(t): DeferredMarshaller(t, context) for t in typing_inspect.get_args(type_)}
+            marshallers = {
+                name_for_type(t): DeferredMarshaller(t, context)
+                for t in typing_inspect.get_args(type_)
+            }
             return UnionMarshaller[type_](type_, marshallers)
 
 
 def name_for_type(type_: Type) -> str:
-    if hasattr(type_, '__origin__'):
+    if hasattr(type_, "__origin__"):
         return name_for_type(type_.__origin__)
-    return type_.__name__ if hasattr(type_, '__name__') else str(type_)
+    return type_.__name__ if hasattr(type_, "__name__") else str(type_)
```

### Comparing `marshy-4.0.0/marshy/marshaller/__init__.py` & `marshy-4.0.2/marshy/marshaller/__init__.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.0/marshy/marshaller/datetime_marshaller.py` & `marshy-4.0.2/marshy/marshaller/datetime_marshaller.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from marshy.marshaller.marshaller_abc import MarshallerABC
 
 
 class DatetimeMarshaller(MarshallerABC[ExternalType]):
     """
     Marshaller for datetime instances to iso format
     """
+
     def __init__(self):
         super().__init__(datetime)
 
     def load(self, item: str) -> datetime:
         loaded = datetime.fromisoformat(item)
         return loaded
```

### Comparing `marshy-4.0.0/marshy/marshaller/deferred_marshaller.py` & `marshy-4.0.2/marshy/marshaller/deferred_marshaller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from typing import TypeVar
 
 from marshy import ExternalType
 from marshy.marshaller.marshaller_abc import MarshallerABC
 from marshy.marshaller_context import MarshallerContext
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 @dataclass(frozen=True)
 class DeferredMarshaller(MarshallerABC[T]):
     marshaller_context: MarshallerContext
 
     def get_marshaller(self) -> MarshallerABC[T]:
```

### Comparing `marshy-4.0.0/marshy/marshaller/enum_marshaller.py` & `marshy-4.0.2/marshy/marshaller/enum_marshaller.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import TypeVar, Union
 
 from marshy.errors import MarshallError
 from marshy.marshaller.marshaller_abc import MarshallerABC
 
-T = TypeVar('T', bound=Enum)
-ERROR_PREFIX = 'INVALID_VALUE__'
+T = TypeVar("T", bound=Enum)
+ERROR_PREFIX = "INVALID_VALUE__"
 
 
 @dataclass(frozen=True)
 class EnumMarshaller(MarshallerABC[T]):
     """
     Marshaller for enums
     """
+
     allow_unknown: bool = False
 
     def load(self, item: Union[str, int, float]) -> T:
         try:
             loaded = self.marshalled_type[item]
             return loaded
         except KeyError as e:
             if self.allow_unknown:
                 pseudo_member = generate_pseudo_member(self.marshalled_type, item)
                 return pseudo_member
-            raise MarshallError(e)
+            raise MarshallError(e) from e
 
     def dump(self, item: T) -> Union[str, int, float]:
         dumped = item.name
         return dumped
 
 
+# pylint: disable=W0212
 def generate_pseudo_member(enum: T, value: Union[str, int, float]):
     pseudo_member = object.__new__(enum)
-    pseudo_member._name_ = f'{ERROR_PREFIX}{str(value).upper()}'
+    pseudo_member._name_ = f"{ERROR_PREFIX}{str(value).upper()}"
     pseudo_member._value_ = value
     # noinspection PyProtectedMember
     pseudo_member = enum._value2member_map_.setdefault(value, pseudo_member)
     return pseudo_member
```

### Comparing `marshy-4.0.0/marshy/marshaller/iterable_marshaller.py` & `marshy-4.0.2/marshy/marshaller/iterable_marshaller.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from dataclasses import dataclass
 from typing import TypeVar, Iterable, List, Callable, Iterator
 
 from marshy import ExternalType
 from marshy.marshaller.marshaller_abc import MarshallerABC
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 @dataclass(frozen=True)
 class IterableMarshaller(MarshallerABC[Iterable[T]]):
     """
     Marshaller for iterable types (lists)
     """
+
     item_marshaller: MarshallerABC[T]
     constructor: Callable[[Iterator[T]], Iterable[T]] = list
 
     def load(self, item: List[ExternalType]) -> Iterable[T]:
         loaded = self.constructor(self.item_marshaller.load(i) for i in item)
         return loaded
```

### Comparing `marshy-4.0.0/marshy/marshaller/json_str_marshaller.py` & `marshy-4.0.2/marshy/marshaller/json_str_marshaller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from typing import TypeVar
 
 from marshy.marshaller.marshaller_abc import MarshallerABC
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class JsonStrMarshaller(MarshallerABC[T]):
     """
     Marshaller for freeform json objects - they are interpreted as strings. (Due to technologies like graphql
     having a dislike for unstructured data)
     """
```

### Comparing `marshy-4.0.0/marshy/marshaller/obj_marshaller.py` & `marshy-4.0.2/marshy/marshaller/obj_marshaller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 from dataclasses import dataclass
 from typing import TypeVar, Tuple, Optional
 
 from marshy.marshaller.marshaller_abc import MarshallerABC
 from marshy.types import ExternalType
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 @dataclass(frozen=True)
 class AttrConfig:
     internal_name: str
     external_name: str
     marshaller: MarshallerABC
     load: bool
     dump: bool
     exclude_dumped_values: Tuple = ()
 
 
-def attr_config(marshaller: MarshallerABC,
-                internal_name: str,
-                external_name: Optional[str] = None,
-                load: bool = True,
-                dump: bool = True,
-                exclude_dumped_values: Tuple = tuple()) -> AttrConfig:
+# pylint: disable=R0913
+def attr_config(
+    marshaller: MarshallerABC,
+    internal_name: str,
+    external_name: Optional[str] = None,
+    load: bool = True,
+    dump: bool = True,
+    exclude_dumped_values: Tuple = tuple(),
+) -> AttrConfig:
     if external_name is None:
         external_name = internal_name
-    return AttrConfig(internal_name, external_name, marshaller, load, dump, exclude_dumped_values)
+    return AttrConfig(
+        internal_name, external_name, marshaller, load, dump, exclude_dumped_values
+    )
 
 
 @dataclass(frozen=True)
 class ObjMarshaller(MarshallerABC[T]):
     attr_configs: Tuple
 
     def load(self, item: ExternalType) -> T:
@@ -39,17 +44,19 @@
                 external_value = item[a.external_name]
                 value = a.marshaller.load(external_value)
                 kwargs[a.internal_name] = value
         loaded = self.marshalled_type(**kwargs)
         return loaded
 
     def dump(self, item: T) -> ExternalType:
-        if hasattr(item, 'get'):
+        if hasattr(item, "get"):
+
             def getter(obj, key):
                 return obj.get(key)
+
         else:
             getter = getattr
 
         dumped = {}
         for a in self.attr_configs:
             if a.dump:
                 value = getter(item, a.internal_name)
```

### Comparing `marshy-4.0.0/marshy/marshaller/optional_marshaller.py` & `marshy-4.0.2/marshy/marshaller/optional_marshaller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TypeVar, Optional
 
 from marshy import ExternalType
 from marshy.marshaller.marshaller_abc import MarshallerABC
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class OptionalMarshaller(MarshallerABC[Optional[T]]):
     """
     Marshaller for optional types
     """
```

### Comparing `marshy-4.0.0/marshy/marshaller/property_marshaller.py` & `marshy-4.0.2/marshy/marshaller/property_marshaller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from typing import TypeVar, Tuple
 
 from marshy import ExternalType
 from marshy.marshaller.marshaller_abc import MarshallerABC
 from marshy.types import ExternalItemType
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 @dataclass(frozen=True)
 class PropertyConfig:
     external_name: str
     marshaller: MarshallerABC
     prop: property
@@ -18,16 +18,19 @@
     exclude_dumped_values: Tuple = ()
 
 
 class PropertyMarshaller(MarshallerABC[T]):
     """
     Marshaller which wraps another and uses property setters / getters.
     """
+
     # noinspection PyDataclass
-    def __init__(self, marshaller: MarshallerABC[T], property_configs: Tuple[PropertyConfig]):
+    def __init__(
+        self, marshaller: MarshallerABC[T], property_configs: Tuple[PropertyConfig]
+    ):
         super().__init__(marshaller.marshalled_type)
         self.marshaller = marshaller
         self.property_configs = property_configs
 
     def load(self, item: ExternalItemType) -> T:
         loaded = self.marshaller.load(item)
         for property_config in self.property_configs:
```

### Comparing `marshy-4.0.0/marshy/marshaller/tuple_marshaller.py` & `marshy-4.0.2/marshy/marshaller/tuple_marshaller.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from dataclasses import dataclass
 from typing import TypeVar, Iterable, List, Tuple, Union
 
 from marshy.types import ExternalItemType, ExternalType
 from marshy.marshaller.marshaller_abc import MarshallerABC
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 @dataclass(frozen=True)
 class TupleMarshaller(MarshallerABC[Iterable[T]]):
     """
     Marshaller for iterable types (lists)
     """
+
     item_marshallers: Tuple[MarshallerABC[T], ...]
 
     def load(self, item: Union[List[ExternalType], ExternalItemType]) -> Iterable[T]:
         if isinstance(item, dict):
-            loaded = tuple(m.load(item[f"t{i}"]) for i, m in enumerate(self.item_marshallers))
+            loaded = tuple(
+                m.load(item[f"t{i}"]) for i, m in enumerate(self.item_marshallers)
+            )
             return loaded
         loaded = tuple(m.load(i) for m, i in zip(self.item_marshallers, item))
         return loaded
 
     def dump(self, item: Iterable[T]) -> List[ExternalType]:
         dumped = [m.dump(i) for m, i in zip(self.item_marshallers, item)]
         return dumped
```

### Comparing `marshy-4.0.0/marshy/marshaller/type_marshaller.py` & `marshy-4.0.2/marshy/marshaller/type_marshaller.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,42 +7,43 @@
 
 
 @dataclass(frozen=True)
 class TypeMarshaller(MarshallerABC[Type]):
     """
     Marshaller for object types - allows setting up a preset 'safe' module list
     """
+
     marshalled_type: Type = Type
     permitted_prefixes: Iterable[str] = field(default_factory=tuple)
     _names_to_types: Dict[str, Type] = field(default_factory=dict)
     _types_to_names: Dict[Type, str] = None
 
     def __post_init__(self):
         types_to_names = {t: n for n, t in self._names_to_types.items()}
-        object.__setattr__(self, '_types_to_names', types_to_names)
+        object.__setattr__(self, "_types_to_names", types_to_names)
 
     def load(self, item: str) -> Type:
         type_ = self._names_to_types.get(item)
         if type_ is not None:
             return type_
         for permitted_prefix in self.permitted_prefixes:
             if item.startswith(permitted_prefix):
-                path = item.split('.')
-                module = '.'.join(path[:-1])
+                path = item.split(".")
+                module = ".".join(path[:-1])
                 module = importlib.import_module(module)
                 type_ = getattr(module, path[-1])
                 self._names_to_types[item] = type_
                 self._types_to_names[type_] = item
                 return type_
-        raise MarshallError(f'type_not_permitted:{item}')
+        raise MarshallError(f"type_not_permitted:{item}")
 
     def dump(self, item: Type) -> str:
         name = self._types_to_names.get(item)
         if name is not None:
             return name
-        path = item.__module__ + '.' + item.__name__
+        path = item.__module__ + "." + item.__name__
         for permitted_prefix in self.permitted_prefixes:
             if path.startswith(permitted_prefix):
                 self._names_to_types[path] = item
                 self._types_to_names[item] = path
                 return path
-        raise MarshallError(f'type_not_permitted:{item}')
+        raise MarshallError(f"type_not_permitted:{item}")
```

### Comparing `marshy-4.0.0/marshy/marshaller/union_marshaller.py` & `marshy-4.0.2/marshy/marshaller/union_marshaller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from typing import TypeVar, Optional, Dict, Type, List, Iterable
 
 from marshy import ExternalType
 from marshy.marshaller.deferred_marshaller import DeferredMarshaller
 from marshy.marshaller.marshaller_abc import MarshallerABC
 from marshy.marshaller_context import MarshallerContext
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class UnionMarshaller(MarshallerABC[T]):
     """
     Marshaller for polymorphic types
     """
 
     # noinspection PyDataclass
-    def __init__(self, marshalled_type: T, marshallers_by_name: Dict[str, MarshallerABC[T]]):
+    def __init__(
+        self, marshalled_type: T, marshallers_by_name: Dict[str, MarshallerABC[T]]
+    ):
         super().__init__(marshalled_type)
         self.marshallers_by_name = marshallers_by_name
-        self.names_by_type = {resolve_type(m.marshalled_type): n for n, m in marshallers_by_name.items()}
+        self.names_by_type = {
+            resolve_type(m.marshalled_type): n for n, m in marshallers_by_name.items()
+        }
 
     def load(self, item: List[ExternalType]) -> T:
         type_name = item[0]
         marshaller = self.marshallers_by_name[type_name]
         loaded = marshaller.load(item[1])
         return loaded
 
@@ -29,14 +33,17 @@
         type_name = self.names_by_type[item.__class__]
         marshaller = self.marshallers_by_name[type_name]
         dumped = marshaller.dump(item)
         return [type_name, dumped]
 
 
 def resolve_type(type_: Type) -> Type:
-    return resolve_type(type_.__origin__) if hasattr(type_, '__origin__') else type_
+    return resolve_type(type_.__origin__) if hasattr(type_, "__origin__") else type_
 
 
-def implementation_marshaller(base_type: Type, impls: Iterable[Type], marshaller_context: MarshallerContext):
-    return UnionMarshaller(base_type, {
-        i.__name__: DeferredMarshaller[i](i, marshaller_context) for i in impls
-    })
+def implementation_marshaller(
+    base_type: Type, impls: Iterable[Type], marshaller_context: MarshallerContext
+):
+    return UnionMarshaller(
+        base_type,
+        {i.__name__: DeferredMarshaller[i](i, marshaller_context) for i in impls},
+    )
```

### Comparing `marshy-4.0.0/marshy/marshaller_context.py` & `marshy-4.0.2/marshy/marshaller_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,39 +5,44 @@
 from marshy.factory.marshaller_factory_abc import MarshallerFactoryABC
 from marshy.marshaller import marshaller_abc
 from marshy.types import ExternalType
 from marshy.utils import resolve_forward_refs
 
 
 class MarshallerContext:
-
-    def __init__(self,
-                 factories: Optional[marshaller_factory_abc.MarshallerFactoryABC] = None,
-                 by_type: Optional[Dict[Type, marshaller_abc.MarshallerABC]] = None):
+    def __init__(
+        self,
+        factories: Optional[marshaller_factory_abc.MarshallerFactoryABC] = None,
+        by_type: Optional[Dict[Type, marshaller_abc.MarshallerABC]] = None,
+    ):
         self._factories = sorted(factories or [], reverse=True)
         self._by_type = dict(by_type or {})
 
-    def register_factory(self, marshaller_factory: marshaller_factory_abc.MarshallerFactoryABC):
+    def register_factory(
+        self, marshaller_factory: marshaller_factory_abc.MarshallerFactoryABC
+    ):
         self._factories.append(marshaller_factory)
         self._factories = sorted(self._factories or [], reverse=True)
 
-    def register_marshaller(self, marshaller: marshaller_abc.MarshallerABC, type_: Type = None):
+    def register_marshaller(
+        self, marshaller: marshaller_abc.MarshallerABC, type_: Type = None
+    ):
         type_ = type_ or marshaller.marshalled_type
         self._by_type[type_] = marshaller
 
     def get_marshaller(self, type_: Type) -> marshaller_abc.MarshallerABC:
         marshaller = self._by_type.get(type_)
         if not marshaller:
             resolved_type = resolve_forward_refs(type_)
             for factory in self._factories:
                 marshaller = factory.create(self, resolved_type)
                 if marshaller:
                     break
             if not marshaller:
-                raise MarshallError(f'NoMarshallerForType:{type_}')
+                raise MarshallError(f"NoMarshallerForType:{type_}")
             self._by_type[type_] = marshaller
         return marshaller
 
     def load(self, type_: Type, to_load: ExternalType):
         marshaller = self.get_marshaller(type_)
         loaded = marshaller.load(to_load)
         return loaded
```

### Comparing `marshy-4.0.0/marshy/utils.py` & `marshy-4.0.2/marshy/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import importlib
 import typing
 
 import typing_inspect
 
 from marshy.errors import MarshallError
 
-_TYPES_BY_ORIGIN = {t.__origin__: t for t in typing.__dict__.values() if hasattr(t, '__origin__')}
+_TYPES_BY_ORIGIN = {
+    t.__origin__: t for t in typing.__dict__.values() if hasattr(t, "__origin__")
+}
 
 
 def resolve_forward_refs(type_: typing.Type) -> typing.Type:
     origin = typing_inspect.get_origin(type_)
     if origin is not None:
         args = list(resolve_forward_refs(a) for a in typing_inspect.get_args(type_))
         typing_origin = _TYPES_BY_ORIGIN.get(origin)
         origin = typing_origin or origin
         return origin[tuple(args)]
     if not typing_inspect.is_forward_ref(type_):
         return type_
     import_name = typing_inspect.get_forward_arg(type_)
-    import_path = import_name.split('.')
-    import_module = '.'.join(import_path[:-1])
+    import_path = import_name.split(".")
+    import_module = ".".join(import_path[:-1])
     if not import_module:
-        raise MarshallError(f'InvalidForwardRef:{type_}:Use full module name!')
+        raise MarshallError(f"InvalidForwardRef:{type_}:Use full module name!")
     imported_module = importlib.import_module(import_module)
     return_type = getattr(imported_module, import_path[-1])
     return return_type
```

### Comparing `marshy-4.0.0/marshy_config_default/__init__.py` & `marshy-4.0.2/marshy_config_default/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 from marshy.factory.dataclass_marshaller_factory import DataclassMarshallerFactory
 from marshy.factory.enum_marshaller_factory import EnumMarshallerFactory
 from marshy.factory.factory_marshaller_factory import FactoryMarshallerFactory
 from marshy.factory.list_marshaller_factory import ListMarshallerFactory
 from marshy.factory.optional_marshaller_factory import OptionalMarshallerFactory
 from marshy.factory.tuple_marshaller_factory import TupleMarshallerFactory
 from marshy.factory.union_marshaller_factory import UnionMarshallerFactory
-from marshy.marshaller import PrimitiveMarshaller, none_marshaller, bool_marshaller, datetime_marshaller
+from marshy.marshaller import (
+    PrimitiveMarshaller,
+    none_marshaller,
+    bool_marshaller,
+    datetime_marshaller,
+)
 from marshy.marshaller.as_str_marshaller import AsStrMarshaller
 from marshy.marshaller.json_str_marshaller import JsonStrMarshaller
 from marshy.marshaller_context import MarshallerContext
 from marshy.types import ExternalItemType, ExternalType
 
 priority = 100
 
@@ -29,8 +34,7 @@
     context.register_factory(OptionalMarshallerFactory())
     context.register_factory(ListMarshallerFactory())
     context.register_factory(FactoryMarshallerFactory())
     context.register_factory(DataclassMarshallerFactory())
     context.register_factory(TupleMarshallerFactory())
     context.register_marshaller(JsonStrMarshaller(ExternalType))
     context.register_marshaller(JsonStrMarshaller(ExternalItemType))
-
```

