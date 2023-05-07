# Comparing `tmp/v8unpack-0.9.2.tar.gz` & `tmp/v8unpack-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\project\python\v8unpack\dist\tmpxwqxzdco\v8unpack-0.9.2.tar", last modified: Mon Sep 19 16:38:13 2022, max compression
+gzip compressed data, was "C:\project\python\v8unpack\dist\tmp9d5lo7q2\v8unpack-0.9.3.tar", last modified: Wed Sep 28 05:01:13 2022, max compression
```

## Comparing `v8unpack-0.9.2.tar` & `v8unpack-0.9.3.tar`

### file list

```diff
@@ -1,105 +1,107 @@
-drwxrwxrwx   0        0        0        0 2022-09-19 16:38:13.000000 v8unpack-0.9.2/
--rw-rw-rw-   0        0        0     1074 2021-09-06 05:35:57.000000 v8unpack-0.9.2/LICENSE
--rw-rw-rw-   0        0        0     6380 2022-09-19 16:38:13.000000 v8unpack-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     5708 2022-09-19 16:28:27.000000 v8unpack-0.9.2/README.md
--rw-rw-rw-   0        0        0       42 2022-09-19 16:38:13.000000 v8unpack-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1172 2022-03-23 05:29:27.000000 v8unpack-0.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-19 16:38:13.000000 v8unpack-0.9.2/src/
-drwxrwxrwx   0        0        0        0 2022-09-19 16:38:13.000000 v8unpack-0.9.2/src/v8unpack/
-drwxrwxrwx   0        0        0        0 2022-09-19 16:38:13.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/
--rw-rw-rw-   0        0        0      352 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/AccumulationRegister.py
--rw-rw-rw-   0        0        0      242 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/AccumulationRegisterForm.py
--rw-rw-rw-   0        0        0      446 2021-10-29 09:53:36.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Catalog.py
--rw-rw-rw-   0        0        0      115 2021-10-06 16:37:45.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/CatalogCommand.py
--rw-rw-rw-   0        0        0      221 2022-02-10 13:35:21.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/CatalogForm.py
--rw-rw-rw-   0        0        0      532 2022-03-04 09:24:02.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/ChartOfCharacteristicType.py
--rw-rw-rw-   0        0        0      186 2021-10-29 09:53:36.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/CommandGroup.py
--rw-rw-rw-   0        0        0      219 2021-10-06 07:10:46.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/CommonCommand.py
--rw-rw-rw-   0        0        0      214 2022-03-04 09:24:02.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/CommonForm.py
--rw-rw-rw-   0        0        0      107 2022-03-04 09:24:02.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/CommonModule.py
--rw-rw-rw-   0        0        0     2109 2021-10-29 09:53:36.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/CommonPicture.py
--rw-rw-rw-   0        0        0      222 2022-09-19 16:20:29.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/CommonTemplate.py
--rw-rw-rw-   0        0        0      367 2022-03-04 09:24:02.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Constant.py
--rw-rw-rw-   0        0        0      410 2022-03-04 09:24:02.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/DataProcessor.py
--rw-rw-rw-   0        0        0      175 2021-11-03 05:42:16.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/DefinedType.py
--rw-rw-rw-   0        0        0      184 2022-03-04 09:24:02.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Document.py
--rw-rw-rw-   0        0        0      116 2021-10-06 16:37:45.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/DocumentCommand.py
--rw-rw-rw-   0        0        0      222 2022-02-10 13:35:21.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/DocumentForm.py
--rw-rw-rw-   0        0        0      200 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/DocumentJournal.py
--rw-rw-rw-   0        0        0      237 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/DocumentJournalForm.py
--rw-rw-rw-   0        0        0      171 2022-03-04 09:24:02.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Enum.py
--rw-rw-rw-   0        0        0      121 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/EventSubscription.py
--rw-rw-rw-   0        0        0      195 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/ExchangePlan.py
--rw-rw-rw-   0        0        0      234 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/ExchangePlanForm.py
--rw-rw-rw-   0        0        0      196 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/FilterCriterion.py
--rw-rw-rw-   0        0        0      237 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/FilterCriterionForm.py
--rw-rw-rw-   0        0        0      346 2022-02-10 13:35:21.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Form.py
--rw-rw-rw-   0        0        0      180 2021-11-03 05:42:16.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/FunctionalOption.py
--rw-rw-rw-   0        0        0      339 2022-03-04 09:24:02.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/InformationRegister.py
--rw-rw-rw-   0        0        0      214 2022-03-04 09:24:02.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/InformationRegisterCommand.py
--rw-rw-rw-   0        0        0      233 2022-03-04 09:24:02.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/InformationRegisterForm.py
--rw-rw-rw-   0        0        0      204 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Interface.py
--rw-rw-rw-   0        0        0       88 2021-10-06 16:43:41.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Language.py
--rw-rw-rw-   0        0        0      323 2021-10-19 11:29:01.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Report.py
--rw-rw-rw-   0        0        0      228 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/ReportForm.py
--rw-rw-rw-   0        0        0      108 2021-10-06 10:56:56.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Role.py
--rw-rw-rw-   0        0        0      116 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/ScheduledJob.py
--rw-rw-rw-   0        0        0      111 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Sequences.py
--rw-rw-rw-   0        0        0      183 2022-03-04 09:24:02.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/SessionParameter.py
--rw-rw-rw-   0        0        0      109 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Style.py
--rw-rw-rw-   0        0        0      183 2022-03-04 09:24:02.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/StyleItem.py
--rw-rw-rw-   0        0        0      728 2021-10-29 09:53:36.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Subsystem.py
--rw-rw-rw-   0        0        0      370 2021-10-29 09:53:36.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/Template.py
--rw-rw-rw-   0        0        0       91 2022-09-19 16:25:55.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/XDTOPackage.py
--rw-rw-rw-   0        0        0     4635 2022-09-19 16:28:27.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-19 16:38:13.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/core/
--rw-rw-rw-   0        0        0     1219 2022-02-09 16:20:35.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/core/Container.py
--rw-rw-rw-   0        0        0      716 2021-10-19 11:29:01.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/core/IncludeEmpty.py
--rw-rw-rw-   0        0        0     1461 2022-02-09 16:20:35.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/core/IncludeSimple.py
--rw-rw-rw-   0        0        0     1037 2022-02-09 16:20:35.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/core/Simple.py
--rw-rw-rw-   0        0        0      693 2021-10-06 10:56:09.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/core/SimpleWithInfo.py
--rw-rw-rw-   0        0        0        0 2021-10-07 14:10:16.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/core/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-19 16:38:13.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/
--rw-rw-rw-   0        0        0      900 2022-02-10 13:35:21.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/CommonForm803.py
--rw-rw-rw-   0        0        0      274 2022-09-19 16:00:34.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/CommonTemplate803.py
--rw-rw-rw-   0        0        0      338 2021-10-19 11:29:01.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/DocumentForm803.py
--rw-rw-rw-   0        0        0    36190 2022-01-15 10:59:03.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Form801.py
--rw-rw-rw-   0        0        0    36689 2022-02-09 17:08:32.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Form802.py
--rw-rw-rw-   0        0        0    17246 2022-09-19 15:45:16.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Form803.py
--rw-rw-rw-   0        0        0     3144 2022-09-19 15:45:16.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Form8x.py
--rw-rw-rw-   0        0        0       80 2021-10-19 11:29:01.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Template801.py
--rw-rw-rw-   0        0        0      684 2021-10-19 11:29:01.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Template802.py
--rw-rw-rw-   0        0        0      724 2021-10-19 11:29:01.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Template803.py
--rw-rw-rw-   0        0        0     6356 2022-09-19 16:14:09.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Template8x.py
--rw-rw-rw-   0        0        0        0 2021-10-07 14:10:26.000000 v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-19 16:38:13.000000 v8unpack-0.9.2/src/v8unpack/MetaObject/
--rw-rw-rw-   0        0        0      199 2022-09-19 16:22:26.000000 v8unpack-0.9.2/src/v8unpack/MetaObject/Configuration802.py
--rw-rw-rw-   0        0        0     2284 2022-09-13 07:22:19.000000 v8unpack-0.9.2/src/v8unpack/MetaObject/Configuration803.py
--rw-rw-rw-   0        0        0     3615 2022-09-19 15:45:16.000000 v8unpack-0.9.2/src/v8unpack/MetaObject/ConfigurationExtension803.py
--rw-rw-rw-   0        0        0     3976 2022-09-13 07:22:19.000000 v8unpack-0.9.2/src/v8unpack/MetaObject/ExternalDataProcessor.py
--rw-rw-rw-   0        0        0      385 2021-10-19 11:29:01.000000 v8unpack-0.9.2/src/v8unpack/MetaObject/ExternalDataProcessor801.py
--rw-rw-rw-   0        0        0      274 2021-10-19 11:29:01.000000 v8unpack-0.9.2/src/v8unpack/MetaObject/ExternalDataProcessor802.py
--rw-rw-rw-   0        0        0      180 2021-10-19 11:29:01.000000 v8unpack-0.9.2/src/v8unpack/MetaObject/ExternalDataProcessor803.py
--rw-rw-rw-   0        0        0     8728 2022-09-19 15:45:16.000000 v8unpack-0.9.2/src/v8unpack/MetaObject/__init__.py
--rw-rw-rw-   0        0        0      168 2022-09-19 16:38:03.000000 v8unpack-0.9.2/src/v8unpack/__init__.py
--rw-rw-rw-   0        0        0       80 2021-10-29 09:53:36.000000 v8unpack-0.9.2/src/v8unpack/__main__.py
--rw-rw-rw-   0        0        0     6124 2022-09-13 07:22:19.000000 v8unpack-0.9.2/src/v8unpack/code_organizer.py
--rw-rw-rw-   0        0        0    11532 2022-01-15 13:20:28.000000 v8unpack-0.9.2/src/v8unpack/container_reader.py
--rw-rw-rw-   0        0        0    11108 2022-03-23 07:09:38.000000 v8unpack-0.9.2/src/v8unpack/container_writer.py
--rw-rw-rw-   0        0        0     6477 2022-09-19 16:06:14.000000 v8unpack-0.9.2/src/v8unpack/decoder.py
--rw-rw-rw-   0        0        0     6912 2022-09-19 16:28:27.000000 v8unpack-0.9.2/src/v8unpack/ext_exception.py
--rw-rw-rw-   0        0        0    10584 2022-09-13 07:22:19.000000 v8unpack-0.9.2/src/v8unpack/file_organizer.py
--rw-rw-rw-   0        0        0     2681 2022-03-02 16:00:37.000000 v8unpack-0.9.2/src/v8unpack/file_organizer_ce.py
--rw-rw-rw-   0        0        0     7844 2022-09-19 16:28:27.000000 v8unpack-0.9.2/src/v8unpack/helper.py
--rw-rw-rw-   0        0        0     1313 2022-04-21 08:04:42.000000 v8unpack-0.9.2/src/v8unpack/index.py
--rw-rw-rw-   0        0        0    16024 2022-09-19 16:28:27.000000 v8unpack-0.9.2/src/v8unpack/json_container_decoder.py
--rw-rw-rw-   0        0        0     6882 2022-09-19 16:33:31.000000 v8unpack-0.9.2/src/v8unpack/metadata_types.py
--rw-rw-rw-   0        0        0    11430 2022-09-13 07:22:19.000000 v8unpack-0.9.2/src/v8unpack/unittest_helper.py
--rw-rw-rw-   0        0        0     9829 2022-09-13 07:22:19.000000 v8unpack-0.9.2/src/v8unpack/v8unpack.py
-drwxrwxrwx   0        0        0        0 2022-09-19 16:38:13.000000 v8unpack-0.9.2/src/v8unpack.egg-info/
--rw-rw-rw-   0        0        0     6380 2022-09-19 16:38:13.000000 v8unpack-0.9.2/src/v8unpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3974 2022-09-19 16:38:13.000000 v8unpack-0.9.2/src/v8unpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-19 16:38:13.000000 v8unpack-0.9.2/src/v8unpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2022-09-19 16:38:13.000000 v8unpack-0.9.2/src/v8unpack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-09-24 08:08:08.000000 v8unpack-0.9.2/src/v8unpack.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2022-09-19 16:38:13.000000 v8unpack-0.9.2/src/v8unpack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-09-28 05:01:13.000000 v8unpack-0.9.3/
+-rw-rw-rw-   0        0        0     1074 2021-09-06 05:35:57.000000 v8unpack-0.9.3/LICENSE
+-rw-rw-rw-   0        0        0     6380 2022-09-28 05:01:13.000000 v8unpack-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5708 2022-09-21 16:02:56.000000 v8unpack-0.9.3/README.md
+-rw-rw-rw-   0        0        0       42 2022-09-28 05:01:13.000000 v8unpack-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1172 2022-03-23 05:29:27.000000 v8unpack-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-28 05:01:13.000000 v8unpack-0.9.3/src/
+drwxrwxrwx   0        0        0        0 2022-09-28 05:01:13.000000 v8unpack-0.9.3/src/v8unpack/
+drwxrwxrwx   0        0        0        0 2022-09-28 05:01:13.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/
+-rw-rw-rw-   0        0        0      352 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/AccumulationRegister.py
+-rw-rw-rw-   0        0        0      242 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/AccumulationRegisterForm.py
+-rw-rw-rw-   0        0        0      446 2021-10-29 09:53:36.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Catalog.py
+-rw-rw-rw-   0        0        0      115 2021-10-06 16:37:45.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/CatalogCommand.py
+-rw-rw-rw-   0        0        0      221 2022-02-10 13:35:21.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/CatalogForm.py
+-rw-rw-rw-   0        0        0      532 2022-03-04 09:24:02.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/ChartOfCharacteristicType.py
+-rw-rw-rw-   0        0        0      186 2021-10-29 09:53:36.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/CommandGroup.py
+-rw-rw-rw-   0        0        0      219 2021-10-06 07:10:46.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/CommonCommand.py
+-rw-rw-rw-   0        0        0      214 2022-03-04 09:24:02.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/CommonForm.py
+-rw-rw-rw-   0        0        0      112 2022-09-21 17:31:15.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/CommonModule.py
+-rw-rw-rw-   0        0        0     2109 2021-10-29 09:53:36.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/CommonPicture.py
+-rw-rw-rw-   0        0        0      222 2022-09-19 16:20:29.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/CommonTemplate.py
+-rw-rw-rw-   0        0        0      367 2022-03-04 09:24:02.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Constant.py
+-rw-rw-rw-   0        0        0      410 2022-03-04 09:24:02.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/DataProcessor.py
+-rw-rw-rw-   0        0        0      175 2021-11-03 05:42:16.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/DefinedType.py
+-rw-rw-rw-   0        0        0      184 2022-03-04 09:24:02.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Document.py
+-rw-rw-rw-   0        0        0      116 2021-10-06 16:37:45.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/DocumentCommand.py
+-rw-rw-rw-   0        0        0      222 2022-02-10 13:35:21.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/DocumentForm.py
+-rw-rw-rw-   0        0        0      200 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/DocumentJournal.py
+-rw-rw-rw-   0        0        0      237 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/DocumentJournalForm.py
+-rw-rw-rw-   0        0        0      171 2022-03-04 09:24:02.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Enum.py
+-rw-rw-rw-   0        0        0      121 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/EventSubscription.py
+-rw-rw-rw-   0        0        0      195 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/ExchangePlan.py
+-rw-rw-rw-   0        0        0      234 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/ExchangePlanForm.py
+-rw-rw-rw-   0        0        0      196 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/FilterCriterion.py
+-rw-rw-rw-   0        0        0      237 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/FilterCriterionForm.py
+-rw-rw-rw-   0        0        0      346 2022-02-10 13:35:21.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Form.py
+-rw-rw-rw-   0        0        0      180 2021-11-03 05:42:16.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/FunctionalOption.py
+-rw-rw-rw-   0        0        0      184 2022-09-21 16:18:40.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/HTTPService.py
+-rw-rw-rw-   0        0        0      339 2022-03-04 09:24:02.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/InformationRegister.py
+-rw-rw-rw-   0        0        0      214 2022-03-04 09:24:02.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/InformationRegisterCommand.py
+-rw-rw-rw-   0        0        0      233 2022-03-04 09:24:02.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/InformationRegisterForm.py
+-rw-rw-rw-   0        0        0      204 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Interface.py
+-rw-rw-rw-   0        0        0       88 2021-10-06 16:43:41.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Language.py
+-rw-rw-rw-   0        0        0      323 2021-10-19 11:29:01.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Report.py
+-rw-rw-rw-   0        0        0      222 2022-09-21 16:40:22.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/ReportForm.py
+-rw-rw-rw-   0        0        0      108 2021-10-06 10:56:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Role.py
+-rw-rw-rw-   0        0        0      116 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/ScheduledJob.py
+-rw-rw-rw-   0        0        0      111 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Sequences.py
+-rw-rw-rw-   0        0        0      183 2022-03-04 09:24:02.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/SessionParameter.py
+-rw-rw-rw-   0        0        0      109 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Style.py
+-rw-rw-rw-   0        0        0      183 2022-03-04 09:24:02.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/StyleItem.py
+-rw-rw-rw-   0        0        0      728 2021-10-29 09:53:36.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Subsystem.py
+-rw-rw-rw-   0        0        0      370 2021-10-29 09:53:36.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/Template.py
+-rw-rw-rw-   0        0        0       91 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/XDTOPackage.py
+-rw-rw-rw-   0        0        0     4635 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-28 05:01:13.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/core/
+-rw-rw-rw-   0        0        0     1219 2022-02-09 16:20:35.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/core/Container.py
+-rw-rw-rw-   0        0        0      716 2021-10-19 11:29:01.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/core/IncludeEmpty.py
+-rw-rw-rw-   0        0        0     1461 2022-02-09 16:20:35.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/core/IncludeSimple.py
+-rw-rw-rw-   0        0        0     1037 2022-02-09 16:20:35.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/core/Simple.py
+-rw-rw-rw-   0        0        0      693 2021-10-06 10:56:09.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/core/SimpleWithInfo.py
+-rw-rw-rw-   0        0        0        0 2021-10-07 14:10:16.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/core/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-28 05:01:13.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/
+-rw-rw-rw-   0        0        0      900 2022-02-10 13:35:21.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/CommonForm803.py
+-rw-rw-rw-   0        0        0      285 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/CommonTemplate803.py
+-rw-rw-rw-   0        0        0      338 2021-10-19 11:29:01.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/DocumentForm803.py
+-rw-rw-rw-   0        0        0    36190 2022-01-15 10:59:03.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Form801.py
+-rw-rw-rw-   0        0        0    36689 2022-02-09 17:08:32.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Form802.py
+-rw-rw-rw-   0        0        0    17246 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Form803.py
+-rw-rw-rw-   0        0        0     3144 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Form8x.py
+-rw-rw-rw-   0        0        0      504 2022-09-21 17:22:04.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/ReportForm803.py
+-rw-rw-rw-   0        0        0       80 2021-10-19 11:29:01.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Template801.py
+-rw-rw-rw-   0        0        0      684 2021-10-19 11:29:01.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Template802.py
+-rw-rw-rw-   0        0        0      724 2021-10-19 11:29:01.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Template803.py
+-rw-rw-rw-   0        0        0     6514 2022-09-21 17:30:38.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Template8x.py
+-rw-rw-rw-   0        0        0        0 2021-10-07 14:10:26.000000 v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-28 05:01:13.000000 v8unpack-0.9.3/src/v8unpack/MetaObject/
+-rw-rw-rw-   0        0        0      199 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaObject/Configuration802.py
+-rw-rw-rw-   0        0        0     2284 2022-09-13 07:22:19.000000 v8unpack-0.9.3/src/v8unpack/MetaObject/Configuration803.py
+-rw-rw-rw-   0        0        0     3615 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/MetaObject/ConfigurationExtension803.py
+-rw-rw-rw-   0        0        0     3976 2022-09-13 07:22:19.000000 v8unpack-0.9.3/src/v8unpack/MetaObject/ExternalDataProcessor.py
+-rw-rw-rw-   0        0        0      385 2021-10-19 11:29:01.000000 v8unpack-0.9.3/src/v8unpack/MetaObject/ExternalDataProcessor801.py
+-rw-rw-rw-   0        0        0      274 2021-10-19 11:29:01.000000 v8unpack-0.9.3/src/v8unpack/MetaObject/ExternalDataProcessor802.py
+-rw-rw-rw-   0        0        0      180 2021-10-19 11:29:01.000000 v8unpack-0.9.3/src/v8unpack/MetaObject/ExternalDataProcessor803.py
+-rw-rw-rw-   0        0        0     9329 2022-09-21 17:39:52.000000 v8unpack-0.9.3/src/v8unpack/MetaObject/__init__.py
+-rw-rw-rw-   0        0        0      168 2022-09-28 05:00:59.000000 v8unpack-0.9.3/src/v8unpack/__init__.py
+-rw-rw-rw-   0        0        0       80 2021-10-29 09:53:36.000000 v8unpack-0.9.3/src/v8unpack/__main__.py
+-rw-rw-rw-   0        0        0     6124 2022-09-13 07:22:19.000000 v8unpack-0.9.3/src/v8unpack/code_organizer.py
+-rw-rw-rw-   0        0        0    11532 2022-01-15 13:20:28.000000 v8unpack-0.9.3/src/v8unpack/container_reader.py
+-rw-rw-rw-   0        0        0    11108 2022-03-23 07:09:38.000000 v8unpack-0.9.3/src/v8unpack/container_writer.py
+-rw-rw-rw-   0        0        0     6477 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/decoder.py
+-rw-rw-rw-   0        0        0     6912 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/ext_exception.py
+-rw-rw-rw-   0        0        0    10584 2022-09-13 07:22:19.000000 v8unpack-0.9.3/src/v8unpack/file_organizer.py
+-rw-rw-rw-   0        0        0     2681 2022-03-02 16:00:37.000000 v8unpack-0.9.3/src/v8unpack/file_organizer_ce.py
+-rw-rw-rw-   0        0        0     7844 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/helper.py
+-rw-rw-rw-   0        0        0     1313 2022-04-21 08:04:42.000000 v8unpack-0.9.3/src/v8unpack/index.py
+-rw-rw-rw-   0        0        0    16024 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/json_container_decoder.py
+-rw-rw-rw-   0        0        0     6882 2022-09-21 16:02:56.000000 v8unpack-0.9.3/src/v8unpack/metadata_types.py
+-rw-rw-rw-   0        0        0    11430 2022-09-13 07:22:19.000000 v8unpack-0.9.3/src/v8unpack/unittest_helper.py
+-rw-rw-rw-   0        0        0     9829 2022-09-13 07:22:19.000000 v8unpack-0.9.3/src/v8unpack/v8unpack.py
+drwxrwxrwx   0        0        0        0 2022-09-28 05:01:13.000000 v8unpack-0.9.3/src/v8unpack.egg-info/
+-rw-rw-rw-   0        0        0     6380 2022-09-28 05:01:13.000000 v8unpack-0.9.3/src/v8unpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4071 2022-09-28 05:01:13.000000 v8unpack-0.9.3/src/v8unpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-28 05:01:13.000000 v8unpack-0.9.3/src/v8unpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2022-09-28 05:01:13.000000 v8unpack-0.9.3/src/v8unpack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2021-09-24 08:08:08.000000 v8unpack-0.9.3/src/v8unpack.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2022-09-28 05:01:13.000000 v8unpack-0.9.3/src/v8unpack.egg-info/top_level.txt
```

### Comparing `v8unpack-0.9.2/LICENSE` & `v8unpack-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/PKG-INFO` & `v8unpack-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v8unpack
-Version: 0.9.2
+Version: 0.9.3
 Summary: Unpacking binaries 1C to JSON for GIT
 Home-page: https://github.com/saby-integration/v8unpack
 Author: Razgovorov Mikhail
 Author-email: 1338833@gmail.com
 License: MIT
 Keywords: 1C CF CFE EPF V8UNPACK SABY SBIS СБИС 1С
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `v8unpack-0.9.2/README.md` & `v8unpack-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/setup.py` & `v8unpack-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/ChartOfCharacteristicType.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/ChartOfCharacteristicType.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/CommonPicture.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/CommonPicture.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/Subsystem.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/Subsystem.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/__init__.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/__init__.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/core/Container.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/core/Container.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/core/IncludeEmpty.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/core/IncludeEmpty.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/core/IncludeSimple.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/core/IncludeSimple.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/core/Simple.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/core/Simple.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/core/SimpleWithInfo.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/core/SimpleWithInfo.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/CommonForm803.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/CommonForm803.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Form801.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Form801.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Form802.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Form802.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Form803.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Form803.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Form8x.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Form8x.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Template802.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Template802.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Template803.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Template803.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaDataObject/versions/Template8x.py` & `v8unpack-0.9.3/src/v8unpack/MetaDataObject/versions/Template8x.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,27 +76,27 @@
             helper.txt_write(self.data, dest_dir, f'{self.header["name"]}.bin', encoding=encoding)
 
     def decode_extension_data(self, src_dir, dest_dir, write):
         self.decode_base64_data(src_dir, dest_dir, write)
 
     def decode_base64_data(self, src_dir, dest_dir, write):
         try:
-            data = helper.json_read(src_dir, f'{self.header["uuid"]}.0.bin')
+            data = helper.json_read(src_dir, f'{self.header["uuid"]}.0.json')
         except FileNotFoundError:
             return
         if data[0][1] and data[0][1][0]:
             self.data = b64decode(data[0][1][0][8:])
             data[0][1][0] = '"данные в отдельном файле"'
             extension = helper.get_extension_from_comment(self.header['comment'])
             if write:
                 helper.bin_write(self.data, dest_dir, f'{self.header["name"]}.{extension}')
 
     def decode_html_data(self, src_dir, dest_dir, write):
         try:
-            data = helper.json_read(src_dir, f'{self.header["uuid"]}.0.bin')
+            data = helper.json_read(src_dir, f'{self.header["uuid"]}.0.json')
         except FileNotFoundError:
             return
         if data[0][3] and data[0][3][0]:
             self.data = b64decode(data[0][3][0][8:])
             data[0][3][0] = '"данные в отдельном файле"'
             if write:
                 helper.bin_write(self.data, dest_dir, f'{self.header["name"]}.html')
@@ -148,21 +148,28 @@
 
     def encode_html_data(self, src_dir, dest_dir):
         bin_data = helper.bin_read(src_dir, f'{self.header["name"]}.html')
         self.raw_data = [[
             "5",
             "1",
             "\"ru\"",
-            ["#base64:" + b64encode(bin_data).decode(encoding='utf-8')],
+            [self._get_b64_string(bin_data)],
             "0"
         ]]
-        helper.json_write(self.raw_data, dest_dir, f'{self.header["uuid"]}.0.bin')
+        helper.json_write(self.raw_data, dest_dir, f'{self.header["uuid"]}.0.json')
+
+    @staticmethod
+    def _get_b64_string(bin_data):
+        if not bin_data:
+            return "##base64:"
+        else:
+            return "#base64:" + b64encode(bin_data).decode(encoding='utf-8')
 
     def _encode_bin_data(self, bin_data, dest_dir):
         self.raw_data = [[
             "1",
-            ["#base64:" + b64encode(bin_data).decode(encoding='utf-8')]
+            [self._get_b64_string(bin_data)]
         ]]
-        helper.json_write(self.raw_data, dest_dir, f'{self.header["uuid"]}.0.bin')
+        helper.json_write(self.raw_data, dest_dir, f'{self.header["uuid"]}.0.json')
 
     def encode_header(self):
         raise NotImplemented()
```

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaObject/Configuration803.py` & `v8unpack-0.9.3/src/v8unpack/MetaObject/Configuration803.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaObject/ConfigurationExtension803.py` & `v8unpack-0.9.3/src/v8unpack/MetaObject/ConfigurationExtension803.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaObject/ExternalDataProcessor.py` & `v8unpack-0.9.3/src/v8unpack/MetaObject/ExternalDataProcessor.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/MetaObject/__init__.py` & `v8unpack-0.9.3/src/v8unpack/MetaObject/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,18 +138,24 @@
             helper.txt_write(code, dest_dir, filename, encoding=encoding)
 
     def decode_code(self, src_dir):
         for code_name in self.ext_code:
             _obj_code_dir = f'{os.path.join(src_dir, self.header["uuid"])}.{self.ext_code[code_name]}'
             if os.path.isdir(_obj_code_dir):
                 self.header[f'code_info_{code_name}'] = helper.json_read(_obj_code_dir, 'info.json')
