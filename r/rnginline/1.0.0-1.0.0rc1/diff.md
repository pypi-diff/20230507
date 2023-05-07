# Comparing `tmp/rnginline-1.0.0.tar.gz` & `tmp/rnginline-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnginline-1.0.0.tar", max compression
+gzip compressed data, was "rnginline-1.0.0rc1.tar", max compression
```

## Comparing `rnginline-1.0.0.tar` & `rnginline-1.0.0rc1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0      579 2023-05-07 15:16:37.969438 rnginline-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     3579 2023-05-07 15:16:37.969438 rnginline-1.0.0/README.md
--rw-r--r--   0        0        0     2853 2023-05-07 15:16:37.969438 rnginline-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    41049 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/__init__.py
--rw-r--r--   0        0        0     5760 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/cmdline.py
--rw-r--r--   0        0        0      584 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/constants.py
--rw-r--r--   0        0        0     1705 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/exceptions.py
--rw-r--r--   0        0        0     2428 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/postprocess.py
--rw-r--r--   0        0        0        0 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/py.typed
--rw-r--r--   0        0        0    10316 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/regexbuilder.py
--rw-r--r--   0        0        0     9530 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/relaxng.rng
--rw-r--r--   0        0        0        0 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/__init__.py
--rw-r--r--   0        0        0      396 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/datatype-library-inheritance/base-external.rng
--rw-r--r--   0        0        0      287 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/datatype-library-inheritance/base-included.rng
--rw-r--r--   0        0        0      269 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/datatype-library-inheritance/external.rng
--rw-r--r--   0        0        0      349 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/datatype-library-inheritance/included.rng
--rw-r--r--   0        0        0      171 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/datatype-library-propagation/a.rng
--rw-r--r--   0        0        0      934 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/datatype-library-propagation/b.rng
--rw-r--r--   0        0        0       20 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/include-invalid-xml/invalid-xml.rng
--rw-r--r--   0        0        0      136 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/include-invalid-xml/ok.rng
--rw-r--r--   0        0        0       29 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/include-non-rng-xml/invalid-xml.rng
--rw-r--r--   0        0        0      136 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/include-non-rng-xml/ok.rng
--rw-r--r--   0        0        0      120 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/include-override-define/included.rng
--rw-r--r--   0        0        0      306 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/include-override-define/start.rng
--rw-r--r--   0        0        0      120 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/include-override-start/included.rng
--rw-r--r--   0        0        0      292 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/include-override-start/start.rng
--rw-r--r--   0        0        0       89 2023-05-07 15:16:37.969438 rnginline-1.0.0/rnginline/test/data/inline-non-grammar-els/foo-el.rng
--rw-r--r--   0        0        0      131 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/inline-non-grammar-els/grammar-foo-el.rng
--rw-r--r--   0        0        0      142 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/inline-non-grammar-els/illegal.rng
--rw-r--r--   0        0        0      144 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/inline-non-grammar-els/legal.rng
--rw-r--r--   0        0        0      118 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/loops/foo/a.rng
--rw-r--r--   0        0        0      141 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/loops/foo/bar/baz/b.rng
--rw-r--r--   0        0        0      114 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/loops/start.rng
--rw-r--r--   0        0        0      269 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/multiple-ref-1-fetch/a/b/c/popular.rng
--rw-r--r--   0        0        0       97 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/multiple-ref-1-fetch/indirect.rng
--rw-r--r--   0        0        0      534 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/multiple-ref-1-fetch/schema.rng
--rw-r--r--   0        0        0      284 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/datatype-library-external/external.rng
--rw-r--r--   0        0        0      294 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/datatype-library-external/included.rng
--rw-r--r--   0        0        0       81 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/datatype-library-external/positive.xml
--rw-r--r--   0        0        0      459 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/datatype-library-external/schema.rng
--rw-r--r--   0        0        0       98 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-1/README.rst
--rw-r--r--   0        0        0       21 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-1/baz.rnc
--rw-r--r--   0        0        0      127 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-1/baz.rng
--rw-r--r--   0        0        0       87 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-1/negative-1.xml
--rw-r--r--   0        0        0       87 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-1/negative-2.xml
--rw-r--r--   0        0        0       73 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-1/positive-1.xml
--rw-r--r--   0        0        0      117 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-1/positive-2.xml
--rw-r--r--   0        0        0      132 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-1/schema.rnc
--rw-r--r--   0        0        0      445 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-1/schema.rng
--rw-r--r--   0        0        0      303 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-2/README.rst
--rw-r--r--   0        0        0       42 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-2/negative-1.xml
--rw-r--r--   0        0        0       33 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-2/positive-1.xml
--rw-r--r--   0        0        0       33 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-2/positive-2.xml
--rw-r--r--   0        0        0      263 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-2/schema.rng
--rw-r--r--   0        0        0      211 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-2/that.rng
--rw-r--r--   0        0        0      157 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-2/this.rng
--rw-r--r--   0        0        0      351 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/1-default-xmlns-unprefixed-names.rng
--rw-r--r--   0        0        0      255 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/2-ns-attributes.rng
--rw-r--r--   0        0        0      308 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/3-qnames.rng
--rw-r--r--   0        0        0      682 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/README.rst
--rw-r--r--   0        0        0      128 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/negative-1.1.xml
--rw-r--r--   0        0        0      113 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/negative-1.2.xml
--rw-r--r--   0        0        0      129 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/negative-2.1.xml
--rw-r--r--   0        0        0      142 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/negative-2.2.xml
--rw-r--r--   0        0        0      186 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/negative-3.1.xml
--rw-r--r--   0        0        0      186 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/negative-3.2.xml
--rw-r--r--   0        0        0      151 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/negative-3.3.xml
--rw-r--r--   0        0        0      169 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/negative-3.4.xml
--rw-r--r--   0        0        0       77 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/positive-1.1.xml
--rw-r--r--   0        0        0      104 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/positive-2.1.xml
--rw-r--r--   0        0        0      133 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/positive-3.1.xml
--rw-r--r--   0        0        0      822 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/schema.rng
--rw-r--r--   0        0        0      352 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/tmp.rng
--rw-r--r--   0        0        0      256 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-ns-override/external.rng
--rw-r--r--   0        0        0       76 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-ns-override/negative-1.xml
--rw-r--r--   0        0        0       76 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-ns-override/positive-1.xml
--rw-r--r--   0        0        0      372 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/external-ref-ns-override/schema.rng
--rw-r--r--   0        0        0      235 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/foreign-attributes/lvl2.rng
--rw-r--r--   0        0        0       88 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/foreign-attributes/lvl3.rng
--rw-r--r--   0        0        0       30 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/foreign-attributes/positive-1.xml
--rw-r--r--   0        0        0      532 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/foreign-attributes/schema.rng
--rw-r--r--   0        0        0      330 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-1/included.rng
--rw-r--r--   0        0        0       37 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-1/negative-1.xml
--rw-r--r--   0        0        0       23 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-1/positive-1.xml
--rw-r--r--   0        0        0       23 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-1/positive-2.xml
--rw-r--r--   0        0        0      273 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-1/schema.rng
--rw-r--r--   0        0        0      403 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect/level-1-a.rng
--rw-r--r--   0        0        0      904 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect/level-2-a.rng
--rw-r--r--   0        0        0       40 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect/negative-1.xml
--rw-r--r--   0        0        0       35 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect/negative-2.xml
--rw-r--r--   0        0        0       22 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect/negative-3.xml
--rw-r--r--   0        0        0      223 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect/other.rng
--rw-r--r--   0        0        0       29 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect/positive-1.xml
--rw-r--r--   0        0        0       35 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect/positive-2.xml
--rw-r--r--   0        0        0      693 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect/schema.rng
--rw-r--r--   0        0        0      373 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/level-1-a.rng
--rw-r--r--   0        0        0      933 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/level-2-a.rng
--rw-r--r--   0        0        0      390 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/level-2-b.rng
--rw-r--r--   0        0        0       41 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/negative-1.xml
--rw-r--r--   0        0        0       47 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/negative-2.xml
--rw-r--r--   0        0        0       35 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/negative-3.xml
--rw-r--r--   0        0        0       33 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/negative-4.xml
--rw-r--r--   0        0        0       26 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/negative-5.xml
--rw-r--r--   0        0        0       26 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/negative-6.xml
--rw-r--r--   0        0        0      187 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/positive-1.xml
--rw-r--r--   0        0        0     1651 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/schema.rng
--rw-r--r--   0        0        0      892 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/overrides/included.rng
--rw-r--r--   0        0        0      743 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/overrides/positive.xml
--rw-r--r--   0        0        0     1647 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/overrides/schema.rng
--rw-r--r--   0        0        0       89 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/xml-base/a/b/baz.rng
--rw-r--r--   0        0        0      284 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/xml-base/a/b/c/d/foo.rng
--rw-r--r--   0        0        0       86 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/xml-base/positive-1.xml
--rw-r--r--   0        0        0      151 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/xml-base/schema.rng
--rw-r--r--   0        0        0      139 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/data/testcases/xml-base/x/y/z/bar.rng
--rw-r--r--   0        0        0      683 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/mini_validator.py
--rw-r--r--   0        0        0     8306 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/test_cmdline.py
--rw-r--r--   0        0        0     1831 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/test_propagate_datatypelibrary.py
--rw-r--r--   0        0        0     6784 2023-05-07 15:16:37.973439 rnginline-1.0.0/rnginline/test/test_regexbuilder.py
--rw-r--r--   0        0        0    19628 2023-05-07 15:16:37.977439 rnginline-1.0.0/rnginline/test/test_rnginline.py
--rw-r--r--   0        0        0     7992 2023-05-07 15:16:37.977439 rnginline-1.0.0/rnginline/test/test_uri.py
--rw-r--r--   0        0        0     8750 2023-05-07 15:16:37.977439 rnginline-1.0.0/rnginline/test/test_uri_regex.py
--rw-r--r--   0        0        0     4508 2023-05-07 15:16:37.977439 rnginline-1.0.0/rnginline/test/test_urlhandlers.py
--rw-r--r--   0        0        0     5348 2023-05-07 15:16:37.977439 rnginline-1.0.0/rnginline/uri.py
--rw-r--r--   0        0        0     7156 2023-05-07 15:16:37.977439 rnginline-1.0.0/rnginline/uri_regex.py
--rw-r--r--   0        0        0     8749 2023-05-07 15:16:37.977439 rnginline-1.0.0/rnginline/urlhandlers.py
--rw-r--r--   0        0        0     5025 1970-01-01 00:00:00.000000 rnginline-1.0.0/PKG-INFO
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

