# Comparing `tmp/rnginline-0.0.2.tar.gz` & `tmp/rnginline-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rnginline-0.0.2.tar", last modified: Sat May 30 15:14:39 2015, max compression
+gzip compressed data, was "rnginline-1.0.0rc1.tar", max compression
```

## Comparing `rnginline-0.0.2.tar` & `rnginline-1.0.0rc1.tar`

### file list

```diff
@@ -1,183 +1,126 @@
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/
--rw-r--r--   0 hal        (501) staff       (20)      109 2015-05-30 13:36:05.000000 rnginline-0.0.2/.coveragerc
--rw-r--r--   0 hal        (501) staff       (20)      321 2015-02-08 23:26:10.000000 rnginline-0.0.2/.editorconfig
--rw-r--r--   0 hal        (501) staff       (20)      134 2015-05-30 13:36:05.000000 rnginline-0.0.2/.gitignore
--rw-r--r--   0 hal        (501) staff       (20)     1669 2015-05-30 13:36:05.000000 rnginline-0.0.2/.travis.yml
--rw-r--r--   0 hal        (501) staff       (20)      329 2015-05-30 15:13:22.000000 rnginline-0.0.2/CHANGELOG.rst
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/docs/
--rw-r--r--   0 hal        (501) staff       (20)     1419 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/api.rst
--rw-r--r--   0 hal        (501) staff       (20)     8705 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/conf.py
--rw-r--r--   0 hal        (501) staff       (20)      326 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/doctest
--rw-r--r--   0 hal        (501) staff       (20)      349 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/external.rng
--rw-r--r--   0 hal        (501) staff       (20)     4191 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/from-cmdline.rst
--rw-r--r--   0 hal        (501) staff       (20)     8618 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/from-python.rst
--rw-r--r--   0 hal        (501) staff       (20)     1337 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/index.rst
--rw-r--r--   0 hal        (501) staff       (20)      395 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/installing.rst
--rw-r--r--   0 hal        (501) staff       (20)     6774 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/Makefile
--rw-r--r--   0 hal        (501) staff       (20)      915 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/quickstart.rst
--rwxr-xr-x   0 hal        (501) staff       (20)     1076 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/rnginline-example.sh
--rw-r--r--   0 hal        (501) staff       (20)      355 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/schema.rng
--rw-r--r--   0 hal        (501) staff       (20)     3973 2015-05-30 13:36:05.000000 rnginline-0.0.2/docs/uri-resolution.rst
--rw-r--r--   0 hal        (501) staff       (20)      579 2015-05-30 13:36:05.000000 rnginline-0.0.2/LICENSE.txt
--rw-r--r--   0 hal        (501) staff       (20)      202 2015-05-30 13:36:05.000000 rnginline-0.0.2/MANIFEST.in
--rw-r--r--   0 hal        (501) staff       (20)     7501 2015-05-30 15:14:39.000000 rnginline-0.0.2/PKG-INFO
--rw-r--r--   0 hal        (501) staff       (20)     5084 2015-05-30 13:36:05.000000 rnginline-0.0.2/README.rst
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/requirements/
--rw-r--r--   0 hal        (501) staff       (20)      186 2015-05-30 13:36:05.000000 rnginline-0.0.2/requirements/all.txt
--rw-r--r--   0 hal        (501) staff       (20)        4 2015-05-30 13:36:05.000000 rnginline-0.0.2/requirements/dev.txt
--rw-r--r--   0 hal        (501) staff       (20)       33 2015-05-30 13:36:05.000000 rnginline-0.0.2/requirements/docs.txt
--rw-r--r--   0 hal        (501) staff       (20)       16 2015-05-30 13:36:05.000000 rnginline-0.0.2/requirements/install.txt
--rw-r--r--   0 hal        (501) staff       (20)       24 2015-05-30 13:36:05.000000 rnginline-0.0.2/requirements/invoke-tasks.txt
--rw-r--r--   0 hal        (501) staff       (20)        7 2015-05-30 13:36:05.000000 rnginline-0.0.2/requirements/pep8.txt
--rw-r--r--   0 hal        (501) staff       (20)       31 2015-05-30 13:36:05.000000 rnginline-0.0.2/requirements/readme.txt
--rw-r--r--   0 hal        (501) staff       (20)       28 2015-05-30 13:36:05.000000 rnginline-0.0.2/requirements/test.txt
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/
--rw-r--r--   0 hal        (501) staff       (20)    32323 2015-05-30 15:03:09.000000 rnginline-0.0.2/rnginline/__init__.py
--rw-r--r--   0 hal        (501) staff       (20)     4718 2015-05-30 13:36:05.000000 rnginline-0.0.2/rnginline/cmdline.py
--rw-r--r--   0 hal        (501) staff       (20)      456 2015-05-30 13:36:05.000000 rnginline-0.0.2/rnginline/constants.py
--rw-r--r--   0 hal        (501) staff       (20)     1312 2015-05-30 13:36:05.000000 rnginline-0.0.2/rnginline/exceptions.py
--rw-r--r--   0 hal        (501) staff       (20)     1997 2015-05-30 13:36:05.000000 rnginline-0.0.2/rnginline/postprocess.py
--rw-r--r--   0 hal        (501) staff       (20)     9430 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/regexbuilder.py
--rw-r--r--   0 hal        (501) staff       (20)     9530 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/relaxng.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/
--rw-r--r--   0 hal        (501) staff       (20)        0 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/__init__.py
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/datatype-library-inheritance/
--rw-r--r--   0 hal        (501) staff       (20)      396 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/datatype-library-inheritance/base-external.rng
--rw-r--r--   0 hal        (501) staff       (20)      287 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/datatype-library-inheritance/base-included.rng
--rw-r--r--   0 hal        (501) staff       (20)      269 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/datatype-library-inheritance/external.rng
--rw-r--r--   0 hal        (501) staff       (20)      349 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/datatype-library-inheritance/included.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/datatype-library-propagation/
--rw-r--r--   0 hal        (501) staff       (20)      171 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/datatype-library-propagation/a.rng
--rw-r--r--   0 hal        (501) staff       (20)      934 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/datatype-library-propagation/b.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/include-invalid-xml/
--rw-r--r--   0 hal        (501) staff       (20)       20 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/include-invalid-xml/invalid-xml.rng
--rw-r--r--   0 hal        (501) staff       (20)      136 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/include-invalid-xml/ok.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/include-non-rng-xml/
--rw-r--r--   0 hal        (501) staff       (20)       29 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/include-non-rng-xml/invalid-xml.rng
--rw-r--r--   0 hal        (501) staff       (20)      136 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/include-non-rng-xml/ok.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/include-override-define/
--rw-r--r--   0 hal        (501) staff       (20)      120 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/include-override-define/included.rng
--rw-r--r--   0 hal        (501) staff       (20)      306 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/include-override-define/start.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/include-override-start/
--rw-r--r--   0 hal        (501) staff       (20)      120 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/include-override-start/included.rng
--rw-r--r--   0 hal        (501) staff       (20)      292 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/include-override-start/start.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/inline-non-grammar-els/
--rw-r--r--   0 hal        (501) staff       (20)       89 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/inline-non-grammar-els/foo-el.rng
--rw-r--r--   0 hal        (501) staff       (20)      131 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/inline-non-grammar-els/grammar-foo-el.rng
--rw-r--r--   0 hal        (501) staff       (20)      142 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/inline-non-grammar-els/illegal.rng
--rw-r--r--   0 hal        (501) staff       (20)      144 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/inline-non-grammar-els/legal.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/loops/
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/loops/foo/
--rw-r--r--   0 hal        (501) staff       (20)      118 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/loops/foo/a.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/loops/foo/bar/
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/loops/foo/bar/baz/
--rw-r--r--   0 hal        (501) staff       (20)      141 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/loops/foo/bar/baz/b.rng
--rw-r--r--   0 hal        (501) staff       (20)      114 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/loops/start.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/multiple-ref-1-fetch/
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/multiple-ref-1-fetch/a/
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/multiple-ref-1-fetch/a/b/
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/multiple-ref-1-fetch/a/b/c/
--rw-r--r--   0 hal        (501) staff       (20)      269 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/multiple-ref-1-fetch/a/b/c/popular.rng
--rw-r--r--   0 hal        (501) staff       (20)       97 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/multiple-ref-1-fetch/indirect.rng
--rw-r--r--   0 hal        (501) staff       (20)      534 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/multiple-ref-1-fetch/schema.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/datatype-library-external/
--rw-r--r--   0 hal        (501) staff       (20)      284 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/datatype-library-external/external.rng
--rw-r--r--   0 hal        (501) staff       (20)      294 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/datatype-library-external/included.rng
--rw-r--r--   0 hal        (501) staff       (20)       81 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/datatype-library-external/positive.xml
--rw-r--r--   0 hal        (501) staff       (20)      459 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/datatype-library-external/schema.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-1/
--rw-r--r--   0 hal        (501) staff       (20)       21 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-1/baz.rnc
--rw-r--r--   0 hal        (501) staff       (20)      127 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-1/baz.rng
--rw-r--r--   0 hal        (501) staff       (20)       87 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-1/negative-1.xml
--rw-r--r--   0 hal        (501) staff       (20)       87 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-1/negative-2.xml
--rw-r--r--   0 hal        (501) staff       (20)       73 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-1/positive-1.xml
--rw-r--r--   0 hal        (501) staff       (20)      117 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-1/positive-2.xml
--rw-r--r--   0 hal        (501) staff       (20)       98 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-1/README.rst
--rw-r--r--   0 hal        (501) staff       (20)      132 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-1/schema.rnc
--rw-r--r--   0 hal        (501) staff       (20)      445 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-1/schema.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-2/
--rw-r--r--   0 hal        (501) staff       (20)       42 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-2/negative-1.xml
--rw-r--r--   0 hal        (501) staff       (20)       33 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-2/positive-1.xml
--rw-r--r--   0 hal        (501) staff       (20)       33 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-2/positive-2.xml
--rw-r--r--   0 hal        (501) staff       (20)      303 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-2/README.rst
--rw-r--r--   0 hal        (501) staff       (20)      263 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-2/schema.rng
--rw-r--r--   0 hal        (501) staff       (20)      211 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-2/that.rng
--rw-r--r--   0 hal        (501) staff       (20)      157 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-2/this.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/
--rw-r--r--   0 hal        (501) staff       (20)      351 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/1-default-xmlns-unprefixed-names.rng
--rw-r--r--   0 hal        (501) staff       (20)      255 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/2-ns-attributes.rng
--rw-r--r--   0 hal        (501) staff       (20)      308 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/3-qnames.rng
--rw-r--r--   0 hal        (501) staff       (20)      128 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/negative-1.1.xml
--rw-r--r--   0 hal        (501) staff       (20)      113 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/negative-1.2.xml
--rw-r--r--   0 hal        (501) staff       (20)      129 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/negative-2.1.xml
--rw-r--r--   0 hal        (501) staff       (20)      142 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/negative-2.2.xml
--rw-r--r--   0 hal        (501) staff       (20)      186 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/negative-3.1.xml
--rw-r--r--   0 hal        (501) staff       (20)      186 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/negative-3.2.xml
--rw-r--r--   0 hal        (501) staff       (20)      151 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/negative-3.3.xml
--rw-r--r--   0 hal        (501) staff       (20)      169 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/negative-3.4.xml
--rw-r--r--   0 hal        (501) staff       (20)       77 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/positive-1.1.xml
--rw-r--r--   0 hal        (501) staff       (20)      104 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/positive-2.1.xml
--rw-r--r--   0 hal        (501) staff       (20)      133 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/positive-3.1.xml
--rw-r--r--   0 hal        (501) staff       (20)      682 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/README.rst
--rw-r--r--   0 hal        (501) staff       (20)      822 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/schema.rng
--rw-r--r--   0 hal        (501) staff       (20)      352 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/tmp.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-ns-override/
--rw-r--r--   0 hal        (501) staff       (20)      256 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-ns-override/external.rng
--rw-r--r--   0 hal        (501) staff       (20)       76 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-ns-override/negative-1.xml
--rw-r--r--   0 hal        (501) staff       (20)       76 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-ns-override/positive-1.xml
--rw-r--r--   0 hal        (501) staff       (20)      372 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/external-ref-ns-override/schema.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/foreign-attributes/
--rw-r--r--   0 hal        (501) staff       (20)      235 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/foreign-attributes/lvl2.rng
--rw-r--r--   0 hal        (501) staff       (20)       88 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/foreign-attributes/lvl3.rng
--rw-r--r--   0 hal        (501) staff       (20)       30 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/foreign-attributes/positive-1.xml
--rw-r--r--   0 hal        (501) staff       (20)      532 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/foreign-attributes/schema.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/include-1/
--rw-r--r--   0 hal        (501) staff       (20)      330 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/include-1/included.rng
--rw-r--r--   0 hal        (501) staff       (20)       37 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/include-1/negative-1.xml
--rw-r--r--   0 hal        (501) staff       (20)       23 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/include-1/positive-1.xml
--rw-r--r--   0 hal        (501) staff       (20)       23 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/include-1/positive-2.xml
--rw-r--r--   0 hal        (501) staff       (20)      273 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/include-1/schema.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/overrides/
--rw-r--r--   0 hal        (501) staff       (20)      892 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/overrides/included.rng
--rw-r--r--   0 hal        (501) staff       (20)      743 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/overrides/positive.xml
--rw-r--r--   0 hal        (501) staff       (20)     1647 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/overrides/schema.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/a/
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/a/b/
--rw-r--r--   0 hal        (501) staff       (20)       89 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/a/b/baz.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/a/b/c/
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/a/b/c/d/
--rw-r--r--   0 hal        (501) staff       (20)      284 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/a/b/c/d/foo.rng
--rw-r--r--   0 hal        (501) staff       (20)       86 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/positive-1.xml
--rw-r--r--   0 hal        (501) staff       (20)      151 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/schema.rng
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/x/
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/x/y/
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/x/y/z/
--rw-r--r--   0 hal        (501) staff       (20)      139 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/data/testcases/xml-base/x/y/z/bar.rng
--rw-r--r--   0 hal        (501) staff       (20)      638 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/mini_validator.py
--rw-r--r--   0 hal        (501) staff       (20)     7741 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/test_cmdline.py
--rw-r--r--   0 hal        (501) staff       (20)     1760 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/test_propagate_datatypelibrary.py
--rw-r--r--   0 hal        (501) staff       (20)     6375 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/test_regexbuilder.py
--rw-r--r--   0 hal        (501) staff       (20)    17416 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/test_rnginline.py
--rw-r--r--   0 hal        (501) staff       (20)     7468 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/test_uri.py
--rw-r--r--   0 hal        (501) staff       (20)     6035 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/test_uri_regex.py
--rw-r--r--   0 hal        (501) staff       (20)     5577 2015-05-30 13:36:06.000000 rnginline-0.0.2/rnginline/test/test_urlhandlers.py
--rw-r--r--   0 hal        (501) staff       (20)     5073 2015-05-30 13:36:07.000000 rnginline-0.0.2/rnginline/uri.py
--rw-r--r--   0 hal        (501) staff       (20)     6944 2015-05-30 13:36:07.000000 rnginline-0.0.2/rnginline/uri_regex.py
--rw-r--r--   0 hal        (501) staff       (20)    10320 2015-05-30 13:36:07.000000 rnginline-0.0.2/rnginline/urlhandlers.py
-drwxr-xr-x   0 hal        (501) staff       (20)        0 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline.egg-info/
--rw-r--r--   0 hal        (501) staff       (20)        1 2015-05-30 15:14:35.000000 rnginline-0.0.2/rnginline.egg-info/dependency_links.txt
--rw-r--r--   0 hal        (501) staff       (20)       54 2015-05-30 15:14:35.000000 rnginline-0.0.2/rnginline.egg-info/entry_points.txt
--rw-r--r--   0 hal        (501) staff       (20)     7501 2015-05-30 15:14:35.000000 rnginline-0.0.2/rnginline.egg-info/PKG-INFO
--rw-r--r--   0 hal        (501) staff       (20)       52 2015-05-30 15:14:35.000000 rnginline-0.0.2/rnginline.egg-info/requires.txt
--rw-r--r--   0 hal        (501) staff       (20)     6257 2015-05-30 15:14:39.000000 rnginline-0.0.2/rnginline.egg-info/SOURCES.txt
--rw-r--r--   0 hal        (501) staff       (20)       10 2015-05-30 15:14:35.000000 rnginline-0.0.2/rnginline.egg-info/top_level.txt
--rw-r--r--   0 hal        (501) staff       (20)       88 2015-05-30 15:14:39.000000 rnginline-0.0.2/setup.cfg
--rw-r--r--   0 hal        (501) staff       (20)     2346 2015-05-30 13:36:07.000000 rnginline-0.0.2/setup.py
--rw-r--r--   0 hal        (501) staff       (20)     7631 2015-05-30 14:38:50.000000 rnginline-0.0.2/tasks.py
--rw-r--r--   0 hal        (501) staff       (20)      885 2015-03-29 17:14:52.000000 rnginline-0.0.2/TODO.txt
--rw-r--r--   0 hal        (501) staff       (20)      516 2015-05-30 13:36:07.000000 rnginline-0.0.2/tox-dist.ini
--rw-r--r--   0 hal        (501) staff       (20)      299 2015-05-30 13:36:07.000000 rnginline-0.0.2/tox-wheelcache.ini
--rw-r--r--   0 hal        (501) staff       (20)      690 2015-05-30 13:36:07.000000 rnginline-0.0.2/tox.ini
+-rw-r--r--   0        0        0      579 2023-05-07 15:08:04.574971 rnginline-1.0.0rc1/LICENSE.txt
+-rw-r--r--   0        0        0     3579 2023-05-07 15:08:04.574971 rnginline-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     2856 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    41049 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/__init__.py
+-rw-r--r--   0        0        0     5760 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/cmdline.py
+-rw-r--r--   0        0        0      584 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/constants.py
+-rw-r--r--   0        0        0     1705 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/exceptions.py
+-rw-r--r--   0        0        0     2428 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/postprocess.py
+-rw-r--r--   0        0        0        0 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/py.typed
+-rw-r--r--   0        0        0    10316 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/regexbuilder.py
+-rw-r--r--   0        0        0     9530 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/relaxng.rng
+-rw-r--r--   0        0        0        0 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/__init__.py
+-rw-r--r--   0        0        0      396 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/datatype-library-inheritance/base-external.rng
+-rw-r--r--   0        0        0      287 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/datatype-library-inheritance/base-included.rng
+-rw-r--r--   0        0        0      269 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/datatype-library-inheritance/external.rng
+-rw-r--r--   0        0        0      349 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/datatype-library-inheritance/included.rng
+-rw-r--r--   0        0        0      171 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/datatype-library-propagation/a.rng
+-rw-r--r--   0        0        0      934 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/datatype-library-propagation/b.rng
+-rw-r--r--   0        0        0       20 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/include-invalid-xml/invalid-xml.rng
+-rw-r--r--   0        0        0      136 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/include-invalid-xml/ok.rng
+-rw-r--r--   0        0        0       29 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/include-non-rng-xml/invalid-xml.rng
+-rw-r--r--   0        0        0      136 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/include-non-rng-xml/ok.rng
+-rw-r--r--   0        0        0      120 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/include-override-define/included.rng
+-rw-r--r--   0        0        0      306 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/include-override-define/start.rng
+-rw-r--r--   0        0        0      120 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/include-override-start/included.rng
+-rw-r--r--   0        0        0      292 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/include-override-start/start.rng
+-rw-r--r--   0        0        0       89 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/inline-non-grammar-els/foo-el.rng
+-rw-r--r--   0        0        0      131 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/inline-non-grammar-els/grammar-foo-el.rng
+-rw-r--r--   0        0        0      142 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/inline-non-grammar-els/illegal.rng
+-rw-r--r--   0        0        0      144 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/inline-non-grammar-els/legal.rng
+-rw-r--r--   0        0        0      118 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/loops/foo/a.rng
+-rw-r--r--   0        0        0      141 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/loops/foo/bar/baz/b.rng
+-rw-r--r--   0        0        0      114 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/loops/start.rng
+-rw-r--r--   0        0        0      269 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/multiple-ref-1-fetch/a/b/c/popular.rng
+-rw-r--r--   0        0        0       97 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/multiple-ref-1-fetch/indirect.rng
+-rw-r--r--   0        0        0      534 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/multiple-ref-1-fetch/schema.rng
+-rw-r--r--   0        0        0      284 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/datatype-library-external/external.rng
+-rw-r--r--   0        0        0      294 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/datatype-library-external/included.rng
+-rw-r--r--   0        0        0       81 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/datatype-library-external/positive.xml
+-rw-r--r--   0        0        0      459 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/datatype-library-external/schema.rng
+-rw-r--r--   0        0        0       98 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-1/README.rst
+-rw-r--r--   0        0        0       21 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-1/baz.rnc
+-rw-r--r--   0        0        0      127 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-1/baz.rng
+-rw-r--r--   0        0        0       87 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-1/negative-1.xml
+-rw-r--r--   0        0        0       87 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-1/negative-2.xml
+-rw-r--r--   0        0        0       73 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-1/positive-1.xml
+-rw-r--r--   0        0        0      117 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-1/positive-2.xml
+-rw-r--r--   0        0        0      132 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-1/schema.rnc
+-rw-r--r--   0        0        0      445 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-1/schema.rng
+-rw-r--r--   0        0        0      303 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-2/README.rst
+-rw-r--r--   0        0        0       42 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-2/negative-1.xml
+-rw-r--r--   0        0        0       33 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-2/positive-1.xml
+-rw-r--r--   0        0        0       33 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-2/positive-2.xml
+-rw-r--r--   0        0        0      263 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-2/schema.rng
+-rw-r--r--   0        0        0      211 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-2/that.rng
+-rw-r--r--   0        0        0      157 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-2/this.rng
+-rw-r--r--   0        0        0      351 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/1-default-xmlns-unprefixed-names.rng
+-rw-r--r--   0        0        0      255 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/2-ns-attributes.rng
+-rw-r--r--   0        0        0      308 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/3-qnames.rng
+-rw-r--r--   0        0        0      682 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/README.rst
+-rw-r--r--   0        0        0      128 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/negative-1.1.xml
+-rw-r--r--   0        0        0      113 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/negative-1.2.xml
+-rw-r--r--   0        0        0      129 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/negative-2.1.xml
+-rw-r--r--   0        0        0      142 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/negative-2.2.xml
+-rw-r--r--   0        0        0      186 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/negative-3.1.xml
+-rw-r--r--   0        0        0      186 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/negative-3.2.xml
+-rw-r--r--   0        0        0      151 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/negative-3.3.xml
+-rw-r--r--   0        0        0      169 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/negative-3.4.xml
+-rw-r--r--   0        0        0       77 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/positive-1.1.xml
+-rw-r--r--   0        0        0      104 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/positive-2.1.xml
+-rw-r--r--   0        0        0      133 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/positive-3.1.xml
+-rw-r--r--   0        0        0      822 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/schema.rng
+-rw-r--r--   0        0        0      352 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/tmp.rng
+-rw-r--r--   0        0        0      256 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-ns-override/external.rng
+-rw-r--r--   0        0        0       76 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-ns-override/negative-1.xml
+-rw-r--r--   0        0        0       76 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-ns-override/positive-1.xml
+-rw-r--r--   0        0        0      372 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-ns-override/schema.rng
+-rw-r--r--   0        0        0      235 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/foreign-attributes/lvl2.rng
+-rw-r--r--   0        0        0       88 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/foreign-attributes/lvl3.rng
+-rw-r--r--   0        0        0       30 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/foreign-attributes/positive-1.xml
+-rw-r--r--   0        0        0      532 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/foreign-attributes/schema.rng
+-rw-r--r--   0        0        0      330 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-1/included.rng
+-rw-r--r--   0        0        0       37 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-1/negative-1.xml
+-rw-r--r--   0        0        0       23 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-1/positive-1.xml
+-rw-r--r--   0        0        0       23 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-1/positive-2.xml
+-rw-r--r--   0        0        0      273 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-1/schema.rng
+-rw-r--r--   0        0        0      403 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect/level-1-a.rng
+-rw-r--r--   0        0        0      904 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect/level-2-a.rng
+-rw-r--r--   0        0        0       40 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect/negative-1.xml
+-rw-r--r--   0        0        0       35 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect/negative-2.xml
+-rw-r--r--   0        0        0       22 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect/negative-3.xml
+-rw-r--r--   0        0        0      223 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect/other.rng
+-rw-r--r--   0        0        0       29 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect/positive-1.xml
+-rw-r--r--   0        0        0       35 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect/positive-2.xml
+-rw-r--r--   0        0        0      693 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect/schema.rng
+-rw-r--r--   0        0        0      373 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/level-1-a.rng
+-rw-r--r--   0        0        0      933 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/level-2-a.rng
+-rw-r--r--   0        0        0      390 2023-05-07 15:08:04.578971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/level-2-b.rng
+-rw-r--r--   0        0        0       41 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/negative-1.xml
+-rw-r--r--   0        0        0       47 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/negative-2.xml
+-rw-r--r--   0        0        0       35 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/negative-3.xml
+-rw-r--r--   0        0        0       33 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/negative-4.xml
+-rw-r--r--   0        0        0       26 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/negative-5.xml
+-rw-r--r--   0        0        0       26 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/negative-6.xml
+-rw-r--r--   0        0        0      187 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/positive-1.xml
+-rw-r--r--   0        0        0     1651 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/schema.rng
+-rw-r--r--   0        0        0      892 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/overrides/included.rng
+-rw-r--r--   0        0        0      743 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/overrides/positive.xml
+-rw-r--r--   0        0        0     1647 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/overrides/schema.rng
+-rw-r--r--   0        0        0       89 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/xml-base/a/b/baz.rng
+-rw-r--r--   0        0        0      284 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/xml-base/a/b/c/d/foo.rng
+-rw-r--r--   0        0        0       86 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/xml-base/positive-1.xml
+-rw-r--r--   0        0        0      151 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/xml-base/schema.rng
+-rw-r--r--   0        0        0      139 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/data/testcases/xml-base/x/y/z/bar.rng
+-rw-r--r--   0        0        0      683 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/mini_validator.py
+-rw-r--r--   0        0        0     8306 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/test_cmdline.py
+-rw-r--r--   0        0        0     1831 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/test_propagate_datatypelibrary.py
+-rw-r--r--   0        0        0     6784 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/test_regexbuilder.py
+-rw-r--r--   0        0        0    19628 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/test_rnginline.py
+-rw-r--r--   0        0        0     7992 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/test_uri.py
+-rw-r--r--   0        0        0     8750 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/test_uri_regex.py
+-rw-r--r--   0        0        0     4508 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/test/test_urlhandlers.py
+-rw-r--r--   0        0        0     5348 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/uri.py
+-rw-r--r--   0        0        0     7156 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/uri_regex.py
+-rw-r--r--   0        0        0     8749 2023-05-07 15:08:04.582971 rnginline-1.0.0rc1/rnginline/urlhandlers.py
+-rw-r--r--   0        0        0     5028 1970-01-01 00:00:00.000000 rnginline-1.0.0rc1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rnginline-0.0.2/LICENSE.txt` & `rnginline-1.0.0rc1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2015 Hal Blackburn
+Copyright 2023 Hal Blackburn
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
      http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rnginline-0.0.2/rnginline/exceptions.py` & `rnginline-1.0.0rc1/rnginline/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,16 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Sequence
