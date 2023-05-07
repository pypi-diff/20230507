# Comparing `tmp/aswan-0.5.8.tar.gz` & `tmp/aswan-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aswan-0.5.8.tar", last modified: Mon Jan  2 11:52:16 2023, max compression
+gzip compressed data, was "aswan-0.5.9.tar", last modified: Wed Feb  8 14:37:21 2023, max compression
```

## Comparing `aswan-0.5.8.tar` & `aswan-0.5.9.tar`

### file list

```diff
@@ -1,106 +1,107 @@
--rw-r--r--   0        0        0      803 2023-01-02 11:52:11.606175 aswan-0.5.8/.github/workflows/test.yml
--rw-r--r--   0        0        0      566 2023-01-02 11:52:11.606175 aswan-0.5.8/.github/workflows/twine_release.yml
--rw-r--r--   0        0        0     1770 2023-01-02 11:52:11.606175 aswan-0.5.8/.gitignore
--rw-r--r--   0        0        0      287 2023-01-02 11:52:11.606175 aswan-0.5.8/.readthedocs.yml
--rw-r--r--   0        0        0      292 2023-01-02 11:52:11.606175 aswan-0.5.8/CITATION.cff
--rw-r--r--   0        0        0     1056 2023-01-02 11:52:11.606175 aswan-0.5.8/LICENSE
--rw-r--r--   0        0        0     2824 2023-01-02 11:52:11.606175 aswan-0.5.8/README.md
--rw-r--r--   0        0        0      744 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/__init__.py
--rw-r--r--   0        0        0     9424 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/connection_session.py
--rw-r--r--   0        0        0     1237 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/constants.py
--rw-r--r--   0        0        0      137 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/depot/__init__.py
--rw-r--r--   0        0        0    13757 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/depot/base.py
--rw-r--r--   0        0        0     5596 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/depot/remote.py
--rw-r--r--   0        0        0       91 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/exceptions.py
--rw-r--r--   0        0        0     2913 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/metadata_handling.py
--rw-r--r--   0        0        0     4165 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/models.py
--rw-r--r--   0        0        0     5914 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/monitor_app.py
--rw-r--r--   0        0        0     3424 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/object_store.py
--rw-r--r--   0        0        0     6684 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/project.py
--rw-r--r--   0        0        0      350 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/resources.py
--rw-r--r--   0        0        0     4285 2023-01-02 11:52:11.606175 aswan-0.5.8/aswan/security.py
--rw-r--r--   0        0        0     1352 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/simplified_functions.py
--rw-r--r--   0        0        0        0 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/__init__.py
--rw-r--r--   0        0        0       86 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/godel_src/__init__.py
--rw-r--r--   0        0        0      705 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/godel_src/app.py
--rw-r--r--   0        0        0     2799 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/godel_src/handlers.py
--rw-r--r--   0        0        0       94 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/godel_src/test_pages/Alonzo_Church.html
--rw-r--r--   0        0        0       18 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/godel_src/test_pages/Axiom.html
--rw-r--r--   0        0        0      432 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/godel_src/test_pages/Entscheidungsproblem
--rw-r--r--   0        0        0      228 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/godel_src/test_pages/Halting_problem.html
--rw-r--r--   0        0        0     1630 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/godel_src/test_pages/godel_wiki.html
--rw-r--r--   0        0        0      627 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/godel_src/test_pages/jstest.html
--rw-r--r--   0        0        0      312 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/godel_src/test_pages/jstest_bad.html
--rw-r--r--   0        0        0      627 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/godel_src/test_pages/jstest_minus.html
--rw-r--r--   0        0        0       10 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/godel_src/test_pages/test_json.json
--rw-r--r--   0        0        0     2421 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/integration/test_godel.py
--rw-r--r--   0        0        0     1784 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/integration/test_godel_load.py
--rw-r--r--   0        0        0      881 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/proxy_src.py
--rw-r--r--   0        0        0        0 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/unit/__init__.py
--rw-r--r--   0        0        0     2844 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/unit/test_conn_session.py
--rw-r--r--   0        0        0     2728 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/unit/test_depot.py
--rw-r--r--   0        0        0     2780 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/unit/test_depot_remotes.py
--rw-r--r--   0        0        0     1640 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/unit/test_metadata_handling.py
--rw-r--r--   0        0        0      485 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/unit/test_monitor_app.py
--rw-r--r--   0        0        0     2291 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/unit/test_object_store.py
--rw-r--r--   0        0        0     1299 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/unit/test_project_class.py
--rw-r--r--   0        0        0      271 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/unit/test_proxy.py
--rw-r--r--   0        0        0     1414 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/unit/test_simplified_functions.py
--rw-r--r--   0        0        0     1347 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/tests/unit/test_utils.py
--rw-r--r--   0        0        0     5052 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/url_handler.py
--rw-r--r--   0        0        0     2473 2023-01-02 11:52:11.610175 aswan-0.5.8/aswan/utils.py
--rw-r--r--   0        0        0     3925 2023-01-02 11:52:11.610175 aswan-0.5.8/conftest.py
--rw-r--r--   0        0        0       97 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.AswanDepot.rst
--rw-r--r--   0        0        0      103 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.BrokenSessionError.rst
--rw-r--r--   0        0        0      687 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.BrowserHandler.rst
--rw-r--r--   0        0        0      121 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.BrowserJsonHandler.rst
--rw-r--r--   0        0        0      121 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.BrowserSoupHandler.rst
--rw-r--r--   0        0        0       94 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.ConnectionError.rst
--rw-r--r--   0        0        0      477 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.ConnectionSession.rst
--rw-r--r--   0        0        0      811 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.ObjectStore.rst
--rw-r--r--   0        0        0      355 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.ParsedCollectionEvent.rst
--rw-r--r--   0        0        0      657 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.Project.rst
--rw-r--r--   0        0        0       94 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.ProxyAuth.rst
--rw-r--r--   0        0        0      792 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.ProxyBase.rst
--rw-r--r--   0        0        0      470 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.RequestHandler.rst
--rw-r--r--   0        0        0      121 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.RequestJsonHandler.rst
--rw-r--r--   0        0        0      121 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.RequestSoupHandler.rst
--rw-r--r--   0        0        0      780 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.Statuses.rst
--rw-r--r--   0        0        0       90 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.add_url_params.rst
--rw-r--r--   0        0        0       72 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.get_json.rst
--rw-r--r--   0        0        0       72 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.get_soup.rst
--rw-r--r--   0        0        0      102 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/api/aswan.run_simple_project.rst
--rw-r--r--   0        0        0       34 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/autosumm.rst
--rw-r--r--   0        0        0     2401 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/conf.py
--rw-r--r--   0        0        0      263 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/index.rst
--rw-r--r--   0        0        0       72 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/notebooks/doc-000-intro.rst
--rw-r--r--   0        0        0       77 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/notebooks/doc-001-quickstart.rst
--rw-r--r--   0        0        0      102 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/release_notes/main.rst
--rw-r--r--   0        0        0       46 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/release_notes/v0.0.0.rst
--rw-r--r--   0        0        0       38 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/release_notes/v0.0.1.rst
--rw-r--r--   0        0        0       29 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/release_notes/v0.1.0.rst
--rw-r--r--   0        0        0       32 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/release_notes/v0.1.1.rst
--rw-r--r--   0        0        0       35 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/release_notes/v0.2.0.rst
--rw-r--r--   0        0        0       27 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/release_notes/v0.3.0.rst
--rw-r--r--   0        0        0       26 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/release_notes/v0.3.1.rst
--rw-r--r--   0        0        0       52 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/release_notes/v0.4.0.rst
--rw-r--r--   0        0        0       40 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/release_notes/v0.4.1.rst
--rw-r--r--   0        0        0       28 2023-01-02 11:52:11.610175 aswan-0.5.8/docs/release_notes/v0.4.2.rst
--rw-r--r--   0        0        0       22 2023-01-02 11:52:11.614175 aswan-0.5.8/docs/release_notes/v0.4.3.rst
--rw-r--r--   0        0        0       22 2023-01-02 11:52:11.614175 aswan-0.5.8/docs/release_notes/v0.4.4.rst
--rw-r--r--   0        0        0       19 2023-01-02 11:52:11.614175 aswan-0.5.8/docs/release_notes/v0.4.5.rst
--rw-r--r--   0        0        0       43 2023-01-02 11:52:11.614175 aswan-0.5.8/docs/release_notes/v0.5.0.rst
--rw-r--r--   0        0        0       53 2023-01-02 11:52:11.614175 aswan-0.5.8/docs/release_notes/v0.5.1.rst
--rw-r--r--   0        0        0       51 2023-01-02 11:52:11.614175 aswan-0.5.8/docs/release_notes/v0.5.2.rst
--rw-r--r--   0        0        0       71 2023-01-02 11:52:11.614175 aswan-0.5.8/docs/release_notes/v0.5.3.rst
--rw-r--r--   0        0        0       42 2023-01-02 11:52:11.614175 aswan-0.5.8/docs/release_notes/v0.5.4.rst
--rw-r--r--   0        0        0       46 2023-01-02 11:52:11.614175 aswan-0.5.8/docs/release_notes/v0.5.5.rst
--rw-r--r--   0        0        0       51 2023-01-02 11:52:11.614175 aswan-0.5.8/docs/release_notes/v0.5.6.rst
--rw-r--r--   0        0        0       38 2023-01-02 11:52:11.614175 aswan-0.5.8/docs/release_notes/v0.5.7.rst
--rw-r--r--   0        0        0       66 2023-01-02 11:52:11.614175 aswan-0.5.8/docs/release_notes/v0.5.8.rst
--rw-r--r--   0        0        0      606 2023-01-02 11:52:11.614175 aswan-0.5.8/notebooks/doc-000-intro.ipynb
--rw-r--r--   0        0        0      686 2023-01-02 11:52:11.614175 aswan-0.5.8/notebooks/doc-001-quickstart.ipynb
--rw-r--r--   0        0        0     9198 2023-01-02 11:52:11.614175 aswan-0.5.8/notebooks/imdb-case.ipynb
--rw-r--r--   0        0        0     4459 2023-01-02 11:52:11.614175 aswan-0.5.8/notebooks/imdb.md
--rw-r--r--   0        0        0      822 2023-01-02 11:52:11.614175 aswan-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 aswan-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      803 2023-02-08 14:37:16.142571 aswan-0.5.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      566 2023-02-08 14:37:16.142571 aswan-0.5.9/.github/workflows/twine_release.yml
+-rw-r--r--   0        0        0     1770 2023-02-08 14:37:16.142571 aswan-0.5.9/.gitignore
+-rw-r--r--   0        0        0      287 2023-02-08 14:37:16.142571 aswan-0.5.9/.readthedocs.yml
+-rw-r--r--   0        0        0      292 2023-02-08 14:37:16.142571 aswan-0.5.9/CITATION.cff
+-rw-r--r--   0        0        0     1056 2023-02-08 14:37:16.142571 aswan-0.5.9/LICENSE
+-rw-r--r--   0        0        0     2834 2023-02-08 14:37:16.142571 aswan-0.5.9/README.md
+-rw-r--r--   0        0        0      744 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/__init__.py
+-rw-r--r--   0        0        0     9424 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/connection_session.py
+-rw-r--r--   0        0        0     1237 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/constants.py
+-rw-r--r--   0        0        0      137 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/depot/__init__.py
+-rw-r--r--   0        0        0    14121 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/depot/base.py
+-rw-r--r--   0        0        0     6016 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/depot/remote.py
+-rw-r--r--   0        0        0       91 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/exceptions.py
+-rw-r--r--   0        0        0     2913 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/metadata_handling.py
+-rw-r--r--   0        0        0     4165 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/models.py
+-rw-r--r--   0        0        0     5914 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/monitor_app.py
+-rw-r--r--   0        0        0     3424 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/object_store.py
+-rw-r--r--   0        0        0     6684 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/project.py
+-rw-r--r--   0        0        0      350 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/resources.py
+-rw-r--r--   0        0        0     4285 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/security.py
+-rw-r--r--   0        0        0     1352 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/simplified_functions.py
+-rw-r--r--   0        0        0        0 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/__init__.py
+-rw-r--r--   0        0        0       86 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/godel_src/__init__.py
+-rw-r--r--   0        0        0      705 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/godel_src/app.py
+-rw-r--r--   0        0        0     2799 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/godel_src/handlers.py
+-rw-r--r--   0        0        0       94 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/godel_src/test_pages/Alonzo_Church.html
+-rw-r--r--   0        0        0       18 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/godel_src/test_pages/Axiom.html
+-rw-r--r--   0        0        0      432 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/godel_src/test_pages/Entscheidungsproblem
+-rw-r--r--   0        0        0      228 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/godel_src/test_pages/Halting_problem.html
+-rw-r--r--   0        0        0     1630 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/godel_src/test_pages/godel_wiki.html
+-rw-r--r--   0        0        0      627 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/godel_src/test_pages/jstest.html
+-rw-r--r--   0        0        0      312 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/godel_src/test_pages/jstest_bad.html
+-rw-r--r--   0        0        0      627 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/godel_src/test_pages/jstest_minus.html
+-rw-r--r--   0        0        0       10 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/godel_src/test_pages/test_json.json
+-rw-r--r--   0        0        0     2421 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/integration/test_godel.py
+-rw-r--r--   0        0        0     1784 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/integration/test_godel_load.py
+-rw-r--r--   0        0        0      881 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/proxy_src.py
+-rw-r--r--   0        0        0        0 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/unit/__init__.py
+-rw-r--r--   0        0        0     2844 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/unit/test_conn_session.py
+-rw-r--r--   0        0        0     2728 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/unit/test_depot.py
+-rw-r--r--   0        0        0     2780 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/unit/test_depot_remotes.py
+-rw-r--r--   0        0        0     1640 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/unit/test_metadata_handling.py
+-rw-r--r--   0        0        0      485 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/unit/test_monitor_app.py
+-rw-r--r--   0        0        0     2291 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/unit/test_object_store.py
+-rw-r--r--   0        0        0     1299 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/unit/test_project_class.py
+-rw-r--r--   0        0        0      271 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/unit/test_proxy.py
+-rw-r--r--   0        0        0     1414 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/unit/test_simplified_functions.py
+-rw-r--r--   0        0        0     1347 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     5052 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/url_handler.py
+-rw-r--r--   0        0        0     2473 2023-02-08 14:37:16.142571 aswan-0.5.9/aswan/utils.py
+-rw-r--r--   0        0        0     3925 2023-02-08 14:37:16.142571 aswan-0.5.9/conftest.py
+-rw-r--r--   0        0        0       97 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.AswanDepot.rst
+-rw-r--r--   0        0        0      103 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.BrokenSessionError.rst
+-rw-r--r--   0        0        0      687 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.BrowserHandler.rst
+-rw-r--r--   0        0        0      121 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.BrowserJsonHandler.rst
+-rw-r--r--   0        0        0      121 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.BrowserSoupHandler.rst
+-rw-r--r--   0        0        0       94 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.ConnectionError.rst
+-rw-r--r--   0        0        0      477 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.ConnectionSession.rst
+-rw-r--r--   0        0        0      811 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.ObjectStore.rst
+-rw-r--r--   0        0        0      355 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.ParsedCollectionEvent.rst
+-rw-r--r--   0        0        0      657 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.Project.rst
+-rw-r--r--   0        0        0       94 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.ProxyAuth.rst
+-rw-r--r--   0        0        0      792 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.ProxyBase.rst
+-rw-r--r--   0        0        0      470 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.RequestHandler.rst
+-rw-r--r--   0        0        0      121 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.RequestJsonHandler.rst
+-rw-r--r--   0        0        0      121 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.RequestSoupHandler.rst
+-rw-r--r--   0        0        0      780 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.Statuses.rst
+-rw-r--r--   0        0        0       90 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.add_url_params.rst
+-rw-r--r--   0        0        0       72 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.get_json.rst
+-rw-r--r--   0        0        0       72 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.get_soup.rst
+-rw-r--r--   0        0        0      102 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/api/aswan.run_simple_project.rst
+-rw-r--r--   0        0        0       34 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/autosumm.rst
+-rw-r--r--   0        0        0     2401 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/conf.py
+-rw-r--r--   0        0        0      263 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/index.rst
+-rw-r--r--   0        0        0       72 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/notebooks/doc-000-intro.rst
+-rw-r--r--   0        0        0       77 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/notebooks/doc-001-quickstart.rst
+-rw-r--r--   0        0        0      102 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/main.rst
+-rw-r--r--   0        0        0       46 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.0.0.rst
+-rw-r--r--   0        0        0       38 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.0.1.rst
+-rw-r--r--   0        0        0       29 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.1.0.rst
+-rw-r--r--   0        0        0       32 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.1.1.rst
+-rw-r--r--   0        0        0       35 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.2.0.rst
+-rw-r--r--   0        0        0       27 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.3.0.rst
+-rw-r--r--   0        0        0       26 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.3.1.rst
+-rw-r--r--   0        0        0       52 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.4.0.rst
+-rw-r--r--   0        0        0       40 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.4.1.rst
+-rw-r--r--   0        0        0       28 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.4.2.rst
+-rw-r--r--   0        0        0       22 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.4.3.rst
+-rw-r--r--   0        0        0       22 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.4.4.rst
+-rw-r--r--   0        0        0       19 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.4.5.rst
+-rw-r--r--   0        0        0       43 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.5.0.rst
+-rw-r--r--   0        0        0       53 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.5.1.rst
+-rw-r--r--   0        0        0       51 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.5.2.rst
+-rw-r--r--   0        0        0       71 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.5.3.rst
+-rw-r--r--   0        0        0       42 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.5.4.rst
+-rw-r--r--   0        0        0       46 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.5.5.rst
+-rw-r--r--   0        0        0       51 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.5.6.rst
+-rw-r--r--   0        0        0       38 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.5.7.rst
+-rw-r--r--   0        0        0       66 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.5.8.rst
+-rw-r--r--   0        0        0       44 2023-02-08 14:37:16.142571 aswan-0.5.9/docs/release_notes/v0.5.9.rst
+-rw-r--r--   0        0        0      606 2023-02-08 14:37:16.142571 aswan-0.5.9/notebooks/doc-000-intro.ipynb
+-rw-r--r--   0        0        0      686 2023-02-08 14:37:16.142571 aswan-0.5.9/notebooks/doc-001-quickstart.ipynb
+-rw-r--r--   0        0        0     9198 2023-02-08 14:37:16.142571 aswan-0.5.9/notebooks/imdb-case.ipynb
+-rw-r--r--   0        0        0     4459 2023-02-08 14:37:16.142571 aswan-0.5.9/notebooks/imdb.md
+-rw-r--r--   0        0        0      822 2023-02-08 14:37:16.142571 aswan-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3804 1970-01-01 00:00:00.000000 aswan-0.5.9/PKG-INFO
```

### Comparing `aswan-0.5.8/.github/workflows/test.yml` & `aswan-0.5.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/.github/workflows/twine_release.yml` & `aswan-0.5.9/.github/workflows/twine_release.yml`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/.gitignore` & `aswan-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/LICENSE` & `aswan-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/README.md` & `aswan-0.5.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # aswan
 
 [![Documentation Status](https://readthedocs.org/projects/aswan/badge/?version=latest)](https://aswan.readthedocs.io/en/latest)
 [![codeclimate](https://img.shields.io/codeclimate/maintainability/endremborza/aswan.svg)](https://codeclimate.com/github/endremborza/aswan)
 [![codecov](https://img.shields.io/codecov/c/github/endremborza/aswan)](https://codecov.io/gh/endremborza/aswan)
 [![pypi](https://img.shields.io/pypi/v/aswan.svg)](https://pypi.org/project/aswan/)
-[![DOI](https://zenodo.org/badge/360285787.svg)](https://zenodo.org/badge/latestdoi/360285787)
-
+[![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.7477587.svg)](https://doi.org/10.5281/zenodo.7477587)
 
 collect and organize data into a T1 data depot 
 named after the [Aswan Dam](https://en.wikipedia.org/wiki/Aswan_Dam)
 
 Collect and compress data from the internet for later parsing
 
 - quick, parallel, customizable to collect
```