### Comparing `rnginline-1.0.0/LICENSE.txt` & `rnginline-1.0.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/README.md` & `rnginline-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/pyproject.toml` & `rnginline-1.0.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rnginline"
-version = "1.0.0"
+version = "1.0.0rc1"
 description = "Flatten multi-file RELAX NG schemas"
 readme = "README.md"
 authors = ["Hal Blackburn <hwtb2@cam.ac.uk>"]
 license = "Apache-2.0"
 repository = "https://github.com/h4l/rnginline"
 documentation = "https://rnginline.readthedocs.io/en/latest/"
 classifiers = [
```

### Comparing `rnginline-1.0.0/rnginline/__init__.py` & `rnginline-1.0.0rc1/rnginline/__init__.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/cmdline.py` & `rnginline-1.0.0rc1/rnginline/cmdline.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/constants.py` & `rnginline-1.0.0rc1/rnginline/constants.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/exceptions.py` & `rnginline-1.0.0rc1/rnginline/exceptions.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/postprocess.py` & `rnginline-1.0.0rc1/rnginline/postprocess.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/regexbuilder.py` & `rnginline-1.0.0rc1/rnginline/regexbuilder.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/relaxng.rng` & `rnginline-1.0.0rc1/rnginline/relaxng.rng`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/data/datatype-library-propagation/b.rng` & `rnginline-1.0.0rc1/rnginline/test/data/datatype-library-propagation/b.rng`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/data/multiple-ref-1-fetch/schema.rng` & `rnginline-1.0.0rc1/rnginline/test/data/multiple-ref-1-fetch/schema.rng`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/README.rst` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/README.rst`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/data/testcases/external-ref-3-namespaces/schema.rng` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/external-ref-3-namespaces/schema.rng`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/data/testcases/foreign-attributes/schema.rng` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/foreign-attributes/schema.rng`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect/level-2-a.rng` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect/level-2-a.rng`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect/schema.rng` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect/schema.rng`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/level-2-a.rng` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/level-2-a.rng`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/data/testcases/include-override-indirect-combined/schema.rng` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/include-override-indirect-combined/schema.rng`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/data/testcases/overrides/included.rng` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/overrides/included.rng`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/data/testcases/overrides/positive.xml` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/overrides/positive.xml`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/data/testcases/overrides/schema.rng` & `rnginline-1.0.0rc1/rnginline/test/data/testcases/overrides/schema.rng`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/mini_validator.py` & `rnginline-1.0.0rc1/rnginline/test/mini_validator.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/test_cmdline.py` & `rnginline-1.0.0rc1/rnginline/test/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/test_propagate_datatypelibrary.py` & `rnginline-1.0.0rc1/rnginline/test/test_propagate_datatypelibrary.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/test_regexbuilder.py` & `rnginline-1.0.0rc1/rnginline/test/test_regexbuilder.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/test_rnginline.py` & `rnginline-1.0.0rc1/rnginline/test/test_rnginline.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/test_uri.py` & `rnginline-1.0.0rc1/rnginline/test/test_uri.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/test_uri_regex.py` & `rnginline-1.0.0rc1/rnginline/test/test_uri_regex.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/test/test_urlhandlers.py` & `rnginline-1.0.0rc1/rnginline/test/test_urlhandlers.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/uri.py` & `rnginline-1.0.0rc1/rnginline/uri.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/uri_regex.py` & `rnginline-1.0.0rc1/rnginline/uri_regex.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/rnginline/urlhandlers.py` & `rnginline-1.0.0rc1/rnginline/urlhandlers.py`

 * *Files identical despite different names*

### Comparing `rnginline-1.0.0/PKG-INFO` & `rnginline-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnginline
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Flatten multi-file RELAX NG schemas
 Home-page: https://github.com/h4l/rnginline
 License: Apache-2.0
 Keywords: relaxng,inline,lxml,xml
 Author: Hal Blackburn
 Author-email: hwtb2@cam.ac.uk
 Requires-Python: >=3.7,<4.0
```