+
 from lxml import etree
 
+if TYPE_CHECKING:
+    from rnginline import InlineContextToken
+
 
 class RelaxngInlineError(BaseException):
     pass
 
 
 class NoAvailableHandlerError(RelaxngInlineError):
     pass
@@ -19,31 +26,39 @@
 
 class DereferenceError(RelaxngInlineError):
     pass
 
 
 class InvalidGrammarError(BadXmlError):
     @classmethod
-    def from_bad_element(cls, el, msg):
-        return cls("{0} in {1} on line {2} {3}"
-                   .format(el.tag, el.getroottree().docinfo.URL or "??",
-                           el.sourceline or "??", msg))
+    def from_bad_element(cls, el: etree._Element, msg: str) -> InvalidGrammarError:
+        return cls(
+            "{0} in {1} on line {2} {3}".format(
+                el.tag, el.getroottree().docinfo.URL or "??", el.sourceline or "??", msg
+            )
+        )
 
 
 class SchemaIncludesSelfError(InvalidGrammarError, DereferenceError):
     @classmethod
-    def from_context_stack(cls, url, trigger_el, stack):
+    def from_context_stack(
+        cls,
+        url: str | None,
+        trigger_el: etree._Element | None,
+        stack: Sequence[tuple[str | None, InlineContextToken, etree._Element | None]],
+    ) -> SchemaIncludesSelfError:
         # Drop tokens from the stack and append the loop-creating el & url
         url_triggers = [(u, t) for (u, _, t) in stack] + [(url, trigger_el)]
 
-        loop = "".join(cls._format_url_trigger(u, t)
-                       for (u, t) in url_triggers)
+        loop = "".join(cls._format_url_trigger(u, t) for (u, t) in url_triggers)
 
-        return cls("A schema referenced itself, creating a loop:\n{0}"
-                   .format(loop))
+        return cls("A schema referenced itself, creating a loop:\n{0}".format(loop))
 
     @classmethod
-    def _format_url_trigger(cls, url, trigger_el):
+    def _format_url_trigger(
+        cls, url: str | None, trigger_el: etree._Element | None
+    ) -> str:
         if trigger_el is None:
-            return url
+            return str(url)
         return ":{0} <{1}> -> \n{2}".format(
-            trigger_el.sourceline, etree.QName(trigger_el).localname, url)
+            trigger_el.sourceline, etree.QName(trigger_el).localname, url
+        )
```

### Comparing `rnginline-0.0.2/rnginline/postprocess.py` & `rnginline-1.0.0rc1/rnginline/postprocess.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,74 @@
-from rnginline import etree
+from typing import Sequence
 
-from rnginline.constants import NSMAP, RNG_DATA_TAG, RNG_VALUE_TAG
+from lxml import etree
+from typing_extensions import Final, Protocol
 
+from rnginline.constants import NSMAP, RNG_DATA_TAG, RNG_VALUE_TAG
 
 __all__ = ["datatypelibrary"]
 
-_lookup_datatype_library = etree.XPath(
-    "string(ancestor-or-self::*[@datatypeLibrary][position()=1]"
-    "/@datatypeLibrary)")
-_data_value_els = etree.XPath("//rng:data|//rng:value", namespaces=NSMAP)
+_lookup_datatype_library: Final = etree.XPath(
+    "string(ancestor-or-self::*[@datatypeLibrary][position()=1]" "/@datatypeLibrary)"
+)
+_data_value_els: Final = etree.XPath("//rng:data|//rng:value", namespaces=NSMAP)
+
+
+class PostProcessor(Protocol):
+    def postprocess(self, grammar: etree._Element) -> etree._Element:
+        ...
 
 
-class PropagateDatatypeLibraryPostProcess(object):
+class PropagateDatatypeLibraryPostProcess(PostProcessor):
     """
     Implements the propagation part of simplification 4.3: datatypeLibrary
     attributes are resolved and explicitly set on each data and value element,
     then removed from all other elements.
 
     This can be used to work around `libxml2 not resolving datatypeLibrary
     attributes from div elements <libxml2 bug>`_.
 
     .. _libxml2 bug: https://bugzilla.gnome.org/show_bug.cgi?id=744146
     """
 
-    def lookup_datatypelibrary(self, element):
-        return _lookup_datatype_library(element)
+    def lookup_datatypelibrary(self, element: etree._Element) -> str:
+        lib = _lookup_datatype_library(element)
+        assert isinstance(lib, str)
+        return lib
 
-    def resolve_datatypelibrary(self, element):
+    def resolve_datatypelibrary(self, element: etree._Element) -> None:
         lib = self.lookup_datatypelibrary(element)
         element.attrib["datatypeLibrary"] = lib
 
-    def postprocess(self, grammar):
+    def postprocess(self, grammar: etree._Element) -> etree._Element:
         # Resolve the datatypeLibrary of all data and value elements
         for element in _data_value_els(grammar):
             self.resolve_datatypelibrary(element)
 
         # Strip datatypeLibrary from all other elements
         for element in grammar.iter():
-            if (element.tag not in [RNG_DATA_TAG, RNG_VALUE_TAG] and
-                    "datatypeLibrary" in element.attrib):
+            if (
+                element.tag not in [RNG_DATA_TAG, RNG_VALUE_TAG]
+                and "datatypeLibrary" in element.attrib
+            ):
                 del element.attrib["datatypeLibrary"]
 
         return grammar
 
-    def __call__(self, grammar):
+    def __call__(self, grammar: etree._Element) -> etree._Element:
         return self.postprocess(grammar)
 
 
-datatypelibrary = PropagateDatatypeLibraryPostProcess()
+datatypelibrary: Final = PropagateDatatypeLibraryPostProcess()
 """
 The default instance of :py:class:`PropagateDatatypeLibraryPostProcess`
 """
 
 
-def get_default_postprocessors():
+def get_default_postprocessors() -> Sequence[PostProcessor]:
     """
     Get a list containing the default postprocessor objects.
 
     Currently contains just :py:data:`datatypelibrary`.
     """
     # For compatibility with libxml2
     return [datatypelibrary]
```

### Comparing `rnginline-0.0.2/rnginline/regexbuilder.py` & `rnginline-1.0.0rc1/rnginline/regexbuilder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,307 +1,338 @@
-from __future__ import unicode_literals
+from __future__ import annotations
 
 import re
+from abc import abstractmethod, abstractproperty
+from typing import Sequence as TypingSequence
 
-import six
 
+class Regex:
+    @abstractmethod
+    def render(self) -> str:
+        ...
 
-@six.python_2_unicode_compatible
-class Regex(object):
-    def compile(self):
+    def compile(self) -> re.Pattern[str]:
         return re.compile(self.render())
 
-    def is_singular(self):
+    def is_singular(self) -> bool:
         return False
 
-    def is_expansive(self):
+    def is_expansive(self) -> bool:
         """
         If this expression B was placed between expressions A and C,
         is_expansive() returns True if the meaning of A or C could be changed.
         """
         return False
 
-    def render_singular(self):
+    def render_singular(self) -> str:
         """
         Render this regex for placement in a context which requires a single
         expression rather than multiple expressions. e.g. in x? <x> must be
         a single expression as ? applies to a single expression.
         """
         rendered = self.render()
         if self.is_singular():
             return rendered
         # Wrap the expressions in an anonymous group to make 1 expression
         return "(?:{0})".format(rendered)
 
-    def render_non_expansive(self):
+    def render_non_expansive(self) -> str:
         """
         Render this expression, allowing it not to be singular as long as it's
         not an expansive expression.
         """
         if self.is_expansive():
             return self.render_singular()
         return self.render()
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.render()
 
-    def __repr__(self):
-        return "<{0} -> ur\"{1}\">".format(
-            type(self).__name__,
-            six.text_type(self).encode("raw_unicode_escape"))
+    def __repr__(self) -> str:
+        return f"<{type(self).__name__} -> {str(self)!r}>"
 
 
 class BaseSequence(Regex):
-    def __init__(self, *expressions):
+    expressions: TypingSequence[Regex]
+
+    def __init__(self, *expressions: Regex) -> None:
         assert isinstance(expressions, tuple)
         assert all(isinstance(e, Regex) for e in expressions), expressions
         self.expressions = expressions
 
-    def is_singular(self):
+    def is_singular(self) -> bool:
         return len(self.expressions) == 1 and self.expressions[0].is_singular()
 
-    def get_operator(self):
+    def get_operator(self) -> str:
         return ""
 
-    def render_expression(self, e):
+    def render_expression(self, e: Regex) -> str:
         # In a sequence of expressions, each expression doesn't need to be
         # singular to maintain its semantics, but the expression can't affect
         # the semantics of its neighbors.
         return e.render_non_expansive()
 
-    def render(self):
+    def render(self) -> str:
         return self.get_operator().join(
-            self.render_expression(e) for e in self.expressions)
+            self.render_expression(e) for e in self.expressions
+        )
 
 
 class Sequence(BaseSequence):
     pass
 
 
 class Literal(Regex):
+    text: str
     _reserved_chars = set("\\.^$*+?{}[]|()")
 
-    def __init__(self, text):
+    def __init__(self, text: str) -> None:
         self.text = text
 
-    def is_singular(self):
+    def is_singular(self) -> bool:
         return len(self.text) == 1
 
-    def needs_escape(self, char):
+    def needs_escape(self, char: str) -> bool:
         return char in self._reserved_chars
 
-    def render(self):
+    def render(self) -> str:
         return "".join(
-            re.escape(char) if self.needs_escape(char) else char
-            for char in self.text)
+            re.escape(char) if self.needs_escape(char) else char for char in self.text
+        )
 
     @classmethod