### Comparing `aswan-0.5.8/aswan/__init__.py` & `aswan-0.5.9/aswan/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     BrowserSoupHandler,
     RequestHandler,
     RequestJsonHandler,
     RequestSoupHandler,
 )
 from .utils import add_url_params
 
-__version__ = "0.5.8"
+__version__ = "0.5.9"
```

### Comparing `aswan-0.5.8/aswan/connection_session.py` & `aswan-0.5.9/aswan/connection_session.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/constants.py` & `aswan-0.5.9/aswan/constants.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/depot/base.py` & `aswan-0.5.9/aswan/depot/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,23 +204,24 @@
         if init:
             self.init_w_complete()
         return self
 
     def purge(self):
         if self.root.exists():
             rmtree(self.root)
+        self._status_cache = self._load_status_cache()
         return self
 
     def init_w_complete(self):
         self.set_as_current(self.get_complete_status())
         return self
 
     def get_complete_status(self) -> Status:
         # either an existing, a new or a blank status
-        leaf, leaf_tree = self._get_leaf()
+        leaf, leaf_tree = self._get_leaf(needs_db=True)
         missing_runs = self.get_all_run_ids() - leaf_tree
         if missing_runs:
             return self.integrate(leaf, missing_runs)
         return leaf
 
     def get_status(self, status_name):
         status = self._status_cache.statuses.get(status_name)
