# Comparing `tmp/generateDS-2.8b.tar.gz` & `tmp/generateDS-2.9a.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/generateDS-2.8b.tar", last modified: Wed Jan 30 21:23:05 2013, max compression
+gzip compressed data, was "dist/generateDS-2.9a.tar", last modified: Thu Feb 21 00:42:14 2013, max compression
```

## Comparing `generateDS-2.8b.tar` & `generateDS-2.9a.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/generateDS.egg-info/
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)        1 2013-01-30 21:23:00.000000 generateDS-2.8b/generateDS.egg-info/dependency_links.txt
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      858 2013-01-30 21:23:00.000000 generateDS-2.8b/generateDS.egg-info/PKG-INFO
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)       14 2013-01-30 21:23:00.000000 generateDS-2.8b/generateDS.egg-info/top_level.txt
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     3844 2013-01-30 21:23:00.000000 generateDS-2.8b/generateDS.egg-info/SOURCES.txt
--rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)     6423 2010-11-01 17:24:11.000000 generateDS-2.8b/gends_user_methods.py
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/gui/
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    38989 2011-01-18 23:39:10.000000 generateDS-2.8b/gui/generateds_gui_session.py
--rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)    94943 2013-01-17 16:24:12.000000 generateDS-2.8b/gui/generateds_gui.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1677 2010-12-08 20:03:32.000000 generateDS-2.8b/gui/generateds_gui_session.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      973 2010-11-01 17:24:11.000000 generateDS-2.8b/gui/sample.session
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    66162 2010-12-08 23:48:30.000000 generateDS-2.8b/gui/generateds_gui.glade
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/SWIG/
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      125 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/test1b.h
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4776 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/testsub.py
--rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)       47 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/run_swig
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)       60 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/test1.i
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      665 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/test1.h
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    60480 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/test1.xml
--rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)    33647 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/generateDS.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    41337 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/testsuper.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     3763 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/README
--rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)       76 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/run_generate
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      196 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/test1a.h
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    16127 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/genswig.zip
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6974 2010-11-01 17:24:11.000000 generateDS-2.8b/SWIG/swigxml15.xsd
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/Demos/
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/Demos/Outline/
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      840 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Outline/outline.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6587 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Outline/outline.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     2224 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Outline/outline_extended.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      844 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Outline/README
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      861 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Outline/outlinetest.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1715 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Outline/outline.xml
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/Demos/Xmlbehavior/
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     2540 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Xmlbehavior/xmlbehavior.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4046 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Xmlbehavior/po_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1452 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Xmlbehavior/po.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    29105 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Xmlbehavior/xmlbehavior.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1520 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Xmlbehavior/README
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4673 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Xmlbehavior/xmlbehavior_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     3055 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Xmlbehavior/xmlbehavior_po.xml
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    22771 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/Xmlbehavior/po.py
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/Demos/People/
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1021 2011-02-01 22:33:59.000000 generateDS-2.8b/Demos/People/a1.session
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    12990 2013-01-30 21:05:20.000000 generateDS-2.8b/Demos/People/people.xsd
--rwxr--r--   0 dkuhlman  (1000) dkuhlman  (1000)      329 2011-02-01 21:34:08.000000 generateDS-2.8b/Demos/People/run_test
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1620 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/People/README
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/Demos/People/Validators/
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)       89 2010-11-01 17:24:11.000000 generateDS-2.8b/Demos/People/Validators/percent.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)       86 2011-05-27 21:54:12.000000 generateDS-2.8b/Demos/People/Validators/FlowType.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5717 2013-01-30 21:06:58.000000 generateDS-2.8b/Demos/People/people.xml
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)   127296 2011-02-01 22:34:02.000000 generateDS-2.8b/Demos/People/peoplesup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    11223 2011-02-01 22:34:02.000000 generateDS-2.8b/Demos/People/peoplesub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4209 2013-01-28 23:39:33.000000 generateDS-2.8b/MANIFEST.in
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)   137574 2013-01-28 23:38:56.000000 generateDS-2.8b/generateDS.html
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5219 2013-01-17 16:24:12.000000 generateDS-2.8b/librarytemplate_howto.txt
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    13398 2010-11-10 21:38:37.000000 generateDS-2.8b/librarytemplate-1.0a.zip
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)      858 2013-01-30 21:23:05.000000 generateDS-2.8b/PKG-INFO
--rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)     3800 2010-11-01 17:24:11.000000 generateDS-2.8b/generate_coverage.py
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/libgenerateDS/
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/libgenerateDS/gui/
-hrw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)        0 2011-01-18 23:39:10.000000 generateDS-2.8b/libgenerateDS/gui/generateds_gui_session.py
-hrwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-17 16:24:12.000000 generateDS-2.8b/libgenerateDS/gui/generateds_gui.py
--rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)     6928 2011-02-15 17:45:34.000000 generateDS-2.8b/libgenerateDS/process_includes.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1634 2013-01-17 16:24:12.000000 generateDS-2.8b/setup.py
--rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)   215063 2013-01-30 17:44:06.000000 generateDS-2.8b/generateDS.py
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/tutorial/
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1278 2013-01-17 16:24:12.000000 generateDS-2.8b/tutorial/generateds_tutorial.txt
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    50837 2013-01-28 23:38:57.000000 generateDS-2.8b/tutorial/generateds_tutorial.html
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/tutorial/Code/
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)   137275 2011-09-23 22:04:32.000000 generateDS-2.8b/tutorial/Code/people_api.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    12378 2011-09-23 21:55:59.000000 generateDS-2.8b/tutorial/Code/people.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      540 2011-09-29 21:14:25.000000 generateDS-2.8b/tutorial/Code/upcase_names.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      345 2010-11-01 17:24:11.000000 generateDS-2.8b/tutorial/Code/member_specs_data.xml
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    29532 2011-09-30 17:39:12.000000 generateDS-2.8b/tutorial/Code/member_specs_api.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1097 2010-11-10 03:33:12.000000 generateDS-2.8b/tutorial/Code/member_specs_test.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      940 2010-11-01 17:24:11.000000 generateDS-2.8b/tutorial/Code/member_specs.xsd
--rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)       65 2010-11-01 17:24:11.000000 generateDS-2.8b/tutorial/Code/member_specs_run
--rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)      172 2011-09-30 17:39:03.000000 generateDS-2.8b/tutorial/Code/member_specs_generate
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5384 2011-09-23 22:02:36.000000 generateDS-2.8b/tutorial/Code/people.xml
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5864 2011-09-30 17:46:26.000000 generateDS-2.8b/tutorial/Code/member_specs_upper.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    12244 2011-09-23 22:50:32.000000 generateDS-2.8b/tutorial/Code/upcase_names_appl.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    12080 2011-09-23 22:04:32.000000 generateDS-2.8b/tutorial/Code/people_appl1.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    33677 2011-09-29 21:36:08.000000 generateDS-2.8b/tutorial/generateds_tutoriala.txt
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    48724 2013-01-28 23:38:57.000000 generateDS-2.8b/tutorial/generateds_tutorial.zip
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)       59 2013-01-30 21:23:05.000000 generateDS-2.8b/setup.cfg
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/django/
--rwxr--r--   0 dkuhlman  (1000) dkuhlman  (1000)     3663 2011-01-28 22:02:22.000000 generateDS-2.8b/django/gends_run_gen_django.py
--rwxr--r--   0 dkuhlman  (1000) dkuhlman  (1000)     9332 2011-01-31 19:40:21.000000 generateDS-2.8b/django/gends_extract_simple_types.py
--rwxr--r--   0 dkuhlman  (1000) dkuhlman  (1000)     3748 2011-02-01 00:04:34.000000 generateDS-2.8b/django/gends_generate_django.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6549 2012-02-18 17:24:41.000000 generateDS-2.8b/django/generatedssuper.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    59043 2013-01-30 20:50:43.000000 generateDS-2.8b/README
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    11356 2013-01-28 23:38:56.000000 generateDS-2.8b/librarytemplate_howto.html
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    92697 2013-01-17 16:24:12.000000 generateDS-2.8b/generateDS.txt
-drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-01-30 21:23:05.000000 generateDS-2.8b/tests/
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    28549 2013-01-30 18:16:20.000000 generateDS-2.8b/tests/simpletype_memberspecs1_sup.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     5149 2013-01-30 18:17:32.000000 generateDS-2.8b/tests/anysimpletype1_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1112 2013-01-30 18:18:57.000000 generateDS-2.8b/tests/ipo2_out.xml
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      867 2013-01-29 22:37:42.000000 generateDS-2.8b/tests/ipo.xml
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    33749 2013-01-30 18:09:25.000000 generateDS-2.8b/tests/abstract_type1_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    25808 2013-01-30 18:18:58.000000 generateDS-2.8b/tests/recursive_simpletype2_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5167 2013-01-30 18:16:21.000000 generateDS-2.8b/tests/simpletype_memberspecs1_sub.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     6378 2013-01-30 18:05:38.000000 generateDS-2.8b/tests/anywildcard1_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      804 2011-09-22 22:24:43.000000 generateDS-2.8b/tests/recursive_simpletype.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5400 2013-01-30 18:10:06.000000 generateDS-2.8b/tests/annotations1_sub.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    31923 2013-01-30 18:18:58.000000 generateDS-2.8b/tests/attr_groups2_sup.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     5005 2013-01-30 18:04:49.000000 generateDS-2.8b/tests/attr_groups1_sub.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)   146346 2013-01-30 18:18:58.000000 generateDS-2.8b/tests/out2_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4871 2013-01-30 18:18:58.000000 generateDS-2.8b/tests/recursive_simpletype2_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    39153 2013-01-30 18:10:45.000000 generateDS-2.8b/tests/simplecontent_restriction1_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     8246 2013-01-09 19:16:35.000000 generateDS-2.8b/tests/people.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4871 2013-01-30 18:07:01.000000 generateDS-2.8b/tests/recursive_simpletype1_sub.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    51155 2013-01-30 18:03:45.000000 generateDS-2.8b/tests/simpletypes_other1_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    34869 2013-01-30 18:10:06.000000 generateDS-2.8b/tests/annotations1_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6300 2013-01-30 18:07:54.000000 generateDS-2.8b/tests/ipo1_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    71296 2013-01-30 18:11:27.000000 generateDS-2.8b/tests/extensions1_sup.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    46609 2013-01-30 18:18:58.000000 generateDS-2.8b/tests/anywildcard2_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     7823 2013-01-30 18:11:27.000000 generateDS-2.8b/tests/extensions1_sub.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     5778 2013-01-30 18:18:59.000000 generateDS-2.8b/tests/simpletypes_other2_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6300 2013-01-30 18:18:57.000000 generateDS-2.8b/tests/ipo2_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5322 2013-01-30 18:18:56.000000 generateDS-2.8b/tests/abstract_type2_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5322 2013-01-30 18:09:25.000000 generateDS-2.8b/tests/abstract_type1_sub.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     6378 2013-01-30 18:18:58.000000 generateDS-2.8b/tests/anywildcard2_sub.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     1188 2012-11-12 23:07:17.000000 generateDS-2.8b/tests/attr_groups.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1827 2011-07-15 18:18:40.000000 generateDS-2.8b/tests/ipo.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6342 2013-01-09 19:24:13.000000 generateDS-2.8b/tests/literal1.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    31923 2013-01-30 18:04:49.000000 generateDS-2.8b/tests/attr_groups1_sup.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    10177 2013-01-30 18:18:58.000000 generateDS-2.8b/tests/out2_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1942 2010-11-01 17:24:11.000000 generateDS-2.8b/tests/simplecontent_restriction.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1324 2010-11-01 17:24:11.000000 generateDS-2.8b/tests/groups.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     2673 2010-11-01 17:24:11.000000 generateDS-2.8b/tests/simpletype_memberspecs.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1427 2010-11-01 17:24:11.000000 generateDS-2.8b/tests/annotations.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    59442 2013-01-30 18:18:57.000000 generateDS-2.8b/tests/ipo2_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     2697 2013-01-17 18:10:43.000000 generateDS-2.8b/tests/simpletypes_other.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      493 2010-11-01 17:24:11.000000 generateDS-2.8b/tests/groups.xml
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    51155 2013-01-30 18:18:59.000000 generateDS-2.8b/tests/simpletypes_other2_sup.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    34869 2013-01-30 18:18:56.000000 generateDS-2.8b/tests/annotations2_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)   142692 2013-01-30 18:08:51.000000 generateDS-2.8b/tests/people_procincl1_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    25808 2013-01-30 18:07:01.000000 generateDS-2.8b/tests/recursive_simpletype1_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      784 2010-08-09 18:32:22.000000 generateDS-2.8b/tests/abstract_type.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    11411 2013-01-30 18:18:57.000000 generateDS-2.8b/tests/people_procincl2_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      689 2010-11-01 17:24:11.000000 generateDS-2.8b/tests/anysimpletype.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)   146346 2013-01-30 18:18:48.000000 generateDS-2.8b/tests/out1_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)   142692 2013-01-30 18:18:57.000000 generateDS-2.8b/tests/people_procincl2_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      959 2010-08-27 22:37:19.000000 generateDS-2.8b/tests/people_procincl.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    11411 2013-01-30 18:08:51.000000 generateDS-2.8b/tests/people_procincl1_sub.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     5005 2013-01-30 18:18:58.000000 generateDS-2.8b/tests/attr_groups2_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      255 2010-11-01 17:24:11.000000 generateDS-2.8b/tests/valueof.xml
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4947 2010-11-01 17:24:11.000000 generateDS-2.8b/tests/extensions.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    59442 2013-01-30 18:07:54.000000 generateDS-2.8b/tests/ipo1_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4146 2013-01-09 19:03:22.000000 generateDS-2.8b/tests/people.xml
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    46609 2013-01-30 18:05:38.000000 generateDS-2.8b/tests/anywildcard1_sup.py
--rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     5400 2013-01-30 18:18:56.000000 generateDS-2.8b/tests/annotations2_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1112 2013-01-29 22:58:40.000000 generateDS-2.8b/tests/ipo1_out.xml
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    10177 2013-01-30 18:18:48.000000 generateDS-2.8b/tests/out1_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    30096 2013-01-30 18:17:32.000000 generateDS-2.8b/tests/anysimpletype1_sup.py
--rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)    16602 2012-11-26 21:24:03.000000 generateDS-2.8b/tests/test.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     2474 2012-01-16 03:36:24.000000 generateDS-2.8b/tests/anywildcard.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     8087 2010-08-27 22:35:37.000000 generateDS-2.8b/tests/people_procincl_b.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     2155 2010-08-30 20:37:45.000000 generateDS-2.8b/tests/people_procincl_a.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6206 2013-01-30 18:10:45.000000 generateDS-2.8b/tests/simplecontent_restriction1_sub.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      896 2010-11-01 17:24:11.000000 generateDS-2.8b/tests/valueof.xsd
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    33749 2013-01-30 18:18:56.000000 generateDS-2.8b/tests/abstract_type2_sup.py
--rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1125 2010-11-01 17:24:11.000000 generateDS-2.8b/LICENSE
--rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)    11359 2013-01-17 16:24:12.000000 generateDS-2.8b/process_includes.py
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/generateDS.egg-info/
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)        1 2013-02-21 00:42:07.000000 generateDS-2.9a/generateDS.egg-info/dependency_links.txt
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      858 2013-02-21 00:42:07.000000 generateDS-2.9a/generateDS.egg-info/PKG-INFO
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)       14 2013-02-21 00:42:07.000000 generateDS-2.9a/generateDS.egg-info/top_level.txt
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     3844 2013-02-21 00:42:08.000000 generateDS-2.9a/generateDS.egg-info/SOURCES.txt
+-rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)     6423 2010-11-01 17:24:11.000000 generateDS-2.9a/gends_user_methods.py
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/gui/
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    38989 2011-01-18 23:39:10.000000 generateDS-2.9a/gui/generateds_gui_session.py
+-rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)    94943 2013-02-18 16:34:29.000000 generateDS-2.9a/gui/generateds_gui.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1677 2010-12-08 20:03:32.000000 generateDS-2.9a/gui/generateds_gui_session.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      973 2010-11-01 17:24:11.000000 generateDS-2.9a/gui/sample.session
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    66162 2010-12-08 23:48:30.000000 generateDS-2.9a/gui/generateds_gui.glade
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/SWIG/
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      125 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/test1b.h
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4776 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/testsub.py
+-rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)       47 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/run_swig
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)       60 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/test1.i
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      665 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/test1.h
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    60480 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/test1.xml
+-rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)    33647 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/generateDS.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    41337 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/testsuper.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     3763 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/README
+-rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)       76 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/run_generate
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      196 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/test1a.h
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    16127 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/genswig.zip
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6974 2010-11-01 17:24:11.000000 generateDS-2.9a/SWIG/swigxml15.xsd
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/Demos/
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/Demos/Outline/
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      840 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Outline/outline.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6587 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Outline/outline.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     2224 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Outline/outline_extended.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      844 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Outline/README
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      861 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Outline/outlinetest.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1715 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Outline/outline.xml
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/Demos/Xmlbehavior/
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     2540 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Xmlbehavior/xmlbehavior.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4046 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Xmlbehavior/po_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1452 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Xmlbehavior/po.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    29105 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Xmlbehavior/xmlbehavior.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1520 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Xmlbehavior/README
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4673 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Xmlbehavior/xmlbehavior_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     3055 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Xmlbehavior/xmlbehavior_po.xml
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    22771 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/Xmlbehavior/po.py
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/Demos/People/
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1021 2011-02-01 22:33:59.000000 generateDS-2.9a/Demos/People/a1.session
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    13743 2013-02-18 17:40:13.000000 generateDS-2.9a/Demos/People/people.xsd
+-rwxr--r--   0 dkuhlman  (1000) dkuhlman  (1000)      329 2011-02-01 21:34:08.000000 generateDS-2.9a/Demos/People/run_test
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1620 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/People/README
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/Demos/People/Validators/
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)       89 2010-11-01 17:24:11.000000 generateDS-2.9a/Demos/People/Validators/percent.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)       86 2011-05-27 21:54:12.000000 generateDS-2.9a/Demos/People/Validators/FlowType.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6268 2013-02-20 19:42:00.000000 generateDS-2.9a/Demos/People/people.xml
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)   127296 2011-02-01 22:34:02.000000 generateDS-2.9a/Demos/People/peoplesup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    11223 2011-02-01 22:34:02.000000 generateDS-2.9a/Demos/People/peoplesub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4209 2013-01-28 23:39:33.000000 generateDS-2.9a/MANIFEST.in
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)   140160 2013-02-21 00:41:26.000000 generateDS-2.9a/generateDS.html
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5219 2013-02-18 16:34:29.000000 generateDS-2.9a/librarytemplate_howto.txt
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    13398 2010-11-10 21:38:37.000000 generateDS-2.9a/librarytemplate-1.0a.zip
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)      858 2013-02-21 00:42:14.000000 generateDS-2.9a/PKG-INFO
+-rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)     3800 2010-11-01 17:24:11.000000 generateDS-2.9a/generate_coverage.py
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/libgenerateDS/
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/libgenerateDS/gui/
+hrw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)        0 2011-01-18 23:39:10.000000 generateDS-2.9a/libgenerateDS/gui/generateds_gui_session.py
+hrwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-18 16:34:29.000000 generateDS-2.9a/libgenerateDS/gui/generateds_gui.py
+-rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)     6928 2011-02-15 17:45:34.000000 generateDS-2.9a/libgenerateDS/process_includes.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1634 2013-02-18 16:34:29.000000 generateDS-2.9a/setup.py
+-rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)   226992 2013-02-20 19:28:10.000000 generateDS-2.9a/generateDS.py
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/tutorial/
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1278 2013-02-18 16:34:29.000000 generateDS-2.9a/tutorial/generateds_tutorial.txt
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    50838 2013-02-21 00:41:26.000000 generateDS-2.9a/tutorial/generateds_tutorial.html
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/tutorial/Code/
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)   137275 2011-09-23 22:04:32.000000 generateDS-2.9a/tutorial/Code/people_api.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    12378 2011-09-23 21:55:59.000000 generateDS-2.9a/tutorial/Code/people.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      540 2011-09-29 21:14:25.000000 generateDS-2.9a/tutorial/Code/upcase_names.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      345 2010-11-01 17:24:11.000000 generateDS-2.9a/tutorial/Code/member_specs_data.xml
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    29532 2011-09-30 17:39:12.000000 generateDS-2.9a/tutorial/Code/member_specs_api.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1097 2010-11-10 03:33:12.000000 generateDS-2.9a/tutorial/Code/member_specs_test.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      940 2010-11-01 17:24:11.000000 generateDS-2.9a/tutorial/Code/member_specs.xsd
+-rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)       65 2010-11-01 17:24:11.000000 generateDS-2.9a/tutorial/Code/member_specs_run
+-rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)      172 2011-09-30 17:39:03.000000 generateDS-2.9a/tutorial/Code/member_specs_generate
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5384 2011-09-23 22:02:36.000000 generateDS-2.9a/tutorial/Code/people.xml
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5864 2011-09-30 17:46:26.000000 generateDS-2.9a/tutorial/Code/member_specs_upper.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    12244 2011-09-23 22:50:32.000000 generateDS-2.9a/tutorial/Code/upcase_names_appl.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    12080 2011-09-23 22:04:32.000000 generateDS-2.9a/tutorial/Code/people_appl1.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    33677 2011-09-29 21:36:08.000000 generateDS-2.9a/tutorial/generateds_tutoriala.txt
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    48722 2013-02-21 00:41:27.000000 generateDS-2.9a/tutorial/generateds_tutorial.zip
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)       59 2013-02-21 00:42:14.000000 generateDS-2.9a/setup.cfg
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/django/
+-rwxr--r--   0 dkuhlman  (1000) dkuhlman  (1000)     3663 2011-01-28 22:02:22.000000 generateDS-2.9a/django/gends_run_gen_django.py
+-rwxr--r--   0 dkuhlman  (1000) dkuhlman  (1000)     9332 2011-01-31 19:40:21.000000 generateDS-2.9a/django/gends_extract_simple_types.py
+-rwxr--r--   0 dkuhlman  (1000) dkuhlman  (1000)     3748 2011-02-01 00:04:34.000000 generateDS-2.9a/django/gends_generate_django.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6549 2012-02-18 17:24:41.000000 generateDS-2.9a/django/generatedssuper.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    61000 2013-02-20 22:45:24.000000 generateDS-2.9a/README
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    11357 2013-02-21 00:41:26.000000 generateDS-2.9a/librarytemplate_howto.html
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    94750 2013-02-18 23:01:47.000000 generateDS-2.9a/generateDS.txt
+drwxrwxr-x   0 dkuhlman  (1000) dkuhlman  (1000)        0 2013-02-21 00:42:14.000000 generateDS-2.9a/tests/
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    30951 2013-02-18 19:24:47.000000 generateDS-2.9a/tests/simpletype_memberspecs1_sup.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     5776 2013-02-18 19:26:04.000000 generateDS-2.9a/tests/anysimpletype1_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1112 2013-02-20 20:03:29.000000 generateDS-2.9a/tests/ipo2_out.xml
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      867 2013-01-29 22:37:42.000000 generateDS-2.9a/tests/ipo.xml
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    36361 2013-02-18 19:19:54.000000 generateDS-2.9a/tests/abstract_type1_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    28121 2013-02-20 20:03:30.000000 generateDS-2.9a/tests/recursive_simpletype2_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5792 2013-02-18 19:24:47.000000 generateDS-2.9a/tests/simpletype_memberspecs1_sub.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     7013 2013-02-18 19:10:22.000000 generateDS-2.9a/tests/anywildcard1_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      804 2011-09-22 22:24:43.000000 generateDS-2.9a/tests/recursive_simpletype.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6025 2013-02-18 19:20:54.000000 generateDS-2.9a/tests/annotations1_sub.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    34165 2013-02-20 20:03:30.000000 generateDS-2.9a/tests/attr_groups2_sup.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     5625 2013-02-18 19:07:42.000000 generateDS-2.9a/tests/attr_groups1_sub.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)   149535 2013-02-20 20:03:31.000000 generateDS-2.9a/tests/out2_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5490 2013-02-20 20:03:30.000000 generateDS-2.9a/tests/recursive_simpletype2_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    41611 2013-02-18 19:21:59.000000 generateDS-2.9a/tests/simplecontent_restriction1_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     8246 2013-01-09 19:16:35.000000 generateDS-2.9a/tests/people.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5490 2013-02-18 19:14:28.000000 generateDS-2.9a/tests/recursive_simpletype1_sub.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    53537 2013-02-18 16:46:24.000000 generateDS-2.9a/tests/simpletypes_other1_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    37390 2013-02-18 19:20:54.000000 generateDS-2.9a/tests/annotations1_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6921 2013-02-18 19:16:07.000000 generateDS-2.9a/tests/ipo1_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    74621 2013-02-18 19:23:59.000000 generateDS-2.9a/tests/extensions1_sup.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    49443 2013-02-20 20:03:30.000000 generateDS-2.9a/tests/anywildcard2_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     8448 2013-02-18 19:23:59.000000 generateDS-2.9a/tests/extensions1_sub.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     6415 2013-02-20 20:03:30.000000 generateDS-2.9a/tests/simpletypes_other2_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6921 2013-02-20 20:03:29.000000 generateDS-2.9a/tests/ipo2_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5943 2013-02-20 20:03:27.000000 generateDS-2.9a/tests/abstract_type2_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     5943 2013-02-18 19:19:54.000000 generateDS-2.9a/tests/abstract_type1_sub.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     7013 2013-02-20 20:03:30.000000 generateDS-2.9a/tests/anywildcard2_sub.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     1188 2012-11-12 23:07:17.000000 generateDS-2.9a/tests/attr_groups.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1827 2011-07-15 18:18:40.000000 generateDS-2.9a/tests/ipo.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6342 2013-01-09 19:24:13.000000 generateDS-2.9a/tests/literal1.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    34165 2013-02-18 19:07:42.000000 generateDS-2.9a/tests/attr_groups1_sup.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    10780 2013-02-20 20:03:31.000000 generateDS-2.9a/tests/out2_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1942 2010-11-01 17:24:11.000000 generateDS-2.9a/tests/simplecontent_restriction.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1324 2010-11-01 17:24:11.000000 generateDS-2.9a/tests/groups.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     2673 2010-11-01 17:24:11.000000 generateDS-2.9a/tests/simpletype_memberspecs.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1427 2010-11-01 17:24:11.000000 generateDS-2.9a/tests/annotations.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    62321 2013-02-20 20:03:29.000000 generateDS-2.9a/tests/ipo2_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     2697 2013-01-17 18:10:43.000000 generateDS-2.9a/tests/simpletypes_other.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      493 2010-11-01 17:24:11.000000 generateDS-2.9a/tests/groups.xml
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    53537 2013-02-20 20:03:30.000000 generateDS-2.9a/tests/simpletypes_other2_sup.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    37390 2013-02-20 20:03:27.000000 generateDS-2.9a/tests/annotations2_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)   146282 2013-02-18 19:19:05.000000 generateDS-2.9a/tests/people_procincl1_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    28121 2013-02-18 19:14:28.000000 generateDS-2.9a/tests/recursive_simpletype1_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      784 2010-08-09 18:32:22.000000 generateDS-2.9a/tests/abstract_type.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    12026 2013-02-20 20:03:29.000000 generateDS-2.9a/tests/people_procincl2_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      689 2010-11-01 17:24:11.000000 generateDS-2.9a/tests/anysimpletype.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)   149535 2013-02-18 19:27:23.000000 generateDS-2.9a/tests/out1_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)   146282 2013-02-20 20:03:29.000000 generateDS-2.9a/tests/people_procincl2_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      959 2010-08-27 22:37:19.000000 generateDS-2.9a/tests/people_procincl.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    12026 2013-02-18 19:19:05.000000 generateDS-2.9a/tests/people_procincl1_sub.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     5625 2013-02-20 20:03:30.000000 generateDS-2.9a/tests/attr_groups2_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      255 2010-11-01 17:24:11.000000 generateDS-2.9a/tests/valueof.xml
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4947 2010-11-01 17:24:11.000000 generateDS-2.9a/tests/extensions.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    62321 2013-02-18 19:16:07.000000 generateDS-2.9a/tests/ipo1_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     4146 2013-01-09 19:03:22.000000 generateDS-2.9a/tests/people.xml
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)    49443 2013-02-18 19:10:22.000000 generateDS-2.9a/tests/anywildcard1_sup.py
+-rw-rw-r--   0 dkuhlman  (1000) dkuhlman  (1000)     6025 2013-02-20 20:03:27.000000 generateDS-2.9a/tests/annotations2_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1112 2013-01-29 22:58:40.000000 generateDS-2.9a/tests/ipo1_out.xml
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    10780 2013-02-18 19:27:23.000000 generateDS-2.9a/tests/out1_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    32500 2013-02-18 19:26:04.000000 generateDS-2.9a/tests/anysimpletype1_sup.py
+-rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)    17824 2013-02-18 22:50:02.000000 generateDS-2.9a/tests/test.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     2474 2012-01-16 03:36:24.000000 generateDS-2.9a/tests/anywildcard.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     8087 2010-08-27 22:35:37.000000 generateDS-2.9a/tests/people_procincl_b.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     2155 2010-08-30 20:37:45.000000 generateDS-2.9a/tests/people_procincl_a.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     6837 2013-02-18 19:21:59.000000 generateDS-2.9a/tests/simplecontent_restriction1_sub.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)      896 2010-11-01 17:24:11.000000 generateDS-2.9a/tests/valueof.xsd
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)    36361 2013-02-20 20:03:27.000000 generateDS-2.9a/tests/abstract_type2_sup.py
+-rw-r--r--   0 dkuhlman  (1000) dkuhlman  (1000)     1125 2010-11-01 17:24:11.000000 generateDS-2.9a/LICENSE
+-rwxr-xr-x   0 dkuhlman  (1000) dkuhlman  (1000)    11359 2013-02-18 16:34:29.000000 generateDS-2.9a/process_includes.py
```

### Comparing `generateDS-2.8b/generateDS.egg-info/PKG-INFO` & `generateDS-2.9a/generateDS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: generateDS
-Version: 2.8b
+Version: 2.9a
 Summary: Generate Python data structures and XML parser from Xschema
 Home-page: http://www.rexx.com/~dkuhlman/generateDS.html
 Author: Dave Kuhlman
 Author-email: dkuhlman@rexx.com
 License: http://www.opensource.org/licenses/mit-license.php
 Description: generateDS.py generates Python data structures (for example, class
         definitions) from an XML Schema document.  These data structures
```

### Comparing `generateDS-2.8b/generateDS.egg-info/SOURCES.txt` & `generateDS-2.9a/generateDS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/gends_user_methods.py` & `generateDS-2.9a/gends_user_methods.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/gui/generateds_gui_session.py` & `generateDS-2.9a/gui/generateds_gui_session.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/gui/generateds_gui.py` & `generateDS-2.9a/gui/generateds_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 # Globals and constants:
 
 #
 # Do not modify the following VERSION comments.
 # Used by updateversion.py.
 ##VERSION##
-VERSION = '2.8b'
+VERSION = '2.9a'
 ##VERSION##
 
 
 Builder = None
 ParamNameList = []
 CmdTemplate = (
     '%(exec_path)s --no-questions' +
```

### Comparing `generateDS-2.8b/gui/generateds_gui_session.xsd` & `generateDS-2.9a/gui/generateds_gui_session.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/gui/sample.session` & `generateDS-2.9a/gui/sample.session`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/gui/generateds_gui.glade` & `generateDS-2.9a/gui/generateds_gui.glade`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/SWIG/testsub.py` & `generateDS-2.9a/SWIG/testsub.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/SWIG/test1.h` & `generateDS-2.9a/SWIG/test1.h`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/SWIG/test1.xml` & `generateDS-2.9a/SWIG/test1.xml`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/SWIG/generateDS.py` & `generateDS-2.9a/SWIG/generateDS.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/SWIG/testsuper.py` & `generateDS-2.9a/SWIG/testsuper.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/SWIG/README` & `generateDS-2.9a/SWIG/README`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/SWIG/genswig.zip` & `generateDS-2.9a/SWIG/genswig.zip`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/SWIG/swigxml15.xsd` & `generateDS-2.9a/SWIG/swigxml15.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Outline/outline.xsd` & `generateDS-2.9a/Demos/Outline/outline.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Outline/outline.py` & `generateDS-2.9a/Demos/Outline/outline.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Outline/outline_extended.py` & `generateDS-2.9a/Demos/Outline/outline_extended.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Outline/README` & `generateDS-2.9a/Demos/Outline/README`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Outline/outlinetest.py` & `generateDS-2.9a/Demos/Outline/outlinetest.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Outline/outline.xml` & `generateDS-2.9a/Demos/Outline/outline.xml`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Xmlbehavior/xmlbehavior.xsd` & `generateDS-2.9a/Demos/Xmlbehavior/xmlbehavior.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Xmlbehavior/po_sub.py` & `generateDS-2.9a/Demos/Xmlbehavior/po_sub.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Xmlbehavior/po.xsd` & `generateDS-2.9a/Demos/Xmlbehavior/po.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Xmlbehavior/xmlbehavior.py` & `generateDS-2.9a/Demos/Xmlbehavior/xmlbehavior.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Xmlbehavior/README` & `generateDS-2.9a/Demos/Xmlbehavior/README`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Xmlbehavior/xmlbehavior_sub.py` & `generateDS-2.9a/Demos/Xmlbehavior/xmlbehavior_sub.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Xmlbehavior/xmlbehavior_po.xml` & `generateDS-2.9a/Demos/Xmlbehavior/xmlbehavior_po.xml`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/Xmlbehavior/po.py` & `generateDS-2.9a/Demos/Xmlbehavior/po.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/People/a1.session` & `generateDS-2.9a/Demos/People/a1.session`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/People/people.xsd` & `generateDS-2.9a/tutorial/Code/people.xsd`

 * *Files 3% similar despite different names*

#### Comparing `generateDS-2.8b/Demos/People/people.xsd` & `generateDS-2.9a/tutorial/Code/people.xsd`

```diff
@@ -81,16 +81,14 @@
                     -->
           <xs:element name="email" type="xs:string"/>
           <xs:element name="elposint" type="xs:positiveInteger"/>
           <xs:element name="elnonposint" type="xs:nonPositiveInteger"/>
           <xs:element name="elnegint" type="xs:negativeInteger"/>
           <xs:element name="elnonnegint" type="xs:nonNegativeInteger"/>
           <xs:element name="eldate" type="xs:date"/>
-          <xs:element name="eldatetime" type="xs:dateTime"/>
-          <xs:element name="eldatetime1" type="xs:dateTime"/>
           <xs:element name="eltoken" type="xs:token"/>
           <xs:element name="elshort" type="xs:short"/>
           <xs:element name="ellong" type="xs:long"/>
           <xs:element name="elparam" type="paramType"/>
           <xs:element name="elarraytypes" type="ArrayTypes"/>
         </xs:sequence>
         <xs:attribute name="language" type="xs:string"/>
@@ -142,18 +140,16 @@
   </xs:element>
   <xs:complexType mixed="0" name="python-programmerType">
     <xs:complexContent>
       <xs:extension base="programmerType">
         <xs:sequence>
           <xs:element name="favorite-editor" type="xs:string"/>
           <xs:element name="flowvalue" type="FlowType"/>
-          <xs:element name="drcs" type="xs:string"/>
         </xs:sequence>
         <xs:attribute name="nick-name"/>
-        <xs:attribute name="drcs" type="xs:string"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:element name="java-programmer" type="java-programmerType">
     <xs:annotation>
       <xs:documentation>A Java programmer type of person.  Programmers are very special
           and Java programmers are nice also, but not as especially wonderful
@@ -161,19 +157,14 @@
     </xs:annotation>
   </xs:element>
   <xs:complexType mixed="0" name="java-programmerType">
     <xs:complexContent>
       <xs:extension base="programmerType">
         <xs:sequence>
           <xs:element name="favorite-editor" type="xs:string"/>
-          <xs:element name="datetime1" type="xs:gYear"/>
-          <xs:element name="datetime2" type="xs:gYearMonth"/>
-          <xs:element name="datetime3" type="xs:gMonth"/>
-          <xs:element name="datetime4" type="xs:gMonthDay"/>
-          <xs:element name="datetime5" type="xs:gDay"/>
         </xs:sequence>
         <xs:attribute name="nick-name"/>
         <xs:attribute name="status"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:element name="agent" type="agentType"/>
```

### Comparing `generateDS-2.8b/Demos/People/README` & `generateDS-2.9a/Demos/People/README`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/People/people.xml` & `generateDS-2.9a/Demos/People/people.xml`

 * *Files 4% similar despite different names*

#### Comparing `generateDS-2.8b/Demos/People/people.xml` & `generateDS-2.9a/Demos/People/people.xml`

```diff
@@ -41,22 +41,31 @@
     <interest>programming</interest>
     <category>0</category>
     <agent>
       <firstname>Darren</firstname>
       <lastname>Diddly</lastname>
       <priority>4.5</priority>
       <info name="Albert Abasinian" type="321" rating="5.33"/>
-      <vehicle type="airplane">
+      <vehicle xsi:type="airplane">
         <wheelcount>36</wheelcount>
         <pilotname>Felicity Flygirl</pilotname>
       </vehicle>
       <vehicle xsi:type="automobile">
         <wheelcount>4</wheelcount>
         <drivername>Daryl Driver</drivername>
       </vehicle>
+      <!-- Note that the following does not work. "xsi:" is omitted.
+                 That means that it is not recognized as an airplane
+                 subtype of the vehicle type, and the pilotname defined
+                 in the subtype is not preserved..
+            -->
+      <vehicle type="airplane">
+        <wheelcount>48</wheelcount>
+        <pilotname>Felicity Flygirl</pilotname>
+      </vehicle>
     </agent>
     <range>25</range>
   </person>
   <specialperson id="2">
     <name>Guardo</name>
     <interest>piano</interest>
     <category>4</category>
@@ -123,15 +132,15 @@
         <fullname>Billy Bailley</fullname>
         <refid>10002</refid>
       </client-handler>
     </promoter>
     <range>26</range>
   </person>
   <person id="4"/>
-  <python-programmer drcs="git" vegetable="tomato" fruit="peach" language="python" area="xml" nick-name="davy" id="232" ratio="8.7" value="abcd">
+  <python-programmer drcs="git" vegetable="tomato" fruit="peach" language="python" area="xml" nick-name="davy" id="232" ratio="8.7" value="abcd" gui_developer="1">
     <favorite-editor>jed</favorite-editor>
     <name>Darrel Dawson</name>
     <interest>hang gliding</interest>
     <category>3344</category>
     <description>An object-orientated programmer</description>
     <email>darrel@happyprogrammers.com</email>
     <drcs>mercurial</drcs>
```

### Comparing `generateDS-2.8b/Demos/People/peoplesup.py` & `generateDS-2.9a/Demos/People/peoplesup.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/Demos/People/peoplesub.py` & `generateDS-2.9a/Demos/People/peoplesub.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/MANIFEST.in` & `generateDS-2.9a/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/generateDS.html` & `generateDS-2.9a/generateDS.html`

 * *Files 0% similar despite different names*

#### Comparing `generateDS-2.8b/generateDS.html` & `generateDS-2.9a/generateDS.html`

```diff
@@ -217,26 +217,26 @@
       <!-- version -->
       <table class="docutils field-list" frame="void" rules="none">
         <col class="field-name"/>
         <col class="field-body"/>
         <tbody valign="top">
           <tr class="field">
             <th class="field-name">revision:</th>
-            <td class="field-body">2.8b</td>
+            <td class="field-body">2.9a</td>
           </tr>
         </tbody>
       </table>
       <!-- version -->
       <table class="docutils field-list" frame="void" rules="none">
         <col class="field-name"/>
         <col class="field-body"/>
         <tbody valign="top">
           <tr class="field">
             <th class="field-name">date:</th>
-            <td class="field-body">January 28, 2013</td>
+            <td class="field-body">February 20, 2013</td>
           </tr>
         </tbody>
       </table>
       <table class="docutils field-list" frame="void" rules="none">
         <col class="field-name"/>
         <col class="field-body"/>
         <tbody valign="top">
@@ -793,14 +793,26 @@
                              Example: --external-encoding='utf-8'.
     --member-specs=list|dict
                              Generate member (type) specifications in each
                              class: a dictionary of instances of class
                              MemberSpec_ containing member name, type,
                              and array or not.  Allowed values are
                              &quot;list&quot; or &quot;dict&quot;.  Default: None.
+    --export=&lt;export-list&gt;   Specifies export functions to be generated.
+                             Value is a whitespace separated list of
+                             any of the following:
+                                 write -- write XML to file
+                                 literal -- write out python code
+                                 etree -- build element tree (can serialize
+                                     to XML)
+                             Examples: --export=&quot;write etree&quot;
+                                       --export=&quot;write&quot;
+                             Default: --export=&quot;write literal&quot;
+    -q, --no-questions       Do not ask questions, for example,
+                             force overwrite.
     --session=mysession.session
                              Load and use options from session file. You can
                              create session file in generateds_gui.py.
     --version                Print version and exit.</pre>
           <p>
             The following command line flags are recognized by
             <tt class="docutils literal">generateDS.py</tt>
@@ -993,14 +1005,82 @@
               <tt class="docutils literal">MemberSpec_</tt>
               .  Allowed
 values are &quot;list&quot; or &quot;dict&quot;.  Default: do
               <em>not</em>
               generate member
 specifications (unless --user-methods specified).
             </dd>
+            <dt>export</dt>
+            <dd>
+              <p class="first">Specify which of the export related member methods are to be
+generated.  The value is a whitespace separated list of any of
+the following:</p>
+              <ul class="simple">
+                <li>
+                  write -- Generate methods
+                  <tt class="docutils literal">export</tt>
+                  ,
+                  <tt class="docutils literal">exportAttributes</tt>
+                  ,
+and
+                  <tt class="docutils literal">exportChildren</tt>
+                  .  These methods write XML to a file.
+                </li>
+                <li>
+                  literal -- Generate methods
+                  <tt class="docutils literal">exportLiteral</tt>
+                  ,
+                  <tt class="docutils literal">exportLiteralAttributes</tt>
+                  and
+                  <tt class="docutils literal">exportLiteralChildren</tt>
+                  .
+These methods write out python code.
+                </li>
+                <li>
+                  etree -- Generate method
+                  <tt class="docutils literal">to_etree</tt>
+                  .  This method builds an
+lxml element tree, which can, for example, be serialized to
+XML using lxml's
+                  <tt class="docutils literal">tostring</tt>
+                  function and searched with the
+lxml xpath capability.  You can also iterate over nodes in the
+tree with the node's
+                  <tt class="docutils literal">getiterator</tt>
+                  ,
+                  <tt class="docutils literal">iterchildren</tt>
+                  , etc,
+and use any of lxml's other capabilities.
+                </li>
+              </ul>
+              <p class="last">
+                For example:
+                <tt class="docutils literal">
+                  <span class="pre">--export=&quot;write</span>
+                  etree&quot;
+                </tt>
+                and
+                <tt class="docutils literal">
+                  <span class="pre">--export=&quot;write&quot;</span>
+                </tt>
+                .  The
+default is:
+                <tt class="docutils literal">
+                  <span class="pre">--export=&quot;write</span>
+                  literal&quot;
+                </tt>
+                .
+              </p>
+            </dd>
+            <dt>q, no-questions</dt>
+            <dd>Do not ask questions.  For example, if the &quot;-f&quot; command line
+option is omitted and the ouput file exists, then generateDS.py
+will not ask whether the file should be overwritten.  (In this
+case, when &quot;-q&quot; is used, the &quot;-f&quot; must be used to force the
+output file to be written.</dd>
             <dt>session=mysession.session</dt>
             <dd>Load and use options from session file. You can create a
 session file in generateds_gui.py, the graphical front-end for
 generateDS.py.  Additional options on the command line can be
 used to override options in the session file.  A session file
 is an XML document, so you can modify it with a text editor.</dd>
             <dt>version</dt>
```

### Comparing `generateDS-2.8b/librarytemplate_howto.txt` & `generateDS-2.9a/librarytemplate_howto.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 :author: Dave Kuhlman
 :address: dkuhlman@rexx.com
     http://www.rexx.com/~dkuhlman
 
 .. version
 
-:revision: 2.8b
+:revision: 2.9a
 
 .. version
 
 :date: |date|
 
 .. |date| date:: %B %d, %Y
```

### Comparing `generateDS-2.8b/librarytemplate-1.0a.zip` & `generateDS-2.9a/librarytemplate-1.0a.zip`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/PKG-INFO` & `generateDS-2.9a/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: generateDS
-Version: 2.8b
+Version: 2.9a
 Summary: Generate Python data structures and XML parser from Xschema
 Home-page: http://www.rexx.com/~dkuhlman/generateDS.html
 Author: Dave Kuhlman
 Author-email: dkuhlman@rexx.com
 License: http://www.opensource.org/licenses/mit-license.php
 Description: generateDS.py generates Python data structures (for example, class
         definitions) from an XML Schema document.  These data structures
```

### Comparing `generateDS-2.8b/generate_coverage.py` & `generateDS-2.9a/generate_coverage.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/libgenerateDS/process_includes.py` & `generateDS-2.9a/libgenerateDS/process_includes.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/setup.py` & `generateDS-2.9a/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 setup(name="generateDS",
 #
 # Do not modify the following VERSION comments.
 # Used by updateversion.py.
 ##VERSION##
-    version="2.8b",
+    version="2.9a",
 ##VERSION##
     author="Dave Kuhlman",
     author_email="dkuhlman@rexx.com",
     maintainer="Dave Kuhlman",
     maintainer_email="dkuhlman@rexx.com",
     url="http://www.rexx.com/~dkuhlman/generateDS.html",
     description="Generate Python data structures and XML parser from Xschema",
```

### Comparing `generateDS-2.8b/generateDS.py` & `generateDS-2.9a/generateDS.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,23 @@
                              Example: --external-encoding='utf-8'.
     --member-specs=list|dict
                              Generate member (type) specifications in each
                              class: a dictionary of instances of class
                              MemberSpec_ containing member name, type,
                              and array or not.  Allowed values are
                              "list" or "dict".  Default: do not generate.
+    --export=<export-list>   Specifies export functions to be generated.
+                             Value is a whitespace separated list of
+                             any of the following:
+                                 write -- write XML to file
+                                 literal -- write out python code
+                                 etree -- build element tree (can serialize
+                                     to XML)
+                             Example: "write etree"
+                             Default: "write"
     -q, --no-questions       Do not ask questions, for example,
                              force overwrite.
     --session=mysession.session
                              Load and use options from session file. You can
                              create session file in generateds_gui.py.  Or,
                              copy and edit sample.session from the
                              distribution.
@@ -151,15 +160,15 @@
 # Global variables etc.
 #
 
 #
 # Do not modify the following VERSION comments.
 # Used by updateversion.py.
 ##VERSION##
-VERSION = '2.8b'
+VERSION = '2.9a'
 ##VERSION##
 
 GenerateProperties = 0
 UseOldGetterSetter = 0
 MemberSpecs = None
 DelayedElements = []
 DelayedElements_subclass = []
@@ -202,14 +211,17 @@
 SimpleTypeDict = {}
 ValidatorBodiesBasePath = None
 UserMethodsPath = None
 UserMethodsModule = None
 XsdNameSpace = ''
 CurrentNamespacePrefix = 'xs:'
 AnyTypeIdentifier = '__ANY__'
+ExportWrite = True
+ExportEtree = False
+ExportLiteral = True
 
 SchemaToPythonTypeMap = {}
 
 # Initialize constants.
 CurrentNamespacePrefix = None
 StringType = None
 TokenType = None
@@ -1075,35 +1087,34 @@
     # We do this recursively because an attribute group can reference
     #   other attribute groups.
     def replace_attributeGroup_names(self):
         for groupName in self.attributeGroupNameList:
             self.replace_attributeGroup_names_1(groupName)
 
     def replace_attributeGroup_names_1(self, groupName):
-            key = None
-            if groupName in AttributeGroups:
-                key = groupName
-            else:
-                # Looking for name space prefix
-                keyList = groupName.split(':')
-                if len(keyList) > 1:
-                    key1 = keyList[1]
-                    if key1 in AttributeGroups:
-                        key = key1
-            if key is not None:
-                attrGroup = AttributeGroups[key]
-                for name in attrGroup.getKeys():
-                    if name in AttributeGroups:
-                        self.replace_attributeGroup_names_1(name)
-                    else:
-                        attr = attrGroup.get(name)
-                        self.attributeDefs[name] = attr
-            else:
-                err_msg('*** Error. attributeGroup %s not defined.\n' % (
-                    groupName, ))
+        key = None
+        if groupName in AttributeGroups:
+            key = groupName
+        else:
+            # Looking for name space prefix
+            key1 = strip_namespace(groupName)
+            if key1 != groupName and key1 in AttributeGroups:
+                key = key1
+        if key is not None:
+            attrGroup = AttributeGroups[key]
+            for name in attrGroup.getKeys():
+                if (name in AttributeGroups or
+                    strip_namespace(name) in AttributeGroups):
+                    self.replace_attributeGroup_names_1(name)
+                else:
+                    attr = attrGroup.get(name)
+                    self.attributeDefs[name] = attr
+        else:
+            err_msg('*** Error. attributeGroup %s not defined.\n' % (
+                groupName, ))
 
     def __str__(self):
         s1 = '<XschemaElement name: "%s" type: "%s">' % \
             (self.getName(), self.getType(), )
         return s1
     __repr__ = __str__
 
@@ -1756,22 +1767,20 @@
                 (fill, name, name, mappedName, name, )
         wrt(s1)
     elif child_type == BooleanType:
         wrt('%s        if self.%s is not None:\n' % (fill, mappedName, ))
         wrt('%s            showIndent(outfile, level, pretty_print)\n' % fill)
         if child.isListType():
             s1 = "%s            outfile.write('<%%s%s>%%s</%%s%s>%%s' %% " \
-                "(namespace_, self.gds_format_boolean_list(self." \
-                "gds_str_lower(str(self.%s)), input_name='%s'), " \
+                "(namespace_, self.gds_format_boolean_list(self.%s, input_name='%s'), " \
                 "namespace_, eol_))\n" % \
                 (fill, name, name, mappedName, name, )
         else:
             s1 = "%s            outfile.write('<%%s%s>%%s</%%s%s>%%s' %% " \
-                "(namespace_, self.gds_format_boolean(self.gds_str_lower" \
-                "(str(self.%s)), input_name='%s'), namespace_, eol_))\n" % \
+                "(namespace_, self.gds_format_boolean(self.%s, input_name='%s'), namespace_, eol_))\n" % \
                 (fill, name, name, mappedName, name, )
         wrt(s1)
     elif child_type == FloatType or \
         child_type == DecimalType:
         wrt('%s        if self.%s is not None:\n' % (fill, mappedName, ))
         wrt('%s            showIndent(outfile, level, pretty_print)\n' % fill)
         if child.isListType():
@@ -1867,22 +1876,20 @@
                 "input_name='%s'), namespace_, eol_))\n" % \
                 (fill, name, name, cleanName, name, )
         wrt(s1)
     elif child_type == BooleanType:
         wrt('%s        showIndent(outfile, level, pretty_print)\n' % fill)
         if child.isListType():
             s1 = "%s        outfile.write('<%%s%s>%%s</%%s%s>%%s' %% " \
-                "(namespace_, self.gds_format_boolean_list(" \
-                "self.gds_str_lower(str(%s_)), input_name='%s'), " \
+                "(namespace_, self.gds_format_boolean_list(%s_, input_name='%s'), " \
                 "namespace_, eol_))\n" % \
                 (fill, name, name, cleanName, name, )
         else:
             s1 = "%s        outfile.write('<%%s%s>%%s</%%s%s>%%s' %% " \
-                "(namespace_, self.gds_format_boolean(" \
-                "self.gds_str_lower(str(%s_)), input_name='%s'), " \
+                "(namespace_, self.gds_format_boolean(%s_, input_name='%s'), " \
                 "namespace_, eol_))\n" % \
                 (fill, name, name, cleanName, name, )
         wrt(s1)
     elif child_type == FloatType or \
         child_type == DecimalType:
         wrt('%s        showIndent(outfile, level, pretty_print)\n' % fill)
         if child.isListType():
@@ -1989,22 +1996,20 @@
                 (fill, name, name, mappedName, name, )
         wrt(s1)
     elif child_type == BooleanType:
         wrt('%s        if self.%s is not None:\n' % (fill, mappedName, ))
         wrt('%s            showIndent(outfile, level, pretty_print)\n' % fill)
         if child.isListType():
             s1 = "%s            outfile.write('<%%s%s>%%s</%%s%s>%%s' %% " \
-                "(namespace_, self.gds_format_boolean_list(" \
-                "self.gds_str_lower(str(self.%s)), input_name='%s'), " \
+                "(namespace_, self.gds_format_boolean_list(self.%s, input_name='%s'), " \
                 "namespace_, eol_))\n" % \
                 (fill, name, name, mappedName, name)
         else:
             s1 = "%s            outfile.write('<%%s%s>%%s</%%s%s>%%s' %% " \
-                "(namespace_, self.gds_format_boolean(" \
-                "self.gds_str_lower(str(self.%s)), input_name='%s'), " \
+                "(namespace_, self.gds_format_boolean(self.%s, input_name='%s'), " \
                 "namespace_, eol_))\n" % \
                 (fill, name, name, mappedName, name)
         wrt(s1)
     elif child_type == FloatType or \
         child_type == DecimalType:
         wrt('%s        if self.%s is not None:\n' % (fill, mappedName, ))
         wrt('%s            showIndent(outfile, level, pretty_print)\n' % fill)
@@ -2051,14 +2056,150 @@
         else:
             s1 = "%s            self.%s.export(outfile, level, namespace_, " \
                 "name_='%s', pretty_print=pretty_print)\n" % \
                 (fill, mappedName, name)
         wrt(s1)
 # end generateExportFn_3
 
+def generateToEtree(wrt, element, Targetnamespace):
+    childCount = countChildren(element, 0)
+    name = element.getName()
+    base = element.getBase()
+    wrt("    def to_etree(self, parent_element=None, name_='%s'):\n" % (name,))
+    parentName, parent = getParentName(element)
+    if parentName and not element.getRestrictionBaseObj():
+        elName = element.getCleanName()
+        wrt("        element = super(%s, self).to_etree("
+            "parent_element, name_)\n" % (elName, ))
+    else:
+        wrt("        if parent_element is None:\n")
+        wrt("            element = etree_.Element('{%s}' + name_)\n" % (
+            Targetnamespace,))
+        wrt("        else:\n")
+        wrt("            element = etree_.SubElement(parent_element, "
+            "'{%s}' + name_)\n" % (Targetnamespace,))
+    if element.getExtended():
+        wrt("        if self.extensiontype_ is not None:\n")
+        wrt("            element.set("
+            "'{http://www.w3.org/2001/XMLSchema-instance}type', "
+            "self.extensiontype_)\n")
+    generateToEtreeAttributes(wrt, element)
+    generateToEtreeChildren(wrt, element, Targetnamespace)
+    wrt("        return element\n")
+# end generateToEtree
+
+def generateToEtreeChildren(wrt, element, Targetnamespace):
+    if len(element.getChildren()) > 0:
+        if element.isMixed():
+            wrt("        for item_ in self.content_:\n")
+            wrt("            item_.to_etree(element)\n")
+        else:
+            for child in element.getChildren():
+                unmappedName = child.getName()
+                name = mapName(cleanupName(child.getName()))
+                type_element = None
+                abstract_child = False
+                type_name = child.getAttrs().get('type')
+                child_type = child.getType()
+                if type_name:
+                    type_element = ElementDict.get(type_name)
+                if type_element and type_element.isAbstract():
+                    abstract_child = True
+                if child_type == AnyTypeIdentifier:
+                    if child.getMaxOccurs() > 1:
+                        wrt('        for obj_ in self.anytypeobjs_:\n')
+                        wrt("            obj_.to_etree(element)\n")
+                    else:
+                        wrt('        if self.anytypeobjs_ is not None:\n')
+                        wrt("            self.anytypeobjs_.to_etree(element)\n")
+                else:
+                    if child.getMaxOccurs() > 1:
+                        wrt("        for %s_ in self.%s:\n" % (name, name,))
+                    else:
+                        wrt("        if self.%s is not None:\n" % (name,))
+                        wrt("            %s_ = self.%s\n" % (name, name,))
+                    if child_type == DateTimeType:
+                        wrt("            etree_.SubElement("
+                            "element, '{%s}%s').text = self."
+                            "gds_format_datetime(%s_)\n" % (
+                                Targetnamespace, unmappedName, name))
+                    elif child_type == DateType:
+                        wrt("            etree_.SubElement("
+                            "element, '{%s}%s').text = self."
+                            "gds_format_date(%s_)\n" % (
+                                Targetnamespace, unmappedName, name))
+                    elif (child_type in StringType or
+                        child_type == TokenType or
+                        child_type in DateTimeGroupType):
+                        wrt("            etree_.SubElement(element, '{%s}%s').text = self.gds_format_string(%s_)\n" % (Targetnamespace, unmappedName, name))
+                    elif child_type in IntegerType or \
+                            child_type == PositiveIntegerType or \
+                            child_type == NonPositiveIntegerType or \
+                            child_type == NegativeIntegerType or \
+                            child_type == NonNegativeIntegerType:
+                        if child.isListType():
+                            wrt("            etree_.SubElement(element, '{%s}%s').text = self.gds_format_integer_list(%s_)\n" % (Targetnamespace, unmappedName, name))
+                        else:
+                            wrt("            etree_.SubElement(element, '{%s}%s').text = self.gds_format_integer(%s_)\n" % (Targetnamespace, unmappedName, name))
+                    elif child_type == BooleanType:
+                        if child.isListType():
+                            wrt("            etree_.SubElement(element, '{%s}%s').text = self.gds_format_boolean_list(%s_)\n" % (Targetnamespace, unmappedName, name))
+                        else:
+                            wrt("            etree_.SubElement(element, '{%s}%s').text = self.gds_format_boolean(%s_)\n" % (Targetnamespace, unmappedName, name))
+                    elif child_type == FloatType or \
+                            child_type == DecimalType:
+                        if child.isListType():
+                            wrt("            etree_.SubElement(element, '{%s}%s').text = self.gds_format_float_list(%s_)\n" % (Targetnamespace, unmappedName, name))
+                        else:
+                            wrt("            etree_.SubElement(element, '{%s}%s').text = self.gds_format_float(%s_)\n" % (Targetnamespace, unmappedName, name))
+                    elif child_type == DoubleType:
+                        if child.isListType():
+                            wrt("            etree_.SubElement(element, '{%s}%s').text = self.gds_format_double_list(%s_)\n" % (Targetnamespace, unmappedName, name))
+                        else:
+                            wrt("            etree_.SubElement(element, '{%s}%s').text = self.gds_format_double(%s_)\n" % (Targetnamespace, unmappedName, name))
+                    elif child_type == Base64Type:
+                        wrt("            etree_.SubElement(element, '{%s}%s').text = self.gds_format_base64(%s_)\n" % (Targetnamespace, unmappedName, name))
+                    else:
+                        wrt("            %s_.to_etree(element, name_='%s')\n" % (
+                            name, unmappedName,))
+#end generateToEtreeChildren
+
+def generateToEtreeAttributes(wrt, element):
+    attrDefs = element.getAttributeDefs()
+    for key in attrDefs.keys():
+        attrDef = attrDefs[key]
+        name = attrDef.getName()
+        cleanName = mapName(cleanupName(name))
+        wrt("        if self.%s is not None:\n" % (cleanName, ))
+        if (attrDef.getType() in StringType or
+            attrDef.getType() in IDTypes or
+            attrDef.getType() == TokenType or
+            attrDef.getType() == TimeType):
+            s1 = '''            element.set('%s', self.gds_format_string(self.%s))\n''' % (name, cleanName, )
+        elif attrDef.getType() in IntegerType or \
+                attrDef.getType() == PositiveIntegerType or \
+                attrDef.getType() == NonPositiveIntegerType or \
+                attrDef.getType() == NegativeIntegerType or \
+                attrDef.getType() == NonNegativeIntegerType:
+            s1 = '''            element.set('%s', self.gds_format_integer(self.%s))\n''' % (name, cleanName, )
+        elif attrDef.getType() == BooleanType:
+            s1 = '''            element.set('%s', self.gds_format_boolean(self.%s))\n''' % (name, cleanName, )
+        elif attrDef.getType() == FloatType or \
+                attrDef.getType() == DecimalType:
+            s1 = '''            element.set('%s', self.gds_format_float(self.%s))\n''' % (name, cleanName, )
+        elif attrDef.getType() == DoubleType:
+            s1 = '''            element.set('%s', self.gds_format_double(self.%s))\n''' % (name, cleanName, )
+        elif attrDef.getType() == DateTimeType:
+            s1 = '''            element.set('%s', self.gds_format_datetime(self.%s))\n''' % (name, cleanName, )
+        elif attrDef.getType() == DateType:
+            s1 = '''            element.set('%s', self.gds_format_date(self.%s))\n''' % (name, cleanName, )
+        else:
+            s1 = '''            element.set('%s', self.%s)\n''' % (name, cleanName, )
+        wrt(s1)
+# end generateToEtreeAttributes
 
 def generateExportAttributes(wrt, element, hasAttributes):
     if len(element.getAttributeDefs()) > 0:
         hasAttributes += 1
         attrDefs = element.getAttributeDefs()
         for key in attrDefs.keys():
             attrDef = attrDefs[key]
@@ -2067,15 +2208,15 @@
             if orig_name is None:
                 orig_name = name
             cleanName = mapName(cleanupName(name))
             if True:            # attrDef.getUse() == 'optional':
                 wrt("        if self.%s is not None and '%s' not in "
                     "already_processed:\n" % (
                     cleanName, cleanName, ))
-                wrt("            already_processed.append('%s')\n" % (
+                wrt("            already_processed.add('%s')\n" % (
                     cleanName, ))
                 indent = "    "
             else:
                 indent = ""
             attrDefType = attrDef.getType()
             if attrDef.getType() == DateTimeType:
                 s1 = '''%s        outfile.write(' %s="%%s"' %% ''' \
@@ -2102,16 +2243,15 @@
                 attrDefType == NonNegativeIntegerType):
                 s1 = '''%s        outfile.write(' %s="%%s"' %% ''' \
                     '''self.gds_format_integer(self.%s, ''' \
                     '''input_name='%s'))\n''' % (
                     indent, orig_name, cleanName, name, )
             elif attrDefType == BooleanType:
                 s1 = '''%s        outfile.write(' %s="%%s"' %% ''' \
-                    '''self.gds_format_boolean(self.gds_str_lower(''' \
-                    '''str(self.%s)), input_name='%s'))\n''' % (
+                    '''self.gds_format_boolean(self.%s, input_name='%s'))\n''' % (
                     indent, orig_name, cleanName, name, )
             elif attrDefType == FloatType or attrDefType == DecimalType:
                 s1 = '''%s        outfile.write(' %s="%%s"' %% self.''' \
                         '''gds_format_float(self.%s, input_name='%s'))\n''' % (
                     indent, orig_name, cleanName, name)
             elif attrDefType == DoubleType:
                 s1 = '''%s        outfile.write(' %s="%%s"' %% ''' \
@@ -2122,15 +2262,15 @@
                 s1 = '''%s        outfile.write(' %s=%%s' %% ''' \
                     '''(quote_attrib(self.%s), ))\n''' % (
                     indent, orig_name, cleanName, )
             wrt(s1)
     if element.getExtended():
         wrt("        if self.extensiontype_ is not None and 'xsi:type' "
             "not in already_processed:\n")
-        wrt("            already_processed.append('xsi:type')\n")
+        wrt("            already_processed.add('xsi:type')\n")
         wrt("            outfile.write("
             "' xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"')\n")
         wrt('''            outfile.write('''
             '''' xsi:type="%s"' % self.extensiontype_)\n''')
     return hasAttributes
 # end generateExportAttributes
 
@@ -2233,15 +2373,15 @@
     wrt('        if pretty_print:\n')
     wrt("            eol_ = '\\n'\n")
     wrt('        else:\n')
     wrt("            eol_ = ''\n")
     wrt('        showIndent(outfile, level, pretty_print)\n')
     wrt("        outfile.write('<%s%s%s' % (namespace_, name_, "
         "namespacedef_ and ' ' + namespacedef_ or '', ))\n")
-    wrt("        already_processed = []\n")
+    wrt("        already_processed = set()\n")
     wrt("        self.exportAttributes(outfile, level, "
         "already_processed, namespace_, name_='%s')\n" %
         (name, ))
     # fix_abstract
     if base and base in ElementDict:
         base_element = ElementDict[base]
         # fix_derived
@@ -2282,34 +2422,34 @@
             xsinamespaceprefix = 'xsi'
             xsinamespace1 = 'http://www.w3.org/2001/XMLSchema-instance'
             xsinamespace2 = '{%s}' % (xsinamespace1, )
             if name.startswith(xsinamespace2):
                 name1 = name[len(xsinamespace2):]
                 name2 = '%s:%s' % (xsinamespaceprefix, name1, )
                 if name2 not in already_processed:
-                    already_processed.append(name2)
+                    already_processed.add(name2)
                     outfile.write(' %s=%s' % (name2, quote_attrib(value), ))
             else:
                 mo = re_.match(Namespace_extract_pat_, name)
                 if mo is not None:
                     namespace, name = mo.group(1, 2)
                     if name not in already_processed:
-                        already_processed.append(name)
+                        already_processed.add(name)
                         if namespace == 'http://www.w3.org/XML/1998/namespace':
                             outfile.write(' %s=%s' % (
                                 name, quote_attrib(value), ))
                         else:
                             unique_counter += 1
                             outfile.write(' xmlns:yyy%d=\"%s\"' % (
                                 unique_counter, namespace, ))
                             outfile.write(' yyy%d:%s=%s' % (
                                 unique_counter, name, quote_attrib(value), ))
                 else:
                     if name not in already_processed:
-                        already_processed.append(name)
+                        already_processed.add(name)
                         outfile.write(' %s=%s' % (
                             name, quote_attrib(value), ))\n""")
     parentName, parent = getParentName(element)
     if parentName:
         hasAttributes += 1
         elName = element.getCleanName()
         wrt("        super(%s, self).exportAttributes("
@@ -2330,16 +2470,14 @@
         elName = element.getCleanName()
         wrt("        super(%s, self).exportChildren(outfile, level, "
             "namespace_, name_, True, pretty_print=pretty_print)\n" %
             (elName, ))
     hasChildren += generateExportChildren(wrt, element, hasChildren, namespace)
     if childCount == 0:   # and not element.isMixed():
         wrt("        pass\n")
-    if True or hasChildren > 0 or element.isMixed():
-        generateHascontentMethod(wrt, element)
 # end generateExportFn
 
 
 #
 # Generate exportLiteral method.
 #
 
@@ -2477,15 +2615,17 @@
 # end generateExportLiteralFn_2
 
 
 def generateExportLiteralFn(wrt, prefix, element):
     wrt("    def exportLiteral(self, outfile, level, name_='%s'):\n" % (
         element.getName(), ))
     wrt("        level += 1\n")
-    wrt("        self.exportLiteralAttributes(outfile, level, [], name_)\n")
+    wrt("        already_processed = set()\n")
+    wrt("        self.exportLiteralAttributes(outfile, level, "
+        "already_processed, name_)\n")
     wrt("        if self.hasContent_():\n")
     wrt("            self.exportLiteralChildren(outfile, level, name_)\n")
     childCount = countChildren(element, 0)
     if element.getSimpleContent() or element.isMixed():
         wrt("        showIndent(outfile, level)\n")
         wrt("        outfile.write('valueOf_ = \"\"\"%s\"\"\",\\n' % "
             "(self.valueOf_,))\n")
@@ -2503,15 +2643,15 @@
         if attrType in SimpleTypeDict:
             attrType = SimpleTypeDict[attrType].getBase()
         if attrType in SimpleTypeDict:
             attrType = SimpleTypeDict[attrType].getBase()
         wrt("        if self.%s is not None and '%s' not in "
             "already_processed:\n" % (
             mappedName, mappedName, ))
-        wrt("            already_processed.append('%s')\n" % (
+        wrt("            already_processed.add('%s')\n" % (
             mappedName, ))
         if (attrType in StringType or
             attrType in IDTypes or
             attrType == TokenType or
             attrType in DateTimeGroupType or
             attrType == NCNameType):
             wrt("            showIndent(outfile, level)\n")
@@ -2635,30 +2775,30 @@
             atype = SimpleTypeDict[atype].getBase()
         if atype == DateTimeType:
             wrt("        value = find_attr_value_('%s', node)\n" % (
                 orig_name, ))
             wrt("        if value is not None and '%s' not in "
                 "already_processed:\n" %
                 (name, ))
-            wrt("            already_processed.append('%s')\n" % (name, ))
+            wrt("            already_processed.add('%s')\n" % (name, ))
             wrt('            try:\n')
             wrt("                self.%s = self.gds_parse_datetime("
                 "value, node, '%s')\n" %
                 (mappedName, name, ))
             wrt('            except ValueError, exp:\n')
             wrt("                raise ValueError("
                 "'Bad date-time attribute (%s): %%s' %% exp)\n" %
                 (name, ))
         elif atype == DateType:
             wrt("        value = find_attr_value_('%s', node)\n" % (
                 orig_name, ))
             wrt("        if value is not None and '%s' not in "
                 "already_processed:\n" %
                 (name, ))
-            wrt("            already_processed.append('%s')\n" % (name, ))
+            wrt("            already_processed.add('%s')\n" % (name, ))
             wrt('            try:\n')
             wrt("                self.%s = self.gds_parse_date("
                 "value, node, '%s')\n" %
                 (mappedName, name, ))
             wrt('            except ValueError, exp:\n')
             wrt("                raise ValueError("
                 "'Bad date attribute (%s): %%s' %% exp)\n" %
@@ -2669,15 +2809,15 @@
             atype == NegativeIntegerType or
             atype == NonNegativeIntegerType):
             wrt("        value = find_attr_value_('%s', node)\n" % (
                 orig_name, ))
             wrt("        if value is not None and '%s' not in "
                 "already_processed:\n" %
                 (name, ))
-            wrt("            already_processed.append('%s')\n" % (name, ))
+            wrt("            already_processed.add('%s')\n" % (name, ))
             wrt('            try:\n')
             wrt("                self.%s = int(value)\n" % (mappedName, ))
             wrt('            except ValueError, exp:\n')
             wrt("                raise_parse_error("
                 "node, 'Bad integer attribute: %s' % exp)\n")
             if atype == PositiveIntegerType:
                 wrt('            if self.%s <= 0:\n' % mappedName)
@@ -2697,54 +2837,54 @@
                     "node, 'Invalid NonNegativeInteger')\n")
         elif atype == BooleanType:
             wrt("        value = find_attr_value_('%s', node)\n" % (
                 orig_name, ))
             wrt("        if value is not None and '%s' not in "
                 "already_processed:\n" %
                 (name, ))
-            wrt("            already_processed.append('%s')\n" % (name, ))
+            wrt("            already_processed.add('%s')\n" % (name, ))
             wrt("            if value in ('true', '1'):\n")
             wrt("                self.%s = True\n" % mappedName)
             wrt("            elif value in ('false', '0'):\n")
             wrt("                self.%s = False\n" % mappedName)
             wrt('            else:\n')
             wrt("                raise_parse_error("
                 "node, 'Bad boolean attribute')\n")
         elif atype == FloatType or atype == DoubleType or atype == DecimalType:
             wrt("        value = find_attr_value_('%s', node)\n" % (
                 orig_name, ))
             wrt("        if value is not None and '%s' not in "
                 "already_processed:\n" %
                 (name, ))
-            wrt("            already_processed.append('%s')\n" % (name, ))
+            wrt("            already_processed.add('%s')\n" % (name, ))
             wrt('            try:\n')
             wrt("                self.%s = float(value)\n" %
                 (mappedName, ))
             wrt('            except ValueError, exp:\n')
             wrt("                raise ValueError('Bad float/double "
                 "attribute (%s): %%s' %% exp)\n" %
                 (name, ))
         elif atype == TokenType:
             wrt("        value = find_attr_value_('%s', node)\n" % (
                 orig_name, ))
             wrt("        if value is not None and '%s' not in "
                 "already_processed:\n" %
                 (name, ))
-            wrt("            already_processed.append('%s')\n" % (name, ))
+            wrt("            already_processed.add('%s')\n" % (name, ))
             wrt("            self.%s = value\n" % (mappedName, ))
             wrt("            self.%s = ' '.join(self.%s.split())\n" %
                 (mappedName, mappedName, ))
         else:
             # Assume attr['type'] in StringType or attr['type'] == DateTimeType
             wrt("        value = find_attr_value_('%s', node)\n" % (
                 orig_name, ))
             wrt("        if value is not None and '%s' not in "
                 "already_processed:\n" %
                 (name, ))
-            wrt("            already_processed.append('%s')\n" % (name, ))
+            wrt("            already_processed.add('%s')\n" % (name, ))
             wrt("            self.%s = value\n" % (mappedName, ))
         typeName = attrDef.getType()
         if typeName and typeName in SimpleTypeDict:
             wrt("            self.validate_%s(self.%s)    "
                 "# validate type %s\n" %
                 (typeName, mappedName, typeName, ))
     if element.getAnyAttribute():
@@ -2754,15 +2894,15 @@
         wrt("            if name not in already_processed:\n")
         wrt('                self.anyAttributes_[name] = value\n')
     if element.getExtended():
         hasAttributes += 1
         wrt("        value = find_attr_value_('xsi:type', node)\n")
         wrt("        if value is not None and 'xsi:type' not in "
             "already_processed:\n")
-        wrt("            already_processed.append('xsi:type')\n")
+        wrt("            already_processed.add('xsi:type')\n")
         wrt("            self.extensiontype_ = value\n")
     return hasAttributes
 # end generateBuildAttributes
 
 
 def generateBuildMixed_1(wrt, prefix, child, headChild, keyword, delayed):
     origName = child.getName()
@@ -3214,15 +3354,16 @@
     return hasChildren
 # end generateBuildStandard
 
 
 def generateBuildFn(wrt, prefix, element, delayed):
     base = element.getBase()
     wrt('    def build(self, node):\n')
-    wrt('        self.buildAttributes(node, node.attrib, [])\n')
+    wrt('        already_processed = set()\n')
+    wrt('        self.buildAttributes(node, node.attrib, already_processed)\n')
     if element.isMixed() or element.getSimpleContent():
         wrt("        self.valueOf_ = get_all_text_(node)\n")
     if element.isMixed():
         wrt("        if node.text is not None:\n")
         wrt("            obj_ = self.mixedclass_("
                 "MixedContainer.CategoryText,\n")
         wrt("                MixedContainer.TypeNone, '', node.text)\n")
@@ -3820,16 +3961,21 @@
     wrt('            return %s%s(*args_, **kwargs_)\n' % (prefix, name))
     wrt('    factory = staticmethod(factory)\n')
     generateGettersAndSetters(wrt, element)
     if Targetnamespace in NamespacesDict:
         namespace = NamespacesDict[Targetnamespace]
     else:
         namespace = ''
-    generateExportFn(wrt, prefix, element, namespace)
-    generateExportLiteralFn(wrt, prefix, element)
+    generateHascontentMethod(wrt, element)
+    if ExportWrite:
+        generateExportFn(wrt, prefix, element, namespace)
+    if ExportEtree:
+        generateToEtree(wrt, element, Targetnamespace)
+    if ExportLiteral:
+        generateExportLiteralFn(wrt, prefix, element)
     generateBuildFn(wrt, prefix, element, delayed)
     generateUserMethods(wrt, element)
     wrt('# end class %s\n' % name)
     wrt('\n\n')
 # end generateClasses
 
 
@@ -3970,15 +4116,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%%s' %% input_data
+            return ('%%s' %% input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%%s' %% input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -4263,14 +4409,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%%s>%%g</%%s>' %%
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%%s>%%s</%%s>' %%
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%%s' %% self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%%d' %% self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%%f' %% self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%%g' %% self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%%s' %% base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%%d, %%d, "%%s", "%%s"),\\n'
                 %% (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -4362,14 +4541,33 @@
 #silence#    sys.stdout.write('<?xml version="1.0" ?>\\n')
 #silence#    rootObj.export(sys.stdout, 0, name_=rootTag,
 #silence#        namespacedef_='%(namespacedef)s',
 #silence#        pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = '%(name)s'
+        rootClass = %(prefix)s%(root)s
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+#silence#    content = etree_.tostring(rootElement, pretty_print=True,
+#silence#        xml_declaration=True, encoding="utf-8")
+#silence#    sys.stdout.write(content)
+#silence#    sys.stdout.write('\\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = '%(name)s'
@@ -4759,18 +4957,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 #silence#    sys.stdout.write('<?xml version="1.0" ?>\\n')
 #silence#    rootObj.export(sys.stdout, 0, name_=rootTag,
 #silence#        namespacedef_='%(namespacedef)s',
 #silence#        pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = '%(name)s'
+        rootClass = supermod.%(root)s
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+#silence#    content = etree_.tostring(rootElement, pretty_print=True,
+#silence#        xml_declaration=True, encoding="utf-8")
+#silence#    sys.stdout.write(content)
+#silence#    sys.stdout.write('\\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = '%(name)s'
@@ -5273,27 +5489,28 @@
 
 def main():
     global Force, GenerateProperties, SubclassSuffix, RootElement, \
         ValidatorBodiesBasePath, UseOldGetterSetter, \
         UserMethodsPath, XsdNameSpace, \
         Namespacedef, NoDates, NoVersion, \
         TEMPLATE_MAIN, TEMPLATE_SUBCLASS_FOOTER, Dirpath, \
-        ExternalEncoding, MemberSpecs, NoQuestions
+        ExternalEncoding, MemberSpecs, NoQuestions, \
+        ExportWrite, ExportEtree, ExportLiteral
     outputText = True
     args = sys.argv[1:]
     try:
         options, args = getopt.getopt(args, 'hfyo:s:p:a:b:mu:q',
             ['help', 'subclass-suffix=',
             'root-element=', 'super=',
             'validator-bodies=', 'use-old-getter-setter',
             'user-methods=', 'no-process-includes', 'silence',
             'namespacedef=', 'external-encoding=',
             'member-specs=', 'no-dates', 'no-versions',
             'no-questions', 'session=',
-            'version',
+            'version', 'export=',
             ])
     except getopt.GetoptError:
         usage()
     prefix = ''
     outFilename = None
     subclassFilename = None
     behaviorFilename = None
@@ -5413,14 +5630,25 @@
         elif option[0] == '--version':
             showVersion = True
         elif option[0] == '--member-specs':
             MemberSpecs = option[1]
             if MemberSpecs not in ('list', 'dict', ):
                 raise RuntimeError(
                     'Option --member-specs must be "list" or "dict".')
+        elif option[0] == '--export':
+            ExportWrite = False
+            ExportEtree = False
+            ExportLiteral = False
+            tmpoptions = option[1].split()
+            if 'write' in tmpoptions:
+                ExportWrite = True
+            if 'etree' in tmpoptions:
+                ExportEtree = True
+            if 'literal' in tmpoptions:
+                ExportLiteral = True
     if showVersion:
         print 'generateDS.py version %s' % VERSION
         sys.exit(0)
     XsdNameSpace = nameSpace
     Namespacedef = namespacedef
     set_type_constants(nameSpace)
     if behaviorFilename and not subclassFilename:
```

### Comparing `generateDS-2.8b/tutorial/generateds_tutorial.txt` & `generateDS-2.9a/tutorial/generateds_tutorial.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     http://www.rexx.com/~dkuhlman
 
 .. Do not modify the following version comments.
    They are used by updateversion.py.
 
 .. version
 
-:revision: 2.8b
+:revision: 2.9a
 
 .. version
 
 :date: |date|
 
 .. |date| date:: %B %d, %Y
```

### Comparing `generateDS-2.8b/tutorial/generateds_tutorial.html` & `generateDS-2.9a/tutorial/generateds_tutorial.html`

 * *Files 0% similar despite different names*

#### Comparing `generateDS-2.8b/tutorial/generateds_tutorial.html` & `generateDS-2.9a/tutorial/generateds_tutorial.html`

```diff
@@ -217,26 +217,26 @@
       <!-- version -->
       <table class="docutils field-list" frame="void" rules="none">
         <col class="field-name"/>
         <col class="field-body"/>
         <tbody valign="top">
           <tr class="field">
             <th class="field-name">revision:</th>
-            <td class="field-body">2.8b</td>
+            <td class="field-body">2.9a</td>
           </tr>
         </tbody>
       </table>
       <!-- version -->
       <table class="docutils field-list" frame="void" rules="none">
         <col class="field-name"/>
         <col class="field-body"/>
         <tbody valign="top">
           <tr class="field">
             <th class="field-name">date:</th>
-            <td class="field-body">January 28, 2013</td>
+            <td class="field-body">February 20, 2013</td>
           </tr>
         </tbody>
       </table>
       <table class="docutils field-list" frame="void" rules="none">
         <col class="field-name"/>
         <col class="field-body"/>
         <tbody valign="top">
```

### Comparing `generateDS-2.8b/tutorial/Code/people_api.py` & `generateDS-2.9a/tutorial/Code/people_api.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tutorial/Code/people.xsd` & `generateDS-2.9a/Demos/People/people.xsd`

 * *Files 12% similar despite different names*

#### Comparing `generateDS-2.8b/tutorial/Code/people.xsd` & `generateDS-2.9a/Demos/People/people.xsd`

```diff
@@ -38,14 +38,15 @@
     </xs:annotation>
   </xs:element>
   <xs:complexType name="personType" mixed="0">
     <xs:sequence>
       <xs:element name="name" type="xs:string"/>
       <xs:element name="interest" type="xs:string" maxOccurs="unbounded"/>
       <xs:element name="category" type="xs:integer"/>
+      <xs:element name="hot.agent" type="hot.agent"/>
       <xs:element name="agent" type="agentType" maxOccurs="unbounded"/>
       <xs:element name="promoter" type="boosterType" maxOccurs="unbounded"/>
       <xs:element name="description" type="xs:string"/>
       <xs:element name="range" type="RangeType"/>
     </xs:sequence>
     <xs:attribute name="value" type="xs:ID"/>
     <xs:attribute name="id" type="xs:integer"/>
@@ -81,14 +82,16 @@
                     -->
           <xs:element name="email" type="xs:string"/>
           <xs:element name="elposint" type="xs:positiveInteger"/>
           <xs:element name="elnonposint" type="xs:nonPositiveInteger"/>
           <xs:element name="elnegint" type="xs:negativeInteger"/>
           <xs:element name="elnonnegint" type="xs:nonNegativeInteger"/>
           <xs:element name="eldate" type="xs:date"/>
+          <xs:element name="eldatetime" type="xs:dateTime"/>
+          <xs:element name="eldatetime1" type="xs:dateTime"/>
           <xs:element name="eltoken" type="xs:token"/>
           <xs:element name="elshort" type="xs:short"/>
           <xs:element name="ellong" type="xs:long"/>
           <xs:element name="elparam" type="paramType"/>
           <xs:element name="elarraytypes" type="ArrayTypes"/>
         </xs:sequence>
         <xs:attribute name="language" type="xs:string"/>
@@ -140,16 +143,19 @@
   </xs:element>
   <xs:complexType mixed="0" name="python-programmerType">
     <xs:complexContent>
       <xs:extension base="programmerType">
         <xs:sequence>
           <xs:element name="favorite-editor" type="xs:string"/>
           <xs:element name="flowvalue" type="FlowType"/>
+          <xs:element name="drcs" type="xs:string"/>
         </xs:sequence>
         <xs:attribute name="nick-name"/>
+        <xs:attribute name="drcs" type="xs:string"/>
+        <xs:attribute name="gui_developer" type="xs:boolean"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:element name="java-programmer" type="java-programmerType">
     <xs:annotation>
       <xs:documentation>A Java programmer type of person.  Programmers are very special
           and Java programmers are nice also, but not as especially wonderful
@@ -157,14 +163,19 @@
     </xs:annotation>
   </xs:element>
   <xs:complexType mixed="0" name="java-programmerType">
     <xs:complexContent>
       <xs:extension base="programmerType">
         <xs:sequence>
           <xs:element name="favorite-editor" type="xs:string"/>
+          <xs:element name="datetime1" type="xs:gYear"/>
+          <xs:element name="datetime2" type="xs:gYearMonth"/>
+          <xs:element name="datetime3" type="xs:gMonth"/>
+          <xs:element name="datetime4" type="xs:gMonthDay"/>
+          <xs:element name="datetime5" type="xs:gDay"/>
         </xs:sequence>
         <xs:attribute name="nick-name"/>
         <xs:attribute name="status"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:element name="agent" type="agentType"/>
@@ -265,8 +276,17 @@
       <xs:extension base="vehicleType">
         <xs:sequence>
           <xs:element name="pilotname" type="xs:string"/>
         </xs:sequence>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
+  <xs:complexType name="hot.agent">
+    <xs:sequence>
+      <xs:element name="firstname" type="xs:string" default="empty\name"/>
+      <xs:element name="lastname" type="xs:string" default="no 'last' name"/>
+      <xs:element name="priority" type="xs:float"/>
+      <xs:element name="startDate" type="xs:date"/>
+    </xs:sequence>
+    <xs:anyAttribute namespace="##other" processContents="lax"/>
+  </xs:complexType>
 </xs:schema>
```

### Comparing `generateDS-2.8b/tutorial/Code/upcase_names.py` & `generateDS-2.9a/tutorial/Code/upcase_names.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tutorial/Code/member_specs_api.py` & `generateDS-2.9a/tutorial/Code/member_specs_api.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tutorial/Code/member_specs_test.py` & `generateDS-2.9a/tutorial/Code/member_specs_test.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tutorial/Code/member_specs.xsd` & `generateDS-2.9a/tutorial/Code/member_specs.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tutorial/Code/people.xml` & `generateDS-2.9a/tutorial/Code/people.xml`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tutorial/Code/member_specs_upper.py` & `generateDS-2.9a/tutorial/Code/member_specs_upper.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tutorial/Code/upcase_names_appl.py` & `generateDS-2.9a/tutorial/Code/upcase_names_appl.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tutorial/Code/people_appl1.py` & `generateDS-2.9a/tutorial/Code/people_appl1.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tutorial/generateds_tutoriala.txt` & `generateDS-2.9a/tutorial/generateds_tutoriala.txt`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tutorial/generateds_tutorial.zip` & `generateDS-2.9a/tutorial/generateds_tutorial.zip`

 * *Files 19% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 48724 bytes, number of entries: 14
--rw-r--r--  3.0 unx     1278 tx defN 13-Jan-17 16:24 generateds_tutorial.txt
--rw-r--r--  3.0 unx    50837 tx defN 13-Jan-28 23:38 generateds_tutorial.html
+Zip file size: 48722 bytes, number of entries: 14
+-rw-r--r--  3.0 unx     1278 tx defN 13-Feb-18 16:34 generateds_tutorial.txt
+-rw-r--r--  3.0 unx    50838 tx defN 13-Feb-21 00:41 generateds_tutorial.html
 drwxr-xr-x  3.0 unx        0 bx stor 11-Oct-01 02:40 Code/
 -rw-r--r--  3.0 unx   137275 tx defN 11-Sep-23 22:04 Code/people_api.py
 -rw-r--r--  3.0 unx      540 tx defN 11-Sep-29 21:14 Code/upcase_names.py
 -rw-r--r--  3.0 unx      345 tx defN 10-Nov-01 17:24 Code/member_specs_data.xml
 -rw-r--r--  3.0 unx    29532 tx defN 11-Sep-30 17:39 Code/member_specs_api.py
 -rw-r--r--  3.0 unx     1097 tx defN 10-Nov-10 03:33 Code/member_specs_test.py
 -rw-r--r--  3.0 unx      940 tx defN 10-Nov-01 17:24 Code/member_specs.xsd
 -rwxr-xr-x  3.0 unx       65 tx defN 10-Nov-01 17:24 Code/member_specs_run
 -rwxr-xr-x  3.0 unx      172 tx defN 11-Sep-30 17:39 Code/member_specs_generate
 -rw-r--r--  3.0 unx     5864 tx defN 11-Sep-30 17:46 Code/member_specs_upper.py
 -rw-r--r--  3.0 unx     9678 tx defN 10-Nov-01 17:24 Code/upcase_names_api.py
 -rw-r--r--  3.0 unx    33677 tx defN 11-Sep-29 21:36 generateds_tutoriala.txt
-14 files, 271300 bytes uncompressed, 46296 bytes compressed:  82.9%
+14 files, 271301 bytes uncompressed, 46294 bytes compressed:  82.9%
```

#### generateds_tutorial.txt

```diff
@@ -7,15 +7,15 @@
     http://www.rexx.com/~dkuhlman
 
 .. Do not modify the following version comments.
    They are used by updateversion.py.
 
 .. version
 
-:revision: 2.8b
+:revision: 2.9a
 
 .. version
 
 :date: |date|
 
 .. |date| date:: %B %d, %Y
```

#### generateds_tutorial.html

##### generateds_tutorial.html

```diff
@@ -217,26 +217,26 @@
       <!-- version -->
       <table class="docutils field-list" frame="void" rules="none">
         <col class="field-name"/>
         <col class="field-body"/>
         <tbody valign="top">
           <tr class="field">
             <th class="field-name">revision:</th>
-            <td class="field-body">2.8b</td>
+            <td class="field-body">2.9a</td>
           </tr>
         </tbody>
       </table>
       <!-- version -->
       <table class="docutils field-list" frame="void" rules="none">
         <col class="field-name"/>
         <col class="field-body"/>
         <tbody valign="top">
           <tr class="field">
             <th class="field-name">date:</th>
-            <td class="field-body">January 28, 2013</td>
+            <td class="field-body">February 20, 2013</td>
           </tr>
         </tbody>
       </table>
       <table class="docutils field-list" frame="void" rules="none">
         <col class="field-name"/>
         <col class="field-body"/>
         <tbody valign="top">
```

### Comparing `generateDS-2.8b/django/gends_run_gen_django.py` & `generateDS-2.9a/django/gends_run_gen_django.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/django/gends_extract_simple_types.py` & `generateDS-2.9a/django/gends_extract_simple_types.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/django/gends_generate_django.py` & `generateDS-2.9a/django/gends_generate_django.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/django/generatedssuper.py` & `generateDS-2.9a/django/generatedssuper.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/README` & `generateDS-2.9a/README`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 minidom module) for XML documents that satisfy the Xschema
 document.  The class definitions contain:
 
 - A constructor with initializers for member variables.
 
 - Get and set methods for member variables.
 
-- A 'build' method used during parsing to populate and instance.
+- A 'build' method used during parsing to populate an instance.
 
-- An 'export' method that will re-create the XML element in an XML
-  document.
+- An 'export' method that will re-create (write out) the XML element
+  in an XML document.
 
 - An 'exportLiteral' method that will write out a text (literal)
   Python data structure that represents the content of the XML
   document.
 
 
 ---------------------------
@@ -137,14 +137,50 @@
 [MIT License -- http://www.opensource.org/licenses/mit-license.php]
 
 
 --------------
 Change history
 --------------
 
+Version 2.9a (02/21/2013)
+- Added support for exporting to an Lxml element tree.  The element
+  tree can then be serialized to XML, e.g. using Lxml
+  etree.tostring().  This innovation is by Logan Owen, who also did
+  most of the work on it (but I helped some, too).  Note that this
+  work is not yet complete; it's still "work in progress"; but it
+  looks very promising.
+- Added --export command line option.  This enables the user to
+  selectively generate export methods for any or all of normal
+  export, export to etree (lxml element tree), or export to literal
+  python code.  This will enable users to reduce bulk in their
+  generated files when any or all of these are not needed.  The
+  default is "write literal", i.e. the normal export methods that we
+  are used to.  Use the --help command line option or read the doc
+  for a description of this option.
+- Fixed a bug that occurs when a schema has an attributeGroup
+  referenced with a name that includes a namespace prefix but the
+  attributeGroup is defined with a name that does *not* have the
+  namespace prefix.  Thanks to Mike Detecca for reporting this and
+  for nudging me in the right direction when I, initially, made the
+  wrong fix.
+- Added unit test for export to etree.
+- Various fixes to the to_etree (export to Lxml element tree)
+  capability: (1) fix to preserve names that contain special
+  characters (e.g. "-" and "."); (2) fix to preserve the type
+  attribute (xsi:type) for abstract types that whose type is set
+  explicitly.  Round turn (XML --> gDS object tree --> lxml element
+  tree --> gDS --> lxml ...) now seems to work reasonably well,
+  although I'm guessing that there are still bits missing (in
+  particular, support for xs:anyAttribute).
+
+Version 2.8c (provisional) (01/30/2013)
+- Changed generated check for attributes that are already_processed
+  to use a set object rather than a list.  Since sets are hashed, I
+  believe that lookup is faster.
+
 Version 2.8b (01/30/2013)
 - Fixed missing underscore in reference to member names in
   generateExportLiteralFn_2.  Thanks to Sergii Chernysh for
   reporting this.
 - Fixed use of NameTable for mapping names when an element has an
   attribute and a child with the same name.  Needed to use correct
   name (original name or mapped name) when doing (1)
```

### Comparing `generateDS-2.8b/librarytemplate_howto.html` & `generateDS-2.9a/librarytemplate_howto.html`

 * *Files 1% similar despite different names*

#### Comparing `generateDS-2.8b/librarytemplate_howto.html` & `generateDS-2.9a/librarytemplate_howto.html`

```diff
@@ -215,26 +215,26 @@
       <!-- version -->
       <table class="docutils field-list" frame="void" rules="none">
         <col class="field-name"/>
         <col class="field-body"/>
         <tbody valign="top">
           <tr class="field">
             <th class="field-name">revision:</th>
-            <td class="field-body">2.8b</td>
+            <td class="field-body">2.9a</td>
           </tr>
         </tbody>
       </table>
       <!-- version -->
       <table class="docutils field-list" frame="void" rules="none">
         <col class="field-name"/>
         <col class="field-body"/>
         <tbody valign="top">
           <tr class="field">
             <th class="field-name">date:</th>
-            <td class="field-body">January 28, 2013</td>
+            <td class="field-body">February 20, 2013</td>
           </tr>
         </tbody>
       </table>
       <div class="section" id="introduction">
         <h1>Introduction</h1>
         <p>This document explains how to use the generateDS.py library
 template to create a package enabling you to distribute a module
```

### Comparing `generateDS-2.8b/generateDS.txt` & `generateDS-2.9a/generateDS.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     http://www.rexx.com/~dkuhlman
 
 .. Do not modify the following version comments.
    They are used by updateversion.py.
 
 .. version
 
-:revision: 2.8b
+:revision: 2.9a
 
 .. version
 
 :date: |date|
 
 .. |date| date:: %B %d, %Y
 
@@ -257,14 +257,26 @@
                                  Example: --external-encoding='utf-8'.
         --member-specs=list|dict
                                  Generate member (type) specifications in each
                                  class: a dictionary of instances of class
                                  MemberSpec_ containing member name, type,
                                  and array or not.  Allowed values are
                                  "list" or "dict".  Default: None.
+        --export=<export-list>   Specifies export functions to be generated.
+                                 Value is a whitespace separated list of
+                                 any of the following:
+                                     write -- write XML to file
+                                     literal -- write out python code
+                                     etree -- build element tree (can serialize
+                                         to XML)
+                                 Examples: --export="write etree"
+                                           --export="write"
+                                 Default: --export="write literal"
+        -q, --no-questions       Do not ask questions, for example,
+                                 force overwrite.
         --session=mysession.session
                                  Load and use options from session file. You can
                                  create session file in generateds_gui.py.
         --version                Print version and exit.        
 
 
 The following command line flags are recognized by ``generateDS.py``:
@@ -418,14 +430,43 @@
     Generate member (type) specifications in each class: a
     dictionary of instances of class ``MemberSpec_`` containing
     member name, type, and array or not.  See `User Methods`_
     section for more information about ``MemberSpec_``.  Allowed
     values are "list" or "dict".  Default: do *not* generate member
     specifications (unless --user-methods specified).
 
+export
+    Specify which of the export related member methods are to be
+    generated.  The value is a whitespace separated list of any of
+    the following:
+
+    - write -- Generate methods ``export``, ``exportAttributes``,
+      and ``exportChildren``.  These methods write XML to a file.
+
+    - literal -- Generate methods ``exportLiteral``,
+      ``exportLiteralAttributes`` and ``exportLiteralChildren``.
+      These methods write out python code.
+
+    - etree -- Generate method ``to_etree``.  This method builds an
+      lxml element tree, which can, for example, be serialized to
+      XML using lxml's ``tostring`` function and searched with the
+      lxml xpath capability.  You can also iterate over nodes in the
+      tree with the node's ``getiterator``, ``iterchildren``, etc,
+      and use any of lxml's other capabilities.
+
+    For example: ``--export="write etree"`` and ``--export="write"``.  The
+    default is: ``--export="write literal"``.
+
+q, no-questions
+    Do not ask questions.  For example, if the "-f" command line
+    option is omitted and the ouput file exists, then generateDS.py
+    will not ask whether the file should be overwritten.  (In this
+    case, when "-q" is used, the "-f" must be used to force the
+    output file to be written.
+
 session=mysession.session
     Load and use options from session file. You can create a
     session file in generateds_gui.py, the graphical front-end for
     generateDS.py.  Additional options on the command line can be
     used to override options in the session file.  A session file
     is an XML document, so you can modify it with a text editor.
```

### Comparing `generateDS-2.8b/tests/simpletype_memberspecs1_sup.py` & `generateDS-2.9a/tests/simpletype_memberspecs1_sup.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -494,67 +527,69 @@
         else:
             return SpecialDate(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_SpecialProperty(self): return self.SpecialProperty
     def set_SpecialProperty(self, SpecialProperty): self.SpecialProperty = SpecialProperty
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='pl:', name_='SpecialDate', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='SpecialDate')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='pl:', name_='SpecialDate'):
         if self.SpecialProperty is not None and 'SpecialProperty' not in already_processed:
-            already_processed.append('SpecialProperty')
+            already_processed.add('SpecialProperty')
             outfile.write(' SpecialProperty=%s' % (self.gds_format_string(quote_attrib(self.SpecialProperty).encode(ExternalEncoding), input_name='SpecialProperty'), ))
     def exportChildren(self, outfile, level, namespace_='pl:', name_='SpecialDate', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='SpecialDate'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.SpecialProperty is not None and 'SpecialProperty' not in already_processed:
-            already_processed.append('SpecialProperty')
+            already_processed.add('SpecialProperty')
             showIndent(outfile, level)
             outfile.write('SpecialProperty = "%s",\n' % (self.SpecialProperty,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('SpecialProperty', node)
         if value is not None and 'SpecialProperty' not in already_processed:
-            already_processed.append('SpecialProperty')
+            already_processed.add('SpecialProperty')
             self.SpecialProperty = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class SpecialDate
 
 
 class ExtremeDate(GeneratedsSuper):
@@ -573,67 +608,69 @@
         else:
             return ExtremeDate(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ExtremeProperty(self): return self.ExtremeProperty
     def set_ExtremeProperty(self, ExtremeProperty): self.ExtremeProperty = ExtremeProperty
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='pl:', name_='ExtremeDate', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='ExtremeDate')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='pl:', name_='ExtremeDate'):
         if self.ExtremeProperty is not None and 'ExtremeProperty' not in already_processed:
-            already_processed.append('ExtremeProperty')
+            already_processed.add('ExtremeProperty')
             outfile.write(' ExtremeProperty=%s' % (self.gds_format_string(quote_attrib(self.ExtremeProperty).encode(ExternalEncoding), input_name='ExtremeProperty'), ))
     def exportChildren(self, outfile, level, namespace_='pl:', name_='ExtremeDate', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='ExtremeDate'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.ExtremeProperty is not None and 'ExtremeProperty' not in already_processed:
-            already_processed.append('ExtremeProperty')
+            already_processed.add('ExtremeProperty')
             showIndent(outfile, level)
             outfile.write('ExtremeProperty = "%s",\n' % (self.ExtremeProperty,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('ExtremeProperty', node)
         if value is not None and 'ExtremeProperty' not in already_processed:
-            already_processed.append('ExtremeProperty')
+            already_processed.add('ExtremeProperty')
             self.ExtremeProperty = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class ExtremeDate
 
 
 GDSClassesMapping = {
@@ -671,14 +708,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'SpecialDate'
+        rootClass = SpecialDate
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'SpecialDate'
```

### Comparing `generateDS-2.8b/tests/anysimpletype1_sub.py` & `generateDS-2.9a/tests/anysimpletype1_sub.py`

 * *Files 7% similar despite different names*

```diff
@@ -106,18 +106,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'test1element'
+        rootClass = supermod.test1element
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'test1element'
```

### Comparing `generateDS-2.8b/tests/ipo2_out.xml` & `generateDS-2.9a/tests/ipo2_out.xml`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/ipo.xml` & `generateDS-2.9a/tests/ipo.xml`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/abstract_type1_sup.py` & `generateDS-2.9a/tests/abstract_type1_sup.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -495,22 +528,29 @@
         else:
             return carrierType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_fleet(self): return self.fleet
     def set_fleet(self, fleet): self.fleet = fleet
     def add_fleet(self, value): self.fleet.append(value)
     def insert_fleet(self, index, value): self.fleet[index] = value
+    def hasContent_(self):
+        if (
+            self.fleet
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='target:', name_='carrierType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='carrierType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -520,24 +560,18 @@
     def exportChildren(self, outfile, level, namespace_='target:', name_='carrierType', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for fleet_ in self.get_fleet():
             fleet_.export(outfile, level, namespace_, name_='fleet', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.fleet
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='carrierType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('fleet=[\n')
@@ -548,15 +582,16 @@
             fleet_.exportLiteral(outfile, level, name_='Vehicle')
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'fleet':
@@ -591,62 +626,64 @@
         if Vehicle.subclass:
             return Vehicle.subclass(*args_, **kwargs_)
         else:
             return Vehicle(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='target:', name_='Vehicle', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='Vehicle')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='target:', name_='Vehicle'):
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
         pass
     def exportChildren(self, outfile, level, namespace_='target:', name_='Vehicle', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='Vehicle'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class Vehicle
 
 
 class Car(Vehicle):
@@ -659,53 +696,55 @@
         pass
     def factory(*args_, **kwargs_):
         if Car.subclass:
             return Car.subclass(*args_, **kwargs_)
         else:
             return Car(*args_, **kwargs_)
     factory = staticmethod(factory)
+    def hasContent_(self):
+        if (
+            super(Car, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='target:', name_='Car', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='Car')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='target:', name_='Car'):
         super(Car, self).exportAttributes(outfile, level, already_processed, namespace_, name_='Car')
     def exportChildren(self, outfile, level, namespace_='target:', name_='Car', fromsubclass_=False, pretty_print=True):
         super(Car, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         pass
-    def hasContent_(self):
-        if (
-            super(Car, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='Car'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(Car, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(Car, self).exportLiteralChildren(outfile, level, name_)
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(Car, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         super(Car, self).buildChildren(child_, node, nodeName_, True)
@@ -723,53 +762,55 @@
         pass
     def factory(*args_, **kwargs_):
         if Plane.subclass:
             return Plane.subclass(*args_, **kwargs_)
         else:
             return Plane(*args_, **kwargs_)
     factory = staticmethod(factory)
+    def hasContent_(self):
+        if (
+            super(Plane, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='target:', name_='Plane', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='Plane')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='target:', name_='Plane'):
         super(Plane, self).exportAttributes(outfile, level, already_processed, namespace_, name_='Plane')
     def exportChildren(self, outfile, level, namespace_='target:', name_='Plane', fromsubclass_=False, pretty_print=True):
         super(Plane, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         pass
-    def hasContent_(self):
-        if (
-            super(Plane, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='Plane'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(Plane, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(Plane, self).exportLiteralChildren(outfile, level, name_)
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(Plane, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         super(Plane, self).buildChildren(child_, node, nodeName_, True)
@@ -814,14 +855,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'carrier'
+        rootClass = carrierType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'carrier'
```

### Comparing `generateDS-2.8b/tests/recursive_simpletype2_sup.py` & `generateDS-2.9a/tests/recursive_simpletype2_sup.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -498,22 +531,31 @@
     factory = staticmethod(factory)
     def get_personId(self): return self.personId
     def set_personId(self, personId): self.personId = personId
     def get_fname(self): return self.fname
     def set_fname(self, fname): self.fname = fname
     def get_lname(self): return self.lname
     def set_lname(self, lname): self.lname = lname
+    def hasContent_(self):
+        if (
+            self.personId is not None or
+            self.fname is not None or
+            self.lname is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='PersonType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='PersonType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -530,26 +572,18 @@
             outfile.write('<%spersonId>%s</%spersonId>%s' % (namespace_, self.gds_format_integer(self.personId, input_name='personId'), namespace_, eol_))
         if self.fname is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfname>%s</%sfname>%s' % (namespace_, self.gds_format_string(quote_xml(self.fname).encode(ExternalEncoding), input_name='fname'), namespace_, eol_))
         if self.lname is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%slname>%s</%slname>%s' % (namespace_, self.gds_format_string(quote_xml(self.lname).encode(ExternalEncoding), input_name='lname'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.personId is not None or
-            self.fname is not None or
-            self.lname is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='PersonType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.personId is not None:
             showIndent(outfile, level)
@@ -557,15 +591,16 @@
         if self.fname is not None:
             showIndent(outfile, level)
             outfile.write('fname=%s,\n' % quote_python(self.fname).encode(ExternalEncoding))
         if self.lname is not None:
             showIndent(outfile, level)
             outfile.write('lname=%s,\n' % quote_python(self.lname).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'personId':
@@ -623,14 +658,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'person'
+        rootClass = PersonType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'person'
```

### Comparing `generateDS-2.8b/tests/simpletype_memberspecs1_sub.py` & `generateDS-2.9a/tests/simpletype_memberspecs1_sub.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,18 +106,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'SpecialDate'
+        rootClass = supermod.SpecialDate
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'SpecialDate'
```

### Comparing `generateDS-2.8b/tests/anywildcard1_sub.py` & `generateDS-2.9a/tests/anywildcard1_sub.py`

 * *Files 16% similar despite different names*

```diff
@@ -134,18 +134,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'PlantType_single'
+        rootClass = supermod.PlantType_single
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'PlantType_single'
```

### Comparing `generateDS-2.8b/tests/recursive_simpletype.xsd` & `generateDS-2.9a/tests/recursive_simpletype.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/annotations1_sub.py` & `generateDS-2.9a/tests/annotations1_sub.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,18 +113,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'document1'
+        rootClass = supermod.document1Type
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'document1'
```

### Comparing `generateDS-2.8b/tests/attr_groups2_sup.py` & `generateDS-2.9a/tests/attr_groups2_sup.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -522,161 +555,163 @@
     def set_value01(self, value01): self.value01 = value01
     def get_value02(self): return self.value02
     def set_value02(self, value02): self.value02 = value02
     def get_value03(self): return self.value03
     def set_value03(self, value03): self.value03 = value03
     def get_sequence(self): return self.sequence
     def set_sequence(self, sequence): self.sequence = sequence
+    def hasContent_(self):
+        if (
+            self.returnedTags is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='GetUserReq', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='GetUserReq')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='GetUserReq'):
         if self.value04 is not None and 'value04' not in already_processed:
-            already_processed.append('value04')
+            already_processed.add('value04')
             outfile.write(' value04="%s"' % self.gds_format_integer(self.value04, input_name='value04'))
         if self.value05 is not None and 'value05' not in already_processed:
-            already_processed.append('value05')
+            already_processed.add('value05')
             outfile.write(' value05=%s' % (self.gds_format_string(quote_attrib(self.value05).encode(ExternalEncoding), input_name='value05'), ))
         if self.value06 is not None and 'value06' not in already_processed:
-            already_processed.append('value06')
+            already_processed.add('value06')
             outfile.write(' value06="%s"' % self.gds_format_integer(self.value06, input_name='value06'))
         if self.value07 is not None and 'value07' not in already_processed:
-            already_processed.append('value07')
+            already_processed.add('value07')
             outfile.write(' value07="%s"' % self.gds_format_integer(self.value07, input_name='value07'))
         if self.value01 is not None and 'value01' not in already_processed:
-            already_processed.append('value01')
+            already_processed.add('value01')
             outfile.write(' value01=%s' % (self.gds_format_string(quote_attrib(self.value01).encode(ExternalEncoding), input_name='value01'), ))
         if self.value02 is not None and 'value02' not in already_processed:
-            already_processed.append('value02')
+            already_processed.add('value02')
             outfile.write(' value02="%s"' % self.gds_format_integer(self.value02, input_name='value02'))
         if self.value03 is not None and 'value03' not in already_processed:
-            already_processed.append('value03')
+            already_processed.add('value03')
             outfile.write(' value03=%s' % (self.gds_format_string(quote_attrib(self.value03).encode(ExternalEncoding), input_name='value03'), ))
         if self.sequence is not None and 'sequence' not in already_processed:
-            already_processed.append('sequence')
+            already_processed.add('sequence')
             outfile.write(' sequence="%s"' % self.gds_format_integer(self.sequence, input_name='sequence'))
     def exportChildren(self, outfile, level, namespace_='', name_='GetUserReq', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.returnedTags is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sreturnedTags>%s</%sreturnedTags>%s' % (namespace_, self.gds_format_string(quote_xml(self.returnedTags).encode(ExternalEncoding), input_name='returnedTags'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.returnedTags is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='GetUserReq'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.value04 is not None and 'value04' not in already_processed:
-            already_processed.append('value04')
+            already_processed.add('value04')
             showIndent(outfile, level)
             outfile.write('value04 = %d,\n' % (self.value04,))
         if self.value05 is not None and 'value05' not in already_processed:
-            already_processed.append('value05')
+            already_processed.add('value05')
             showIndent(outfile, level)
             outfile.write('value05 = "%s",\n' % (self.value05,))
         if self.value06 is not None and 'value06' not in already_processed:
-            already_processed.append('value06')
+            already_processed.add('value06')
             showIndent(outfile, level)
             outfile.write('value06 = %d,\n' % (self.value06,))
         if self.value07 is not None and 'value07' not in already_processed:
-            already_processed.append('value07')
+            already_processed.add('value07')
             showIndent(outfile, level)
             outfile.write('value07 = %d,\n' % (self.value07,))
         if self.value01 is not None and 'value01' not in already_processed:
-            already_processed.append('value01')
+            already_processed.add('value01')
             showIndent(outfile, level)
             outfile.write('value01 = "%s",\n' % (self.value01,))
         if self.value02 is not None and 'value02' not in already_processed:
-            already_processed.append('value02')
+            already_processed.add('value02')
             showIndent(outfile, level)
             outfile.write('value02 = %d,\n' % (self.value02,))
         if self.value03 is not None and 'value03' not in already_processed:
-            already_processed.append('value03')
+            already_processed.add('value03')
             showIndent(outfile, level)
             outfile.write('value03 = "%s",\n' % (self.value03,))
         if self.sequence is not None and 'sequence' not in already_processed:
-            already_processed.append('sequence')
+            already_processed.add('sequence')
             showIndent(outfile, level)
             outfile.write('sequence = %d,\n' % (self.sequence,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.returnedTags is not None:
             showIndent(outfile, level)
             outfile.write('returnedTags=%s,\n' % quote_python(self.returnedTags).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('value04', node)
         if value is not None and 'value04' not in already_processed:
-            already_processed.append('value04')
+            already_processed.add('value04')
             try:
                 self.value04 = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('value05', node)
         if value is not None and 'value05' not in already_processed:
-            already_processed.append('value05')
+            already_processed.add('value05')
             self.value05 = value
         value = find_attr_value_('value06', node)
         if value is not None and 'value06' not in already_processed:
-            already_processed.append('value06')
+            already_processed.add('value06')
             try:
                 self.value06 = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('value07', node)
         if value is not None and 'value07' not in already_processed:
-            already_processed.append('value07')
+            already_processed.add('value07')
             try:
                 self.value07 = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('value01', node)
         if value is not None and 'value01' not in already_processed:
-            already_processed.append('value01')
+            already_processed.add('value01')
             self.value01 = value
         value = find_attr_value_('value02', node)
         if value is not None and 'value02' not in already_processed:
-            already_processed.append('value02')
+            already_processed.add('value02')
             try:
                 self.value02 = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('value03', node)
         if value is not None and 'value03' not in already_processed:
-            already_processed.append('value03')
+            already_processed.add('value03')
             self.value03 = value
         value = find_attr_value_('sequence', node)
         if value is not None and 'sequence' not in already_processed:
-            already_processed.append('sequence')
+            already_processed.add('sequence')
             try:
                 self.sequence = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'returnedTags':
             returnedTags_ = child_.text
@@ -721,14 +756,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'getUser'
+        rootClass = GetUserReq
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'getUser'
```

### Comparing `generateDS-2.8b/tests/attr_groups1_sub.py` & `generateDS-2.9a/tests/attr_groups1_sub.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,18 +99,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'getUser'
+        rootClass = supermod.GetUserReq
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'getUser'
```

### Comparing `generateDS-2.8b/tests/out2_sup.py` & `generateDS-2.9a/tests/out2_sup.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -531,22 +564,33 @@
     def set_python_programmer(self, python_programmer): self.python_programmer = python_programmer
     def add_python_programmer(self, value): self.python_programmer.append(value)
     def insert_python_programmer(self, index, value): self.python_programmer[index] = value
     def get_java_programmer(self): return self.java_programmer
     def set_java_programmer(self, java_programmer): self.java_programmer = java_programmer
     def add_java_programmer(self, value): self.java_programmer.append(value)
     def insert_java_programmer(self, index, value): self.java_programmer[index] = value
+    def hasContent_(self):
+        if (
+            self.comments or
+            self.person or
+            self.programmer or
+            self.python_programmer or
+            self.java_programmer
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='people', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='people')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -564,28 +608,18 @@
             person_.export(outfile, level, namespace_, name_='person', pretty_print=pretty_print)
         for programmer_ in self.programmer:
             programmer_.export(outfile, level, namespace_, name_='programmer', pretty_print=pretty_print)
         for python_programmer_ in self.python_programmer:
             python_programmer_.export(outfile, level, namespace_, name_='python-programmer', pretty_print=pretty_print)
         for java_programmer_ in self.java_programmer:
             java_programmer_.export(outfile, level, namespace_, name_='java-programmer', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.comments or
-            self.person or
-            self.programmer or
-            self.python_programmer or
-            self.java_programmer
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='people'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('comments=[\n')
@@ -644,15 +678,16 @@
             java_programmer_.exportLiteral(outfile, level, name_='java-programmer')
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'comments':
@@ -761,47 +796,48 @@
     factory = staticmethod(factory)
     def get_emp(self): return self.emp
     def set_emp(self, emp): self.emp = emp
     def add_emp(self, value): self.emp.append(value)
     def insert_emp(self, index, value): self.emp[index] = value
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.emp or
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='comments', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='comments')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='comments'):
         pass
     def exportChildren(self, outfile, level, namespace_='', name_='comments', fromsubclass_=False, pretty_print=True):
         if not fromsubclass_:
             for item_ in self.content_:
                 item_.export(outfile, level, item_.name, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.emp or
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='comments'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
@@ -809,15 +845,16 @@
         outfile.write('content_ = [\n')
         for item_ in self.content_:
             item_.exportLiteral(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('],\n')
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         if node.text is not None:
             obj_ = self.mixedclass_(MixedContainer.CategoryText,
                 MixedContainer.TypeNone, '', node.text)
             self.content_.append(obj_)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
@@ -953,48 +990,60 @@
     def set_ratio(self, ratio): self.ratio = ratio
     def get_id(self): return self.id
     def set_id(self, id): self.id = id
     def get_value(self): return self.value
     def set_value(self, value): self.value = value
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.interest or
+            self.category is not None or
+            self.agent or
+            self.promoter or
+            self.description is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='person', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='person')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='person'):
         if self.vegetable is not None and 'vegetable' not in already_processed:
-            already_processed.append('vegetable')
+            already_processed.add('vegetable')
             outfile.write(' vegetable=%s' % (self.gds_format_string(quote_attrib(self.vegetable).encode(ExternalEncoding), input_name='vegetable'), ))
         if self.fruit is not None and 'fruit' not in already_processed:
-            already_processed.append('fruit')
+            already_processed.add('fruit')
             outfile.write(' fruit=%s' % (self.gds_format_string(quote_attrib(self.fruit).encode(ExternalEncoding), input_name='fruit'), ))
         if self.ratio is not None and 'ratio' not in already_processed:
-            already_processed.append('ratio')
+            already_processed.add('ratio')
             outfile.write(' ratio="%s"' % self.gds_format_float(self.ratio, input_name='ratio'))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             outfile.write(' id="%s"' % self.gds_format_integer(self.id, input_name='id'))
         if self.value is not None and 'value' not in already_processed:
-            already_processed.append('value')
+            already_processed.add('value')
             outfile.write(' value=%s' % (self.gds_format_string(quote_attrib(self.value).encode(ExternalEncoding), input_name='value'), ))
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
     def exportChildren(self, outfile, level, namespace_='', name_='person', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
@@ -1010,50 +1059,39 @@
         for agent_ in self.agent:
             agent_.export(outfile, level, namespace_, name_='agent', pretty_print=pretty_print)
         for promoter_ in self.promoter:
             promoter_.export(outfile, level, namespace_, name_='promoter', pretty_print=pretty_print)
         if self.description is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdescription>%s</%sdescription>%s' % (namespace_, self.gds_format_string(quote_xml(self.description).encode(ExternalEncoding), input_name='description'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.interest or
-            self.category is not None or
-            self.agent or
-            self.promoter or
-            self.description is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='person'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.vegetable is not None and 'vegetable' not in already_processed:
-            already_processed.append('vegetable')
+            already_processed.add('vegetable')
             showIndent(outfile, level)
             outfile.write('vegetable = "%s",\n' % (self.vegetable,))
         if self.fruit is not None and 'fruit' not in already_processed:
-            already_processed.append('fruit')
+            already_processed.add('fruit')
             showIndent(outfile, level)
             outfile.write('fruit = "%s",\n' % (self.fruit,))
         if self.ratio is not None and 'ratio' not in already_processed:
-            already_processed.append('ratio')
+            already_processed.add('ratio')
             showIndent(outfile, level)
             outfile.write('ratio = %f,\n' % (self.ratio,))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             showIndent(outfile, level)
             outfile.write('id = %d,\n' % (self.id,))
         if self.value is not None and 'value' not in already_processed:
-            already_processed.append('value')
+            already_processed.add('value')
             showIndent(outfile, level)
             outfile.write('value = "%s",\n' % (self.value,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
             outfile.write('name=%s,\n' % quote_python(self.name).encode(ExternalEncoding))
         showIndent(outfile, level)
@@ -1092,48 +1130,49 @@
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
         if self.description is not None:
             showIndent(outfile, level)
             outfile.write('description=%s,\n' % quote_python(self.description).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('vegetable', node)
         if value is not None and 'vegetable' not in already_processed:
-            already_processed.append('vegetable')
+            already_processed.add('vegetable')
             self.vegetable = value
         value = find_attr_value_('fruit', node)
         if value is not None and 'fruit' not in already_processed:
-            already_processed.append('fruit')
+            already_processed.add('fruit')
             self.fruit = value
         value = find_attr_value_('ratio', node)
         if value is not None and 'ratio' not in already_processed:
-            already_processed.append('ratio')
+            already_processed.add('ratio')
             try:
                 self.ratio = float(value)
             except ValueError, exp:
                 raise ValueError('Bad float/double attribute (ratio): %s' % exp)
         value = find_attr_value_('id', node)
         if value is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             try:
                 self.id = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('value', node)
         if value is not None and 'value' not in already_processed:
-            already_processed.append('value')
+            already_processed.add('value')
             self.value = value
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
             name_ = child_.text
             name_ = self.gds_validate_string(name_, node, 'name')
             self.name = name_
         elif nodeName_ == 'interest':
@@ -1296,52 +1335,71 @@
     def set_attrposint(self, attrposint): self.attrposint = attrposint
     def get_attrnonnegint(self): return self.attrnonnegint
     def set_attrnonnegint(self, attrnonnegint): self.attrnonnegint = attrnonnegint
     def get_attrnonposint(self): return self.attrnonposint
     def set_attrnonposint(self, attrnonposint): self.attrnonposint = attrnonposint
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.email is not None or
+            self.elposint is not None or
+            self.elnonposint is not None or
+            self.elnegint is not None or
+            self.elnonnegint is not None or
+            self.eldate is not None or
+            self.eldatetime is not None or
+            self.eltoken is not None or
+            self.elshort is not None or
+            self.ellong is not None or
+            self.elparam is not None or
+            self.elarraytypes is not None or
+            super(programmer, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='programmer', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='programmer')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='programmer'):
         super(programmer, self).exportAttributes(outfile, level, already_processed, namespace_, name_='programmer')
         if self.language is not None and 'language' not in already_processed:
-            already_processed.append('language')
+            already_processed.add('language')
             outfile.write(' language=%s' % (self.gds_format_string(quote_attrib(self.language).encode(ExternalEncoding), input_name='language'), ))
         if self.area is not None and 'area' not in already_processed:
-            already_processed.append('area')
+            already_processed.add('area')
             outfile.write(' area=%s' % (self.gds_format_string(quote_attrib(self.area).encode(ExternalEncoding), input_name='area'), ))
         if self.attrnegint is not None and 'attrnegint' not in already_processed:
-            already_processed.append('attrnegint')
+            already_processed.add('attrnegint')
             outfile.write(' attrnegint="%s"' % self.gds_format_integer(self.attrnegint, input_name='attrnegint'))
         if self.attrposint is not None and 'attrposint' not in already_processed:
-            already_processed.append('attrposint')
+            already_processed.add('attrposint')
             outfile.write(' attrposint="%s"' % self.gds_format_integer(self.attrposint, input_name='attrposint'))
         if self.attrnonnegint is not None and 'attrnonnegint' not in already_processed:
-            already_processed.append('attrnonnegint')
+            already_processed.add('attrnonnegint')
             outfile.write(' attrnonnegint="%s"' % self.gds_format_integer(self.attrnonnegint, input_name='attrnonnegint'))
         if self.attrnonposint is not None and 'attrnonposint' not in already_processed:
-            already_processed.append('attrnonposint')
+            already_processed.add('attrnonposint')
             outfile.write(' attrnonposint="%s"' % self.gds_format_integer(self.attrnonposint, input_name='attrnonposint'))
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
     def exportChildren(self, outfile, level, namespace_='', name_='programmer', fromsubclass_=False, pretty_print=True):
         super(programmer, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
@@ -1377,61 +1435,43 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sellong>%s</%sellong>%s' % (namespace_, self.gds_format_integer(self.ellong, input_name='ellong'), namespace_, eol_))
         if self.elparam is not None:
             self.elparam.export(outfile, level, namespace_, name_='elparam', pretty_print=pretty_print)
         if self.elarraytypes is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%selarraytypes>%s</%selarraytypes>%s' % (namespace_, self.gds_format_string(quote_xml(self.elarraytypes).encode(ExternalEncoding), input_name='elarraytypes'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.email is not None or
-            self.elposint is not None or
-            self.elnonposint is not None or
-            self.elnegint is not None or
-            self.elnonnegint is not None or
-            self.eldate is not None or
-            self.eldatetime is not None or
-            self.eltoken is not None or
-            self.elshort is not None or
-            self.ellong is not None or
-            self.elparam is not None or
-            self.elarraytypes is not None or
-            super(programmer, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='programmer'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.language is not None and 'language' not in already_processed:
-            already_processed.append('language')
+            already_processed.add('language')
             showIndent(outfile, level)
             outfile.write('language = "%s",\n' % (self.language,))
         if self.area is not None and 'area' not in already_processed:
-            already_processed.append('area')
+            already_processed.add('area')
             showIndent(outfile, level)
             outfile.write('area = "%s",\n' % (self.area,))
         if self.attrnegint is not None and 'attrnegint' not in already_processed:
-            already_processed.append('attrnegint')
+            already_processed.add('attrnegint')
             showIndent(outfile, level)
             outfile.write('attrnegint = %d,\n' % (self.attrnegint,))
         if self.attrposint is not None and 'attrposint' not in already_processed:
-            already_processed.append('attrposint')
+            already_processed.add('attrposint')
             showIndent(outfile, level)
             outfile.write('attrposint = %d,\n' % (self.attrposint,))
         if self.attrnonnegint is not None and 'attrnonnegint' not in already_processed:
-            already_processed.append('attrnonnegint')
+            already_processed.add('attrnonnegint')
             showIndent(outfile, level)
             outfile.write('attrnonnegint = %d,\n' % (self.attrnonnegint,))
         if self.attrnonposint is not None and 'attrnonposint' not in already_processed:
-            already_processed.append('attrnonposint')
+            already_processed.add('attrnonposint')
             showIndent(outfile, level)
             outfile.write('attrnonposint = %d,\n' % (self.attrnonposint,))
         super(programmer, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(programmer, self).exportLiteralChildren(outfile, level, name_)
         if self.email is not None:
             showIndent(outfile, level)
@@ -1469,66 +1509,67 @@
             self.elparam.exportLiteral(outfile, level, name_='elparam')
             showIndent(outfile, level)
             outfile.write('),\n')
         if self.elarraytypes is not None:
             showIndent(outfile, level)
             outfile.write('elarraytypes=%s,\n' % quote_python(self.elarraytypes).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('language', node)
         if value is not None and 'language' not in already_processed:
-            already_processed.append('language')
+            already_processed.add('language')
             self.language = value
         value = find_attr_value_('area', node)
         if value is not None and 'area' not in already_processed:
-            already_processed.append('area')
+            already_processed.add('area')
             self.area = value
         value = find_attr_value_('attrnegint', node)
         if value is not None and 'attrnegint' not in already_processed:
-            already_processed.append('attrnegint')
+            already_processed.add('attrnegint')
             try:
                 self.attrnegint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrnegint >= 0:
                 raise_parse_error(node, 'Invalid NegativeInteger')
         value = find_attr_value_('attrposint', node)
         if value is not None and 'attrposint' not in already_processed:
-            already_processed.append('attrposint')
+            already_processed.add('attrposint')
             try:
                 self.attrposint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrposint <= 0:
                 raise_parse_error(node, 'Invalid PositiveInteger')
         value = find_attr_value_('attrnonnegint', node)
         if value is not None and 'attrnonnegint' not in already_processed:
-            already_processed.append('attrnonnegint')
+            already_processed.add('attrnonnegint')
             try:
                 self.attrnonnegint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrnonnegint < 0:
                 raise_parse_error(node, 'Invalid NonNegativeInteger')
         value = find_attr_value_('attrnonposint', node)
         if value is not None and 'attrnonposint' not in already_processed:
-            already_processed.append('attrnonposint')
+            already_processed.add('attrnonposint')
             try:
                 self.attrnonposint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrnonposint > 0:
                 raise_parse_error(node, 'Invalid NonPositiveInteger')
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
         super(programmer, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'email':
             email_ = child_.text
             email_ = self.gds_validate_string(email_, node, 'email')
             self.email = email_
@@ -1698,123 +1739,125 @@
     def set_sid(self, sid): self.sid = sid
     def get_type(self): return self.type_
     def set_type(self, type_): self.type_ = type_
     def get_id(self): return self.id
     def set_id(self, id): self.id = id
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='param', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='param')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='param'):
         if self.semantic is not None and 'semantic' not in already_processed:
-            already_processed.append('semantic')
+            already_processed.add('semantic')
             outfile.write(' semantic=%s' % (self.gds_format_string(quote_attrib(self.semantic).encode(ExternalEncoding), input_name='semantic'), ))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             outfile.write(' name=%s' % (quote_attrib(self.name), ))
         if self.flow is not None and 'flow' not in already_processed:
-            already_processed.append('flow')
+            already_processed.add('flow')
             outfile.write(' flow=%s' % (quote_attrib(self.flow), ))
         if self.sid is not None and 'sid' not in already_processed:
-            already_processed.append('sid')
+            already_processed.add('sid')
             outfile.write(' sid=%s' % (quote_attrib(self.sid), ))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             outfile.write(' type=%s' % (self.gds_format_string(quote_attrib(self.type_).encode(ExternalEncoding), input_name='type'), ))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             outfile.write(' id=%s' % (self.gds_format_string(quote_attrib(self.id).encode(ExternalEncoding), input_name='id'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='param', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='param'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.semantic is not None and 'semantic' not in already_processed:
-            already_processed.append('semantic')
+            already_processed.add('semantic')
             showIndent(outfile, level)
             outfile.write('semantic = "%s",\n' % (self.semantic,))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             showIndent(outfile, level)
             outfile.write('name = "%s",\n' % (self.name,))
         if self.flow is not None and 'flow' not in already_processed:
-            already_processed.append('flow')
+            already_processed.add('flow')
             showIndent(outfile, level)
             outfile.write('flow = %s,\n' % (self.flow,))
         if self.sid is not None and 'sid' not in already_processed:
-            already_processed.append('sid')
+            already_processed.add('sid')
             showIndent(outfile, level)
             outfile.write('sid = "%s",\n' % (self.sid,))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             showIndent(outfile, level)
             outfile.write('type_ = "%s",\n' % (self.type_,))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             showIndent(outfile, level)
             outfile.write('id = "%s",\n' % (self.id,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('semantic', node)
         if value is not None and 'semantic' not in already_processed:
-            already_processed.append('semantic')
+            already_processed.add('semantic')
             self.semantic = value
             self.semantic = ' '.join(self.semantic.split())
         value = find_attr_value_('name', node)
         if value is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             self.name = value
         value = find_attr_value_('flow', node)
         if value is not None and 'flow' not in already_processed:
-            already_processed.append('flow')
+            already_processed.add('flow')
             self.flow = value
         value = find_attr_value_('sid', node)
         if value is not None and 'sid' not in already_processed:
-            already_processed.append('sid')
+            already_processed.add('sid')
             self.sid = value
         value = find_attr_value_('type', node)
         if value is not None and 'type' not in already_processed:
-            already_processed.append('type')
+            already_processed.add('type')
             self.type_ = value
         value = find_attr_value_('id', node)
         if value is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             self.id = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
     def walk_and_update(self):
         members = param._member_data_items
         for member in members:
             obj1 = getattr(self, member.get_name())
@@ -1880,77 +1923,79 @@
         else:
             return python_programmer(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_favorite_editor(self): return self.favorite_editor
     def set_favorite_editor(self, favorite_editor): self.favorite_editor = favorite_editor
     def get_nick_name(self): return self.nick_name
     def set_nick_name(self, nick_name): self.nick_name = nick_name
+    def hasContent_(self):
+        if (
+            self.favorite_editor is not None or
+            super(python_programmer, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='python-programmer', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='python-programmer')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='python-programmer'):
         super(python_programmer, self).exportAttributes(outfile, level, already_processed, namespace_, name_='python-programmer')
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             outfile.write(' nick-name=%s' % (self.gds_format_string(quote_attrib(self.nick_name).encode(ExternalEncoding), input_name='nick-name'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='python-programmer', fromsubclass_=False, pretty_print=True):
         super(python_programmer, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.favorite_editor is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfavorite-editor>%s</%sfavorite-editor>%s' % (namespace_, self.gds_format_string(quote_xml(self.favorite_editor).encode(ExternalEncoding), input_name='favorite-editor'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.favorite_editor is not None or
-            super(python_programmer, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='python-programmer'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             showIndent(outfile, level)
             outfile.write('nick_name = "%s",\n' % (self.nick_name,))
         super(python_programmer, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(python_programmer, self).exportLiteralChildren(outfile, level, name_)
         if self.favorite_editor is not None:
             showIndent(outfile, level)
             outfile.write('favorite_editor=%s,\n' % quote_python(self.favorite_editor).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('nick-name', node)
         if value is not None and 'nick-name' not in already_processed:
-            already_processed.append('nick-name')
+            already_processed.add('nick-name')
             self.nick_name = value
         super(python_programmer, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'favorite-editor':
             favorite_editor_ = child_.text
             favorite_editor_ = self.gds_validate_string(favorite_editor_, node, 'favorite_editor')
             self.favorite_editor = favorite_editor_
@@ -2025,88 +2070,90 @@
     factory = staticmethod(factory)
     def get_favorite_editor(self): return self.favorite_editor
     def set_favorite_editor(self, favorite_editor): self.favorite_editor = favorite_editor
     def get_status(self): return self.status
     def set_status(self, status): self.status = status
     def get_nick_name(self): return self.nick_name
     def set_nick_name(self, nick_name): self.nick_name = nick_name
+    def hasContent_(self):
+        if (
+            self.favorite_editor is not None or
+            super(java_programmer, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='java-programmer', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='java-programmer')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='java-programmer'):
         super(java_programmer, self).exportAttributes(outfile, level, already_processed, namespace_, name_='java-programmer')
         if self.status is not None and 'status' not in already_processed:
-            already_processed.append('status')
+            already_processed.add('status')
             outfile.write(' status=%s' % (self.gds_format_string(quote_attrib(self.status).encode(ExternalEncoding), input_name='status'), ))
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             outfile.write(' nick-name=%s' % (self.gds_format_string(quote_attrib(self.nick_name).encode(ExternalEncoding), input_name='nick-name'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='java-programmer', fromsubclass_=False, pretty_print=True):
         super(java_programmer, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.favorite_editor is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfavorite-editor>%s</%sfavorite-editor>%s' % (namespace_, self.gds_format_string(quote_xml(self.favorite_editor).encode(ExternalEncoding), input_name='favorite-editor'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.favorite_editor is not None or
-            super(java_programmer, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='java-programmer'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.status is not None and 'status' not in already_processed:
-            already_processed.append('status')
+            already_processed.add('status')
             showIndent(outfile, level)
             outfile.write('status = "%s",\n' % (self.status,))
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             showIndent(outfile, level)
             outfile.write('nick_name = "%s",\n' % (self.nick_name,))
         super(java_programmer, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(java_programmer, self).exportLiteralChildren(outfile, level, name_)
         if self.favorite_editor is not None:
             showIndent(outfile, level)
             outfile.write('favorite_editor=%s,\n' % quote_python(self.favorite_editor).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('status', node)
         if value is not None and 'status' not in already_processed:
-            already_processed.append('status')
+            already_processed.add('status')
             self.status = value
         value = find_attr_value_('nick-name', node)
         if value is not None and 'nick-name' not in already_processed:
-            already_processed.append('nick-name')
+            already_processed.add('nick-name')
             self.nick_name = value
         super(java_programmer, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'favorite-editor':
             favorite_editor_ = child_.text
             favorite_editor_ = self.gds_validate_string(favorite_editor_, node, 'favorite_editor')
             self.favorite_editor = favorite_editor_
@@ -2184,22 +2231,32 @@
     def set_firstname(self, firstname): self.firstname = firstname
     def get_lastname(self): return self.lastname
     def set_lastname(self, lastname): self.lastname = lastname
     def get_priority(self): return self.priority
     def set_priority(self, priority): self.priority = priority
     def get_info(self): return self.info
     def set_info(self, info): self.info = info
+    def hasContent_(self):
+        if (
+            self.firstname is not None or
+            self.lastname is not None or
+            self.priority is not None or
+            self.info is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='agent', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='agent')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2218,27 +2275,18 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%slastname>%s</%slastname>%s' % (namespace_, self.gds_format_string(quote_xml(self.lastname).encode(ExternalEncoding), input_name='lastname'), namespace_, eol_))
         if self.priority is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%spriority>%s</%spriority>%s' % (namespace_, self.gds_format_float(self.priority, input_name='priority'), namespace_, eol_))
         if self.info is not None:
             self.info.export(outfile, level, namespace_, name_='info', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.firstname is not None or
-            self.lastname is not None or
-            self.priority is not None or
-            self.info is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='agent'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.firstname is not None:
             showIndent(outfile, level)
@@ -2252,15 +2300,16 @@
         if self.info is not None:
             showIndent(outfile, level)
             outfile.write('info=model_.info(\n')
             self.info.exportLiteral(outfile, level)
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'firstname':
@@ -2356,22 +2405,32 @@
     def set_firstname(self, firstname): self.firstname = firstname
     def get_lastname(self): return self.lastname
     def set_lastname(self, lastname): self.lastname = lastname
     def get_priority(self): return self.priority
     def set_priority(self, priority): self.priority = priority
     def get_info(self): return self.info
     def set_info(self, info): self.info = info
+    def hasContent_(self):
+        if (
+            self.firstname is not None or
+            self.lastname is not None or
+            self.priority is not None or
+            self.info is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='special-agent', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='special-agent')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2390,27 +2449,18 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%slastname>%s</%slastname>%s' % (namespace_, self.gds_format_string(quote_xml(self.lastname).encode(ExternalEncoding), input_name='lastname'), namespace_, eol_))
         if self.priority is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%spriority>%s</%spriority>%s' % (namespace_, self.gds_format_float(self.priority, input_name='priority'), namespace_, eol_))
         if self.info is not None:
             self.info.export(outfile, level, namespace_, name_='info', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.firstname is not None or
-            self.lastname is not None or
-            self.priority is not None or
-            self.info is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='special-agent'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.firstname is not None:
             showIndent(outfile, level)
@@ -2424,15 +2474,16 @@
         if self.info is not None:
             showIndent(outfile, level)
             outfile.write('info=model_.info(\n')
             self.info.exportLiteral(outfile, level)
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'firstname':
@@ -2555,22 +2606,35 @@
     def set_type(self, type_): self.type_ = type_
     def add_type(self, value): self.type_.append(value)
     def insert_type(self, index, value): self.type_[index] = value
     def get_client_handler(self): return self.client_handler
     def set_client_handler(self, client_handler): self.client_handler = client_handler
     def add_client_handler(self, value): self.client_handler.append(value)
     def insert_client_handler(self, index, value): self.client_handler[index] = value
+    def hasContent_(self):
+        if (
+            self.firstname is not None or
+            self.lastname is not None or
+            self.other_name is not None or
+            self.classxx is not None or
+            self.other_value or
+            self.type_ or
+            self.client_handler
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='booster', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='booster')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2598,30 +2662,18 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sother-value>%s</%sother-value>%s' % (namespace_, self.gds_format_float(other_value_, input_name='other-value'), namespace_, eol_))
         for type_ in self.type_:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%stype>%s</%stype>%s' % (namespace_, self.gds_format_float(type_, input_name='type'), namespace_, eol_))
         for client_handler_ in self.client_handler:
             client_handler_.export(outfile, level, namespace_, name_='client-handler', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.firstname is not None or
-            self.lastname is not None or
-            self.other_name is not None or
-            self.classxx is not None or
-            self.other_value or
-            self.type_ or
-            self.client_handler
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='booster'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.firstname is not None:
             showIndent(outfile, level)
@@ -2662,15 +2714,16 @@
             client_handler_.exportLiteral(outfile, level, name_='client-handlerType')
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'firstname':
@@ -2787,91 +2840,93 @@
     factory = staticmethod(factory)
     def get_rating(self): return self.rating
     def set_rating(self, rating): self.rating = rating
     def get_type(self): return self.type_
     def set_type(self, type_): self.type_ = type_
     def get_name(self): return self.name
     def set_name(self, name): self.name = name
+    def hasContent_(self):
+        if (
+
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='info', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='info')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='info'):
         if self.rating is not None and 'rating' not in already_processed:
-            already_processed.append('rating')
+            already_processed.add('rating')
             outfile.write(' rating="%s"' % self.gds_format_float(self.rating, input_name='rating'))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             outfile.write(' type="%s"' % self.gds_format_integer(self.type_, input_name='type'))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             outfile.write(' name=%s' % (self.gds_format_string(quote_attrib(self.name).encode(ExternalEncoding), input_name='name'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='info', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='info'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.rating is not None and 'rating' not in already_processed:
-            already_processed.append('rating')
+            already_processed.add('rating')
             showIndent(outfile, level)
             outfile.write('rating = %f,\n' % (self.rating,))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             showIndent(outfile, level)
             outfile.write('type_ = %d,\n' % (self.type_,))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             showIndent(outfile, level)
             outfile.write('name = "%s",\n' % (self.name,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('rating', node)
         if value is not None and 'rating' not in already_processed:
-            already_processed.append('rating')
+            already_processed.add('rating')
             try:
                 self.rating = float(value)
             except ValueError, exp:
                 raise ValueError('Bad float/double attribute (rating): %s' % exp)
         value = find_attr_value_('type', node)
         if value is not None and 'type' not in already_processed:
-            already_processed.append('type')
+            already_processed.add('type')
             try:
                 self.type_ = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('name', node)
         if value is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             self.name = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
     def walk_and_update(self):
         members = info._member_data_items
         for member in members:
             obj1 = getattr(self, member.get_name())
@@ -2936,22 +2991,30 @@
         else:
             return client_handlerType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_fullname(self): return self.fullname
     def set_fullname(self, fullname): self.fullname = fullname
     def get_refid(self): return self.refid
     def set_refid(self, refid): self.refid = refid
+    def hasContent_(self):
+        if (
+            self.fullname is not None or
+            self.refid is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='client-handlerType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='client-handlerType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2965,38 +3028,32 @@
             eol_ = ''
         if self.fullname is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfullname>%s</%sfullname>%s' % (namespace_, self.gds_format_string(quote_xml(self.fullname).encode(ExternalEncoding), input_name='fullname'), namespace_, eol_))
         if self.refid is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%srefid>%s</%srefid>%s' % (namespace_, self.gds_format_integer(self.refid, input_name='refid'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.fullname is not None or
-            self.refid is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='client-handlerType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.fullname is not None:
             showIndent(outfile, level)
             outfile.write('fullname=%s,\n' % quote_python(self.fullname).encode(ExternalEncoding))
         if self.refid is not None:
             showIndent(outfile, level)
             outfile.write('refid=%d,\n' % self.refid)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'fullname':
@@ -3098,14 +3155,33 @@
     sys.stdout.write('<?xml version="1.0" ?>\n')
     rootObj.export(sys.stdout, 0, name_=rootTag,
         namespacedef_='',
         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'people'
+        rootClass = people
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+    content = etree_.tostring(rootElement, pretty_print=True,
+        xml_declaration=True, encoding="utf-8")
+    sys.stdout.write(content)
+    sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'people'
```

### Comparing `generateDS-2.8b/tests/recursive_simpletype2_sub.py` & `generateDS-2.9a/tests/recursive_simpletype2_sub.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,18 +99,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'person'
+        rootClass = supermod.PersonType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'person'
```

### Comparing `generateDS-2.8b/tests/simplecontent_restriction1_sup.py` & `generateDS-2.9a/tests/simplecontent_restriction1_sup.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -521,141 +554,143 @@
     def set_schemeVersionID(self, schemeVersionID): self.schemeVersionID = schemeVersionID
     def get_schemeURI(self): return self.schemeURI
     def set_schemeURI(self, schemeURI): self.schemeURI = schemeURI
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='IdentifierType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='IdentifierType')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='IdentifierType'):
         if self.schemeDataURI is not None and 'schemeDataURI' not in already_processed:
-            already_processed.append('schemeDataURI')
+            already_processed.add('schemeDataURI')
             outfile.write(' schemeDataURI=%s' % (self.gds_format_string(quote_attrib(self.schemeDataURI).encode(ExternalEncoding), input_name='schemeDataURI'), ))
         if self.schemeID is not None and 'schemeID' not in already_processed:
-            already_processed.append('schemeID')
+            already_processed.add('schemeID')
             outfile.write(' schemeID=%s' % (self.gds_format_string(quote_attrib(self.schemeID).encode(ExternalEncoding), input_name='schemeID'), ))
         if self.schemeAgencyName is not None and 'schemeAgencyName' not in already_processed:
-            already_processed.append('schemeAgencyName')
+            already_processed.add('schemeAgencyName')
             outfile.write(' schemeAgencyName=%s' % (self.gds_format_string(quote_attrib(self.schemeAgencyName).encode(ExternalEncoding), input_name='schemeAgencyName'), ))
         if self.schemeAgencyID is not None and 'schemeAgencyID' not in already_processed:
-            already_processed.append('schemeAgencyID')
+            already_processed.add('schemeAgencyID')
             outfile.write(' schemeAgencyID=%s' % (self.gds_format_string(quote_attrib(self.schemeAgencyID).encode(ExternalEncoding), input_name='schemeAgencyID'), ))
         if self.schemeName is not None and 'schemeName' not in already_processed:
-            already_processed.append('schemeName')
+            already_processed.add('schemeName')
             outfile.write(' schemeName=%s' % (self.gds_format_string(quote_attrib(self.schemeName).encode(ExternalEncoding), input_name='schemeName'), ))
         if self.schemeVersionID is not None and 'schemeVersionID' not in already_processed:
-            already_processed.append('schemeVersionID')
+            already_processed.add('schemeVersionID')
             outfile.write(' schemeVersionID=%s' % (self.gds_format_string(quote_attrib(self.schemeVersionID).encode(ExternalEncoding), input_name='schemeVersionID'), ))
         if self.schemeURI is not None and 'schemeURI' not in already_processed:
-            already_processed.append('schemeURI')
+            already_processed.add('schemeURI')
             outfile.write(' schemeURI=%s' % (self.gds_format_string(quote_attrib(self.schemeURI).encode(ExternalEncoding), input_name='schemeURI'), ))
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
     def exportChildren(self, outfile, level, namespace_='', name_='IdentifierType', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='IdentifierType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.schemeDataURI is not None and 'schemeDataURI' not in already_processed:
-            already_processed.append('schemeDataURI')
+            already_processed.add('schemeDataURI')
             showIndent(outfile, level)
             outfile.write('schemeDataURI = "%s",\n' % (self.schemeDataURI,))
         if self.schemeID is not None and 'schemeID' not in already_processed:
-            already_processed.append('schemeID')
+            already_processed.add('schemeID')
             showIndent(outfile, level)
             outfile.write('schemeID = "%s",\n' % (self.schemeID,))
         if self.schemeAgencyName is not None and 'schemeAgencyName' not in already_processed:
-            already_processed.append('schemeAgencyName')
+            already_processed.add('schemeAgencyName')
             showIndent(outfile, level)
             outfile.write('schemeAgencyName = "%s",\n' % (self.schemeAgencyName,))
         if self.schemeAgencyID is not None and 'schemeAgencyID' not in already_processed:
-            already_processed.append('schemeAgencyID')
+            already_processed.add('schemeAgencyID')
             showIndent(outfile, level)
             outfile.write('schemeAgencyID = "%s",\n' % (self.schemeAgencyID,))
         if self.schemeName is not None and 'schemeName' not in already_processed:
-            already_processed.append('schemeName')
+            already_processed.add('schemeName')
             showIndent(outfile, level)
             outfile.write('schemeName = "%s",\n' % (self.schemeName,))
         if self.schemeVersionID is not None and 'schemeVersionID' not in already_processed:
-            already_processed.append('schemeVersionID')
+            already_processed.add('schemeVersionID')
             showIndent(outfile, level)
             outfile.write('schemeVersionID = "%s",\n' % (self.schemeVersionID,))
         if self.schemeURI is not None and 'schemeURI' not in already_processed:
-            already_processed.append('schemeURI')
+            already_processed.add('schemeURI')
             showIndent(outfile, level)
             outfile.write('schemeURI = "%s",\n' % (self.schemeURI,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('schemeDataURI', node)
         if value is not None and 'schemeDataURI' not in already_processed:
-            already_processed.append('schemeDataURI')
+            already_processed.add('schemeDataURI')
             self.schemeDataURI = value
         value = find_attr_value_('schemeID', node)
         if value is not None and 'schemeID' not in already_processed:
-            already_processed.append('schemeID')
+            already_processed.add('schemeID')
             self.schemeID = value
         value = find_attr_value_('schemeAgencyName', node)
         if value is not None and 'schemeAgencyName' not in already_processed:
-            already_processed.append('schemeAgencyName')
+            already_processed.add('schemeAgencyName')
             self.schemeAgencyName = value
         value = find_attr_value_('schemeAgencyID', node)
         if value is not None and 'schemeAgencyID' not in already_processed:
-            already_processed.append('schemeAgencyID')
+            already_processed.add('schemeAgencyID')
             self.schemeAgencyID = value
         value = find_attr_value_('schemeName', node)
         if value is not None and 'schemeName' not in already_processed:
-            already_processed.append('schemeName')
+            already_processed.add('schemeName')
             self.schemeName = value
         value = find_attr_value_('schemeVersionID', node)
         if value is not None and 'schemeVersionID' not in already_processed:
-            already_processed.append('schemeVersionID')
+            already_processed.add('schemeVersionID')
             self.schemeVersionID = value
         value = find_attr_value_('schemeURI', node)
         if value is not None and 'schemeURI' not in already_processed:
-            already_processed.append('schemeURI')
+            already_processed.add('schemeURI')
             self.schemeURI = value
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class IdentifierType
 
 
 class BillOfResourcesIDType(IdentifierType):
@@ -671,57 +706,59 @@
         if BillOfResourcesIDType.subclass:
             return BillOfResourcesIDType.subclass(*args_, **kwargs_)
         else:
             return BillOfResourcesIDType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_ or
+            super(BillOfResourcesIDType, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='BillOfResourcesIDType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='BillOfResourcesIDType')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='BillOfResourcesIDType'):
         super(BillOfResourcesIDType, self).exportAttributes(outfile, level, already_processed, namespace_, name_='BillOfResourcesIDType')
     def exportChildren(self, outfile, level, namespace_='', name_='BillOfResourcesIDType', fromsubclass_=False, pretty_print=True):
         super(BillOfResourcesIDType, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_ or
-            super(BillOfResourcesIDType, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='BillOfResourcesIDType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(BillOfResourcesIDType, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(BillOfResourcesIDType, self).exportLiteralChildren(outfile, level, name_)
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(BillOfResourcesIDType, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
@@ -742,57 +779,59 @@
         if BillOfMaterialIDType.subclass:
             return BillOfMaterialIDType.subclass(*args_, **kwargs_)
         else:
             return BillOfMaterialIDType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_ or
+            super(BillOfMaterialIDType, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='BillOfMaterialIDType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='BillOfMaterialIDType')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='BillOfMaterialIDType'):
         super(BillOfMaterialIDType, self).exportAttributes(outfile, level, already_processed, namespace_, name_='BillOfMaterialIDType')
     def exportChildren(self, outfile, level, namespace_='', name_='BillOfMaterialIDType', fromsubclass_=False, pretty_print=True):
         super(BillOfMaterialIDType, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_ or
-            super(BillOfMaterialIDType, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='BillOfMaterialIDType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(BillOfMaterialIDType, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(BillOfMaterialIDType, self).exportLiteralChildren(outfile, level, name_)
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(BillOfMaterialIDType, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
@@ -835,14 +874,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'IdentifierType'
+        rootClass = IdentifierType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'IdentifierType'
```

### Comparing `generateDS-2.8b/tests/people.xsd` & `generateDS-2.9a/tests/people.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/recursive_simpletype1_sub.py` & `generateDS-2.9a/tests/recursive_simpletype1_sub.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,18 +99,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'person'
+        rootClass = supermod.PersonType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'person'
```

### Comparing `generateDS-2.8b/tests/simpletypes_other1_sup.py` & `generateDS-2.9a/tests/simpletypes_other1_sup.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -495,22 +528,29 @@
         else:
             return simpleTypeTestsType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_simpleTypeTest(self): return self.simpleTypeTest
     def set_simpleTypeTest(self, simpleTypeTest): self.simpleTypeTest = simpleTypeTest
     def add_simpleTypeTest(self, value): self.simpleTypeTest.append(value)
     def insert_simpleTypeTest(self, index, value): self.simpleTypeTest[index] = value
+    def hasContent_(self):
+        if (
+            self.simpleTypeTest
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='simpleTypeTestsType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='simpleTypeTestsType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -521,24 +561,18 @@
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for simpleTypeTest_ in self.simpleTypeTest:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%ssimpleTypeTest>%s</%ssimpleTypeTest>%s' % (namespace_, self.gds_format_string(quote_xml(simpleTypeTest_).encode(ExternalEncoding), input_name='simpleTypeTest'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.simpleTypeTest
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='simpleTypeTestsType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('simpleTypeTest=[\n')
@@ -546,15 +580,16 @@
         for simpleTypeTest_ in self.simpleTypeTest:
             showIndent(outfile, level)
             outfile.write('%s,\n' % quote_python(simpleTypeTest_).encode(ExternalEncoding))
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'simpleTypeTest':
@@ -696,22 +731,49 @@
     def insert_dateVal2(self, index, value): self.dateVal2[index] = value
     def get_dateTimeVal1(self): return self.dateTimeVal1
     def set_dateTimeVal1(self, dateTimeVal1): self.dateTimeVal1 = dateTimeVal1
     def get_dateTimeVal2(self): return self.dateTimeVal2
     def set_dateTimeVal2(self, dateTimeVal2): self.dateTimeVal2 = dateTimeVal2
     def add_dateTimeVal2(self, value): self.dateTimeVal2.append(value)
     def insert_dateTimeVal2(self, index, value): self.dateTimeVal2[index] = value
+    def hasContent_(self):
+        if (
+            self.datetime1 is not None or
+            self.datetime2 is not None or
+            self.datetime3 is not None or
+            self.datetime4 is not None or
+            self.datetime5 is not None or
+            self.integerVal1 is not None or
+            self.integerVal2 or
+            self.stringVal1 is not None or
+            self.stringVal2 or
+            self.booleanVal1 is not None or
+            self.booleanVal2 or
+            self.decimalVal1 is not None or
+            self.decimalVal2 or
+            self.doubleVal1 is not None or
+            self.doubleVal2 or
+            self.floatVal1 is not None or
+            self.floatVal2 or
+            self.dateVal1 is not None or
+            self.dateVal2 or
+            self.dateTimeVal1 is not None or
+            self.dateTimeVal2
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='simpleTypeTest', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='simpleTypeTest')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -748,18 +810,18 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sstringVal1>%s</%sstringVal1>%s' % (namespace_, self.gds_format_string(quote_xml(self.stringVal1).encode(ExternalEncoding), input_name='stringVal1'), namespace_, eol_))
         for stringVal2_ in self.stringVal2:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sstringVal2>%s</%sstringVal2>%s' % (namespace_, self.gds_format_string(quote_xml(stringVal2_).encode(ExternalEncoding), input_name='stringVal2'), namespace_, eol_))
         if self.booleanVal1 is not None:
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sbooleanVal1>%s</%sbooleanVal1>%s' % (namespace_, self.gds_format_boolean(self.gds_str_lower(str(self.booleanVal1)), input_name='booleanVal1'), namespace_, eol_))
+            outfile.write('<%sbooleanVal1>%s</%sbooleanVal1>%s' % (namespace_, self.gds_format_boolean(self.booleanVal1, input_name='booleanVal1'), namespace_, eol_))
         for booleanVal2_ in self.booleanVal2:
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sbooleanVal2>%s</%sbooleanVal2>%s' % (namespace_, self.gds_format_boolean(self.gds_str_lower(str(booleanVal2_)), input_name='booleanVal2'), namespace_, eol_))
+            outfile.write('<%sbooleanVal2>%s</%sbooleanVal2>%s' % (namespace_, self.gds_format_boolean(booleanVal2_, input_name='booleanVal2'), namespace_, eol_))
         if self.decimalVal1 is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdecimalVal1>%s</%sdecimalVal1>%s' % (namespace_, self.gds_format_float(self.decimalVal1, input_name='decimalVal1'), namespace_, eol_))
         for decimalVal2_ in self.decimalVal2:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdecimalVal2>%s</%sdecimalVal2>%s' % (namespace_, self.gds_format_float(decimalVal2_, input_name='decimalVal2'), namespace_, eol_))
         if self.doubleVal1 is not None:
@@ -782,44 +844,18 @@
             outfile.write('<%sdateVal2>%s</%sdateVal2>%s' % (namespace_, self.gds_format_date(dateVal2_, input_name='dateVal2'), namespace_, eol_))
         if self.dateTimeVal1 is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdateTimeVal1>%s</%sdateTimeVal1>%s' % (namespace_, self.gds_format_datetime(self.dateTimeVal1, input_name='dateTimeVal1'), namespace_, eol_))
         for dateTimeVal2_ in self.dateTimeVal2:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdateTimeVal2>%s</%sdateTimeVal2>%s' % (namespace_, self.gds_format_datetime(dateTimeVal2_, input_name='dateTimeVal2'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.datetime1 is not None or
-            self.datetime2 is not None or
-            self.datetime3 is not None or
-            self.datetime4 is not None or
-            self.datetime5 is not None or
-            self.integerVal1 is not None or
-            self.integerVal2 or
-            self.stringVal1 is not None or
-            self.stringVal2 or
-            self.booleanVal1 is not None or
-            self.booleanVal2 or
-            self.decimalVal1 is not None or
-            self.decimalVal2 or
-            self.doubleVal1 is not None or
-            self.doubleVal2 or
-            self.floatVal1 is not None or
-            self.floatVal2 or
-            self.dateVal1 is not None or
-            self.dateVal2 or
-            self.dateTimeVal1 is not None or
-            self.dateTimeVal2
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='simpleTypeTest'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.datetime1 is not None:
             showIndent(outfile, level)
@@ -929,15 +965,16 @@
         for dateTimeVal2_ in self.dateTimeVal2:
             showIndent(outfile, level)
             outfile.write('%s,\n' % self.gds_format_datetime(dateTimeVal2_, input_name='dateTimeVal2'))
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'datetime1':
@@ -1107,14 +1144,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'simpleTypeTests'
+        rootClass = simpleTypeTestsType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'simpleTypeTests'
```

### Comparing `generateDS-2.8b/tests/annotations1_sup.py` & `generateDS-2.9a/tests/annotations1_sup.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -497,22 +530,30 @@
         else:
             return document1Type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_comments(self): return self.comments
     def set_comments(self, comments): self.comments = comments
     def get_otherdoc(self): return self.otherdoc
     def set_otherdoc(self, otherdoc): self.otherdoc = otherdoc
+    def hasContent_(self):
+        if (
+            self.comments is not None or
+            self.otherdoc is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='document1Type', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='document1Type')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -525,25 +566,18 @@
         else:
             eol_ = ''
         if self.comments is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scomments>%s</%scomments>%s' % (namespace_, self.gds_format_string(quote_xml(self.comments).encode(ExternalEncoding), input_name='comments'), namespace_, eol_))
         if self.otherdoc is not None:
             self.otherdoc.export(outfile, level, namespace_, name_='otherdoc', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.comments is not None or
-            self.otherdoc is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='document1Type'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.comments is not None:
             showIndent(outfile, level)
@@ -551,15 +585,16 @@
         if self.otherdoc is not None:
             showIndent(outfile, level)
             outfile.write('otherdoc=model_.document2Type(\n')
             self.otherdoc.exportLiteral(outfile, level, name_='otherdoc')
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'comments':
@@ -596,22 +631,31 @@
     factory = staticmethod(factory)
     def get_comments(self): return self.comments
     def set_comments(self, comments): self.comments = comments
     def get_rating(self): return self.rating
     def set_rating(self, rating): self.rating = rating
     def get_anotherdoc(self): return self.anotherdoc
     def set_anotherdoc(self, anotherdoc): self.anotherdoc = anotherdoc
+    def hasContent_(self):
+        if (
+            self.comments is not None or
+            self.rating is not None or
+            self.anotherdoc is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='document2Type', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='document2Type')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -627,26 +671,18 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scomments>%s</%scomments>%s' % (namespace_, self.gds_format_string(quote_xml(self.comments).encode(ExternalEncoding), input_name='comments'), namespace_, eol_))
         if self.rating is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%srating>%s</%srating>%s' % (namespace_, self.gds_format_integer(self.rating, input_name='rating'), namespace_, eol_))
         if self.anotherdoc is not None:
             self.anotherdoc.export(outfile, level, namespace_, name_='anotherdoc', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.comments is not None or
-            self.rating is not None or
-            self.anotherdoc is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='document2Type'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.comments is not None:
             showIndent(outfile, level)
@@ -657,15 +693,16 @@
         if self.anotherdoc is not None:
             showIndent(outfile, level)
             outfile.write('anotherdoc=model_.document3Type(\n')
             self.anotherdoc.exportLiteral(outfile, level, name_='anotherdoc')
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'comments':
@@ -704,22 +741,30 @@
         else:
             return document3Type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_comments(self): return self.comments
     def set_comments(self, comments): self.comments = comments
     def get_rating(self): return self.rating
     def set_rating(self, rating): self.rating = rating
+    def hasContent_(self):
+        if (
+            self.comments is not None or
+            self.rating is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='document3Type', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='document3Type')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -733,38 +778,32 @@
             eol_ = ''
         if self.comments is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scomments>%s</%scomments>%s' % (namespace_, self.gds_format_string(quote_xml(self.comments).encode(ExternalEncoding), input_name='comments'), namespace_, eol_))
         if self.rating is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%srating>%s</%srating>%s' % (namespace_, self.gds_format_integer(self.rating, input_name='rating'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.comments is not None or
-            self.rating is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='document3Type'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.comments is not None:
             showIndent(outfile, level)
             outfile.write('comments=%s,\n' % quote_python(self.comments).encode(ExternalEncoding))
         if self.rating is not None:
             showIndent(outfile, level)
             outfile.write('rating=%d,\n' % self.rating)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'comments':
@@ -820,14 +859,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'document1'
+        rootClass = document1Type
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'document1'
```

### Comparing `generateDS-2.8b/tests/ipo1_sub.py` & `generateDS-2.9a/tests/ipo1_sub.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,18 +134,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
     sys.stdout.write('<?xml version="1.0" ?>\n')
     rootObj.export(sys.stdout, 0, name_=rootTag,
         namespacedef_='',
         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'purchaseOrder'
+        rootClass = supermod.PurchaseOrderType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+    content = etree_.tostring(rootElement, pretty_print=True,
+        xml_declaration=True, encoding="utf-8")
+    sys.stdout.write(content)
+    sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'purchaseOrder'
```

### Comparing `generateDS-2.8b/tests/extensions1_sup.py` & `generateDS-2.9a/tests/extensions1_sup.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -494,67 +527,69 @@
         else:
             return SpecialDate(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_SpecialProperty(self): return self.SpecialProperty
     def set_SpecialProperty(self, SpecialProperty): self.SpecialProperty = SpecialProperty
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='SpecialDate', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='SpecialDate')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='SpecialDate'):
         if self.SpecialProperty is not None and 'SpecialProperty' not in already_processed:
-            already_processed.append('SpecialProperty')
+            already_processed.add('SpecialProperty')
             outfile.write(' SpecialProperty=%s' % (self.gds_format_string(quote_attrib(self.SpecialProperty).encode(ExternalEncoding), input_name='SpecialProperty'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='SpecialDate', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='SpecialDate'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.SpecialProperty is not None and 'SpecialProperty' not in already_processed:
-            already_processed.append('SpecialProperty')
+            already_processed.add('SpecialProperty')
             showIndent(outfile, level)
             outfile.write('SpecialProperty = "%s",\n' % (self.SpecialProperty,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('SpecialProperty', node)
         if value is not None and 'SpecialProperty' not in already_processed:
-            already_processed.append('SpecialProperty')
+            already_processed.add('SpecialProperty')
             self.SpecialProperty = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class SpecialDate
 
 
 class ExtremeDate(GeneratedsSuper):
@@ -573,67 +608,69 @@
         else:
             return ExtremeDate(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ExtremeProperty(self): return self.ExtremeProperty
     def set_ExtremeProperty(self, ExtremeProperty): self.ExtremeProperty = ExtremeProperty
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='ExtremeDate', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='ExtremeDate')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='ExtremeDate'):
         if self.ExtremeProperty is not None and 'ExtremeProperty' not in already_processed:
-            already_processed.append('ExtremeProperty')
+            already_processed.add('ExtremeProperty')
             outfile.write(' ExtremeProperty=%s' % (self.gds_format_string(quote_attrib(self.ExtremeProperty).encode(ExternalEncoding), input_name='ExtremeProperty'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='ExtremeDate', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='ExtremeDate'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.ExtremeProperty is not None and 'ExtremeProperty' not in already_processed:
-            already_processed.append('ExtremeProperty')
+            already_processed.add('ExtremeProperty')
             showIndent(outfile, level)
             outfile.write('ExtremeProperty = "%s",\n' % (self.ExtremeProperty,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('ExtremeProperty', node)
         if value is not None and 'ExtremeProperty' not in already_processed:
-            already_processed.append('ExtremeProperty')
+            already_processed.add('ExtremeProperty')
             self.ExtremeProperty = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class ExtremeDate
 
 
 class singleExtremeDate(GeneratedsSuper):
@@ -652,67 +689,69 @@
         else:
             return singleExtremeDate(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ExtremeProperty(self): return self.ExtremeProperty
     def set_ExtremeProperty(self, ExtremeProperty): self.ExtremeProperty = ExtremeProperty
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='singleExtremeDate', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='singleExtremeDate')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='singleExtremeDate'):
         if self.ExtremeProperty is not None and 'ExtremeProperty' not in already_processed:
-            already_processed.append('ExtremeProperty')
+            already_processed.add('ExtremeProperty')
             outfile.write(' ExtremeProperty=%s' % (self.gds_format_string(quote_attrib(self.ExtremeProperty).encode(ExternalEncoding), input_name='ExtremeProperty'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='singleExtremeDate', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='singleExtremeDate'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.ExtremeProperty is not None and 'ExtremeProperty' not in already_processed:
-            already_processed.append('ExtremeProperty')
+            already_processed.add('ExtremeProperty')
             showIndent(outfile, level)
             outfile.write('ExtremeProperty = "%s",\n' % (self.ExtremeProperty,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('ExtremeProperty', node)
         if value is not None and 'ExtremeProperty' not in already_processed:
-            already_processed.append('ExtremeProperty')
+            already_processed.add('ExtremeProperty')
             self.ExtremeProperty = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class singleExtremeDate
 
 
 class containerType(GeneratedsSuper):
@@ -736,22 +775,30 @@
     factory = staticmethod(factory)
     def get_simplefactoid(self): return self.simplefactoid
     def set_simplefactoid(self, simplefactoid): self.simplefactoid = simplefactoid
     def add_simplefactoid(self, value): self.simplefactoid.append(value)
     def insert_simplefactoid(self, index, value): self.simplefactoid[index] = value
     def get_mixedfactoid(self): return self.mixedfactoid
     def set_mixedfactoid(self, mixedfactoid): self.mixedfactoid = mixedfactoid
+    def hasContent_(self):
+        if (
+            self.simplefactoid or
+            self.mixedfactoid is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='containerType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='containerType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -763,25 +810,18 @@
             eol_ = '\n'
         else:
             eol_ = ''
         for simplefactoid_ in self.simplefactoid:
             simplefactoid_.export(outfile, level, namespace_, name_='simplefactoid', pretty_print=pretty_print)
         if self.mixedfactoid is not None:
             self.mixedfactoid.export(outfile, level, namespace_, name_='mixedfactoid', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.simplefactoid or
-            self.mixedfactoid is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='containerType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('simplefactoid=[\n')
@@ -798,15 +838,16 @@
         if self.mixedfactoid is not None:
             showIndent(outfile, level)
             outfile.write('mixedfactoid=model_.mixedFactoidType(\n')
             self.mixedfactoid.exportLiteral(outfile, level, name_='mixedfactoid')
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'simplefactoid':
@@ -835,22 +876,29 @@
             return simpleFactoidType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_relation(self): return self.relation
     def set_relation(self, relation): self.relation = relation
     def validate_RelationType(self, value):
         # Validate type RelationType, a restriction on RelationType2.
         pass
+    def hasContent_(self):
+        if (
+            self.relation is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='simpleFactoidType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='simpleFactoidType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -861,34 +909,29 @@
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.relation is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%srelation>%s</%srelation>%s' % (namespace_, self.gds_format_string(quote_xml(self.relation).encode(ExternalEncoding), input_name='relation'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.relation is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='simpleFactoidType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.relation is not None:
             showIndent(outfile, level)
             outfile.write('relation=%s,\n' % quote_python(self.relation).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'relation':
@@ -927,47 +970,48 @@
     def get_relation(self): return self.relation
     def set_relation(self, relation): self.relation = relation
     def validate_RelationType(self, value):
         # Validate type RelationType, a restriction on RelationType2.
         pass
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.relation is not None or
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='mixedFactoidType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='mixedFactoidType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='mixedFactoidType'):
         pass
     def exportChildren(self, outfile, level, namespace_='', name_='mixedFactoidType', fromsubclass_=False, pretty_print=True):
         if not fromsubclass_:
             for item_ in self.content_:
                 item_.export(outfile, level, item_.name, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.relation is not None or
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='mixedFactoidType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
@@ -975,15 +1019,16 @@
         outfile.write('content_ = [\n')
         for item_ in self.content_:
             item_.exportLiteral(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('],\n')
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         if node.text is not None:
             obj_ = self.mixedclass_(MixedContainer.CategoryText,
                 MixedContainer.TypeNone, '', node.text)
             self.content_.append(obj_)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
@@ -1026,86 +1071,88 @@
     def set_BaseProperty1(self, BaseProperty1): self.BaseProperty1 = BaseProperty1
     def get_BaseProperty2(self): return self.BaseProperty2
     def set_BaseProperty2(self, BaseProperty2): self.BaseProperty2 = BaseProperty2
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='BaseType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='BaseType')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='BaseType'):
         if self.BaseProperty1 is not None and 'BaseProperty1' not in already_processed:
-            already_processed.append('BaseProperty1')
+            already_processed.add('BaseProperty1')
             outfile.write(' BaseProperty1=%s' % (self.gds_format_string(quote_attrib(self.BaseProperty1).encode(ExternalEncoding), input_name='BaseProperty1'), ))
         if self.BaseProperty2 is not None and 'BaseProperty2' not in already_processed:
-            already_processed.append('BaseProperty2')
+            already_processed.add('BaseProperty2')
             outfile.write(' BaseProperty2=%s' % (self.gds_format_string(quote_attrib(self.BaseProperty2).encode(ExternalEncoding), input_name='BaseProperty2'), ))
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
     def exportChildren(self, outfile, level, namespace_='', name_='BaseType', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='BaseType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.BaseProperty1 is not None and 'BaseProperty1' not in already_processed:
-            already_processed.append('BaseProperty1')
+            already_processed.add('BaseProperty1')
             showIndent(outfile, level)
             outfile.write('BaseProperty1 = "%s",\n' % (self.BaseProperty1,))
         if self.BaseProperty2 is not None and 'BaseProperty2' not in already_processed:
-            already_processed.append('BaseProperty2')
+            already_processed.add('BaseProperty2')
             showIndent(outfile, level)
             outfile.write('BaseProperty2 = "%s",\n' % (self.BaseProperty2,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('BaseProperty1', node)
         if value is not None and 'BaseProperty1' not in already_processed:
-            already_processed.append('BaseProperty1')
+            already_processed.add('BaseProperty1')
             self.BaseProperty1 = value
         value = find_attr_value_('BaseProperty2', node)
         if value is not None and 'BaseProperty2' not in already_processed:
-            already_processed.append('BaseProperty2')
+            already_processed.add('BaseProperty2')
             self.BaseProperty2 = value
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class BaseType
 
 
 class DerivedType(BaseType):
@@ -1129,83 +1176,85 @@
     factory = staticmethod(factory)
     def get_DerivedProperty1(self): return self.DerivedProperty1
     def set_DerivedProperty1(self, DerivedProperty1): self.DerivedProperty1 = DerivedProperty1
     def get_DerivedProperty2(self): return self.DerivedProperty2
     def set_DerivedProperty2(self, DerivedProperty2): self.DerivedProperty2 = DerivedProperty2
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_ or
+            super(DerivedType, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='DerivedType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='DerivedType')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='DerivedType'):
         super(DerivedType, self).exportAttributes(outfile, level, already_processed, namespace_, name_='DerivedType')
         if self.DerivedProperty1 is not None and 'DerivedProperty1' not in already_processed:
-            already_processed.append('DerivedProperty1')
+            already_processed.add('DerivedProperty1')
             outfile.write(' DerivedProperty1=%s' % (self.gds_format_string(quote_attrib(self.DerivedProperty1).encode(ExternalEncoding), input_name='DerivedProperty1'), ))
         if self.DerivedProperty2 is not None and 'DerivedProperty2' not in already_processed:
-            already_processed.append('DerivedProperty2')
+            already_processed.add('DerivedProperty2')
             outfile.write(' DerivedProperty2=%s' % (self.gds_format_string(quote_attrib(self.DerivedProperty2).encode(ExternalEncoding), input_name='DerivedProperty2'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='DerivedType', fromsubclass_=False, pretty_print=True):
         super(DerivedType, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_ or
-            super(DerivedType, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='DerivedType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.DerivedProperty1 is not None and 'DerivedProperty1' not in already_processed:
-            already_processed.append('DerivedProperty1')
+            already_processed.add('DerivedProperty1')
             showIndent(outfile, level)
             outfile.write('DerivedProperty1 = "%s",\n' % (self.DerivedProperty1,))
         if self.DerivedProperty2 is not None and 'DerivedProperty2' not in already_processed:
-            already_processed.append('DerivedProperty2')
+            already_processed.add('DerivedProperty2')
             showIndent(outfile, level)
             outfile.write('DerivedProperty2 = "%s",\n' % (self.DerivedProperty2,))
         super(DerivedType, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(DerivedType, self).exportLiteralChildren(outfile, level, name_)
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('DerivedProperty1', node)
         if value is not None and 'DerivedProperty1' not in already_processed:
-            already_processed.append('DerivedProperty1')
+            already_processed.add('DerivedProperty1')
             self.DerivedProperty1 = value
         value = find_attr_value_('DerivedProperty2', node)
         if value is not None and 'DerivedProperty2' not in already_processed:
-            already_processed.append('DerivedProperty2')
+            already_processed.add('DerivedProperty2')
             self.DerivedProperty2 = value
         super(DerivedType, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class DerivedType
 
 
@@ -1225,67 +1274,69 @@
         else:
             return MyInteger(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_MyAttr(self): return self.MyAttr
     def set_MyAttr(self, MyAttr): self.MyAttr = MyAttr
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='MyInteger', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='MyInteger')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='MyInteger'):
         if self.MyAttr is not None and 'MyAttr' not in already_processed:
-            already_processed.append('MyAttr')
+            already_processed.add('MyAttr')
             outfile.write(' MyAttr=%s' % (self.gds_format_string(quote_attrib(self.MyAttr).encode(ExternalEncoding), input_name='MyAttr'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='MyInteger', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='MyInteger'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.MyAttr is not None and 'MyAttr' not in already_processed:
-            already_processed.append('MyAttr')
+            already_processed.add('MyAttr')
             showIndent(outfile, level)
             outfile.write('MyAttr = "%s",\n' % (self.MyAttr,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('MyAttr', node)
         if value is not None and 'MyAttr' not in already_processed:
-            already_processed.append('MyAttr')
+            already_processed.add('MyAttr')
             self.MyAttr = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class MyInteger
 
 
 class MyBoolean(GeneratedsSuper):
@@ -1304,67 +1355,69 @@
         else:
             return MyBoolean(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_MyAttr(self): return self.MyAttr
     def set_MyAttr(self, MyAttr): self.MyAttr = MyAttr
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='MyBoolean', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='MyBoolean')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='MyBoolean'):
         if self.MyAttr is not None and 'MyAttr' not in already_processed:
-            already_processed.append('MyAttr')
+            already_processed.add('MyAttr')
             outfile.write(' MyAttr=%s' % (self.gds_format_string(quote_attrib(self.MyAttr).encode(ExternalEncoding), input_name='MyAttr'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='MyBoolean', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='MyBoolean'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.MyAttr is not None and 'MyAttr' not in already_processed:
-            already_processed.append('MyAttr')
+            already_processed.add('MyAttr')
             showIndent(outfile, level)
             outfile.write('MyAttr = "%s",\n' % (self.MyAttr,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('MyAttr', node)
         if value is not None and 'MyAttr' not in already_processed:
-            already_processed.append('MyAttr')
+            already_processed.add('MyAttr')
             self.MyAttr = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class MyBoolean
 
 
 class MyFloat(GeneratedsSuper):
@@ -1383,67 +1436,69 @@
         else:
             return MyFloat(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_MyAttr(self): return self.MyAttr
     def set_MyAttr(self, MyAttr): self.MyAttr = MyAttr
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='MyFloat', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='MyFloat')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='MyFloat'):
         if self.MyAttr is not None and 'MyAttr' not in already_processed:
-            already_processed.append('MyAttr')
+            already_processed.add('MyAttr')
             outfile.write(' MyAttr=%s' % (self.gds_format_string(quote_attrib(self.MyAttr).encode(ExternalEncoding), input_name='MyAttr'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='MyFloat', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='MyFloat'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.MyAttr is not None and 'MyAttr' not in already_processed:
-            already_processed.append('MyAttr')
+            already_processed.add('MyAttr')
             showIndent(outfile, level)
             outfile.write('MyAttr = "%s",\n' % (self.MyAttr,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('MyAttr', node)
         if value is not None and 'MyAttr' not in already_processed:
-            already_processed.append('MyAttr')
+            already_processed.add('MyAttr')
             self.MyAttr = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class MyFloat
 
 
 class MyDouble(GeneratedsSuper):
@@ -1462,67 +1517,69 @@
         else:
             return MyDouble(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_MyAttr(self): return self.MyAttr
     def set_MyAttr(self, MyAttr): self.MyAttr = MyAttr
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='MyDouble', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='MyDouble')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='MyDouble'):
         if self.MyAttr is not None and 'MyAttr' not in already_processed:
-            already_processed.append('MyAttr')
+            already_processed.add('MyAttr')
             outfile.write(' MyAttr=%s' % (self.gds_format_string(quote_attrib(self.MyAttr).encode(ExternalEncoding), input_name='MyAttr'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='MyDouble', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='MyDouble'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.MyAttr is not None and 'MyAttr' not in already_processed:
-            already_processed.append('MyAttr')
+            already_processed.add('MyAttr')
             showIndent(outfile, level)
             outfile.write('MyAttr = "%s",\n' % (self.MyAttr,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('MyAttr', node)
         if value is not None and 'MyAttr' not in already_processed:
-            already_processed.append('MyAttr')
+            already_processed.add('MyAttr')
             self.MyAttr = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class MyDouble
 
 
 GDSClassesMapping = {
@@ -1563,14 +1620,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'container'
+        rootClass = containerType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'container'
```

### Comparing `generateDS-2.8b/tests/anywildcard2_sup.py` & `generateDS-2.9a/tests/anywildcard2_sup.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -498,22 +531,31 @@
     factory = staticmethod(factory)
     def get_name(self): return self.name
     def set_name(self, name): self.name = name
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def get_description(self): return self.description
     def set_description(self, description): self.description = description
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.anytypeobjs_ is not None or
+            self.description is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='PlantType_single', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='PlantType_single')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -528,26 +570,18 @@
         if self.name is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sname>%s</%sname>%s' % (namespace_, self.gds_format_string(quote_xml(self.name).encode(ExternalEncoding), input_name='name'), namespace_, eol_))
         if self.description is not None:
             self.description.export(outfile, level, namespace_, name_='description', pretty_print=pretty_print)
         if self.anytypeobjs_ is not None:
             self.anytypeobjs_.export(outfile, level, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.anytypeobjs_ is not None or
-            self.description is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='PlantType_single'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
@@ -561,15 +595,16 @@
         if self.description is not None:
             showIndent(outfile, level)
             outfile.write('description=model_.DescriptionType(\n')
             self.description.exportLiteral(outfile, level, name_='description')
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
@@ -612,22 +647,31 @@
     def set_name(self, name): self.name = name
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
     def get_description(self): return self.description
     def set_description(self, description): self.description = description
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.anytypeobjs_ or
+            self.description is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='PlantType_multiple', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='PlantType_multiple')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -642,26 +686,18 @@
         if self.name is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sname>%s</%sname>%s' % (namespace_, self.gds_format_string(quote_xml(self.name).encode(ExternalEncoding), input_name='name'), namespace_, eol_))
         if self.description is not None:
             self.description.export(outfile, level, namespace_, name_='description', pretty_print=pretty_print)
         for obj_ in self.anytypeobjs_:
             obj_.export(outfile, level, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.anytypeobjs_ or
-            self.description is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='PlantType_multiple'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
@@ -677,15 +713,16 @@
         if self.description is not None:
             showIndent(outfile, level)
             outfile.write('description=model_.DescriptionType(\n')
             self.description.exportLiteral(outfile, level, name_='description')
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
@@ -720,22 +757,30 @@
         else:
             return DescriptionType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_name(self): return self.name
     def set_name(self, name): self.name = name
     def get_size(self): return self.size
     def set_size(self, size): self.size = size
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.size is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='DescriptionType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='DescriptionType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -749,38 +794,32 @@
             eol_ = ''
         if self.name is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sname>%s</%sname>%s' % (namespace_, self.gds_format_string(quote_xml(self.name).encode(ExternalEncoding), input_name='name'), namespace_, eol_))
         if self.size is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%ssize>%s</%ssize>%s' % (namespace_, self.gds_format_string(quote_xml(self.size).encode(ExternalEncoding), input_name='size'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.size is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='DescriptionType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
             outfile.write('name=%s,\n' % quote_python(self.name).encode(ExternalEncoding))
         if self.size is not None:
             showIndent(outfile, level)
             outfile.write('size=%s,\n' % quote_python(self.size).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
@@ -811,22 +850,30 @@
         else:
             return CatalogType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_name(self): return self.name
     def set_name(self, name): self.name = name
     def get_catagory(self): return self.catagory
     def set_catagory(self, catagory): self.catagory = catagory
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.catagory is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='CatalogType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='CatalogType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -840,38 +887,32 @@
             eol_ = ''
         if self.name is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sname>%s</%sname>%s' % (namespace_, self.gds_format_string(quote_xml(self.name).encode(ExternalEncoding), input_name='name'), namespace_, eol_))
         if self.catagory is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scatagory>%s</%scatagory>%s' % (namespace_, self.gds_format_integer(self.catagory, input_name='catagory'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.catagory is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='CatalogType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
             outfile.write('name=%s,\n' % quote_python(self.name).encode(ExternalEncoding))
         if self.catagory is not None:
             showIndent(outfile, level)
             outfile.write('catagory=%d,\n' % self.catagory)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
@@ -901,22 +942,29 @@
         if PlantType_single_nochild.subclass:
             return PlantType_single_nochild.subclass(*args_, **kwargs_)
         else:
             return PlantType_single_nochild(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
+    def hasContent_(self):
+        if (
+            self.anytypeobjs_ is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='PlantType_single_nochild', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='PlantType_single_nochild')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -926,37 +974,32 @@
     def exportChildren(self, outfile, level, namespace_='', name_='PlantType_single_nochild', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.anytypeobjs_ is not None:
             self.anytypeobjs_.export(outfile, level, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.anytypeobjs_ is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='PlantType_single_nochild'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.anytypeobjs_ is not None:
             showIndent(outfile, level)
             outfile.write('anytypeobjs_=model_.anytypeobjs_(\n')
             self.anytypeobjs_.exportLiteral(outfile, level)
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         obj_ = self.gds_build_any(child_, 'PlantType_single_nochild')
@@ -982,22 +1025,29 @@
         else:
             return PlantType_multiple_nochild(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
+    def hasContent_(self):
+        if (
+            self.anytypeobjs_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='PlantType_multiple_nochild', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='PlantType_multiple_nochild')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -1007,39 +1057,34 @@
     def exportChildren(self, outfile, level, namespace_='', name_='PlantType_multiple_nochild', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for obj_ in self.anytypeobjs_:
             obj_.export(outfile, level, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.anytypeobjs_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='PlantType_multiple_nochild'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('anytypeobjs_=[\n')
         level += 1
         for anytypeobjs_ in self.anytypeobjs_:
             anytypeobjs_.exportLiteral(outfile, level)
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         obj_ = self.gds_build_any(child_, 'PlantType_multiple_nochild')
@@ -1084,14 +1129,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'PlantType_single'
+        rootClass = PlantType_single
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'PlantType_single'
```

### Comparing `generateDS-2.8b/tests/extensions1_sub.py` & `generateDS-2.9a/tests/extensions1_sub.py`

 * *Files 7% similar despite different names*

```diff
@@ -176,18 +176,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'container'
+        rootClass = supermod.containerType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'container'
```

### Comparing `generateDS-2.8b/tests/simpletypes_other2_sub.py` & `generateDS-2.9a/tests/simpletypes_other2_sub.py`

 * *Files 10% similar despite different names*

```diff
@@ -106,18 +106,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'simpleTypeTests'
+        rootClass = supermod.simpleTypeTestsType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'simpleTypeTests'
```

### Comparing `generateDS-2.8b/tests/ipo2_sub.py` & `generateDS-2.9a/tests/ipo2_sub.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,18 +134,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
     sys.stdout.write('<?xml version="1.0" ?>\n')
     rootObj.export(sys.stdout, 0, name_=rootTag,
         namespacedef_='',
         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'purchaseOrder'
+        rootClass = supermod.PurchaseOrderType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+    content = etree_.tostring(rootElement, pretty_print=True,
+        xml_declaration=True, encoding="utf-8")
+    sys.stdout.write(content)
+    sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'purchaseOrder'
```

### Comparing `generateDS-2.8b/tests/abstract_type2_sub.py` & `generateDS-2.9a/tests/abstract_type2_sub.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,18 +120,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'carrier'
+        rootClass = supermod.carrierType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'carrier'
```

### Comparing `generateDS-2.8b/tests/abstract_type1_sub.py` & `generateDS-2.9a/tests/abstract_type1_sub.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,18 +120,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'carrier'
+        rootClass = supermod.carrierType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'carrier'
```

### Comparing `generateDS-2.8b/tests/anywildcard2_sub.py` & `generateDS-2.9a/tests/anywildcard2_sub.py`

 * *Files 16% similar despite different names*

```diff
@@ -134,18 +134,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'PlantType_single'
+        rootClass = supermod.PlantType_single
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'PlantType_single'
```

### Comparing `generateDS-2.8b/tests/attr_groups.xsd` & `generateDS-2.9a/tests/attr_groups.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/ipo.xsd` & `generateDS-2.9a/tests/ipo.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/literal1.py` & `generateDS-2.9a/tests/literal1.py`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/attr_groups1_sup.py` & `generateDS-2.9a/tests/attr_groups1_sup.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -522,161 +555,163 @@
     def set_value01(self, value01): self.value01 = value01
     def get_value02(self): return self.value02
     def set_value02(self, value02): self.value02 = value02
     def get_value03(self): return self.value03
     def set_value03(self, value03): self.value03 = value03
     def get_sequence(self): return self.sequence
     def set_sequence(self, sequence): self.sequence = sequence
+    def hasContent_(self):
+        if (
+            self.returnedTags is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='GetUserReq', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='GetUserReq')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='GetUserReq'):
         if self.value04 is not None and 'value04' not in already_processed:
-            already_processed.append('value04')
+            already_processed.add('value04')
             outfile.write(' value04="%s"' % self.gds_format_integer(self.value04, input_name='value04'))
         if self.value05 is not None and 'value05' not in already_processed:
-            already_processed.append('value05')
+            already_processed.add('value05')
             outfile.write(' value05=%s' % (self.gds_format_string(quote_attrib(self.value05).encode(ExternalEncoding), input_name='value05'), ))
         if self.value06 is not None and 'value06' not in already_processed:
-            already_processed.append('value06')
+            already_processed.add('value06')
             outfile.write(' value06="%s"' % self.gds_format_integer(self.value06, input_name='value06'))
         if self.value07 is not None and 'value07' not in already_processed:
-            already_processed.append('value07')
+            already_processed.add('value07')
             outfile.write(' value07="%s"' % self.gds_format_integer(self.value07, input_name='value07'))
         if self.value01 is not None and 'value01' not in already_processed:
-            already_processed.append('value01')
+            already_processed.add('value01')
             outfile.write(' value01=%s' % (self.gds_format_string(quote_attrib(self.value01).encode(ExternalEncoding), input_name='value01'), ))
         if self.value02 is not None and 'value02' not in already_processed:
-            already_processed.append('value02')
+            already_processed.add('value02')
             outfile.write(' value02="%s"' % self.gds_format_integer(self.value02, input_name='value02'))
         if self.value03 is not None and 'value03' not in already_processed:
-            already_processed.append('value03')
+            already_processed.add('value03')
             outfile.write(' value03=%s' % (self.gds_format_string(quote_attrib(self.value03).encode(ExternalEncoding), input_name='value03'), ))
         if self.sequence is not None and 'sequence' not in already_processed:
-            already_processed.append('sequence')
+            already_processed.add('sequence')
             outfile.write(' sequence="%s"' % self.gds_format_integer(self.sequence, input_name='sequence'))
     def exportChildren(self, outfile, level, namespace_='', name_='GetUserReq', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.returnedTags is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sreturnedTags>%s</%sreturnedTags>%s' % (namespace_, self.gds_format_string(quote_xml(self.returnedTags).encode(ExternalEncoding), input_name='returnedTags'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.returnedTags is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='GetUserReq'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.value04 is not None and 'value04' not in already_processed:
-            already_processed.append('value04')
+            already_processed.add('value04')
             showIndent(outfile, level)
             outfile.write('value04 = %d,\n' % (self.value04,))
         if self.value05 is not None and 'value05' not in already_processed:
-            already_processed.append('value05')
+            already_processed.add('value05')
             showIndent(outfile, level)
             outfile.write('value05 = "%s",\n' % (self.value05,))
         if self.value06 is not None and 'value06' not in already_processed:
-            already_processed.append('value06')
+            already_processed.add('value06')
             showIndent(outfile, level)
             outfile.write('value06 = %d,\n' % (self.value06,))
         if self.value07 is not None and 'value07' not in already_processed:
-            already_processed.append('value07')
+            already_processed.add('value07')
             showIndent(outfile, level)
             outfile.write('value07 = %d,\n' % (self.value07,))
         if self.value01 is not None and 'value01' not in already_processed:
-            already_processed.append('value01')
+            already_processed.add('value01')
             showIndent(outfile, level)
             outfile.write('value01 = "%s",\n' % (self.value01,))
         if self.value02 is not None and 'value02' not in already_processed:
-            already_processed.append('value02')
+            already_processed.add('value02')
             showIndent(outfile, level)
             outfile.write('value02 = %d,\n' % (self.value02,))
         if self.value03 is not None and 'value03' not in already_processed:
-            already_processed.append('value03')
+            already_processed.add('value03')
             showIndent(outfile, level)
             outfile.write('value03 = "%s",\n' % (self.value03,))
         if self.sequence is not None and 'sequence' not in already_processed:
-            already_processed.append('sequence')
+            already_processed.add('sequence')
             showIndent(outfile, level)
             outfile.write('sequence = %d,\n' % (self.sequence,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.returnedTags is not None:
             showIndent(outfile, level)
             outfile.write('returnedTags=%s,\n' % quote_python(self.returnedTags).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('value04', node)
         if value is not None and 'value04' not in already_processed:
-            already_processed.append('value04')
+            already_processed.add('value04')
             try:
                 self.value04 = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('value05', node)
         if value is not None and 'value05' not in already_processed:
-            already_processed.append('value05')
+            already_processed.add('value05')
             self.value05 = value
         value = find_attr_value_('value06', node)
         if value is not None and 'value06' not in already_processed:
-            already_processed.append('value06')
+            already_processed.add('value06')
             try:
                 self.value06 = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('value07', node)
         if value is not None and 'value07' not in already_processed:
-            already_processed.append('value07')
+            already_processed.add('value07')
             try:
                 self.value07 = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('value01', node)
         if value is not None and 'value01' not in already_processed:
-            already_processed.append('value01')
+            already_processed.add('value01')
             self.value01 = value
         value = find_attr_value_('value02', node)
         if value is not None and 'value02' not in already_processed:
-            already_processed.append('value02')
+            already_processed.add('value02')
             try:
                 self.value02 = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('value03', node)
         if value is not None and 'value03' not in already_processed:
-            already_processed.append('value03')
+            already_processed.add('value03')
             self.value03 = value
         value = find_attr_value_('sequence', node)
         if value is not None and 'sequence' not in already_processed:
-            already_processed.append('sequence')
+            already_processed.add('sequence')
             try:
                 self.sequence = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'returnedTags':
             returnedTags_ = child_.text
@@ -721,14 +756,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'getUser'
+        rootClass = GetUserReq
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'getUser'
```

### Comparing `generateDS-2.8b/tests/out2_sub.py` & `generateDS-2.9a/tests/out2_sub.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,18 +176,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
     sys.stdout.write('<?xml version="1.0" ?>\n')
     rootObj.export(sys.stdout, 0, name_=rootTag,
         namespacedef_='',
         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'people'
+        rootClass = supermod.people
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+    content = etree_.tostring(rootElement, pretty_print=True,
+        xml_declaration=True, encoding="utf-8")
+    sys.stdout.write(content)
+    sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'people'
```

### Comparing `generateDS-2.8b/tests/simplecontent_restriction.xsd` & `generateDS-2.9a/tests/simplecontent_restriction.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/groups.xsd` & `generateDS-2.9a/tests/groups.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/simpletype_memberspecs.xsd` & `generateDS-2.9a/tests/simpletype_memberspecs.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/annotations.xsd` & `generateDS-2.9a/tests/annotations.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/ipo2_sup.py` & `generateDS-2.9a/tests/ipo2_sup.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -506,33 +539,43 @@
     def set_billTo(self, billTo): self.billTo = billTo
     def get_comment(self): return self.comment
     def set_comment(self, comment): self.comment = comment
     def get_items(self): return self.items
     def set_items(self, items): self.items = items
     def get_orderDate(self): return self.orderDate
     def set_orderDate(self, orderDate): self.orderDate = orderDate
+    def hasContent_(self):
+        if (
+            self.shipTo is not None or
+            self.billTo is not None or
+            self.comment is not None or
+            self.items is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='PurchaseOrderType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='PurchaseOrderType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='ipo:', name_='PurchaseOrderType'):
         if self.orderDate is not None and 'orderDate' not in already_processed:
-            already_processed.append('orderDate')
+            already_processed.add('orderDate')
             outfile.write(' orderDate="%s"' % self.gds_format_date(self.orderDate, input_name='orderDate'))
     def exportChildren(self, outfile, level, namespace_='ipo:', name_='PurchaseOrderType', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.shipTo is not None:
@@ -540,32 +583,23 @@
         if self.billTo is not None:
             self.billTo.export(outfile, level, namespace_, name_='billTo', pretty_print=pretty_print)
         if self.comment is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scomment>%s</%scomment>%s' % (namespace_, self.gds_format_string(quote_xml(self.comment).encode(ExternalEncoding), input_name='comment'), namespace_, eol_))
         if self.items is not None:
             self.items.export(outfile, level, namespace_, name_='items', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.shipTo is not None or
-            self.billTo is not None or
-            self.comment is not None or
-            self.items is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='PurchaseOrderType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.orderDate is not None and 'orderDate' not in already_processed:
-            already_processed.append('orderDate')
+            already_processed.add('orderDate')
             showIndent(outfile, level)
             outfile.write('orderDate = "%s",\n' % (self.orderDate,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.shipTo is not None:
             showIndent(outfile, level)
             outfile.write('shipTo=model_.Address(\n')
             self.shipTo.exportLiteral(outfile, level, name_='shipTo')
@@ -583,22 +617,23 @@
         if self.items is not None:
             showIndent(outfile, level)
             outfile.write('items=model_.Items(\n')
             self.items.exportLiteral(outfile, level, name_='items')
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('orderDate', node)
         if value is not None and 'orderDate' not in already_processed:
-            already_processed.append('orderDate')
+            already_processed.add('orderDate')
             try:
                 self.orderDate = self.gds_parse_date(value, node, 'orderDate')
             except ValueError, exp:
                 raise ValueError('Bad date attribute (orderDate): %s' % exp)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'shipTo':
             class_obj_ = self.get_class_obj_(child_, Address)
@@ -638,22 +673,29 @@
         else:
             return Items(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_item(self): return self.item
     def set_item(self, item): self.item = item
     def add_item(self, value): self.item.append(value)
     def insert_item(self, index, value): self.item[index] = value
+    def hasContent_(self):
+        if (
+            self.item
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='Items', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='Items')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -663,24 +705,18 @@
     def exportChildren(self, outfile, level, namespace_='ipo:', name_='Items', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for item_ in self.item:
             item_.export(outfile, level, namespace_, name_='item', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.item
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='Items'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('item=[\n')
@@ -691,15 +727,16 @@
             item_.exportLiteral(outfile, level, name_='itemType')
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'item':
@@ -732,33 +769,42 @@
     def set_name(self, name): self.name = name
     def get_street(self): return self.street
     def set_street(self, street): self.street = street
     def get_city(self): return self.city
     def set_city(self, city): self.city = city
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.street is not None or
+            self.city is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='Address', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='Address')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='ipo:', name_='Address'):
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
         pass
     def exportChildren(self, outfile, level, namespace_='ipo:', name_='Address', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
@@ -768,26 +814,18 @@
             outfile.write('<%sname>%s</%sname>%s' % (namespace_, self.gds_format_string(quote_xml(self.name).encode(ExternalEncoding), input_name='name'), namespace_, eol_))
         if self.street is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sstreet>%s</%sstreet>%s' % (namespace_, self.gds_format_string(quote_xml(self.street).encode(ExternalEncoding), input_name='street'), namespace_, eol_))
         if self.city is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scity>%s</%scity>%s' % (namespace_, self.gds_format_string(quote_xml(self.city).encode(ExternalEncoding), input_name='city'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.street is not None or
-            self.city is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='Address'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
@@ -795,22 +833,23 @@
         if self.street is not None:
             showIndent(outfile, level)
             outfile.write('street=%s,\n' % quote_python(self.street).encode(ExternalEncoding))
         if self.city is not None:
             showIndent(outfile, level)
             outfile.write('city=%s,\n' % quote_python(self.city).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
             name_ = child_.text
             name_ = self.gds_validate_string(name_, node, 'name')
             self.name = name_
         elif nodeName_ == 'street':
@@ -844,22 +883,31 @@
     def get_state(self): return self.state
     def set_state(self, state): self.state = state
     def validate_USState(self, value):
         # Validate type USState, a restriction on string.
         pass
     def get_zip(self): return self.zip
     def set_zip(self, zip): self.zip = zip
+    def hasContent_(self):
+        if (
+            self.state is not None or
+            self.zip is not None or
+            super(USAddress, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='USAddress', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='USAddress')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -874,40 +922,33 @@
             eol_ = ''
         if self.state is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sstate>%s</%sstate>%s' % (namespace_, self.gds_format_string(quote_xml(self.state).encode(ExternalEncoding), input_name='state'), namespace_, eol_))
         if self.zip is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%szip>%s</%szip>%s' % (namespace_, self.gds_format_integer(self.zip, input_name='zip'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.state is not None or
-            self.zip is not None or
-            super(USAddress, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='USAddress'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(USAddress, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(USAddress, self).exportLiteralChildren(outfile, level, name_)
         if self.state is not None:
             showIndent(outfile, level)
             outfile.write('state=%s,\n' % quote_python(self.state).encode(ExternalEncoding))
         if self.zip is not None:
             showIndent(outfile, level)
             outfile.write('zip=%d,\n' % self.zip)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(USAddress, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'state':
@@ -957,95 +998,97 @@
         pass
     def get_category(self): return self.category
     def set_category(self, category): self.category = category
     def get_category_attr(self): return self.category_attr
     def set_category_attr(self, category_attr): self.category_attr = category_attr
     def get_exportCode(self): return self.exportCode
     def set_exportCode(self, exportCode): self.exportCode = exportCode
+    def hasContent_(self):
+        if (
+            self.postcode is not None or
+            self.category is not None or
+            super(UKAddress, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='UKAddress', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='UKAddress')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='ipo:', name_='UKAddress'):
         super(UKAddress, self).exportAttributes(outfile, level, already_processed, namespace_, name_='UKAddress')
         if self.category_attr is not None and 'category_attr' not in already_processed:
-            already_processed.append('category_attr')
+            already_processed.add('category_attr')
             outfile.write(' category=%s' % (quote_attrib(self.category_attr), ))
         if self.exportCode is not None and 'exportCode' not in already_processed:
-            already_processed.append('exportCode')
+            already_processed.add('exportCode')
             outfile.write(' exportCode="%s"' % self.gds_format_integer(self.exportCode, input_name='exportCode'))
     def exportChildren(self, outfile, level, namespace_='ipo:', name_='UKAddress', fromsubclass_=False, pretty_print=True):
         super(UKAddress, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.postcode is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%spostcode>%s</%spostcode>%s' % (namespace_, self.gds_format_string(quote_xml(self.postcode).encode(ExternalEncoding), input_name='postcode'), namespace_, eol_))
         if self.category is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scategory>%s</%scategory>%s' % (namespace_, self.gds_format_string(quote_xml(self.category).encode(ExternalEncoding), input_name='category'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.postcode is not None or
-            self.category is not None or
-            super(UKAddress, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='UKAddress'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.category_attr is not None and 'category_attr' not in already_processed:
-            already_processed.append('category_attr')
+            already_processed.add('category_attr')
             showIndent(outfile, level)
             outfile.write('category_attr = %s,\n' % (self.category_attr,))
         if self.exportCode is not None and 'exportCode' not in already_processed:
-            already_processed.append('exportCode')
+            already_processed.add('exportCode')
             showIndent(outfile, level)
             outfile.write('exportCode = %d,\n' % (self.exportCode,))
         super(UKAddress, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(UKAddress, self).exportLiteralChildren(outfile, level, name_)
         if self.postcode is not None:
             showIndent(outfile, level)
             outfile.write('postcode=%s,\n' % quote_python(self.postcode).encode(ExternalEncoding))
         if self.category is not None:
             showIndent(outfile, level)
             outfile.write('category=%s,\n' % quote_python(self.category).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('category', node)
         if value is not None and 'category_attr' not in already_processed:
-            already_processed.append('category_attr')
+            already_processed.add('category_attr')
             self.category_attr = value
         value = find_attr_value_('exportCode', node)
         if value is not None and 'exportCode' not in already_processed:
-            already_processed.append('exportCode')
+            already_processed.add('exportCode')
             try:
                 self.exportCode = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.exportCode <= 0:
                 raise_parse_error(node, 'Invalid PositiveInteger')
         super(UKAddress, self).buildAttributes(node, attrs, already_processed)
@@ -1095,33 +1138,44 @@
     def set_USPrice(self, USPrice): self.USPrice = USPrice
     def get_comment(self): return self.comment
     def set_comment(self, comment): self.comment = comment
     def get_shipDate(self): return self.shipDate
     def set_shipDate(self, shipDate): self.shipDate = shipDate
     def get_partNum(self): return self.partNum
     def set_partNum(self, partNum): self.partNum = partNum
+    def hasContent_(self):
+        if (
+            self.productName is not None or
+            self.quantity is not None or
+            self.USPrice is not None or
+            self.comment is not None or
+            self.shipDate is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='itemType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='itemType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='ipo:', name_='itemType'):
         if self.partNum is not None and 'partNum' not in already_processed:
-            already_processed.append('partNum')
+            already_processed.add('partNum')
             outfile.write(' partNum=%s' % (quote_attrib(self.partNum), ))
     def exportChildren(self, outfile, level, namespace_='ipo:', name_='itemType', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.productName is not None:
@@ -1135,33 +1189,23 @@
             outfile.write('<%sUSPrice>%s</%sUSPrice>%s' % (namespace_, self.gds_format_float(self.USPrice, input_name='USPrice'), namespace_, eol_))
         if self.comment is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scomment>%s</%scomment>%s' % (namespace_, self.gds_format_string(quote_xml(self.comment).encode(ExternalEncoding), input_name='comment'), namespace_, eol_))
         if self.shipDate is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sshipDate>%s</%sshipDate>%s' % (namespace_, self.gds_format_date(self.shipDate, input_name='shipDate'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.productName is not None or
-            self.quantity is not None or
-            self.USPrice is not None or
-            self.comment is not None or
-            self.shipDate is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='itemType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.partNum is not None and 'partNum' not in already_processed:
-            already_processed.append('partNum')
+            already_processed.add('partNum')
             showIndent(outfile, level)
             outfile.write('partNum = %s,\n' % (self.partNum,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.productName is not None:
             showIndent(outfile, level)
             outfile.write('productName=%s,\n' % quote_python(self.productName).encode(ExternalEncoding))
         if self.quantity is not None:
@@ -1173,22 +1217,23 @@
         if self.comment is not None:
             showIndent(outfile, level)
             outfile.write('comment=%s,\n' % quote_python(self.comment).encode(ExternalEncoding))
         if self.shipDate is not None:
             showIndent(outfile, level)
             outfile.write('shipDate=datetime_.strptime("%s", "%%Y-%%m-%%d"),\n' % self.gds_format_date(self.shipDate, input_name='shipDate'))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('partNum', node)
         if value is not None and 'partNum' not in already_processed:
-            already_processed.append('partNum')
+            already_processed.add('partNum')
             self.partNum = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'productName':
             productName_ = child_.text
             productName_ = self.gds_validate_string(productName_, node, 'productName')
             self.productName = productName_
         elif nodeName_ == 'quantity':
@@ -1229,51 +1274,53 @@
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if quantity.subclass:
             return quantity.subclass(*args_, **kwargs_)
         else:
             return quantity(*args_, **kwargs_)
     factory = staticmethod(factory)
+    def hasContent_(self):
+        if (
+
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='quantity', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='quantity')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='ipo:', name_='quantity'):
         pass
     def exportChildren(self, outfile, level, namespace_='ipo:', name_='quantity', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='quantity'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
@@ -1320,14 +1367,33 @@
     sys.stdout.write('<?xml version="1.0" ?>\n')
     rootObj.export(sys.stdout, 0, name_=rootTag,
         namespacedef_='',
         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'purchaseOrder'
+        rootClass = PurchaseOrderType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+    content = etree_.tostring(rootElement, pretty_print=True,
+        xml_declaration=True, encoding="utf-8")
+    sys.stdout.write(content)
+    sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'purchaseOrder'
```

### Comparing `generateDS-2.8b/tests/simpletypes_other.xsd` & `generateDS-2.9a/tests/simpletypes_other.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/simpletypes_other2_sup.py` & `generateDS-2.9a/tests/simpletypes_other2_sup.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -495,22 +528,29 @@
         else:
             return simpleTypeTestsType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_simpleTypeTest(self): return self.simpleTypeTest
     def set_simpleTypeTest(self, simpleTypeTest): self.simpleTypeTest = simpleTypeTest
     def add_simpleTypeTest(self, value): self.simpleTypeTest.append(value)
     def insert_simpleTypeTest(self, index, value): self.simpleTypeTest[index] = value
+    def hasContent_(self):
+        if (
+            self.simpleTypeTest
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='simpleTypeTestsType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='simpleTypeTestsType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -521,24 +561,18 @@
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for simpleTypeTest_ in self.simpleTypeTest:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%ssimpleTypeTest>%s</%ssimpleTypeTest>%s' % (namespace_, self.gds_format_string(quote_xml(simpleTypeTest_).encode(ExternalEncoding), input_name='simpleTypeTest'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.simpleTypeTest
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='simpleTypeTestsType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('simpleTypeTest=[\n')
@@ -546,15 +580,16 @@
         for simpleTypeTest_ in self.simpleTypeTest:
             showIndent(outfile, level)
             outfile.write('%s,\n' % quote_python(simpleTypeTest_).encode(ExternalEncoding))
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'simpleTypeTest':
@@ -696,22 +731,49 @@
     def insert_dateVal2(self, index, value): self.dateVal2[index] = value
     def get_dateTimeVal1(self): return self.dateTimeVal1
     def set_dateTimeVal1(self, dateTimeVal1): self.dateTimeVal1 = dateTimeVal1
     def get_dateTimeVal2(self): return self.dateTimeVal2
     def set_dateTimeVal2(self, dateTimeVal2): self.dateTimeVal2 = dateTimeVal2
     def add_dateTimeVal2(self, value): self.dateTimeVal2.append(value)
     def insert_dateTimeVal2(self, index, value): self.dateTimeVal2[index] = value
+    def hasContent_(self):
+        if (
+            self.datetime1 is not None or
+            self.datetime2 is not None or
+            self.datetime3 is not None or
+            self.datetime4 is not None or
+            self.datetime5 is not None or
+            self.integerVal1 is not None or
+            self.integerVal2 or
+            self.stringVal1 is not None or
+            self.stringVal2 or
+            self.booleanVal1 is not None or
+            self.booleanVal2 or
+            self.decimalVal1 is not None or
+            self.decimalVal2 or
+            self.doubleVal1 is not None or
+            self.doubleVal2 or
+            self.floatVal1 is not None or
+            self.floatVal2 or
+            self.dateVal1 is not None or
+            self.dateVal2 or
+            self.dateTimeVal1 is not None or
+            self.dateTimeVal2
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='simpleTypeTest', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='simpleTypeTest')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -748,18 +810,18 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sstringVal1>%s</%sstringVal1>%s' % (namespace_, self.gds_format_string(quote_xml(self.stringVal1).encode(ExternalEncoding), input_name='stringVal1'), namespace_, eol_))
         for stringVal2_ in self.stringVal2:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sstringVal2>%s</%sstringVal2>%s' % (namespace_, self.gds_format_string(quote_xml(stringVal2_).encode(ExternalEncoding), input_name='stringVal2'), namespace_, eol_))
         if self.booleanVal1 is not None:
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sbooleanVal1>%s</%sbooleanVal1>%s' % (namespace_, self.gds_format_boolean(self.gds_str_lower(str(self.booleanVal1)), input_name='booleanVal1'), namespace_, eol_))
+            outfile.write('<%sbooleanVal1>%s</%sbooleanVal1>%s' % (namespace_, self.gds_format_boolean(self.booleanVal1, input_name='booleanVal1'), namespace_, eol_))
         for booleanVal2_ in self.booleanVal2:
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sbooleanVal2>%s</%sbooleanVal2>%s' % (namespace_, self.gds_format_boolean(self.gds_str_lower(str(booleanVal2_)), input_name='booleanVal2'), namespace_, eol_))
+            outfile.write('<%sbooleanVal2>%s</%sbooleanVal2>%s' % (namespace_, self.gds_format_boolean(booleanVal2_, input_name='booleanVal2'), namespace_, eol_))
         if self.decimalVal1 is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdecimalVal1>%s</%sdecimalVal1>%s' % (namespace_, self.gds_format_float(self.decimalVal1, input_name='decimalVal1'), namespace_, eol_))
         for decimalVal2_ in self.decimalVal2:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdecimalVal2>%s</%sdecimalVal2>%s' % (namespace_, self.gds_format_float(decimalVal2_, input_name='decimalVal2'), namespace_, eol_))
         if self.doubleVal1 is not None:
@@ -782,44 +844,18 @@
             outfile.write('<%sdateVal2>%s</%sdateVal2>%s' % (namespace_, self.gds_format_date(dateVal2_, input_name='dateVal2'), namespace_, eol_))
         if self.dateTimeVal1 is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdateTimeVal1>%s</%sdateTimeVal1>%s' % (namespace_, self.gds_format_datetime(self.dateTimeVal1, input_name='dateTimeVal1'), namespace_, eol_))
         for dateTimeVal2_ in self.dateTimeVal2:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdateTimeVal2>%s</%sdateTimeVal2>%s' % (namespace_, self.gds_format_datetime(dateTimeVal2_, input_name='dateTimeVal2'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.datetime1 is not None or
-            self.datetime2 is not None or
-            self.datetime3 is not None or
-            self.datetime4 is not None or
-            self.datetime5 is not None or
-            self.integerVal1 is not None or
-            self.integerVal2 or
-            self.stringVal1 is not None or
-            self.stringVal2 or
-            self.booleanVal1 is not None or
-            self.booleanVal2 or
-            self.decimalVal1 is not None or
-            self.decimalVal2 or
-            self.doubleVal1 is not None or
-            self.doubleVal2 or
-            self.floatVal1 is not None or
-            self.floatVal2 or
-            self.dateVal1 is not None or
-            self.dateVal2 or
-            self.dateTimeVal1 is not None or
-            self.dateTimeVal2
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='simpleTypeTest'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.datetime1 is not None:
             showIndent(outfile, level)
@@ -929,15 +965,16 @@
         for dateTimeVal2_ in self.dateTimeVal2:
             showIndent(outfile, level)
             outfile.write('%s,\n' % self.gds_format_datetime(dateTimeVal2_, input_name='dateTimeVal2'))
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'datetime1':
@@ -1107,14 +1144,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'simpleTypeTests'
+        rootClass = simpleTypeTestsType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'simpleTypeTests'
```

### Comparing `generateDS-2.8b/tests/annotations2_sup.py` & `generateDS-2.9a/tests/annotations2_sup.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -497,22 +530,30 @@
         else:
             return document1Type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_comments(self): return self.comments
     def set_comments(self, comments): self.comments = comments
     def get_otherdoc(self): return self.otherdoc
     def set_otherdoc(self, otherdoc): self.otherdoc = otherdoc
+    def hasContent_(self):
+        if (
+            self.comments is not None or
+            self.otherdoc is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='document1Type', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='document1Type')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -525,25 +566,18 @@
         else:
             eol_ = ''
         if self.comments is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scomments>%s</%scomments>%s' % (namespace_, self.gds_format_string(quote_xml(self.comments).encode(ExternalEncoding), input_name='comments'), namespace_, eol_))
         if self.otherdoc is not None:
             self.otherdoc.export(outfile, level, namespace_, name_='otherdoc', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.comments is not None or
-            self.otherdoc is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='document1Type'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.comments is not None:
             showIndent(outfile, level)
@@ -551,15 +585,16 @@
         if self.otherdoc is not None:
             showIndent(outfile, level)
             outfile.write('otherdoc=model_.document2Type(\n')
             self.otherdoc.exportLiteral(outfile, level, name_='otherdoc')
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'comments':
@@ -596,22 +631,31 @@
     factory = staticmethod(factory)
     def get_comments(self): return self.comments
     def set_comments(self, comments): self.comments = comments
     def get_rating(self): return self.rating
     def set_rating(self, rating): self.rating = rating
     def get_anotherdoc(self): return self.anotherdoc
     def set_anotherdoc(self, anotherdoc): self.anotherdoc = anotherdoc
+    def hasContent_(self):
+        if (
+            self.comments is not None or
+            self.rating is not None or
+            self.anotherdoc is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='document2Type', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='document2Type')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -627,26 +671,18 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scomments>%s</%scomments>%s' % (namespace_, self.gds_format_string(quote_xml(self.comments).encode(ExternalEncoding), input_name='comments'), namespace_, eol_))
         if self.rating is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%srating>%s</%srating>%s' % (namespace_, self.gds_format_integer(self.rating, input_name='rating'), namespace_, eol_))
         if self.anotherdoc is not None:
             self.anotherdoc.export(outfile, level, namespace_, name_='anotherdoc', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.comments is not None or
-            self.rating is not None or
-            self.anotherdoc is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='document2Type'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.comments is not None:
             showIndent(outfile, level)
@@ -657,15 +693,16 @@
         if self.anotherdoc is not None:
             showIndent(outfile, level)
             outfile.write('anotherdoc=model_.document3Type(\n')
             self.anotherdoc.exportLiteral(outfile, level, name_='anotherdoc')
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'comments':
@@ -704,22 +741,30 @@
         else:
             return document3Type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_comments(self): return self.comments
     def set_comments(self, comments): self.comments = comments
     def get_rating(self): return self.rating
     def set_rating(self, rating): self.rating = rating
+    def hasContent_(self):
+        if (
+            self.comments is not None or
+            self.rating is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='document3Type', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='document3Type')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -733,38 +778,32 @@
             eol_ = ''
         if self.comments is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scomments>%s</%scomments>%s' % (namespace_, self.gds_format_string(quote_xml(self.comments).encode(ExternalEncoding), input_name='comments'), namespace_, eol_))
         if self.rating is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%srating>%s</%srating>%s' % (namespace_, self.gds_format_integer(self.rating, input_name='rating'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.comments is not None or
-            self.rating is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='document3Type'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.comments is not None:
             showIndent(outfile, level)
             outfile.write('comments=%s,\n' % quote_python(self.comments).encode(ExternalEncoding))
         if self.rating is not None:
             showIndent(outfile, level)
             outfile.write('rating=%d,\n' % self.rating)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'comments':
@@ -820,14 +859,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'document1'
+        rootClass = document1Type
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'document1'
```

### Comparing `generateDS-2.8b/tests/people_procincl1_sup.py` & `generateDS-2.9a/tests/people_procincl1_sup.py`

 * *Files 12% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -541,22 +574,34 @@
     def set_python_programmer(self, python_programmer): self.python_programmer = python_programmer
     def add_python_programmer(self, value): self.python_programmer.append(value)
     def insert_python_programmer(self, index, value): self.python_programmer[index] = value
     def get_java_programmer(self): return self.java_programmer
     def set_java_programmer(self, java_programmer): self.java_programmer = java_programmer
     def add_java_programmer(self, value): self.java_programmer.append(value)
     def insert_java_programmer(self, index, value): self.java_programmer[index] = value
+    def hasContent_(self):
+        if (
+            self.comments or
+            self.person or
+            self.specialperson or
+            self.programmer or
+            self.python_programmer or
+            self.java_programmer
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='people', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='people')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -576,29 +621,18 @@
             specialperson_.export(outfile, level, namespace_, name_='specialperson', pretty_print=pretty_print)
         for programmer_ in self.programmer:
             programmer_.export(outfile, level, namespace_, name_='programmer', pretty_print=pretty_print)
         for python_programmer_ in self.python_programmer:
             python_programmer_.export(outfile, level, namespace_, name_='python-programmer', pretty_print=pretty_print)
         for java_programmer_ in self.java_programmer:
             java_programmer_.export(outfile, level, namespace_, name_='java-programmer', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.comments or
-            self.person or
-            self.specialperson or
-            self.programmer or
-            self.python_programmer or
-            self.java_programmer
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='people'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('comments=[\n')
@@ -669,15 +703,16 @@
             java_programmer_.exportLiteral(outfile, level, name_='java-programmer')
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'comments':
@@ -748,48 +783,49 @@
     def insert_emp(self, index, value): self.emp[index] = value
     def get_bold(self): return self.bold
     def set_bold(self, bold): self.bold = bold
     def add_bold(self, value): self.bold.append(value)
     def insert_bold(self, index, value): self.bold[index] = value
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.emp or
+            self.bold or
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='comments', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='comments')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='comments'):
         pass
     def exportChildren(self, outfile, level, namespace_='', name_='comments', fromsubclass_=False, pretty_print=True):
         if not fromsubclass_:
             for item_ in self.content_:
                 item_.export(outfile, level, item_.name, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.emp or
-            self.bold or
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='comments'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
@@ -803,15 +839,16 @@
         outfile.write('content_ = [\n')
         for item_ in self.content_:
             item_.exportLiteral(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('],\n')
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         if node.text is not None:
             obj_ = self.mixedclass_(MixedContainer.CategoryText,
                 MixedContainer.TypeNone, '', node.text)
             self.content_.append(obj_)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
@@ -909,48 +946,60 @@
     def set_ratio(self, ratio): self.ratio = ratio
     def get_id(self): return self.id
     def set_id(self, id): self.id = id
     def get_value(self): return self.value
     def set_value(self, value): self.value = value
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.interest or
+            self.category is not None or
+            self.agent or
+            self.promoter or
+            self.description is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='person', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='person')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='person'):
         if self.vegetable is not None and 'vegetable' not in already_processed:
-            already_processed.append('vegetable')
+            already_processed.add('vegetable')
             outfile.write(' vegetable=%s' % (self.gds_format_string(quote_attrib(self.vegetable).encode(ExternalEncoding), input_name='vegetable'), ))
         if self.fruit is not None and 'fruit' not in already_processed:
-            already_processed.append('fruit')
+            already_processed.add('fruit')
             outfile.write(' fruit=%s' % (self.gds_format_string(quote_attrib(self.fruit).encode(ExternalEncoding), input_name='fruit'), ))
         if self.ratio is not None and 'ratio' not in already_processed:
-            already_processed.append('ratio')
+            already_processed.add('ratio')
             outfile.write(' ratio="%s"' % self.gds_format_float(self.ratio, input_name='ratio'))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             outfile.write(' id="%s"' % self.gds_format_integer(self.id, input_name='id'))
         if self.value is not None and 'value' not in already_processed:
-            already_processed.append('value')
+            already_processed.add('value')
             outfile.write(' value=%s' % (self.gds_format_string(quote_attrib(self.value).encode(ExternalEncoding), input_name='value'), ))
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
     def exportChildren(self, outfile, level, namespace_='', name_='person', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
@@ -966,50 +1015,39 @@
         for agent_ in self.agent:
             agent_.export(outfile, level, namespace_, name_='agent', pretty_print=pretty_print)
         for promoter_ in self.promoter:
             promoter_.export(outfile, level, namespace_, name_='promoter', pretty_print=pretty_print)
         if self.description is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdescription>%s</%sdescription>%s' % (namespace_, self.gds_format_string(quote_xml(self.description).encode(ExternalEncoding), input_name='description'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.interest or
-            self.category is not None or
-            self.agent or
-            self.promoter or
-            self.description is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='person'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.vegetable is not None and 'vegetable' not in already_processed:
-            already_processed.append('vegetable')
+            already_processed.add('vegetable')
             showIndent(outfile, level)
             outfile.write('vegetable = "%s",\n' % (self.vegetable,))
         if self.fruit is not None and 'fruit' not in already_processed:
-            already_processed.append('fruit')
+            already_processed.add('fruit')
             showIndent(outfile, level)
             outfile.write('fruit = "%s",\n' % (self.fruit,))
         if self.ratio is not None and 'ratio' not in already_processed:
-            already_processed.append('ratio')
+            already_processed.add('ratio')
             showIndent(outfile, level)
             outfile.write('ratio = %f,\n' % (self.ratio,))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             showIndent(outfile, level)
             outfile.write('id = %d,\n' % (self.id,))
         if self.value is not None and 'value' not in already_processed:
-            already_processed.append('value')
+            already_processed.add('value')
             showIndent(outfile, level)
             outfile.write('value = "%s",\n' % (self.value,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
             outfile.write('name=%s,\n' % quote_python(self.name).encode(ExternalEncoding))
         showIndent(outfile, level)
@@ -1048,48 +1086,49 @@
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
         if self.description is not None:
             showIndent(outfile, level)
             outfile.write('description=%s,\n' % quote_python(self.description).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('vegetable', node)
         if value is not None and 'vegetable' not in already_processed:
-            already_processed.append('vegetable')
+            already_processed.add('vegetable')
             self.vegetable = value
         value = find_attr_value_('fruit', node)
         if value is not None and 'fruit' not in already_processed:
-            already_processed.append('fruit')
+            already_processed.add('fruit')
             self.fruit = value
         value = find_attr_value_('ratio', node)
         if value is not None and 'ratio' not in already_processed:
-            already_processed.append('ratio')
+            already_processed.add('ratio')
             try:
                 self.ratio = float(value)
             except ValueError, exp:
                 raise ValueError('Bad float/double attribute (ratio): %s' % exp)
         value = find_attr_value_('id', node)
         if value is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             try:
                 self.id = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('value', node)
         if value is not None and 'value' not in already_processed:
-            already_processed.append('value')
+            already_processed.add('value')
             self.value = value
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
             name_ = child_.text
             name_ = self.gds_validate_string(name_, node, 'name')
             self.name = name_
         elif nodeName_ == 'interest':
@@ -1129,52 +1168,54 @@
         pass
     def factory(*args_, **kwargs_):
         if specialperson.subclass:
             return specialperson.subclass(*args_, **kwargs_)
         else:
             return specialperson(*args_, **kwargs_)
     factory = staticmethod(factory)
+    def hasContent_(self):
+        if (
+            super(specialperson, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='specialperson', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='specialperson')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='specialperson'):
         super(specialperson, self).exportAttributes(outfile, level, already_processed, namespace_, name_='specialperson')
     def exportChildren(self, outfile, level, namespace_='', name_='specialperson', fromsubclass_=False, pretty_print=True):
         super(specialperson, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            super(specialperson, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='specialperson'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(specialperson, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(specialperson, self).exportLiteralChildren(outfile, level, name_)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(specialperson, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         super(specialperson, self).buildChildren(child_, node, nodeName_, True)
@@ -1220,123 +1261,125 @@
     def set_sid(self, sid): self.sid = sid
     def get_type(self): return self.type_
     def set_type(self, type_): self.type_ = type_
     def get_id(self): return self.id
     def set_id(self, id): self.id = id
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='param', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='param')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='param'):
         if self.semantic is not None and 'semantic' not in already_processed:
-            already_processed.append('semantic')
+            already_processed.add('semantic')
             outfile.write(' semantic=%s' % (self.gds_format_string(quote_attrib(self.semantic).encode(ExternalEncoding), input_name='semantic'), ))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             outfile.write(' name=%s' % (quote_attrib(self.name), ))
         if self.flow is not None and 'flow' not in already_processed:
-            already_processed.append('flow')
+            already_processed.add('flow')
             outfile.write(' flow=%s' % (quote_attrib(self.flow), ))
         if self.sid is not None and 'sid' not in already_processed:
-            already_processed.append('sid')
+            already_processed.add('sid')
             outfile.write(' sid=%s' % (quote_attrib(self.sid), ))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             outfile.write(' type=%s' % (self.gds_format_string(quote_attrib(self.type_).encode(ExternalEncoding), input_name='type'), ))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             outfile.write(' id=%s' % (self.gds_format_string(quote_attrib(self.id).encode(ExternalEncoding), input_name='id'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='param', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='param'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.semantic is not None and 'semantic' not in already_processed:
-            already_processed.append('semantic')
+            already_processed.add('semantic')
             showIndent(outfile, level)
             outfile.write('semantic = "%s",\n' % (self.semantic,))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             showIndent(outfile, level)
             outfile.write('name = "%s",\n' % (self.name,))
         if self.flow is not None and 'flow' not in already_processed:
-            already_processed.append('flow')
+            already_processed.add('flow')
             showIndent(outfile, level)
             outfile.write('flow = %s,\n' % (self.flow,))
         if self.sid is not None and 'sid' not in already_processed:
-            already_processed.append('sid')
+            already_processed.add('sid')
             showIndent(outfile, level)
             outfile.write('sid = "%s",\n' % (self.sid,))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             showIndent(outfile, level)
             outfile.write('type_ = "%s",\n' % (self.type_,))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             showIndent(outfile, level)
             outfile.write('id = "%s",\n' % (self.id,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('semantic', node)
         if value is not None and 'semantic' not in already_processed:
-            already_processed.append('semantic')
+            already_processed.add('semantic')
             self.semantic = value
             self.semantic = ' '.join(self.semantic.split())
         value = find_attr_value_('name', node)
         if value is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             self.name = value
         value = find_attr_value_('flow', node)
         if value is not None and 'flow' not in already_processed:
-            already_processed.append('flow')
+            already_processed.add('flow')
             self.flow = value
         value = find_attr_value_('sid', node)
         if value is not None and 'sid' not in already_processed:
-            already_processed.append('sid')
+            already_processed.add('sid')
             self.sid = value
         value = find_attr_value_('type', node)
         if value is not None and 'type' not in already_processed:
-            already_processed.append('type')
+            already_processed.add('type')
             self.type_ = value
         value = find_attr_value_('id', node)
         if value is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             self.id = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class param
 
 
 class agent(GeneratedsSuper):
@@ -1372,22 +1415,33 @@
     def set_priority(self, priority): self.priority = priority
     def get_info(self): return self.info
     def set_info(self, info): self.info = info
     def get_vehicle(self): return self.vehicle
     def set_vehicle(self, vehicle): self.vehicle = vehicle
     def add_vehicle(self, value): self.vehicle.append(value)
     def insert_vehicle(self, index, value): self.vehicle[index] = value
+    def hasContent_(self):
+        if (
+            self.firstname is not None or
+            self.lastname is not None or
+            self.priority is not None or
+            self.info is not None or
+            self.vehicle
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='agent', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='agent')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -1408,28 +1462,18 @@
         if self.priority is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%spriority>%s</%spriority>%s' % (namespace_, self.gds_format_float(self.priority, input_name='priority'), namespace_, eol_))
         if self.info is not None:
             self.info.export(outfile, level, namespace_, name_='info', pretty_print=pretty_print)
         for vehicle_ in self.get_vehicle():
             vehicle_.export(outfile, level, namespace_, name_='vehicle', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.firstname is not None or
-            self.lastname is not None or
-            self.priority is not None or
-            self.info is not None or
-            self.vehicle
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='agent'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.firstname is not None:
             showIndent(outfile, level)
@@ -1455,15 +1499,16 @@
             vehicle_.exportLiteral(outfile, level)
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'firstname':
@@ -1533,22 +1578,32 @@
     def set_firstname(self, firstname): self.firstname = firstname
     def get_lastname(self): return self.lastname
     def set_lastname(self, lastname): self.lastname = lastname
     def get_priority(self): return self.priority
     def set_priority(self, priority): self.priority = priority
     def get_info(self): return self.info
     def set_info(self, info): self.info = info
+    def hasContent_(self):
+        if (
+            self.firstname is not None or
+            self.lastname is not None or
+            self.priority is not None or
+            self.info is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='special-agent', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='special-agent')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -1567,27 +1622,18 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%slastname>%s</%slastname>%s' % (namespace_, self.gds_format_string(quote_xml(self.lastname).encode(ExternalEncoding), input_name='lastname'), namespace_, eol_))
         if self.priority is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%spriority>%s</%spriority>%s' % (namespace_, self.gds_format_float(self.priority, input_name='priority'), namespace_, eol_))
         if self.info is not None:
             self.info.export(outfile, level, namespace_, name_='info', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.firstname is not None or
-            self.lastname is not None or
-            self.priority is not None or
-            self.info is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='special-agent'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.firstname is not None:
             showIndent(outfile, level)
@@ -1601,15 +1647,16 @@
         if self.info is not None:
             showIndent(outfile, level)
             outfile.write('info=model_.info(\n')
             self.info.exportLiteral(outfile, level)
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'firstname':
@@ -1690,33 +1737,46 @@
     def insert_type(self, index, value): self.type_[index] = value
     def get_client_handler(self): return self.client_handler
     def set_client_handler(self, client_handler): self.client_handler = client_handler
     def add_client_handler(self, value): self.client_handler.append(value)
     def insert_client_handler(self, index, value): self.client_handler[index] = value
     def get_member_id(self): return self.member_id
     def set_member_id(self, member_id): self.member_id = member_id
+    def hasContent_(self):
+        if (
+            self.firstname is not None or
+            self.lastname is not None or
+            self.other_name is not None or
+            self.classxx is not None or
+            self.other_value or
+            self.type_ or
+            self.client_handler
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='booster', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='booster')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='booster'):
         if self.member_id is not None and 'member_id' not in already_processed:
-            already_processed.append('member_id')
+            already_processed.add('member_id')
             outfile.write(' member-id=%s' % (self.gds_format_string(quote_attrib(self.member_id).encode(ExternalEncoding), input_name='member-id'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='booster', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.firstname is not None:
@@ -1735,35 +1795,23 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sother-value>%s</%sother-value>%s' % (namespace_, self.gds_format_float(other_value_, input_name='other-value'), namespace_, eol_))
         for type_ in self.type_:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%stype>%s</%stype>%s' % (namespace_, self.gds_format_float(type_, input_name='type'), namespace_, eol_))
         for client_handler_ in self.client_handler:
             client_handler_.export(outfile, level, namespace_, name_='client-handler', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.firstname is not None or
-            self.lastname is not None or
-            self.other_name is not None or
-            self.classxx is not None or
-            self.other_value or
-            self.type_ or
-            self.client_handler
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='booster'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.member_id is not None and 'member_id' not in already_processed:
-            already_processed.append('member_id')
+            already_processed.add('member_id')
             showIndent(outfile, level)
             outfile.write('member_id = "%s",\n' % (self.member_id,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.firstname is not None:
             showIndent(outfile, level)
             outfile.write('firstname=%s,\n' % quote_python(self.firstname).encode(ExternalEncoding))
         if self.lastname is not None:
@@ -1802,22 +1850,23 @@
             client_handler_.exportLiteral(outfile, level, name_='client-handlerType')
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('member-id', node)
         if value is not None and 'member-id' not in already_processed:
-            already_processed.append('member-id')
+            already_processed.add('member-id')
             self.member_id = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'firstname':
             firstname_ = child_.text
             firstname_ = self.gds_validate_string(firstname_, node, 'firstname')
             self.firstname = firstname_
         elif nodeName_ == 'lastname':
@@ -1884,91 +1933,93 @@
     factory = staticmethod(factory)
     def get_rating(self): return self.rating
     def set_rating(self, rating): self.rating = rating
     def get_type(self): return self.type_
     def set_type(self, type_): self.type_ = type_
     def get_name(self): return self.name
     def set_name(self, name): self.name = name
+    def hasContent_(self):
+        if (
+
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='info', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='info')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='info'):
         if self.rating is not None and 'rating' not in already_processed:
-            already_processed.append('rating')
+            already_processed.add('rating')
             outfile.write(' rating="%s"' % self.gds_format_float(self.rating, input_name='rating'))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             outfile.write(' type="%s"' % self.gds_format_integer(self.type_, input_name='type'))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             outfile.write(' name=%s' % (self.gds_format_string(quote_attrib(self.name).encode(ExternalEncoding), input_name='name'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='info', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='info'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.rating is not None and 'rating' not in already_processed:
-            already_processed.append('rating')
+            already_processed.add('rating')
             showIndent(outfile, level)
             outfile.write('rating = %f,\n' % (self.rating,))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             showIndent(outfile, level)
             outfile.write('type_ = %d,\n' % (self.type_,))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             showIndent(outfile, level)
             outfile.write('name = "%s",\n' % (self.name,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('rating', node)
         if value is not None and 'rating' not in already_processed:
-            already_processed.append('rating')
+            already_processed.add('rating')
             try:
                 self.rating = float(value)
             except ValueError, exp:
                 raise ValueError('Bad float/double attribute (rating): %s' % exp)
         value = find_attr_value_('type', node)
         if value is not None and 'type' not in already_processed:
-            already_processed.append('type')
+            already_processed.add('type')
             try:
                 self.type_ = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('name', node)
         if value is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             self.name = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class info
 
 
 class vehicle(GeneratedsSuper):
@@ -1986,71 +2037,73 @@
         else:
             return vehicle(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_wheelcount(self): return self.wheelcount
     def set_wheelcount(self, wheelcount): self.wheelcount = wheelcount
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.wheelcount is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='vehicle', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='vehicle')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='vehicle'):
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
         pass
     def exportChildren(self, outfile, level, namespace_='', name_='vehicle', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.wheelcount is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%swheelcount>%s</%swheelcount>%s' % (namespace_, self.gds_format_integer(self.wheelcount, input_name='wheelcount'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.wheelcount is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='vehicle'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.wheelcount is not None:
             showIndent(outfile, level)
             outfile.write('wheelcount=%d,\n' % self.wheelcount)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'wheelcount':
             sval_ = child_.text
             try:
                 ival_ = int(sval_)
             except (TypeError, ValueError), exp:
@@ -2073,22 +2126,30 @@
         if automobile.subclass:
             return automobile.subclass(*args_, **kwargs_)
         else:
             return automobile(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_drivername(self): return self.drivername
     def set_drivername(self, drivername): self.drivername = drivername
+    def hasContent_(self):
+        if (
+            self.drivername is not None or
+            super(automobile, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='automobile', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='automobile')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2100,36 +2161,30 @@
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.drivername is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdrivername>%s</%sdrivername>%s' % (namespace_, self.gds_format_string(quote_xml(self.drivername).encode(ExternalEncoding), input_name='drivername'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.drivername is not None or
-            super(automobile, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='automobile'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(automobile, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(automobile, self).exportLiteralChildren(outfile, level, name_)
         if self.drivername is not None:
             showIndent(outfile, level)
             outfile.write('drivername=%s,\n' % quote_python(self.drivername).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(automobile, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'drivername':
@@ -2153,22 +2208,30 @@
         if airplane.subclass:
             return airplane.subclass(*args_, **kwargs_)
         else:
             return airplane(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_pilotname(self): return self.pilotname
     def set_pilotname(self, pilotname): self.pilotname = pilotname
+    def hasContent_(self):
+        if (
+            self.pilotname is not None or
+            super(airplane, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='airplane', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='airplane')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2180,36 +2243,30 @@
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.pilotname is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%spilotname>%s</%spilotname>%s' % (namespace_, self.gds_format_string(quote_xml(self.pilotname).encode(ExternalEncoding), input_name='pilotname'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.pilotname is not None or
-            super(airplane, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='airplane'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(airplane, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(airplane, self).exportLiteralChildren(outfile, level, name_)
         if self.pilotname is not None:
             showIndent(outfile, level)
             outfile.write('pilotname=%s,\n' % quote_python(self.pilotname).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(airplane, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'pilotname':
@@ -2305,52 +2362,70 @@
     def set_attrposint(self, attrposint): self.attrposint = attrposint
     def get_attrnonnegint(self): return self.attrnonnegint
     def set_attrnonnegint(self, attrnonnegint): self.attrnonnegint = attrnonnegint
     def get_attrnonposint(self): return self.attrnonposint
     def set_attrnonposint(self, attrnonposint): self.attrnonposint = attrnonposint
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.email is not None or
+            self.elposint is not None or
+            self.elnonposint is not None or
+            self.elnegint is not None or
+            self.elnonnegint is not None or
+            self.eldate is not None or
+            self.eltoken is not None or
+            self.elshort is not None or
+            self.ellong is not None or
+            self.elparam is not None or
+            self.elarraytypes is not None or
+            super(programmer, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='programmer', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='programmer')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='programmer'):
         super(programmer, self).exportAttributes(outfile, level, already_processed, namespace_, name_='programmer')
         if self.language is not None and 'language' not in already_processed:
-            already_processed.append('language')
+            already_processed.add('language')
             outfile.write(' language=%s' % (self.gds_format_string(quote_attrib(self.language).encode(ExternalEncoding), input_name='language'), ))
         if self.area is not None and 'area' not in already_processed:
-            already_processed.append('area')
+            already_processed.add('area')
             outfile.write(' area=%s' % (self.gds_format_string(quote_attrib(self.area).encode(ExternalEncoding), input_name='area'), ))
         if self.attrnegint is not None and 'attrnegint' not in already_processed:
-            already_processed.append('attrnegint')
+            already_processed.add('attrnegint')
             outfile.write(' attrnegint="%s"' % self.gds_format_integer(self.attrnegint, input_name='attrnegint'))
         if self.attrposint is not None and 'attrposint' not in already_processed:
-            already_processed.append('attrposint')
+            already_processed.add('attrposint')
             outfile.write(' attrposint="%s"' % self.gds_format_integer(self.attrposint, input_name='attrposint'))
         if self.attrnonnegint is not None and 'attrnonnegint' not in already_processed:
-            already_processed.append('attrnonnegint')
+            already_processed.add('attrnonnegint')
             outfile.write(' attrnonnegint="%s"' % self.gds_format_integer(self.attrnonnegint, input_name='attrnonnegint'))
         if self.attrnonposint is not None and 'attrnonposint' not in already_processed:
-            already_processed.append('attrnonposint')
+            already_processed.add('attrnonposint')
             outfile.write(' attrnonposint="%s"' % self.gds_format_integer(self.attrnonposint, input_name='attrnonposint'))
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
     def exportChildren(self, outfile, level, namespace_='', name_='programmer', fromsubclass_=False, pretty_print=True):
         super(programmer, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
@@ -2383,60 +2458,43 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sellong>%s</%sellong>%s' % (namespace_, self.gds_format_integer(self.ellong, input_name='ellong'), namespace_, eol_))
         if self.elparam is not None:
             self.elparam.export(outfile, level, namespace_, name_='elparam', pretty_print=pretty_print)
         if self.elarraytypes is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%selarraytypes>%s</%selarraytypes>%s' % (namespace_, self.gds_format_string(quote_xml(self.elarraytypes).encode(ExternalEncoding), input_name='elarraytypes'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.email is not None or
-            self.elposint is not None or
-            self.elnonposint is not None or
-            self.elnegint is not None or
-            self.elnonnegint is not None or
-            self.eldate is not None or
-            self.eltoken is not None or
-            self.elshort is not None or
-            self.ellong is not None or
-            self.elparam is not None or
-            self.elarraytypes is not None or
-            super(programmer, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='programmer'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.language is not None and 'language' not in already_processed:
-            already_processed.append('language')
+            already_processed.add('language')
             showIndent(outfile, level)
             outfile.write('language = "%s",\n' % (self.language,))
         if self.area is not None and 'area' not in already_processed:
-            already_processed.append('area')
+            already_processed.add('area')
             showIndent(outfile, level)
             outfile.write('area = "%s",\n' % (self.area,))
         if self.attrnegint is not None and 'attrnegint' not in already_processed:
-            already_processed.append('attrnegint')
+            already_processed.add('attrnegint')
             showIndent(outfile, level)
             outfile.write('attrnegint = %d,\n' % (self.attrnegint,))
         if self.attrposint is not None and 'attrposint' not in already_processed:
-            already_processed.append('attrposint')
+            already_processed.add('attrposint')
             showIndent(outfile, level)
             outfile.write('attrposint = %d,\n' % (self.attrposint,))
         if self.attrnonnegint is not None and 'attrnonnegint' not in already_processed:
-            already_processed.append('attrnonnegint')
+            already_processed.add('attrnonnegint')
             showIndent(outfile, level)
             outfile.write('attrnonnegint = %d,\n' % (self.attrnonnegint,))
         if self.attrnonposint is not None and 'attrnonposint' not in already_processed:
-            already_processed.append('attrnonposint')
+            already_processed.add('attrnonposint')
             showIndent(outfile, level)
             outfile.write('attrnonposint = %d,\n' % (self.attrnonposint,))
         super(programmer, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(programmer, self).exportLiteralChildren(outfile, level, name_)
         if self.email is not None:
             showIndent(outfile, level)
@@ -2471,66 +2529,67 @@
             self.elparam.exportLiteral(outfile, level, name_='elparam')
             showIndent(outfile, level)
             outfile.write('),\n')
         if self.elarraytypes is not None:
             showIndent(outfile, level)
             outfile.write('elarraytypes=%s,\n' % quote_python(self.elarraytypes).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('language', node)
         if value is not None and 'language' not in already_processed:
-            already_processed.append('language')
+            already_processed.add('language')
             self.language = value
         value = find_attr_value_('area', node)
         if value is not None and 'area' not in already_processed:
-            already_processed.append('area')
+            already_processed.add('area')
             self.area = value
         value = find_attr_value_('attrnegint', node)
         if value is not None and 'attrnegint' not in already_processed:
-            already_processed.append('attrnegint')
+            already_processed.add('attrnegint')
             try:
                 self.attrnegint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrnegint >= 0:
                 raise_parse_error(node, 'Invalid NegativeInteger')
         value = find_attr_value_('attrposint', node)
         if value is not None and 'attrposint' not in already_processed:
-            already_processed.append('attrposint')
+            already_processed.add('attrposint')
             try:
                 self.attrposint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrposint <= 0:
                 raise_parse_error(node, 'Invalid PositiveInteger')
         value = find_attr_value_('attrnonnegint', node)
         if value is not None and 'attrnonnegint' not in already_processed:
-            already_processed.append('attrnonnegint')
+            already_processed.add('attrnonnegint')
             try:
                 self.attrnonnegint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrnonnegint < 0:
                 raise_parse_error(node, 'Invalid NonNegativeInteger')
         value = find_attr_value_('attrnonposint', node)
         if value is not None and 'attrnonposint' not in already_processed:
-            already_processed.append('attrnonposint')
+            already_processed.add('attrnonposint')
             try:
                 self.attrnonposint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrnonposint > 0:
                 raise_parse_error(node, 'Invalid NonPositiveInteger')
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
         super(programmer, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'email':
             email_ = child_.text
             email_ = self.gds_validate_string(email_, node, 'email')
             self.email = email_
@@ -2628,22 +2687,30 @@
         else:
             return client_handlerType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_fullname(self): return self.fullname
     def set_fullname(self, fullname): self.fullname = fullname
     def get_refid(self): return self.refid
     def set_refid(self, refid): self.refid = refid
+    def hasContent_(self):
+        if (
+            self.fullname is not None or
+            self.refid is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='client-handlerType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='client-handlerType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2657,38 +2724,32 @@
             eol_ = ''
         if self.fullname is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfullname>%s</%sfullname>%s' % (namespace_, self.gds_format_string(quote_xml(self.fullname).encode(ExternalEncoding), input_name='fullname'), namespace_, eol_))
         if self.refid is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%srefid>%s</%srefid>%s' % (namespace_, self.gds_format_integer(self.refid, input_name='refid'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.fullname is not None or
-            self.refid is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='client-handlerType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.fullname is not None:
             showIndent(outfile, level)
             outfile.write('fullname=%s,\n' % quote_python(self.fullname).encode(ExternalEncoding))
         if self.refid is not None:
             showIndent(outfile, level)
             outfile.write('refid=%d,\n' % self.refid)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'fullname':
@@ -2730,88 +2791,90 @@
     factory = staticmethod(factory)
     def get_favorite_editor(self): return self.favorite_editor
     def set_favorite_editor(self, favorite_editor): self.favorite_editor = favorite_editor
     def get_status(self): return self.status
     def set_status(self, status): self.status = status
     def get_nick_name(self): return self.nick_name
     def set_nick_name(self, nick_name): self.nick_name = nick_name
+    def hasContent_(self):
+        if (
+            self.favorite_editor is not None or
+            super(java_programmer, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='java-programmer', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='java-programmer')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='java-programmer'):
         super(java_programmer, self).exportAttributes(outfile, level, already_processed, namespace_, name_='java-programmer')
         if self.status is not None and 'status' not in already_processed:
-            already_processed.append('status')
+            already_processed.add('status')
             outfile.write(' status=%s' % (self.gds_format_string(quote_attrib(self.status).encode(ExternalEncoding), input_name='status'), ))
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             outfile.write(' nick-name=%s' % (self.gds_format_string(quote_attrib(self.nick_name).encode(ExternalEncoding), input_name='nick-name'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='java-programmer', fromsubclass_=False, pretty_print=True):
         super(java_programmer, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.favorite_editor is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfavorite-editor>%s</%sfavorite-editor>%s' % (namespace_, self.gds_format_string(quote_xml(self.favorite_editor).encode(ExternalEncoding), input_name='favorite-editor'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.favorite_editor is not None or
-            super(java_programmer, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='java-programmer'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.status is not None and 'status' not in already_processed:
-            already_processed.append('status')
+            already_processed.add('status')
             showIndent(outfile, level)
             outfile.write('status = "%s",\n' % (self.status,))
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             showIndent(outfile, level)
             outfile.write('nick_name = "%s",\n' % (self.nick_name,))
         super(java_programmer, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(java_programmer, self).exportLiteralChildren(outfile, level, name_)
         if self.favorite_editor is not None:
             showIndent(outfile, level)
             outfile.write('favorite_editor=%s,\n' % quote_python(self.favorite_editor).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('status', node)
         if value is not None and 'status' not in already_processed:
-            already_processed.append('status')
+            already_processed.add('status')
             self.status = value
         value = find_attr_value_('nick-name', node)
         if value is not None and 'nick-name' not in already_processed:
-            already_processed.append('nick-name')
+            already_processed.add('nick-name')
             self.nick_name = value
         super(java_programmer, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'favorite-editor':
             favorite_editor_ = child_.text
             favorite_editor_ = self.gds_validate_string(favorite_editor_, node, 'favorite_editor')
             self.favorite_editor = favorite_editor_
@@ -2838,77 +2901,79 @@
         else:
             return python_programmer(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_favorite_editor(self): return self.favorite_editor
     def set_favorite_editor(self, favorite_editor): self.favorite_editor = favorite_editor
     def get_nick_name(self): return self.nick_name
     def set_nick_name(self, nick_name): self.nick_name = nick_name
+    def hasContent_(self):
+        if (
+            self.favorite_editor is not None or
+            super(python_programmer, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='python-programmer', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='python-programmer')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='python-programmer'):
         super(python_programmer, self).exportAttributes(outfile, level, already_processed, namespace_, name_='python-programmer')
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             outfile.write(' nick-name=%s' % (self.gds_format_string(quote_attrib(self.nick_name).encode(ExternalEncoding), input_name='nick-name'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='python-programmer', fromsubclass_=False, pretty_print=True):
         super(python_programmer, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.favorite_editor is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfavorite-editor>%s</%sfavorite-editor>%s' % (namespace_, self.gds_format_string(quote_xml(self.favorite_editor).encode(ExternalEncoding), input_name='favorite-editor'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.favorite_editor is not None or
-            super(python_programmer, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='python-programmer'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             showIndent(outfile, level)
             outfile.write('nick_name = "%s",\n' % (self.nick_name,))
         super(python_programmer, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(python_programmer, self).exportLiteralChildren(outfile, level, name_)
         if self.favorite_editor is not None:
             showIndent(outfile, level)
             outfile.write('favorite_editor=%s,\n' % quote_python(self.favorite_editor).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('nick-name', node)
         if value is not None and 'nick-name' not in already_processed:
-            already_processed.append('nick-name')
+            already_processed.add('nick-name')
             self.nick_name = value
         super(python_programmer, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'favorite-editor':
             favorite_editor_ = child_.text
             favorite_editor_ = self.gds_validate_string(favorite_editor_, node, 'favorite_editor')
             self.favorite_editor = favorite_editor_
@@ -2954,14 +3019,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'people'
+        rootClass = people
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'people'
```

### Comparing `generateDS-2.8b/tests/recursive_simpletype1_sup.py` & `generateDS-2.9a/tests/recursive_simpletype1_sup.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -498,22 +531,31 @@
     factory = staticmethod(factory)
     def get_personId(self): return self.personId
     def set_personId(self, personId): self.personId = personId
     def get_fname(self): return self.fname
     def set_fname(self, fname): self.fname = fname
     def get_lname(self): return self.lname
     def set_lname(self, lname): self.lname = lname
+    def hasContent_(self):
+        if (
+            self.personId is not None or
+            self.fname is not None or
+            self.lname is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='PersonType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='PersonType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -530,26 +572,18 @@
             outfile.write('<%spersonId>%s</%spersonId>%s' % (namespace_, self.gds_format_integer(self.personId, input_name='personId'), namespace_, eol_))
         if self.fname is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfname>%s</%sfname>%s' % (namespace_, self.gds_format_string(quote_xml(self.fname).encode(ExternalEncoding), input_name='fname'), namespace_, eol_))
         if self.lname is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%slname>%s</%slname>%s' % (namespace_, self.gds_format_string(quote_xml(self.lname).encode(ExternalEncoding), input_name='lname'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.personId is not None or
-            self.fname is not None or
-            self.lname is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='PersonType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.personId is not None:
             showIndent(outfile, level)
@@ -557,15 +591,16 @@
         if self.fname is not None:
             showIndent(outfile, level)
             outfile.write('fname=%s,\n' % quote_python(self.fname).encode(ExternalEncoding))
         if self.lname is not None:
             showIndent(outfile, level)
             outfile.write('lname=%s,\n' % quote_python(self.lname).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'personId':
@@ -623,14 +658,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'person'
+        rootClass = PersonType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'person'
```

### Comparing `generateDS-2.8b/tests/abstract_type.xsd` & `generateDS-2.9a/tests/abstract_type.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/people_procincl2_sub.py` & `generateDS-2.9a/tests/people_procincl2_sub.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,18 +204,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'people'
+        rootClass = supermod.people
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'people'
```

### Comparing `generateDS-2.8b/tests/anysimpletype.xsd` & `generateDS-2.9a/tests/anysimpletype.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/out1_sup.py` & `generateDS-2.9a/tests/out1_sup.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -531,22 +564,33 @@
     def set_python_programmer(self, python_programmer): self.python_programmer = python_programmer
     def add_python_programmer(self, value): self.python_programmer.append(value)
     def insert_python_programmer(self, index, value): self.python_programmer[index] = value
     def get_java_programmer(self): return self.java_programmer
     def set_java_programmer(self, java_programmer): self.java_programmer = java_programmer
     def add_java_programmer(self, value): self.java_programmer.append(value)
     def insert_java_programmer(self, index, value): self.java_programmer[index] = value
+    def hasContent_(self):
+        if (
+            self.comments or
+            self.person or
+            self.programmer or
+            self.python_programmer or
+            self.java_programmer
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='people', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='people')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -564,28 +608,18 @@
             person_.export(outfile, level, namespace_, name_='person', pretty_print=pretty_print)
         for programmer_ in self.programmer:
             programmer_.export(outfile, level, namespace_, name_='programmer', pretty_print=pretty_print)
         for python_programmer_ in self.python_programmer:
             python_programmer_.export(outfile, level, namespace_, name_='python-programmer', pretty_print=pretty_print)
         for java_programmer_ in self.java_programmer:
             java_programmer_.export(outfile, level, namespace_, name_='java-programmer', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.comments or
-            self.person or
-            self.programmer or
-            self.python_programmer or
-            self.java_programmer
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='people'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('comments=[\n')
@@ -644,15 +678,16 @@
             java_programmer_.exportLiteral(outfile, level, name_='java-programmer')
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'comments':
@@ -761,47 +796,48 @@
     factory = staticmethod(factory)
     def get_emp(self): return self.emp
     def set_emp(self, emp): self.emp = emp
     def add_emp(self, value): self.emp.append(value)
     def insert_emp(self, index, value): self.emp[index] = value
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.emp or
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='comments', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='comments')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='comments'):
         pass
     def exportChildren(self, outfile, level, namespace_='', name_='comments', fromsubclass_=False, pretty_print=True):
         if not fromsubclass_:
             for item_ in self.content_:
                 item_.export(outfile, level, item_.name, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.emp or
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='comments'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
@@ -809,15 +845,16 @@
         outfile.write('content_ = [\n')
         for item_ in self.content_:
             item_.exportLiteral(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('],\n')
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         if node.text is not None:
             obj_ = self.mixedclass_(MixedContainer.CategoryText,
                 MixedContainer.TypeNone, '', node.text)
             self.content_.append(obj_)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
@@ -953,48 +990,60 @@
     def set_ratio(self, ratio): self.ratio = ratio
     def get_id(self): return self.id
     def set_id(self, id): self.id = id
     def get_value(self): return self.value
     def set_value(self, value): self.value = value
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.interest or
+            self.category is not None or
+            self.agent or
+            self.promoter or
+            self.description is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='person', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='person')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='person'):
         if self.vegetable is not None and 'vegetable' not in already_processed:
-            already_processed.append('vegetable')
+            already_processed.add('vegetable')
             outfile.write(' vegetable=%s' % (self.gds_format_string(quote_attrib(self.vegetable).encode(ExternalEncoding), input_name='vegetable'), ))
         if self.fruit is not None and 'fruit' not in already_processed:
-            already_processed.append('fruit')
+            already_processed.add('fruit')
             outfile.write(' fruit=%s' % (self.gds_format_string(quote_attrib(self.fruit).encode(ExternalEncoding), input_name='fruit'), ))
         if self.ratio is not None and 'ratio' not in already_processed:
-            already_processed.append('ratio')
+            already_processed.add('ratio')
             outfile.write(' ratio="%s"' % self.gds_format_float(self.ratio, input_name='ratio'))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             outfile.write(' id="%s"' % self.gds_format_integer(self.id, input_name='id'))
         if self.value is not None and 'value' not in already_processed:
-            already_processed.append('value')
+            already_processed.add('value')
             outfile.write(' value=%s' % (self.gds_format_string(quote_attrib(self.value).encode(ExternalEncoding), input_name='value'), ))
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
     def exportChildren(self, outfile, level, namespace_='', name_='person', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
@@ -1010,50 +1059,39 @@
         for agent_ in self.agent:
             agent_.export(outfile, level, namespace_, name_='agent', pretty_print=pretty_print)
         for promoter_ in self.promoter:
             promoter_.export(outfile, level, namespace_, name_='promoter', pretty_print=pretty_print)
         if self.description is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdescription>%s</%sdescription>%s' % (namespace_, self.gds_format_string(quote_xml(self.description).encode(ExternalEncoding), input_name='description'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.interest or
-            self.category is not None or
-            self.agent or
-            self.promoter or
-            self.description is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='person'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.vegetable is not None and 'vegetable' not in already_processed:
-            already_processed.append('vegetable')
+            already_processed.add('vegetable')
             showIndent(outfile, level)
             outfile.write('vegetable = "%s",\n' % (self.vegetable,))
         if self.fruit is not None and 'fruit' not in already_processed:
-            already_processed.append('fruit')
+            already_processed.add('fruit')
             showIndent(outfile, level)
             outfile.write('fruit = "%s",\n' % (self.fruit,))
         if self.ratio is not None and 'ratio' not in already_processed:
-            already_processed.append('ratio')
+            already_processed.add('ratio')
             showIndent(outfile, level)
             outfile.write('ratio = %f,\n' % (self.ratio,))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             showIndent(outfile, level)
             outfile.write('id = %d,\n' % (self.id,))
         if self.value is not None and 'value' not in already_processed:
-            already_processed.append('value')
+            already_processed.add('value')
             showIndent(outfile, level)
             outfile.write('value = "%s",\n' % (self.value,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
             outfile.write('name=%s,\n' % quote_python(self.name).encode(ExternalEncoding))
         showIndent(outfile, level)
@@ -1092,48 +1130,49 @@
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
         if self.description is not None:
             showIndent(outfile, level)
             outfile.write('description=%s,\n' % quote_python(self.description).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('vegetable', node)
         if value is not None and 'vegetable' not in already_processed:
-            already_processed.append('vegetable')
+            already_processed.add('vegetable')
             self.vegetable = value
         value = find_attr_value_('fruit', node)
         if value is not None and 'fruit' not in already_processed:
-            already_processed.append('fruit')
+            already_processed.add('fruit')
             self.fruit = value
         value = find_attr_value_('ratio', node)
         if value is not None and 'ratio' not in already_processed:
-            already_processed.append('ratio')
+            already_processed.add('ratio')
             try:
                 self.ratio = float(value)
             except ValueError, exp:
                 raise ValueError('Bad float/double attribute (ratio): %s' % exp)
         value = find_attr_value_('id', node)
         if value is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             try:
                 self.id = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('value', node)
         if value is not None and 'value' not in already_processed:
-            already_processed.append('value')
+            already_processed.add('value')
             self.value = value
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
             name_ = child_.text
             name_ = self.gds_validate_string(name_, node, 'name')
             self.name = name_
         elif nodeName_ == 'interest':
@@ -1296,52 +1335,71 @@
     def set_attrposint(self, attrposint): self.attrposint = attrposint
     def get_attrnonnegint(self): return self.attrnonnegint
     def set_attrnonnegint(self, attrnonnegint): self.attrnonnegint = attrnonnegint
     def get_attrnonposint(self): return self.attrnonposint
     def set_attrnonposint(self, attrnonposint): self.attrnonposint = attrnonposint
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.email is not None or
+            self.elposint is not None or
+            self.elnonposint is not None or
+            self.elnegint is not None or
+            self.elnonnegint is not None or
+            self.eldate is not None or
+            self.eldatetime is not None or
+            self.eltoken is not None or
+            self.elshort is not None or
+            self.ellong is not None or
+            self.elparam is not None or
+            self.elarraytypes is not None or
+            super(programmer, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='programmer', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='programmer')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='programmer'):
         super(programmer, self).exportAttributes(outfile, level, already_processed, namespace_, name_='programmer')
         if self.language is not None and 'language' not in already_processed:
-            already_processed.append('language')
+            already_processed.add('language')
             outfile.write(' language=%s' % (self.gds_format_string(quote_attrib(self.language).encode(ExternalEncoding), input_name='language'), ))
         if self.area is not None and 'area' not in already_processed:
-            already_processed.append('area')
+            already_processed.add('area')
             outfile.write(' area=%s' % (self.gds_format_string(quote_attrib(self.area).encode(ExternalEncoding), input_name='area'), ))
         if self.attrnegint is not None and 'attrnegint' not in already_processed:
-            already_processed.append('attrnegint')
+            already_processed.add('attrnegint')
             outfile.write(' attrnegint="%s"' % self.gds_format_integer(self.attrnegint, input_name='attrnegint'))
         if self.attrposint is not None and 'attrposint' not in already_processed:
-            already_processed.append('attrposint')
+            already_processed.add('attrposint')
             outfile.write(' attrposint="%s"' % self.gds_format_integer(self.attrposint, input_name='attrposint'))
         if self.attrnonnegint is not None and 'attrnonnegint' not in already_processed:
-            already_processed.append('attrnonnegint')
+            already_processed.add('attrnonnegint')
             outfile.write(' attrnonnegint="%s"' % self.gds_format_integer(self.attrnonnegint, input_name='attrnonnegint'))
         if self.attrnonposint is not None and 'attrnonposint' not in already_processed:
-            already_processed.append('attrnonposint')
+            already_processed.add('attrnonposint')
             outfile.write(' attrnonposint="%s"' % self.gds_format_integer(self.attrnonposint, input_name='attrnonposint'))
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
     def exportChildren(self, outfile, level, namespace_='', name_='programmer', fromsubclass_=False, pretty_print=True):
         super(programmer, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
@@ -1377,61 +1435,43 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sellong>%s</%sellong>%s' % (namespace_, self.gds_format_integer(self.ellong, input_name='ellong'), namespace_, eol_))
         if self.elparam is not None:
             self.elparam.export(outfile, level, namespace_, name_='elparam', pretty_print=pretty_print)
         if self.elarraytypes is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%selarraytypes>%s</%selarraytypes>%s' % (namespace_, self.gds_format_string(quote_xml(self.elarraytypes).encode(ExternalEncoding), input_name='elarraytypes'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.email is not None or
-            self.elposint is not None or
-            self.elnonposint is not None or
-            self.elnegint is not None or
-            self.elnonnegint is not None or
-            self.eldate is not None or
-            self.eldatetime is not None or
-            self.eltoken is not None or
-            self.elshort is not None or
-            self.ellong is not None or
-            self.elparam is not None or
-            self.elarraytypes is not None or
-            super(programmer, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='programmer'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.language is not None and 'language' not in already_processed:
-            already_processed.append('language')
+            already_processed.add('language')
             showIndent(outfile, level)
             outfile.write('language = "%s",\n' % (self.language,))
         if self.area is not None and 'area' not in already_processed:
-            already_processed.append('area')
+            already_processed.add('area')
             showIndent(outfile, level)
             outfile.write('area = "%s",\n' % (self.area,))
         if self.attrnegint is not None and 'attrnegint' not in already_processed:
-            already_processed.append('attrnegint')
+            already_processed.add('attrnegint')
             showIndent(outfile, level)
             outfile.write('attrnegint = %d,\n' % (self.attrnegint,))
         if self.attrposint is not None and 'attrposint' not in already_processed:
-            already_processed.append('attrposint')
+            already_processed.add('attrposint')
             showIndent(outfile, level)
             outfile.write('attrposint = %d,\n' % (self.attrposint,))
         if self.attrnonnegint is not None and 'attrnonnegint' not in already_processed:
-            already_processed.append('attrnonnegint')
+            already_processed.add('attrnonnegint')
             showIndent(outfile, level)
             outfile.write('attrnonnegint = %d,\n' % (self.attrnonnegint,))
         if self.attrnonposint is not None and 'attrnonposint' not in already_processed:
-            already_processed.append('attrnonposint')
+            already_processed.add('attrnonposint')
             showIndent(outfile, level)
             outfile.write('attrnonposint = %d,\n' % (self.attrnonposint,))
         super(programmer, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(programmer, self).exportLiteralChildren(outfile, level, name_)
         if self.email is not None:
             showIndent(outfile, level)
@@ -1469,66 +1509,67 @@
             self.elparam.exportLiteral(outfile, level, name_='elparam')
             showIndent(outfile, level)
             outfile.write('),\n')
         if self.elarraytypes is not None:
             showIndent(outfile, level)
             outfile.write('elarraytypes=%s,\n' % quote_python(self.elarraytypes).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('language', node)
         if value is not None and 'language' not in already_processed:
-            already_processed.append('language')
+            already_processed.add('language')
             self.language = value
         value = find_attr_value_('area', node)
         if value is not None and 'area' not in already_processed:
-            already_processed.append('area')
+            already_processed.add('area')
             self.area = value
         value = find_attr_value_('attrnegint', node)
         if value is not None and 'attrnegint' not in already_processed:
-            already_processed.append('attrnegint')
+            already_processed.add('attrnegint')
             try:
                 self.attrnegint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrnegint >= 0:
                 raise_parse_error(node, 'Invalid NegativeInteger')
         value = find_attr_value_('attrposint', node)
         if value is not None and 'attrposint' not in already_processed:
-            already_processed.append('attrposint')
+            already_processed.add('attrposint')
             try:
                 self.attrposint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrposint <= 0:
                 raise_parse_error(node, 'Invalid PositiveInteger')
         value = find_attr_value_('attrnonnegint', node)
         if value is not None and 'attrnonnegint' not in already_processed:
-            already_processed.append('attrnonnegint')
+            already_processed.add('attrnonnegint')
             try:
                 self.attrnonnegint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrnonnegint < 0:
                 raise_parse_error(node, 'Invalid NonNegativeInteger')
         value = find_attr_value_('attrnonposint', node)
         if value is not None and 'attrnonposint' not in already_processed:
-            already_processed.append('attrnonposint')
+            already_processed.add('attrnonposint')
             try:
                 self.attrnonposint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrnonposint > 0:
                 raise_parse_error(node, 'Invalid NonPositiveInteger')
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
         super(programmer, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'email':
             email_ = child_.text
             email_ = self.gds_validate_string(email_, node, 'email')
             self.email = email_
@@ -1698,123 +1739,125 @@
     def set_sid(self, sid): self.sid = sid
     def get_type(self): return self.type_
     def set_type(self, type_): self.type_ = type_
     def get_id(self): return self.id
     def set_id(self, id): self.id = id
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='param', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='param')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='param'):
         if self.semantic is not None and 'semantic' not in already_processed:
-            already_processed.append('semantic')
+            already_processed.add('semantic')
             outfile.write(' semantic=%s' % (self.gds_format_string(quote_attrib(self.semantic).encode(ExternalEncoding), input_name='semantic'), ))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             outfile.write(' name=%s' % (quote_attrib(self.name), ))
         if self.flow is not None and 'flow' not in already_processed:
-            already_processed.append('flow')
+            already_processed.add('flow')
             outfile.write(' flow=%s' % (quote_attrib(self.flow), ))
         if self.sid is not None and 'sid' not in already_processed:
-            already_processed.append('sid')
+            already_processed.add('sid')
             outfile.write(' sid=%s' % (quote_attrib(self.sid), ))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             outfile.write(' type=%s' % (self.gds_format_string(quote_attrib(self.type_).encode(ExternalEncoding), input_name='type'), ))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             outfile.write(' id=%s' % (self.gds_format_string(quote_attrib(self.id).encode(ExternalEncoding), input_name='id'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='param', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='param'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.semantic is not None and 'semantic' not in already_processed:
-            already_processed.append('semantic')
+            already_processed.add('semantic')
             showIndent(outfile, level)
             outfile.write('semantic = "%s",\n' % (self.semantic,))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             showIndent(outfile, level)
             outfile.write('name = "%s",\n' % (self.name,))
         if self.flow is not None and 'flow' not in already_processed:
-            already_processed.append('flow')
+            already_processed.add('flow')
             showIndent(outfile, level)
             outfile.write('flow = %s,\n' % (self.flow,))
         if self.sid is not None and 'sid' not in already_processed:
-            already_processed.append('sid')
+            already_processed.add('sid')
             showIndent(outfile, level)
             outfile.write('sid = "%s",\n' % (self.sid,))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             showIndent(outfile, level)
             outfile.write('type_ = "%s",\n' % (self.type_,))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             showIndent(outfile, level)
             outfile.write('id = "%s",\n' % (self.id,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('semantic', node)
         if value is not None and 'semantic' not in already_processed:
-            already_processed.append('semantic')
+            already_processed.add('semantic')
             self.semantic = value
             self.semantic = ' '.join(self.semantic.split())
         value = find_attr_value_('name', node)
         if value is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             self.name = value
         value = find_attr_value_('flow', node)
         if value is not None and 'flow' not in already_processed:
-            already_processed.append('flow')
+            already_processed.add('flow')
             self.flow = value
         value = find_attr_value_('sid', node)
         if value is not None and 'sid' not in already_processed:
-            already_processed.append('sid')
+            already_processed.add('sid')
             self.sid = value
         value = find_attr_value_('type', node)
         if value is not None and 'type' not in already_processed:
-            already_processed.append('type')
+            already_processed.add('type')
             self.type_ = value
         value = find_attr_value_('id', node)
         if value is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             self.id = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
     def walk_and_update(self):
         members = param._member_data_items
         for member in members:
             obj1 = getattr(self, member.get_name())
@@ -1880,77 +1923,79 @@
         else:
             return python_programmer(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_favorite_editor(self): return self.favorite_editor
     def set_favorite_editor(self, favorite_editor): self.favorite_editor = favorite_editor
     def get_nick_name(self): return self.nick_name
     def set_nick_name(self, nick_name): self.nick_name = nick_name
+    def hasContent_(self):
+        if (
+            self.favorite_editor is not None or
+            super(python_programmer, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='python-programmer', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='python-programmer')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='python-programmer'):
         super(python_programmer, self).exportAttributes(outfile, level, already_processed, namespace_, name_='python-programmer')
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             outfile.write(' nick-name=%s' % (self.gds_format_string(quote_attrib(self.nick_name).encode(ExternalEncoding), input_name='nick-name'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='python-programmer', fromsubclass_=False, pretty_print=True):
         super(python_programmer, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.favorite_editor is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfavorite-editor>%s</%sfavorite-editor>%s' % (namespace_, self.gds_format_string(quote_xml(self.favorite_editor).encode(ExternalEncoding), input_name='favorite-editor'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.favorite_editor is not None or
-            super(python_programmer, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='python-programmer'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             showIndent(outfile, level)
             outfile.write('nick_name = "%s",\n' % (self.nick_name,))
         super(python_programmer, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(python_programmer, self).exportLiteralChildren(outfile, level, name_)
         if self.favorite_editor is not None:
             showIndent(outfile, level)
             outfile.write('favorite_editor=%s,\n' % quote_python(self.favorite_editor).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('nick-name', node)
         if value is not None and 'nick-name' not in already_processed:
-            already_processed.append('nick-name')
+            already_processed.add('nick-name')
             self.nick_name = value
         super(python_programmer, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'favorite-editor':
             favorite_editor_ = child_.text
             favorite_editor_ = self.gds_validate_string(favorite_editor_, node, 'favorite_editor')
             self.favorite_editor = favorite_editor_
@@ -2025,88 +2070,90 @@
     factory = staticmethod(factory)
     def get_favorite_editor(self): return self.favorite_editor
     def set_favorite_editor(self, favorite_editor): self.favorite_editor = favorite_editor
     def get_status(self): return self.status
     def set_status(self, status): self.status = status
     def get_nick_name(self): return self.nick_name
     def set_nick_name(self, nick_name): self.nick_name = nick_name
+    def hasContent_(self):
+        if (
+            self.favorite_editor is not None or
+            super(java_programmer, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='java-programmer', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='java-programmer')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='java-programmer'):
         super(java_programmer, self).exportAttributes(outfile, level, already_processed, namespace_, name_='java-programmer')
         if self.status is not None and 'status' not in already_processed:
-            already_processed.append('status')
+            already_processed.add('status')
             outfile.write(' status=%s' % (self.gds_format_string(quote_attrib(self.status).encode(ExternalEncoding), input_name='status'), ))
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             outfile.write(' nick-name=%s' % (self.gds_format_string(quote_attrib(self.nick_name).encode(ExternalEncoding), input_name='nick-name'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='java-programmer', fromsubclass_=False, pretty_print=True):
         super(java_programmer, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.favorite_editor is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfavorite-editor>%s</%sfavorite-editor>%s' % (namespace_, self.gds_format_string(quote_xml(self.favorite_editor).encode(ExternalEncoding), input_name='favorite-editor'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.favorite_editor is not None or
-            super(java_programmer, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='java-programmer'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.status is not None and 'status' not in already_processed:
-            already_processed.append('status')
+            already_processed.add('status')
             showIndent(outfile, level)
             outfile.write('status = "%s",\n' % (self.status,))
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             showIndent(outfile, level)
             outfile.write('nick_name = "%s",\n' % (self.nick_name,))
         super(java_programmer, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(java_programmer, self).exportLiteralChildren(outfile, level, name_)
         if self.favorite_editor is not None:
             showIndent(outfile, level)
             outfile.write('favorite_editor=%s,\n' % quote_python(self.favorite_editor).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('status', node)
         if value is not None and 'status' not in already_processed:
-            already_processed.append('status')
+            already_processed.add('status')
             self.status = value
         value = find_attr_value_('nick-name', node)
         if value is not None and 'nick-name' not in already_processed:
-            already_processed.append('nick-name')
+            already_processed.add('nick-name')
             self.nick_name = value
         super(java_programmer, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'favorite-editor':
             favorite_editor_ = child_.text
             favorite_editor_ = self.gds_validate_string(favorite_editor_, node, 'favorite_editor')
             self.favorite_editor = favorite_editor_
@@ -2184,22 +2231,32 @@
     def set_firstname(self, firstname): self.firstname = firstname
     def get_lastname(self): return self.lastname
     def set_lastname(self, lastname): self.lastname = lastname
     def get_priority(self): return self.priority
     def set_priority(self, priority): self.priority = priority
     def get_info(self): return self.info
     def set_info(self, info): self.info = info
+    def hasContent_(self):
+        if (
+            self.firstname is not None or
+            self.lastname is not None or
+            self.priority is not None or
+            self.info is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='agent', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='agent')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2218,27 +2275,18 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%slastname>%s</%slastname>%s' % (namespace_, self.gds_format_string(quote_xml(self.lastname).encode(ExternalEncoding), input_name='lastname'), namespace_, eol_))
         if self.priority is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%spriority>%s</%spriority>%s' % (namespace_, self.gds_format_float(self.priority, input_name='priority'), namespace_, eol_))
         if self.info is not None:
             self.info.export(outfile, level, namespace_, name_='info', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.firstname is not None or
-            self.lastname is not None or
-            self.priority is not None or
-            self.info is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='agent'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.firstname is not None:
             showIndent(outfile, level)
@@ -2252,15 +2300,16 @@
         if self.info is not None:
             showIndent(outfile, level)
             outfile.write('info=model_.info(\n')
             self.info.exportLiteral(outfile, level)
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'firstname':
@@ -2356,22 +2405,32 @@
     def set_firstname(self, firstname): self.firstname = firstname
     def get_lastname(self): return self.lastname
     def set_lastname(self, lastname): self.lastname = lastname
     def get_priority(self): return self.priority
     def set_priority(self, priority): self.priority = priority
     def get_info(self): return self.info
     def set_info(self, info): self.info = info
+    def hasContent_(self):
+        if (
+            self.firstname is not None or
+            self.lastname is not None or
+            self.priority is not None or
+            self.info is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='special-agent', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='special-agent')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2390,27 +2449,18 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%slastname>%s</%slastname>%s' % (namespace_, self.gds_format_string(quote_xml(self.lastname).encode(ExternalEncoding), input_name='lastname'), namespace_, eol_))
         if self.priority is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%spriority>%s</%spriority>%s' % (namespace_, self.gds_format_float(self.priority, input_name='priority'), namespace_, eol_))
         if self.info is not None:
             self.info.export(outfile, level, namespace_, name_='info', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.firstname is not None or
-            self.lastname is not None or
-            self.priority is not None or
-            self.info is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='special-agent'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.firstname is not None:
             showIndent(outfile, level)
@@ -2424,15 +2474,16 @@
         if self.info is not None:
             showIndent(outfile, level)
             outfile.write('info=model_.info(\n')
             self.info.exportLiteral(outfile, level)
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'firstname':
@@ -2555,22 +2606,35 @@
     def set_type(self, type_): self.type_ = type_
     def add_type(self, value): self.type_.append(value)
     def insert_type(self, index, value): self.type_[index] = value
     def get_client_handler(self): return self.client_handler
     def set_client_handler(self, client_handler): self.client_handler = client_handler
     def add_client_handler(self, value): self.client_handler.append(value)
     def insert_client_handler(self, index, value): self.client_handler[index] = value
+    def hasContent_(self):
+        if (
+            self.firstname is not None or
+            self.lastname is not None or
+            self.other_name is not None or
+            self.classxx is not None or
+            self.other_value or
+            self.type_ or
+            self.client_handler
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='booster', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='booster')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2598,30 +2662,18 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sother-value>%s</%sother-value>%s' % (namespace_, self.gds_format_float(other_value_, input_name='other-value'), namespace_, eol_))
         for type_ in self.type_:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%stype>%s</%stype>%s' % (namespace_, self.gds_format_float(type_, input_name='type'), namespace_, eol_))
         for client_handler_ in self.client_handler:
             client_handler_.export(outfile, level, namespace_, name_='client-handler', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.firstname is not None or
-            self.lastname is not None or
-            self.other_name is not None or
-            self.classxx is not None or
-            self.other_value or
-            self.type_ or
-            self.client_handler
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='booster'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.firstname is not None:
             showIndent(outfile, level)
@@ -2662,15 +2714,16 @@
             client_handler_.exportLiteral(outfile, level, name_='client-handlerType')
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'firstname':
@@ -2787,91 +2840,93 @@
     factory = staticmethod(factory)
     def get_rating(self): return self.rating
     def set_rating(self, rating): self.rating = rating
     def get_type(self): return self.type_
     def set_type(self, type_): self.type_ = type_
     def get_name(self): return self.name
     def set_name(self, name): self.name = name
+    def hasContent_(self):
+        if (
+
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='info', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='info')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='info'):
         if self.rating is not None and 'rating' not in already_processed:
-            already_processed.append('rating')
+            already_processed.add('rating')
             outfile.write(' rating="%s"' % self.gds_format_float(self.rating, input_name='rating'))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             outfile.write(' type="%s"' % self.gds_format_integer(self.type_, input_name='type'))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             outfile.write(' name=%s' % (self.gds_format_string(quote_attrib(self.name).encode(ExternalEncoding), input_name='name'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='info', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='info'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.rating is not None and 'rating' not in already_processed:
-            already_processed.append('rating')
+            already_processed.add('rating')
             showIndent(outfile, level)
             outfile.write('rating = %f,\n' % (self.rating,))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             showIndent(outfile, level)
             outfile.write('type_ = %d,\n' % (self.type_,))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             showIndent(outfile, level)
             outfile.write('name = "%s",\n' % (self.name,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('rating', node)
         if value is not None and 'rating' not in already_processed:
-            already_processed.append('rating')
+            already_processed.add('rating')
             try:
                 self.rating = float(value)
             except ValueError, exp:
                 raise ValueError('Bad float/double attribute (rating): %s' % exp)
         value = find_attr_value_('type', node)
         if value is not None and 'type' not in already_processed:
-            already_processed.append('type')
+            already_processed.add('type')
             try:
                 self.type_ = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('name', node)
         if value is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             self.name = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
     def walk_and_update(self):
         members = info._member_data_items
         for member in members:
             obj1 = getattr(self, member.get_name())
@@ -2936,22 +2991,30 @@
         else:
             return client_handlerType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_fullname(self): return self.fullname
     def set_fullname(self, fullname): self.fullname = fullname
     def get_refid(self): return self.refid
     def set_refid(self, refid): self.refid = refid
+    def hasContent_(self):
+        if (
+            self.fullname is not None or
+            self.refid is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='client-handlerType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='client-handlerType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2965,38 +3028,32 @@
             eol_ = ''
         if self.fullname is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfullname>%s</%sfullname>%s' % (namespace_, self.gds_format_string(quote_xml(self.fullname).encode(ExternalEncoding), input_name='fullname'), namespace_, eol_))
         if self.refid is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%srefid>%s</%srefid>%s' % (namespace_, self.gds_format_integer(self.refid, input_name='refid'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.fullname is not None or
-            self.refid is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='client-handlerType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.fullname is not None:
             showIndent(outfile, level)
             outfile.write('fullname=%s,\n' % quote_python(self.fullname).encode(ExternalEncoding))
         if self.refid is not None:
             showIndent(outfile, level)
             outfile.write('refid=%d,\n' % self.refid)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'fullname':
@@ -3098,14 +3155,33 @@
     sys.stdout.write('<?xml version="1.0" ?>\n')
     rootObj.export(sys.stdout, 0, name_=rootTag,
         namespacedef_='',
         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'people'
+        rootClass = people
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+    content = etree_.tostring(rootElement, pretty_print=True,
+        xml_declaration=True, encoding="utf-8")
+    sys.stdout.write(content)
+    sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'people'
```

### Comparing `generateDS-2.8b/tests/people_procincl2_sup.py` & `generateDS-2.9a/tests/people_procincl2_sup.py`

 * *Files 12% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -541,22 +574,34 @@
     def set_python_programmer(self, python_programmer): self.python_programmer = python_programmer
     def add_python_programmer(self, value): self.python_programmer.append(value)
     def insert_python_programmer(self, index, value): self.python_programmer[index] = value
     def get_java_programmer(self): return self.java_programmer
     def set_java_programmer(self, java_programmer): self.java_programmer = java_programmer
     def add_java_programmer(self, value): self.java_programmer.append(value)
     def insert_java_programmer(self, index, value): self.java_programmer[index] = value
+    def hasContent_(self):
+        if (
+            self.comments or
+            self.person or
+            self.specialperson or
+            self.programmer or
+            self.python_programmer or
+            self.java_programmer
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='people', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='people')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -576,29 +621,18 @@
             specialperson_.export(outfile, level, namespace_, name_='specialperson', pretty_print=pretty_print)
         for programmer_ in self.programmer:
             programmer_.export(outfile, level, namespace_, name_='programmer', pretty_print=pretty_print)
         for python_programmer_ in self.python_programmer:
             python_programmer_.export(outfile, level, namespace_, name_='python-programmer', pretty_print=pretty_print)
         for java_programmer_ in self.java_programmer:
             java_programmer_.export(outfile, level, namespace_, name_='java-programmer', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.comments or
-            self.person or
-            self.specialperson or
-            self.programmer or
-            self.python_programmer or
-            self.java_programmer
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='people'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('comments=[\n')
@@ -669,15 +703,16 @@
             java_programmer_.exportLiteral(outfile, level, name_='java-programmer')
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'comments':
@@ -748,48 +783,49 @@
     def insert_emp(self, index, value): self.emp[index] = value
     def get_bold(self): return self.bold
     def set_bold(self, bold): self.bold = bold
     def add_bold(self, value): self.bold.append(value)
     def insert_bold(self, index, value): self.bold[index] = value
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.emp or
+            self.bold or
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='comments', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='comments')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='comments'):
         pass
     def exportChildren(self, outfile, level, namespace_='', name_='comments', fromsubclass_=False, pretty_print=True):
         if not fromsubclass_:
             for item_ in self.content_:
                 item_.export(outfile, level, item_.name, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.emp or
-            self.bold or
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='comments'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
@@ -803,15 +839,16 @@
         outfile.write('content_ = [\n')
         for item_ in self.content_:
             item_.exportLiteral(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('],\n')
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         if node.text is not None:
             obj_ = self.mixedclass_(MixedContainer.CategoryText,
                 MixedContainer.TypeNone, '', node.text)
             self.content_.append(obj_)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
@@ -909,48 +946,60 @@
     def set_ratio(self, ratio): self.ratio = ratio
     def get_id(self): return self.id
     def set_id(self, id): self.id = id
     def get_value(self): return self.value
     def set_value(self, value): self.value = value
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.interest or
+            self.category is not None or
+            self.agent or
+            self.promoter or
+            self.description is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='person', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='person')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='person'):
         if self.vegetable is not None and 'vegetable' not in already_processed:
-            already_processed.append('vegetable')
+            already_processed.add('vegetable')
             outfile.write(' vegetable=%s' % (self.gds_format_string(quote_attrib(self.vegetable).encode(ExternalEncoding), input_name='vegetable'), ))
         if self.fruit is not None and 'fruit' not in already_processed:
-            already_processed.append('fruit')
+            already_processed.add('fruit')
             outfile.write(' fruit=%s' % (self.gds_format_string(quote_attrib(self.fruit).encode(ExternalEncoding), input_name='fruit'), ))
         if self.ratio is not None and 'ratio' not in already_processed:
-            already_processed.append('ratio')
+            already_processed.add('ratio')
             outfile.write(' ratio="%s"' % self.gds_format_float(self.ratio, input_name='ratio'))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             outfile.write(' id="%s"' % self.gds_format_integer(self.id, input_name='id'))
         if self.value is not None and 'value' not in already_processed:
-            already_processed.append('value')
+            already_processed.add('value')
             outfile.write(' value=%s' % (self.gds_format_string(quote_attrib(self.value).encode(ExternalEncoding), input_name='value'), ))
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
     def exportChildren(self, outfile, level, namespace_='', name_='person', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
@@ -966,50 +1015,39 @@
         for agent_ in self.agent:
             agent_.export(outfile, level, namespace_, name_='agent', pretty_print=pretty_print)
         for promoter_ in self.promoter:
             promoter_.export(outfile, level, namespace_, name_='promoter', pretty_print=pretty_print)
         if self.description is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdescription>%s</%sdescription>%s' % (namespace_, self.gds_format_string(quote_xml(self.description).encode(ExternalEncoding), input_name='description'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.interest or
-            self.category is not None or
-            self.agent or
-            self.promoter or
-            self.description is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='person'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.vegetable is not None and 'vegetable' not in already_processed:
-            already_processed.append('vegetable')
+            already_processed.add('vegetable')
             showIndent(outfile, level)
             outfile.write('vegetable = "%s",\n' % (self.vegetable,))
         if self.fruit is not None and 'fruit' not in already_processed:
-            already_processed.append('fruit')
+            already_processed.add('fruit')
             showIndent(outfile, level)
             outfile.write('fruit = "%s",\n' % (self.fruit,))
         if self.ratio is not None and 'ratio' not in already_processed:
-            already_processed.append('ratio')
+            already_processed.add('ratio')
             showIndent(outfile, level)
             outfile.write('ratio = %f,\n' % (self.ratio,))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             showIndent(outfile, level)
             outfile.write('id = %d,\n' % (self.id,))
         if self.value is not None and 'value' not in already_processed:
-            already_processed.append('value')
+            already_processed.add('value')
             showIndent(outfile, level)
             outfile.write('value = "%s",\n' % (self.value,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
             outfile.write('name=%s,\n' % quote_python(self.name).encode(ExternalEncoding))
         showIndent(outfile, level)
@@ -1048,48 +1086,49 @@
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
         if self.description is not None:
             showIndent(outfile, level)
             outfile.write('description=%s,\n' % quote_python(self.description).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('vegetable', node)
         if value is not None and 'vegetable' not in already_processed:
-            already_processed.append('vegetable')
+            already_processed.add('vegetable')
             self.vegetable = value
         value = find_attr_value_('fruit', node)
         if value is not None and 'fruit' not in already_processed:
-            already_processed.append('fruit')
+            already_processed.add('fruit')
             self.fruit = value
         value = find_attr_value_('ratio', node)
         if value is not None and 'ratio' not in already_processed:
-            already_processed.append('ratio')
+            already_processed.add('ratio')
             try:
                 self.ratio = float(value)
             except ValueError, exp:
                 raise ValueError('Bad float/double attribute (ratio): %s' % exp)
         value = find_attr_value_('id', node)
         if value is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             try:
                 self.id = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('value', node)
         if value is not None and 'value' not in already_processed:
-            already_processed.append('value')
+            already_processed.add('value')
             self.value = value
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
             name_ = child_.text
             name_ = self.gds_validate_string(name_, node, 'name')
             self.name = name_
         elif nodeName_ == 'interest':
@@ -1129,52 +1168,54 @@
         pass
     def factory(*args_, **kwargs_):
         if specialperson.subclass:
             return specialperson.subclass(*args_, **kwargs_)
         else:
             return specialperson(*args_, **kwargs_)
     factory = staticmethod(factory)
+    def hasContent_(self):
+        if (
+            super(specialperson, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='specialperson', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='specialperson')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='specialperson'):
         super(specialperson, self).exportAttributes(outfile, level, already_processed, namespace_, name_='specialperson')
     def exportChildren(self, outfile, level, namespace_='', name_='specialperson', fromsubclass_=False, pretty_print=True):
         super(specialperson, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            super(specialperson, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='specialperson'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(specialperson, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(specialperson, self).exportLiteralChildren(outfile, level, name_)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(specialperson, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         super(specialperson, self).buildChildren(child_, node, nodeName_, True)
@@ -1220,123 +1261,125 @@
     def set_sid(self, sid): self.sid = sid
     def get_type(self): return self.type_
     def set_type(self, type_): self.type_ = type_
     def get_id(self): return self.id
     def set_id(self, id): self.id = id
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='param', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='param')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='param'):
         if self.semantic is not None and 'semantic' not in already_processed:
-            already_processed.append('semantic')
+            already_processed.add('semantic')
             outfile.write(' semantic=%s' % (self.gds_format_string(quote_attrib(self.semantic).encode(ExternalEncoding), input_name='semantic'), ))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             outfile.write(' name=%s' % (quote_attrib(self.name), ))
         if self.flow is not None and 'flow' not in already_processed:
-            already_processed.append('flow')
+            already_processed.add('flow')
             outfile.write(' flow=%s' % (quote_attrib(self.flow), ))
         if self.sid is not None and 'sid' not in already_processed:
-            already_processed.append('sid')
+            already_processed.add('sid')
             outfile.write(' sid=%s' % (quote_attrib(self.sid), ))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             outfile.write(' type=%s' % (self.gds_format_string(quote_attrib(self.type_).encode(ExternalEncoding), input_name='type'), ))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             outfile.write(' id=%s' % (self.gds_format_string(quote_attrib(self.id).encode(ExternalEncoding), input_name='id'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='param', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='param'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.semantic is not None and 'semantic' not in already_processed:
-            already_processed.append('semantic')
+            already_processed.add('semantic')
             showIndent(outfile, level)
             outfile.write('semantic = "%s",\n' % (self.semantic,))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             showIndent(outfile, level)
             outfile.write('name = "%s",\n' % (self.name,))
         if self.flow is not None and 'flow' not in already_processed:
-            already_processed.append('flow')
+            already_processed.add('flow')
             showIndent(outfile, level)
             outfile.write('flow = %s,\n' % (self.flow,))
         if self.sid is not None and 'sid' not in already_processed:
-            already_processed.append('sid')
+            already_processed.add('sid')
             showIndent(outfile, level)
             outfile.write('sid = "%s",\n' % (self.sid,))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             showIndent(outfile, level)
             outfile.write('type_ = "%s",\n' % (self.type_,))
         if self.id is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             showIndent(outfile, level)
             outfile.write('id = "%s",\n' % (self.id,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('semantic', node)
         if value is not None and 'semantic' not in already_processed:
-            already_processed.append('semantic')
+            already_processed.add('semantic')
             self.semantic = value
             self.semantic = ' '.join(self.semantic.split())
         value = find_attr_value_('name', node)
         if value is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             self.name = value
         value = find_attr_value_('flow', node)
         if value is not None and 'flow' not in already_processed:
-            already_processed.append('flow')
+            already_processed.add('flow')
             self.flow = value
         value = find_attr_value_('sid', node)
         if value is not None and 'sid' not in already_processed:
-            already_processed.append('sid')
+            already_processed.add('sid')
             self.sid = value
         value = find_attr_value_('type', node)
         if value is not None and 'type' not in already_processed:
-            already_processed.append('type')
+            already_processed.add('type')
             self.type_ = value
         value = find_attr_value_('id', node)
         if value is not None and 'id' not in already_processed:
-            already_processed.append('id')
+            already_processed.add('id')
             self.id = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class param
 
 
 class agent(GeneratedsSuper):
@@ -1372,22 +1415,33 @@
     def set_priority(self, priority): self.priority = priority
     def get_info(self): return self.info
     def set_info(self, info): self.info = info
     def get_vehicle(self): return self.vehicle
     def set_vehicle(self, vehicle): self.vehicle = vehicle
     def add_vehicle(self, value): self.vehicle.append(value)
     def insert_vehicle(self, index, value): self.vehicle[index] = value
+    def hasContent_(self):
+        if (
+            self.firstname is not None or
+            self.lastname is not None or
+            self.priority is not None or
+            self.info is not None or
+            self.vehicle
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='agent', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='agent')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -1408,28 +1462,18 @@
         if self.priority is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%spriority>%s</%spriority>%s' % (namespace_, self.gds_format_float(self.priority, input_name='priority'), namespace_, eol_))
         if self.info is not None:
             self.info.export(outfile, level, namespace_, name_='info', pretty_print=pretty_print)
         for vehicle_ in self.get_vehicle():
             vehicle_.export(outfile, level, namespace_, name_='vehicle', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.firstname is not None or
-            self.lastname is not None or
-            self.priority is not None or
-            self.info is not None or
-            self.vehicle
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='agent'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.firstname is not None:
             showIndent(outfile, level)
@@ -1455,15 +1499,16 @@
             vehicle_.exportLiteral(outfile, level)
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'firstname':
@@ -1533,22 +1578,32 @@
     def set_firstname(self, firstname): self.firstname = firstname
     def get_lastname(self): return self.lastname
     def set_lastname(self, lastname): self.lastname = lastname
     def get_priority(self): return self.priority
     def set_priority(self, priority): self.priority = priority
     def get_info(self): return self.info
     def set_info(self, info): self.info = info
+    def hasContent_(self):
+        if (
+            self.firstname is not None or
+            self.lastname is not None or
+            self.priority is not None or
+            self.info is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='special-agent', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='special-agent')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -1567,27 +1622,18 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%slastname>%s</%slastname>%s' % (namespace_, self.gds_format_string(quote_xml(self.lastname).encode(ExternalEncoding), input_name='lastname'), namespace_, eol_))
         if self.priority is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%spriority>%s</%spriority>%s' % (namespace_, self.gds_format_float(self.priority, input_name='priority'), namespace_, eol_))
         if self.info is not None:
             self.info.export(outfile, level, namespace_, name_='info', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.firstname is not None or
-            self.lastname is not None or
-            self.priority is not None or
-            self.info is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='special-agent'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.firstname is not None:
             showIndent(outfile, level)
@@ -1601,15 +1647,16 @@
         if self.info is not None:
             showIndent(outfile, level)
             outfile.write('info=model_.info(\n')
             self.info.exportLiteral(outfile, level)
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'firstname':
@@ -1690,33 +1737,46 @@
     def insert_type(self, index, value): self.type_[index] = value
     def get_client_handler(self): return self.client_handler
     def set_client_handler(self, client_handler): self.client_handler = client_handler
     def add_client_handler(self, value): self.client_handler.append(value)
     def insert_client_handler(self, index, value): self.client_handler[index] = value
     def get_member_id(self): return self.member_id
     def set_member_id(self, member_id): self.member_id = member_id
+    def hasContent_(self):
+        if (
+            self.firstname is not None or
+            self.lastname is not None or
+            self.other_name is not None or
+            self.classxx is not None or
+            self.other_value or
+            self.type_ or
+            self.client_handler
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='booster', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='booster')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='booster'):
         if self.member_id is not None and 'member_id' not in already_processed:
-            already_processed.append('member_id')
+            already_processed.add('member_id')
             outfile.write(' member-id=%s' % (self.gds_format_string(quote_attrib(self.member_id).encode(ExternalEncoding), input_name='member-id'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='booster', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.firstname is not None:
@@ -1735,35 +1795,23 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sother-value>%s</%sother-value>%s' % (namespace_, self.gds_format_float(other_value_, input_name='other-value'), namespace_, eol_))
         for type_ in self.type_:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%stype>%s</%stype>%s' % (namespace_, self.gds_format_float(type_, input_name='type'), namespace_, eol_))
         for client_handler_ in self.client_handler:
             client_handler_.export(outfile, level, namespace_, name_='client-handler', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.firstname is not None or
-            self.lastname is not None or
-            self.other_name is not None or
-            self.classxx is not None or
-            self.other_value or
-            self.type_ or
-            self.client_handler
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='booster'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.member_id is not None and 'member_id' not in already_processed:
-            already_processed.append('member_id')
+            already_processed.add('member_id')
             showIndent(outfile, level)
             outfile.write('member_id = "%s",\n' % (self.member_id,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.firstname is not None:
             showIndent(outfile, level)
             outfile.write('firstname=%s,\n' % quote_python(self.firstname).encode(ExternalEncoding))
         if self.lastname is not None:
@@ -1802,22 +1850,23 @@
             client_handler_.exportLiteral(outfile, level, name_='client-handlerType')
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('member-id', node)
         if value is not None and 'member-id' not in already_processed:
-            already_processed.append('member-id')
+            already_processed.add('member-id')
             self.member_id = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'firstname':
             firstname_ = child_.text
             firstname_ = self.gds_validate_string(firstname_, node, 'firstname')
             self.firstname = firstname_
         elif nodeName_ == 'lastname':
@@ -1884,91 +1933,93 @@
     factory = staticmethod(factory)
     def get_rating(self): return self.rating
     def set_rating(self, rating): self.rating = rating
     def get_type(self): return self.type_
     def set_type(self, type_): self.type_ = type_
     def get_name(self): return self.name
     def set_name(self, name): self.name = name
+    def hasContent_(self):
+        if (
+
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='info', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='info')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='info'):
         if self.rating is not None and 'rating' not in already_processed:
-            already_processed.append('rating')
+            already_processed.add('rating')
             outfile.write(' rating="%s"' % self.gds_format_float(self.rating, input_name='rating'))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             outfile.write(' type="%s"' % self.gds_format_integer(self.type_, input_name='type'))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             outfile.write(' name=%s' % (self.gds_format_string(quote_attrib(self.name).encode(ExternalEncoding), input_name='name'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='info', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='info'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.rating is not None and 'rating' not in already_processed:
-            already_processed.append('rating')
+            already_processed.add('rating')
             showIndent(outfile, level)
             outfile.write('rating = %f,\n' % (self.rating,))
         if self.type_ is not None and 'type_' not in already_processed:
-            already_processed.append('type_')
+            already_processed.add('type_')
             showIndent(outfile, level)
             outfile.write('type_ = %d,\n' % (self.type_,))
         if self.name is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             showIndent(outfile, level)
             outfile.write('name = "%s",\n' % (self.name,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('rating', node)
         if value is not None and 'rating' not in already_processed:
-            already_processed.append('rating')
+            already_processed.add('rating')
             try:
                 self.rating = float(value)
             except ValueError, exp:
                 raise ValueError('Bad float/double attribute (rating): %s' % exp)
         value = find_attr_value_('type', node)
         if value is not None and 'type' not in already_processed:
-            already_processed.append('type')
+            already_processed.add('type')
             try:
                 self.type_ = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
         value = find_attr_value_('name', node)
         if value is not None and 'name' not in already_processed:
-            already_processed.append('name')
+            already_processed.add('name')
             self.name = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class info
 
 
 class vehicle(GeneratedsSuper):
@@ -1986,71 +2037,73 @@
         else:
             return vehicle(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_wheelcount(self): return self.wheelcount
     def set_wheelcount(self, wheelcount): self.wheelcount = wheelcount
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.wheelcount is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='vehicle', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='vehicle')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='vehicle'):
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
         pass
     def exportChildren(self, outfile, level, namespace_='', name_='vehicle', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.wheelcount is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%swheelcount>%s</%swheelcount>%s' % (namespace_, self.gds_format_integer(self.wheelcount, input_name='wheelcount'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.wheelcount is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='vehicle'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.wheelcount is not None:
             showIndent(outfile, level)
             outfile.write('wheelcount=%d,\n' % self.wheelcount)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'wheelcount':
             sval_ = child_.text
             try:
                 ival_ = int(sval_)
             except (TypeError, ValueError), exp:
@@ -2073,22 +2126,30 @@
         if automobile.subclass:
             return automobile.subclass(*args_, **kwargs_)
         else:
             return automobile(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_drivername(self): return self.drivername
     def set_drivername(self, drivername): self.drivername = drivername
+    def hasContent_(self):
+        if (
+            self.drivername is not None or
+            super(automobile, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='automobile', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='automobile')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2100,36 +2161,30 @@
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.drivername is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sdrivername>%s</%sdrivername>%s' % (namespace_, self.gds_format_string(quote_xml(self.drivername).encode(ExternalEncoding), input_name='drivername'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.drivername is not None or
-            super(automobile, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='automobile'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(automobile, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(automobile, self).exportLiteralChildren(outfile, level, name_)
         if self.drivername is not None:
             showIndent(outfile, level)
             outfile.write('drivername=%s,\n' % quote_python(self.drivername).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(automobile, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'drivername':
@@ -2153,22 +2208,30 @@
         if airplane.subclass:
             return airplane.subclass(*args_, **kwargs_)
         else:
             return airplane(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_pilotname(self): return self.pilotname
     def set_pilotname(self, pilotname): self.pilotname = pilotname
+    def hasContent_(self):
+        if (
+            self.pilotname is not None or
+            super(airplane, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='airplane', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='airplane')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2180,36 +2243,30 @@
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.pilotname is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%spilotname>%s</%spilotname>%s' % (namespace_, self.gds_format_string(quote_xml(self.pilotname).encode(ExternalEncoding), input_name='pilotname'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.pilotname is not None or
-            super(airplane, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='airplane'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(airplane, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(airplane, self).exportLiteralChildren(outfile, level, name_)
         if self.pilotname is not None:
             showIndent(outfile, level)
             outfile.write('pilotname=%s,\n' % quote_python(self.pilotname).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(airplane, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'pilotname':
@@ -2305,52 +2362,70 @@
     def set_attrposint(self, attrposint): self.attrposint = attrposint
     def get_attrnonnegint(self): return self.attrnonnegint
     def set_attrnonnegint(self, attrnonnegint): self.attrnonnegint = attrnonnegint
     def get_attrnonposint(self): return self.attrnonposint
     def set_attrnonposint(self, attrnonposint): self.attrnonposint = attrnonposint
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.email is not None or
+            self.elposint is not None or
+            self.elnonposint is not None or
+            self.elnegint is not None or
+            self.elnonnegint is not None or
+            self.eldate is not None or
+            self.eltoken is not None or
+            self.elshort is not None or
+            self.ellong is not None or
+            self.elparam is not None or
+            self.elarraytypes is not None or
+            super(programmer, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='programmer', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='programmer')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='programmer'):
         super(programmer, self).exportAttributes(outfile, level, already_processed, namespace_, name_='programmer')
         if self.language is not None and 'language' not in already_processed:
-            already_processed.append('language')
+            already_processed.add('language')
             outfile.write(' language=%s' % (self.gds_format_string(quote_attrib(self.language).encode(ExternalEncoding), input_name='language'), ))
         if self.area is not None and 'area' not in already_processed:
-            already_processed.append('area')
+            already_processed.add('area')
             outfile.write(' area=%s' % (self.gds_format_string(quote_attrib(self.area).encode(ExternalEncoding), input_name='area'), ))
         if self.attrnegint is not None and 'attrnegint' not in already_processed:
-            already_processed.append('attrnegint')
+            already_processed.add('attrnegint')
             outfile.write(' attrnegint="%s"' % self.gds_format_integer(self.attrnegint, input_name='attrnegint'))
         if self.attrposint is not None and 'attrposint' not in already_processed:
-            already_processed.append('attrposint')
+            already_processed.add('attrposint')
             outfile.write(' attrposint="%s"' % self.gds_format_integer(self.attrposint, input_name='attrposint'))
         if self.attrnonnegint is not None and 'attrnonnegint' not in already_processed:
-            already_processed.append('attrnonnegint')
+            already_processed.add('attrnonnegint')
             outfile.write(' attrnonnegint="%s"' % self.gds_format_integer(self.attrnonnegint, input_name='attrnonnegint'))
         if self.attrnonposint is not None and 'attrnonposint' not in already_processed:
-            already_processed.append('attrnonposint')
+            already_processed.add('attrnonposint')
             outfile.write(' attrnonposint="%s"' % self.gds_format_integer(self.attrnonposint, input_name='attrnonposint'))
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
     def exportChildren(self, outfile, level, namespace_='', name_='programmer', fromsubclass_=False, pretty_print=True):
         super(programmer, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
@@ -2383,60 +2458,43 @@
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sellong>%s</%sellong>%s' % (namespace_, self.gds_format_integer(self.ellong, input_name='ellong'), namespace_, eol_))
         if self.elparam is not None:
             self.elparam.export(outfile, level, namespace_, name_='elparam', pretty_print=pretty_print)
         if self.elarraytypes is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%selarraytypes>%s</%selarraytypes>%s' % (namespace_, self.gds_format_string(quote_xml(self.elarraytypes).encode(ExternalEncoding), input_name='elarraytypes'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.email is not None or
-            self.elposint is not None or
-            self.elnonposint is not None or
-            self.elnegint is not None or
-            self.elnonnegint is not None or
-            self.eldate is not None or
-            self.eltoken is not None or
-            self.elshort is not None or
-            self.ellong is not None or
-            self.elparam is not None or
-            self.elarraytypes is not None or
-            super(programmer, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='programmer'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.language is not None and 'language' not in already_processed:
-            already_processed.append('language')
+            already_processed.add('language')
             showIndent(outfile, level)
             outfile.write('language = "%s",\n' % (self.language,))
         if self.area is not None and 'area' not in already_processed:
-            already_processed.append('area')
+            already_processed.add('area')
             showIndent(outfile, level)
             outfile.write('area = "%s",\n' % (self.area,))
         if self.attrnegint is not None and 'attrnegint' not in already_processed:
-            already_processed.append('attrnegint')
+            already_processed.add('attrnegint')
             showIndent(outfile, level)
             outfile.write('attrnegint = %d,\n' % (self.attrnegint,))
         if self.attrposint is not None and 'attrposint' not in already_processed:
-            already_processed.append('attrposint')
+            already_processed.add('attrposint')
             showIndent(outfile, level)
             outfile.write('attrposint = %d,\n' % (self.attrposint,))
         if self.attrnonnegint is not None and 'attrnonnegint' not in already_processed:
-            already_processed.append('attrnonnegint')
+            already_processed.add('attrnonnegint')
             showIndent(outfile, level)
             outfile.write('attrnonnegint = %d,\n' % (self.attrnonnegint,))
         if self.attrnonposint is not None and 'attrnonposint' not in already_processed:
-            already_processed.append('attrnonposint')
+            already_processed.add('attrnonposint')
             showIndent(outfile, level)
             outfile.write('attrnonposint = %d,\n' % (self.attrnonposint,))
         super(programmer, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(programmer, self).exportLiteralChildren(outfile, level, name_)
         if self.email is not None:
             showIndent(outfile, level)
@@ -2471,66 +2529,67 @@
             self.elparam.exportLiteral(outfile, level, name_='elparam')
             showIndent(outfile, level)
             outfile.write('),\n')
         if self.elarraytypes is not None:
             showIndent(outfile, level)
             outfile.write('elarraytypes=%s,\n' % quote_python(self.elarraytypes).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('language', node)
         if value is not None and 'language' not in already_processed:
-            already_processed.append('language')
+            already_processed.add('language')
             self.language = value
         value = find_attr_value_('area', node)
         if value is not None and 'area' not in already_processed:
-            already_processed.append('area')
+            already_processed.add('area')
             self.area = value
         value = find_attr_value_('attrnegint', node)
         if value is not None and 'attrnegint' not in already_processed:
-            already_processed.append('attrnegint')
+            already_processed.add('attrnegint')
             try:
                 self.attrnegint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrnegint >= 0:
                 raise_parse_error(node, 'Invalid NegativeInteger')
         value = find_attr_value_('attrposint', node)
         if value is not None and 'attrposint' not in already_processed:
-            already_processed.append('attrposint')
+            already_processed.add('attrposint')
             try:
                 self.attrposint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrposint <= 0:
                 raise_parse_error(node, 'Invalid PositiveInteger')
         value = find_attr_value_('attrnonnegint', node)
         if value is not None and 'attrnonnegint' not in already_processed:
-            already_processed.append('attrnonnegint')
+            already_processed.add('attrnonnegint')
             try:
                 self.attrnonnegint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrnonnegint < 0:
                 raise_parse_error(node, 'Invalid NonNegativeInteger')
         value = find_attr_value_('attrnonposint', node)
         if value is not None and 'attrnonposint' not in already_processed:
-            already_processed.append('attrnonposint')
+            already_processed.add('attrnonposint')
             try:
                 self.attrnonposint = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.attrnonposint > 0:
                 raise_parse_error(node, 'Invalid NonPositiveInteger')
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
         super(programmer, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'email':
             email_ = child_.text
             email_ = self.gds_validate_string(email_, node, 'email')
             self.email = email_
@@ -2628,22 +2687,30 @@
         else:
             return client_handlerType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_fullname(self): return self.fullname
     def set_fullname(self, fullname): self.fullname = fullname
     def get_refid(self): return self.refid
     def set_refid(self, refid): self.refid = refid
+    def hasContent_(self):
+        if (
+            self.fullname is not None or
+            self.refid is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='client-handlerType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='client-handlerType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -2657,38 +2724,32 @@
             eol_ = ''
         if self.fullname is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfullname>%s</%sfullname>%s' % (namespace_, self.gds_format_string(quote_xml(self.fullname).encode(ExternalEncoding), input_name='fullname'), namespace_, eol_))
         if self.refid is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%srefid>%s</%srefid>%s' % (namespace_, self.gds_format_integer(self.refid, input_name='refid'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.fullname is not None or
-            self.refid is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='client-handlerType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.fullname is not None:
             showIndent(outfile, level)
             outfile.write('fullname=%s,\n' % quote_python(self.fullname).encode(ExternalEncoding))
         if self.refid is not None:
             showIndent(outfile, level)
             outfile.write('refid=%d,\n' % self.refid)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'fullname':
@@ -2730,88 +2791,90 @@
     factory = staticmethod(factory)
     def get_favorite_editor(self): return self.favorite_editor
     def set_favorite_editor(self, favorite_editor): self.favorite_editor = favorite_editor
     def get_status(self): return self.status
     def set_status(self, status): self.status = status
     def get_nick_name(self): return self.nick_name
     def set_nick_name(self, nick_name): self.nick_name = nick_name
+    def hasContent_(self):
+        if (
+            self.favorite_editor is not None or
+            super(java_programmer, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='java-programmer', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='java-programmer')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='java-programmer'):
         super(java_programmer, self).exportAttributes(outfile, level, already_processed, namespace_, name_='java-programmer')
         if self.status is not None and 'status' not in already_processed:
-            already_processed.append('status')
+            already_processed.add('status')
             outfile.write(' status=%s' % (self.gds_format_string(quote_attrib(self.status).encode(ExternalEncoding), input_name='status'), ))
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             outfile.write(' nick-name=%s' % (self.gds_format_string(quote_attrib(self.nick_name).encode(ExternalEncoding), input_name='nick-name'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='java-programmer', fromsubclass_=False, pretty_print=True):
         super(java_programmer, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.favorite_editor is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfavorite-editor>%s</%sfavorite-editor>%s' % (namespace_, self.gds_format_string(quote_xml(self.favorite_editor).encode(ExternalEncoding), input_name='favorite-editor'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.favorite_editor is not None or
-            super(java_programmer, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='java-programmer'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.status is not None and 'status' not in already_processed:
-            already_processed.append('status')
+            already_processed.add('status')
             showIndent(outfile, level)
             outfile.write('status = "%s",\n' % (self.status,))
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             showIndent(outfile, level)
             outfile.write('nick_name = "%s",\n' % (self.nick_name,))
         super(java_programmer, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(java_programmer, self).exportLiteralChildren(outfile, level, name_)
         if self.favorite_editor is not None:
             showIndent(outfile, level)
             outfile.write('favorite_editor=%s,\n' % quote_python(self.favorite_editor).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('status', node)
         if value is not None and 'status' not in already_processed:
-            already_processed.append('status')
+            already_processed.add('status')
             self.status = value
         value = find_attr_value_('nick-name', node)
         if value is not None and 'nick-name' not in already_processed:
-            already_processed.append('nick-name')
+            already_processed.add('nick-name')
             self.nick_name = value
         super(java_programmer, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'favorite-editor':
             favorite_editor_ = child_.text
             favorite_editor_ = self.gds_validate_string(favorite_editor_, node, 'favorite_editor')
             self.favorite_editor = favorite_editor_
@@ -2838,77 +2901,79 @@
         else:
             return python_programmer(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_favorite_editor(self): return self.favorite_editor
     def set_favorite_editor(self, favorite_editor): self.favorite_editor = favorite_editor
     def get_nick_name(self): return self.nick_name
     def set_nick_name(self, nick_name): self.nick_name = nick_name
+    def hasContent_(self):
+        if (
+            self.favorite_editor is not None or
+            super(python_programmer, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='python-programmer', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='python-programmer')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='python-programmer'):
         super(python_programmer, self).exportAttributes(outfile, level, already_processed, namespace_, name_='python-programmer')
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             outfile.write(' nick-name=%s' % (self.gds_format_string(quote_attrib(self.nick_name).encode(ExternalEncoding), input_name='nick-name'), ))
     def exportChildren(self, outfile, level, namespace_='', name_='python-programmer', fromsubclass_=False, pretty_print=True):
         super(python_programmer, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.favorite_editor is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sfavorite-editor>%s</%sfavorite-editor>%s' % (namespace_, self.gds_format_string(quote_xml(self.favorite_editor).encode(ExternalEncoding), input_name='favorite-editor'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.favorite_editor is not None or
-            super(python_programmer, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='python-programmer'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.nick_name is not None and 'nick_name' not in already_processed:
-            already_processed.append('nick_name')
+            already_processed.add('nick_name')
             showIndent(outfile, level)
             outfile.write('nick_name = "%s",\n' % (self.nick_name,))
         super(python_programmer, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(python_programmer, self).exportLiteralChildren(outfile, level, name_)
         if self.favorite_editor is not None:
             showIndent(outfile, level)
             outfile.write('favorite_editor=%s,\n' % quote_python(self.favorite_editor).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('nick-name', node)
         if value is not None and 'nick-name' not in already_processed:
-            already_processed.append('nick-name')
+            already_processed.add('nick-name')
             self.nick_name = value
         super(python_programmer, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'favorite-editor':
             favorite_editor_ = child_.text
             favorite_editor_ = self.gds_validate_string(favorite_editor_, node, 'favorite_editor')
             self.favorite_editor = favorite_editor_
@@ -2954,14 +3019,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'people'
+        rootClass = people
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'people'
```

### Comparing `generateDS-2.8b/tests/people_procincl.xsd` & `generateDS-2.9a/tests/people_procincl.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/people_procincl1_sub.py` & `generateDS-2.9a/tests/people_procincl1_sub.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,18 +204,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'people'
+        rootClass = supermod.people
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'people'
```

### Comparing `generateDS-2.8b/tests/attr_groups2_sub.py` & `generateDS-2.9a/tests/attr_groups2_sub.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,18 +99,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'getUser'
+        rootClass = supermod.GetUserReq
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'getUser'
```

### Comparing `generateDS-2.8b/tests/extensions.xsd` & `generateDS-2.9a/tests/extensions.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/ipo1_sup.py` & `generateDS-2.9a/tests/ipo1_sup.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -506,33 +539,43 @@
     def set_billTo(self, billTo): self.billTo = billTo
     def get_comment(self): return self.comment
     def set_comment(self, comment): self.comment = comment
     def get_items(self): return self.items
     def set_items(self, items): self.items = items
     def get_orderDate(self): return self.orderDate
     def set_orderDate(self, orderDate): self.orderDate = orderDate
+    def hasContent_(self):
+        if (
+            self.shipTo is not None or
+            self.billTo is not None or
+            self.comment is not None or
+            self.items is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='PurchaseOrderType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='PurchaseOrderType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='ipo:', name_='PurchaseOrderType'):
         if self.orderDate is not None and 'orderDate' not in already_processed:
-            already_processed.append('orderDate')
+            already_processed.add('orderDate')
             outfile.write(' orderDate="%s"' % self.gds_format_date(self.orderDate, input_name='orderDate'))
     def exportChildren(self, outfile, level, namespace_='ipo:', name_='PurchaseOrderType', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.shipTo is not None:
@@ -540,32 +583,23 @@
         if self.billTo is not None:
             self.billTo.export(outfile, level, namespace_, name_='billTo', pretty_print=pretty_print)
         if self.comment is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scomment>%s</%scomment>%s' % (namespace_, self.gds_format_string(quote_xml(self.comment).encode(ExternalEncoding), input_name='comment'), namespace_, eol_))
         if self.items is not None:
             self.items.export(outfile, level, namespace_, name_='items', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.shipTo is not None or
-            self.billTo is not None or
-            self.comment is not None or
-            self.items is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='PurchaseOrderType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.orderDate is not None and 'orderDate' not in already_processed:
-            already_processed.append('orderDate')
+            already_processed.add('orderDate')
             showIndent(outfile, level)
             outfile.write('orderDate = "%s",\n' % (self.orderDate,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.shipTo is not None:
             showIndent(outfile, level)
             outfile.write('shipTo=model_.Address(\n')
             self.shipTo.exportLiteral(outfile, level, name_='shipTo')
@@ -583,22 +617,23 @@
         if self.items is not None:
             showIndent(outfile, level)
             outfile.write('items=model_.Items(\n')
             self.items.exportLiteral(outfile, level, name_='items')
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('orderDate', node)
         if value is not None and 'orderDate' not in already_processed:
-            already_processed.append('orderDate')
+            already_processed.add('orderDate')
             try:
                 self.orderDate = self.gds_parse_date(value, node, 'orderDate')
             except ValueError, exp:
                 raise ValueError('Bad date attribute (orderDate): %s' % exp)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'shipTo':
             class_obj_ = self.get_class_obj_(child_, Address)
@@ -638,22 +673,29 @@
         else:
             return Items(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_item(self): return self.item
     def set_item(self, item): self.item = item
     def add_item(self, value): self.item.append(value)
     def insert_item(self, index, value): self.item[index] = value
+    def hasContent_(self):
+        if (
+            self.item
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='Items', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='Items')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -663,24 +705,18 @@
     def exportChildren(self, outfile, level, namespace_='ipo:', name_='Items', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for item_ in self.item:
             item_.export(outfile, level, namespace_, name_='item', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.item
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='Items'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('item=[\n')
@@ -691,15 +727,16 @@
             item_.exportLiteral(outfile, level, name_='itemType')
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'item':
@@ -732,33 +769,42 @@
     def set_name(self, name): self.name = name
     def get_street(self): return self.street
     def set_street(self, street): self.street = street
     def get_city(self): return self.city
     def set_city(self, city): self.city = city
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.street is not None or
+            self.city is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='Address', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='Address')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='ipo:', name_='Address'):
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
         pass
     def exportChildren(self, outfile, level, namespace_='ipo:', name_='Address', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
@@ -768,26 +814,18 @@
             outfile.write('<%sname>%s</%sname>%s' % (namespace_, self.gds_format_string(quote_xml(self.name).encode(ExternalEncoding), input_name='name'), namespace_, eol_))
         if self.street is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sstreet>%s</%sstreet>%s' % (namespace_, self.gds_format_string(quote_xml(self.street).encode(ExternalEncoding), input_name='street'), namespace_, eol_))
         if self.city is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scity>%s</%scity>%s' % (namespace_, self.gds_format_string(quote_xml(self.city).encode(ExternalEncoding), input_name='city'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.street is not None or
-            self.city is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='Address'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
@@ -795,22 +833,23 @@
         if self.street is not None:
             showIndent(outfile, level)
             outfile.write('street=%s,\n' % quote_python(self.street).encode(ExternalEncoding))
         if self.city is not None:
             showIndent(outfile, level)
             outfile.write('city=%s,\n' % quote_python(self.city).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
             name_ = child_.text
             name_ = self.gds_validate_string(name_, node, 'name')
             self.name = name_
         elif nodeName_ == 'street':
@@ -844,22 +883,31 @@
     def get_state(self): return self.state
     def set_state(self, state): self.state = state
     def validate_USState(self, value):
         # Validate type USState, a restriction on string.
         pass
     def get_zip(self): return self.zip
     def set_zip(self, zip): self.zip = zip
+    def hasContent_(self):
+        if (
+            self.state is not None or
+            self.zip is not None or
+            super(USAddress, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='USAddress', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='USAddress')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -874,40 +922,33 @@
             eol_ = ''
         if self.state is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sstate>%s</%sstate>%s' % (namespace_, self.gds_format_string(quote_xml(self.state).encode(ExternalEncoding), input_name='state'), namespace_, eol_))
         if self.zip is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%szip>%s</%szip>%s' % (namespace_, self.gds_format_integer(self.zip, input_name='zip'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.state is not None or
-            self.zip is not None or
-            super(USAddress, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='USAddress'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(USAddress, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(USAddress, self).exportLiteralChildren(outfile, level, name_)
         if self.state is not None:
             showIndent(outfile, level)
             outfile.write('state=%s,\n' % quote_python(self.state).encode(ExternalEncoding))
         if self.zip is not None:
             showIndent(outfile, level)
             outfile.write('zip=%d,\n' % self.zip)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(USAddress, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'state':
@@ -957,95 +998,97 @@
         pass
     def get_category(self): return self.category
     def set_category(self, category): self.category = category
     def get_category_attr(self): return self.category_attr
     def set_category_attr(self, category_attr): self.category_attr = category_attr
     def get_exportCode(self): return self.exportCode
     def set_exportCode(self, exportCode): self.exportCode = exportCode
+    def hasContent_(self):
+        if (
+            self.postcode is not None or
+            self.category is not None or
+            super(UKAddress, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='UKAddress', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='UKAddress')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='ipo:', name_='UKAddress'):
         super(UKAddress, self).exportAttributes(outfile, level, already_processed, namespace_, name_='UKAddress')
         if self.category_attr is not None and 'category_attr' not in already_processed:
-            already_processed.append('category_attr')
+            already_processed.add('category_attr')
             outfile.write(' category=%s' % (quote_attrib(self.category_attr), ))
         if self.exportCode is not None and 'exportCode' not in already_processed:
-            already_processed.append('exportCode')
+            already_processed.add('exportCode')
             outfile.write(' exportCode="%s"' % self.gds_format_integer(self.exportCode, input_name='exportCode'))
     def exportChildren(self, outfile, level, namespace_='ipo:', name_='UKAddress', fromsubclass_=False, pretty_print=True):
         super(UKAddress, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.postcode is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%spostcode>%s</%spostcode>%s' % (namespace_, self.gds_format_string(quote_xml(self.postcode).encode(ExternalEncoding), input_name='postcode'), namespace_, eol_))
         if self.category is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scategory>%s</%scategory>%s' % (namespace_, self.gds_format_string(quote_xml(self.category).encode(ExternalEncoding), input_name='category'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.postcode is not None or
-            self.category is not None or
-            super(UKAddress, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='UKAddress'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.category_attr is not None and 'category_attr' not in already_processed:
-            already_processed.append('category_attr')
+            already_processed.add('category_attr')
             showIndent(outfile, level)
             outfile.write('category_attr = %s,\n' % (self.category_attr,))
         if self.exportCode is not None and 'exportCode' not in already_processed:
-            already_processed.append('exportCode')
+            already_processed.add('exportCode')
             showIndent(outfile, level)
             outfile.write('exportCode = %d,\n' % (self.exportCode,))
         super(UKAddress, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(UKAddress, self).exportLiteralChildren(outfile, level, name_)
         if self.postcode is not None:
             showIndent(outfile, level)
             outfile.write('postcode=%s,\n' % quote_python(self.postcode).encode(ExternalEncoding))
         if self.category is not None:
             showIndent(outfile, level)
             outfile.write('category=%s,\n' % quote_python(self.category).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('category', node)
         if value is not None and 'category_attr' not in already_processed:
-            already_processed.append('category_attr')
+            already_processed.add('category_attr')
             self.category_attr = value
         value = find_attr_value_('exportCode', node)
         if value is not None and 'exportCode' not in already_processed:
-            already_processed.append('exportCode')
+            already_processed.add('exportCode')
             try:
                 self.exportCode = int(value)
             except ValueError, exp:
                 raise_parse_error(node, 'Bad integer attribute: %s' % exp)
             if self.exportCode <= 0:
                 raise_parse_error(node, 'Invalid PositiveInteger')
         super(UKAddress, self).buildAttributes(node, attrs, already_processed)
@@ -1095,33 +1138,44 @@
     def set_USPrice(self, USPrice): self.USPrice = USPrice
     def get_comment(self): return self.comment
     def set_comment(self, comment): self.comment = comment
     def get_shipDate(self): return self.shipDate
     def set_shipDate(self, shipDate): self.shipDate = shipDate
     def get_partNum(self): return self.partNum
     def set_partNum(self, partNum): self.partNum = partNum
+    def hasContent_(self):
+        if (
+            self.productName is not None or
+            self.quantity is not None or
+            self.USPrice is not None or
+            self.comment is not None or
+            self.shipDate is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='itemType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='itemType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='ipo:', name_='itemType'):
         if self.partNum is not None and 'partNum' not in already_processed:
-            already_processed.append('partNum')
+            already_processed.add('partNum')
             outfile.write(' partNum=%s' % (quote_attrib(self.partNum), ))
     def exportChildren(self, outfile, level, namespace_='ipo:', name_='itemType', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.productName is not None:
@@ -1135,33 +1189,23 @@
             outfile.write('<%sUSPrice>%s</%sUSPrice>%s' % (namespace_, self.gds_format_float(self.USPrice, input_name='USPrice'), namespace_, eol_))
         if self.comment is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scomment>%s</%scomment>%s' % (namespace_, self.gds_format_string(quote_xml(self.comment).encode(ExternalEncoding), input_name='comment'), namespace_, eol_))
         if self.shipDate is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sshipDate>%s</%sshipDate>%s' % (namespace_, self.gds_format_date(self.shipDate, input_name='shipDate'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.productName is not None or
-            self.quantity is not None or
-            self.USPrice is not None or
-            self.comment is not None or
-            self.shipDate is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='itemType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.partNum is not None and 'partNum' not in already_processed:
-            already_processed.append('partNum')
+            already_processed.add('partNum')
             showIndent(outfile, level)
             outfile.write('partNum = %s,\n' % (self.partNum,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.productName is not None:
             showIndent(outfile, level)
             outfile.write('productName=%s,\n' % quote_python(self.productName).encode(ExternalEncoding))
         if self.quantity is not None:
@@ -1173,22 +1217,23 @@
         if self.comment is not None:
             showIndent(outfile, level)
             outfile.write('comment=%s,\n' % quote_python(self.comment).encode(ExternalEncoding))
         if self.shipDate is not None:
             showIndent(outfile, level)
             outfile.write('shipDate=datetime_.strptime("%s", "%%Y-%%m-%%d"),\n' % self.gds_format_date(self.shipDate, input_name='shipDate'))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('partNum', node)
         if value is not None and 'partNum' not in already_processed:
-            already_processed.append('partNum')
+            already_processed.add('partNum')
             self.partNum = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'productName':
             productName_ = child_.text
             productName_ = self.gds_validate_string(productName_, node, 'productName')
             self.productName = productName_
         elif nodeName_ == 'quantity':
@@ -1229,51 +1274,53 @@
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if quantity.subclass:
             return quantity.subclass(*args_, **kwargs_)
         else:
             return quantity(*args_, **kwargs_)
     factory = staticmethod(factory)
+    def hasContent_(self):
+        if (
+
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='ipo:', name_='quantity', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='quantity')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='ipo:', name_='quantity'):
         pass
     def exportChildren(self, outfile, level, namespace_='ipo:', name_='quantity', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='quantity'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
@@ -1320,14 +1367,33 @@
     sys.stdout.write('<?xml version="1.0" ?>\n')
     rootObj.export(sys.stdout, 0, name_=rootTag,
         namespacedef_='',
         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'purchaseOrder'
+        rootClass = PurchaseOrderType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+    content = etree_.tostring(rootElement, pretty_print=True,
+        xml_declaration=True, encoding="utf-8")
+    sys.stdout.write(content)
+    sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'purchaseOrder'
```

### Comparing `generateDS-2.8b/tests/people.xml` & `generateDS-2.9a/tests/people.xml`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/anywildcard1_sup.py` & `generateDS-2.9a/tests/anywildcard1_sup.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -498,22 +531,31 @@
     factory = staticmethod(factory)
     def get_name(self): return self.name
     def set_name(self, name): self.name = name
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def get_description(self): return self.description
     def set_description(self, description): self.description = description
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.anytypeobjs_ is not None or
+            self.description is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='PlantType_single', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='PlantType_single')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -528,26 +570,18 @@
         if self.name is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sname>%s</%sname>%s' % (namespace_, self.gds_format_string(quote_xml(self.name).encode(ExternalEncoding), input_name='name'), namespace_, eol_))
         if self.description is not None:
             self.description.export(outfile, level, namespace_, name_='description', pretty_print=pretty_print)
         if self.anytypeobjs_ is not None:
             self.anytypeobjs_.export(outfile, level, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.anytypeobjs_ is not None or
-            self.description is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='PlantType_single'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
@@ -561,15 +595,16 @@
         if self.description is not None:
             showIndent(outfile, level)
             outfile.write('description=model_.DescriptionType(\n')
             self.description.exportLiteral(outfile, level, name_='description')
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
@@ -612,22 +647,31 @@
     def set_name(self, name): self.name = name
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
     def get_description(self): return self.description
     def set_description(self, description): self.description = description
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.anytypeobjs_ or
+            self.description is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='PlantType_multiple', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='PlantType_multiple')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -642,26 +686,18 @@
         if self.name is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sname>%s</%sname>%s' % (namespace_, self.gds_format_string(quote_xml(self.name).encode(ExternalEncoding), input_name='name'), namespace_, eol_))
         if self.description is not None:
             self.description.export(outfile, level, namespace_, name_='description', pretty_print=pretty_print)
         for obj_ in self.anytypeobjs_:
             obj_.export(outfile, level, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.anytypeobjs_ or
-            self.description is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='PlantType_multiple'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
@@ -677,15 +713,16 @@
         if self.description is not None:
             showIndent(outfile, level)
             outfile.write('description=model_.DescriptionType(\n')
             self.description.exportLiteral(outfile, level, name_='description')
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
@@ -720,22 +757,30 @@
         else:
             return DescriptionType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_name(self): return self.name
     def set_name(self, name): self.name = name
     def get_size(self): return self.size
     def set_size(self, size): self.size = size
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.size is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='DescriptionType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='DescriptionType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -749,38 +794,32 @@
             eol_ = ''
         if self.name is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sname>%s</%sname>%s' % (namespace_, self.gds_format_string(quote_xml(self.name).encode(ExternalEncoding), input_name='name'), namespace_, eol_))
         if self.size is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%ssize>%s</%ssize>%s' % (namespace_, self.gds_format_string(quote_xml(self.size).encode(ExternalEncoding), input_name='size'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.size is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='DescriptionType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
             outfile.write('name=%s,\n' % quote_python(self.name).encode(ExternalEncoding))
         if self.size is not None:
             showIndent(outfile, level)
             outfile.write('size=%s,\n' % quote_python(self.size).encode(ExternalEncoding))
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
@@ -811,22 +850,30 @@
         else:
             return CatalogType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_name(self): return self.name
     def set_name(self, name): self.name = name
     def get_catagory(self): return self.catagory
     def set_catagory(self, catagory): self.catagory = catagory
+    def hasContent_(self):
+        if (
+            self.name is not None or
+            self.catagory is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='CatalogType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='CatalogType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -840,38 +887,32 @@
             eol_ = ''
         if self.name is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sname>%s</%sname>%s' % (namespace_, self.gds_format_string(quote_xml(self.name).encode(ExternalEncoding), input_name='name'), namespace_, eol_))
         if self.catagory is not None:
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scatagory>%s</%scatagory>%s' % (namespace_, self.gds_format_integer(self.catagory, input_name='catagory'), namespace_, eol_))
-    def hasContent_(self):
-        if (
-            self.name is not None or
-            self.catagory is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='CatalogType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.name is not None:
             showIndent(outfile, level)
             outfile.write('name=%s,\n' % quote_python(self.name).encode(ExternalEncoding))
         if self.catagory is not None:
             showIndent(outfile, level)
             outfile.write('catagory=%d,\n' % self.catagory)
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'name':
@@ -901,22 +942,29 @@
         if PlantType_single_nochild.subclass:
             return PlantType_single_nochild.subclass(*args_, **kwargs_)
         else:
             return PlantType_single_nochild(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
+    def hasContent_(self):
+        if (
+            self.anytypeobjs_ is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='PlantType_single_nochild', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='PlantType_single_nochild')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -926,37 +974,32 @@
     def exportChildren(self, outfile, level, namespace_='', name_='PlantType_single_nochild', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.anytypeobjs_ is not None:
             self.anytypeobjs_.export(outfile, level, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.anytypeobjs_ is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='PlantType_single_nochild'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         if self.anytypeobjs_ is not None:
             showIndent(outfile, level)
             outfile.write('anytypeobjs_=model_.anytypeobjs_(\n')
             self.anytypeobjs_.exportLiteral(outfile, level)
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         obj_ = self.gds_build_any(child_, 'PlantType_single_nochild')
@@ -982,22 +1025,29 @@
         else:
             return PlantType_multiple_nochild(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
+    def hasContent_(self):
+        if (
+            self.anytypeobjs_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='PlantType_multiple_nochild', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='PlantType_multiple_nochild')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -1007,39 +1057,34 @@
     def exportChildren(self, outfile, level, namespace_='', name_='PlantType_multiple_nochild', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for obj_ in self.anytypeobjs_:
             obj_.export(outfile, level, namespace_, pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.anytypeobjs_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='PlantType_multiple_nochild'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('anytypeobjs_=[\n')
         level += 1
         for anytypeobjs_ in self.anytypeobjs_:
             anytypeobjs_.exportLiteral(outfile, level)
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         obj_ = self.gds_build_any(child_, 'PlantType_multiple_nochild')
@@ -1084,14 +1129,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'PlantType_single'
+        rootClass = PlantType_single
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'PlantType_single'
```

### Comparing `generateDS-2.8b/tests/annotations2_sub.py` & `generateDS-2.9a/tests/annotations2_sub.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,18 +113,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'document1'
+        rootClass = supermod.document1Type
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'document1'
```

### Comparing `generateDS-2.8b/tests/ipo1_out.xml` & `generateDS-2.9a/tests/ipo1_out.xml`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/out1_sub.py` & `generateDS-2.9a/tests/out1_sub.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,18 +176,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
     sys.stdout.write('<?xml version="1.0" ?>\n')
     rootObj.export(sys.stdout, 0, name_=rootTag,
         namespacedef_='',
         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'people'
+        rootClass = supermod.people
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+    content = etree_.tostring(rootElement, pretty_print=True,
+        xml_declaration=True, encoding="utf-8")
+    sys.stdout.write(content)
+    sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'people'
```

### Comparing `generateDS-2.8b/tests/anysimpletype1_sup.py` & `generateDS-2.9a/tests/anysimpletype1_sup.py`

 * *Files 10% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -494,74 +527,76 @@
         else:
             return test1element(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_test1member(self): return self.test1member
     def set_test1member(self, test1member): self.test1member = test1member
     def get_test1attribute(self): return self.test1attribute
     def set_test1attribute(self, test1attribute): self.test1attribute = test1attribute
+    def hasContent_(self):
+        if (
+            self.test1member is not None
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='test1element', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='test1element')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='', name_='test1element'):
         if self.test1attribute is not None and 'test1attribute' not in already_processed:
-            already_processed.append('test1attribute')
+            already_processed.add('test1attribute')
             outfile.write(' test1attribute=%s' % (quote_attrib(self.test1attribute), ))
     def exportChildren(self, outfile, level, namespace_='', name_='test1element', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.test1member is not None:
             self.test1member.export(outfile, level, namespace_, name_='test1member', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.test1member is not None
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='test1element'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         if self.test1attribute is not None and 'test1attribute' not in already_processed:
-            already_processed.append('test1attribute')
+            already_processed.add('test1attribute')
             showIndent(outfile, level)
             outfile.write('test1attribute = %s,\n' % (self.test1attribute,))
     def exportLiteralChildren(self, outfile, level, name_):
         if self.test1member is not None:
             showIndent(outfile, level)
             outfile.write('test1member=model_.cimAnySimpleType(\n')
             self.test1member.exportLiteral(outfile, level, name_='test1member')
             showIndent(outfile, level)
             outfile.write('),\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('test1attribute', node)
         if value is not None and 'test1attribute' not in already_processed:
-            already_processed.append('test1attribute')
+            already_processed.add('test1attribute')
             self.test1attribute = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'test1member':
             obj_ = cimAnySimpleType.factory()
             obj_.build(child_)
             self.set_test1member(obj_)
 # end class test1element
@@ -582,22 +617,29 @@
         else:
             return cimAnySimpleType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
     def get_anyAttributes_(self): return self.anyAttributes_
     def set_anyAttributes_(self, anyAttributes_): self.anyAttributes_ = anyAttributes_
+    def hasContent_(self):
+        if (
+            self.valueOf_
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='', name_='cimAnySimpleType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='cimAnySimpleType')
         if self.hasContent_():
             outfile.write('>')
             outfile.write(str(self.valueOf_).encode(ExternalEncoding))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -608,61 +650,56 @@
             xsinamespaceprefix = 'xsi'
             xsinamespace1 = 'http://www.w3.org/2001/XMLSchema-instance'
             xsinamespace2 = '{%s}' % (xsinamespace1, )
             if name.startswith(xsinamespace2):
                 name1 = name[len(xsinamespace2):]
                 name2 = '%s:%s' % (xsinamespaceprefix, name1, )
                 if name2 not in already_processed:
-                    already_processed.append(name2)
+                    already_processed.add(name2)
                     outfile.write(' %s=%s' % (name2, quote_attrib(value), ))
             else:
                 mo = re_.match(Namespace_extract_pat_, name)
                 if mo is not None:
                     namespace, name = mo.group(1, 2)
                     if name not in already_processed:
-                        already_processed.append(name)
+                        already_processed.add(name)
                         if namespace == 'http://www.w3.org/XML/1998/namespace':
                             outfile.write(' %s=%s' % (
                                 name, quote_attrib(value), ))
                         else:
                             unique_counter += 1
                             outfile.write(' xmlns:yyy%d="%s"' % (
                                 unique_counter, namespace, ))
                             outfile.write(' yyy%d:%s=%s' % (
                                 unique_counter, name, quote_attrib(value), ))
                 else:
                     if name not in already_processed:
-                        already_processed.append(name)
+                        already_processed.add(name)
                         outfile.write(' %s=%s' % (
                             name, quote_attrib(value), ))
         pass
     def exportChildren(self, outfile, level, namespace_='', name_='cimAnySimpleType', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-            self.valueOf_
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='cimAnySimpleType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
         showIndent(outfile, level)
         outfile.write('valueOf_ = """%s""",\n' % (self.valueOf_,))
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         for name, value in self.anyAttributes_.items():
             showIndent(outfile, level)
             outfile.write('%s = "%s",\n' % (name, value,))
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         self.valueOf_ = get_all_text_(node)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         self.anyAttributes_ = {}
         for name, value in attrs.items():
@@ -709,14 +746,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'test1element'
+        rootClass = test1element
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'test1element'
```

### Comparing `generateDS-2.8b/tests/test.py` & `generateDS-2.9a/tests/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 import sys
 import subprocess
 import getopt
 import unittest
+from lxml import etree
 
 
 class GenTest(unittest.TestCase):
     def execute(self, cmd, cwd=None):
         p = subprocess.Popen(cmd, cwd=cwd,
             stdout=subprocess.PIPE, stderr=subprocess.PIPE,
             shell=True)
@@ -224,15 +225,15 @@
         content1 = infile.read()
         infile.close()
         infile = open('literal2.py', 'r')
         content2 = infile.read()
         infile.close()
         self.failUnlessEqual(content1, content2)
 
-    def test_010_extensions(self):
+    def test_010_simplecontent_restriction(self):
         cmdTempl = ('python generateDS.py --no-dates --no-versions '
             '--silence --member-specs=list -f '
             '-o tests/%s2_sup.py -s tests/%s2_sub.py '
             '--super=%s2_sup tests/%s.xsd'
             )
         t_ = 'simplecontent_restriction'
         cmd = cmdTempl % (t_, t_, t_, t_, )
@@ -379,14 +380,42 @@
         cmd = 'diff %s1_sup.py %s2_sup.py' % (t_, t_, )
         result, err = self.execute(cmd)
         self.check_result(result, err, ('sys.stdout.write',))
         cmd = 'diff %s1_sub.py %s2_sub.py' % (t_, t_, )
         result, err = self.execute(cmd)
         self.check_result(result, err, ())
 
+    def test_019_to_etree(self):
+        cmdTempl = ('python generateDS.py --no-dates --no-versions '
+            '--silence --member-specs=list -f '
+            '-o tests/%s2_sup.py -s tests/%s2_sub.py '
+            '--export="etree" --silence '
+            '--super=%s2_sup '
+            'tests/%s.xsd'
+            )
+        t_ = 'to_etree'
+        cmd = cmdTempl % (t_, t_, t_, t_, )
+        result, _ = self.execute(cmd, cwd='..')
+        cmd = 'diff %s1_sup.py %s2_sup.py' % (t_, t_, )
+        result, err = self.execute(cmd)
+        self.check_result(result, err, ('sys.stdout.write',))
+        cmd = 'diff %s1_sub.py %s2_sub.py' % (t_, t_, )
+        result, err = self.execute(cmd)
+        self.check_result(result, err, ())
+        import to_etree2_sup
+        rootObj, rootElement = to_etree2_sup.parseEtree('to_etree.xml')
+        content = etree.tostring(rootElement, pretty_print=True,
+            xml_declaration=True, encoding="utf-8")
+        outfile = open('to_etree2.xml', 'w')
+        outfile.write(content)
+        outfile.close()
+        cmd = 'diff %s1.xml %s2.xml' % (t_, t_, )
+        result, err = self.execute(cmd)
+        self.check_result(result, err, ())
+
     def check_result(self, result, err, ignore_strings):
         self.failUnlessEqual(len(result), 0)
         self.failUnlessEqual(len(err), 0)
         return True
 ##         if len(err) > 0:
 ##             return False
 ##         lines = result.split('\n')
```

### Comparing `generateDS-2.8b/tests/anywildcard.xsd` & `generateDS-2.9a/tests/anywildcard.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/people_procincl_b.xsd` & `generateDS-2.9a/tests/people_procincl_b.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/people_procincl_a.xsd` & `generateDS-2.9a/tests/people_procincl_a.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/simplecontent_restriction1_sub.py` & `generateDS-2.9a/tests/simplecontent_restriction1_sub.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,18 +113,36 @@
     rootObj.build(rootNode)
     # Enable Python to collect the space used by the DOM.
     doc = None
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
-    doc = None
     return rootObj
 
 
+def parseEtree(inFilename):
+    doc = parsexml_(inFilename)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'IdentifierType'
+        rootClass = supermod.IdentifierType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'IdentifierType'
```

### Comparing `generateDS-2.8b/tests/valueof.xsd` & `generateDS-2.9a/tests/valueof.xsd`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/tests/abstract_type2_sup.py` & `generateDS-2.9a/tests/abstract_type2_sup.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             for value in values:
                 try:
                     fvalue = float(value)
                 except (TypeError, ValueError), exp:
                     raise_parse_error(node, 'Requires sequence of doubles')
             return input_data
         def gds_format_boolean(self, input_data, input_name=''):
-            return '%s' % input_data
+            return ('%s' % input_data).lower()
         def gds_validate_boolean(self, input_data, node, input_name=''):
             return input_data
         def gds_format_boolean_list(self, input_data, input_name=''):
             return '%s' % input_data
         def gds_validate_boolean_list(self, input_data, node, input_name=''):
             values = input_data.split()
             for value in values:
@@ -427,14 +427,47 @@
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeDouble:
             outfile.write('<%s>%g</%s>' %
                 (self.name, self.value, self.name))
         elif self.content_type == MixedContainer.TypeBase64:
             outfile.write('<%s>%s</%s>' %
                 (self.name, base64.b64encode(self.value), self.name))
+    def to_etree(self, element):
+        if self.category == MixedContainer.CategoryText:
+            # Prevent exporting empty content as empty lines.
+            if self.value.strip():
+                if len(element) > 0:
+                    if element[-1].tail is None:
+                        element[-1].tail = self.value
+                    else:
+                        element[-1].tail += self.value
+                else:
+                    if element.text is None:
+                        element.text = self.value
+                    else:
+                        element.text += self.value
+        elif self.category == MixedContainer.CategorySimple:
+            subelement = etree_.SubElement(element, '%s' % self.name)
+            subelement.text = self.to_etree_simple()
+        else:    # category == MixedContainer.CategoryComplex
+            self.value.to_etree(element)
+    def to_etree_simple(self):
+        if self.content_type == MixedContainer.TypeString:
+            text = self.value
+        elif (self.content_type == MixedContainer.TypeInteger or
+                self.content_type == MixedContainer.TypeBoolean):
+            text = '%d' % self.value
+        elif (self.content_type == MixedContainer.TypeFloat or
+                self.content_type == MixedContainer.TypeDecimal):
+            text = '%f' % self.value
+        elif self.content_type == MixedContainer.TypeDouble:
+            text = '%g' % self.value
+        elif self.content_type == MixedContainer.TypeBase64:
+            text = '%s' % base64.b64encode(self.value)
+        return text
     def exportLiteral(self, outfile, level, name):
         if self.category == MixedContainer.CategoryText:
             showIndent(outfile, level)
             outfile.write('model_.MixedContainer(%d, %d, "%s", "%s"),\n'
                 % (self.category, self.content_type, self.name, self.value))
         elif self.category == MixedContainer.CategorySimple:
             showIndent(outfile, level)
@@ -495,22 +528,29 @@
         else:
             return carrierType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_fleet(self): return self.fleet
     def set_fleet(self, fleet): self.fleet = fleet
     def add_fleet(self, value): self.fleet.append(value)
     def insert_fleet(self, index, value): self.fleet[index] = value
+    def hasContent_(self):
+        if (
+            self.fleet
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='target:', name_='carrierType', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='carrierType')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
@@ -520,24 +560,18 @@
     def exportChildren(self, outfile, level, namespace_='target:', name_='carrierType', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         for fleet_ in self.get_fleet():
             fleet_.export(outfile, level, namespace_, name_='fleet', pretty_print=pretty_print)
-    def hasContent_(self):
-        if (
-            self.fleet
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='carrierType'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         showIndent(outfile, level)
         outfile.write('fleet=[\n')
@@ -548,15 +582,16 @@
             fleet_.exportLiteral(outfile, level, name_='Vehicle')
             showIndent(outfile, level)
             outfile.write('),\n')
         level -= 1
         showIndent(outfile, level)
         outfile.write('],\n')
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         pass
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         if nodeName_ == 'fleet':
@@ -591,62 +626,64 @@
         if Vehicle.subclass:
             return Vehicle.subclass(*args_, **kwargs_)
         else:
             return Vehicle(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
+    def hasContent_(self):
+        if (
+
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='target:', name_='Vehicle', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='Vehicle')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='target:', name_='Vehicle'):
         if self.extensiontype_ is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             outfile.write(' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"')
             outfile.write(' xsi:type="%s"' % self.extensiontype_)
         pass
     def exportChildren(self, outfile, level, namespace_='target:', name_='Vehicle', fromsubclass_=False, pretty_print=True):
         pass
-    def hasContent_(self):
-        if (
-
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='Vehicle'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         pass
     def exportLiteralChildren(self, outfile, level, name_):
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('xsi:type', node)
         if value is not None and 'xsi:type' not in already_processed:
-            already_processed.append('xsi:type')
+            already_processed.add('xsi:type')
             self.extensiontype_ = value
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         pass
 # end class Vehicle
 
 
 class Car(Vehicle):
@@ -659,53 +696,55 @@
         pass
     def factory(*args_, **kwargs_):
         if Car.subclass:
             return Car.subclass(*args_, **kwargs_)
         else:
             return Car(*args_, **kwargs_)
     factory = staticmethod(factory)
+    def hasContent_(self):
+        if (
+            super(Car, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='target:', name_='Car', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='Car')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='target:', name_='Car'):
         super(Car, self).exportAttributes(outfile, level, already_processed, namespace_, name_='Car')
     def exportChildren(self, outfile, level, namespace_='target:', name_='Car', fromsubclass_=False, pretty_print=True):
         super(Car, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         pass
-    def hasContent_(self):
-        if (
-            super(Car, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='Car'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(Car, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(Car, self).exportLiteralChildren(outfile, level, name_)
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(Car, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         super(Car, self).buildChildren(child_, node, nodeName_, True)
@@ -723,53 +762,55 @@
         pass
     def factory(*args_, **kwargs_):
         if Plane.subclass:
             return Plane.subclass(*args_, **kwargs_)
         else:
             return Plane(*args_, **kwargs_)
     factory = staticmethod(factory)
+    def hasContent_(self):
+        if (
+            super(Plane, self).hasContent_()
+            ):
+            return True
+        else:
+            return False
     def export(self, outfile, level, namespace_='target:', name_='Plane', namespacedef_='', pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespace_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
-        already_processed = []
+        already_processed = set()
         self.exportAttributes(outfile, level, already_processed, namespace_, name_='Plane')
         if self.hasContent_():
             outfile.write('>%s' % (eol_, ))
             self.exportChildren(outfile, level + 1, namespace_, name_, pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespace_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def exportAttributes(self, outfile, level, already_processed, namespace_='target:', name_='Plane'):
         super(Plane, self).exportAttributes(outfile, level, already_processed, namespace_, name_='Plane')
     def exportChildren(self, outfile, level, namespace_='target:', name_='Plane', fromsubclass_=False, pretty_print=True):
         super(Plane, self).exportChildren(outfile, level, namespace_, name_, True, pretty_print=pretty_print)
         pass
-    def hasContent_(self):
-        if (
-            super(Plane, self).hasContent_()
-            ):
-            return True
-        else:
-            return False
     def exportLiteral(self, outfile, level, name_='Plane'):
         level += 1
-        self.exportLiteralAttributes(outfile, level, [], name_)
+        already_processed = set()
+        self.exportLiteralAttributes(outfile, level, already_processed, name_)
         if self.hasContent_():
             self.exportLiteralChildren(outfile, level, name_)
     def exportLiteralAttributes(self, outfile, level, already_processed, name_):
         super(Plane, self).exportLiteralAttributes(outfile, level, already_processed, name_)
     def exportLiteralChildren(self, outfile, level, name_):
         super(Plane, self).exportLiteralChildren(outfile, level, name_)
         pass
     def build(self, node):
-        self.buildAttributes(node, node.attrib, [])
+        already_processed = set()
+        self.buildAttributes(node, node.attrib, already_processed)
         for child in node:
             nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
             self.buildChildren(child, node, nodeName_)
     def buildAttributes(self, node, attrs, already_processed):
         super(Plane, self).buildAttributes(node, attrs, already_processed)
     def buildChildren(self, child_, node, nodeName_, fromsubclass_=False):
         super(Plane, self).buildChildren(child_, node, nodeName_, True)
@@ -814,14 +855,33 @@
 ##     sys.stdout.write('<?xml version="1.0" ?>\n')
 ##     rootObj.export(sys.stdout, 0, name_=rootTag,
 ##         namespacedef_='',
 ##         pretty_print=True)
     return rootObj
 
 
+def parseEtree(inFileName):
+    doc = parsexml_(inFileName)
+    rootNode = doc.getroot()
+    rootTag, rootClass = get_root_tag(rootNode)
+    if rootClass is None:
+        rootTag = 'carrier'
+        rootClass = carrierType
+    rootObj = rootClass.factory()
+    rootObj.build(rootNode)
+    # Enable Python to collect the space used by the DOM.
+    doc = None
+    rootElement = rootObj.to_etree(None, name_=rootTag)
+##     content = etree_.tostring(rootElement, pretty_print=True,
+##         xml_declaration=True, encoding="utf-8")
+##     sys.stdout.write(content)
+##     sys.stdout.write('\n')
+    return rootObj, rootElement
+
+
 def parseString(inString):
     from StringIO import StringIO
     doc = parsexml_(StringIO(inString))
     rootNode = doc.getroot()
     rootTag, rootClass = get_root_tag(rootNode)
     if rootClass is None:
         rootTag = 'carrier'
```

### Comparing `generateDS-2.8b/LICENSE` & `generateDS-2.9a/LICENSE`

 * *Files identical despite different names*

### Comparing `generateDS-2.8b/process_includes.py` & `generateDS-2.9a/process_includes.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #
 # Globals and constants
 
 #
 # Do not modify the following VERSION comments.
 # Used by updateversion.py.
 ##VERSION##
-VERSION = '2.8b'
+VERSION = '2.9a'
 ##VERSION##
 
 Namespaces = {'xs': 'http://www.w3.org/2001/XMLSchema'}
 Xsd_namespace_uri = 'http://www.w3.org/2001/XMLSchema'
 
 
 #
```