-    def from_codepoint(cls, code_point):
+    def from_codepoint(cls, code_point: int) -> Literal:
         """
         Create a Literal matching the specified unicode code point. In
         interpreters using UTF-16 as their string representation (< 3.3)
         this will create (and match) surrogate pairs for code points above the
         BMP.
         """
-        return cls("\\U{0:08X}".format(code_point)
-                   .encode("ascii").decode("unicode_escape"))
+        return cls(
+            "\\U{0:08X}".format(code_point).encode("ascii").decode("unicode_escape")
+        )
 
 
 class Choice(BaseSequence):
-    def get_operator(self):
+    def get_operator(self) -> str:
         return "|"
 
-    def is_expansive(self):
+    def is_expansive(self) -> bool:
         # The choice operator is greedy, it includes as much as possible either
         # side, so if one is present in the expression, it's "expansive" (will
         # change the meaning of expressions next to it).
         return not self.is_singular()
 
 
 class Capture(Sequence):
-    def __init__(self, *expressions, **kwargs):
+    name: str | None
+
+    def __init__(self, *expressions: Regex, name: str | None = None) -> None:
         """
         Create a capturing regex group, optionally with a name.
         Args:
             name: If provided, create a named group with this name.
         """
         super(Capture, self).__init__(*expressions)
 
-        name = kwargs.pop("name", None)
         if name is not None and not is_name(name):
             raise ValueError("Invalid capture group name: {0}".format(name))
         self.name = name
 
-        if kwargs:
-            raise ValueError("Got unexpected kwargs: {0}".format(kwargs))
-
-    def render(self):
+    def render(self) -> str:
         expressions = super(Capture, self).render()
 
         if self.name is not None:
             return "(?P<{0}>{1})".format(self.name, expressions)
         return "({0})".format(expressions)
 
-    def is_singular(self):
+    def is_singular(self) -> bool:
         # A capture group always renders as a group, so it's always singular
         return True
 
 
 class Set(Regex):
-    def __init__(self, *items):
+    ranges: TypingSequence[SetRange]
+
+    def __init__(
+        self, *items: Set | SetRange | int | str | tuple[int | str, int | str]
+    ) -> None:
         if len(items) == 0:
             raise ValueError("empty Set()")
-        self.ranges = [SetRange.create(i)
-                       for i in items if not isinstance(i, Set)]
+        self.ranges = [SetRange.create(i) for i in items if not isinstance(i, Set)]
         # Merge sub set items
-        self.ranges += [range
-                        for set in items if isinstance(set, Set)
-                        for range in set.ranges]
-
-    def render(self):
-        contents = "".join(i.render(pos == 0)
-                           for pos, i in enumerate(self.ranges))
+        self.ranges += [
+            range for set in items if isinstance(set, Set) for range in set.ranges
+        ]
+
+    def render(self) -> str:
+        contents = "".join(i.render(pos == 0) for pos, i in enumerate(self.ranges))
         return "[{0}]".format(contents)
 
-    def is_singular(self):
+    def is_singular(self) -> bool:
         # Sets are always singular (1 expression)
         return True
 
 
 class SetRange(object):
-    def __init__(self, start, end):
+    start: int
+    end: int
+
+    def __init__(self, start: int, end: int) -> None:
         if end < start:
-            raise ValueError("end < start. start: {0}, end: {1}"
-                             .format(start, end))
+            raise ValueError("end < start. start: {0}, end: {1}".format(start, end))
         self.start = start
         self.end = end
 
-    def is_single(self):
+    def is_single(self) -> bool:
         return self.start == self.end
 
     @classmethod
-    def create(cls, item):
+    def create(
+        cls, item: SetRange | int | str | tuple[int | str, int | str]
+    ) -> SetRange:
         if isinstance(item, SetRange):
             return item
-        if isinstance(item, (int, six.text_type)):
+        if isinstance(item, (int, str)):
             codepoint = cls.get_codepoint(item)
             return SetRange(codepoint, codepoint)
         if len(item) == 2:
             start, end = item
             return SetRange(cls.get_codepoint(start), cls.get_codepoint(end))
-        raise ValueError("Don't know how to create a SetItem from: {0!r}"
-                         .format(item))
+        raise ValueError("Don't know how to create a SetItem from: {0!r}".format(item))
 
     @staticmethod
-    def get_codepoint(item):
+    def get_codepoint(item: int | str) -> int:
         if isinstance(item, int):
             return item
         return ord(item)
 
-    def needs_escape(self, char, is_first):
+    def needs_escape(self, char: str, is_first: bool) -> bool:
         # The ^ must be escaped if it's the first char in the set
         return (is_first and char == "^") or char in "\\]-"
 
-    def render_char(self, code_point, is_first):
-        char = six.unichr(code_point)
+    def render_char(self, code_point: int, is_first: bool) -> str:
+        char = chr(code_point)
         if self.needs_escape(char, is_first):
             return re.escape(char)
         return char
 
-    def render(self, is_first):
+    def render(self, is_first: bool) -> str:
         """
         Args:
             is_first: True if this is the first range in the set
         """
         if self.is_single():
             return self.render_char(self.start, is_first)
         else:
-            return "{0}-{1}".format(self.render_char(self.start, is_first),
-                                    self.render_char(self.end, False))
+            return "{0}-{1}".format(
+                self.render_char(self.start, is_first),
+                self.render_char(self.end, False),
+            )
 
-    def intersects(self, range):
+    def intersects(self, range: SetRange) -> bool:
         start, end = range.start, range.end
         ends_before = self.end < start
         starts_after = self.start > end
         return (not ends_before) and (not starts_after)
 
 
 class UnaryOperator(Regex):
-    def __init__(self, expression):
+    expression: Regex
+
+    def __init__(self, expression: Regex) -> None:
         assert isinstance(expression, Regex), expression
         self.expression = expression
 
+    @abstractproperty
+    def operator(self) -> str:
+        ...
+
     # Note that instances are not singular by default
 
-    def render(self):
+    def render(self) -> str:
         # The subexpression must be singular
-        return "{0}{1}".format(
-            self.expression.render_singular(), self.operator)
+        return "{0}{1}".format(self.expression.render_singular(), self.operator)
 
 
 class Repeat(UnaryOperator):
-    def __init__(self, expression, min=None, max=None, count=None):
+    min: int | None
+    max: int | None
+
+    def __init__(
+        self,
+        expression: Regex,
+        min: int | None = None,
+        max: int | None = None,
+        count: int | None = None,
+    ) -> None:
         super(Repeat, self).__init__(expression)
 
         if count is not None:
             assert min is None and max is None
             min = count
             max = count
 
         assert min is None or min >= 0
         assert max is None or max >= 0
-        assert ((min is None and max is None) or
-                (min is None or max is None) or
-                min <= max), (min, max)
+        assert (
+            (min is None and max is None) or (min is None or max is None) or min <= max
+        ), (min, max)
 
         self.min = min
         self.max = max
 
     @property
-    def operator(self):
+    def operator(self) -> str:
         if self.min is None and self.max is None:
             return "*"
         elif self.min == 1 and self.max is None:
             return "+"
         elif self.min == 0 and self.max == 1:
             return "?"
         elif self.min == self.max:
+            assert self.min is not None
             return "{{{0:d}}}".format(self.min)
         elif self.min is None:
+            assert self.max is not None
             return "{{,{0:d}}}".format(self.max)
         elif self.max is None:
             return "{{{0:d},}}".format(self.min)
         else:
             return "{{{0:d},{1:d}}}".format(self.min, self.max)
 
 
 class ZeroOrMore(Repeat):
-    def __init__(self, expresion):
-        super(ZeroOrMore, self).__init__(expresion)
+    def __init__(self, expression: Regex) -> None:
+        super(ZeroOrMore, self).__init__(expression)
 
 
 class OneOrMore(Repeat):
-    def __init__(self, expresion):
-        super(OneOrMore, self).__init__(expresion, min=1)
+    def __init__(self, expression: Regex) -> None:
+        super(OneOrMore, self).__init__(expression, min=1)
 
 
 class Optional(Repeat):
-    def __init__(self, expresion):
-        super(Optional, self).__init__(expresion, min=0, max=1)
+    def __init__(self, expression: Regex) -> None:
+        super(Optional, self).__init__(expression, min=0, max=1)
 
 
 class StandAlone(Regex):
     """
-    Base class for stand alone expressions like ^, $, \w, etc.
+    Base class for stand alone expressions like ^, $, \\w, etc.
     """
 
-    def render(self):
+    @abstractproperty
+    def representation(self) -> str:
+        ...
+
+    def render(self) -> str:
         return self.representation
 
-    def is_singular(self):
+    def is_singular(self) -> bool:
         # These are always singular as they're stand alone expressions
         return True
 
 
 class Start(StandAlone):
     representation = "^"
 
@@ -313,10 +344,10 @@
 class Whitespace(StandAlone):
     representation = r"\s"
 
 
 NAME = re.compile(r"^[a-zA-Z_]\w*$")
 
 
-def is_name(string):
+def is_name(string: str) -> bool:
     """Returns: True if string is a Python name/identifier."""
     return bool(NAME.match(string))
```

### Comparing `rnginline-0.0.2/rnginline/relaxng.rng` & `rnginline-1.0.0rc1/rnginline/relaxng.rng`

 * *Files identical despite different names*

### Comparing `rnginline-0.0.2/rnginline/test/data/datatype-library-propagation/b.rng` & `rnginline-1.0.0rc1/rnginline/test/data/datatype-library-propagation/b.rng`

 * *Files identical despite different names*

### Comparing `rnginline-0.0.2/rnginline/test/data/multiple-ref-1-fetch/schema.rng` & `rnginline-1.0.0rc1/rnginline/test/data/multiple-ref-1-fetch/schema.rng`

 * *Files identical despite different names*

### Comparing `rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/README.rst` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/README.rst`

 * *Files identical despite different names*

### Comparing `rnginline-0.0.2/rnginline/test/data/testcases/external-ref-3-namespaces/schema.rng` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/schema.rng`

 * *Files identical despite different names*

### Comparing `rnginline-0.0.2/rnginline/test/data/testcases/foreign-attributes/schema.rng` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/foreign-attributes/schema.rng`

 * *Files identical despite different names*

### Comparing `rnginline-0.0.2/rnginline/test/data/testcases/overrides/included.rng` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/overrides/included.rng`

 * *Files identical despite different names*

### Comparing `rnginline-0.0.2/rnginline/test/data/testcases/overrides/positive.xml` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/overrides/positive.xml`

 * *Files identical despite different names*

### Comparing `rnginline-0.0.2/rnginline/test/data/testcases/overrides/schema.rng` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/overrides/schema.rng`

 * *Files identical despite different names*