@@ -303,24 +304,29 @@
 
         for ev_iter in event_iters:
             for ev in filter(_filter, get_sorted_coll_events(ev_iter)):
                 yield ParsedCollectionEvent(ev, self.object_store)
                 if only_latest:
                     urls.add(ev.url)
 
-    def _get_leaf(self):
+    def _get_leaf(self, needs_db=False):
         # just one that has no children
         # and has the most runs in its tree
         most_runs = 0
         leaf, leaf_tree = Status(), set()
-        for status_path in self.statuses_path.iterdir():
-            status_name = status_path.name
+        self.statuses_path.mkdir(exist_ok=True)
+        local_names = [sp.name for sp in self.statuses_path.iterdir()]
+        status_names = set([*local_names, *self._status_cache.statuses.keys()])
+        for status_name in status_names:
             candidate = self.get_status(status_name)
             if self._status_cache.parent_keys[status_name]:
                 continue
+            sdb = self.statuses_path / status_name / STATUS_DB_ZIP
+            if needs_db and (not sdb.exists()):
+                continue
             candidate_tree = self._get_full_run_tree(candidate)
             _run_count = len(candidate_tree)
             if _run_count >= most_runs:
                 leaf, leaf_tree = candidate, candidate_tree
                 most_runs = _run_count
         return leaf, leaf_tree
