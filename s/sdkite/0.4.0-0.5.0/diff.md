# Comparing `tmp/sdkite-0.4.0.tar.gz` & `tmp/sdkite-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkite-0.4.0.tar", last modified: Sun Apr 16 19:04:13 2023, max compression
+gzip compressed data, was "sdkite-0.5.0.tar", last modified: Sun May  7 17:50:13 2023, max compression
```

## Comparing `sdkite-0.4.0.tar` & `sdkite-0.5.0.tar`

### file list

```diff
@@ -1,104 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.957939 sdkite-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-16 19:04:04.000000 sdkite-0.4.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.949939 sdkite-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.949939 sdkite-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-16 19:04:04.000000 sdkite-0.4.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-16 19:04:04.000000 sdkite-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-16 19:04:04.000000 sdkite-0.4.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-16 19:04:04.000000 sdkite-0.4.0/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-16 19:04:04.000000 sdkite-0.4.0/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-16 19:04:04.000000 sdkite-0.4.0/.vscode/env
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-16 19:04:04.000000 sdkite-0.4.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-16 19:04:04.000000 sdkite-0.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-16 19:04:04.000000 sdkite-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 19:04:04.000000 sdkite-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-16 19:04:13.957939 sdkite-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-16 19:04:04.000000 sdkite-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-16 19:04:04.000000 sdkite-0.4.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/docs/src/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/docs/src/css/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/http_auth.md
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/http_engine.md
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/http_replay.md
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/http_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/http_response.md
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/pagination.md
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/typing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-16 19:04:04.000000 sdkite-0.4.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-16 19:04:04.000000 sdkite-0.4.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-16 19:04:04.000000 sdkite-0.4.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-16 19:04:13.957939 sdkite-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      196 2023-04-16 19:04:04.000000 sdkite-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.949939 sdkite-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/src/sdkite/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 19:04:13.000000 sdkite-0.4.0/src/sdkite/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/src/sdkite/http/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/_stringescape.py
--rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/engine_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/engine_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/src/sdkite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-16 19:04:13.000000 sdkite-0.4.0/src/sdkite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-16 19:04:13.000000 sdkite-0.4.0/src/sdkite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:04:13.000000 sdkite-0.4.0/src/sdkite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-16 19:04:13.000000 sdkite-0.4.0/src/sdkite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 19:04:13.000000 sdkite-0.4.0/src/sdkite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/tests/integration/recorded/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/recorded/public_version.json
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/recorded/users_1337.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/recorded/users_all_1.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/recorded/users_all_2.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/recorded/users_all_3.json
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/test_adapter_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/test_http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.957939 sdkite-0.4.0/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.957939 sdkite-0.4.0/tests/unit/http/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.949939 sdkite-0.4.0/tests/unit/http/engine_replay/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.957939 sdkite-0.4.0/tests/unit/http/engine_replay/base/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/base/get_foo.json
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/base/get_root.json
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/base/post_encoding.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.957939 sdkite-0.4.0/tests/unit/http/engine_replay/base/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/base/subfolder/in_subfolder.json
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/base/wrong_ext.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.957939 sdkite-0.4.0/tests/unit/http/engine_replay/extra/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/extra/get_bar.json
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/extra/get_foo.json
--rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_adapter_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_adapter_adapter_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_engine_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_engine_replay_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_engine_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_model_httpheaderdict.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_stringescape.py
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_utils_encode_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_utils_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16119 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/test_pagination_pep570.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-16 19:04:04.000000 sdkite-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.438433 sdkite-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-07 17:50:08.000000 sdkite-0.5.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.426432 sdkite-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.430432 sdkite-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-07 17:50:08.000000 sdkite-0.5.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-07 17:50:08.000000 sdkite-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-07 17:50:08.000000 sdkite-0.5.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-07 17:50:08.000000 sdkite-0.5.0/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 17:50:08.000000 sdkite-0.5.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.430432 sdkite-0.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-07 17:50:08.000000 sdkite-0.5.0/.vscode/env
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-07 17:50:08.000000 sdkite-0.5.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-07 17:50:08.000000 sdkite-0.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-07 17:50:08.000000 sdkite-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 17:50:08.000000 sdkite-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-07 17:50:13.438433 sdkite-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-07 17:50:08.000000 sdkite-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-07 17:50:08.000000 sdkite-0.5.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.430432 sdkite-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.430432 sdkite-0.5.0/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/src/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.430432 sdkite-0.5.0/docs/src/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/src/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/src/http_auth.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/src/http_engine.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/src/http_replay.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/src/http_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/src/http_response.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/src/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/src/pagination.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/src/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-07 17:50:08.000000 sdkite-0.5.0/docs/src/typing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-07 17:50:08.000000 sdkite-0.5.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-07 17:50:08.000000 sdkite-0.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-07 17:50:08.000000 sdkite-0.5.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-07 17:50:13.438433 sdkite-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      196 2023-05-07 17:50:08.000000 sdkite-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.426432 sdkite-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.434432 sdkite-0.5.0/src/sdkite/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 17:50:13.000000 sdkite-0.5.0/src/sdkite/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.434432 sdkite-0.5.0/src/sdkite/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/http/_stringescape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/http/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/http/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/http/engine_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/http/engine_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/http/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/http/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/http/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-07 17:50:08.000000 sdkite-0.5.0/src/sdkite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.434432 sdkite-0.5.0/src/sdkite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-07 17:50:13.000000 sdkite-0.5.0/src/sdkite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-07 17:50:13.000000 sdkite-0.5.0/src/sdkite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 17:50:13.000000 sdkite-0.5.0/src/sdkite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-07 17:50:13.000000 sdkite-0.5.0/src/sdkite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 17:50:13.000000 sdkite-0.5.0/src/sdkite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.434432 sdkite-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.434432 sdkite-0.5.0/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.434432 sdkite-0.5.0/tests/integration/recorded/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/integration/recorded/public_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/integration/recorded/users_1337.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/integration/recorded/users_all_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/integration/recorded/users_all_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/integration/recorded/users_all_3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/integration/test_adapter_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/integration/test_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.434432 sdkite-0.5.0/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.438433 sdkite-0.5.0/tests/unit/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.426432 sdkite-0.5.0/tests/unit/http/engine_replay/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.438433 sdkite-0.5.0/tests/unit/http/engine_replay/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/engine_replay/base/get_foo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/engine_replay/base/get_root.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/engine_replay/base/post_encoding.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.438433 sdkite-0.5.0/tests/unit/http/engine_replay/base/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/engine_replay/base/subfolder/in_subfolder.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/engine_replay/base/wrong_ext.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:50:13.438433 sdkite-0.5.0/tests/unit/http/engine_replay/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/engine_replay/extra/get_bar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/engine_replay/extra/get_foo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/test_adapter_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/test_adapter_adapter_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/test_engine_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/test_engine_replay_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/test_engine_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/test_model_httpheaderdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/test_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/test_stringescape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/test_utils_encode_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/test_utils_status_codes_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/http/test_utils_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16119 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/test_pagination_pep570.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-07 17:50:08.000000 sdkite-0.5.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-07 17:50:08.000000 sdkite-0.5.0/tox.ini
```

### Comparing `sdkite-0.4.0/.github/workflows/build.yml` & `sdkite-0.5.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/.vscode/settings.json` & `sdkite-0.5.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/CHANGELOG.md` & `sdkite-0.5.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,34 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/), and this project
 adheres to [Semantic Versioning](https://semver.org/).
 
+## [0.5.0] - 2023-05-07
+
+[0.5.0]: https://github.com/rogdham/sdkite/compare/v0.4.0...v0.5.0
+
+v0.5.0 works on unexpected cases: exceptions & HTTP status codes
+
+### :boom: Breaking changes
+
+- By default, an exception is raised when an HTTP responses has a non-200 status codes
+- All exceptions raised by HTTP engines are now instances of `HTTPError`
+
+### :rocket: Added
+
+- Allow to specify expected status codes of HTTP responses with the
+  `expected_status_codes` parameter
+- The response returned by HTTP engines can be used as a context manager; in that case,
+  exceptions happening within the context manager are re-raised though
+  `HTTPContextError`, which gives the context in which the exception ocurred; this is
+  also useful to clean resources for certain HTTP engines
+
 ## [0.4.0] - 2023-04-16
 
 [0.4.0]: https://github.com/rogdham/sdkite/compare/v0.3.0...v0.4.0
 
 v0.4.0 introduces request retrying and timeout
 
 ### :boom: Breaking changes
```

### Comparing `sdkite-0.4.0/LICENSE.txt` & `sdkite-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/PKG-INFO` & `sdkite-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkite
-Version: 0.4.0
+Version: 0.5.0
 Summary: Simple framework for building SDKs and API clients
 Home-page: https://github.com/rogdham/sdkite
 Author: Rogdham
 Author-email: contact@rogdham.net
 License: MIT
 Project-URL: Documentation, https://sdkite.rogdham.net/
 Project-URL: Source, https://github.com/rogdham/sdkite
@@ -59,15 +59,16 @@
 
 - [x] Minimal documentation
 - [ ] Complete documentation
 - [ ] Improve HTTP adapter
   - [x] Support for more request body types (basic types)
   - [ ] Support for even more request body types (files, iterables)
   - [x] Handle retrying
-  - [ ] Handle _bad_ status codes
+  - [x] Handle _bad_ status codes
   - [x] Builtin auth handlers like basic auth
   - [x] Usual shortcuts like `.get(...)` for `.request('get', ...)`
   - [ ] Allow to disable interceptors on a specific request
-  - [ ] Wrapt `requests`' exceptions
+  - [x] Wrapt `requests`' exceptions
   - [ ] Support more HTTP adapters
+  - [ ] Real end-to-end integration test for HTTP endpoints
 - [ ] Remove `requests` from dependencies
 - [ ] And more!
```

### Comparing `sdkite-0.4.0/README.md` & `sdkite-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 - [x] Minimal documentation
 - [ ] Complete documentation
 - [ ] Improve HTTP adapter
   - [x] Support for more request body types (basic types)
   - [ ] Support for even more request body types (files, iterables)
   - [x] Handle retrying
-  - [ ] Handle _bad_ status codes
+  - [x] Handle _bad_ status codes
   - [x] Builtin auth handlers like basic auth
   - [x] Usual shortcuts like `.get(...)` for `.request('get', ...)`
   - [ ] Allow to disable interceptors on a specific request
-  - [ ] Wrapt `requests`' exceptions
+  - [x] Wrapt `requests`' exceptions
   - [ ] Support more HTTP adapters
+  - [ ] Real end-to-end integration test for HTTP endpoints
 - [ ] Remove `requests` from dependencies
 - [ ] And more!
```

### Comparing `sdkite-0.4.0/docs/conftest.py` & `sdkite-0.5.0/docs/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Dict, Iterator, List, Optional, Tuple, cast
 
 import pytest
 from requests_mock import Mocker
 
 from sdkite import Client
 from sdkite.http import HTTPRequest, HTTPResponse
+import sdkite.http.adapter as adapter_module
 
 
 @pytest.fixture(scope="module", autouse=True)
 def _import_pytest(doctest_namespace: Dict[str, object]) -> None:
     doctest_namespace["Iterator"] = Iterator
     doctest_namespace["Path"] = Path
 
@@ -64,14 +65,19 @@
     #
     requests_mock.register_uri(
         "GET",
         "https://api.example.com/world/npc/interact?name=ranis",
         text="Have you found the Telvanni spy?",
     )
     requests_mock.register_uri(
+        "GET",
+        "https://api.example.com/world/npc/interact?name=waldo",
+        status_code=404,
+    )
+    requests_mock.register_uri(
         "POST",
         "https://api.example.com/world/npc/search",
         additional_matcher=lambda request: cast(
             bool,
             request.json() == {"city": "Balmora", "faction": "Mage", "min_level": 8},
         ),
         json=["marayn", "masalinie", "ranis"],
@@ -95,14 +101,28 @@
     requests_mock.register_uri(
         "GET",
         "https://api.example.com/noauth",
         additional_matcher=lambda request: "Authorization" not in request.headers,
         text="The /noauth endpoint has been called without auth",
     )
 
+    #
+    # http_response
+    #
+    requests_mock.register_uri(
+        "GET",
+        "https://api.example.com/user/1",
+        json={"name": "Alice", "age": 42},
+    )
+    requests_mock.register_uri(
+        "GET",
+        "https://api.example.com/user/2",
+        json={"name": "Bob"},
+    )
+
 
 @pytest.fixture(autouse=True)
 def _create_replay_store(tmp_path: Path) -> None:
     store = tmp_path / "replay"
     store.mkdir()
     (store / "ping.json").write_bytes(
         rb"""{
@@ -127,7 +147,14 @@
 def _change_directory(tmp_path: Path) -> Iterator[None]:
     cwd = getcwd()
     try:
         chdir(tmp_path)
         yield
     finally:
         chdir(cwd)
+
+
+@pytest.fixture(autouse=True)
+def _patched_adapter(monkeypatch: pytest.MonkeyPatch) -> None:
+    # change default value for faster tests
+    monkeypatch.setattr(adapter_module, "_DEFAULT_WAIT_INITIAL", 0)
+    monkeypatch.setattr(adapter_module, "_DEFAULT_WAIT_JITTER", 0)
```

### Comparing `sdkite-0.4.0/docs/mkdocs.yml` & `sdkite-0.5.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/docs/src/css/extra.css` & `sdkite-0.5.0/docs/src/css/extra.css`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/docs/src/http_auth.md` & `sdkite-0.5.0/docs/src/http_auth.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/docs/src/http_engine.md` & `sdkite-0.5.0/docs/src/http_engine.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/docs/src/http_replay.md` & `sdkite-0.5.0/docs/src/http_replay.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/docs/src/http_request.md` & `sdkite-0.5.0/docs/src/http_request.md`

 * *Files 24% similar despite different names*

```diff
@@ -60,20 +60,40 @@
 The later values override the former ones, in a case-insensitive manner.
 
 !!! Note
 
     Depending on the `body_encoding` value, a `content-type` header may be automatically
     added.
 
+## Expected status codes
+
+The `expected_status_codes` parameter allows to specify which status codes are expected
+to be returned in the HTTP response. An `HTTPStatusCodeError` if the value in the
+response is unexpected.
+
+This argument can be:
+
+- An `int` (e.g. `204`)
+- A `str` where the character `x` means “any digit” (e.g. `"2xx"`)
+- An iterable of the previous items (e.g. `("2xx", 404)`)
+
+!!! Warning
+
+    By default, only the `200` status code is considered expected.
+
+    In contrast, other libraries such as [requests](https://github.com/psf/requests)
+    consider only status codes `4xx` and `5xx` to be unexpected.
+
 ## Stream mode
 
 To ask the server to stream the response, set the `stream_response` parameter to `True`.
 
 It is then recommended to use the `data_stream` attribute of
-[the response object](http_response.md).
+[the response object](http_response.md#attributes) and to use it
+[as a context manager](http_response.md#usage-as-a-context-manager).
 
 ## Retry options
 
 If an exception is raised when performing the request, 2 more attempts will be made with
 some wait time between them.
 
 This can be customized by passing some arguments:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sdkite-0.4.0/docs/src/index.md` & `sdkite-0.5.0/docs/src/index.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/docs/src/pagination.md` & `sdkite-0.5.0/docs/src/pagination.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/docs/src/quickstart.md` & `sdkite-0.5.0/docs/src/quickstart.md`

 * *Files 7% similar despite different names*

```diff
@@ -82,16 +82,24 @@
     ...         self._auth.password = password
 
     >>> world = World("Nerevarine", "Incarnate")
 
     >>> world.npc.interact("ranis")
     'Have you found the Telvanni spy?'
 
+    >>> world.npc.interact("waldo")
+    Traceback (most recent call last):
+        ...
+    sdkite.http.exceptions.HTTPStatusCodeError: Unexpected status code: 404
+
     >>> path = Path("book.txt")
     >>> world.book.download("bk_words_of_the_wind", path)
     >>> path.read_text()[:18]
     'Words of the Wind\n'
 
 - Sub-clients are used to group endpoints together, and are automatically instantiated
+- [Status codes are checked](http_request.md#expected-status-codes) and an exception is
+  raised on missmatch (only `200` is allowed by default)
 - [Basic authentication](http_auth.md) is set up on the root client, to be used on all
   sub-clients
-- Response streaming is used to store the content of a book into a file
+- [Response streaming](http_request.md#stream-mode) is used to store the content of a
+  book into a file
```

### Comparing `sdkite-0.4.0/docs/src/typing.md` & `sdkite-0.5.0/docs/src/typing.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/mypy.ini` & `sdkite-0.5.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/ruff.toml` & `sdkite-0.5.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/setup.cfg` & `sdkite-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/src/sdkite/adapter.py` & `sdkite-0.5.0/src/sdkite/adapter.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/src/sdkite/client.py` & `sdkite-0.5.0/src/sdkite/client.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/src/sdkite/http/__init__.py` & `sdkite-0.5.0/src/sdkite/http/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 from sdkite.http.adapter import HTTPAdapter, HTTPAdapterSendRequest, HTTPAdapterSpec
 from sdkite.http.auth import BasicAuth, NoAuth
+from sdkite.http.exceptions import (
+    HTTPConnectionError,
+    HTTPContextError,
+    HTTPError,
+    HTTPStatusCodeError,
+    HTTPTimeoutError,
+)
 from sdkite.http.model import (
     HTTPBodyEncoding,
     HTTPHeaderDict,
     HTTPRequest,
     HTTPRequestAttemptInfo,
     HTTPResponse,
 )
@@ -12,14 +19,20 @@
     # sdkite.http.adapter
     "HTTPAdapter",
     "HTTPAdapterSendRequest",
     "HTTPAdapterSpec",
     # sdkite.http.auth
     "BasicAuth",
     "NoAuth",
+    # sdkite.http.exceptions
+    "HTTPConnectionError",
+    "HTTPContextError",
+    "HTTPError",
+    "HTTPStatusCodeError",
+    "HTTPTimeoutError",
     # sdkite.http.model
     "HTTPBodyEncoding",
     "HTTPHeaderDict",
     "HTTPRequest",
     "HTTPRequestAttemptInfo",
     "HTTPResponse",
 )
```

### Comparing `sdkite-0.4.0/src/sdkite/http/_stringescape.py` & `sdkite-0.5.0/src/sdkite/http/_stringescape.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/src/sdkite/http/adapter.py` & `sdkite-0.5.0/src/sdkite/http/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from copy import deepcopy
 from dataclasses import dataclass
 from functools import partial
 from inspect import BoundArguments, signature
 import sys
-from typing import Any, Dict, List, Optional, Set, Tuple, TypeVar
+from typing import Any, Dict, List, Optional, Set, Tuple, TypeVar, Union
 import warnings
 
 from tenacity import (
     RetryCallState,
     Retrying,
     stop_after_attempt,
     wait_exponential_jitter,
 )
 
 from sdkite import Adapter, AdapterSpec
 from sdkite.http.engine_requests import HTTPEngineRequests
+from sdkite.http.exceptions import HTTPStatusCodeError
 from sdkite.http.model import (
     HTTPBodyEncoding,
     HTTPHeaderDict,
     HTTPRequest,
     HTTPRequestAttemptInfo,
     HTTPResponse,
 )
-from sdkite.http.utils import encode_request_body, urlsjoin
+from sdkite.http.utils import build_status_code_check, encode_request_body, urlsjoin
 from sdkite.utils import last_not_none, zip_reverse
 
 if sys.version_info < (3, 8):  # pragma: no cover
     from typing_extensions import Literal, Protocol
 else:  # pragma: no cover
     from typing import Literal, Protocol
 
 if sys.version_info < (3, 9):  # pragma: no cover
-    from typing import Callable, Mapping
+    from typing import Callable, Iterable, Mapping
 else:  # pragma: no cover
-    from collections.abc import Callable, Mapping
+    from collections.abc import Callable, Iterable, Mapping
 
 if sys.version_info < (3, 10):  # pragma: no cover
     from typing_extensions import ParamSpec
 else:  # pragma: no cover
     from typing import ParamSpec
 
 
@@ -58,14 +59,15 @@
         self,
         url: Optional[str] = None,
         *,
         body: object = None,
         body_encoding: HTTPBodyEncoding = HTTPBodyEncoding.AUTO,
         headers: Optional[Mapping[str, str]] = None,
         stream_response: bool = False,
+        expected_status_codes: Union[int, str, Iterable[Union[int, str]]] = 200,
     ) -> HTTPResponse:
         ...
 
 
 class _HTTPAdapterRequestWithoutMethod:
     name: str
 
@@ -131,20 +133,23 @@
         method: str,
         url: Optional[str] = None,
         *,
         body: object = None,
         body_encoding: HTTPBodyEncoding = HTTPBodyEncoding.AUTO,
         headers: Optional[Mapping[str, str]] = None,
         stream_response: bool = False,
+        expected_status_codes: Union[int, str, Iterable[Union[int, str]]] = 200,
         retry_nb_attempts: Optional[int] = None,
         retry_callback: Optional[Callable[[HTTPRequestAttemptInfo], None]] = None,
         retry_wait_initial: Optional[float] = None,
         retry_wait_max: Optional[float] = None,
         retry_wait_jitter: Optional[float] = None,
     ) -> HTTPResponse:
+        check_status_code = build_status_code_check(expected_status_codes)
+
         #
         # create request
         #
 
         # method
         method = method.upper()
 
@@ -229,14 +234,25 @@
                 # send request
                 response = self._send_request(request)
 
                 # response interceptors
                 for interceptor in self._get_interceptors("response_interceptor"):
                     response = interceptor(response, self)
 
+                # status code check
+                if not check_status_code(response.status_code):
+                    raise HTTPStatusCodeError(
+                        status_code=response.status_code,
+                        request=initial_request,
+                        response=response,
+                    )
+
+        response._set_context(  # pylint: disable=protected-access)  # noqa: SLF001
+            initial_request
+        )
         return response
 
     def _get_interceptors(
         self,
         kind: Literal["request_interceptor", "response_interceptor"],
     ) -> List[Callable[[T, "HTTPAdapter"], T]]:
         seen_names: Set[str] = set()
```

### Comparing `sdkite-0.4.0/src/sdkite/http/auth.py` & `sdkite-0.5.0/src/sdkite/http/auth.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/src/sdkite/http/engine_replay.py` & `sdkite-0.5.0/src/sdkite/http/engine_replay.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,25 +189,25 @@
         # recording mode
         if self.recording:
             # perform request
             if self.engine is None:
                 self.engine = HTTPEngineRequests()
 
             real_request = self.recording_request_modifier(deepcopy(request))
-            real_response = self.engine(real_request)
-            received_response = HTTPResponseReplay(
-                _RecordedResponse(
-                    status_code=real_response.status_code,
-                    reason=real_response.reason,
-                    headers=dict(real_response.headers),
-                    body=list(real_response.data_stream)
-                    if real_request.stream_response
-                    else [real_response.data_bytes],
+            with self.engine(real_request) as real_response:
+                received_response = HTTPResponseReplay(
+                    _RecordedResponse(
+                        status_code=real_response.status_code,
+                        reason=real_response.reason,
+                        headers=dict(real_response.headers),
+                        body=list(real_response.data_stream)
+                        if real_request.stream_response
+                        else [real_response.data_bytes],
+                    )
                 )
-            )
             response = self.recording_response_modifier(received_response)
 
             # save recorded response
             recorded_basename = self.recording_compute_basename(request, response)
             recorded_path = self.recording_path_dir / f"{recorded_basename}.json"
             with recorded_path.open("w") as recorded_fp:
                 json.dump(
```

### Comparing `sdkite-0.4.0/src/sdkite/http/model.py` & `sdkite-0.5.0/src/sdkite/http/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from abc import ABC, abstractmethod
+from contextlib import suppress
 from dataclasses import dataclass
 from enum import Enum, auto, unique
 import sys
-from typing import Dict, List, Tuple, Union
+from types import TracebackType
+from typing import Dict, List, Optional, Tuple, Type, Union
+
+from sdkite.http.exceptions import HTTPContextError
 
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import Iterable, Iterator, Mapping, MutableMapping
 else:  # pragma: no cover
     from collections.abc import Iterable, Iterator, Mapping, MutableMapping
 
+if sys.version_info < (3, 11):  # pragma: no cover
+    from typing_extensions import Self
+else:  # pragma: no cover
+    from typing import Self
+
 
 class HTTPHeaderDict(MutableMapping[str, str]):
     __slots__ = ["_contents"]
 
     def __init__(
         self,
         items: Union[None, Mapping[str, str], Iterable[Tuple[str, str]]] = None,
@@ -69,14 +78,16 @@
     url: str
     headers: HTTPHeaderDict
     body: Union[bytes, Iterator[bytes]]
     stream_response: bool
 
 
 class HTTPResponse(ABC):
+    __context: Optional[HTTPRequest] = None
+
     @property
     @abstractmethod
     def raw(self) -> object:
         """
         The response object coming from the adapter
         """
 
@@ -125,14 +136,42 @@
     @property
     @abstractmethod
     def data_json(self) -> object:
         """
         The body of the response JSON-decoded, for easier access.
         """
 
+    def _close(self) -> None:  # noqa: B027
+        pass
+
+    def _set_context(self, context: HTTPRequest) -> None:
+        self.__context = context
+
+    def __enter__(self) -> Self:
+        return self
+
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> None:
+        with suppress(Exception):
+            self._close()
+        if exc_val and self.__context:
+            raise HTTPContextError.from_exception(
+                exc_val,
+                request=self.__context,
+                response=self,
+            ) from exc_val
+
+    def __del__(self) -> None:
+        with suppress(Exception):
+            self._close()
+
 
 @dataclass
 class HTTPRequestAttemptInfo:
     attempt_number: int
     exception: BaseException
     initial_request: HTTPRequest
     seconds_since_start: float
```

### Comparing `sdkite-0.4.0/src/sdkite/http/utils.py` & `sdkite-0.5.0/src/sdkite/http/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from contextlib import contextmanager
 from functools import reduce
 import json
+import re
 import secrets
 import sys
-from typing import Optional, Tuple, Union
+from typing import Optional, Set, Tuple, Union
 from urllib.parse import quote_plus
 from urllib.parse import urljoin as _urljoin
 
 from sdkite.http.model import HTTPBodyEncoding
 
 if sys.version_info < (3, 9):  # pragma: no cover
-    from typing import Iterable, Iterator
+    from typing import Callable, Iterable, Iterator
 else:  # pragma: no cover
-    from collections.abc import Iterable, Iterator
+    from collections.abc import Callable, Iterable, Iterator
 
 if sys.version_info < (3, 10):  # pragma: no cover
     NoneType = type(None)
 else:  # pragma: no cover
     from types import NoneType
 
 
@@ -311,7 +312,36 @@
         if ex.path:
             error_msg += f" ({'>'.join(ex.path)})"
         error_msg += f" of type '{type(ex.obj).__name__}'"
         error_msg += f" with '{original_encoding.name}' encoding"
         raise TypeError(error_msg) from None
 
     return data, content_type
+
+
+_SINGLE_STATUS_CODE_PATTERN = re.compile(r"^[0-9x]{3}$")
+
+
+def build_status_code_check(
+    status_codes: Union[int, str, Iterable[Union[int, str]]]
+) -> Callable[[int], bool]:
+    if isinstance(status_codes, (int, str)):
+        status_codes = (status_codes,)
+
+    parts: Set[str] = set()
+    for status_code in status_codes:
+        if isinstance(status_code, int):
+            status_code = f"{status_code:03d}"  # noqa: PLW2901
+        if _SINGLE_STATUS_CODE_PATTERN.match(status_code):
+            parts.add(status_code.replace("x", "[0-9]"))
+        else:
+            raise ValueError(
+                f"Invalid status code (must match /{_SINGLE_STATUS_CODE_PATTERN.pattern}/)"
+                f": {status_code}"
+            )
+
+    pattern = re.compile(f"^{'|'.join(sorted(parts))}$")
+
+    def status_code_check(code: int) -> bool:
+        return bool(pattern.match(f"{code:03d}"))
+
+    return status_code_check
```

### Comparing `sdkite-0.4.0/src/sdkite/pagination.py` & `sdkite-0.5.0/src/sdkite/pagination.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/src/sdkite.egg-info/PKG-INFO` & `sdkite-0.5.0/src/sdkite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkite
-Version: 0.4.0
+Version: 0.5.0
 Summary: Simple framework for building SDKs and API clients
 Home-page: https://github.com/rogdham/sdkite
 Author: Rogdham
 Author-email: contact@rogdham.net
 License: MIT
 Project-URL: Documentation, https://sdkite.rogdham.net/
 Project-URL: Source, https://github.com/rogdham/sdkite
@@ -59,15 +59,16 @@
 
 - [x] Minimal documentation
 - [ ] Complete documentation
 - [ ] Improve HTTP adapter
   - [x] Support for more request body types (basic types)
   - [ ] Support for even more request body types (files, iterables)
   - [x] Handle retrying
-  - [ ] Handle _bad_ status codes
+  - [x] Handle _bad_ status codes
   - [x] Builtin auth handlers like basic auth
   - [x] Usual shortcuts like `.get(...)` for `.request('get', ...)`
   - [ ] Allow to disable interceptors on a specific request
-  - [ ] Wrapt `requests`' exceptions
+  - [x] Wrapt `requests`' exceptions
   - [ ] Support more HTTP adapters
+  - [ ] Real end-to-end integration test for HTTP endpoints
 - [ ] Remove `requests` from dependencies
 - [ ] And more!
```

### Comparing `sdkite-0.4.0/src/sdkite.egg-info/SOURCES.txt` & `sdkite-0.5.0/src/sdkite.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,28 +30,30 @@
 docs/src/quickstart.md
 docs/src/typing.md
 docs/src/css/extra.css
 src/sdkite/__init__.py
 src/sdkite/_version.py
 src/sdkite/adapter.py
 src/sdkite/client.py
+src/sdkite/exceptions.py
 src/sdkite/pagination.py
 src/sdkite/py.typed
 src/sdkite/utils.py
 src/sdkite.egg-info/PKG-INFO
 src/sdkite.egg-info/SOURCES.txt
 src/sdkite.egg-info/dependency_links.txt
 src/sdkite.egg-info/requires.txt
 src/sdkite.egg-info/top_level.txt
 src/sdkite/http/__init__.py
 src/sdkite/http/_stringescape.py
 src/sdkite/http/adapter.py
 src/sdkite/http/auth.py
 src/sdkite/http/engine_replay.py
 src/sdkite/http/engine_requests.py
+src/sdkite/http/exceptions.py
 src/sdkite/http/model.py
 src/sdkite/http/utils.py
 tests/conftest.py
 tests/integration/test_adapter_simple.py
 tests/integration/test_http.py
 tests/integration/recorded/public_version.json
 tests/integration/recorded/users_1337.json
@@ -67,16 +69,18 @@
 tests/unit/http/test_adapter_adapter.py
 tests/unit/http/test_adapter_adapter_spec.py
 tests/unit/http/test_auth.py
 tests/unit/http/test_engine_replay.py
 tests/unit/http/test_engine_replay_recording.py
 tests/unit/http/test_engine_requests.py
 tests/unit/http/test_model_httpheaderdict.py
+tests/unit/http/test_model_response.py
 tests/unit/http/test_stringescape.py
 tests/unit/http/test_utils_encode_request_body.py
+tests/unit/http/test_utils_status_codes_check.py
 tests/unit/http/test_utils_url.py
 tests/unit/http/engine_replay/base/get_foo.json
 tests/unit/http/engine_replay/base/get_root.json
 tests/unit/http/engine_replay/base/post_encoding.json
 tests/unit/http/engine_replay/base/wrong_ext.txt
 tests/unit/http/engine_replay/base/subfolder/in_subfolder.json
 tests/unit/http/engine_replay/extra/get_bar.json
```

### Comparing `sdkite-0.4.0/tests/conftest.py` & `sdkite-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/integration/test_adapter_simple.py` & `sdkite-0.5.0/tests/integration/test_adapter_simple.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/integration/test_http.py` & `sdkite-0.5.0/tests/integration/test_http.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/http/engine_replay/base/post_encoding.json` & `sdkite-0.5.0/tests/unit/http/engine_replay/base/post_encoding.json`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/http/test_adapter_adapter_spec.py` & `sdkite-0.5.0/tests/unit/http/test_adapter_adapter_spec.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/http/test_auth.py` & `sdkite-0.5.0/tests/unit/http/test_auth.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/http/test_engine_replay.py` & `sdkite-0.5.0/tests/unit/http/test_engine_replay.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/http/test_engine_replay_recording.py` & `sdkite-0.5.0/tests/unit/http/test_engine_replay_recording.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 import time
 from typing import Set
 
 import pytest
 from requests_mock import Mocker, NoMockAddress
 
-from sdkite.http import HTTPHeaderDict, HTTPRequest
+from sdkite.http import HTTPError, HTTPHeaderDict, HTTPRequest
 from sdkite.http.engine_replay import HTTPEngineReplay, HTTPResponseReplay
 
 REPLAY_PATH = Path(__file__).parent / "engine_replay"
 
 
 @pytest.fixture(autouse=True)
 def _patched_time(monkeypatch: pytest.MonkeyPatch) -> None:
@@ -142,18 +142,21 @@
         method="GET",
         url="https://example.com/",
         headers=HTTPHeaderDict(),
         body=b"",
         stream_response=False,
     )
     with pytest.raises(
-        NoMockAddress,
-        match=re.escape("No mock address: GET https://example.com/"),
-    ):
+        HTTPError,
+        match=re.escape("NoMockAddress: No mock address: GET https://example.com/"),
+    ) as excinfo:
         response = engine(request)
+    assert (  # pylint: disable=unidiomatic-typecheck
+        type(excinfo.value.__context__) is NoMockAddress
+    )
 
 
 @pytest.mark.parametrize("recording", [True, False])
 def test_recording_modifiers(
     tmp_path: Path, requests_mock: Mocker, recording: bool
 ) -> None:
     expected_recording = rb"""{
```

### Comparing `sdkite-0.4.0/tests/unit/http/test_engine_requests.py` & `sdkite-0.5.0/tests/unit/http/test_engine_requests.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/http/test_model_httpheaderdict.py` & `sdkite-0.5.0/tests/unit/http/test_model_httpheaderdict.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/http/test_stringescape.py` & `sdkite-0.5.0/tests/unit/http/test_stringescape.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/http/test_utils_encode_request_body.py` & `sdkite-0.5.0/tests/unit/http/test_utils_encode_request_body.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/http/test_utils_url.py` & `sdkite-0.5.0/tests/unit/http/test_utils_url.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/test_adapter.py` & `sdkite-0.5.0/tests/unit/test_adapter.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/test_client.py` & `sdkite-0.5.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/test_pagination.py` & `sdkite-0.5.0/tests/unit/test_pagination.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tests/unit/test_pagination_pep570.py` & `sdkite-0.5.0/tests/unit/test_pagination_pep570.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.4.0/tox.ini` & `sdkite-0.5.0/tox.ini`

 * *Files identical despite different names*