### Comparing `rnginline-0.0.2/rnginline/test/mini_validator.py` & `rnginline-1.0.0rc1/rnginline/test/mini_validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 A very simple program to check if an XML file matches a RELAX NG schema.
 
 usage: mini_validator <rngfile> <xmlfile>
 """
-from __future__ import unicode_literals, print_function
+from __future__ import annotations
 
 import sys
 
 import docopt
 from lxml import etree
 
 
-def main(argv=None):
+def main(argv: list[str] | str | None = None) -> None:
     try:
         validate(argv)
     except Exception as e:
         print("fatal: {0}".format(e))
         sys.exit(1)
 
 
-def validate(argv):
+def validate(argv: list[str] | str | None) -> None:
     options = docopt.docopt(__doc__, argv=argv)
 
     xml = etree.parse(options["<xmlfile>"])
     validator = etree.RelaxNG(etree.parse(options["<rngfile>"]))
 
     if not validator(xml):
         sys.exit(2)
```

### Comparing `rnginline-0.0.2/rnginline/test/test_cmdline.py` & `rnginline-1.0.0rc1/rnginline/test/test_cmdline.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,238 +1,262 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals
+from __future__ import annotations
 
-import re
+import io
 import os
-from os import path
+import re
 import tempfile
 from contextlib import contextmanager
+from os import path
+from typing import Generator
+from unittest.mock import Mock
 
-from lxml import etree
-import pkg_resources
+import importlib_resources
 import pytest
-import six
+from lxml import etree
 
-from rnginline import _get_cwd
+from rnginline import _get_cwd, urlhandlers
 from rnginline.cmdline import main as rng_main
-from rnginline.test.mini_validator import main as minival_main
 from rnginline.exceptions import RelaxngInlineError
-from rnginline import urlhandlers
-
+from rnginline.test.mini_validator import main as minival_main
 from rnginline.test.test_rnginline import (
-    test_testcases_testcases, ttt_ids)
+    SchemaTestCase,
+    test_testcases_testcases,
+    ttt_ids,
+)
 
 
-def _code(sysexit):
+def _code(sysexit: SystemExit | int) -> str | int | None:
     # For some py.test's ExceptionInfo objects in Py26 have an int for the
     # .value attr instead of the actual exception.
     if isinstance(sysexit, int):
         return sysexit
     return sysexit.code
 
 
 @contextmanager
-def change_dir(path):
+def change_dir(path: str) -> Generator[str, None, None]:
     old_cwd = _get_cwd()
     os.chdir(path)
     yield path
     os.chdir(old_cwd)
 
 
-def test_change_dir():
+def test_change_dir() -> None:
     old_cwd = _get_cwd()
     new_dir = tempfile.mkdtemp()
 
     with change_dir(new_dir) as dir:
         assert dir == new_dir
         assert path.realpath(_get_cwd()) == path.realpath(new_dir)
 
     assert path.realpath(_get_cwd()) == path.realpath(old_cwd)
     os.rmdir(new_dir)
 
 
 @pytest.fixture(scope="module")
-def testcase_dir():
+def testcase_dir() -> str:
     """
     Extract testcase data to the filesystem for access by command line tools.
     """
-    return pkg_resources.resource_filename("rnginline.test",
-                                           "data/testcases")
+    return str(importlib_resources.files("rnginline.test") / "data/testcases")
 
 
-def _external_path(testcase_dir, pkg_path):
+def _external_path(testcase_dir: str, pkg_path: str) -> str:
     assert pkg_path.startswith("data/testcases/")
-    tc_path = pkg_path[len("data/testcases/"):]
+    tc_path = pkg_path[len("data/testcases/") :]
     return path.join(testcase_dir, tc_path)
 
 
-def _cmdline_args(argv):
-    if six.PY2:
-        return [a.encode("utf-8") for a in argv]
-    return argv
-
-
-@pytest.mark.parametrize("schema_file,test_file,should_match",
-                         test_testcases_testcases, ids=ttt_ids)
-def test_cmdline(testcase_dir, schema_file, test_file, should_match):
-    schema_external = _external_path(testcase_dir, schema_file)
-    xml_external = _external_path(testcase_dir, test_file)
-
+@pytest.mark.parametrize("example", test_testcases_testcases, ids=ttt_ids)
+def test_cmdline(example: SchemaTestCase) -> None:
     # Get a temp file to write the inlined schema to
     fd, inlined_schema = tempfile.mkstemp()
     os.fdopen(fd).close()
 
-    # Generate the inlined schema with the command line tool
-    try:
-        rng_main(argv=_cmdline_args([schema_external, inlined_schema]))
-    except SystemExit as e:
-        if e.code not in [None, 0]:
-            pytest.fail("rnginline.cmdline exited with status: {0}"
-                        .format(e.code))
-
-    try:
-        minival_main(argv=_cmdline_args([inlined_schema, xml_external]))
-        status = 0
-    except SystemExit as e:
-        status = 0 if e.code is None else e.code
+    with importlib_resources.as_file(example.schema_file) as schema_file:
+        # Generate the inlined schema with the command line tool
+        try:
+            rng_main(argv=[str(schema_file), inlined_schema])
+        except SystemExit as e:
+            if e.code not in [None, 0]:
+                pytest.fail(f"rnginline.cmdline exited with status: {e.code}")
+
+    with importlib_resources.as_file(example.xml_file) as xml_file:
+        try:
+            minival_main(argv=[inlined_schema, str(xml_file)])
+            status: str | int | None = 0
+        except SystemExit as e:
+            status = 0 if e.code is None else e.code
 
     # Cleanup the schema we generated
     os.unlink(inlined_schema)
 
     if status not in [0, 2]:
-        pytest.fail("mini_validator exited abnormally: {0}".format(status))
+        pytest.fail(f"mini_validator exited abnormally: {status}")
 
-    if should_match:
+    if example.should_match:
         if status != 0:
-            pytest.fail("{0} should match {1} but didn't"
-                        .format(test_file, schema_file))
+            pytest.fail(
+                f"{example.xml_file.name} should match "
+                f"{example.schema_file.name} but didn't"
+            )
     else:
         if status != 2:
-            pytest.fail("{0} shouldn't match {1} but did"
-                        .format(test_file, schema_file))
+            pytest.fail(
+                f"{example.xml_file.name} shouldn't match "
+                f"{example.schema_file.name} but did"
+            )
 
 
-def test_cmdline_from_non_ascii_dir(testcase_dir):
+def test_cmdline_from_non_ascii_dir(testcase_dir: str) -> None:
     schema = _external_path(testcase_dir, "data/testcases/xml-base/schema.rng")
-    xml = _external_path(testcase_dir,
-                         "data/testcases/xml-base/positive-1.xml")
+    xml = _external_path(testcase_dir, "data/testcases/xml-base/positive-1.xml")
 
     with change_dir(tempfile.mkdtemp(suffix="-åß∂ƒ\U00010438-")) as new_dir:
         inlined_schema = "schema-inlined.rng"
 
         # Generate the inlined schema with the command line tool
-        rng_main(argv=_cmdline_args([path.relpath(schema), inlined_schema]))
+        rng_main(argv=[path.relpath(schema), inlined_schema])
 
         # Validate the generated schema matches the expected xml
-        minival_main(argv=_cmdline_args([inlined_schema, path.relpath(xml)]))
+        minival_main(argv=[inlined_schema, path.relpath(xml)])
 
         os.unlink(inlined_schema)
     os.rmdir(new_dir)
 
 
-@pytest.mark.parametrize("base_arg",
-                         ["--default-base-uri", "--base-uri", "-b"])
-@pytest.mark.parametrize("stdout_arg", [[], ["-"]],
-                         ids=["implicit stdout", "minus char"])
-def test_cmdline_stdin_stdout(testcase_dir, stdout_arg, base_arg, monkeypatch):
+@pytest.mark.parametrize("base_arg", ["--default-base-uri", "--base-uri", "-b"])
+@pytest.mark.parametrize(
+    "stdout_arg", [[], ["-"]], ids=["implicit stdout", "minus char"]
+)
+def test_cmdline_stdin_stdout(
+    testcase_dir: str,
+    stdout_arg: list[str],
+    base_arg: str,
+    monkeypatch: pytest.MonkeyPatch,
+) -> None:
     # Note that using stdin is rather awkward as it means we don't know what
     # the base URI of the input is. So that has to be set explicitly using
     # --default-base-uri.
 
     schema_path = "data/testcases/xml-base/schema.rng"
 
     schema_bytes = urlhandlers.pydata.dereference(
-        urlhandlers.pydata.makeurl("rnginline.test", schema_path))
+        urlhandlers.pydata.makeurl("rnginline.test", schema_path)
+    )
     xml_bytes = urlhandlers.pydata.dereference(
-        urlhandlers.pydata.makeurl("rnginline.test",
-                                   "data/testcases/xml-base/positive-1.xml"))
+        urlhandlers.pydata.makeurl(
+            "rnginline.test", "data/testcases/xml-base/positive-1.xml"
+        )
+    )
 
     # The default base URI must be a URI rather than URI-reference
     is_abs = base_arg == "--default-base-uri"
-    base = urlhandlers.file.makeurl(_external_path(testcase_dir, schema_path),
-                                    abs=is_abs)
+    base = urlhandlers.file.makeurl(
+        _external_path(testcase_dir, schema_path), abs=is_abs
+    )
 
-    new_stdin = six.BytesIO(schema_bytes)
-    new_stdout = six.BytesIO()
-    new_stdin.buffer = new_stdin  # fake sys.stdin.buffer for Py 3
-    new_stdout.buffer = new_stdout
+    new_stdin = io.BytesIO(schema_bytes)
+    new_stdout = io.BytesIO()
 
-    monkeypatch.setattr("sys.stdin", new_stdin)
-    monkeypatch.setattr("sys.stdout", new_stdout)
+    monkeypatch.setattr("sys.stdin", Mock())
+    monkeypatch.setattr("sys.stdin.buffer", new_stdin)
+    monkeypatch.setattr("sys.stdout", Mock())
+    monkeypatch.setattr("sys.stdout.buffer", new_stdout)
 
     # Generate the inlined schema with the command line tool
-    rng_main(argv=_cmdline_args(
-        [base_arg, base, "--stdin"] + stdout_arg))
+    rng_main(argv=[base_arg, base, "--stdin"] + stdout_arg)
 
     new_stdout.seek(0)
     schema = etree.RelaxNG(file=new_stdout)
     assert schema(etree.XML(xml_bytes))
 
 
-@pytest.mark.parametrize("base_uri_arg",
-                         ["--default-base-uri", "--base-uri", "-b"])
-def test_cmdline_rejects_invalid_base_uri(base_uri_arg, monkeypatch):
+@pytest.mark.parametrize("base_uri_arg", ["--default-base-uri", "--base-uri", "-b"])
+def test_cmdline_rejects_invalid_base_uri(
+    base_uri_arg: str, monkeypatch: pytest.MonkeyPatch
+) -> None:
     bad_uri = "/foo bar"  # contains a space
 
-    stderr = six.StringIO()
+    stderr = io.StringIO()
     monkeypatch.setattr("sys.stderr", stderr)
 
     with pytest.raises(SystemExit) as excinfo:
-        rng_main(argv=_cmdline_args([base_uri_arg, bad_uri, "/dev/null"]))
+        rng_main(argv=[base_uri_arg, bad_uri, "/dev/null"])
     stderr.seek(0)
 
     assert _code(excinfo.value) == 1
     assert "base-uri" in stderr.read()
 
 
-def test_cmdline_traceback_produces_traceback(monkeypatch):
-    stderr = six.StringIO()
+def test_cmdline_traceback_produces_traceback(monkeypatch: pytest.MonkeyPatch) -> None:
+    stderr = io.StringIO()
     monkeypatch.setattr("sys.stderr", stderr)
 
     # Patch stdin to blow up when read is called
     class MyTestingRngError(RelaxngInlineError):
         pass
 
     class Boomer(object):
-        def read(self):
+        def read(self) -> None:
             raise MyTestingRngError("boom!")
+
     stdin = Boomer()
-    stdin.buffer = stdin  # emulate sys.stdin.buffer for Py 3
-    monkeypatch.setattr("sys.stdin", stdin)
+    monkeypatch.setattr("sys.stdin", Mock())
+    monkeypatch.setattr("sys.stdin.buffer", stdin)
 
     with pytest.raises(SystemExit):
-        rng_main(argv=_cmdline_args(["--traceback", "--stdin"]))
+        rng_main(argv=["--traceback", "--stdin"])
     stderr.seek(0)
 
-    assert re.search("""MyTestingRngError\(.boom!.\)""", stderr.read())
+    assert re.search(r"MyTestingRngError\(.boom!.\)", stderr.read())
 
 
-@pytest.mark.parametrize("compat_arg,should_match_input", [
-    # If libxml2 compat is disabled then the output will match the input
-    (["--no-libxml2-compat"], True),
-    # If compat's on (the default) then the input will be modified to put
-    # datatypeLibrary on the data el.
-    ([], False)
-])
+@pytest.mark.parametrize(
+    "compat_arg,should_match_input",
+    [
+        # If libxml2 compat is disabled then the output will match the input
+        (["--no-libxml2-compat"], True),
+        # If compat's on (the default) then the input will be modified to put
+        # datatypeLibrary on the data el.
+        ([], False),
+    ],
+)
 def test_cmdline_no_libxml2_compat_disables_compat(
-        compat_arg, should_match_input, monkeypatch):
-    input = (
+    compat_arg: list[str], should_match_input: bool, monkeypatch: pytest.MonkeyPatch
+) -> None:
+    input_xml = (
         '<element name="start" xmlns="http://relaxng.org/ns/structure/1.0" '
         'datatypeLibrary="foo">'
         '<data type="bar"/>'
-        '</element>'
+        "</element>"
     )
-    input = etree.tostring(etree.XML(input), method="c14n")
+    input = etree.tostring(etree.XML(input_xml), method="c14n")
 
-    stdin = six.BytesIO(input)
-    stdout = six.BytesIO()
-    stdin.buffer = stdin
-    stdout.buffer = stdout
+    stdin = io.BytesIO(input)
+    stdout = io.BytesIO()
 
-    monkeypatch.setattr("sys.stdin", stdin)
-    monkeypatch.setattr("sys.stdout", stdout)
+    monkeypatch.setattr("sys.stdin", Mock())
+    monkeypatch.setattr("sys.stdin.buffer", stdin)
+    monkeypatch.setattr("sys.stdout", Mock())
+    monkeypatch.setattr("sys.stdout.buffer", stdout)
 
-    rng_main(argv=_cmdline_args(compat_arg + ["--stdin"]))
+    rng_main(argv=compat_arg + ["--stdin"])
     stdout.seek(0)
     output = etree.tostring(etree.XML(stdout.read()), method="c14n")
 
     assert (input == output) == should_match_input
+
+
+def test_cmdline_prints_usage_error_when_cli_arguments_are_wrong(
+    capsys: pytest.CaptureFixture[str],
+) -> None:
+    with pytest.raises(SystemExit) as excinfo:
+        rng_main(argv=["--frob"])
+
+    assert excinfo.value.code == 1
+    _, err = capsys.readouterr()
+    assert re.search(
+        "rnginline couldn't understand the command line options it received", err
+    )
+    assert re.search("^usage: rnginline", err, re.MULTILINE)
+    assert re.search("rnginline --help", err)
```

### Comparing `rnginline-0.0.2/rnginline/test/test_propagate_datatypelibrary.py` & `rnginline-1.0.0rc1/rnginline/test/test_propagate_datatypelibrary.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-from __future__ import unicode_literals
+from __future__ import annotations
 
 import copy
 
-from lxml import etree
 import pytest
+from lxml import etree
 
+from rnginline import urlhandlers
 from rnginline.constants import NSMAP
 from rnginline.postprocess import datatypelibrary
-from rnginline import urlhandlers
 
 
-@pytest.mark.parametrize("xml,expected", [
-    ('<a datatypeLibrary="a"><b><c id="start"/></b></a>', "a"),
-    ('<a datatypeLibrary="a"><b><c datatypeLibrary="c" id="start"/></b></a>',
-     "c"),
-    ('<a datatypeLibrary="a"><b datatypeLibrary="b"><c id="start"/></b></a>',
-     "b"),
-    ('<a datatypeLibrary="a"><b><c datatypeLibrary="c" id="start"/></b></a>',
-     "c"),
-    ('<a datatypeLibrary="a"><b><c datatypeLibrary="" id="start"/></b></a>',
-     ""),
-    ('<a><b><c id="start"/></b></a>', ""),
-])
-def test_lookup_datatypelibrary(xml, expected):
+@pytest.mark.parametrize(
+    "xml,expected",
+    [
+        ('<a datatypeLibrary="a"><b><c id="start"/></b></a>', "a"),
+        ('<a datatypeLibrary="a"><b><c datatypeLibrary="c" id="start"/></b></a>', "c"),
+        ('<a datatypeLibrary="a"><b datatypeLibrary="b"><c id="start"/></b></a>', "b"),
+        ('<a datatypeLibrary="a"><b><c datatypeLibrary="c" id="start"/></b></a>', "c"),
+        ('<a datatypeLibrary="a"><b><c datatypeLibrary="" id="start"/></b></a>', ""),
+        ('<a><b><c id="start"/></b></a>', ""),
+    ],
+)
+def test_lookup_datatypelibrary(xml: str, expected: str) -> None:
     root = etree.XML(xml)
-    start, = root.xpath("//*[@id='start']")
+    (start,) = root.xpath("//*[@id='start']")
 
     assert datatypelibrary.lookup_datatypelibrary(start) == expected
 
 
-@pytest.mark.parametrize("path", [
-    "data/datatype-library-propagation/a.rng",
-    "data/datatype-library-propagation/b.rng"
-])
-def test_propagate_datatype_library(path):
+@pytest.mark.parametrize(
+    "path",
+    [
+        "data/datatype-library-propagation/a.rng",
+        "data/datatype-library-propagation/b.rng",
+    ],
+)
+def test_propagate_datatype_library(path: str) -> None:
     url = urlhandlers.pydata.makeurl("rnginline.test", path)
     el = etree.XML(urlhandlers.pydata.dereference(url))
 
     propagated = datatypelibrary(copy.deepcopy(el))
 
     # Ensure we've not lost any elements
     assert len(list(el.iter())) == len(list(propagated.iter()))
 
     # Only data/value els have datatype library attrs
-    assert (propagated.xpath("//rng:data|//rng:value", namespaces=NSMAP) ==
-            propagated.xpath("//*[@datatypeLibrary]"))
+    assert propagated.xpath(
+        "//rng:data|//rng:value", namespaces=NSMAP
+    ) == propagated.xpath("//*[@datatypeLibrary]")
 
     # Ensure the resolved values match those we expect
     for el in propagated.xpath("//rng:data|//rng:value", namespaces=NSMAP):
         assert el.attrib["datatypeLibrary"] == el.attrib["{expected}expected"]
```

### Comparing `rnginline-0.0.2/rnginline/test/test_regexbuilder.py` & `rnginline-1.0.0rc1/rnginline/test/test_regexbuilder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,46 @@
-from __future__ import unicode_literals
+from __future__ import annotations
 
-from copy import copy
+import re
+from dataclasses import dataclass, replace
+from typing import Mapping
+from typing import Sequence as TypingSequence
 
 import pytest
-import six
 
-from rnginline.regexbuilder import (Literal, Set, OneOrMore, ZeroOrMore,
-                                    Choice, Capture, Sequence, Repeat,
-                                    Optional, Start, End, SetRange, Whitespace)
-
-
-class _TestString(object):
-    def __init__(self, string, groups=None, groupdict=None, length=None,
-                 should_match=True):
-        self.string = string
-        self.groups = groups
-        self.groupdict = groupdict
-        self.length = length
-        self.should_match = should_match
-
-    def __invert__(self):
-        inverted = copy(self)
-        inverted.should_match = not self.should_match
-        return inverted
+from rnginline.regexbuilder import (
+    Capture,
+    Choice,
+    End,
+    Literal,
+    OneOrMore,
+    Optional,
+    Regex,
+    Repeat,
+    Sequence,
+    Set,
+    SetRange,
+    Start,
+    Whitespace,
+    ZeroOrMore,
+)
+
+
+@dataclass(frozen=True)
+class _TestString:
+    string: str
+    groups: TypingSequence[str | None] | None = None
+    groupdict: Mapping[str, str] | None = None
+    length: int | None = None
+    should_match: bool = True
 
-    def run(self, regex):
+    def __invert__(self) -> _TestString:
+        return replace(self, should_match=not self.should_match)
+
+    def run(self, regex: re.Pattern[str]) -> None:
         match = regex.match(self.string)
 
         # For debugging
         msg = (match, regex, self.string)
 
         length = self.length or len(self.string)
 
@@ -38,158 +50,176 @@
             if self.groups is not None:
                 assert match.groups() == self.groups, msg
             if self.groupdict is not None:
                 assert match.groupdict() == self.groupdict, msg
         else:
             assert not match or match.end() != length, msg
 
-    def __repr__(self):
-        return ("{0}({1!r}, groups={2!r}, length={3!r}, should_match={4!r})"
-                .format(type(self), self.string, self.groups, self.length,
-                        self.should_match))
-
 
-class _TestCase(object):
-    def __init__(self, node, *test_strings, **kwargs):
+@dataclass(init=False)
+class _TestCase:
+    node: Regex
+    test_strings: TypingSequence[_TestString]
+
+    def __init__(
+        self, node: Regex, *test_strings: str | _TestString, wrap: bool = True
+    ) -> None:
         if len(test_strings) == 0:
             raise ValueError("no test strings provided")
 
-        wrap = kwargs.get("wrap", True)
-
         if wrap is True:
             # We generally want to match with ^<pattern>$, otherwise patterns
             # like this won't match the entire input, even though they could:
             # re.match("(/[a-z]+)*|([a-z]+)", "foo")  # 0 length match
             self.node = Sequence(Start(), node, End())
         else:
             self.node = node
         self.test_strings = [
-            _TestString(ts) if isinstance(ts, six.text_type) else ts
-            for ts in test_strings
+            _TestString(ts) if isinstance(ts, str) else ts for ts in test_strings
         ]
 
-    def run(self):
+    def run(self) -> None:
         regex = self.node.compile()
 
         for test_string in self.test_strings:
             test_string.run(regex)
 
-    def __repr__(self):
-        test_strings = ""
-        if self.test_strings:
-            test_strings = ", " + ", ".join(
-                repr(ts) for ts in self.test_strings)
-        return "{0}({1!r}{2})".format(
-            type(self).__name__, self.node, test_strings)
-
 
 tc = _TestCase
 ts = _TestString
 
 
-@pytest.mark.parametrize("test_case", [
-    tc(Literal("foo"), ts("foo"), ~ts("afoo")),
-    tc(Literal("".join(six.unichr(x) for x in range(256))),
-       "".join(six.unichr(x) for x in range(256))),
-    tc(Literal.from_codepoint(0x10155), ts("\U00010155")),
-    tc(Literal.from_codepoint(ord("x")), ts("x")),
-
-    tc(OneOrMore(Literal("a")), ~ts(""), "a", "aa", "aaa", "aaaaaaaaaaaaaaa"),
-    tc(ZeroOrMore(Literal("a")), "", "a", "aa", "aaa", "aaaaaaaaaaaaaa"),
-
-    tc(Set("a", "d", "f"), "a", "d", "f", ~ts("b"), ~ts("e"), ~ts("g")),
-    tc(Set("^"), "^", ~ts("a"), ~ts("")),
-    tc(Set("]"), "]", ~ts("a"), ~ts("")),
-    tc(Set("\\"), "\\", ~ts("a"), ~ts("")),
-    tc(Set(SetRange.create(SetRange.create(ord("x")))), "x"),
-
-    tc(OneOrMore(Set(("a", "f"))), "abcdef", "fedcba", "aa", "fdf"),
-    # Nested Sets
-    tc(OneOrMore(Set(Set(("a", "f")))), "abcdef", "fedcba", "aa", "fdf"),
-
-    tc(Choice(Literal("foo"), Literal("bar")), "foo", "bar", ~ts("foobar")),
-
-    tc(Capture(Literal("foo")), ts("foo", groups=("foo",))),
-    tc(Optional(Capture(Literal("foo"))),
-       ts("foo", groups=("foo",)), ts("", groups=(None,))),
-    tc(Sequence(Capture(Literal("foo")), Literal(":"),
-                Capture(Literal("bar"))),
-       ts("foo:bar", groups=("foo", "bar"))),
-    tc(Choice(Capture(Literal("foo")), Capture(Literal("bar"))),
-       ts("foo", groups=("foo", None)), ts("bar", groups=(None, "bar"))),
-
-    tc(Repeat(Literal("abc"), count=3), "abcabcabc", ~ts("abcabc"),
-       ~ts("abcabcabcabc")),
-    tc(Repeat(Literal("ab"), min=2, max=4), "abab", "ababab", "abababab",
-       ~ts("ab"), ~ts("ababababab")),
-
-    tc(Repeat(Literal("ab"), min=2, max=None), "abab", "ababab",
-       "ababababab" * 100, ~ts("ab")),
-
-    tc(Repeat(Literal("ab"), min=None, max=10), ~ts("ab" * 11),
-       *["ab" * n for n in range(1, 11)]),
-
-    tc(Sequence(Literal("foo"), Optional(Literal("bar")), Literal("baz")),
-       "foobaz", "foobarbaz"),
-
-    tc(Optional(Repeat(Literal("x"), min=2, max=4)), "", "xx", "xxx", "xxxx",
-       ~ts("x")),
-
-    tc(Sequence(
-        Capture(OneOrMore(Set("a")), name="foo"),
-        Capture(OneOrMore(Set("b")), name="bar")),
-       ts("aaaabb", groupdict=dict(foo="aaaa", bar="bb"))),
-
-    tc(ZeroOrMore(Whitespace()),
-       "", "  ", "\t\t  \t")
-
-])
-def test_regex_builder_node(test_case):
+@pytest.mark.parametrize(
+    "test_case",
+    [
+        tc(Literal("foo"), ts("foo"), ~ts("afoo")),
+        tc(
+            Literal("".join(chr(x) for x in range(256))),
+            "".join(chr(x) for x in range(256)),
+        ),
+        tc(Literal.from_codepoint(0x10155), ts("\U00010155")),
+        tc(Literal.from_codepoint(ord("x")), ts("x")),
+        tc(OneOrMore(Literal("a")), ~ts(""), "a", "aa", "aaa", "aaaaaaaaaaaaaaa"),
+        tc(ZeroOrMore(Literal("a")), "", "a", "aa", "aaa", "aaaaaaaaaaaaaa"),
+        tc(Set("a", "d", "f"), "a", "d", "f", ~ts("b"), ~ts("e"), ~ts("g")),
+        tc(Set("^"), "^", ~ts("a"), ~ts("")),
+        tc(Set("]"), "]", ~ts("a"), ~ts("")),
+        tc(Set("\\"), "\\", ~ts("a"), ~ts("")),
+        tc(Set(SetRange.create(SetRange.create(ord("x")))), "x"),
+        tc(OneOrMore(Set(("a", "f"))), "abcdef", "fedcba", "aa", "fdf"),
+        # Nested Sets
+        tc(OneOrMore(Set(Set(("a", "f")))), "abcdef", "fedcba", "aa", "fdf"),
+        tc(Choice(Literal("foo"), Literal("bar")), "foo", "bar", ~ts("foobar")),
+        tc(Capture(Literal("foo")), ts("foo", groups=("foo",))),
+        tc(
+            Optional(Capture(Literal("foo"))),
+            ts("foo", groups=("foo",)),
+            ts("", groups=(None,)),
+        ),
+        tc(
+            Sequence(Capture(Literal("foo")), Literal(":"), Capture(Literal("bar"))),
+            ts("foo:bar", groups=("foo", "bar")),
+        ),
+        tc(
+            Choice(Capture(Literal("foo")), Capture(Literal("bar"))),
+            ts("foo", groups=("foo", None)),
+            ts("bar", groups=(None, "bar")),
+        ),
+        tc(
+            Repeat(Literal("abc"), count=3),
+            "abcabcabc",
+            ~ts("abcabc"),
+            ~ts("abcabcabcabc"),
+        ),
+        tc(
+            Repeat(Literal("ab"), min=2, max=4),
+            "abab",
+            "ababab",
+            "abababab",
+            ~ts("ab"),
+            ~ts("ababababab"),
+        ),
+        tc(
+            Repeat(Literal("ab"), min=2, max=None),
+            "abab",
+            "ababab",
+            "ababababab" * 100,
+            ~ts("ab"),
+        ),
+        tc(
+            Repeat(Literal("ab"), min=None, max=10),
+            ~ts("ab" * 11),
+            *["ab" * n for n in range(1, 11)],
+        ),
+        tc(
+            Sequence(Literal("foo"), Optional(Literal("bar")), Literal("baz")),
+            "foobaz",
+            "foobarbaz",
+        ),
+        tc(
+            Optional(Repeat(Literal("x"), min=2, max=4)),
+            "",
+            "xx",
+            "xxx",
+            "xxxx",
+            ~ts("x"),
+        ),
+        tc(
+            Sequence(
+                Capture(OneOrMore(Set("a")), name="foo"),
+                Capture(OneOrMore(Set("b")), name="bar"),
+            ),
+            ts("aaaabb", groupdict=dict(foo="aaaa", bar="bb")),
+        ),
+        tc(ZeroOrMore(Whitespace()), "", "  ", "\t\t  \t"),
+    ],
+)
+def test_regex_builder_node(test_case: _TestCase) -> None:
     test_case.run()
 
 
-def test_capture_name_must_by_python_name():
+def test_capture_name_must_by_python_name() -> None:
     with pytest.raises(ValueError):
         Capture(Literal("lol"), name="foo-bar")  # hyphen not allowed in names
 
 
-def test_capture_rejects_unknown_kwargs():
-    with pytest.raises(ValueError):
-        Capture(Literal("lol"), foo="bar")  # unrecognised keyword arg
+def test_capture_rejects_unknown_kwargs() -> None:
+    with pytest.raises(TypeError, match="got an unexpected keyword argument"):
+        Capture(Literal("lol"), foo="bar")  # type: ignore[call-arg]
 
 
-def test_set_cannot_be_empty():
+def test_set_cannot_be_empty() -> None:
     with pytest.raises(ValueError):
         Set()
 
 
-def test_set_range_cannot_be_reversed():
+def test_set_range_cannot_be_reversed() -> None:
     with pytest.raises(ValueError):
         SetRange(20, 10)
 
 
-def test_set_range_create_rejects_unknown_args():
+def test_set_range_create_rejects_unknown_args() -> None:
     with pytest.raises(ValueError):
-        SetRange.create([1, 2, 3])
-
-
-@pytest.mark.parametrize("a,b,intersects", [
-    (SetRange(3, 3), SetRange(3, 3), True),
-    (SetRange(3, 3), SetRange(4, 4), False),
-
-    (SetRange(100, 110), SetRange(110, 120), True),
-    (SetRange(110, 120), SetRange(100, 110), True),
+        SetRange.create([1, 2, 3])  # type: ignore[arg-type]
 
-    (SetRange(50, 100), SetRange(40, 60), True),
-    (SetRange(40, 60), SetRange(50, 100), True),
 
-    (SetRange(70, 80), SetRange(50, 100), True),
-    (SetRange(50, 100), SetRange(70, 80), True)
-])
-def test_set_range_intersects(a, b, intersects):
+@pytest.mark.parametrize(
+    "a,b,intersects",
+    [
+        (SetRange(3, 3), SetRange(3, 3), True),
+        (SetRange(3, 3), SetRange(4, 4), False),
+        (SetRange(100, 110), SetRange(110, 120), True),
+        (SetRange(110, 120), SetRange(100, 110), True),
+        (SetRange(50, 100), SetRange(40, 60), True),
+        (SetRange(40, 60), SetRange(50, 100), True),
+        (SetRange(70, 80), SetRange(50, 100), True),
+        (SetRange(50, 100), SetRange(70, 80), True),
+    ],
+)
+def test_set_range_intersects(a: SetRange, b: SetRange, intersects: bool) -> None:
     assert a.intersects(b) == intersects
 
 
-def test_repr():
+def test_repr() -> None:
     expr = Choice(Literal("foo"), Repeat(Literal("bar"), min=3, max=8))
     assert "Choice" in repr(expr)
     assert "foo|(?:bar){3,8}" in repr(expr)
```

### Comparing `rnginline-0.0.2/rnginline/test/test_rnginline.py` & `rnginline-1.0.0rc1/rnginline/test/test_rnginline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,185 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals
+from __future__ import annotations
 
-import re
 import io
+import re
+from dataclasses import dataclass
+from pathlib import Path
+from typing import Sequence
+from unittest import mock
+from urllib.parse import urlsplit
 
-from lxml import etree
+import importlib_resources
 import pytest
-import pkg_resources as pr  # setuptools, but only used in tests
-import mock
+from importlib_resources.abc import Traversable
+from lxml import etree
 
 import rnginline
-from rnginline import DeferredXmlInsertion, uri
-
-from rnginline import urlhandlers
-
+from rnginline import DeferredXmlInsertion, InlineContextToken, uri, urlhandlers
 from rnginline.exceptions import (
-    InvalidGrammarError, SchemaIncludesSelfError, NoAvailableHandlerError,
-    ParseError)
-
+    InvalidGrammarError,
+    NoAvailableHandlerError,
+    ParseError,
+    SchemaIncludesSelfError,
+)
 
 TESTPKG = "rnginline.test"
 
 DATA_URI = urlhandlers.pydata.makeurl(TESTPKG, "data/")
 
 
-def _load_testcases():
-    root_dir = "data/testcases"
-    assert pr.resource_isdir(TESTPKG, root_dir)
-
-    testcases = []
-    for tc_dir in pr.resource_listdir(TESTPKG, root_dir):
-        files = pr.resource_listdir(TESTPKG, "/".join([root_dir, tc_dir]))
-
-        schema = "/".join((root_dir, tc_dir, "schema.rng"))
-        positive_cases = ["/".join([root_dir, tc_dir, f]) for f in files
-                          if re.match("^positive.*\.xml$", f)]
-        negative_cases = ["/".join([root_dir, tc_dir, f]) for f in files
-                          if re.match("^negative.*\.xml$", f)]
-
-        assert positive_cases
-        assert not [f for _files in [[schema], positive_cases, negative_cases]
-                    for f in _files if not pr.resource_exists(__name__, f)]
-
-        for file in positive_cases:
-            testcases.append((schema, file, True))
-        for file in negative_cases:
-            testcases.append((schema, file, False))
+@dataclass(frozen=True)
+class SchemaTestCase:
+    base_url: str
+    schema_file: Traversable
+    xml_file: Traversable
+    should_match: bool
+
+    @property
+    def name(self) -> str:
+        return Path(urlsplit(self.base_url).path).name
+
+    @property
+    def schema_url(self) -> str:
+        return uri.resolve(self.base_url, self.schema_file.name)
+
+
+def _load_testcases() -> "Sequence[SchemaTestCase]":
+    testcases_dir = importlib_resources.files(TESTPKG) / "data/testcases"
+    testcases_url = urlhandlers.pydata.makeurl(TESTPKG, "data/testcases/")
+    assert testcases_dir.is_dir()
+
+    testcases: list[SchemaTestCase] = []
+
+    for tc_dir in testcases_dir.iterdir():
+        tc_dir_url = uri.resolve(testcases_url, f"{tc_dir.name}/")
+
+        schema = tc_dir / "schema.rng"
+        positive_cases = [
+            f for f in tc_dir.iterdir() if re.match(r"^positive.*\.xml$", f.name)
+        ]
+        negative_cases = [
+            f for f in tc_dir.iterdir() if re.match(r"^negative.*\.xml$", f.name)
+        ]
+
+        assert len(positive_cases) > 0
+
+        testcases.extend(
+            SchemaTestCase(
+                base_url=tc_dir_url,
+                schema_file=schema,
+                xml_file=file,
+                should_match=should_match,
+            )
+            for (files, should_match) in [
+                (positive_cases, True),
+                (negative_cases, False),
+            ]
+            for file in files
+        )
 
-    assert testcases
+    assert len(testcases) > 0
     return testcases
 
 
-@pytest.mark.parametrize("href_text,encoded_url", [
-    # Spaces are escaped
-    ("/foo/bar baz.txt", "/foo/bar%20baz.txt"),
-    ("file:///foo/bar baz.txt", "file:///foo/bar%20baz.txt"),
-
-    ("http://example.com/Heizölrückstoßabdämpfung",
-     "http://example.com/Heiz%C3%B6lr%C3%BCcksto%C3%9Fabd%C3%A4mpfung"),
-
-    # urls which are already escaped are not double escaped
-    ("/foo/bar%20baz.txt", "/foo/bar%20baz.txt")
-])
-def test_escape_reserved(href_text, encoded_url):
+@pytest.mark.parametrize(
+    "href_text,encoded_url",
+    [
+        # Spaces are escaped
+        ("/foo/bar baz.txt", "/foo/bar%20baz.txt"),
+        ("file:///foo/bar baz.txt", "file:///foo/bar%20baz.txt"),
+        (
+            "http://example.com/Heizölrückstoßabdämpfung",
+            "http://example.com/Heiz%C3%B6lr%C3%BCcksto%C3%9Fabd%C3%A4mpfung",
+        ),
+        # urls which are already escaped are not double escaped
+        ("/foo/bar%20baz.txt", "/foo/bar%20baz.txt"),
+    ],
+)
+def test_escape_reserved(href_text: str, encoded_url: str) -> None:
     assert rnginline.escape_reserved_characters(href_text) == encoded_url
 
 
-def test_include_cant_inline_non_grammar_elements():
+def test_include_cant_inline_non_grammar_elements() -> None:
     """
     Verify that <include>s can't pull in a RNG file that doesn't start with a
     <grammar>.
     """
     illegal_url = urlhandlers.pydata.makeurl(
-        TESTPKG, "data/inline-non-grammar-els/illegal.rng")
+        TESTPKG, "data/inline-non-grammar-els/illegal.rng"
+    )
 
     with pytest.raises(InvalidGrammarError):
         rnginline.inline(url=illegal_url)
 
     legal_url = urlhandlers.pydata.makeurl(
-        TESTPKG, "data/inline-non-grammar-els/legal.rng")
+        TESTPKG, "data/inline-non-grammar-els/legal.rng"
+    )
     schema = rnginline.inline(url=legal_url)
 
     assert schema(etree.XML("<foo/>"))
 
 
-@pytest.mark.parametrize("schema_path", [
-    "data/datatype-library-inheritance/base-included.rng",
-    "data/datatype-library-inheritance/base-external.rng"
-])
-def test_inlined_files_dont_inherit_datatype(schema_path):
+@pytest.mark.parametrize(
+    "schema_path",
+    [
+        "data/datatype-library-inheritance/base-included.rng",
+        "data/datatype-library-inheritance/base-external.rng",
+    ],
+)
+def test_inlined_files_dont_inherit_datatype(schema_path: str) -> None:
     illegal_url = urlhandlers.pydata.makeurl(TESTPKG, schema_path)
 
     # Inlining will succeed
     grammar = rnginline.inline(url=illegal_url, create_validator=False)
 
     # But constructing a validator from the grammar XML will fail
     with pytest.raises(etree.RelaxNGError):
         etree.RelaxNG(grammar)
 
 
-def _testcase_id(tc):
-    prefix = "data/testcases/"
-    schema, file, should_match = tc
-
-    assert schema.startswith(prefix)
-    assert file.startswith(prefix)
-
-    return "{0},{1},{2}".format(schema[len(prefix):], file[len(prefix):],
-                                should_match)
+def _testcase_id(tc: SchemaTestCase) -> str:
+    return (
+        f"name:{tc.name},schema:{tc.schema_file.name},xml:{tc.xml_file.name},"
+        f"should_match:{tc.should_match}"
+    )
 
 
 test_testcases_testcases = _load_testcases()
 ttt_ids = [_testcase_id(tc) for tc in test_testcases_testcases]
 
 
-@pytest.mark.parametrize("schema_file,test_file,should_match",
-                         test_testcases_testcases, ids=ttt_ids)
-def test_testcases(schema_file, test_file, should_match):
-    schema = rnginline.inline(
-        urlhandlers.pydata.makeurl(TESTPKG, schema_file))
+@pytest.mark.parametrize("example", test_testcases_testcases, ids=ttt_ids)
+def test_testcases(example: SchemaTestCase) -> None:
+    schema = rnginline.inline(example.schema_url)
+
+    with importlib_resources.as_file(example.xml_file) as xml_path:
+        with xml_path.open("rb") as xml_file:
+            xml = etree.parse(xml_file)
 
-    xml = etree.parse(pr.resource_stream(TESTPKG, test_file))
-
-    if should_match:
+    if example.should_match:
         try:
             # Should match
             schema.assertValid(xml)
         except etree.DocumentInvalid:
-            pytest.fail("{0} should match {1} but didn't: {2}"
-                        .format(test_file, schema_file, schema.error_log))
+            pytest.fail(
+                f"{example.xml_file.name} should match {example.schema_file.name} "
+                f"but didn't: {schema.error_log}"
+            )
     else:
         with pytest.raises(etree.DocumentInvalid):
             # Shouldn't match
             schema.assertValid(xml)
-            pytest.fail("{0} shouldn't match {1} but did"
-                        .format(test_file, schema_file))
+            pytest.fail(
+                f"{example.xml_file.name} shouldn't match "
+                f"{example.schema_file.name} but did"
+            )
 
 
-def test_lxml_doesnt_honor_namespace_prefixes():
+def test_lxml_doesnt_honour_namespace_prefixes() -> None:
     a = etree.XML("""<a xmlns="foo" xmlns:f1="foo"><f1:b/></a>""")
     b = list(a)[0]
     c = etree.XML("""<f2:c xmlns:f2="foo" xmlns:f3="foo"><f3:d/></f2:c>""")
     d = list(c)[0]
 
     assert a.prefix is None
     assert b.prefix == "f1"
@@ -149,18 +187,18 @@
     assert d.prefix == "f3"
 
     # Now merge them, we'll lose the prefixes
     b.insert(0, c)
     assert a.prefix is None
     assert b.prefix == "f1"  # This won't change as we've not reinserted it
     assert c.prefix is None  # These get nuked though
-    assert d.prefix is None
+    assert d.prefix is None  # type: ignore[unreachable]
 
 
-def test_deferred_xml_insertion__replace():
+def test_deferred_xml_insertion__replace() -> None:
     a = etree.XML("""<a xmlns="foo" xmlns:f1="foo"><f1:b/></a>""")
     b = list(a)[0]
     c = etree.XML("""<f2:c xmlns:f2="foo" xmlns:f3="foo"><f3:d/></f2:c>""")
     d = list(c)[0]
 
     assert a.prefix is None
     assert c.prefix == "f2"
@@ -177,43 +215,67 @@
 
     # The prefixes are not nuked though
     assert new_a.prefix is None and new_a.tag == "{foo}a"
     assert new_c.prefix == "f2" and new_c.tag == "{foo}c"
     assert new_d.prefix == "f3" and new_d.tag == "{foo}d"
 
 
-def test_deferred_xml_insertion__replace_root_can_only_happen_once():
+def test_deferred_xml_insertion__replace_root_can_only_happen_once() -> None:
     a = etree.XML("""<a><b/></a>""")
     c = etree.XML("""<c><d/></c>""")
     d = list(c)[0]
 
     dxi = DeferredXmlInsertion(a)
     dxi.register_replace(a, c)
 
     # We don't allow the root to be replaced twice. Mainly because we never
     # need to, so it would indicate an error.
     with pytest.raises(ValueError):
         dxi.register_replace(a, d)
 
 
-def test_deferred_xml_insertion__perform_insertions_can_only_happen_once():
+def test_deferred_xml_insertion__perform_insertions_can_only_happen_once() -> None:
     a = etree.XML("""<a><b/></a>""")
     b = list(a)[0]
     c = etree.XML("""<c><d/></c>""")
 
     dxi = DeferredXmlInsertion(a)
     dxi.register_replace(b, c)
 
     dxi.perform_insertions()  # first time
     # We don't allow insertions to be performed twice, as it's never necessary
     with pytest.raises(AssertionError):
         dxi.perform_insertions()  # second time
 
 
-def test_foreign_attrs_cant_be_in_default_ns():
+def test_deferred_xml_insertion__iter_root_elements() -> None:
+    level0 = etree.XML("""<level0><thing/></level0>""")
+    level1a = etree.XML("""<level1a><thing/></level1a>""")
+    level1b = etree.XML("""<level1b/>""")
+    level2a = etree.XML("""<level2a/>""")
+    level2b = etree.XML("""<level2b/>""")
+    other = etree.XML("""<foo/>""")
+
+    dxi_l1a = DeferredXmlInsertion(level1a)
+    dxi_l1a.register_replace(
+        old_el=list(level1a)[0], new_el=DeferredXmlInsertion(level2a)
+    )
+    dxi_l1b = DeferredXmlInsertion(level1b)
+    dxi_l1b.register_insert(parent=level1b, index=0, el=DeferredXmlInsertion(level2b))
+
+    dxi = DeferredXmlInsertion(level0)
+    dxi.register_replace(old_el=list(level0)[0], new_el=dxi_l1a)
+    dxi.register_insert(parent=level0, index=1, el=dxi_l1b)
+    dxi.register_insert(parent=level0, index=2, el=other)
+
+    roots = [root for root in dxi.iter_root_elements()]
+    assert roots == [level0, level1a, level2a, level1b, level2b, other]
+
+
+def test_foreign_attrs_cant_be_in_default_ns() -> None:
     xml = """\
     <grammar xmlns="http://relaxng.org/ns/structure/1.0">
         <start {0}>
             <element name="foo">
                 <empty/>
             </element>
         </start>