```

### Comparing `aswan-0.5.8/aswan/depot/remote.py` & `aswan-0.5.9/aswan/depot/remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,18 +57,22 @@
             rem_abs_path = f"{conn.cwd}/{rel_elem}"
             conn.put(elem.as_posix(), rem_abs_path)
 
     def _pull(self, conn: "Connection", complete: bool, post_status: Optional[str]):
         _ls = partial(self._remote_ls, conn)
         _mv = partial(self._conn_move, conn)
         self._merge_status_cache(conn)
+        # TODO: all this set() thing brings a bit of uncertainty
         remote_statuses = set(_ls(self.statuses_path))
-        if not complete:
-            remote_statuses.difference_update(self._load_status_cache().statuses.keys())
-        for rem_status in remote_statuses:
+        if complete:
+            ctx_to_pull = remote_statuses
+        else:
+            ctx_to_pull = remote_statuses.difference(self._status_cache.statuses.keys())
+        logger.info(f"pulling {len(ctx_to_pull)} status contexts")
+        for rem_status in ctx_to_pull:
             _mv(self.statuses_path / rem_status / CONTEXT_YAML)
         leaf, leaf_tree = self._get_leaf()
         status_dbs_to_pull = set()
         if complete:
             status_dbs_to_pull = remote_statuses
         elif leaf.name in remote_statuses:
             status_dbs_to_pull.add(leaf.name)