-                self.code[code_name] = self.read_raw_code(_obj_code_dir, 'text.bin')
-
-                encoding = helper.detect_by_bom(os.path.join(_obj_code_dir, 'text.bin'), 'utf-8')
-                self.header[f'code_encoding_{code_name}'] = encoding  # можно безболезненно поменять на utf-8-sig
+                try:
+                    self.code[code_name] = self.read_raw_code(_obj_code_dir, 'text.bin')
+                    encoding = helper.detect_by_bom(os.path.join(_obj_code_dir, 'text.bin'), 'utf-8')
+                    self.header[f'code_encoding_{code_name}'] = encoding  # можно безболезненно поменять на utf-8-sig
+                except FileNotFoundError as err:
+                    # todo могут быть зашифрованные модули тогда файл будет # image.json - зашифрованный контент
+                    if os.path.isfile(os.path.join(_obj_code_dir, 'text.json')):
+                        print(f'Работа с зашифрованными модулями пока не поддерживается, обратитесь к разработчику')
+                    else:
+                        raise err from err
 
     def write_decode_code(self, dest_dir, file_name):
         for code_name in self.code:
             if self.code[code_name]:
                 helper.txt_write(self.code[code_name], dest_dir, f'{file_name}.{code_name}.1c')
 
     def encode_code(self, src_dir, file_name):