@@ -221,83 +283,95 @@
     """
     rnginline.inline(etree=etree.XML(xml.format("")))
 
     with pytest.raises(InvalidGrammarError):
         rnginline.inline(etree=etree.XML(xml.format('illegal-attr="abc"')))
 
 
-def test_include_loops_trigger_error():
+def test_include_loops_trigger_error() -> None:
     with pytest.raises(SchemaIncludesSelfError):
         rnginline.inline(
-            url=urlhandlers.pydata.makeurl(TESTPKG, "data/loops/start.rng"))
+            url=urlhandlers.pydata.makeurl(TESTPKG, "data/loops/start.rng")
+        )
 
 
-def test_include_cant_override_start_if_no_start_in_included_file():
+def test_include_cant_override_start_if_no_start_in_included_file() -> None:
     with pytest.raises(InvalidGrammarError):
-        rnginline.inline(url=urlhandlers.pydata.makeurl(
-            TESTPKG, "data/include-override-start/start.rng"))
+        rnginline.inline(
+            url=urlhandlers.pydata.makeurl(
+                TESTPKG, "data/include-override-start/start.rng"
+            )
+        )
 
 
-def test_include_cant_override_define_if_no_matching_define_in_included_file():
+def test_include_cant_override_define_if_no_matching_define_in_included_file() -> None:
     with pytest.raises(InvalidGrammarError):
-        rnginline.inline(url=urlhandlers.pydata.makeurl(
-            TESTPKG, "data/include-override-define/start.rng"))
-
-
-@pytest.mark.parametrize("xml,index,expected", [
-    ("""<a xmlns="foo" xmlns:f1="foo"/>""", 0, 0),
-    ("""<a xmlns="foo" xmlns:f1="foo"/>""", -2, 0),
-    ("""<a xmlns="foo" xmlns:f1="foo"/>""", 2, 0),
-    ("""<a xmlns="foo" xmlns:f1="foo"><b/></a>""", 0, 0),
-    ("""<a xmlns="foo" xmlns:f1="foo"><b/></a>""", 1, 1),
-    ("""<a xmlns="foo" xmlns:f1="foo"><b/></a>""", 4, 1),
-    ("""<a xmlns="foo" xmlns:f1="foo"><b/></a>""", -1, 0),
-    ("""<a xmlns="foo" xmlns:f1="foo"><b/><b/><b/></a>""", -1, 2),
-    ("""<a xmlns="foo" xmlns:f1="foo"><b/><b/><b/></a>""", -2, 1),
-    ("""<a xmlns="foo" xmlns:f1="foo"><b/><b/><b/></a>""", -3, 0),
-    ("""<a xmlns="foo" xmlns:f1="foo"><b/><b/><b/></a>""", 3, 3),
-    ("""<a xmlns="foo" xmlns:f1="foo"><b/><b/><b/></a>""", 5, 3)
-])
-def test_deferred_xml_insertion__insert(xml, index, expected):
+        rnginline.inline(
+            url=urlhandlers.pydata.makeurl(
+                TESTPKG, "data/include-override-define/start.rng"
+            )
+        )
+
+
+@pytest.mark.parametrize(
+    "xml,index,expected",
+    [
+        ("""<a xmlns="foo" xmlns:f1="foo"/>""", 0, 0),
+        ("""<a xmlns="foo" xmlns:f1="foo"/>""", -2, 0),
+        ("""<a xmlns="foo" xmlns:f1="foo"/>""", 2, 0),
+        ("""<a xmlns="foo" xmlns:f1="foo"><b/></a>""", 0, 0),
+        ("""<a xmlns="foo" xmlns:f1="foo"><b/></a>""", 1, 1),
+        ("""<a xmlns="foo" xmlns:f1="foo"><b/></a>""", 4, 1),
+        ("""<a xmlns="foo" xmlns:f1="foo"><b/></a>""", -1, 0),
+        ("""<a xmlns="foo" xmlns:f1="foo"><b/><b/><b/></a>""", -1, 2),
+        ("""<a xmlns="foo" xmlns:f1="foo"><b/><b/><b/></a>""", -2, 1),
+        ("""<a xmlns="foo" xmlns:f1="foo"><b/><b/><b/></a>""", -3, 0),
+        ("""<a xmlns="foo" xmlns:f1="foo"><b/><b/><b/></a>""", 3, 3),
+        ("""<a xmlns="foo" xmlns:f1="foo"><b/><b/><b/></a>""", 5, 3),
+    ],
+)
+def test_deferred_xml_insertion__insert(xml: str, index: int, expected: int) -> None:
     a = etree.XML(xml)
     c = etree.XML("""<f2:c xmlns:f2="foo" xmlns:f3="foo"><f3:d/></f2:c>""")
     d = list(c)[0]
 
     assert a.prefix is None
     assert c.prefix == "f2"
     assert d.prefix == "f3"
 
     dxi = DeferredXmlInsertion(a)
     dxi.register_insert(a, index, c)
     new_a = dxi.perform_insertions()
     new_c = new_a.find("{foo}c")
+    assert new_c is not None
     new_d = list(new_c)[0]
 
     assert new_a.prefix is None
     assert new_c.prefix == "f2"
     assert new_d.prefix == "f3"
 
     assert new_a.index(new_c) == expected
 
 
-def test_multiple_references_to_same_uri_results_in_1_fetch():
+def test_multiple_references_to_same_uri_results_in_1_fetch() -> None:
     handler = urlhandlers.PackageDataUrlHandler()
     # Mock the dereference method to allow calls to be observed
-    handler.dereference = mock.Mock(side_effect=handler.dereference)
+    handler.dereference = mock.Mock(  # type: ignore[method-assign]
+        side_effect=handler.dereference
+    )
 
-    url = urlhandlers.pydata.makeurl(
-        TESTPKG, "data/multiple-ref-1-fetch/schema.rng")
+    url = urlhandlers.pydata.makeurl(TESTPKG, "data/multiple-ref-1-fetch/schema.rng")
 
     rnginline.inline(url=url, handlers=[handler])
 
     # schema.rng, indrect.rng & 5x popular.rng = 3 fetches total
     assert len(handler.dereference.mock_calls) == 3
 
 
-def test_inline_url_arguments_are_resolved_against_default_base_uri():
+def test_inline_url_arguments_are_resolved_against_default_base_uri() -> None:
     class Stop(Exception):
         pass
 
     # Mock the dereference method to allow calls to be observed
     handler = mock.MagicMock()
     handler.can_handle.return_value = True
     handler.dereference.side_effect = Stop
@@ -313,207 +387,224 @@
     expected_url = uri.resolve(expected_base, url)
     assert expected_url.startswith(expected_base)
     assert expected_url.endswith("somefile.txt")
 
     handler.dereference.assert_called_once_with(expected_url)
 
 
-def test_override_default_base_uri():
-    default_base_uri = urlhandlers.pydata.makeurl(TESTPKG,
-                                                  "data/testcases/xml-base/")
-    schema = rnginline.inline(url="schema.rng",
-                                  default_base_uri=default_base_uri)
+def test_override_default_base_uri() -> None:
+    default_base_uri = urlhandlers.pydata.makeurl(TESTPKG, "data/testcases/xml-base/")
+    schema = rnginline.inline(url="schema.rng", default_base_uri=default_base_uri)
 
     xml_url = uri.resolve(default_base_uri, "positive-1.xml")
     xml = etree.fromstring(urlhandlers.pydata.dereference(xml_url))
 
     assert schema(xml)
 
 
-def test_overridden_default_base_uri_must_be_absolute():
+def test_overridden_default_base_uri_must_be_absolute() -> None:
     """
     The default base URI must be an absolute URI. i.e. matches the URI grammar,
     not the URI-reference grammar.
     """
     relative_uri = "/some/path/blah"
     assert uri.is_uri_reference(relative_uri)
     assert not uri.is_uri(relative_uri)
 
     with pytest.raises(ValueError):
         rnginline.Inliner(default_base_uri=relative_uri)
 
 
-def test_provide_base_uri():
+def test_provide_base_uri() -> None:
     """
     This tests manually specifying a base URI to use for the source.
     """
-    base_uri = urlhandlers.pydata.makeurl(TESTPKG,
-                                          "data/testcases/xml-base/schema.rng")
+    base_uri = urlhandlers.pydata.makeurl(TESTPKG, "data/testcases/xml-base/schema.rng")
     # Use a file object so that the inliner won't know the URI of the src
     fileobj = io.BytesIO(urlhandlers.pydata.dereference(base_uri))
 
-    schema = rnginline.inline(fileobj, base_uri=base_uri,
-                              # our base URI is absolute, so the default
-                              # base won't have any effect.
-                              default_base_uri="x:/blah")
+    schema = rnginline.inline(
+        fileobj,
+        base_uri=base_uri,
+        # our base URI is absolute, so the default
+        # base won't have any effect.
+        default_base_uri="x:/blah",
+    )
 
     xml_url = uri.resolve(base_uri, "positive-1.xml")
     xml = etree.fromstring(urlhandlers.pydata.dereference(xml_url))
 
     assert schema(xml)
 
 
-def test_overridden_base_uri_must_be_uri_ref():
+def test_overridden_base_uri_must_be_uri_ref() -> None:
     """
     The base URI, if specified, must match the URI-reference grammar. i.e. it
     is a relative or absolute URI.
     """
     bad_uri = "x:/some/path/spaces not allowed/oops"
     assert not uri.is_uri_reference(bad_uri)
 
     with pytest.raises(ValueError):
         rnginline.inline(
             # some random schema, not of any significance
             uri.resolve(DATA_URI, "testcases/include-1/schema.rng"),
-            base_uri=bad_uri)
+            base_uri=bad_uri,
+        )
 
 
-def test_unhandleable_url_raises_error():
+def test_unhandleable_url_raises_error() -> None:
     with pytest.raises(NoAvailableHandlerError):
         rnginline.inline(url="my-fancy-url-scheme:/foo")
 
 
-def test_context_pushes_must_have_parents_except_first():
+def test_context_pushes_must_have_parents_except_first() -> None:
     context = rnginline.InlineContext()
 
     with context.track("x:/some/url"):
         with pytest.raises(ValueError):
             # Tracking second URL without passing context el: not allowed
             with context.track("x:/other/url"):
                 pass
 
 
-def test_including_invalid_xml_file_raises_parse_error():
-    url = urlhandlers.pydata.makeurl(TESTPKG,
-                                     "data/include-invalid-xml/ok.rng")
+def test_including_invalid_xml_file_raises_parse_error() -> None:
+    url = urlhandlers.pydata.makeurl(TESTPKG, "data/include-invalid-xml/ok.rng")
     with pytest.raises(ParseError):
         rnginline.inline(url=url)
 
 
-def test_including_non_rng_xml_file_raises_invalid_grammar_error():
-    url = urlhandlers.pydata.makeurl(TESTPKG,
-                                     "data/include-non-rng-xml/ok.rng")
+def test_including_non_rng_xml_file_raises_invalid_grammar_error() -> None:
+    url = urlhandlers.pydata.makeurl(TESTPKG, "data/include-non-rng-xml/ok.rng")
     with pytest.raises(InvalidGrammarError):
         rnginline.inline(url=url)
 
 
-def test_calling_inline_with_0_args_raises_value_error():
+def test_calling_inline_with_0_args_raises_value_error() -> None:
     with pytest.raises(ValueError):
         rnginline.inline()
 
 
-def test_inline_etree_el_with_no_base_uri_uses_default_base_uri():
-    base_url = urlhandlers.pydata.makeurl(TESTPKG,
-                                          "data/testcases/xml-base/")
-    schema_bytes = urlhandlers.pydata.dereference(
-        uri.resolve(base_url, "schema.rng"))
+def test_inline_etree_el_with_no_base_uri_uses_default_base_uri() -> None:
+    base_url = urlhandlers.pydata.makeurl(TESTPKG, "data/testcases/xml-base/")
+    schema_bytes = urlhandlers.pydata.dereference(uri.resolve(base_url, "schema.rng"))
 
     schema_el = etree.fromstring(schema_bytes)
     assert schema_el.getroottree().docinfo.URL is None
 
     # The default-default base URI is the pwd, so let's use something else
     # to demonstrate this. An unhandlable URI will result in a
     # NoAvailableHandlerError when the first href is dereferenced.
     with pytest.raises(NoAvailableHandlerError):
         rnginline.inline(etree=schema_el, default_base_uri="x:")
 
     # If we use a sensible default base URI the references will be resolved OK,
     # even though the XML document itself has no base URI
     schema = rnginline.inline(etree=schema_el, default_base_uri=base_url)
 
-    assert schema(etree.fromstring(urlhandlers.pydata.dereference(
-        uri.resolve(base_url, "positive-1.xml"))))
+    assert schema(
+        etree.fromstring(
+            urlhandlers.pydata.dereference(uri.resolve(base_url, "positive-1.xml"))
+        )
+    )
 
 
-def test_inline_args_etree_as_src():
+def test_inline_args_etree_as_src() -> None:
     url = uri.resolve(DATA_URI, "testcases/xml-base/schema.rng")
-    schema_el = etree.fromstring(urlhandlers.pydata.dereference(
-        uri.resolve(DATA_URI, "testcases/xml-base/schema.rng")), base_url=url)
+    schema_el = etree.fromstring(
+        urlhandlers.pydata.dereference(
+            uri.resolve(DATA_URI, "testcases/xml-base/schema.rng")
+        ),
+        base_url=url,
+    )
 
     assert etree.iselement(schema_el)
 
     # pass schema_el as src, should be detected as an Element
     schema = rnginline.inline(schema_el)
 
-    assert schema(etree.fromstring(urlhandlers.pydata.dereference(
-        uri.resolve(url, "positive-1.xml"))))
+    assert schema(
+        etree.fromstring(
+            urlhandlers.pydata.dereference(uri.resolve(url, "positive-1.xml"))
+        )
+    )
 
 
-def test_inline_args_etree_doc_as_src():
+def test_inline_args_etree_doc_as_src() -> None:
     url = uri.resolve(DATA_URI, "testcases/xml-base/schema.rng")
-    schema_el = etree.fromstring(urlhandlers.pydata.dereference(
-        uri.resolve(DATA_URI, "testcases/xml-base/schema.rng")), base_url=url)
+    schema_el = etree.fromstring(
+        urlhandlers.pydata.dereference(
+            uri.resolve(DATA_URI, "testcases/xml-base/schema.rng")
+        ),
+        base_url=url,
+    )
 
     schema_root = schema_el.getroottree()
     assert not etree.iselement(schema_root)
 
     # pass etree document (not el) as src, should pull out root el and use it
     schema = rnginline.inline(schema_root)
 
-    assert schema(etree.fromstring(urlhandlers.pydata.dereference(
-        uri.resolve(url, "positive-1.xml"))))
+    assert schema(
+        etree.fromstring(
+            urlhandlers.pydata.dereference(uri.resolve(url, "positive-1.xml"))
+        )
+    )
 
 
-def test_inline_args_url_refs_must_be_valid():
+def test_inline_args_url_refs_must_be_valid() -> None:
     bad_url = "/tmp/File Name With Spaces"
     assert not uri.is_uri_reference(bad_url)
 
     with pytest.raises(ValueError):
         rnginline.inline(url=bad_url)
 
 
-def test_inline_args_fs_path_as_src():
+def test_inline_args_fs_path_as_src() -> None:
     grammar_xml = b"""
     <element name="start" xmlns="http://relaxng.org/ns/structure/1.0">
         <empty/>
     </element>
     """
     path = "/some/dir/Filename with spaces.rng"
     handler = urlhandlers.FilesystemUrlHandler()
-    handler.dereference = mock.Mock(side_effect=[grammar_xml])
+    handler.dereference = mock.Mock(  # type: ignore[method-assign]
+        side_effect=[grammar_xml]
+    )
 
     rnginline.inline(path, handlers=[handler])
 
     handler.dereference.assert_called_once_with(
-        urlhandlers.file.makeurl(path, abs=True))
+        urlhandlers.file.makeurl(path, abs=True)
+    )
 
 
-def test_inline_args_passing_garbage():
+def test_inline_args_passing_garbage() -> None:
     with pytest.raises(ValueError):
         # pass a useless arg as src
-        rnginline.inline(1234)
+        rnginline.inline(1234)  # type: ignore[call-overload]
 
 
-def test_context_pop_with_no_context_raises_error():
+def test_context_pop_with_no_context_raises_error() -> None:
     context = rnginline.InlineContext()
 
     with pytest.raises(ValueError):
-        context._pop_context("x:/url", None)
+        context._pop_context("x:/url", None)  # type: ignore[arg-type]
 
 
-def test_context_pop_with_mismatching_url_raises_error():
+def test_context_pop_with_mismatching_url_raises_error() -> None:
     context = rnginline.InlineContext()
     token = context._push_context("x:/foo", None)
 
     with pytest.raises(ValueError):
         # different URL to push call
         context._pop_context("x:/bar", token)
 
 
-def test_context_pop_with_mismatching_token_raises_error():
+def test_context_pop_with_mismatching_token_raises_error() -> None:
     context = rnginline.InlineContext()
     url = "x:/foo"
     context._push_context(url, None)  # Ignore the returned token
 
     with pytest.raises(ValueError):
         # different token to push call
-        context._pop_context(url, object())
+        context._pop_context(url, InlineContextToken())
```

### Comparing `rnginline-0.0.2/rnginline/test/test_urlhandlers.py` & `rnginline-1.0.0rc1/rnginline/test/test_urlhandlers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,181 +1,143 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals
+from __future__ import annotations
 
 import os
 import tempfile
+from urllib import parse
 
 import pytest
-import six
-from six.moves.urllib import parse
 
 from rnginline.exceptions import DereferenceError
-from rnginline.urlhandlers import (reject_bytes, ensure_parsed, quote,
-                                   unquote, file, pydata)
+from rnginline.urlhandlers import ensure_parsed, file, pydata
 
 
-def test_reject_bytes():
-    reject_bytes(foo="bar", bar="baz", baz="boz")
-
-    with pytest.raises(ValueError) as excinfo:
-        reject_bytes(foo="bar", bar=b"baz", baz="boz")
-
-    assert "bar" in six.text_type(excinfo.value)
-
-
-def test_ensure_parsed():
+def test_ensure_parsed() -> None:
     assert isinstance(ensure_parsed("x:/foo"), parse.SplitResult)
-    assert isinstance(ensure_parsed(parse.urlsplit("x:/foo")),
-                      parse.SplitResult)
+    assert isinstance(ensure_parsed(parse.urlsplit("x:/foo")), parse.SplitResult)
 
 
-@pytest.mark.parametrize("text", [
-    "foo",
-    "ƒß∂åƒ∂ß",
-    "abc\U00010300\U00010410def"
-])
-def test_quoting_roundtrip(text):
-    quoted = quote(text)
-    unquoted = unquote(quoted)
-
-    # Always working with text, not bytes
-    assert isinstance(text, six.text_type)
-    assert isinstance(quoted, six.text_type)
-    assert isinstance(unquoted, six.text_type)
-
-    # The quoted result should have no non-ascii chars
-    assert quoted.encode("ascii").decode("ascii") == quoted
-
-    # End result should match the input
-    assert unquoted == text
-
-
-@pytest.mark.parametrize("path,abs,expected_url,expected_path", [
-    ("foo", True, "file:foo", "foo"),
-    ("foo", False, "foo", "foo"),
-    ("foo", None, "foo", "foo"),
-    ("/some/dir/foo", True, "file:/some/dir/foo", "/some/dir/foo"),
-    ("/some/dir/foo", False, "/some/dir/foo", "/some/dir/foo"),
-    ("/some/dir/foo", None, "/some/dir/foo", "/some/dir/foo"),
-
-    ("some dir/foo bar", True,
-     "file:some%20dir/foo%20bar", "some dir/foo bar"),
-    ("some dir/foo bar", False,
-     "some%20dir/foo%20bar", "some dir/foo bar"),
-    ("some dir/foo bar", None,
-     "some%20dir/foo%20bar", "some dir/foo bar")
-])
-def test_file_url_roundtrip(path, abs, expected_url, expected_path):
+@pytest.mark.parametrize(
+    "path,abs,expected_url,expected_path",
+    [
+        ("foo", True, "file:foo", "foo"),
+        ("foo", False, "foo", "foo"),
+        ("foo", None, "foo", "foo"),
+        ("/some/dir/foo", True, "file:/some/dir/foo", "/some/dir/foo"),
+        ("/some/dir/foo", False, "/some/dir/foo", "/some/dir/foo"),
+        ("/some/dir/foo", None, "/some/dir/foo", "/some/dir/foo"),
+        ("some dir/foo bar", True, "file:some%20dir/foo%20bar", "some dir/foo bar"),
+        ("some dir/foo bar", False, "some%20dir/foo%20bar", "some dir/foo bar"),
+        ("some dir/foo bar", None, "some%20dir/foo%20bar", "some dir/foo bar"),
+    ],
+)
+def test_file_url_roundtrip(
+    path: str, abs: bool | None, expected_url: str, expected_path: str
+) -> None:
     kwargs = {"abs": abs} if abs is not None else {}
     result_url = file.makeurl(path, **kwargs)
 
-    assert isinstance(result_url, six.text_type)
+    assert isinstance(result_url, str)
     assert result_url == expected_url
 
     result_path = None
     try:
         result_path = file.breakurl(result_url)
         assert result_path is not None
     except ValueError as e:
         if expected_path is not None:
             raise e
 
-    assert isinstance(result_url, (six.text_type, type(None)))
+    assert isinstance(result_url, (str, type(None)))
     assert result_path == expected_path
 
 
-def test_file_breakurl_permits_relative_urls():
+def test_file_breakurl_permits_relative_urls() -> None:
     assert file.breakurl("foo/bar%20baz.txt") == "foo/bar baz.txt"
 
 
-def test_file_breakurl_rejects_abs_urls_of_wrong_scheme():
+def test_file_breakurl_rejects_abs_urls_of_wrong_scheme() -> None:
     with pytest.raises(ValueError):
         file.breakurl("notfile:foo/bar%20baz.txt")
 
 
-def test_fs_handler_handles_file_uris():
+def test_fs_handler_handles_file_uris() -> None:
     assert file.can_handle(parse.urlsplit("file:some/file"))
 
 
-def test_fs_handler_doesnt_handle_raw_paths():
+def test_fs_handler_doesnt_handle_raw_paths() -> None:
     assert not file.can_handle(parse.urlsplit("some/file"))
 
 
-def test_file_url_creates_file_urls():
+def test_file_url_creates_file_urls() -> None:
     file_url = file.makeurl("some/file/∑´^¨∂ƒ", abs=True)
-    assert type(file_url) == six.text_type
+    assert type(file_url) == str
     assert file_url == "file:some/file/%E2%88%91%C2%B4%5E%C2%A8%E2%88%82%C6%92"
     assert file.breakurl(file_url) == "some/file/∑´^¨∂ƒ"
 
 
-def test_fs_handler_raises_dereference_error_on_missing_files():
+def test_fs_handler_raises_dereference_error_on_missing_files() -> None:
     handle, path = tempfile.mkstemp(suffix="∆˚¬ß∂ƒ")
     os.close(handle)
     os.unlink(path)
 
     url = file.makeurl(path, abs=True)
     with pytest.raises(DereferenceError) as e:
         file.dereference(parse.urlsplit(url))
-    assert url in six.text_type(e.value)
+    assert url in str(e.value)
 
 
-def test_fs_handler_reads_file_at_url():
+def test_fs_handler_reads_file_at_url() -> None:
     handle, path = tempfile.mkstemp(suffix="∆˚¬ß∂ƒ")
 
     contents = "This is some text\nblah blah\n´∑®ƒ∂ß˚\n".encode("utf-8")
 
     with os.fdopen(handle, "wb") as f:
         f.write(contents)
 
     url = file.makeurl(path, abs=True)
     result = file.dereference(parse.urlsplit(url))
     assert result == contents
     os.unlink(path)
 
 
-data_data_data_uri = ("pydata://rnginline.test/data/"
-                      "data-%C9%90%CA%87%C9%90p-data.txt")
+data_data_data_uri = "pydata://rnginline.test/data/" "data-%C9%90%CA%87%C9%90p-data.txt"
 
 
-def test_pydata_uri_creation():
-    assert type(data_data_data_uri) == six.text_type
+def test_pydata_uri_creation() -> None:
+    assert type(data_data_data_uri) == str
     package, path = "rnginline.test", "data/data-ɐʇɐp-data.txt"
     created_url = pydata.makeurl(package, path)
 
-    assert type(created_url) == six.text_type
+    assert type(created_url) == str
     assert data_data_data_uri == created_url
     assert pydata.breakurl(created_url) == (package, path)
 
 
-def test_pydata_path_must_be_relative():
+def test_pydata_path_must_be_relative() -> None:
     with pytest.raises(ValueError):
         pydata.makeurl("foo", "/abs/path")
 
 
-def test_pydata_package_name_must_be_python_name():
+def test_pydata_package_name_must_be_python_name() -> None:
     with pytest.raises(ValueError):
         pydata.makeurl("ƒancy-name", "foo/bar")
 
 
-@pytest.mark.skipif(six.PY3, reason="Python 2 specific behaviour")
-def test_pydata_uri_creation_allows_package_as_bytes():
-    # On py2 __name__ is a byte string, so it makes sense to accept bytes for
-    # the package
-    pydata.makeurl("foo".encode("ascii"), "bar.txt")
-
-
-def test_pydata_url_deconstruct_requries_pydata_scheme():
+def test_pydata_url_deconstruct_requries_pydata_scheme() -> None:
     with pytest.raises(ValueError):
         pydata.breakurl("foo://bar/baz")
 
 
-def test_pydata_handler_handles_pydata_uris():
+def test_pydata_handler_handles_pydata_uris() -> None:
     assert pydata.can_handle(parse.urlsplit(data_data_data_uri))
 
 
-@pytest.mark.parametrize("url", [
-    pydata.makeurl("rnginline.tset", "data"),  # dir, not file
-    pydata.makeurl("rnginline.tset", "data/jfklsjflsdf.txt")
-])
-def test_pydata_handler_raises_dereference_error_on_missing_file(url):
+@pytest.mark.parametrize(
+    "url",
+    [
+        pydata.makeurl("rnginline.tset", "data"),  # dir, not file
+        pydata.makeurl("rnginline.tset", "data/jfklsjflsdf.txt"),
+    ],
+)
+def test_pydata_handler_raises_dereference_error_on_missing_file(url: str) -> None:
     with pytest.raises(DereferenceError):
         pydata.dereference(url)
```

### Comparing `rnginline-0.0.2/rnginline/uri.py` & `rnginline-1.0.0rc1/rnginline/uri.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 """
 This module contains URI related functions, implemented according to
 `RFC 3986`_.
 
 .. _RFC 3986: https://tools.ietf.org/html/rfc3986
 """
-from __future__ import unicode_literals
+from __future__ import annotations
 
-from six.moves.urllib.parse import urlsplit, SplitResult
+from typing import Union
+from urllib.parse import SplitResult, urlsplit
 
 from rnginline import uri_regex
 
+__all__ = ["UriSyntaxError", "is_uri", "is_uri_reference", "resolve", "recombine"]
 
-__all__ = ["UriSyntaxError", "is_uri", "is_uri_reference", "resolve",
-           "recombine"]
+SplitResultInput = Union[
+    SplitResult, "tuple[str | None, str | None, str | None, str | None, str | None]"
+]
 
 
 class UriSyntaxError(ValueError):
     pass
 
 
-def is_uri(text):
+def is_uri(text: str) -> bool:
     """
     Checks if text matches the "URI" grammar rule from RFC 3986.
 
     Note the URI rule is LESS general than URI-reference - it requires an
     absolute URI with a scheme.
     """
     return _matches_uri_pattern_rule("URI", text)
 
 
-def is_uri_reference(text):
+def is_uri_reference(text: str) -> bool:
     """
     Checks if text matches the "URI-reference" grammar rule from RFC 3986.
 
     Note that the URI-reference rule is MORE general than URI - it can be
     a relative path by itself or an absolute URI with scheme.
     """
     return _matches_uri_pattern_rule("URI-reference", text)
 
 
-def _matches_uri_pattern_rule(rule, text):
+def _matches_uri_pattern_rule(rule: uri_regex.RfcName, text: str) -> bool:
     return bool(uri_regex.get_regex(rule).match(text))
 
 
-def resolve(base, reference, strict=True):
+def resolve(base: str, reference: str, strict: bool = True) -> str:
     """
     Resolve a reference URI against a base URI to form a target URI.
 
     Implements relative URI resolution according to RFC 3986 section 5.2.
     "Relative Resolution".
 
     Note that urllib.urljoin does not work with non-standard schemes (like our
     pydata: scheme) hence this implementation...
     """
     if not is_uri(base):
         raise UriSyntaxError("base was not a valid URI: {0}".format(base))
     if not is_uri_reference(reference):
-        raise UriSyntaxError("reference was not a valid URI-reference: {0}"
-                             .format(reference))
+        raise UriSyntaxError(
+            "reference was not a valid URI-reference: {0}".format(reference)
+        )
 
     b, ref = urlsplit(base), urlsplit(reference)
 
     scheme, authority, path, query, fragment = None, None, None, None, None
 
     if not strict and ref.scheme == b.scheme:
         ref = SplitResult("", *ref[1:])
@@ -92,37 +96,37 @@
             authority = b.netloc
         scheme = b.scheme
     fragment = ref.fragment
 
     return recombine(SplitResult(scheme, authority, path, query, fragment))
 
 
-def _merge(base, ref_path):
+def _merge(base: SplitResult, ref_path: str) -> str:
     """
     Resolve ref_path against the base path.
 
     Implements 5.2.3. Merge Paths.
     """
     if base.netloc and not base.path:
         assert not ref_path.startswith("/")
         return "/" + ref_path
     base_parts = base.path.split("/")
     if len(base_parts) == 1:
         return ref_path
     return "/".join(base_parts[:-1] + ref_path.split("/"))
 
 
-def _remove_dot_segments(path):
+def _remove_dot_segments(path: str) -> str:
     """
     Remove . and .. segments from path.
 
     Implements 5.2.4. Remove Dot Segments.
     """
     input = path
-    output = []
+    output: list[str] = []
 
     while input:
         # A
         if input.startswith("./"):
             input = input[2:]
         elif input.startswith("../"):
             input = input[3:]
@@ -151,38 +155,39 @@
             else:
                 output += input
                 input = ""
 
     return "".join(output)
 
 
-def recombine(spliturl):
+def recombine(spliturl: SplitResultInput) -> str:
     """
     Combine a SplitResult into a URI string.
 
     Implements section 5.3 Component Recomposition.
     """
     scheme, netloc, path, query, fragment = spliturl
     out = []
 
     # Refuse to construct a broken URI-reference
     if netloc and path and not path.startswith("/"):
         raise UriSyntaxError(
             "With a netloc present the path must be absolute or empty. "
-            "path: {0}".format(path))
+            "path: {0}".format(path)
+        )
 
     if scheme:
         out.append(scheme)
         out.append(":")
 
     if netloc:
         out.append("//")
         out.append(netloc)
 
-    out.append(path)
+    out.append(path or "")
 
     if query:
         out.append("?")
         out.append(query)
 
     if fragment:
         out.append("#")
```

### Comparing `rnginline-0.0.2/rnginline/uri_regex.py` & `rnginline-1.0.0rc1/rnginline/uri_regex.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 """
 This module provides regular expressions matching the ABNF rules for URIs
 specified in Appendix A of rfc 3986:
 
     https://tools.ietf.org/html/rfc3986#appendix-A
 """
-from __future__ import unicode_literals
+from __future__ import annotations
 
-from rnginline.regexbuilder import (Set, Sequence, Literal, Optional,
-                                    Choice, ZeroOrMore, OneOrMore, Repeat,
-                                    Regex, Start, End)
+import re
+from functools import lru_cache
+from typing import Mapping
+
+from typing_extensions import Literal as TypingLiteral
+
+from rnginline.regexbuilder import (
+    Choice,
+    End,
+    Literal,
+    OneOrMore,
+    Optional,
+    Regex,
+    Repeat,
+    Sequence,
+    Set,
+    Start,
+    ZeroOrMore,
+)
 
 # The rules here are named according to those in RFC 3986, but transformed to
 # make them valid Python identifiers. Mixed case rules are lower cased and,
 # hyphens are replaced with underscores.
 
 ALPHA = Set(("a", "z"), ("A", "Z"))
 DIGIT = Set(("0", "9"))
@@ -30,144 +46,193 @@
 
 pchar = Choice(pct_encoded, Set(unreserved, sub_delims, *list(":@")))
 
 query = ZeroOrMore(Choice(pchar, Set(*list("/?"))))
 
 fragment = query
 
-segment_nz_nc = OneOrMore(Choice(pct_encoded,
-                                 Set(unreserved, sub_delims, "@")))
+segment_nz_nc = OneOrMore(Choice(pct_encoded, Set(unreserved, sub_delims, "@")))
 
 segment_nz = OneOrMore(pchar)
 
 segment = ZeroOrMore(pchar)
 
 path_empty = Literal("")
 
 _zom_segments = ZeroOrMore(Sequence(Literal("/"), segment))
 
 path_rootless = Sequence(segment_nz, _zom_segments)
 
 path_noscheme = Sequence(segment_nz_nc, _zom_segments)
 
-path_absolute = Sequence(
-    Literal("/"), Optional(Sequence(segment_nz, _zom_segments)))
+path_absolute = Sequence(Literal("/"), Optional(Sequence(segment_nz, _zom_segments)))
 
 path_abempty = _zom_segments
 
-path = Choice(path_abempty,
-              path_absolute,
-              path_noscheme,
-              path_rootless,
-              path_empty)
+path = Choice(path_abempty, path_absolute, path_noscheme, path_rootless, path_empty)
 
 reg_name = ZeroOrMore(Choice(pct_encoded, Set(unreserved, sub_delims)))
 
 dec_octet = Choice(
     DIGIT,
     Sequence(Set((0x31, 0x39)), DIGIT),
     Sequence(Literal("1"), Repeat(DIGIT, count=2)),
     Sequence(Literal("2"), Set((0x30, 0x34)), DIGIT),
-    Sequence(Literal("25"), Set((0x30, 0x35))))
+    Sequence(Literal("25"), Set((0x30, 0x35))),
+)
 
-ipv4address = Sequence(dec_octet, Literal("."),
-                       dec_octet, Literal("."),
-                       dec_octet, Literal("."), dec_octet)
+ipv4address = Sequence(
+    dec_octet, Literal("."), dec_octet, Literal("."), dec_octet, Literal("."), dec_octet
+)
 
 h16 = Repeat(HEXDIG, min=1, max=4)
 
 ls32 = Choice(Sequence(h16, Literal(":"), h16), ipv4address)
 
 ipv6address = Choice(
     Sequence(Repeat(Sequence(h16, Literal(":")), count=6), ls32),
+    Sequence(Literal("::"), Repeat(Sequence(h16, Literal(":")), count=5), ls32),
+    Sequence(
+        Optional(h16), Literal("::"), Repeat(Sequence(h16, Literal(":")), count=4), ls32
+    ),
+    Sequence(
+        Optional(Sequence(Repeat(Sequence(h16, Literal(":")), max=1), h16)),
+        Literal("::"),
+        Repeat(Sequence(h16, Literal(":")), count=3),
+        ls32,
+    ),
+    Sequence(
+        Optional(Sequence(Repeat(Sequence(h16, Literal(":")), max=2), h16)),
+        Literal("::"),
+        Repeat(Sequence(h16, Literal(":")), count=2),
+        ls32,
+    ),
+    Sequence(
+        Optional(Sequence(Repeat(Sequence(h16, Literal(":")), max=3), h16)),
+        Literal("::"),
+        h16,
+        Literal(":"),
+        ls32,
+    ),
+    Sequence(
+        Optional(Sequence(Repeat(Sequence(h16, Literal(":")), max=4), h16)),
+        Literal("::"),
+        ls32,
+    ),
+    Sequence(
+        Optional(Sequence(Repeat(Sequence(h16, Literal(":")), max=5), h16)),
+        Literal("::"),
+        h16,
+    ),
+    Sequence(
+        Optional(Sequence(Repeat(Sequence(h16, Literal(":")), max=6), h16)),
+        Literal("::"),
+    ),
+)
 
-    Sequence(Literal("::"),
-             Repeat(Sequence(h16, Literal(":")), count=5), ls32),
+ipvfuture = Sequence(
+    Literal("v"),
+    OneOrMore(HEXDIG),
+    Literal("."),
+    OneOrMore(Set(unreserved, sub_delims, ":")),
+)
 
-    Sequence(Optional(h16),
-             Literal("::"),
-             Repeat(Sequence(h16, Literal(":")), count=4), ls32),
-
-    Sequence(Optional(Sequence(Repeat(Sequence(h16, Literal(":")),
-                                      max=1), h16)),
-             Literal("::"),
-             Repeat(Sequence(h16, Literal(":")), count=3), ls32),
-
-    Sequence(Optional(Sequence(Repeat(Sequence(h16, Literal(":")),
-                                      max=2), h16)),
-             Literal("::"),
-             Repeat(Sequence(h16, Literal(":")), count=2), ls32),
-
-    Sequence(Optional(Sequence(Repeat(Sequence(h16, Literal(":")),
-                                      max=3), h16)),
-             Literal("::"), h16, Literal(":"), ls32),
-
-    Sequence(Optional(Sequence(Repeat(Sequence(h16, Literal(":")),
-                                      max=4), h16)),
-             Literal("::"), ls32),
-
-    Sequence(Optional(Sequence(Repeat(Sequence(h16, Literal(":")),
-                                      max=5), h16)),
-             Literal("::"), h16),
-
-    Sequence(Optional(Sequence(Repeat(Sequence(h16, Literal(":")),
-                                      max=6), h16)),
-             Literal("::")),
-)
-
-ipvfuture = Sequence(Literal("v"), OneOrMore(HEXDIG), Literal("."),
-                     OneOrMore(Set(unreserved, sub_delims, ":")))
-
-ip_literal = Sequence(Literal("["),
-                      Choice(ipv6address, ipvfuture),
-                      Literal("]"))
+ip_literal = Sequence(Literal("["), Choice(ipv6address, ipvfuture), Literal("]"))
 
 port = ZeroOrMore(DIGIT)
 
 host = Choice(ip_literal, ipv4address, reg_name)
 
-userinfo = ZeroOrMore(Choice(pct_encoded,
-                      Set(unreserved, sub_delims, ":")))
+userinfo = ZeroOrMore(Choice(pct_encoded, Set(unreserved, sub_delims, ":")))
 
-authority = Sequence(Optional(Sequence(userinfo, Literal("@"))),
-                     host,
-                     Optional(Sequence(Literal(":"), port)))
+authority = Sequence(
+    Optional(Sequence(userinfo, Literal("@"))),
+    host,
+    Optional(Sequence(Literal(":"), port)),
+)
 
-scheme = Sequence(ALPHA,
-                  ZeroOrMore(Set(ALPHA, DIGIT, *list("+-."))))
+scheme = Sequence(ALPHA, ZeroOrMore(Set(ALPHA, DIGIT, *list("+-."))))
 
 relative_part = Choice(
     Sequence(Literal("//"), authority, path_abempty),
     path_absolute,
     path_noscheme,
-    path_empty
+    path_empty,
 )
 
-relative_ref = Sequence(relative_part,
-                        Optional(Sequence(Literal("?"), query)),
-                        Optional(Sequence(Literal("#"), fragment)))
+relative_ref = Sequence(
+    relative_part,
+    Optional(Sequence(Literal("?"), query)),
+    Optional(Sequence(Literal("#"), fragment)),
+)
 
 hier_part = Choice(
     Sequence(Literal("//"), authority, path_abempty),
     path_absolute,
     path_rootless,
-    path_empty
+    path_empty,
 )
 
-absolute_uri = Sequence(scheme, Literal(":"), hier_part,
-                        Optional(Sequence(Literal("?"), query)))
+absolute_uri = Sequence(
+    scheme, Literal(":"), hier_part, Optional(Sequence(Literal("?"), query))
+)
 
-uri = Sequence(scheme, Literal(":"), hier_part,
-               Optional(Sequence(Literal("?"), query)),
-               Optional(Sequence(Literal("#"), fragment)))
+uri = Sequence(
+    scheme,
+    Literal(":"),
+    hier_part,
+    Optional(Sequence(Literal("?"), query)),
+    Optional(Sequence(Literal("#"), fragment)),
+)
 
 uri_reference = Choice(uri, relative_ref)
 
+RfcName = TypingLiteral[
+    "URI",
+    "hier-part",
+    "URI-reference",
+    "absolute-URI",
+    "relative-ref",
+    "relative-part",
+    "scheme",
+    "authority",
+    "userinfo",
+    "host",
+    "port",
+    "IP-literal",
+    "IPvFuture",
+    "IPv6address",
+    "h16",
+    "ls32",
+    "IPv4address",
+    "dec-octet",
+    "reg-name",
+    "path",
+    "path-abempty",
+    "path-absolute",
+    "path-noscheme",
+    "path-rootless",
+    "path-empty",
+    "segment",
+    "segment-nz",
+    "segment-nz-nc",
+    "pchar",
+    "query",
+    "fragment",
+    "pct-encoded",
+    "unreserved",
+    "reserved",
+    "gen-delims",
+    "sub-delims",
+    "HEXDIG",
+    "ALPHA",
+    "DIGIT",
+]
 
-_rfc_names = {
+_rfc_names: Mapping[RfcName, Regex] = {
     "URI": uri,
     "hier-part": hier_part,
     "URI-reference": uri_reference,
     "absolute-URI": absolute_uri,
     "relative-ref": relative_ref,
     "relative-part": relative_part,
     "scheme": scheme,
@@ -198,31 +263,29 @@
     "pct-encoded": pct_encoded,
     "unreserved": unreserved,
     "reserved": reserved,
     "gen-delims": gen_delims,
     "sub-delims": sub_delims,
     "HEXDIG": HEXDIG,
     "ALPHA": ALPHA,
-    "DIGIT": DIGIT
+    "DIGIT": DIGIT,
 }
 
-_compiled_rule_cache = {}
 
-
-def get_regex(rule_name):
+@lru_cache(maxsize=len(_rfc_names))
+def get_regex(rule_name: RfcName) -> re.Pattern[str]:
     """
     Get a compiled regex which matches an entire string against the named rule
     from RFC 3986.
     """
-    if rule_name not in _compiled_rule_cache:
-        if rule_name not in _rfc_names:
-            raise ValueError("Unknown rule name: {0}".format(rule_name))
-        rule = _rfc_names[rule_name]
-        # Need to place the rule between ^ and $ anchors, as the rules can't
-        # include them by default.
-        wrapped = Sequence(Start(), rule, End())
-        _compiled_rule_cache[rule_name] = wrapped.compile()
-    return _compiled_rule_cache[rule_name]
+    if rule_name not in _rfc_names:
+        raise ValueError("Unknown rule name: {0}".format(rule_name))
+    rule = _rfc_names[rule_name]
+    # Need to place the rule between ^ and $ anchors, as the rules can't
+    # include them by default.
+    wrapped = Sequence(Start(), rule, End())
+    return wrapped.compile()
 
 
-__all__ = ["get_regex"] + ([n for (n, v) in locals().items()
-                            if not n.startswith("_") and isinstance(v, Regex)])
+__all__ = ["get_regex"] + (
+    [n for (n, v) in locals().items() if not n.startswith("_") and isinstance(v, Regex)]
+)
```

### Comparing `rnginline-0.0.2/rnginline/urlhandlers.py` & `rnginline-1.0.0rc1/rnginline/urlhandlers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,126 +1,80 @@
-# -*- coding: utf-8 -*-
 """
 This module contains the built-in URL Handlers provided by ``rnginline``.
 
 URL Handler objects are responsible for:
 
 * Saying if they can handle a URL — ``can_handle(url)``
 * Fetching the data referenced by a URL — ``dereference(url)``
 """
 
-from __future__ import unicode_literals
+from __future__ import annotations
 
+import os
 import pkgutil
 import re
+from typing import Sequence
+from urllib import parse
+from urllib.parse import SplitResult, quote, unquote
+from urllib.request import pathname2url, url2pathname
 
-import six
-from six.moves.urllib import parse
-from six.moves.urllib.request import pathname2url, url2pathname
+from typing_extensions import Final, Protocol
 
-from rnginline.exceptions import DereferenceError
 from rnginline import uri
-
+from rnginline.exceptions import DereferenceError
 
 __all__ = ["file", "pydata"]
 
 # Python package pattern
 PACKAGE = re.compile(r"^[a-zA-Z_][a-zA-Z0-9_]+(\.[a-zA-Z_][a-zA-Z0-9_]+)*$")
 
 
-def reject_bytes(**kwargs):
-    """
-    Raise a ValueError if any of the kwarg values are six.binary_type.
-    """
-    for name, value in kwargs.items():
-        if isinstance(value, six.binary_type):
-            raise ValueError(
-                "Use {0} for {1}, not {2}. got: {3!r}"
-                .format(six.text_type.__name__, name, six.binary_type.__name__,
-                        value))
-
-
-def ensure_parsed(uri):
-    reject_bytes(uri=uri)
-    if isinstance(uri, six.text_type):
+def ensure_parsed(uri: str | SplitResult) -> SplitResult:
+    if isinstance(uri, str):
         return parse.urlsplit(uri)
     assert len(uri) == 5
     return uri
 
 
-def quote(text, quoting_func=parse.quote):
-    """
-    Pass a text string through quoting_func, following the conventions of the
-    Python version.
-
-    Args:
-        text: A text (not byte) string to be encoded by quoting_func.
-        quoting_func: The function to perform the URI-encoding. On PY2 this
-            func will receive and produce bytes, on PY3 it will receive and
-            produce text.
-    Returns: A text (not byte) string, encoded by quoting_func.
-    """
-    reject_bytes(text=text)
-
-    if six.PY3:
-        return quoting_func(text)
-
-    # Handle Python 2 weirdness
-    return quoting_func(text.encode("utf-8")).decode("ascii")
-
-
-def unquote(uri_encoded_text, unquoting_func=parse.unquote):
-    """
-    Pass a percent-encoded string through unquoting_func, following the
-    conventions of the Python version.
-
-    Args:
-        uri_encoded_text: A text (not byte) string, possibly containing
-            percent-encoded escapes.
-        unquoting_func: The function to escape the percent encoded escapes. On
-            PY2 this func will receive and produce bytes. On PY3 it will
-            receive and produce text.
-    Returns:
-        A text (not byte) string decoded by unquoting_func.
-    """
-    reject_bytes(uri_encoded_text=uri_encoded_text)
-
-    if six.PY3:
-        return unquoting_func(uri_encoded_text)
+def _validate_py_pkg_name(package: str) -> None:
+    if not PACKAGE.match(package):
+        raise ValueError(
+            "package is not a valid Python package name: {0}".format(package)
+        )
 
-    return unquoting_func(uri_encoded_text.encode("ascii")).decode("utf-8")
 
+class UrlHandler(Protocol):
+    def can_handle(self, url: str | SplitResult) -> bool:
+        ...
 
-def _validate_py_pkg_name(package):
-    if not PACKAGE.match(package):
-        raise ValueError("package is not a valid Python package name: {0}"
-                         .format(package))
+    def dereference(self, url: str | SplitResult) -> bytes:
+        ...
 
 
-class FilesystemUrlHandler(object):
+class FilesystemUrlHandler(UrlHandler):
     """
     A ``UrlHandler`` for ``file:`` URLs. This handler can resolve references to
     files on the local filesystem.
     """
 
-    def can_handle(self, url):
+    def can_handle(self, url: str | SplitResult) -> bool:
         """
         Check if this handler supports ``url``.
 
         This handler supports URLs with the ``file:`` scheme.
 
         Args:
             url: A URL as a string.
 
         Returns:
             bool: True if ``url`` is supported by this handler, False otherwise
         """
         return ensure_parsed(url).scheme == "file"
 
-    def dereference(self, url):
+    def dereference(self, url: str | SplitResult) -> bytes:
         """
         Read the contents of the file identified by ``url``.
 
         Args:
             url: A ``file:`` URL
 
         Returns:
@@ -141,21 +95,20 @@
         # characters, so needs decoding as UTF-8
         path = self.breakurl(url)
 
         try:
             with open(path, "rb") as f:
                 return f.read()
         except IOError as cause:
-            err = DereferenceError(
-                "Unable to dereference file url: {0} : {1}"
-                .format(uri.recombine(url), cause))
-            six.raise_from(err, cause)
+            raise DereferenceError(
+                f"Unable to dereference file url: {uri.recombine(url)} : {cause}"
+            ) from cause
 
     @staticmethod
-    def makeurl(file_path, abs=False):
+    def makeurl(file_path: str | os.PathLike[str], abs: bool = False) -> str:
         """
         Create relative or absolute URL pointing to the filesystem path
         ``file_path``.
 
         (Absolute refers to whether or not the URL has a scheme, not whether
         the path is absolute.)
 
@@ -175,23 +128,21 @@
             >>> file.makeurl('/tmp/foo', abs=True)
             'file:/tmp/foo'
             >>> file.makeurl('file.txt')
             'file.txt'
             >>> file.makeurl('file.txt', abs=True)
             'file:file.txt'
         """
-        reject_bytes(file_path=file_path)
-
-        path = quote(file_path, quoting_func=pathname2url)
+        path = pathname2url(os.fspath(file_path))
         if abs is True:
             return uri.resolve("file:", path)
         return path
 
     @staticmethod