@@ -76,25 +80,27 @@
         remote_runs = set(_ls(self.runs_path))
         runs_to_pull = remote_runs - leaf_tree
         if post_status is not None:
             break_status = self.get_status(post_status)
             runs_to_pull = remote_runs - self._get_full_run_tree(break_status)
         elif complete:
             runs_to_pull = remote_runs
-
+        logger.info(f"pulling {len(status_dbs_to_pull)} status dbs")
         for status in status_dbs_to_pull:
             _mv(self.statuses_path / status / STATUS_DB_ZIP)
+        logger.info(f"pulling {len(runs_to_pull)} runs")
         for run in runs_to_pull:
             _mv(self.runs_path / run / EVENTS_ZIP)
         needed_objects = None
         if post_status is not None:
             pcevs = self.get_handler_events(only_latest=False, past_runs=runs_to_pull)
             needed_objects = set([pcev.cev.extend().output_file for pcev in pcevs])
+            logger.info(f"pulling {len(needed_objects)} objects")
 
-        if (not complete) and (post_status is None):
+        if (not complete) and (not needed_objects):
             return runs_to_pull
 
         for obj_dir in _ls(self.object_store_path, False):
             for obj_file in _ls(self.object_store_path / obj_dir):
                 if (not complete) and (obj_file not in needed_objects):
                     continue
                 _mv(self.object_store_path / obj_dir / obj_file)