```

### Comparing `v8unpack-0.9.2/src/v8unpack/code_organizer.py` & `v8unpack-0.9.3/src/v8unpack/code_organizer.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/container_reader.py` & `v8unpack-0.9.3/src/v8unpack/container_reader.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/container_writer.py` & `v8unpack-0.9.3/src/v8unpack/container_writer.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/decoder.py` & `v8unpack-0.9.3/src/v8unpack/decoder.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/ext_exception.py` & `v8unpack-0.9.3/src/v8unpack/ext_exception.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/file_organizer.py` & `v8unpack-0.9.3/src/v8unpack/file_organizer.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/file_organizer_ce.py` & `v8unpack-0.9.3/src/v8unpack/file_organizer_ce.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/helper.py` & `v8unpack-0.9.3/src/v8unpack/helper.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/index.py` & `v8unpack-0.9.3/src/v8unpack/index.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/json_container_decoder.py` & `v8unpack-0.9.3/src/v8unpack/json_container_decoder.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/metadata_types.py` & `v8unpack-0.9.3/src/v8unpack/metadata_types.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/unittest_helper.py` & `v8unpack-0.9.3/src/v8unpack/unittest_helper.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack/v8unpack.py` & `v8unpack-0.9.3/src/v8unpack/v8unpack.py`

 * *Files identical despite different names*

### Comparing `v8unpack-0.9.2/src/v8unpack.egg-info/PKG-INFO` & `v8unpack-0.9.3/src/v8unpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v8unpack
-Version: 0.9.2
+Version: 0.9.3
 Summary: Unpacking binaries 1C to JSON for GIT
 Home-page: https://github.com/saby-integration/v8unpack
 Author: Razgovorov Mikhail
 Author-email: 1338833@gmail.com
 License: MIT
 Keywords: 1C CF CFE EPF V8UNPACK SABY SBIS СБИС 1С
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `v8unpack-0.9.2/src/v8unpack.egg-info/SOURCES.txt` & `v8unpack-0.9.3/src/v8unpack.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 src/v8unpack/MetaDataObject/EventSubscription.py
 src/v8unpack/MetaDataObject/ExchangePlan.py
 src/v8unpack/MetaDataObject/ExchangePlanForm.py
 src/v8unpack/MetaDataObject/FilterCriterion.py
 src/v8unpack/MetaDataObject/FilterCriterionForm.py
 src/v8unpack/MetaDataObject/Form.py
 src/v8unpack/MetaDataObject/FunctionalOption.py
+src/v8unpack/MetaDataObject/HTTPService.py
 src/v8unpack/MetaDataObject/InformationRegister.py
 src/v8unpack/MetaDataObject/InformationRegisterCommand.py
 src/v8unpack/MetaDataObject/InformationRegisterForm.py
 src/v8unpack/MetaDataObject/Interface.py
 src/v8unpack/MetaDataObject/Language.py
 src/v8unpack/MetaDataObject/Report.py
 src/v8unpack/MetaDataObject/ReportForm.py
@@ -76,14 +77,15 @@
 src/v8unpack/MetaDataObject/versions/CommonForm803.py
 src/v8unpack/MetaDataObject/versions/CommonTemplate803.py
 src/v8unpack/MetaDataObject/versions/DocumentForm803.py
 src/v8unpack/MetaDataObject/versions/Form801.py
 src/v8unpack/MetaDataObject/versions/Form802.py
 src/v8unpack/MetaDataObject/versions/Form803.py
 src/v8unpack/MetaDataObject/versions/Form8x.py
+src/v8unpack/MetaDataObject/versions/ReportForm803.py
 src/v8unpack/MetaDataObject/versions/Template801.py
 src/v8unpack/MetaDataObject/versions/Template802.py
 src/v8unpack/MetaDataObject/versions/Template803.py
 src/v8unpack/MetaDataObject/versions/Template8x.py
 src/v8unpack/MetaDataObject/versions/__init__.py
 src/v8unpack/MetaObject/Configuration802.py
 src/v8unpack/MetaObject/Configuration803.py
```