-    def breakurl(file_url):
+    def breakurl(file_url: str | SplitResult) -> str:
         """
         Decode a ``file:`` URL into a filesystem path.
 
         Args:
             file_url: The URL to decode. Can be an absolute URL with a
                 ``file:`` scheme, or a relative URL without a scheme.
         Returns:
@@ -204,49 +155,50 @@
             >>> file.breakurl('some/path/file%20name.dat')
             'some/path/file name.dat'
         """
         url = ensure_parsed(file_url)
         scheme, _, path, _, _ = url
 
         if scheme not in ("file", ""):
-            raise ValueError("Expected a file: or scheme-less (relative) URL, "
-                             "got: {0}".format(uri.recombine(url)))
+            raise ValueError(
+                "Expected a file: or scheme-less (relative) URL, "
+                "got: {0}".format(uri.recombine(url))
+            )
 
-        return unquote(ensure_parsed(file_url).path,
-                       unquoting_func=url2pathname)
+        return url2pathname(path)
 
 
-class PackageDataUrlHandler(object):
+class PackageDataUrlHandler(UrlHandler):
     """
     A URL Handler which allows data files in Python packages to be referenced.
 
     The URLs handled by instances of this class are layed out as follows::
 
         pydata://<package-path>/<path-under-package>
 
     For example ``pydata://rnginline.test/data/loops/start.rng``.
     """
 
