# Comparing `tmp/mkdocstrings-python-0.8.3.tar.gz` & `tmp/mkdocstrings-python-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocstrings-python-0.8.3.tar", last modified: Wed Jan  4 21:33:55 2023, max compression
+gzip compressed data, was "mkdocstrings-python-0.9.0.tar", last modified: Mon Apr  3 14:20:24 2023, max compression
```

## Comparing `mkdocstrings-python-0.8.3.tar` & `mkdocstrings-python-0.9.0.tar`

### file list

```diff
@@ -1,64 +1,71 @@
--rw-r--r--   0 pawamoy   (1000) users      (984)      754 2022-12-05 15:56:07.219720 mkdocstrings-python-0.8.3/LICENSE
--rw-r--r--   0 pawamoy   (1000) users      (984)     3760 2022-12-05 15:56:07.219720 mkdocstrings-python-0.8.3/README.md
--rw-r--r--   0 pawamoy   (1000) users      (984)     3088 2022-12-05 15:56:07.219720 mkdocstrings-python-0.8.3/pyproject.toml
--rw-r--r--   0 pawamoy   (1000) users      (984)        0 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/py.typed
--rw-r--r--   0 pawamoy   (1000) users      (984)      342 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (984)    13997 2023-01-04 21:21:36.001261 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/handler.py
--rw-r--r--   0 pawamoy   (1000) users      (984)     6219 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/rendering.py
--rw-r--r--   0 pawamoy   (1000) users      (984)     2532 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     4853 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/children.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     4186 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/class.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      269 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     2465 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      400 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     2475 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     3134 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     2132 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     3111 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     3081 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     2115 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     3051 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     1353 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      590 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     2532 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/function.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      245 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     1852 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/module.html
--rw-r--r--   0 pawamoy   (1000) users      (984)     2055 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       37 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/attribute.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       36 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/children.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       33 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/class.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       48 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       48 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       46 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       54 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       48 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       44 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       46 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       45 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       43 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       44 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       37 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/docstring.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       38 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/expression.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       36 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/function.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       34 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/labels.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       34 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/module.html
--rw-r--r--   0 pawamoy   (1000) users      (984)       37 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/signature.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      703 2022-12-05 15:56:07.223053 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/style.css
--rw-r--r--   0 pawamoy   (1000) users      (984)      224 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/mkdocs/exceptions.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      277 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/mkdocs/keyword_args.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      293 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/mkdocs/parameters.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      200 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/mkdocs/return.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      137 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/mkdocs/style.css
--rw-r--r--   0 pawamoy   (1000) users      (984)      196 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/mkdocs/yield.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      545 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      601 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      618 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      494 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/readthedocs/returns.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      600 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
--rw-r--r--   0 pawamoy   (1000) users      (984)      490 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/readthedocs/yields.html
--rw-r--r--   0 pawamoy   (1000) users      (984)      174 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/tests/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (984)     2619 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/tests/conftest.py
--rw-r--r--   0 pawamoy   (1000) users      (984)     3063 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/tests/test_handler.py
--rw-r--r--   0 pawamoy   (1000) users      (984)     1377 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/tests/test_rendering.py
--rw-r--r--   0 pawamoy   (1000) users      (984)     1111 2022-12-05 15:56:07.226387 mkdocstrings-python-0.8.3/tests/test_themes.py
--rw-------   0 pawamoy   (1000) users      (984)     5205 2023-01-04 21:33:55.561232 mkdocstrings-python-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-04-01 14:36:13.301342 mkdocstrings-python-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3758 2023-04-01 14:36:13.404674 mkdocstrings-python-0.9.0/README.md
+-rw-r--r--   0        0        0     2318 2023-04-01 14:36:13.404674 mkdocstrings-python-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-01 14:36:13.198010 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/py.typed
+-rw-r--r--   0        0        0      326 2023-04-01 14:36:34.291024 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/__init__.py
+-rw-r--r--   0        0        0    17401 2023-04-03 14:17:32.034907 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/handler.py
+-rw-r--r--   0        0        0     6336 2023-04-01 15:17:37.426937 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/rendering.py
+-rw-r--r--   0        0        0     2532 2022-04-29 13:33:38.953329 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
+-rw-r--r--   0        0        0     5053 2023-04-01 15:33:24.336417 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html
+-rw-r--r--   0        0        0     4186 2022-04-29 17:28:38.933216 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html
+-rw-r--r--   0        0        0      269 2022-02-13 13:38:05.822420 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
+-rw-r--r--   0        0        0     2465 2022-04-29 23:09:02.903315 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
+-rw-r--r--   0        0        0      400 2022-03-01 18:29:05.585970 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
+-rw-r--r--   0        0        0     2475 2022-04-29 23:09:07.859915 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
+-rw-r--r--   0        0        0     3134 2022-04-29 23:09:10.543213 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
+-rw-r--r--   0        0        0     2132 2022-04-29 23:09:12.233190 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
+-rw-r--r--   0        0        0     3111 2022-04-29 23:09:14.279830 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
+-rw-r--r--   0        0        0     3081 2022-04-29 23:09:16.163138 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
+-rw-r--r--   0        0        0     2115 2022-04-29 23:09:18.059779 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
+-rw-r--r--   0        0        0     3051 2022-04-29 23:09:20.759743 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
+-rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
+-rw-r--r--   0        0        0      590 2022-04-29 22:21:21.405388 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
+-rw-r--r--   0        0        0     2532 2022-04-29 17:28:35.633273 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html
+-rw-r--r--   0        0        0      245 2022-05-08 08:40:49.298304 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
+-rw-r--r--   0        0        0     1852 2022-04-29 17:36:56.831573 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html
+-rw-r--r--   0        0        0     2055 2022-11-13 16:53:10.704878 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/attribute.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/children.html
+-rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/class.html
+-rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
+-rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
+-rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
+-rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
+-rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
+-rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
+-rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
+-rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/docstring.html
+-rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/expression.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/function.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/labels.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/module.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/signature.html
+-rw-r--r--   0        0        0      703 2022-03-03 18:21:59.514950 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/style.css
+-rw-r--r--   0        0        0      224 2021-10-30 13:54:10.019274 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/mkdocs/exceptions.html
+-rw-r--r--   0        0        0      277 2021-10-30 13:54:10.202605 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/mkdocs/keyword_args.html
+-rw-r--r--   0        0        0      293 2021-10-30 13:54:10.019274 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/mkdocs/parameters.html
+-rw-r--r--   0        0        0      200 2021-10-30 13:54:10.092606 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/mkdocs/return.html
+-rw-r--r--   0        0        0      137 2021-10-30 13:54:10.199272 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/mkdocs/style.css
+-rw-r--r--   0        0        0      196 2021-10-30 13:54:10.202605 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/mkdocs/yield.html
+-rw-r--r--   0        0        0      545 2021-10-30 13:54:09.842609 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html
+-rw-r--r--   0        0        0      601 2021-11-06 17:58:09.459000 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html
+-rw-r--r--   0        0        0      618 2021-11-06 17:59:12.206399 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html
+-rw-r--r--   0        0        0      494 2021-11-06 17:58:14.115000 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/returns.html
+-rw-r--r--   0        0        0      600 2021-10-30 13:54:09.942608 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
+-rw-r--r--   0        0        0      490 2021-11-06 17:58:20.568000 mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/yields.html
+-rw-r--r--   0        0        0       37 2022-02-07 16:51:30.472324 mkdocstrings-python-0.9.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2022-02-07 16:51:30.472324 mkdocstrings-python-0.9.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      295 2022-02-07 16:51:30.472324 mkdocstrings-python-0.9.0/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      689 2022-02-08 11:16:01.880696 mkdocstrings-python-0.9.0/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2022-02-08 11:16:01.880696 mkdocstrings-python-0.9.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-02-08 11:16:01.880696 mkdocstrings-python-0.9.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        9 2022-02-08 11:16:01.397369 mkdocstrings-python-0.9.0/tests/.pytest_cache/v/randomly_seed
+-rw-r--r--   0        0        0      174 2023-04-01 14:36:13.194677 mkdocstrings-python-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     3042 2023-04-01 15:31:03.805108 mkdocstrings-python-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     3222 2023-04-01 15:27:04.848491 mkdocstrings-python-0.9.0/tests/test_handler.py
+-rw-r--r--   0        0        0     1515 2023-04-01 15:25:49.732868 mkdocstrings-python-0.9.0/tests/test_rendering.py
+-rw-r--r--   0        0        0     1332 2023-04-01 15:22:56.275453 mkdocstrings-python-0.9.0/tests/test_themes.py
+-rw-r--r--   0        0        0     5203 1970-01-01 00:00:00.000000 mkdocstrings-python-0.9.0/PKG-INFO
```

### Comparing `mkdocstrings-python-0.8.3/LICENSE` & `mkdocstrings-python-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/README.md` & `mkdocstrings-python-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # adapt to your dependencies manager
 [project]
 dependencies = [
     "mkdocstrings[python]>=0.18",
 ]
 ```
 
-You can also explicitely depend on the handler:
+You can also explicitly depend on the handler:
 
 ```toml title="pyproject.toml"
 # PEP 621 dependencies declaration
 # adapt to your dependencies manager
 [project]
 dependencies = [
     "mkdocstrings-python",
@@ -55,31 +55,31 @@
 
 ## Features
 
 - **Data collection from source code**: collection of the object-tree and the docstrings is done thanks to
   [Griffe](https://github.com/mkdocstrings/griffe).
 
 - **Support for type annotations:** Griffe collects your type annotations and *mkdocstrings* uses them
-  to display parameters types or return types. It is even able to automatically add cross-references
-  to other objects from your API, from the standard library or from third-party libraries!
+  to display parameter types or return types. It is even able to automatically add cross-references
+  to other objects from your API, from the standard library or third-party libraries!
   See [how to load inventories](https://mkdocstrings.github.io/usage/#cross-references-to-other-projects-inventories) to enable it.
 
-- **Recursive documentation of Python objects:** just use the module dotted-path as identifier, and you get the full
+- **Recursive documentation of Python objects:** just use the module dotted-path as an identifier, and you get the full
   module docs. You don't need to inject documentation for each class, function, etc.
 
 - **Support for documented attributes:** attributes (variables) followed by a docstring (triple-quoted string) will
   be recognized by Griffe in modules, classes and even in `__init__` methods.
 
 - **Multiple docstring-styles support:** common support for Google-style, Numpydoc-style,
   and Sphinx-style docstrings. See [Griffe's documentation](https://mkdocstrings.github.io/griffe/docstrings/) on docstrings support.
 
 - **Admonition support in Google docstrings:** blocks like `Note:` or `Warning:` will be transformed
   to their [admonition](https://squidfunk.github.io/mkdocs-material/reference/admonitions/) equivalent.
   *We do not support nested admonitions in docstrings!*
 
 - **Every object has a TOC entry:** we render a heading for each object, meaning *MkDocs* picks them into the Table
-  of Contents, which is nicely display by the Material theme. Thanks to *mkdocstrings* cross-reference ability,
+  of Contents, which is nicely displayed by the Material theme. Thanks to *mkdocstrings* cross-reference ability,
   you can reference other objects within your docstrings, with the classic Markdown syntax:
   `[this object][package.module.object]` or directly with `[package.module.object][]`
 
 - **Source code display:** *mkdocstrings* can add a collapsible div containing the highlighted source code
   of the Python object.
```

#### html2text {}

```diff
@@ -2,38 +2,38 @@
                       A Python handler for mkdocstrings.
              [ci] [documentation] [pypi_version] [gitpod] [gitter]
 ---
                                   [logo.png]
 ## Installation You can install this handler as a *mkdocstrings* extra: ```toml
 title="pyproject.toml" # PEP 621 dependencies declaration # adapt to your
 dependencies manager [project] dependencies = [ "mkdocstrings[python]>=0.18", ]
-``` You can also explicitely depend on the handler: ```toml
+``` You can also explicitly depend on the handler: ```toml
 title="pyproject.toml" # PEP 621 dependencies declaration # adapt to your
 dependencies manager [project] dependencies = [ "mkdocstrings-python", ] ``` ##
 Preview  ![mkdocstrings_python_gif](https://user-images.githubusercontent.com/
 3999221/77157838-7184db80-6aa2-11ea-9f9a-fe77405202de.gif) ## Features - **Data
 collection from source code**: collection of the object-tree and the docstrings
 is done thanks to [Griffe](https://github.com/mkdocstrings/griffe). - **Support
 for type annotations:** Griffe collects your type annotations and
-*mkdocstrings* uses them to display parameters types or return types. It is
-even able to automatically add cross-references to other objects from your API,
-from the standard library or from third-party libraries! See [how to load
-inventories](https://mkdocstrings.github.io/usage/#cross-references-to-other-
-projects-inventories) to enable it. - **Recursive documentation of Python
-objects:** just use the module dotted-path as identifier, and you get the full
-module docs. You don't need to inject documentation for each class, function,
-etc. - **Support for documented attributes:** attributes (variables) followed
-by a docstring (triple-quoted string) will be recognized by Griffe in modules,
+*mkdocstrings* uses them to display parameter types or return types. It is even
+able to automatically add cross-references to other objects from your API, from
+the standard library or third-party libraries! See [how to load inventories]
+(https://mkdocstrings.github.io/usage/#cross-references-to-other-projects-
+inventories) to enable it. - **Recursive documentation of Python objects:**
+just use the module dotted-path as an identifier, and you get the full module
+docs. You don't need to inject documentation for each class, function, etc. -
+**Support for documented attributes:** attributes (variables) followed by a
+docstring (triple-quoted string) will be recognized by Griffe in modules,
 classes and even in `__init__` methods. - **Multiple docstring-styles support:
 ** common support for Google-style, Numpydoc-style, and Sphinx-style
 docstrings. See [Griffe's documentation](https://mkdocstrings.github.io/griffe/
 docstrings/) on docstrings support. - **Admonition support in Google
 docstrings:** blocks like `Note:` or `Warning:` will be transformed to their
 [admonition](https://squidfunk.github.io/mkdocs-material/reference/admonitions/
 ) equivalent. *We do not support nested admonitions in docstrings!* - **Every
 object has a TOC entry:** we render a heading for each object, meaning *MkDocs*
-picks them into the Table of Contents, which is nicely display by the Material
-theme. Thanks to *mkdocstrings* cross-reference ability, you can reference
-other objects within your docstrings, with the classic Markdown syntax: `[this
-object][package.module.object]` or directly with `[package.module.object][]` -
-**Source code display:** *mkdocstrings* can add a collapsible div containing
-the highlighted source code of the Python object.
+picks them into the Table of Contents, which is nicely displayed by the
+Material theme. Thanks to *mkdocstrings* cross-reference ability, you can
+reference other objects within your docstrings, with the classic Markdown
+syntax: `[this object][package.module.object]` or directly with `
+[package.module.object][]` - **Source code display:** *mkdocstrings* can add a
+collapsible div containing the highlighted source code of the Python object.
```

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/handler.py` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 """This module implements a handler for the Python language."""
 
 from __future__ import annotations
 
+import copy
 import glob
 import os
 import posixpath
 import re
 import sys
 from collections import ChainMap
 from contextlib import suppress
-from typing import Any, BinaryIO, Iterator, Optional, Tuple
+from typing import TYPE_CHECKING, Any, BinaryIO, Iterator, Mapping
 
-from griffe.agents.extensions import load_extensions
 from griffe.collections import LinesCollection, ModulesCollection
 from griffe.docstrings.parsers import Parser
 from griffe.exceptions import AliasResolutionError
 from griffe.loader import GriffeLoader
 from griffe.logger import patch_loggers
-from markdown import Markdown
 from mkdocstrings.extension import PluginError
 from mkdocstrings.handlers.base import BaseHandler, CollectionError, CollectorItem
 from mkdocstrings.inventory import Inventory
 from mkdocstrings.loggers import get_logger
 
 from mkdocstrings_handlers.python import rendering
 
+try:
+    from griffe.extensions import load_extensions
+except ImportError:
+    # TODO: remove once support for Griffe 0.25 is dropped
+    from griffe.agents.extensions import load_extensions  # type: ignore[no-redef]
+
+if TYPE_CHECKING:
+    from markdown import Markdown
+
+
 if sys.version_info >= (3, 11):
     from contextlib import chdir
 else:
     # TODO: remove once support for Python 3.10 is dropped
     from contextlib import contextmanager
 
-    @contextmanager  # noqa: WPS440
-    def chdir(path: str):  # noqa: D103,WPS440
+    @contextmanager
+    def chdir(path: str) -> Iterator[None]:  # noqa: D103
         old_wd = os.getcwd()
         os.chdir(path)
         try:
             yield
         finally:
             os.chdir(old_wd)
 
@@ -74,24 +83,36 @@
         "show_category_heading": False,
         "show_if_no_docstring": False,
         "show_signature": True,
         "show_signature_annotations": False,
         "separate_signature": False,
         "line_length": 60,
         "merge_init_into_class": False,
+        "show_docstring_attributes": True,
+        "show_docstring_description": True,
+        "show_docstring_examples": True,
+        "show_docstring_other_parameters": True,
+        "show_docstring_parameters": True,
+        "show_docstring_raises": True,
+        "show_docstring_receives": True,
+        "show_docstring_returns": True,
+        "show_docstring_warns": True,
+        "show_docstring_yields": True,
         "show_source": True,
         "show_bases": True,
         "show_submodules": False,
         "group_by_category": True,
         "heading_level": 2,
         "members_order": rendering.Order.alphabetical.value,
         "docstring_section_style": "table",
         "members": None,
         "filters": ["!^_[^_]"],
         "annotations_path": "brief",
+        "preload_modules": None,
+        "load_external_modules": False,
     }
     """
     Attributes: Headings options:
         heading_level (int): The initial heading level to use. Default: `2`.
         show_root_heading (bool): Show the heading of the object at the root of the documentation tree
             (i.e. the object referenced by the identifier after `:::`). Default: `False`.
         show_root_toc_entry (bool): If the root heading is not shown, at least add a ToC entry for it. Default: `True`.
@@ -114,29 +135,53 @@
     Attributes: Docstrings options:
         docstring_style (str): The docstring style to use: `google`, `numpy`, `sphinx`, or `None`. Default: `"google"`.
         docstring_options (dict): The options for the docstring parser. See parsers under [`griffe.docstrings`][].
         docstring_section_style (str): The style used to render docstring sections. Options: `table`, `list`, `spacy`. Default: `"table"`.
         line_length (int): Maximum line length when formatting code/signatures. Default: `60`.
         merge_init_into_class (bool): Whether to merge the `__init__` method into the class' signature and docstring. Default: `False`.
         show_if_no_docstring (bool): Show the object heading even if it has no docstring or children with docstrings. Default: `False`.
+        show_docstring_attributes (bool): Whether to display the "Attributes" section in the object's docstring. Default: `True`.
+        show_docstring_description (bool): Whether to display the textual block (including admonitions) in the object's docstring. Default: `True`.
+        show_docstring_examples (bool): Whether to display the "Examples" section in the object's docstring. Default: `True`.
+        show_docstring_other_parameters (bool): Whether to display the "Other Parameters" section in the object's docstring. Default: `True`.
+        show_docstring_parameters (bool): Whether to display the "Parameters" section in the object's docstring. Default: `True`.
+        show_docstring_raises (bool): Whether to display the "Raises" section in the object's docstring. Default: `True`.
+        show_docstring_receives (bool): Whether to display the "Receives" section in the object's docstring. Default: `True`.
+        show_docstring_returns (bool): Whether to display the "Returns" section in the object's docstring. Default: `True`.
+        show_docstring_warns (bool): Whether to display the "Warns" section in the object's docstring. Default: `True`.
+        show_docstring_yields (bool): Whether to display the "Yields" section in the object's docstring. Default: `True`.
 
     Attributes: Signatures/annotations options:
         annotations_path (str): The verbosity for annotations path: `brief` (recommended), or `source` (as written in the source). Default: `"brief"`.
         show_signature (bool): Show methods and functions signatures. Default: `True`.
         show_signature_annotations (bool): Show the type annotations in methods and functions signatures. Default: `False`.
         separate_signature (bool): Whether to put the whole signature in a code block below the heading.
             If Black is installed, the signature is also formatted using it. Default: `False`.
 
     Attributes: Additional options:
         show_bases (bool): Show the base classes of a class. Default: `True`.
         show_source (bool): Show the source code of this object. Default: `True`.
-    """  # noqa: E501
+        preload_modules (list[str] | None): Pre-load modules that are
+            not specified directly in autodoc instructions (`::: identifier`).
+            It is useful when you want to render documentation for a particular member of an object,
+            and this member is imported from another package than its parent.
+
+            For an imported member to be rendered, you need to add it to the `__all__` attribute
+            of the importing module.
+
+            The modules must be listed as an array of strings. Default: `None`.
+
+    """
 
     def __init__(
-        self, *args: Any, config_file_path: str | None = None, paths: list[str] | None = None, **kwargs: Any
+        self,
+        *args: Any,
+        config_file_path: str | None = None,
+        paths: list[str] | None = None,
+        **kwargs: Any,
     ) -> None:
         """Initialize the handler.
 
         Parameters:
             *args: Handler name, theme and custom templates.
             config_file_path: The MkDocs configuration file path.
             paths: A list of paths to use as Griffe search paths.
@@ -149,107 +194,122 @@
         with chdir(glob_base_dir):
             resolved_globs = [glob.glob(path) for path in paths]
         paths = [path for glob_list in resolved_globs for path in glob_list]
         if not paths and config_file_path:
             paths.append(os.path.dirname(config_file_path))
         search_paths = [path for path in sys.path if path]  # eliminate empty path
         for path in reversed(paths):
-            if not os.path.isabs(path):
-                if config_file_path:
-                    path = os.path.abspath(os.path.join(os.path.dirname(config_file_path), path))
+            if not os.path.isabs(path) and config_file_path:
+                path = os.path.abspath(os.path.join(os.path.dirname(config_file_path), path))  # noqa: PLW2901
             if path not in search_paths:
                 search_paths.insert(0, path)
         self._paths = search_paths
         self._modules_collection: ModulesCollection = ModulesCollection()
         self._lines_collection: LinesCollection = LinesCollection()
 
     @classmethod
     def load_inventory(
         cls,
         in_file: BinaryIO,
         url: str,
-        base_url: Optional[str] = None,
-        **kwargs: Any,
-    ) -> Iterator[Tuple[str, str]]:
+        base_url: str | None = None,
+        domains: list[str] | None = None,
+        **kwargs: Any,  # noqa: ARG003
+    ) -> Iterator[tuple[str, str]]:
         """Yield items and their URLs from an inventory file streamed from `in_file`.
 
         This implements mkdocstrings' `load_inventory` "protocol" (see [`mkdocstrings.plugin`][mkdocstrings.plugin]).
 
         Arguments:
             in_file: The binary file-like object to read the inventory from.
             url: The URL that this file is being streamed from (used to guess `base_url`).
             base_url: The URL that this inventory's sub-paths are relative to.
+            domains: A list of domain strings to filter the inventory by, when not passed, "py" will be used.
             **kwargs: Ignore additional arguments passed from the config.
 
         Yields:
             Tuples of (item identifier, item URL).
         """
+        domains = domains or ["py"]
         if base_url is None:
             base_url = posixpath.dirname(url)
 
-        for item in Inventory.parse_sphinx(in_file, domain_filter=("py",)).values():  # noqa: WPS526
+        for item in Inventory.parse_sphinx(in_file, domain_filter=domains).values():
             yield item.name, posixpath.join(base_url, item.uri)
 
-    def collect(self, identifier: str, config: dict) -> CollectorItem:  # noqa: D102,WPS231
+    def collect(self, identifier: str, config: Mapping[str, Any]) -> CollectorItem:  # noqa: D102
         module_name = identifier.split(".", 1)[0]
         unknown_module = module_name not in self._modules_collection
         if config.get("fallback", False) and unknown_module:
             raise CollectionError("Not loading additional modules during fallback")
 
-        final_config = ChainMap(config, self.default_config)
+        # See: https://github.com/python/typeshed/issues/8430
+        mutable_config = dict(copy.deepcopy(config))
+        final_config = ChainMap(mutable_config, self.default_config)
         parser_name = final_config["docstring_style"]
         parser_options = final_config["docstring_options"]
         parser = parser_name and Parser(parser_name)
 
         if unknown_module:
             loader = GriffeLoader(
                 extensions=load_extensions(final_config.get("extensions", [])),
                 search_paths=self._paths,
                 docstring_parser=parser,
                 docstring_options=parser_options,
                 modules_collection=self._modules_collection,
                 lines_collection=self._lines_collection,
             )
             try:
+                for pre_loaded_module in final_config.get("preload_modules") or []:
+                    if pre_loaded_module not in self._modules_collection:
+                        loader.load_module(pre_loaded_module)
                 loader.load_module(module_name)
             except ImportError as error:
                 raise CollectionError(str(error)) from error
-
-            unresolved, iterations = loader.resolve_aliases(implicit=False, external=False)
+            unresolved, iterations = loader.resolve_aliases(
+                implicit=False,
+                external=final_config["load_external_modules"],
+            )
             if unresolved:
                 logger.debug(f"{len(unresolved)} aliases were still unresolved after {iterations} iterations")
                 logger.debug(f"Unresolved aliases: {', '.join(sorted(unresolved))}")
 
         try:
             doc_object = self._modules_collection[identifier]
-        except KeyError as error:  # noqa: WPS440
+        except KeyError as error:
             raise CollectionError(f"{identifier} could not be found") from error
+        except AliasResolutionError as error:
+            raise CollectionError(str(error)) from error
 
         if not unknown_module:
             with suppress(AliasResolutionError):
                 if doc_object.docstring is not None:
                     doc_object.docstring.parser = parser
                     doc_object.docstring.parser_options = parser_options
 
         return doc_object
 
-    def render(self, data: CollectorItem, config: dict) -> str:  # noqa: D102 (ignore missing docstring)
-        final_config = ChainMap(config, self.default_config)
+    def render(self, data: CollectorItem, config: Mapping[str, Any]) -> str:  # noqa: D102 (ignore missing docstring)
+        # See https://github.com/python/typeshed/issues/8430
+        mutabled_config = dict(copy.deepcopy(config))
+        final_config = ChainMap(mutabled_config, self.default_config)
 
         template = self.env.get_template(f"{data.kind.value}.html")
 
         # Heading level is a "state" variable, that will change at each step
         # of the rendering recursion. Therefore, it's easier to use it as a plain value
         # than as an item in a dictionary.
         heading_level = final_config["heading_level"]
         try:
             final_config["members_order"] = rendering.Order(final_config["members_order"])
-        except ValueError:
+        except ValueError as error:
             choices = "', '".join(item.value for item in rendering.Order)
-            raise PluginError(f"Unknown members_order '{final_config['members_order']}', choose between '{choices}'.")
+            raise PluginError(
+                f"Unknown members_order '{final_config['members_order']}', choose between '{choices}'.",
+            ) from error
 
         if final_config["filters"]:
             final_config["filters"] = [
                 (re.compile(filtr.lstrip("!")), filtr.startswith("!")) for filtr in final_config["filters"]
             ]
 
         return template.render(
@@ -272,19 +332,19 @@
         try:
             return list({data.path, data.canonical_path, *data.aliases})
         except AliasResolutionError:
             return [data.path]
 
 
 def get_handler(
-    theme: str,  # noqa: W0613 (unused argument config)
-    custom_templates: Optional[str] = None,
+    theme: str,
+    custom_templates: str | None = None,
     config_file_path: str | None = None,
     paths: list[str] | None = None,
-    **config: Any,
+    **config: Any,  # noqa: ARG001
 ) -> PythonHandler:
     """Simply return an instance of `PythonHandler`.
 
     Arguments:
         theme: The theme to use when rendering contents.
         custom_templates: Directory containing custom templates.
         config_file_path: The MkDocs configuration file path.
```

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/rendering.py` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/rendering.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 
 from __future__ import annotations
 
 import enum
 import re
 import sys
 from functools import lru_cache
-from typing import Any, Pattern, Sequence
+from typing import TYPE_CHECKING, Any, Callable, Match, Pattern, Sequence
 
-from griffe.dataclasses import Alias, Object
 from markupsafe import Markup
-from mkdocstrings.handlers.base import CollectorItem
 from mkdocstrings.loggers import get_logger
 
+if TYPE_CHECKING:
+    from griffe.dataclasses import Alias, Object
+    from mkdocstrings.handlers.base import CollectorItem
+
 logger = get_logger(__name__)
 
 
 class Order(enum.Enum):
     """Enumeration for the possible members ordering."""
 
     alphabetical = "alphabetical"
@@ -98,15 +100,15 @@
         for name in members_list:
             if name in members_dict:
                 sorted_members.append(members_dict[name])
         return sorted_members
     return sorted(members, key=order_map[order])
 
 
-def do_crossref(path: str, brief: bool = True) -> Markup:
+def do_crossref(path: str, *, brief: bool = True) -> Markup:
     """Filter to create cross-references.
 
     Parameters:
         path: The path to link to.
         brief: Show only the last part of the path, add full path as hover.
 
     Returns:
@@ -114,60 +116,61 @@
     """
     full_path = path
     if brief:
         path = full_path.split(".")[-1]
     return Markup("<span data-autorefs-optional-hover={full_path}>{path}</span>").format(full_path=full_path, path=path)
 
 
-def do_multi_crossref(text: str, code: bool = True) -> Markup:
+def do_multi_crossref(text: str, *, code: bool = True) -> Markup:
     """Filter to create cross-references.
 
     Parameters:
         text: The text to scan.
         code: Whether to wrap the result in a code tag.
 
     Returns:
         Markup text.
     """
     group_number = 0
     variables = {}
 
-    def repl(match):  # noqa: WPS430
-        nonlocal group_number  # noqa: WPS420
+    def repl(match: Match) -> str:
+        nonlocal group_number
         group_number += 1
         path = match.group()
         path_var = f"path{group_number}"
         variables[path_var] = path
         return f"<span data-autorefs-optional-hover={{{path_var}}}>{{{path_var}}}</span>"
 
     text = re.sub(r"([\w.]+)", repl, text)
     if code:
         text = f"<code>{text}</code>"
     return Markup(text).format(**variables)
 
 
-def _keep_object(name, filters):
+def _keep_object(name: str, filters: Sequence[tuple[Pattern, bool]]) -> bool:
     keep = None
     rules = set()
     for regex, exclude in filters:
         rules.add(exclude)
         if regex.search(name):
             keep = not exclude
     if keep is None:
-        if rules == {False}:  # noqa: WPS531
+        if rules == {False}:
             # only included stuff, no match = reject
             return False
         # only excluded stuff, or included and excluded stuff, no match = keep
         return True
     return keep
 
 
 def do_filter_objects(
     objects_dictionary: dict[str, Object | Alias],
-    filters: list[tuple[bool, Pattern]] | None = None,
+    *,
+    filters: Sequence[tuple[Pattern, bool]] | None = None,
     members_list: list[str] | None = None,
     keep_no_docstrings: bool = True,
 ) -> list[Object | Alias]:
     """Filter a dictionary of objects based on their docstrings.
 
     Parameters:
         objects_dictionary: The dictionary of objects.
@@ -191,19 +194,19 @@
         objects = [obj for obj in objects if _keep_object(obj.name, filters)]
     if keep_no_docstrings:
         return objects
     return [obj for obj in objects if obj.has_docstrings]
 
 
 @lru_cache(maxsize=1)
-def _get_black_formatter():
+def _get_black_formatter() -> Callable[[str, int], str]:
     try:
         from black import Mode, format_str
     except ModuleNotFoundError:
         logger.warning("Formatting signatures requires Black to be installed.")
         return lambda text, _: text
 
-    def formatter(code, line_length):  # noqa: WPS430
+    def formatter(code: str, line_length: int) -> str:
         mode = Mode(line_length=line_length)
         return format_str(code, mode=mode)
 
     return formatter
```

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/children.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html`

 * *Files 7% similar despite different names*

```diff
@@ -15,45 +15,45 @@
 
         {% if config.show_category_heading %}
           {% set extra_level = 1 %}
         {% else %}
           {% set extra_level = 0 %}
         {% endif %}
 
-        {% with attributes = obj.attributes|filter_objects(config.filters, members_list, config.show_if_no_docstring) %}
+        {% with attributes = obj.attributes|filter_objects(filters=config.filters, members_list=members_list, keep_no_docstrings=config.show_if_no_docstring) %}
           {% if attributes %}
             {% if config.show_category_heading %}
               {% filter heading(heading_level, id=html_id ~ "-attributes") %}Attributes{% endfilter %}
             {% endif %}
             {% with heading_level = heading_level + extra_level %}
               {% for attribute in attributes|order_members(config.members_order, members_list) %}
                 {% if not attribute.is_alias or attribute.is_explicitely_exported %}
                   {% include "attribute.html" with context %}
                 {% endif %}
               {% endfor %}
             {% endwith %}
           {% endif %}
         {% endwith %}
 
-        {% with classes = obj.classes|filter_objects(config.filters, members_list, config.show_if_no_docstring) %}
+        {% with classes = obj.classes|filter_objects(filters=config.filters, members_list=members_list, keep_no_docstrings=config.show_if_no_docstring) %}
           {% if classes %}
             {% if config.show_category_heading %}
               {% filter heading(heading_level, id=html_id ~ "-classes") %}Classes{% endfilter %}
             {% endif %}
             {% with heading_level = heading_level + extra_level %}
               {% for class in classes|order_members(config.members_order, members_list) %}
                 {% if not class.is_alias or class.is_explicitely_exported %}
                   {% include "class.html" with context %}
                 {% endif %}
               {% endfor %}
             {% endwith %}
           {% endif %}
         {% endwith %}
 
-        {% with functions = obj.functions|filter_objects(config.filters, members_list, config.show_if_no_docstring) %}
+        {% with functions = obj.functions|filter_objects(filters=config.filters, members_list=members_list, keep_no_docstrings=config.show_if_no_docstring) %}
           {% if functions %}
             {% if config.show_category_heading %}
               {% filter heading(heading_level, id=html_id ~ "-functions") %}Functions{% endfilter %}
             {% endif %}
             {% with heading_level = heading_level + extra_level %}
               {% for function in functions|order_members(config.members_order, members_list) %}
                 {% if not (obj.kind.value == "class" and function.name == "__init__" and config.merge_init_into_class) %}
@@ -63,15 +63,15 @@
                 {% endif %}
               {% endfor %}
             {% endwith %}
           {% endif %}
         {% endwith %}
 
         {% if config.show_submodules %}
-          {% with modules = obj.modules|filter_objects(config.filters, members_list, config.show_if_no_docstring) %}
+          {% with modules = obj.modules|filter_objects(filters=config.filters, members_list=members_list, keep_no_docstrings=config.show_if_no_docstring) %}
             {% if modules %}
               {% if config.show_category_heading %}
                 {% filter heading(heading_level, id=html_id ~ "-modules") %}Modules{% endfilter %}
               {% endif %}
               {% with heading_level = heading_level + extra_level %}
                 {% for module in modules|order_members(config.members_order, members_list) %}
                   {% if not module.is_alias or module.is_explicitely_exported %}
@@ -84,15 +84,15 @@
         {% endif %}
 
       {% endwith %}
 
     {% else %}
 
       {% for child in obj.members|
-          filter_objects(config.filters, members_list, config.show_if_no_docstring)|
+          filter_objects(filters=config.filters, members_list=members_list, keep_no_docstrings=config.show_if_no_docstring)|
           order_members(config.members_order, members_list) %}
 
         {% if not (obj.kind.value == "class" and child.name == "__init__" and config.merge_init_into_class) %}
 
           {% if child.kind.value == "attribute" %}
             {% with attribute = child %}
               {% include "attribute.html" with context %}
```

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/class.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 {% if docstring_sections %}
   {{ log.debug("Rendering docstring") }}
   {% for section in docstring_sections %}
-    {% if section.kind.value == "text" %}
+    {% if config.show_docstring_description and section.kind.value == "text" %}
       {{ section.value|convert_markdown(heading_level, html_id) }}
-    {% elif section.kind.value == "attributes" %}
+    {% elif config.show_docstring_attributes and section.kind.value == "attributes" %}
       {% include "docstring/attributes.html" with context %}
-    {% elif section.kind.value == "parameters" %}
+    {% elif config.show_docstring_parameters and section.kind.value == "parameters" %}
       {% include "docstring/parameters.html" with context %}
-    {% elif section.kind.value == "other parameters" %}
+    {% elif config.show_docstring_other_parameters and section.kind.value == "other parameters" %}
       {% include "docstring/other_parameters.html" with context %}
-    {% elif section.kind.value == "raises" %}
+    {% elif config.show_docstring_raises and section.kind.value == "raises" %}
       {% include "docstring/raises.html" with context %}
-      {% elif section.kind.value == "warns" %}
-        {% include "docstring/warns.html" with context %}
-    {% elif section.kind.value == "yields" %}
+    {% elif config.show_docstring_warns and section.kind.value == "warns" %}
+      {% include "docstring/warns.html" with context %}
+    {% elif config.show_docstring_yields and section.kind.value == "yields" %}
       {% include "docstring/yields.html" with context %}
-      {% elif section.kind.value == "receives" %}
-        {% include "docstring/receives.html" with context %}
-    {% elif section.kind.value == "returns" %}
+    {% elif config.show_docstring_receives and section.kind.value == "receives" %}
+      {% include "docstring/receives.html" with context %}
+    {% elif config.show_docstring_returns and section.kind.value == "returns" %}
       {% include "docstring/returns.html" with context %}
-    {% elif section.kind.value == "examples" %}
+    {% elif config.show_docstring_examples and section.kind.value == "examples" %}
       {% include "docstring/examples.html" with context %}
-    {% elif section.kind.value == "admonition" %}
+    {% elif config.show_docstring_description and section.kind.value == "admonition" %}
       {% include "docstring/admonition.html" with context %}
     {% endif %}
   {% endfor %}
 {% endif %}
```

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/expression.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/function.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/module.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/_base/signature.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/material/style.css` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/material/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/src/mkdocstrings_handlers/python/templates/readthedocs/style.css` & `mkdocstrings-python-0.9.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings-python-0.8.3/tests/conftest.py` & `mkdocstrings-python-0.9.0/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,90 +1,96 @@
 """Configuration for the pytest test suite."""
 
 from __future__ import annotations
 
 from collections import ChainMap
+from typing import TYPE_CHECKING, Any, Iterator
 
 import pytest
 from markdown.core import Markdown
 from mkdocs import config
 from mkdocs.config.defaults import get_schema
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from mkdocstrings.plugin import MkdocstringsPlugin
+
+    from mkdocstrings_handlers.python.handler import PythonHandler
+
 
 @pytest.fixture(name="mkdocs_conf")
-def fixture_mkdocs_conf(request, tmp_path):
+def fixture_mkdocs_conf(request: pytest.FixtureRequest, tmp_path: Path) -> Iterator[config.Config]:
     """Yield a MkDocs configuration object.
 
     Parameters:
         request: Pytest fixture.
         tmp_path: Pytest fixture.
 
     Yields:
         MkDocs config.
     """
-    conf = config.Config(schema=get_schema())
-    while hasattr(request, "_parent_request") and hasattr(request._parent_request, "_parent_request"):  # noqa: WPS437
-        request = request._parent_request  # noqa: WPS437
+    conf = config.Config(schema=get_schema())  # type: ignore[call-arg]
+    while hasattr(request, "_parent_request") and hasattr(request._parent_request, "_parent_request"):
+        request = request._parent_request
 
     conf_dict = {
         "site_name": "foo",
         "site_url": "https://example.org/",
         "site_dir": str(tmp_path),
         "plugins": [{"mkdocstrings": {"default_handler": "python"}}],
         **getattr(request, "param", {}),
     }
     # Re-create it manually as a workaround for https://github.com/mkdocs/mkdocs/issues/2289
-    mdx_configs = dict(ChainMap(*conf_dict.get("markdown_extensions", [])))
+    mdx_configs: dict[str, Any] = dict(ChainMap(*conf_dict.get("markdown_extensions", [])))  # type: ignore[arg-type]
 
     conf.load_dict(conf_dict)
     assert conf.validate() == ([], [])
 
     conf["mdx_configs"] = mdx_configs
     conf["markdown_extensions"].insert(0, "toc")  # Guaranteed to be added by MkDocs.
 
     conf = conf["plugins"]["mkdocstrings"].on_config(conf)
     conf = conf["plugins"]["autorefs"].on_config(conf)
     yield conf
     conf["plugins"]["mkdocstrings"].on_post_build(conf)
 
 
 @pytest.fixture(name="plugin")
-def fixture_plugin(mkdocs_conf):
+def fixture_plugin(mkdocs_conf: config.Config) -> MkdocstringsPlugin:
     """Return a plugin instance.
 
     Parameters:
         mkdocs_conf: Pytest fixture: [tests.conftest.fixture_mkdocs_conf][].
 
     Returns:
         mkdocstrings plugin instance.
     """
-    plugin = mkdocs_conf["plugins"]["mkdocstrings"]
-    plugin.md = Markdown(extensions=mkdocs_conf["markdown_extensions"], extension_configs=mkdocs_conf["mdx_configs"])
-    return plugin
+    return mkdocs_conf["plugins"]["mkdocstrings"]
 
 
 @pytest.fixture(name="ext_markdown")
-def fixture_ext_markdown(plugin):
+def fixture_ext_markdown(mkdocs_conf: config.Config) -> Markdown:
     """Return a Markdown instance with MkdocstringsExtension.
 
     Parameters:
-        plugin: Pytest fixture: [tests.conftest.fixture_plugin][].
+        mkdocs_conf: Pytest fixture: [tests.conftest.fixture_mkdocs_conf][].
 
     Returns:
         A Markdown instance.
     """
-    return plugin.md
+    return Markdown(extensions=mkdocs_conf["markdown_extensions"], extension_configs=mkdocs_conf["mdx_configs"])
 
 
 @pytest.fixture(name="handler")
-def fixture_handler(plugin):
+def fixture_handler(plugin: MkdocstringsPlugin, ext_markdown: Markdown) -> PythonHandler:
     """Return a handler instance.
 
     Parameters:
         plugin: Pytest fixture: [tests.conftest.fixture_plugin][].
 
     Returns:
         A handler instance.
     """
     handler = plugin.handlers.get_handler("python")
-    handler._update_env(plugin.md, plugin.handlers._config)  # noqa: WPS437
-    return handler
+    handler._update_env(ext_markdown, plugin.handlers._config)
+    return handler  # type: ignore[return-value]
```

### Comparing `mkdocstrings-python-0.8.3/tests/test_handler.py` & `mkdocstrings-python-0.9.0/tests/test_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 """Tests for the `handler` module."""
 
+from __future__ import annotations
+
 import os
 from glob import glob
+from typing import TYPE_CHECKING
 
 import pytest
 from griffe.docstrings.dataclasses import DocstringSectionExamples, DocstringSectionKind
 
 from mkdocstrings_handlers.python.handler import CollectionError, PythonHandler, get_handler
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
-def test_collect_missing_module():
+def test_collect_missing_module() -> None:
     """Assert error is raised for missing modules."""
     handler = get_handler(theme="material")
     with pytest.raises(CollectionError):
         handler.collect("aaaaaaaa", {})
 
 
-def test_collect_missing_module_item():
+def test_collect_missing_module_item() -> None:
     """Assert error is raised for missing items within existing modules."""
     handler = get_handler(theme="material")
     with pytest.raises(CollectionError):
         handler.collect("mkdocstrings.aaaaaaaa", {})
 
 
-def test_collect_module():
+def test_collect_module() -> None:
     """Assert existing module can be collected."""
     handler = get_handler(theme="material")
     assert handler.collect("mkdocstrings", {})
 
 
-def test_collect_with_null_parser():
+def test_collect_with_null_parser() -> None:
     """Assert we can pass `None` as parser when collecting."""
     handler = get_handler(theme="material")
     assert handler.collect("mkdocstrings", {"docstring_style": None})
 
 
 @pytest.mark.parametrize(
     "handler",
     [
         {"theme": "mkdocs"},
         {"theme": "readthedocs"},
         {"theme": {"name": "material"}},
     ],
     indirect=["handler"],
 )
-def test_render_docstring_examples_section(handler):
+def test_render_docstring_examples_section(handler: PythonHandler) -> None:
     """Assert docstrings' examples section can be rendered.
 
     Parameters:
         handler: A handler instance (parametrized).
     """
     section = DocstringSectionExamples(
         value=[
@@ -59,15 +65,15 @@
     template = handler.env.get_template("docstring/examples.html")
     rendered = template.render(section=section)
     assert "<p>This is an example.</p>" in rendered
     assert "print" in rendered
     assert "Hello" in rendered
 
 
-def test_expand_globs(tmp_path):
+def test_expand_globs(tmp_path: Path) -> None:
     """Assert globs are correctly expanded.
 
     Parameters:
         tmp_path: Pytext fixture that creates a temporary directory.
     """
     globbed_names = (
         "expanded_a",
@@ -77,24 +83,24 @@
     )
     globbed_paths = [tmp_path.joinpath(globbed_name) for globbed_name in globbed_names]
     for path in globbed_paths:
         path.touch()
     handler = PythonHandler(
         handler="python",
         theme="material",
-        config_file_path=tmp_path / "mkdocs.yml",
+        config_file_path=str(tmp_path.joinpath("mkdocs.yml")),
         paths=["*exp*"],
     )
-    for path in globbed_paths:  # noqa: WPS440
-        assert str(path) in handler._paths  # noqa: WPS437
+    for path in globbed_paths:
+        assert str(path) in handler._paths
 
 
-def test_expand_globs_without_changing_directory():
+def test_expand_globs_without_changing_directory() -> None:
     """Assert globs are correctly expanded when we are already in the right directory."""
     handler = PythonHandler(
         handler="python",
         theme="material",
         config_file_path="mkdocs.yml",
         paths=["*.md"],
     )
     for path in list(glob(os.path.abspath(".") + "/*.md")):
-        assert path in handler._paths  # noqa: WPS437
+        assert path in handler._paths
```

### Comparing `mkdocstrings-python-0.8.3/tests/test_rendering.py` & `mkdocstrings-python-0.9.0/tests/test_rendering.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Tests for the `rendering` module."""
 
+from __future__ import annotations
+
 import re
 from dataclasses import dataclass
+from typing import Any
 
 import pytest
 
 from mkdocstrings_handlers.python import rendering
 
 
-def test_format_code_and_signature():
+def test_format_code_and_signature() -> None:
     """Assert code and signatures can be Black-formatted."""
     assert rendering.do_format_code("print('Hello')", 100)
     assert rendering.do_format_code('print("Hello")', 100)
     assert rendering.do_format_signature("(param: str = 'hello') -> 'Class'", 100)
     assert rendering.do_format_signature('(param: str = "hello") -> "Class"', 100)
 
 
@@ -24,19 +27,19 @@
 @pytest.mark.parametrize(
     ("names", "filter_params", "expected_names"),
     [
         (["aa", "ab", "ac", "da"], {"filters": [(re.compile("^a[^b]"), True)]}, {"ab", "da"}),
         (["aa", "ab", "ac", "da"], {"members_list": ["aa", "ab"]}, {"aa", "ab"}),
     ],
 )
-def test_filter_objects(names, filter_params, expected_names):
+def test_filter_objects(names: list[str], filter_params: dict[str, Any], expected_names: set[str]) -> None:
     """Assert the objects filter works correctly.
 
     Parameters:
         names: Names of the objects.
         filter_params: Parameters passed to the filter function.
         expected_names: Names expected to be kept.
     """
     objects = {name: _FakeObject(name) for name in names}
-    filtered = rendering.do_filter_objects(objects, **filter_params)
+    filtered = rendering.do_filter_objects(objects, **filter_params)  # type: ignore[arg-type]
     filtered_names = {obj.name for obj in filtered}
     assert set(filtered_names) == set(expected_names)
```

### Comparing `mkdocstrings-python-0.8.3/tests/test_themes.py` & `mkdocstrings-python-0.9.0/tests/test_themes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 """Tests for the different themes we claim to support."""
 
+from __future__ import annotations
+
 import sys
+from typing import TYPE_CHECKING
 
 import pytest
 
+if TYPE_CHECKING:
+    from markdown import Markdown
+    from mkdocstrings.plugin import MkdocstringsPlugin
+
 
 @pytest.mark.parametrize(
     "plugin",
     [
         {"theme": "mkdocs"},
         {"theme": "readthedocs"},
         {"theme": {"name": "material"}},
@@ -23,18 +30,18 @@
         "mkdocstrings.plugin",
         "mkdocstrings.handlers.base",
         "mkdocstrings.handlers.rendering",
         "mkdocstrings_handlers.python",
     ],
 )
 @pytest.mark.skipif(sys.version_info < (3, 7), reason="material is not installed on Python 3.6")
-def test_render_themes_templates_python(module, plugin):
+def test_render_themes_templates_python(module: str, plugin: MkdocstringsPlugin, ext_markdown: Markdown) -> None:
     """Test rendering of a given theme's templates.
 
     Parameters:
         module: Parametrized argument.
         plugin: Pytest fixture: [tests.conftest.fixture_plugin][].
     """
     handler = plugin.handlers.get_handler("python")
-    handler._update_env(plugin.md, plugin.handlers._config)  # noqa: WPS437
+    handler._update_env(ext_markdown, plugin.handlers._config)
     data = handler.collect(module, {})
     handler.render(data, {})
```

### Comparing `mkdocstrings-python-0.8.3/PKG-INFO` & `mkdocstrings-python-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocstrings-python
-Version: 0.8.3
+Version: 0.9.0
 Summary: A Python handler for mkdocstrings.
 License: ISC
 Author-email: Timothée Mazzucotelli <pawamoy@pm.me>
 Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -65,15 +65,15 @@
 # adapt to your dependencies manager
 [project]
 dependencies = [
     "mkdocstrings[python]>=0.18",
 ]
 ```
 
-You can also explicitely depend on the handler:
+You can also explicitly depend on the handler:
 
 ```toml title="pyproject.toml"
 # PEP 621 dependencies declaration
 # adapt to your dependencies manager
 [project]
 dependencies = [
     "mkdocstrings-python",
@@ -87,32 +87,32 @@
 
 ## Features
 
 - **Data collection from source code**: collection of the object-tree and the docstrings is done thanks to
   [Griffe](https://github.com/mkdocstrings/griffe).
 
 - **Support for type annotations:** Griffe collects your type annotations and *mkdocstrings* uses them
-  to display parameters types or return types. It is even able to automatically add cross-references
-  to other objects from your API, from the standard library or from third-party libraries!
+  to display parameter types or return types. It is even able to automatically add cross-references
+  to other objects from your API, from the standard library or third-party libraries!
   See [how to load inventories](https://mkdocstrings.github.io/usage/#cross-references-to-other-projects-inventories) to enable it.
 
-- **Recursive documentation of Python objects:** just use the module dotted-path as identifier, and you get the full
+- **Recursive documentation of Python objects:** just use the module dotted-path as an identifier, and you get the full
   module docs. You don't need to inject documentation for each class, function, etc.
 
 - **Support for documented attributes:** attributes (variables) followed by a docstring (triple-quoted string) will
   be recognized by Griffe in modules, classes and even in `__init__` methods.
 
 - **Multiple docstring-styles support:** common support for Google-style, Numpydoc-style,
   and Sphinx-style docstrings. See [Griffe's documentation](https://mkdocstrings.github.io/griffe/docstrings/) on docstrings support.
 
 - **Admonition support in Google docstrings:** blocks like `Note:` or `Warning:` will be transformed
   to their [admonition](https://squidfunk.github.io/mkdocs-material/reference/admonitions/) equivalent.
   *We do not support nested admonitions in docstrings!*
 
 - **Every object has a TOC entry:** we render a heading for each object, meaning *MkDocs* picks them into the Table
-  of Contents, which is nicely display by the Material theme. Thanks to *mkdocstrings* cross-reference ability,
+  of Contents, which is nicely displayed by the Material theme. Thanks to *mkdocstrings* cross-reference ability,
   you can reference other objects within your docstrings, with the classic Markdown syntax:
   `[this object][package.module.object]` or directly with `[package.module.object][]`
 
 - **Source code display:** *mkdocstrings* can add a collapsible div containing the highlighted source code
   of the Python object.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocstrings-python Version: 0.8.3 Summary: A
+Metadata-Version: 2.1 Name: mkdocstrings-python Version: 0.9.0 Summary: A
 Python handler for mkdocstrings. License: ISC Author-email: TimothÃ©e
 Mazzucotelli
 pm.me> Requires-Python: >=3.7 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
@@ -22,38 +22,38 @@
                       A Python handler for mkdocstrings.
              [ci] [documentation] [pypi_version] [gitpod] [gitter]
 ---
                                   [logo.png]
 ## Installation You can install this handler as a *mkdocstrings* extra: ```toml
 title="pyproject.toml" # PEP 621 dependencies declaration # adapt to your
 dependencies manager [project] dependencies = [ "mkdocstrings[python]>=0.18", ]
-``` You can also explicitely depend on the handler: ```toml
+``` You can also explicitly depend on the handler: ```toml
 title="pyproject.toml" # PEP 621 dependencies declaration # adapt to your
 dependencies manager [project] dependencies = [ "mkdocstrings-python", ] ``` ##
 Preview  ![mkdocstrings_python_gif](https://user-images.githubusercontent.com/
 3999221/77157838-7184db80-6aa2-11ea-9f9a-fe77405202de.gif) ## Features - **Data
 collection from source code**: collection of the object-tree and the docstrings
 is done thanks to [Griffe](https://github.com/mkdocstrings/griffe). - **Support
 for type annotations:** Griffe collects your type annotations and
-*mkdocstrings* uses them to display parameters types or return types. It is
-even able to automatically add cross-references to other objects from your API,
-from the standard library or from third-party libraries! See [how to load
-inventories](https://mkdocstrings.github.io/usage/#cross-references-to-other-
-projects-inventories) to enable it. - **Recursive documentation of Python
-objects:** just use the module dotted-path as identifier, and you get the full
-module docs. You don't need to inject documentation for each class, function,
-etc. - **Support for documented attributes:** attributes (variables) followed
-by a docstring (triple-quoted string) will be recognized by Griffe in modules,
+*mkdocstrings* uses them to display parameter types or return types. It is even
+able to automatically add cross-references to other objects from your API, from
+the standard library or third-party libraries! See [how to load inventories]
+(https://mkdocstrings.github.io/usage/#cross-references-to-other-projects-
+inventories) to enable it. - **Recursive documentation of Python objects:**
+just use the module dotted-path as an identifier, and you get the full module
+docs. You don't need to inject documentation for each class, function, etc. -
+**Support for documented attributes:** attributes (variables) followed by a
+docstring (triple-quoted string) will be recognized by Griffe in modules,
 classes and even in `__init__` methods. - **Multiple docstring-styles support:
 ** common support for Google-style, Numpydoc-style, and Sphinx-style
 docstrings. See [Griffe's documentation](https://mkdocstrings.github.io/griffe/
 docstrings/) on docstrings support. - **Admonition support in Google
 docstrings:** blocks like `Note:` or `Warning:` will be transformed to their
 [admonition](https://squidfunk.github.io/mkdocs-material/reference/admonitions/
 ) equivalent. *We do not support nested admonitions in docstrings!* - **Every
 object has a TOC entry:** we render a heading for each object, meaning *MkDocs*
-picks them into the Table of Contents, which is nicely display by the Material
-theme. Thanks to *mkdocstrings* cross-reference ability, you can reference
-other objects within your docstrings, with the classic Markdown syntax: `[this
-object][package.module.object]` or directly with `[package.module.object][]` -
-**Source code display:** *mkdocstrings* can add a collapsible div containing
-the highlighted source code of the Python object.
+picks them into the Table of Contents, which is nicely displayed by the
+Material theme. Thanks to *mkdocstrings* cross-reference ability, you can
+reference other objects within your docstrings, with the classic Markdown
+syntax: `[this object][package.module.object]` or directly with `
+[package.module.object][]` - **Source code display:** *mkdocstrings* can add a
+collapsible div containing the highlighted source code of the Python object.
```