@@ -111,14 +117,15 @@
             conn.get(rem_path, tmp_path.as_posix())
         except invoke.UnexpectedExit:
             pass
 
         rem_cache = StatusCache.read(tmp_path)
         tmp_path.unlink(missing_ok=True)
         self._status_cache.merge(rem_cache)
+        self._status_cache.dump(self._cache_path)
 
     def _remote_ls(self, conn, dir_path: Path, only_remote=True) -> list[str]:
         import invoke
 
         local_posix = dir_path.relative_to(self.root).as_posix()
         try:
             _ls: list[str] = conn.run(f"ls {local_posix}", hide=True).stdout.split()
```

### Comparing `aswan-0.5.8/aswan/metadata_handling.py` & `aswan-0.5.9/aswan/metadata_handling.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/models.py` & `aswan-0.5.9/aswan/models.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/monitor_app.py` & `aswan-0.5.9/aswan/monitor_app.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/object_store.py` & `aswan-0.5.9/aswan/object_store.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/project.py` & `aswan-0.5.9/aswan/project.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/security.py` & `aswan-0.5.9/aswan/security.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/simplified_functions.py` & `aswan-0.5.9/aswan/simplified_functions.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/godel_src/app.py` & `aswan-0.5.9/aswan/tests/godel_src/app.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/godel_src/handlers.py` & `aswan-0.5.9/aswan/tests/godel_src/handlers.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/godel_src/test_pages/godel_wiki.html` & `aswan-0.5.9/aswan/tests/godel_src/test_pages/godel_wiki.html`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/godel_src/test_pages/jstest.html` & `aswan-0.5.9/aswan/tests/godel_src/test_pages/jstest.html`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/godel_src/test_pages/jstest_minus.html` & `aswan-0.5.9/aswan/tests/godel_src/test_pages/jstest_minus.html`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/integration/test_godel.py` & `aswan-0.5.9/aswan/tests/integration/test_godel.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/integration/test_godel_load.py` & `aswan-0.5.9/aswan/tests/integration/test_godel_load.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/proxy_src.py` & `aswan-0.5.9/aswan/tests/proxy_src.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/unit/test_conn_session.py` & `aswan-0.5.9/aswan/tests/unit/test_conn_session.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/unit/test_depot.py` & `aswan-0.5.9/aswan/tests/unit/test_depot.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/unit/test_depot_remotes.py` & `aswan-0.5.9/aswan/tests/unit/test_depot_remotes.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/unit/test_metadata_handling.py` & `aswan-0.5.9/aswan/tests/unit/test_metadata_handling.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/unit/test_object_store.py` & `aswan-0.5.9/aswan/tests/unit/test_object_store.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/unit/test_project_class.py` & `aswan-0.5.9/aswan/tests/unit/test_project_class.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/unit/test_simplified_functions.py` & `aswan-0.5.9/aswan/tests/unit/test_simplified_functions.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/tests/unit/test_utils.py` & `aswan-0.5.9/aswan/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/url_handler.py` & `aswan-0.5.9/aswan/url_handler.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/aswan/utils.py` & `aswan-0.5.9/aswan/utils.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/conftest.py` & `aswan-0.5.9/conftest.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/docs/api/aswan.BrowserHandler.rst` & `aswan-0.5.9/docs/api/aswan.BrowserHandler.rst`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/docs/api/aswan.ObjectStore.rst` & `aswan-0.5.9/docs/api/aswan.ObjectStore.rst`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/docs/api/aswan.Project.rst` & `aswan-0.5.9/docs/api/aswan.Project.rst`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/docs/api/aswan.ProxyBase.rst` & `aswan-0.5.9/docs/api/aswan.ProxyBase.rst`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/docs/api/aswan.Statuses.rst` & `aswan-0.5.9/docs/api/aswan.Statuses.rst`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/docs/conf.py` & `aswan-0.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/notebooks/doc-000-intro.ipynb` & `aswan-0.5.9/notebooks/doc-000-intro.ipynb`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/notebooks/doc-001-quickstart.ipynb` & `aswan-0.5.9/notebooks/doc-001-quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/notebooks/imdb-case.ipynb` & `aswan-0.5.9/notebooks/imdb-case.ipynb`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/notebooks/imdb.md` & `aswan-0.5.9/notebooks/imdb.md`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/pyproject.toml` & `aswan-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aswan-0.5.8/PKG-INFO` & `aswan-0.5.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aswan
-Version: 0.5.8
+Version: 0.5.9
 Summary: Data collection manager
 Author-email: Endre Márk Borza <endremborza@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
 Requires-Dist: html5lib
@@ -30,16 +30,15 @@
 
 # aswan
 
 [![Documentation Status](https://readthedocs.org/projects/aswan/badge/?version=latest)](https://aswan.readthedocs.io/en/latest)
 [![codeclimate](https://img.shields.io/codeclimate/maintainability/endremborza/aswan.svg)](https://codeclimate.com/github/endremborza/aswan)
 [![codecov](https://img.shields.io/codecov/c/github/endremborza/aswan)](https://codecov.io/gh/endremborza/aswan)
 [![pypi](https://img.shields.io/pypi/v/aswan.svg)](https://pypi.org/project/aswan/)
-[![DOI](https://zenodo.org/badge/360285787.svg)](https://zenodo.org/badge/latestdoi/360285787)
-
+[![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.7477587.svg)](https://doi.org/10.5281/zenodo.7477587)
 
 collect and organize data into a T1 data depot 
 named after the [Aswan Dam](https://en.wikipedia.org/wiki/Aswan_Dam)
 
 Collect and compress data from the internet for later parsing
 
 - quick, parallel, customizable to collect
```