-    scheme = "pydata"
+    scheme: Final = "pydata"
 
-    def can_handle(self, url):
+    def can_handle(self, url: str | SplitResult) -> bool:
         """
         Check if this handler supports ``url``.
 
         This handler supports URLs with the ``pydata:`` scheme.
 
         Args:
             url: A URL as a string.
 
         Returns:
             bool: True if ``url`` is supported by this handler, False otherwise
         """
         return ensure_parsed(url).scheme == self.scheme
 
-    def dereference(self, url):
+    def dereference(self, url: str | SplitResult) -> bytes:
         """
         Get the contents of the data file identified by ``url``
 
         ``pkgutil.get_data()`` is used to fetch the data.
 
         Args:
             url: A ``pydata:`` URL pointing at a file under a Python package
@@ -259,49 +211,47 @@
         assert self.can_handle(url)
 
         package, pkg_path = self.breakurl(url)
 
         data = pkgutil.get_data(package, pkg_path)
 
         if data is None:
-            raise DereferenceError("Unable to dereference url: {0}"
-                                   .format(url))
+            raise DereferenceError("Unable to dereference url: {0}".format(url))
 
         return data
 
     @classmethod
-    def makeurl(cls, package, resource_path):
+    def makeurl(cls, package: str, resource_path: str) -> str:
         """
         Create a URL referencing data under a Python package.
 
         Args:
             package: A dotted path you'd use to import the package in question
             resource_path: The path under the package to a data file
         Returns:
             ...: A URL of the form ``pydata://<package>/<resource_path>``
 
         Example:
             >>> from rnginline.urlhandlers import pydata
             >>> pydata.makeurl('mypkg.subpkg', 'some/file.txt')
             'pydata://mypkg.subpkg/some/file.txt'
         """
-        # Python 2 uses bytes for __name__, so no point in rejecting non-text
-        reject_bytes(resource_path=resource_path)
         _validate_py_pkg_name(package)
 
         if resource_path.startswith("/"):
-            raise ValueError("resource_path must not start with a slash: {0}"
-                             .format(resource_path))
+            raise ValueError(
+                f"resource_path must not start with a slash: {resource_path}"
+            )
 
         path = quote("/" + resource_path)
 
         return uri.recombine((cls.scheme, package, path, None, None))
 
     @classmethod
-    def breakurl(cls, url):
+    def breakurl(cls, url: str | SplitResult) -> tuple[str, str]:
         """
         Deconstruct a ``pydata:`` URL into constituent parts.
 
         Args:
             url: A ``pydata:`` URL
         Returns:
             A 2-tuple of the package and path contained in the URL
@@ -311,33 +261,33 @@
             >>> pydata.breakurl('pydata://mypkg.subpkg/some/file.txt')
             ('mypkg.subpkg', 'some/file.txt')
         """
         url = ensure_parsed(url)
         scheme, package, path, _, _ = url
 
         if scheme != cls.scheme:
-            raise ValueError("Not a pydata: URL: {0}".format(url.geturl()))
+            raise ValueError(f"Not a pydata: URL: {url.geturl()}")
 
         package = unquote(package)
         path = unquote(path)
 
         _validate_py_pkg_name(package)
 
         return package, path[1:] if path else path
 
 
-file = FilesystemUrlHandler()
+file: Final[FilesystemUrlHandler] = FilesystemUrlHandler()
 """
 The default instance of :class:`FilesystemUrlHandler`
 """
 
-pydata = PackageDataUrlHandler()
+pydata: Final[PackageDataUrlHandler] = PackageDataUrlHandler()
 """
 The default instance of :class:`PackageDataUrlHandler`
 """
 
 
-def get_default_handlers():
+def get_default_handlers() -> Sequence[UrlHandler]:
     """
     Get a list of the default URL Handler objects.
     """
     return [file, pydata]
```

