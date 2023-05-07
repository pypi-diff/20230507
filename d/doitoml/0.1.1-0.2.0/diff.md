# Comparing `tmp/doitoml-0.1.1.tar.gz` & `tmp/doitoml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doitoml-0.1.1.tar", last modified: Tue May  2 14:10:48 2023, max compression
+gzip compressed data, was "doitoml-0.2.0.tar", last modified: Sun May  7 21:39:34 2023, max compression
```

## Comparing `doitoml-0.1.1.tar` & `doitoml-0.2.0.tar`

### file list

```diff
@@ -1,140 +1,170 @@
--rw-r--r--   0        0        0     1064 2023-05-02 14:10:48.000000 doitoml-0.1.1/.binder/environment.yml
--rw-r--r--   0        0        0       79 2023-05-02 14:10:48.000000 doitoml-0.1.1/.binder/postBuild
--rw-r--r--   0        0        0      851 2023-05-02 14:10:48.000000 doitoml-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      645 2023-05-02 14:10:48.000000 doitoml-0.1.1/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0        0        0      487 2023-05-02 14:10:48.000000 doitoml-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      926 2023-05-02 14:10:48.000000 doitoml-0.1.1/.github/ISSUE_TEMPLATE/release.md
--rw-r--r--   0        0        0      503 2023-05-02 14:10:48.000000 doitoml-0.1.1/.github/environment.yml
--rw-r--r--   0        0        0      845 2023-05-02 14:10:48.000000 doitoml-0.1.1/.github/pull_request_template.md
--rw-r--r--   0        0        0      140 2023-05-02 14:10:48.000000 doitoml-0.1.1/.github/reqs/build.txt
--rw-r--r--   0        0        0     1258 2023-05-02 14:10:48.000000 doitoml-0.1.1/.github/workflows/badges.yml
--rw-r--r--   0        0        0     5554 2023-05-02 14:10:48.000000 doitoml-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      115 2023-05-02 14:10:48.000000 doitoml-0.1.1/.gitignore
--rw-r--r--   0        0        0      297 2023-05-02 14:10:48.000000 doitoml-0.1.1/.readthedocs.yml
--rw-r--r--   0        0        0       72 2023-05-02 14:10:48.000000 doitoml-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      690 2023-05-02 14:10:48.000000 doitoml-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1500 2023-05-02 14:10:48.000000 doitoml-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     4638 2023-05-02 14:10:48.000000 doitoml-0.1.1/README.md
--rw-r--r--   0        0        0     3869 2023-05-02 14:10:48.000000 doitoml-0.1.1/_actions.py
--rw-r--r--   0        0        0      923 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/_static/css/theme.css
--rw-r--r--   0        0        0     1175 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/_static/img/anvil.svg
--rw-r--r--   0        0        0     5087 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/_static/img/logo.svg
--rw-r--r--   0        0        0     2345 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/_static/js/mermaid.mjs
--rw-r--r--   0        0        0      404 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/_templates/mermaid10.html
--rw-r--r--   0        0        0     3299 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/conf.py
--rw-r--r--   0        0        0      539 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/environment.yml
--rw-r--r--   0        0        0     3298 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/how-to/dsl.md
--rw-r--r--   0        0        0      106 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/how-to/index.md
--rw-r--r--   0        0        0     1458 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/how-to/logging.md
--rw-r--r--   0        0        0     1750 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/how-to/templates.md
--rw-r--r--   0        0        0     3289 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/how-to/user-python.md
--rw-r--r--   0        0        0      779 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/index.md
--rw-r--r--   0        0        0     2762 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/reference/api.md
--rw-r--r--   0        0        0       37 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/reference/changelog.md
--rw-r--r--   0        0        0     6282 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/reference/cheatsheet.md
--rw-r--r--   0        0        0      127 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/reference/index.md
--rw-r--r--   0        0        0       47 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/reference/license.md
--rw-r--r--   0        0        0       84 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/reference/schema.md
--rw-r--r--   0        0        0    10467 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/tutorials/getting-started.ipynb
--rw-r--r--   0        0        0       91 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/tutorials/index.md
--rw-r--r--   0        0        0       40 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/understanding/contributing.md
--rw-r--r--   0        0        0     3153 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/understanding/doit-good.md
--rw-r--r--   0        0        0     2095 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/understanding/extending.md
--rw-r--r--   0        0        0      119 2023-05-02 14:10:48.000000 doitoml-0.1.1/docs/understanding/index.md
--rw-r--r--   0        0        0      817 2023-05-02 14:10:48.000000 doitoml-0.1.1/dodo.py
--rw-r--r--   0        0        0        7 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/no-dodo-js/.gitignore
--rw-r--r--   0        0        0      182 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/no-dodo-js/package.json
--rw-r--r--   0        0        0      283 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/no-dodo-js/pyproject.toml
--rw-r--r--   0        0        0        7 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/no-dodo/.gitignore
--rw-r--r--   0        0        0      376 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/no-dodo/pyproject.toml
--rw-r--r--   0        0        0      122 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/.gitignore
--rw-r--r--   0        0        0        0 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/LICENSE
--rw-r--r--   0        0        0      376 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/README.md
--rw-r--r--   0        0        0     1485 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/_yarn.py
--rw-r--r--   0        0        0      134 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/dodo.py
--rw-r--r--   0        0        0      302 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/environment.yml
--rw-r--r--   0        0        0       43 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/js/index.ts
--rw-r--r--   0        0        0      274 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/js/tsconfig.json
--rw-r--r--   0        0        0        0 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/my_custom/__init__.py
--rw-r--r--   0        0        0     3869 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/my_custom/_actions.py
--rw-r--r--   0        0        0     3202 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/package.json
--rw-r--r--   0        0        0     2931 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/src/example_web/__init__.py
--rw-r--r--   0        0        0      497 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/src/example_web/app.py
--rw-r--r--   0        0        0        0 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/style/index.css
--rw-r--r--   0        0        0      282 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/py-js-web/webpack.config.js
--rw-r--r--   0        0        0       19 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/template-jinja2/.gitignore
--rw-r--r--   0        0        0      505 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/template-jinja2/pyproject.toml
--rw-r--r--   0        0        0       31 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/template-json-e/.gitignore
--rw-r--r--   0        0        0      288 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/template-json-e/README.md
--rw-r--r--   0        0        0     3869 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/template-json-e/_actions.py
--rw-r--r--   0        0        0        4 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/template-json-e/a/README.md
--rw-r--r--   0        0        0       18 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/template-json-e/a/a.py
--rw-r--r--   0        0        0      298 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/template-json-e/a/pyproject.toml
--rw-r--r--   0        0        0        4 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/template-json-e/b/README.md
--rw-r--r--   0        0        0       18 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/template-json-e/b/b.py
--rw-r--r--   0        0        0      298 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/template-json-e/b/pyproject.toml
--rw-r--r--   0        0        0     2904 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/template-json-e/pyproject.toml
--rw-r--r--   0        0        0       13 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/uptodate-py/.gitignore
--rw-r--r--   0        0        0      232 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/uptodate-py/_uptodate.py
--rw-r--r--   0        0        0      806 2023-05-02 14:10:48.000000 doitoml-0.1.1/examples/uptodate-py/pyproject.toml
--rw-r--r--   0        0        0       15 2023-05-02 14:10:48.000000 doitoml-0.1.1/js/.prettierignore
--rw-r--r--   0        0        0     2076 2023-05-02 14:10:48.000000 doitoml-0.1.1/js/package.json
--rw-r--r--   0        0        0     1329 2023-05-02 14:10:48.000000 doitoml-0.1.1/js/yarn.lock
--rw-r--r--   0        0        0    12638 2023-05-02 14:10:48.000000 doitoml-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      188 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/__init__.py
--rw-r--r--   0        0        0      131 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/_version.py
--rw-r--r--   0        0        0       41 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/actors/__init__.py
--rw-r--r--   0        0        0     1280 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/actors/_actor.py
--rw-r--r--   0        0        0     1732 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/actors/py.py
--rw-r--r--   0        0        0    24796 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/config.py
--rw-r--r--   0        0        0     2744 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/constants.py
--rw-r--r--   0        0        0    10280 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/doitoml.py
--rw-r--r--   0        0        0     7488 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/dsl.py
--rw-r--r--   0        0        0     2816 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/entry_points.py
--rw-r--r--   0        0        0     2071 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/errors.py
--rw-r--r--   0        0        0      829 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/loaders.py
--rw-r--r--   0        0        0        0 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/py.typed
--rw-r--r--   0        0        0       39 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/schema/__init__.py
--rw-r--r--   0        0        0     4647 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/schema/_v0.schema.json
--rw-r--r--   0        0        0     2243 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/schema/_v0_schema.py
--rw-r--r--   0        0        0     3085 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/schema/v0.schema.toml
--rw-r--r--   0        0        0     2426 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/schema/validator.py
--rw-r--r--   0        0        0       53 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/sources/__init__.py
--rw-r--r--   0        0        0     3979 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/sources/_config.py
--rw-r--r--   0        0        0     2694 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/sources/_source.py
--rw-r--r--   0        0        0       25 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/sources/json/__init__.py
--rw-r--r--   0        0        0      650 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/sources/json/_json.py
--rw-r--r--   0        0        0     1094 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/sources/json/package.py
--rw-r--r--   0        0        0       20 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/sources/toml/__init__.py
--rw-r--r--   0        0        0      640 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/sources/toml/_toml.py
--rw-r--r--   0        0        0      983 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/sources/toml/pyproject.py
--rw-r--r--   0        0        0       20 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/sources/yaml/__init__.py
--rw-r--r--   0        0        0      749 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/sources/yaml/_yaml.py
--rw-r--r--   0        0        0       38 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/templaters/__init__.py
--rw-r--r--   0        0        0      581 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/templaters/_templater.py
--rw-r--r--   0        0        0     2158 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/templaters/jinja2.py
--rw-r--r--   0        0        0     3032 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/templaters/jsone.py
--rw-r--r--   0        0        0     2929 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/types.py
--rw-r--r--   0        0        0       37 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/updaters/__init__.py
--rw-r--r--   0        0        0      856 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/updaters/_updater.py
--rw-r--r--   0        0        0     2197 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/updaters/doit_tools.py
--rw-r--r--   0        0        0     1567 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/updaters/py.py
--rw-r--r--   0        0        0       42 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/utils/__init__.py
--rw-r--r--   0        0        0      820 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/utils/json.py
--rw-r--r--   0        0        0     1280 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/utils/log.py
--rw-r--r--   0        0        0      371 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/utils/path.py
--rw-r--r--   0        0        0     4734 2023-05-02 14:10:48.000000 doitoml-0.1.1/src/doitoml/utils/py.py
--rw-r--r--   0        0        0       25 2023-05-02 14:10:48.000000 doitoml-0.1.1/test/__init__.py
--rw-r--r--   0        0        0     3708 2023-05-02 14:10:48.000000 doitoml-0.1.1/test/conftest.py
--rw-r--r--   0        0        0     1883 2023-05-02 14:10:48.000000 doitoml-0.1.1/test/test_actors.py
--rw-r--r--   0        0        0     8136 2023-05-02 14:10:48.000000 doitoml-0.1.1/test/test_config.py
--rw-r--r--   0        0        0     2164 2023-05-02 14:10:48.000000 doitoml-0.1.1/test/test_dsl.py
--rw-r--r--   0        0        0     4361 2023-05-02 14:10:48.000000 doitoml-0.1.1/test/test_examples.py
--rw-r--r--   0        0        0      166 2023-05-02 14:10:48.000000 doitoml-0.1.1/test/test_metadata.py
--rw-r--r--   0        0        0      570 2023-05-02 14:10:48.000000 doitoml-0.1.1/test/test_parse_fails.py
--rw-r--r--   0        0        0      501 2023-05-02 14:10:48.000000 doitoml-0.1.1/test/test_schema.py
--rw-r--r--   0        0        0      523 2023-05-02 14:10:48.000000 doitoml-0.1.1/test/test_self.py
--rw-r--r--   0        0        0     2411 2023-05-02 14:10:48.000000 doitoml-0.1.1/test/test_templaters.py
--rw-r--r--   0        0        0     2132 2023-05-02 14:10:48.000000 doitoml-0.1.1/test/test_updaters.py
--rw-r--r--   0        0        0     5987 1970-01-01 00:00:00.000000 doitoml-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1190 2023-05-07 21:39:34.000000 doitoml-0.2.0/.binder/environment.yml
+-rw-r--r--   0        0        0       79 2023-05-07 21:39:34.000000 doitoml-0.2.0/.binder/postBuild
+-rw-r--r--   0        0        0      851 2023-05-07 21:39:34.000000 doitoml-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      645 2023-05-07 21:39:34.000000 doitoml-0.2.0/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0        0        0      487 2023-05-07 21:39:34.000000 doitoml-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      926 2023-05-07 21:39:34.000000 doitoml-0.2.0/.github/ISSUE_TEMPLATE/release.md
+-rw-r--r--   0        0        0      503 2023-05-07 21:39:34.000000 doitoml-0.2.0/.github/environment.yml
+-rw-r--r--   0        0        0      845 2023-05-07 21:39:34.000000 doitoml-0.2.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      140 2023-05-07 21:39:34.000000 doitoml-0.2.0/.github/reqs/build.txt
+-rw-r--r--   0        0        0     1258 2023-05-07 21:39:34.000000 doitoml-0.2.0/.github/workflows/badges.yml
+-rw-r--r--   0        0        0     5554 2023-05-07 21:39:34.000000 doitoml-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      138 2023-05-07 21:39:34.000000 doitoml-0.2.0/.gitignore
+-rw-r--r--   0        0        0      369 2023-05-07 21:39:34.000000 doitoml-0.2.0/.readthedocs.yml
+-rw-r--r--   0        0        0      486 2023-05-07 21:39:34.000000 doitoml-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      690 2023-05-07 21:39:34.000000 doitoml-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1500 2023-05-07 21:39:34.000000 doitoml-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     4638 2023-05-07 21:39:34.000000 doitoml-0.2.0/README.md
+-rw-r--r--   0        0        0     3928 2023-05-07 21:39:34.000000 doitoml-0.2.0/_actions.py
+-rw-r--r--   0        0        0     1159 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/_static/css/theme.css
+-rw-r--r--   0        0        0     1120 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/_static/ideas/doitbot.md
+-rw-r--r--   0        0        0       92 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/_static/ideas/doitdot.md
+-rw-r--r--   0        0        0     1175 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/_static/img/anvil.svg
+-rw-r--r--   0        0        0     5087 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/_static/img/logo.svg
+-rw-r--r--   0        0        0     2345 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/_static/js/mermaid.mjs
+-rw-r--r--   0        0        0      404 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/_templates/mermaid10.html
+-rw-r--r--   0        0        0     3364 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      616 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/demo.md
+-rw-r--r--   0        0        0      736 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/environment.yml
+-rw-r--r--   0        0        0     3495 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/how-to/dsl.md
+-rw-r--r--   0        0        0      106 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/how-to/index.md
+-rw-r--r--   0        0        0     1458 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/how-to/logging.md
+-rw-r--r--   0        0        0     1750 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/how-to/templates.md
+-rw-r--r--   0        0        0     4145 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/how-to/user-python.md
+-rw-r--r--   0        0        0      875 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/index.md
+-rw-r--r--   0        0        0     3176 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/reference/api.md
+-rw-r--r--   0        0        0       37 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/reference/changelog.md
+-rw-r--r--   0        0        0     7983 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/reference/cheatsheet.md
+-rw-r--r--   0        0        0      127 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/reference/index.md
+-rw-r--r--   0        0        0       47 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/reference/license.md
+-rw-r--r--   0        0        0       84 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/reference/schema.md
+-rw-r--r--   0        0        0    10467 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/tutorials/getting-started.ipynb
+-rw-r--r--   0        0        0       91 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/tutorials/index.md
+-rw-r--r--   0        0        0       40 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/understanding/contributing.md
+-rw-r--r--   0        0        0     3153 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/understanding/doit-good.md
+-rw-r--r--   0        0        0     2095 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/understanding/extending.md
+-rw-r--r--   0        0        0      119 2023-05-07 21:39:34.000000 doitoml-0.2.0/docs/understanding/index.md
+-rw-r--r--   0        0        0      817 2023-05-07 21:39:34.000000 doitoml-0.2.0/dodo.py
+-rw-r--r--   0        0        0       31 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/mono/.gitignore
+-rw-r--r--   0        0        0      198 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/mono/README.md
+-rw-r--r--   0        0        0        4 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/mono/a/README.md
+-rw-r--r--   0        0        0       18 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/mono/a/a.py
+-rw-r--r--   0        0        0      670 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/mono/a/pyproject.toml
+-rw-r--r--   0        0        0        4 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/mono/b/README.md
+-rw-r--r--   0        0        0       30 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/mono/b/index.js
+-rw-r--r--   0        0        0      634 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/mono/b/package.json
+-rw-r--r--   0        0        0      654 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/mono/pyproject.toml
+-rw-r--r--   0        0        0        7 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/no-dodo-js/.gitignore
+-rw-r--r--   0        0        0      182 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/no-dodo-js/package.json
+-rw-r--r--   0        0        0      283 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/no-dodo-js/pyproject.toml
+-rw-r--r--   0        0        0        7 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/no-dodo/.gitignore
+-rw-r--r--   0        0        0      376 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/no-dodo/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/LICENSE
+-rw-r--r--   0        0        0      376 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/README.md
+-rw-r--r--   0        0        0     1485 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/_yarn.py
+-rw-r--r--   0        0        0      134 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/dodo.py
+-rw-r--r--   0        0        0      302 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/environment.yml
+-rw-r--r--   0        0        0       43 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/js/index.ts
+-rw-r--r--   0        0        0      274 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/js/tsconfig.json
+-rw-r--r--   0        0        0        0 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/my_custom/__init__.py
+-rw-r--r--   0        0        0     3928 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/my_custom/_actions.py
+-rw-r--r--   0        0        0     3202 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/package.json
+-rw-r--r--   0        0        0     2931 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/src/example_web/__init__.py
+-rw-r--r--   0        0        0      497 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/src/example_web/app.py
+-rw-r--r--   0        0        0        0 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/style/index.css
+-rw-r--r--   0        0        0      282 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/py-js-web/webpack.config.js
+-rw-r--r--   0        0        0       19 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/template-jinja2/.gitignore
+-rw-r--r--   0        0        0      505 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/template-jinja2/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/template-json-e/.gitignore
+-rw-r--r--   0        0        0      288 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/template-json-e/README.md
+-rw-r--r--   0        0        0     3928 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/template-json-e/_actions.py
+-rw-r--r--   0        0        0        4 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/template-json-e/a/README.md
+-rw-r--r--   0        0        0       18 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/template-json-e/a/a.py
+-rw-r--r--   0        0        0      298 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/template-json-e/a/pyproject.toml
+-rw-r--r--   0        0        0        4 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/template-json-e/b/README.md
+-rw-r--r--   0        0        0       18 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/template-json-e/b/b.py
+-rw-r--r--   0        0        0      298 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/template-json-e/b/pyproject.toml
+-rw-r--r--   0        0        0     2904 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/template-json-e/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/uptodate-py/.gitignore
+-rw-r--r--   0        0        0      232 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/uptodate-py/_uptodate.py
+-rw-r--r--   0        0        0      806 2023-05-07 21:39:34.000000 doitoml-0.2.0/examples/uptodate-py/pyproject.toml
+-rw-r--r--   0        0        0       15 2023-05-07 21:39:34.000000 doitoml-0.2.0/js/.prettierignore
+-rw-r--r--   0        0        0     2118 2023-05-07 21:39:34.000000 doitoml-0.2.0/js/package.json
+-rw-r--r--   0        0        0     1329 2023-05-07 21:39:34.000000 doitoml-0.2.0/js/yarn.lock
+-rw-r--r--   0        0        0     7559 2023-05-07 21:39:34.000000 doitoml-0.2.0/lite/demo.ipynb
+-rw-r--r--   0        0        0     2574 2023-05-07 21:39:34.000000 doitoml-0.2.0/lite/dodo.py
+-rw-r--r--   0        0        0      985 2023-05-07 21:39:34.000000 doitoml-0.2.0/lite/jupyter_lite_config.json
+-rw-r--r--   0        0        0     2100 2023-05-07 21:39:34.000000 doitoml-0.2.0/lite/logo.svg
+-rw-r--r--   0        0        0      189 2023-05-07 21:39:34.000000 doitoml-0.2.0/lite/playground-examples/python-and-js/package.json
+-rw-r--r--   0        0        0      174 2023-05-07 21:39:34.000000 doitoml-0.2.0/lite/playground-examples/python-and-js/pyproject.toml
+-rw-r--r--   0        0        0      165 2023-05-07 21:39:34.000000 doitoml-0.2.0/lite/playground-examples/simple-pyproject/pyproject.toml
+-rw-r--r--   0        0        0      337 2023-05-07 21:39:34.000000 doitoml-0.2.0/lite/playground-examples/tokens-and-paths/pyproject.toml
+-rw-r--r--   0        0        0    12050 2023-05-07 21:39:34.000000 doitoml-0.2.0/lite/playground.ipynb
+-rw-r--r--   0        0        0      613 2023-05-07 21:39:34.000000 doitoml-0.2.0/lite/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-05-07 21:39:34.000000 doitoml-0.2.0/lite/requirements.txt
+-rw-r--r--   0        0        0    13978 2023-05-07 21:39:34.000000 doitoml-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      188 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/_version.py
+-rw-r--r--   0        0        0       41 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/actors/__init__.py
+-rw-r--r--   0        0        0     1280 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/actors/_actor.py
+-rw-r--r--   0        0        0     1732 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/actors/py.py
+-rw-r--r--   0        0        0    27660 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/config.py
+-rw-r--r--   0        0        0     2903 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/constants.py
+-rw-r--r--   0        0        0    10450 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/doitoml.py
+-rw-r--r--   0        0        0     8016 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/dsl.py
+-rw-r--r--   0        0        0     2968 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/entry_points.py
+-rw-r--r--   0        0        0     2236 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/errors.py
+-rw-r--r--   0        0        0      829 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/loaders.py
+-rw-r--r--   0        0        0        0 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/py.typed
+-rw-r--r--   0        0        0       39 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/schema/__init__.py
+-rw-r--r--   0        0        0     5009 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/schema/_v0.schema.json
+-rw-r--r--   0        0        0     2310 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/schema/_v0_schema.py
+-rw-r--r--   0        0        0     3163 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/schema/v0.schema.toml
+-rw-r--r--   0        0        0     2426 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/schema/validator.py
+-rw-r--r--   0        0        0       44 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/skippers/__init__.py
+-rw-r--r--   0        0        0      583 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/skippers/_skipper.py
+-rw-r--r--   0        0        0     1360 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/skippers/bools.py
+-rw-r--r--   0        0        0     1055 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/skippers/path.py
+-rw-r--r--   0        0        0     2391 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/skippers/py.py
+-rw-r--r--   0        0        0       53 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/sources/__init__.py
+-rw-r--r--   0        0        0     4101 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/sources/_config.py
+-rw-r--r--   0        0        0     2694 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/sources/_source.py
+-rw-r--r--   0        0        0       25 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/sources/json/__init__.py
+-rw-r--r--   0        0        0      650 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/sources/json/_json.py
+-rw-r--r--   0        0        0     1094 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/sources/json/package.py
+-rw-r--r--   0        0        0       20 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/sources/toml/__init__.py
+-rw-r--r--   0        0        0      640 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/sources/toml/_toml.py
+-rw-r--r--   0        0        0      983 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/sources/toml/pyproject.py
+-rw-r--r--   0        0        0       20 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/sources/yaml/__init__.py
+-rw-r--r--   0        0        0      749 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/sources/yaml/_yaml.py
+-rw-r--r--   0        0        0       38 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/templaters/__init__.py
+-rw-r--r--   0        0        0      581 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/templaters/_templater.py
+-rw-r--r--   0        0        0     2158 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/templaters/jinja2.py
+-rw-r--r--   0        0        0     3032 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/templaters/jsone.py
+-rw-r--r--   0        0        0     2929 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/types.py
+-rw-r--r--   0        0        0       37 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/updaters/__init__.py
+-rw-r--r--   0        0        0      856 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/updaters/_updater.py
+-rw-r--r--   0        0        0     2197 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/updaters/doit_tools.py
+-rw-r--r--   0        0        0     1567 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/updaters/py.py
+-rw-r--r--   0        0        0       42 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/utils/__init__.py
+-rw-r--r--   0        0        0      820 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/utils/json.py
+-rw-r--r--   0        0        0     1280 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/utils/log.py
+-rw-r--r--   0        0        0      371 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/utils/path.py
+-rw-r--r--   0        0        0     4734 2023-05-07 21:39:34.000000 doitoml-0.2.0/src/doitoml/utils/py.py
+-rw-r--r--   0        0        0       25 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/__init__.py
+-rw-r--r--   0        0        0     4432 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/conftest.py
+-rw-r--r--   0        0        0     1883 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/test_actors.py
+-rw-r--r--   0        0        0     8134 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/test_config.py
+-rw-r--r--   0        0        0     2164 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/test_dsl.py
+-rw-r--r--   0        0        0     4361 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/test_examples.py
+-rw-r--r--   0        0        0      166 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/test_metadata.py
+-rw-r--r--   0        0        0      570 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/test_parse_fails.py
+-rw-r--r--   0        0        0      501 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/test_schema.py
+-rw-r--r--   0        0        0      523 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/test_self.py
+-rw-r--r--   0        0        0     2481 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/test_skip.py
+-rw-r--r--   0        0        0     2411 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/test_templaters.py
+-rw-r--r--   0        0        0     1298 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/test_unsafe_path.py
+-rw-r--r--   0        0        0     2132 2023-05-07 21:39:34.000000 doitoml-0.2.0/test/test_updaters.py
+-rw-r--r--   0        0        0     6338 1970-01-01 00:00:00.000000 doitoml-0.2.0/PKG-INFO
```

### Comparing `doitoml-0.1.1/.binder/environment.yml` & `doitoml-0.2.0/.binder/environment.yml`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,16 @@
   # build deps
   # publish deps
   - twine
   # publish deps
   # lint deps
   - black
   - mypy
+  - nbqa
+  - nbstripout
   - nodejs >=18,<19
   - ruff
   - ssort
   - taplo
   - types-jinja2
   - types-jsonschema
   - types-pyyaml
@@ -41,27 +43,32 @@
   - pytest-html
   - pytest-json-report
   - pytest-xdist
   - tomli-w
   - python-build
   # test deps
   # demo deps
+  - ipylab
   - ipywidgets >=8
+  - jupyterlab >=3.6.3,<4
   - jupyterlab-markup
-  - jupyterlab >=3.6.1,<4
   # demo deps
   # docs deps
   - docutils >=0.19
+  - jupyterlite-pyodide-kernel
+  - jupyterlite-core-with-libarchive
   - myst-nb
   - pydata-sphinx-theme
   - sphinx-autobuild
   - sphinx-autodoc-typehints
   - sphinx-copybutton
   - sphinx-design
   - sphinx-jsonschema
   - sphinxcontrib-mermaid
+  - importnb
+  - scour
   # docs deps
   # check deps
   - pytest-check-links
   # check deps
 
 name: doitoml-demo
```

### Comparing `doitoml-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `doitoml-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/.github/ISSUE_TEMPLATE/docs.md` & `doitoml-0.2.0/.github/ISSUE_TEMPLATE/docs.md`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/.github/ISSUE_TEMPLATE/release.md` & `doitoml-0.2.0/.github/ISSUE_TEMPLATE/release.md`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/.github/pull_request_template.md` & `doitoml-0.2.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/.github/workflows/badges.yml` & `doitoml-0.2.0/.github/workflows/badges.yml`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/.github/workflows/ci.yml` & `doitoml-0.2.0/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 env:
   PYTHONUNBUFFERED: "1"
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   CI: "1"
 
   # our stuff
-  CACHE_EPOCH: "4"
+  CACHE_EPOCH: "5"
 
 jobs:
   build:
     name: build
     runs-on: ${{ matrix.os }}-latest
     strategy:
       matrix:
```

### Comparing `doitoml-0.1.1/CONTRIBUTING.md` & `doitoml-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/LICENSE.txt` & `doitoml-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/README.md` & `doitoml-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/_actions.py` & `doitoml-0.2.0/_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,20 +94,21 @@
 
     hashfile.write_text(output, **UTF8)
 
     if not quiet:
         print(output)
 
 
-def toml2json(src: Path, dest: Path) -> None:
+def toml2json(src_path: str, dest_path: str) -> None:
     try:
         import tomllib
     except ImportError:
         import tomli as tomllib
-
+    src = Path(src_path)
+    dest = Path(dest_path)
     dest.parent.mkdir(exist_ok=True, parents=True)
     dest.write_text(
         json.dumps(tomllib.loads(src.read_text(**UTF8)), indent=2, sort_keys=True),
         **UTF8,
     )
```

### Comparing `doitoml-0.1.1/docs/_static/img/anvil.svg` & `doitoml-0.2.0/docs/_static/img/anvil.svg`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/docs/_static/img/logo.svg` & `doitoml-0.2.0/docs/_static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/docs/_static/js/mermaid.mjs` & `doitoml-0.2.0/docs/_static/js/mermaid.mjs`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/docs/conf.py` & `doitoml-0.2.0/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """documentation for ``doitoml``."""
 import datetime
 import os
 import re
 from pathlib import Path
-from typing import Any, Tuple
+from typing import Any, Dict, Tuple
 
 import tomli
 
 os.environ.update(IN_SPHINX="1")
 
 
 def patch_jsonschema() -> None:
@@ -95,16 +95,17 @@
 
 # warnings
 suppress_warnings = ["autosectionlabel.*"]
 
 # theme
 templates_path = ["_templates"]
 html_static_path = [
-    "_static",
+    "../build/lite",
     "../dist",
+    "_static",
 ]
 html_theme = "pydata_sphinx_theme"
 html_logo = "_static/img/logo.svg"
 html_favicon = "_static/img/logo.svg"
 html_css_files = ["css/theme.css"]
 
 html_theme_options = {
@@ -115,17 +116,19 @@
         {
             "name": "PyPI",
             "url": PROJ_DATA["project"]["urls"]["PyPI"],
             "icon": "fa-brands fa-python",
         },
         {
             "name": "conda-forge",
-            "url": "https://github.com/conda-forge/doitoml-feedstock#about-doitoml",
+            "url": "https://github.com/conda-forge/doitoml-split-feedstock",
             "icon": "_static/img/anvil.svg",
             "type": "local",
         },
     ],
     "footer_end": ["mermaid10"],
 }
 
+html_sidebars: Dict[str, Any] = {"demo": []}
+
 if REPO_INFO is not None:
     html_context = {**REPO_INFO.groupdict(), "doc_path": "docs"}
```

### Comparing `doitoml-0.1.1/docs/environment.yml` & `doitoml-0.2.0/docs/environment.yml`

 * *Files 23% similar despite different names*

```diff
@@ -15,20 +15,30 @@
   - jsonschema-with-format
   - pyyaml
   # optional deps
   # build deps
   - flit >=3.8
   - jsonschema-gentypes
   # build deps
+  # demo deps
+  - ipylab
+  - ipywidgets >=8
+  - jupyterlab >=3.6.3,<4
+  - jupyterlab-markup
+  # demo deps
   # docs deps
   - docutils >=0.19
+  - jupyterlite-pyodide-kernel
+  - jupyterlite-core-with-libarchive
   - myst-nb
   - pydata-sphinx-theme
   - sphinx-autobuild
   - sphinx-autodoc-typehints
   - sphinx-copybutton
   - sphinx-design
   - sphinx-jsonschema
   - sphinxcontrib-mermaid
+  - importnb
+  - scour
   # docs deps
 
 name: doitoml-docs
```

### Comparing `doitoml-0.1.1/docs/how-to/dsl.md` & `doitoml-0.2.0/docs/how-to/dsl.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 The _`doit`-specific language_ provides some declarative shortcuts to techniques that
 usually require more complex Python or shell.
 
 ## `${}` Get Environment Variables
 
 > Get the value of an environment variable. Usually executed before any other parsers.
+> All config sources share the _same_ namespace.
 
 <div class="jp-Mermaid">
 
 ```{mermaid}
 flowchart LR
 
 any-before --> dollar-leftbrace --> var-name --> rightbrace --> any-after
@@ -102,35 +103,36 @@
 ```
 
 ````
 
 ## `::` Reference a path or token
 
 > Get the value of any `paths` or `tokens`, either in the same `doitoml` configuration
-> file, or with a named prefix.
+> file, or with a named prefix (including {mod}`fnmatch` wildcards).
 
 <div class="jp-Mermaid">
 
 ```{mermaid}
 flowchart LR
 
-colon-colon --> namespaces --> token_or_path
+colon-colon --> prefixes --> token_or_path
 token_or_path -.-> path & tokens
 
-namespace -.-> prefix
+prefix & prefix-wildcard -.-> source-prefix
 
 colon-colon([<code>::</code>])
 token_or_path([<code>::</code><i>token or path</i>])
 
-subgraph namespaces [0 or 1 namespace]
-  namespace([<code>::</code><i>namespace</i>])
+subgraph prefixes [0 or 1 prefix]
+  prefix([<code>::</code><i>prefix</i>])
+  prefix-wildcard(["<code>::</code>[<i>fragment, <code>?</code>, or <code>*</code>] ...</i>"])
 end
 
 subgraph doitoml ["<code>doitoml</code> configuration"]
-  prefix("<code>prefix = ...</code>")
+  source-prefix("<code>prefix = ...</code>")
   subgraph paths ["<code>.paths</code>"]
     path("<code>some_path = [...]</code>")
   end
   subgraph tokens ["<code>.tokens</code>"]
     token("<code>some_token = [...]</code>")
   end
 end
```

### Comparing `doitoml-0.1.1/docs/how-to/logging.md` & `doitoml-0.2.0/docs/how-to/logging.md`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/docs/how-to/templates.md` & `doitoml-0.2.0/docs/how-to/templates.md`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/docs/how-to/user-python.md` & `doitoml-0.2.0/docs/how-to/user-python.md`

 * *Files 16% similar despite different names*

```diff
@@ -140,7 +140,47 @@
 ```toml
 # child/pyproject.toml
 [tool.doitoml.tasks.greet]
 actions = [
     {py = {"../my_actions:greetings:greet" = {args = ["hello", "world"] } }
 ]
 ```
+
+### Importing `dodo`
+
+In a project with `doit`'s default `dodo.py` layout, the `dodo` module itself can be
+imported...
+
+```toml
+# pyproject.toml
+[tool.doitoml.tasks.greet]
+actions=[{ py = {"dodo:greet": { kwargs = { whom = "world" } } } }]
+
+[tool.doitoml.tasks.greet]
+actions=[{ py = {"dodo:dump": { } } }]
+```
+
+... and even explore a `DoiTOML` instance.
+
+```py
+# dodo.py
+from doitoml import DoiTOML
+doitoml = DoiTOML()
+globals().update(doitoml.tasks())
+
+def greet(whom):
+    print(f"Hello {whom}")
+    return True
+
+def dump():
+    from pygments import highlight
+    from pygments.lexers import YamlLexer
+    from pygments.formatters import TerminalFormatter
+    from yaml import safe_dump
+    print(
+        highlight(
+            safe_dump(doitoml.config.to_dict()),
+            YamlLexer(),
+            TerminalFormatter(bg="dark")
+        )
+    )
+```
```

### Comparing `doitoml-0.1.1/docs/index.md` & `doitoml-0.2.0/docs/index.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-00000000: 6060 607b 6869 6e74 7d0a 5472 7920 7468  ```{hint}.Try th
-00000010: 6520 5b67 6574 7469 6e67 2073 7461 7274  e [getting start
-00000020: 6564 5d20 7475 746f 7269 616c 206f 7220  ed] tutorial or 
-00000030: 7468 6520 5b63 6865 6174 7368 6565 745d  the [cheatsheet]
-00000040: 0a60 6060 0a0a 5b67 6574 7469 6e67 2073  .```..[getting s
-00000050: 7461 7274 6564 5d3a 202e 2f74 7574 6f72  tarted]: ./tutor
-00000060: 6961 6c73 2f67 6574 7469 6e67 2d73 7461  ials/getting-sta
-00000070: 7274 6564 2e69 7079 6e62 0a5b 6368 6561  rted.ipynb.[chea
-00000080: 7473 6865 6574 5d3a 202e 2f72 6566 6572  tsheet]: ./refer
-00000090: 656e 6365 2f63 6865 6174 7368 6565 742e  ence/cheatsheet.
-000000a0: 6d64 0a0a 6060 607b 6772 6964 7d20 320a  md..```{grid} 2.
-000000b0: 0a20 207e 7e7e 7b67 7269 642d 6974 656d  .  ~~~{grid-item
-000000c0: 2d63 6172 647d 2020 7475 746f 7269 616c  -card}  tutorial
-000000d0: 730a 2020 3a6c 696e 6b3a 202e 2f74 7574  s.  :link: ./tut
-000000e0: 6f72 6961 6c73 2f69 6e64 6578 2e68 746d  orials/index.htm
-000000f0: 6c0a 2020 6c65 6172 6e69 6e67 2d6f 7269  l.  learning-ori
-00000100: 656e 7465 6420 7475 746f 7269 616c 730a  ented tutorials.
-00000110: 2020 7e7e 7e0a 2020 7e7e 7e7b 6772 6964    ~~~.  ~~~{grid
-00000120: 2d69 7465 6d2d 6361 7264 7d20 2068 6f77  -item-card}  how
-00000130: 2d74 6f0a 2020 3a6c 696e 6b3a 202e 2f68  -to.  :link: ./h
-00000140: 6f77 2d74 6f2f 696e 6465 782e 6874 6d6c  ow-to/index.html
-00000150: 0a20 2067 6f61 6c2d 6f72 6965 6e74 6564  .  goal-oriented
-00000160: 2068 6f77 2d74 6f20 6775 6964 6573 0a20   how-to guides. 
-00000170: 207e 7e7e 0a60 6060 0a0a 6060 607b 6772   ~~~.```..```{gr
-00000180: 6964 7d20 320a 2020 7e7e 7e7b 6772 6964  id} 2.  ~~~{grid
-00000190: 2d69 7465 6d2d 6361 7264 7d20 2075 6e64  -item-card}  und
-000001a0: 6572 7374 616e 6469 6e67 0a20 203a 6c69  erstanding.  :li
-000001b0: 6e6b 3a20 2e2f 756e 6465 7273 7461 6e64  nk: ./understand
-000001c0: 696e 672f 696e 6465 782e 6874 6d6c 0a20  ing/index.html. 
-000001d0: 2075 6e64 6572 7374 616e 6469 6e67 2d6f   understanding-o
-000001e0: 7269 656e 7465 6420 6469 7363 7573 7369  riented discussi
-000001f0: 6f6e 730a 2020 7e7e 7e0a 2020 7e7e 7e7b  ons.  ~~~.  ~~~{
-00000200: 6772 6964 2d69 7465 6d2d 6361 7264 7d20  grid-item-card} 
-00000210: 2072 6566 6572 656e 6365 0a20 203a 6c69   reference.  :li
-00000220: 6e6b 3a20 2e2f 7265 6665 7265 6e63 652f  nk: ./reference/
-00000230: 696e 6465 782e 6874 6d6c 0a20 2069 6e66  index.html.  inf
-00000240: 6f72 6d61 7469 6f6e 2d6f 7269 656e 7465  ormation-oriente
-00000250: 6420 7265 6665 7265 6e63 6520 6d61 7465  d reference mate
-00000260: 7269 616c 0a20 207e 7e7e 0a60 6060 0a0a  rial.  ~~~.```..
-00000270: 6060 607b 696e 636c 7564 657d 202e 2e2f  ```{include} ../
-00000280: 5245 4144 4d45 2e6d 640a 0a60 6060 0a0a  README.md..```..
-00000290: 2323 2064 6f63 756d 656e 7461 7469 6f6e  ## documentation
-000002a0: 2063 6f6e 7465 6e74 730a 0a60 6060 7b74   contents..```{t
-000002b0: 6f63 7472 6565 7d0a 3a6d 6178 6465 7074  octree}.:maxdept
-000002c0: 683a 2032 0a0a 7475 746f 7269 616c 732f  h: 2..tutorials/
-000002d0: 696e 6465 780a 686f 772d 746f 2f69 6e64  index.how-to/ind
-000002e0: 6578 0a75 6e64 6572 7374 616e 6469 6e67  ex.understanding
-000002f0: 2f69 6e64 6578 0a72 6566 6572 656e 6365  /index.reference
-00000300: 2f69 6e64 6578 0a60 6060 0a              /index.```.
+00000000: 6060 607b 6869 6e74 7d0a 5374 6172 7420  ```{hint}.Start 
+00000010: 7769 7468 2074 6865 205b 6765 7474 696e  with the [gettin
+00000020: 6720 7374 6172 7465 645d 2074 7574 6f72  g started] tutor
+00000030: 6961 6c2c 2074 6865 205b 6368 6561 7473  ial, the [cheats
+00000040: 6865 6574 5d2c 206f 722e 2e2e 0a0a 7e7e  heet], or.....~~
+00000050: 7e7b 6275 7474 6f6e 2d6c 696e 6b7d 202e  ~{button-link} .
+00000060: 2f64 656d 6f2e 6874 6d6c 0a3a 636f 6c6f  /demo.html.:colo
+00000070: 723a 2070 7269 6d61 7279 0a3a 6578 7061  r: primary.:expa
+00000080: 6e64 3a0a 5472 7920 2a2a 646f 6974 6f6d  nd:.Try **doitom
+00000090: 6c2a 2a20 4e6f 770a 7e7e 7e0a 6060 600a  l** Now.~~~.```.
+000000a0: 0a60 6060 7b67 7269 647d 2032 0a0a 2020  .```{grid} 2..  
+000000b0: 7e7e 7e7b 6772 6964 2d69 7465 6d2d 6361  ~~~{grid-item-ca
+000000c0: 7264 7d20 2074 7574 6f72 6961 6c73 0a20  rd}  tutorials. 
+000000d0: 203a 6c69 6e6b 3a20 2e2f 7475 746f 7269   :link: ./tutori
+000000e0: 616c 732f 696e 6465 782e 6874 6d6c 0a20  als/index.html. 
+000000f0: 206c 6561 726e 696e 672d 6f72 6965 6e74   learning-orient
+00000100: 6564 2074 7574 6f72 6961 6c73 0a20 207e  ed tutorials.  ~
+00000110: 7e7e 0a20 207e 7e7e 7b67 7269 642d 6974  ~~.  ~~~{grid-it
+00000120: 656d 2d63 6172 647d 2020 686f 772d 746f  em-card}  how-to
+00000130: 0a20 203a 6c69 6e6b 3a20 2e2f 686f 772d  .  :link: ./how-
+00000140: 746f 2f69 6e64 6578 2e68 746d 6c0a 2020  to/index.html.  
+00000150: 676f 616c 2d6f 7269 656e 7465 6420 686f  goal-oriented ho
+00000160: 772d 746f 2067 7569 6465 730a 2020 7e7e  w-to guides.  ~~
+00000170: 7e0a 6060 600a 0a60 6060 7b67 7269 647d  ~.```..```{grid}
+00000180: 2032 0a20 207e 7e7e 7b67 7269 642d 6974   2.  ~~~{grid-it
+00000190: 656d 2d63 6172 647d 2020 756e 6465 7273  em-card}  unders
+000001a0: 7461 6e64 696e 670a 2020 3a6c 696e 6b3a  tanding.  :link:
+000001b0: 202e 2f75 6e64 6572 7374 616e 6469 6e67   ./understanding
+000001c0: 2f69 6e64 6578 2e68 746d 6c0a 2020 756e  /index.html.  un
+000001d0: 6465 7273 7461 6e64 696e 672d 6f72 6965  derstanding-orie
+000001e0: 6e74 6564 2064 6973 6375 7373 696f 6e73  nted discussions
+000001f0: 0a20 207e 7e7e 0a20 207e 7e7e 7b67 7269  .  ~~~.  ~~~{gri
+00000200: 642d 6974 656d 2d63 6172 647d 2020 7265  d-item-card}  re
+00000210: 6665 7265 6e63 650a 2020 3a6c 696e 6b3a  ference.  :link:
+00000220: 202e 2f72 6566 6572 656e 6365 2f69 6e64   ./reference/ind
+00000230: 6578 2e68 746d 6c0a 2020 696e 666f 726d  ex.html.  inform
+00000240: 6174 696f 6e2d 6f72 6965 6e74 6564 2072  ation-oriented r
+00000250: 6566 6572 656e 6365 206d 6174 6572 6961  eference materia
+00000260: 6c0a 2020 7e7e 7e0a 6060 600a 0a60 6060  l.  ~~~.```..```
+00000270: 7b69 6e63 6c75 6465 7d20 2e2e 2f52 4541  {include} ../REA
+00000280: 444d 452e 6d64 0a0a 6060 600a 0a23 2320  DME.md..```..## 
+00000290: 646f 6375 6d65 6e74 6174 696f 6e20 636f  documentation co
+000002a0: 6e74 656e 7473 0a0a 6060 607b 746f 6374  ntents..```{toct
+000002b0: 7265 657d 0a3a 6d61 7864 6570 7468 3a20  ree}.:maxdepth: 
+000002c0: 320a 0a64 656d 6f0a 7475 746f 7269 616c  2..demo.tutorial
+000002d0: 732f 696e 6465 780a 686f 772d 746f 2f69  s/index.how-to/i
+000002e0: 6e64 6578 0a75 6e64 6572 7374 616e 6469  ndex.understandi
+000002f0: 6e67 2f69 6e64 6578 0a72 6566 6572 656e  ng/index.referen
+00000300: 6365 2f69 6e64 6578 0a60 6060 0a0a 5b67  ce/index.```..[g
+00000310: 6574 7469 6e67 2073 7461 7274 6564 5d3a  etting started]:
+00000320: 202e 2f74 7574 6f72 6961 6c73 2f67 6574   ./tutorials/get
+00000330: 7469 6e67 2d73 7461 7274 6564 2e69 7079  ting-started.ipy
+00000340: 6e62 0a5b 6368 6561 7473 6865 6574 5d3a  nb.[cheatsheet]:
+00000350: 202e 2f72 6566 6572 656e 6365 2f63 6865   ./reference/che
+00000360: 6174 7368 6565 742e 6d64 0a              atsheet.md.
```

### Comparing `doitoml-0.1.1/docs/reference/api.md` & `doitoml-0.2.0/docs/reference/api.md`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,42 @@
 ### `doit.tools` Updaters
 
 ```{eval-rst}
 .. currentmodule:: doitoml
 .. automodule:: doitoml.updaters.doit_tools
 ```
 
+## Skippers
+
+```{eval-rst}
+.. currentmodule:: doitoml
+.. automodule:: doitoml.skippers._skipper
+```
+
+### Boolean Skippers
+
+```{eval-rst}
+.. currentmodule:: doitoml
+.. automodule:: doitoml.skippers.bools
+```
+
+### Path Skippers
+
+```{eval-rst}
+.. currentmodule:: doitoml
+.. automodule:: doitoml.skippers.path
+```
+
+### Python Skippers
+
+```{eval-rst}
+.. currentmodule:: doitoml
+.. automodule:: doitoml.skippers.py
+```
+
 ## Templates
 
 ```{eval-rst}
 .. currentmodule:: doitoml
 .. automodule:: doitoml.templaters._templater
 ```
```

### Comparing `doitoml-0.1.1/docs/reference/cheatsheet.md` & `doitoml-0.2.0/docs/reference/cheatsheet.md`

 * *Files 16% similar despite different names*

```diff
@@ -36,36 +36,74 @@
 
 > The [pydoit documentation](https://pydoit.org/tasks.html) provides a number of other
 > fields: many of these only make sense in a `dodo.py`, or otherwise don't lend
 > themselves cleanly to declarative, portable tasks.
 
 </details>
 
-### `actions`
+## `actions`
 
-| action kind | example                                             | description                                        |
+| action kind | TOML example                                        | description                                        |
 | ----------- | --------------------------------------------------- | -------------------------------------------------- |
 | _string_    | `echo 1`                                            | passed directly to `doit` without any manipulation |
 | _token_     | `["echo", "1"]`                                     | each token expanded by the [DSL]                   |
 | _actor_     | `{py={"shutil.copy2"={args=["a"], kwargs={b="c"}}}` | each token in `(kw)args` expanded by the [DSL]     |
 
-### `doitoml` task metadata
+## `doitoml` task metadata
 
 > Put these in your `task.{task name}.meta.doitoml` to fune-tune the behavior of tasks.
 
 | field title | field data type            | field description                                                                                 |
 | ----------- | -------------------------- | ------------------------------------------------------------------------------------------------- |
 | **`cwd`**   | string or `Path`           | the current working directory for _shell_, _token_, and _actor_ tasks                             |
 | **`env`**   | dictionary of strings      | environment variables to overload for a specific task                                             |
-| **`skip`**  | string or `bool`           | if _falsey_, this task will not appear in `doit list` or be included in `doit run`                |
+| **`skip`**  | string or `bool` or dict   | if _falsey_, this task will not appear in `doit list` or be included in `doit run`                |
 | **`log`**   | (list of) string or `Path` | file(s) to capture output of actions, e.g. `task.log` or `["task.stdout.log", "task.stderr.log"]` |
 
+## `skip` values
+
+`skip` uses simple, normalized JSON `bool`-like values directly.
+
+More complex behaviors can be built from dictionary-based values.
+
+| skip kind      | true TOML example                   | will skip if...                    |
+| -------------- | ----------------------------------- | ---------------------------------- |
+| **`any`**      | `{any=[0, "TRUE"]}`                 | _any_ value is truthy              |
+| **`all`**      | `{all=[1, "${A_TRUE_ENV_VAR}"]}`    | _all_ values is truthy             |
+| **`not`**      | `{not=0}`                           | the value is falsey                |
+| **`exists`**   | `{exists=["::pyproject_toml"]}`     | all paths exist                    |
+| **`platform`** | `{platform={system=".*Windows.*"}}` | `platform` value (as JSON) matches |
+
 ## `doitoml` configuration
 
-| key                | default | field data type | field description                                                                                      |
-| ------------------ | ------- | --------------- | ------------------------------------------------------------------------------------------------------ |
-| **`config_paths`** | `[]`    | list of strings | relative paths to find more `doitoml` config sources: can use the `:get` [DSL] to extract partial data |
-| **`fail_quietly`** | `true`  | `bool`          | try to emit short, helpful errors with context                                                         |
-| **`update_env`**   | `true`  | `bool`          | use the `env` key to update the outer running environment variables                                    |
-| **`validate`**     | `true`  | `bool`          | use `jsonschema` to preflight tasks before `doit`                                                      |
+| key                | default                | field data type | field description                                                                                      |
+| ------------------ | ---------------------- | --------------- | ------------------------------------------------------------------------------------------------------ |
+| **`config_paths`** | `[]`                   | list of strings | relative paths to find more `doitoml` config sources: can use the `:get` [DSL] to extract partial data |
+| **`fail_quietly`** | `true`                 | `bool`          | try to emit short, helpful errors with context                                                         |
+| **`update_env`**   | `true`                 | `bool`          | use the `env` key to update the outer running environment variables                                    |
+| **`validate`**     | `true`                 | `bool`          | use `jsonschema` to preflight tasks before `doit`                                                      |
+| **`safe_paths`**   | parent of first config | list of strings | paths that are considered "safe" for doitoml to work with.                                             |
 
 [dsl]: ../how-to/dsl.md
+
+<style>
+    .bd-container, .bd-container__inner, .bd-content, .bd-article-container, .bd-article, #demo {
+        width: 100% !important;
+        max-width: unset !important;
+        justify-content: stretch;
+        flex: 1;
+        display: flex;
+        flex-direction: column;
+    }
+    .bd-header-article, .bd-sidebar-secondary, .bd-footer-article, .bd-footer, .bd-sidebar-primary, h1 {
+        display: none;
+    }
+    article > section  {
+        display: flex;
+        flex-direction: row;
+        flex-wrap: wrap;
+    }
+    article > section > section {
+        max-width: 45em;
+        padding-right: 1em;
+    }
+</style>
```

### Comparing `doitoml-0.1.1/docs/tutorials/getting-started.ipynb` & `doitoml-0.2.0/docs/tutorials/getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/docs/understanding/doit-good.md` & `doitoml-0.2.0/docs/understanding/doit-good.md`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/docs/understanding/extending.md` & `doitoml-0.2.0/docs/understanding/extending.md`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/dodo.py` & `doitoml-0.2.0/dodo.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/examples/py-js-web/_yarn.py` & `doitoml-0.2.0/examples/py-js-web/_yarn.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/examples/py-js-web/my_custom/_actions.py` & `doitoml-0.2.0/examples/py-js-web/my_custom/_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,20 +94,21 @@
 
     hashfile.write_text(output, **UTF8)
 
     if not quiet:
         print(output)
 
 
-def toml2json(src: Path, dest: Path) -> None:
+def toml2json(src_path: str, dest_path: str) -> None:
     try:
         import tomllib
     except ImportError:
         import tomli as tomllib
-
+    src = Path(src_path)
+    dest = Path(dest_path)
     dest.parent.mkdir(exist_ok=True, parents=True)
     dest.write_text(
         json.dumps(tomllib.loads(src.read_text(**UTF8)), indent=2, sort_keys=True),
         **UTF8,
     )
```

### Comparing `doitoml-0.1.1/examples/py-js-web/package.json` & `doitoml-0.2.0/examples/py-js-web/package.json`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/examples/py-js-web/pyproject.toml` & `doitoml-0.2.0/examples/py-js-web/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/examples/template-json-e/_actions.py` & `doitoml-0.2.0/examples/template-json-e/_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,20 +94,21 @@
 
     hashfile.write_text(output, **UTF8)
 
     if not quiet:
         print(output)
 
 
-def toml2json(src: Path, dest: Path) -> None:
+def toml2json(src_path: str, dest_path: str) -> None:
     try:
         import tomllib
     except ImportError:
         import tomli as tomllib
-
+    src = Path(src_path)
+    dest = Path(dest_path)
     dest.parent.mkdir(exist_ok=True, parents=True)
     dest.write_text(
         json.dumps(tomllib.loads(src.read_text(**UTF8)), indent=2, sort_keys=True),
         **UTF8,
     )
```

### Comparing `doitoml-0.1.1/examples/template-json-e/pyproject.toml` & `doitoml-0.2.0/examples/template-json-e/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/examples/uptodate-py/pyproject.toml` & `doitoml-0.2.0/examples/uptodate-py/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/js/package.json` & `doitoml-0.2.0/js/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998139880952381%*

 * *Differences: {"'doitoml'": "{'paths': {'all_prettier': {insert: [(4, ':rglob::../lite::*.json::*.yml')]}}}"}*

```diff
@@ -6,14 +6,15 @@
     "doitoml": {
         "paths": {
             "all_prettier": [
                 ":glob::.::*.yml::*.json",
                 ":glob::..::*.md::*.json::*.yml",
                 ":glob::../.binder::*.yml",
                 ":glob::../examples::*/*.json",
+                ":rglob::../lite::*.json::*.yml",
                 ":rglob::../.github::*.yml::*.md",
                 ":rglob::../docs::*.md::*.html::*.yml::*.css::*.mjs::!ipynb_checkpoints"
             ],
             "prettier_ignore": [
                 ".prettierignore"
             ],
             "yarn_in": [
```

### Comparing `doitoml-0.1.1/js/yarn.lock` & `doitoml-0.2.0/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/pyproject.toml` & `doitoml-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core<4,>=3.7.1"]
 
 [project]
 name = "doitoml"
-version = "0.1.1"
+version = "0.2.0"
 description = "Load declarative tasks for doit from TOML, JSON, YAML, and other files."
 readme = "README.md"
 authors = [{name = "doitoml contributors", email = "deathbeds@googlegroups.com"}]
 requires-python = ">=3.8"
 classifiers = [
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python :: 3 :: Only",
@@ -17,14 +17,23 @@
 dependencies = ["doit >=0.36.0", "typing_extensions", "tomli ; python_version<\"3.11\""]
 [project.optional-dependencies]
 all = ["doitoml[json-e]", "doitoml[jinja2]", "doitoml[jsonschema]", "doitoml[pyyaml]"]
 json-e = ["json-e >=4"]
 jinja2 = ["jinja2 >=3"]
 jsonschema = ["jsonschema >=4"]
 yaml = ["pyyaml >=5"]
+test = [
+  "build",
+  "pytest-console-scripts",
+  "pytest-cov",
+  "pytest-html-report",
+  "pytest-json-report",
+  "pytest-xdist",
+  "tomli-w",
+]
 [project.urls]
 "Bug Tracker" = "https://github.com/deathbeds/doitoml/issues"
 "Changelog" = "https://github.com/deathbeds/doitoml/blob/main/CHANGELOG.md"
 "Documentation" = "https://doitoml.rtfd.io"
 "PyPI" = "https://pypi.org/project/doitoml"
 "Source" = "https://github.com/deathbeds/doitoml/tree/main"
 [project.entry-points."doit.LOADER"]
@@ -46,14 +55,21 @@
 [project.entry-points."doitoml.templater.v0"]
 json-e = "doitoml.templaters.jsone:JsonE"
 jinja2 = "doitoml.templaters.jinja2:Jinja2"
 [project.entry-points."doitoml.updater.v0"]
 config_changed = "doitoml.updaters.doit_tools:ConfigChanged"
 run_once = "doitoml.updaters.doit_tools:RunOnce"
 py = "doitoml.updaters.py:PyUpdater"
+[project.entry-points."doitoml.skipper.v0"]
+any = "doitoml.skippers.bools:Any_"
+all = "doitoml.skippers.bools:All"
+not = "doitoml.skippers.bools:Not"
+exists = "doitoml.skippers.path:Exists"
+platform = "doitoml.skippers.py:Platform"
+py = "doitoml.skippers.py:Py"
 
 [tool.pytest.ini_options]
 cache_dir = "build/.cache/pytest"
 script_launch_mode = "subprocess"
 addopts = [
   # for humans
   "--html=build/reports/pytest.html",
@@ -61,23 +77,21 @@
   "--cov-report=html:build/reports/htmlcov",
   "--cov-report=term-missing:skip-covered",
   "--color=yes",
   # for robots
   "--json-report",
   "--json-report-file=build/reports/pytest.json",
   # xdist
-  "-n=auto",
   "--dist=worksteal",
   # cov
   "--cov=doitoml",
   "--cov-branch",
   "--cov-context=test",
   "--no-cov-on-fail",
   # misc
-  "-vv",
   "--ff",
   "--tb=long",
 ]
 
 [tool.coverage.html]
 show_contexts = true
 
@@ -119,15 +133,14 @@
 par_type = "thread"
 
 [tool.doit.commands.list]
 status = true
 subtasks = true
 
 [tool.ruff]
-# fix = true
 ignore = [
   "D211",
   "D213",
   # if it doesn't bother mypy...
   "ANN101",
   "ANN401",
   "PGH003",
@@ -193,70 +206,80 @@
 "dodo.py" = ["BLE001"]
 "doit_tools.py" = ["ARG002"]
 "doitoml.py" = ["PLR0913"]
 "dsl.py" = ["ARG002"]
 "entry_points.py" = ["BLE001"]
 "jinja2.py" = ["ARG002"]
 "test/**/*.py" = ["S101", "T201", "T203"]
+"lite/*.py" = ["D205", "INP001", "E402", "ANN201", "D103", "T201", "ANN001", "D100"]
 
 [tool.doitoml]
 prefix = ""
-config_paths = ["js/package.json"]
+config_paths = ["js/package.json", ":get::json::lite/jupyter_lite_config.json::doitoml"]
 validate = true
 
 [tool.doitoml.env]
 BLACK_CACHE_DIR = "./build/.cache/black"
 DOITOML_SDIST = "doitoml-${DOITOML_VERSION}.tar.gz"
 DOITOML_VERSION = ":get::toml::pyproject.toml::project::version"
 DOITOML_WHEEL = "doitoml-${DOITOML_VERSION}-py3-none-any.whl"
 PIP_DOWNLOAD_CACHE = "./build/.cache/pip"
 RUST_LOG = "error"
 SOURCE_DATE_EPOCH = ":get|0::json::build/source_date_epoch.json::SOURCE_DATE_EPOCH"
 DOITOML_SKIP_CODEGEN = "0"
 COV_FAIL_UNDER = "100"
+JUPYTER_PLATFORM_DIRS = "1"
 
 [tool.doitoml.tokens]
 sphinx_opts = ["-b", "html", "docs", "build/docs"]
 taplo_opts = [
   "--option=array_auto_collapse=true",
   "--option=compact_inline_tables=true",
   "--option=column_width=88",
 ]
 check_links_opts = [
-  "--check-links-ignore=https://",
-  "--check-links-ignore=builtins",
+  "--check-links-ignore",
+  "(https://|builtins|genindex)",
+  "--links-ext=html",
   "--no-cov",
   "--check-anchors",
   "--html=build/reports/pytest-check-links.html",
   "-p",
   "no:importnb",
   "--json-report-file=build/reports/pytest-check-links.json",
   "--tb=no",
+  "-n=10",
 ]
 pym = ["python3", "-m"]
 pip = ["::pym", "pip"]
 
 [tool.doitoml.paths]
 whl = ["dist/${DOITOML_WHEEL}"]
 sdist = ["dist/${DOITOML_SDIST}"]
 all_dist = ["::whl", "::sdist"]
 dist_hash = ["dist/SHA256SUMS"]
 docs_py = ["docs/conf.py"]
 docs_etc = [":rglob::docs/_static::*.*", ":rglob::docs/_templates::*.*"]
 all_misc_py = ["dodo.py", "_actions.py", "::all_py_test", "::docs_py"]
+demo_py = [":glob::lite::*.py"]
 all_py = ["::all_py_src", "::all_misc_py"]
-all_ssort = ["::py_src", "::all_misc_py"]
+all_ssort = ["::py_src", "::all_misc_py", "::demo_py"]
 py_src = [":rglob::src::*.py::!/_v0*"]
 all_py_src = [":rglob::src::*.py"]
-all_ipynb = [":rglob::docs::*.ipynb::!ipynb_checkpoints"]
+docs_logo = ["docs/_static/img/logo.svg"]
+all_ipynb = [
+  ":rglob::docs::*.ipynb::!ipynb_checkpoints",
+  ":rglob::lite::*.ipynb::!ipynb_checkpoints",
+]
 all_py_test = [":rglob::test::*.py"]
 ppt = ["pyproject.toml"]
-all_ppt = ["::ppt", ":glob::examples::*/pyproject.toml"]
+all_ppt = ["::ppt", ":glob::examples::*/pyproject.toml", "lite/pyproject.toml"]
 all_schema_toml = [":rglob::src/doitoml::*.toml"]
-all_toml = ["::all_ppt", "::all_schema_toml"]
+all_demo_toml = [":rglob::lite::*.toml::!.ipynb_checkpoints"]
+all_toml = ["::all_ppt", "::all_schema_toml", "::all_demo_toml"]
 all_py_dist = ["::ppt", "::py_src", "README.md", "LICENSE.txt"]
 _actions = ["_actions.py"]
 _ex_actions = ["examples/py-js-web/my_custom/_actions.py"]
 _tmpl_actions = ["examples/template-json-e/_actions.py"]
 all_examples = [
   ":glob::examples/py-js-web::*.json::*.toml::*.yml::*.py::*.js",
   ":rglob::examples/py-js-web/src::*.*",
@@ -276,14 +299,20 @@
 
 [tool.doitoml.tasks.bootstrap]
 meta = {doitoml = {log = "build/bootstrap.txt"}}
 targets = ["::bootstrap_txt"]
 actions = [
   [
     "::pip",
+    "uninstall",
+    "doitoml",
+    "-y",
+  ],
+  [
+    "::pip",
     "install",
     "-vv",
     "-e",
     ".",
     "--no-deps",
     "--ignore-installed",
     "--no-build-isolation",
@@ -339,14 +368,35 @@
 actions = [["ruff", "--fix", "::all_py"]]
 
 [tool.doitoml.tasks.fix.toml]
 doc = "Format TOML with taplo"
 file_dep = ["::all_toml"]
 actions = [["taplo", "fmt", "::taplo_opts", "::all_toml"]]
 
+[tool.doitoml.tasks.fix.ipynb]
+doc = "Format notebooks with nbqa"
+file_dep = ["::all_ipynb"]
+actions = [
+  [
+    "nbstripout",
+    "::all_ipynb",
+  ],
+  [
+    "nbqa",
+    "black",
+    "::all_ipynb",
+  ],
+  [
+    "nbqa",
+    "ruff",
+    "--fix-only",
+    "::all_ipynb",
+  ],
+]
+
 [tool.doitoml.tasks.lint.py.black]
 doc = "Check python formatting with `black`"
 file_dep = ["::ppt", "::all_py"]
 actions = [["black", "--quiet", "--check", "::all_py"]]
 
 [tool.doitoml.tasks.lint.py.ruff]
 doc = "Check python syntax with `ruff`"
@@ -376,35 +426,36 @@
     "::_actions",
     "::_tmpl_actions",
   ]}}},
 ]
 
 [tool.doitoml.tasks.test.unit]
 doc = "Run unit tests with pytest"
-file_dep = ["::ppt", "::all_py", "::all_py_test", "::all_examples"]
+file_dep = ["::ppt", "::all_py", "::all_py_test", "::all_examples", "::lite::config"]
 task_dep = ["test:preflight"]
-actions = [["pytest"]]
+actions = [["pytest", "-n=auto", "-vv"]]
 
 [tool.doitoml.tasks.test.full]
 doc = "Run all tests with pytest"
 file_dep = ["::ppt", "::all_py", "::all_py_test", "::all_examples"]
 task_dep = ["test:unit"]
-actions = [["pytest", "--cov-fail-under=${COV_FAIL_UNDER}"]]
+actions = [["pytest", "-n=auto", "-vv", "--cov-fail-under=${COV_FAIL_UNDER}"]]
 meta = {doitoml = {env = {DOITOML_TEST_FULL_EXAMPLES = 1}}}
 
 [tool.doitoml.tasks.docs.sphinx]
 doc = "Build documentation with `sphinx`"
 file_dep = [
   "::py_src",
   "::ppt",
   "::all_md",
   "::all_ipynb",
   "::docs_py",
   "::docs_etc",
   "::dist_hash",
+  "::lite::build_targets",
 ]
 actions = [["sphinx-build", "-W", "--color", "::sphinx_opts"]]
 targets = ["::docs_buildinfo"]
 
 [tool.doitoml.tasks.docs.check.links]
 doc = "Check documentation with `pytest-check-links`"
 file_dep = ["::docs_buildinfo", "::ppt"]
@@ -469,14 +520,19 @@
     "# docs deps",
   ]}}},
   {py = {"_actions:replace_between" = {args = [
     "::env_binder",
     "::env_docs",
     "# optional deps",
   ]}}},
+  {py = {"_actions:replace_between" = {args = [
+    "::env_binder",
+    "::env_docs",
+    "# demo deps",
+  ]}}},
 ]
 
 [tool.doitoml.tasks.env.test]
 file_dep = ["::env_binder"]
 targets = ["::env_test"]
 actions = [
   {py = {"_actions:replace_between" = {args = [
```

### Comparing `doitoml-0.1.1/src/doitoml/actors/_actor.py` & `doitoml-0.2.0/src/doitoml/actors/_actor.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/actors/py.py` & `doitoml-0.2.0/src/doitoml/actors/py.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/config.py` & `doitoml-0.2.0/src/doitoml/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Handles discovering, loading, and normalizing configuration."""
+import json
 import os
 import warnings
 from copy import deepcopy
 from pathlib import Path
 from pprint import pformat
 from typing import (
     TYPE_CHECKING,
@@ -16,28 +17,29 @@
     cast,
 )
 
 from .constants import (
     DEFAULTS,
     DOIT_TASK,
     DOITOML_META,
-    FALSEY,
     NAME,
 )
 from .errors import (
     ActionError,
     ConfigError,
     DoitomlError,
     MissingDependencyError,
     NoActorError,
     NoConfigError,
     NoTemplaterError,
     PrefixError,
+    SkipError,
     TemplaterError,
     UnresolvedError,
+    UnsafePathError,
 )
 from .schema._v0_schema import DoitomlSchema
 from .sources._config import ConfigParser, ConfigSource
 from .sources._source import Source
 from .types import (
     Action,
     LogPaths,
@@ -79,38 +81,41 @@
     paths: PrefixedStrings
     templates: PrefixedTemplates
     tokens: PrefixedStrings
     update_env: Optional[bool]
     fail_quietly: Optional[bool]
     discover_config_paths: Optional[bool]
     validate: Optional[bool]
+    safe_paths: List[str]
 
     def __init__(
         self,
         doitoml: "DoiTOML",
         config_paths: Paths,
         *,
         update_env: Optional[bool] = None,
         fail_quietly: Optional[bool] = None,
         discover_config_paths: Optional[bool] = None,
         validate: Optional[bool] = None,
+        safe_paths: Optional[List[str]] = None,
     ) -> None:
         """Create empty configuration and discover sources."""
         self.validate = validate
         self.doitoml = doitoml
         self.config_paths = config_paths
         self.sources = {}
         self.tasks = {}
         self.paths = {}
         self.env = {}
         self.tokens = {}
         self.templates = {}
         self.update_env = update_env
         self.fail_quietly = fail_quietly
         self.discover_config_paths = discover_config_paths
+        self.safe_paths = safe_paths or []
 
     def to_dict(self) -> DoitomlSchema:
         """Return a normalized subset of config data."""
         env = dict(**self.env)
         env.update(os.environ)
 
         as_dict: DoitomlSchema = to_json(
@@ -123,45 +128,60 @@
             },
         )
 
         return as_dict
 
     def initialize(self) -> None:
         """Perform a few passes to configure everything."""
-        # first find the env
         self.sources = self.find_config_sources()
-
+        # load top-level config values from the first config
         top_config = [*self.sources.values()][0]
-
-        unresolved_env = self.init_env({}, RETRIES)
-        if unresolved_env:
-            message = (
-                f"Failed to resolve environment variables: {pformat(unresolved_env)}"
-            )
-            raise UnresolvedError(message)
-
-        # load other top-level config values from the first config
         for key in DEFAULTS.ALL_FROM_FIRST_CONFIG:
             if getattr(self, key, None) is None:
                 setattr(self, key, top_config.raw_config.get(key, True))
 
-        # ...then find the paths
-        unresolved_paths = self.init_paths({}, RETRIES)
-        if unresolved_paths:
-            message = f"Failed to resolve paths: {pformat(unresolved_paths)}"
-            raise UnresolvedError(message)
+        unresolved_env: EnvDict = {}
+        unresolved_paths: PrefixedStrings = {}
+        unresolved_tokens: PrefixedStrings = {}
+        retry = RETRIES
+
+        # .. allow some retries for cross (but not circular) references
+        while retry:
+            retry -= 1
+            try:
+                unresolved_env = self.init_env(unresolved_env, RETRIES)
+                unresolved_paths = self.init_paths(unresolved_paths, RETRIES)
+                unresolved_tokens = self.init_tokens(unresolved_tokens, RETRIES)
+            except UnresolvedError:  # pragma: no cover
+                pass
+            if not any([unresolved_env, unresolved_paths, unresolved_tokens]):
+                break
 
-        # ...then find the commands
-        unresolved_commands = self.init_commands({}, RETRIES)
-        if unresolved_commands:
-            message = f"Failed to resolve commands: {pformat(unresolved_commands)}"
-            raise UnresolvedError(message)
+        if not retry:
+            message = [f"Gave up after {RETRIES} retries!"]
+            if unresolved_env:
+                message += [
+                    f"Failed to resolve environment variables: "
+                    f"{pformat(unresolved_env)}",
+                ]
+
+            if unresolved_paths:
+                message += [f"Failed to resolve paths: {pformat(unresolved_paths)}"]
+
+            if unresolved_tokens:
+                message += [
+                    f"Failed to resolve tokens: {pformat(unresolved_tokens)}",
+                ]
+
+            raise UnresolvedError("\n".join(message))
+
+        # ... then templates
         self.init_templates()
 
-        # .. then find the tasks
+        # ... then find the tasks
         self.init_tasks()
 
         self.maybe_validate()
 
     def maybe_validate(self) -> None:
         """Validate if requested, or."""
         if self.validate is False:
@@ -194,17 +214,22 @@
             unchecked_paths += self.find_fallback_config_sources()
 
         if not unchecked_paths:
             path = self.doitoml.cwd / DEFAULTS.CONFIG_PATH
             if path.exists():
                 unchecked_paths += [path]
 
+        if unchecked_paths and not self.safe_paths:
+            self.safe_paths = [str(unchecked_paths[0].parent.as_posix())]
+
         while unchecked_paths:
             config_path = unchecked_paths.pop(0)
-            config_source = self.load_config_source(Path(config_path))
+            config_source = self.load_config_source(
+                Path(self.check_safe_path(str(config_path.as_posix()))),
+            )
             self.find_one_config_source(config_source, config_sources)
 
         if not config_sources:
             message = "No ``doitoml`` config found"
             raise NoConfigError(message)
 
         return config_sources
@@ -274,14 +299,21 @@
 
     def init_source_env(self, source: ConfigSource, unresolved_env: EnvDict) -> None:
         """Initialize the env declared in a single source."""
         env = self.env
         raw_config = source.raw_config
         for env_key, env_value in raw_config.get("env", {}).items():
             if env_key in env:
+                self.doitoml.log.info(
+                    "$%s already set to `%s`: not setting with `%s` from %s",
+                    env_key,
+                    env[env_key],
+                    env_value,
+                    source,
+                )
                 continue
 
             new_key_value = self.resolve_one_env(source, env_value)
 
             if new_key_value is None:
                 unresolved_env[env_key] = env_value
             else:
@@ -291,16 +323,22 @@
     def resolve_one_env(self, source: ConfigSource, env_value: Any) -> Optional[str]:
         """Resolve a single env member."""
         new_value = str(env_value)
         for dsl in self.doitoml.entry_points.dsl.values():
             match = dsl.pattern.search(new_value)
             if match is not None:
                 try:
-                    new_value = str(dsl.transform_token(source, match, env_value)[0])
-                    break
+                    resolved = dsl.transform_token(
+                        source,
+                        match,
+                        new_value or env_value,
+                    )
+                    if resolved is None:  # pragma: no cover
+                        return None
+                    return str(resolved[0])
                 except DoitomlError:
                     return None
         return new_value
 
     def init_paths(
         self,
         unresolved_paths: PrefixedStrings,
@@ -315,31 +353,44 @@
             unresolved_paths = self.init_paths(
                 unresolved_paths,
                 0,
             )
 
         return unresolved_paths
 
-    def init_commands(
+    def check_safe_path(self, path: str) -> str:
+        """Check if some paths are safe."""
+        if any(path.startswith(safe) for safe in self.safe_paths):
+            return path
+
+        nl = "\n  -"
+        message = (
+            f"The path is outside the known `safe_paths`: {path}"
+            "\n"
+            f"""{nl}{nl.join(self.safe_paths)}"""
+        )
+        raise UnsafePathError(message)
+
+    def init_tokens(
         self,
-        unresolved_commands: PrefixedStrings,
+        unresolved_tokens: PrefixedStrings,
         retries: int,
     ) -> PrefixedStrings:
         """Find all commands in all sources."""
         for source in self.sources.values():
-            self.init_source_commands(source, unresolved_commands)
+            self.init_source_tokens(source, unresolved_tokens)
 
-        while unresolved_commands and retries:
+        while unresolved_tokens and retries:
             retries -= 1
-            unresolved_commands = self.init_commands(
-                unresolved_commands,
+            unresolved_tokens = self.init_tokens(
+                unresolved_tokens,
                 0,
             )
 
-        return unresolved_commands
+        return unresolved_tokens
 
     def init_source_paths(
         self,
         source: ConfigSource,
         unresolved_paths: PrefixedStrings,
     ) -> None:
         """Find the prefixed paths declared in a single source."""
@@ -356,34 +407,34 @@
                 unresolved_paths[source.prefix, path_key] = unresolved_specs
                 continue
             self.paths[source.prefix, path_key] = sorted(
                 {Path(p).as_posix() for p in found_paths},
             )
             unresolved_paths.pop((source.prefix, path_key), None)
 
-    def init_source_commands(
+    def init_source_tokens(
         self,
         source: ConfigSource,
-        unresolved_commands: PrefixedStrings,
+        unresolved_tokens: PrefixedStrings,
     ) -> None:
         """Find the prefixed paths declared in a single source."""
         raw_config = source.raw_config
         path_key: str
         for path_key, path_specs in raw_config.get(DEFAULTS.TOKENS, {}).items():
             found_tokens, unresolved_specs = self.resolve_some_path_specs(
                 source,
                 path_specs,
                 source_relative=False,
             )
 
             if unresolved_specs:
-                unresolved_commands[source.prefix, path_key] = unresolved_specs
+                unresolved_tokens[source.prefix, path_key] = unresolved_specs
                 continue
             self.tokens[source.prefix, path_key] = found_tokens
-            unresolved_commands.pop((source.prefix, path_key), None)
+            unresolved_tokens.pop((source.prefix, path_key), None)
 
     def resolve_one_path_spec(
         self,
         source: ConfigSource,
         spec: str,
         source_relative: bool,
         cwd: Optional[Path] = None,
@@ -401,19 +452,22 @@
                 resolved = dsl.transform_token(source, match, spec)
                 if resolved is None:
                     return None
                 break
 
         if resolved:
             if source_relative:
-                return [(cwd / r).resolve().as_posix() for r in resolved]
+                return [
+                    self.check_safe_path((cwd / r).resolve().as_posix())
+                    for r in resolved
+                ]
             return resolved
 
         if source_relative:
-            return [(cwd / spec).resolve().as_posix()]
+            return [self.check_safe_path((cwd / spec).resolve().as_posix())]
 
         return [spec]
 
     def init_templates(self) -> None:
         """Copy templates (for now)."""
         for prefix, source in self.sources.items():
             raw_templates = source.raw_config.get("templates", {})
@@ -480,17 +534,16 @@
         )  # type: ignore
 
         meta = cast(dict, task_or_group.get(DOIT_TASK.META))
 
         if isinstance(meta, dict) and NAME in meta:
             dt_meta = meta[NAME]
             if isinstance(dt_meta, dict) and DOITOML_META.SKIP in dt_meta:
-                skip = str(dt_meta.get(DOITOML_META.SKIP, "0"))
-                found = self.resolve_one_path_spec(source, skip, source_relative=False)
-                if found and str(found[0]).strip().lower() not in FALSEY:
+                skip = dt_meta.get(DOITOML_META.SKIP, "0")
+                if self.resolve_one_skip(source, skip):
                     return
 
         if maybe_old_actions:
             task = cast(Task, task_or_group)
             yield from self.resolve_one_task(source, prefixes, task)
             return
 
@@ -499,14 +552,34 @@
             for subtask_prefixes, subtask in self.resolve_one_task_or_group(
                 source,
                 (*prefixes, subtask_prefix),
                 subtask_or_group,
             ):
                 yield subtask_prefixes, subtask
 
+    def resolve_one_skip(self, source: ConfigSource, skip: Any) -> bool:
+        """Maybe skip discovery of task (and all its children)."""
+        if skip is None:
+            return False
+        if isinstance(skip, (int, bool, float)):
+            return bool(skip)
+        if isinstance(skip, str):
+            found = self.resolve_one_path_spec(source, skip, source_relative=False)
+            if not found:  # pragma: no cover
+                return False
+            json_val = json.loads(str(found[0]).lower().strip())
+            return bool(json_val)
+        if isinstance(skip, dict):
+            for key, skipper in self.doitoml.entry_points.skippers.items():
+                if key in skip:
+                    return skipper.should_skip(source, skip[key])
+
+        message = f"Skip in {source} is ambiguous: {skip}"
+        raise SkipError(message)
+
     def resolve_one_task(
         self,
         source: ConfigSource,
         prefixes: Tuple[str, ...],
         task: Task,
     ) -> PrefixedTaskGenerator:
         """Resolve a single simple task."""
@@ -573,15 +646,22 @@
         return {}, [*uptodate.keys()]
 
     def normalize_task_meta(self, source: ConfigSource, task: Task) -> Task:
         """Normalize task metadata."""
         new_task = deepcopy(task)
         meta = cast(dict, cast(dict, new_task).setdefault(DOIT_TASK.META, {}))
         dt_meta = cast(dict, meta.setdefault(NAME, {}))
-        dt_cwd = Path(dt_meta.get(DOITOML_META.CWD, source.path.parent))
+        raw_cwd = self.resolve_one_path_spec(
+            source,
+            dt_meta.get(DOITOML_META.CWD, str(source.path.parent)),
+            source_relative=True,
+        )
+        dt_cwd = Path(
+            self.check_safe_path(raw_cwd[0] if raw_cwd else str(source.path.parent)),
+        )
         dt_log_paths = self.build_log_paths(
             source,
             dt_meta.get(DOITOML_META.LOG),
             dt_cwd,
         )
         dt_meta[DOITOML_META.LOG] = dt_log_paths
         dt_meta[DOITOML_META.CWD] = dt_cwd
@@ -617,15 +697,15 @@
                 cwd=cwd,
             )
 
             if not maybe_stream_path:  # pragma: no cover
                 message = f"Unresolved log path {stream}"
                 raise ConfigError(message)
 
-            maybe_paths[i] = Path(maybe_stream_path[0])
+            maybe_paths[i] = Path(self.check_safe_path(maybe_stream_path[0]))
 
         return self.check_log_paths(*maybe_paths)
 
     def check_log_paths(self, stderr_path: Any, stdout_path: Any) -> LogPaths:
         """Verify log paths."""
         for path in [stderr_path, stdout_path]:
             if path and path.is_dir():
```

### Comparing `doitoml-0.1.1/src/doitoml/constants.py` & `doitoml-0.2.0/src/doitoml/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     CONFIG: Literal["doitoml.config-parser.v0"] = "doitoml.config-parser.v0"
     #: extend the ``doitoml`` actor vocabulary
     ACTOR: Literal["doitoml.actor.v0"] = "doitoml.actor.v0"
     #: extend the ``doitoml`` templater vocabulary
     TEMPLATER: Literal["doitoml.templater.v0"] = "doitoml.templater.v0"
     #: extend the ``doitoml`` uptodate vocabulary
     UPDATER: Literal["doitoml.updater.v0"] = "doitoml.updater.v0"
+    #: extend the ``doitoml`` skip vocabulary
+    SKIPPER: Literal["doitoml.skipper.v0"] = "doitoml.skipper.v0"
 
 
 class DOIT_TASK:
 
     """A collection of well-known ``doit`` keys."""
 
     #: ``doit`` actions
@@ -76,7 +78,10 @@
     LOG: Literal["log"] = "log"
     #: the file that defined the task
     SOURCE: Literal["source"] = "source"
 
 
 #: all the false things
 FALSEY = ["", "false", "0", "0.0", "{}", "[]", "null", "none"]
+
+#: fnmatch triggers
+FNMATCH_WILDCARDS = "*?["
```

### Comparing `doitoml-0.1.1/src/doitoml/doitoml.py` & `doitoml-0.2.0/src/doitoml/doitoml.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,26 +45,28 @@
         cwd: Optional[Path] = None,
         update_env: Optional[bool] = None,
         fail_quietly: Optional[bool] = None,
         log: Optional[logging.Logger] = None,
         log_level: MaybeLogLevel = None,
         discover_config_paths: Optional[bool] = None,
         validate: Optional[bool] = None,
+        safe_paths: Optional[List[str]] = None,
     ) -> None:
         """Initialize a ``doitoml`` task generator."""
         self.cwd = Path(cwd) if cwd else Path.cwd()
         try:
             self.log = self.init_log(log, log_level)
             self.entry_points = EntryPoints(self)
             self.config = self.init_config(
                 config_paths or [],
                 update_env=update_env,
                 fail_quietly=fail_quietly,
                 discover_config_paths=discover_config_paths,
                 validate=validate,
+                safe_paths=safe_paths,
             )
             # initialize late for ``entry_points`` that reference ``self.entry_points``
             self.entry_points.initialize()
             self.config.initialize()
 
         except DoitomlError as err:
             if fail_quietly or (
@@ -92,23 +94,25 @@
     def init_config(
         self,
         config_paths: PathOrStrings,
         update_env: Optional[bool] = None,
         fail_quietly: Optional[bool] = None,
         discover_config_paths: Optional[bool] = None,
         validate: Optional[bool] = None,
+        safe_paths: Optional[List[str]] = None,
     ) -> Config:
         """Initialize configuration."""
         return Config(
             self,
             [(self.cwd / path).resolve() for path in config_paths],
             update_env=update_env,
             fail_quietly=fail_quietly,
             discover_config_paths=discover_config_paths,
             validate=validate,
+            safe_paths=safe_paths,
         )
 
     def tasks(self) -> Dict[str, TaskFunction]:
         """Generate functions compatible with the default ``doit`` loader style."""
         tasks = {}
 
         task_groups = self.group_tasks(self.config.tasks)
```

### Comparing `doitoml-0.1.1/src/doitoml/dsl.py` & `doitoml-0.2.0/src/doitoml/dsl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Domain-specific language for declarative ``doit`` task generation."""
 
 import abc
+import fnmatch
 import json
 import os
 import re
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, List, Tuple, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Tuple, cast
+
+from doitoml.constants import FNMATCH_WILDCARDS
 
 from .errors import DslError
 from .types import Strings
 
 if TYPE_CHECKING:
     from .doitoml import DoiTOML
     from .sources._config import ConfigSource
@@ -48,31 +51,47 @@
 class PathRef(DSL):
 
     """Look for previously-found paths."""
 
     #: paths go before all other built-in DSL
     rank = 80
 
-    pattern = re.compile(r"^::((?P<prefix>[^:]+)::)?(?P<ref>[^:]+)$")
+    pattern = re.compile(r"^::((?P<prefix>[^:]*)::)?(?P<ref>[^:]+)$")
 
     def transform_token(
         self,
         source: "ConfigSource",
         match: re.Match[str],
         raw_token: str,
         **kwargs: Any,
     ) -> Strings:
         """Expand a path name (with optional prefix) to a previously-found value."""
         groups = match.groupdict()
         ref: str = groups["ref"]
-        prefix: str = groups["prefix"] or source.prefix
-        tokens = self.doitoml.config.tokens.get((prefix, ref))
-        if tokens:
-            return tokens
-        return self.doitoml.config.paths.get((prefix, ref))  # type: ignore
+        prefix = source.prefix if groups["prefix"] is None else groups["prefix"]
+
+        config = self.doitoml.config
+
+        if any(c in prefix for c in FNMATCH_WILDCARDS):
+            prefixes = fnmatch.filter(sorted(config.sources), prefix)
+        else:
+            prefixes = [prefix]
+
+        prefix_tokens: Dict[str, List[str]] = {}
+
+        for prefix in prefixes:
+            for named in [config.paths, config.tokens]:
+                from_named = named.get((prefix, ref))
+                if from_named is not None:
+                    prefix_tokens[prefix] = from_named
+
+        if prefix_tokens:
+            return sum(prefix_tokens.values(), [])
+
+        return None  # type: ignore
 
 
 class EnvReplacer(DSL):
 
     """A wrapper for UNIX-style variable expansion."""
 
     pattern = re.compile(r"\$\{([^\}]+)\}")
```

### Comparing `doitoml-0.1.1/src/doitoml/entry_points.py` & `doitoml-0.2.0/src/doitoml/entry_points.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 else:  # pragma: no cover
     from importlib.metadata import entry_points
 
 if TYPE_CHECKING:
     from .actors._actor import Actor
     from .doitoml import DoiTOML
     from .dsl import DSL
+    from .skippers._skipper import Skipper
     from .sources._config import ConfigParser
     from .sources._source import Parser
     from .templaters._templater import Templater
     from .updaters._updater import Updater
 
 
 class EntryPoints:
@@ -28,14 +29,15 @@
     doitoml: "DoiTOML"
     dsl: Dict[str, "DSL"]
     parsers: Dict[str, "Parser"]
     config_parsers: Dict[str, "ConfigParser"]
     actors: Dict[str, "Actor"]
     templaters: Dict[str, "Templater"]
     updaters: Dict[str, "Updater"]
+    skippers: Dict[str, "Skipper"]
 
     def __init__(self, doitoml: "DoiTOML") -> None:
         """Create a new collection of loaded ``entry_points``."""
         self.doitoml = doitoml
 
     def initialize(self) -> None:
         """Load all ``entry_points``."""
@@ -43,14 +45,15 @@
         self.config_parsers = self.load_entry_point_group(ENTRY_POINTS.CONFIG)
         self.parsers = self.load_entry_point_group(ENTRY_POINTS.PARSER)
         # load DSL, which might reference parsers
         self.dsl = self.load_entry_point_group(ENTRY_POINTS.DSL)
         self.actors = self.load_entry_point_group(ENTRY_POINTS.ACTOR)
         self.templaters = self.load_entry_point_group(ENTRY_POINTS.TEMPLATER)
         self.updaters = self.load_entry_point_group(ENTRY_POINTS.UPDATER)
+        self.skippers = self.load_entry_point_group(ENTRY_POINTS.SKIPPER)
 
     def load_entry_point_group(self, group: str) -> Dict[str, Any]:
         """Find and load ``entry_points`` from installed packages."""
         eps = {}
 
         for entry_point in entry_points(group=group):
             try:
```

### Comparing `doitoml-0.1.1/src/doitoml/errors.py` & `doitoml-0.2.0/src/doitoml/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,24 @@
 
 
 class ConfigError(DoitomlError):
 
     """An error related to configuration."""
 
 
+class UnsafePathError(ConfigError):
+
+    """An error related to unsafe paths."""
+
+
+class SkipError(ConfigError):
+
+    """An error related to an ambiguous skip."""
+
+
 class NoConfigError(ConfigError):
 
     """An error when no configuration at all is found."""
 
 
 class UnresolvedError(ConfigError):
```

### Comparing `doitoml-0.1.1/src/doitoml/loaders.py` & `doitoml-0.2.0/src/doitoml/loaders.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/schema/_v0.schema.json` & `doitoml-0.2.0/src/doitoml/schema/_v0.schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999705882352942%*

 * *Differences: {"'definitions'": "{'meta-doitoml': {'properties': {'skip': {replace: OrderedDict([('oneOf', "*

 * *                  "[OrderedDict([('type', 'string')]), OrderedDict([('type', 'number')]), "*

 * *                  "OrderedDict([('type', 'null')]), OrderedDict([('type', 'object')])])])}}}}"}*

```diff
@@ -116,15 +116,28 @@
                                 "type": "null"
                             }
                         ]
                     },
                     "type": "array"
                 },
                 "skip": {
-                    "type": "string"
+                    "oneOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "number"
+                        },
+                        {
+                            "type": "null"
+                        },
+                        {
+                            "type": "object"
+                        }
+                    ]
                 },
                 "source": {
                     "type": "string"
                 }
             },
             "required": [
                 "cwd",
```

### Comparing `doitoml-0.1.1/src/doitoml/schema/_v0_schema.py` & `doitoml-0.2.0/src/doitoml/schema/_v0_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,17 @@
     cwd: Required[str]
     """ Required property """
 
     env: "EnvironmentVariables"
     log: Required[List["_DoitomlMetadataaLogItem"]]
     """ Required property """
 
-    skip: str
+    skip: Union[str, Union[int, float], None, Dict[str, Any]]
+    """ oneOf """
+
     source: Required[str]
     """ Required property """
 
 
 class DoitomlSchema(TypedDict, total=False):
 
     """doitoml Schema.
```

### Comparing `doitoml-0.1.1/src/doitoml/schema/v0.schema.toml` & `doitoml-0.2.0/src/doitoml/schema/v0.schema.toml`

 * *Files 10% similar despite different names*

```diff
@@ -55,15 +55,20 @@
 additionalProperties = false
 required = ["cwd", "log", "source"]
 
 [definitions.meta-doitoml.properties]
 cwd = {type = "string"}
 env = {"$ref" = "#/definitions/env"}
 log = {type = "array", items = {oneOf = [{type = "string"}, {type = "null"}]}}
-skip = {type = "string"}
+skip = {oneOf = [
+  {type = "string"},
+  {type = "number"},
+  {type = "null"},
+  {type = "object"},
+]}
 source = {type = "string"}
 
 [definitions.actions]
 type = "array"
 items = {"$ref" = "#/definitions/action"}
 
 [definitions.action]
```

### Comparing `doitoml-0.1.1/src/doitoml/schema/validator.py` & `doitoml-0.2.0/src/doitoml/schema/validator.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/sources/_config.py` & `doitoml-0.2.0/src/doitoml/sources/_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Handles discovering, loading, and normalizing configuration."""
 import abc
+import os
 import re
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Tuple, cast
 
 from doitoml.constants import DEFAULTS
 from doitoml.errors import ConfigError
 from doitoml.types import Strings
@@ -54,15 +55,20 @@
         """Extract a raw ``doitoml`` configuration from this source."""
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, ConfigSource) and other.path == self.path
 
     def __repr__(self) -> str:
         """Format the source for warnings and errors."""
-        return f"<{self.__class__.__name__} prefix='{self.prefix}' path='{self.path}'>"
+        return (
+            f"<{self.__class__.__name__}"
+            f" prefix='{self.prefix}' "
+            f" path='{os.path.relpath(str(self.path), str(Path.cwd()))}'"
+            f">"
+        )
 
 
 class WrapperConfigSource(ConfigSource):
 
     """A config source which wraps another source with a specific root."""
 
     child_source: Source
```

### Comparing `doitoml-0.1.1/src/doitoml/sources/_source.py` & `doitoml-0.2.0/src/doitoml/sources/_source.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/sources/json/_json.py` & `doitoml-0.2.0/src/doitoml/sources/json/_json.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/sources/json/package.py` & `doitoml-0.2.0/src/doitoml/sources/json/package.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/sources/toml/_toml.py` & `doitoml-0.2.0/src/doitoml/sources/toml/_toml.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/sources/toml/pyproject.py` & `doitoml-0.2.0/src/doitoml/sources/toml/pyproject.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/sources/yaml/_yaml.py` & `doitoml-0.2.0/src/doitoml/sources/yaml/_yaml.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/templaters/_templater.py` & `doitoml-0.2.0/src/doitoml/templaters/_templater.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/templaters/jinja2.py` & `doitoml-0.2.0/src/doitoml/templaters/jinja2.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/templaters/jsone.py` & `doitoml-0.2.0/src/doitoml/templaters/jsone.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/types.py` & `doitoml-0.2.0/src/doitoml/types.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/updaters/_updater.py` & `doitoml-0.2.0/src/doitoml/updaters/_updater.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/updaters/doit_tools.py` & `doitoml-0.2.0/src/doitoml/updaters/doit_tools.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/updaters/py.py` & `doitoml-0.2.0/src/doitoml/updaters/py.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/utils/json.py` & `doitoml-0.2.0/src/doitoml/utils/json.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/utils/log.py` & `doitoml-0.2.0/src/doitoml/utils/log.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/src/doitoml/utils/py.py` & `doitoml-0.2.0/src/doitoml/utils/py.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/test/conftest.py` & `doitoml-0.2.0/test/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test configuration and fixtures for ``doitoml``."""
+import json
 import logging
 import os
 import shutil
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Dict, Generator, Tuple
 
 import pytest
@@ -37,15 +38,17 @@
 
 HERE = Path(__file__).parent
 ROOT = HERE.parent
 
 SELF_DODO = ROOT / "dodo.py"
 SELF_PPT = ROOT / "pyproject.toml"
 SELF_JS = ROOT / "js"
+SELF_LITE = ROOT / "lite"
 SELF_PACKAGE_JSON = SELF_JS / "package.json"
+SELF_LITE_CONFIG = SELF_LITE / "jupyter_lite_config.json"
 
 EXAMPLES_ROOT = ROOT / "examples"
 EXAMPLE_PPT = sorted(EXAMPLES_ROOT.glob("*/pyproject.toml"))
 
 
 @pytest.fixture(params=[p.parent.name for p in EXAMPLE_PPT])
 def a_data_example(
@@ -66,21 +69,23 @@
     shutil.rmtree(dest, ignore_errors=True)
 
 
 @pytest.fixture()
 def a_self_test_skeleton(tmp_path: Path) -> Generator[Path, None, None]:
     """Provide ``doitoml``'s own ``doitoml`` configuration."""
     dest = tmp_path / "self"
-    js_dest = dest / "js"
-    js_dest.mkdir(parents=True)
-    for path in [SELF_DODO, SELF_PPT]:
-        shutil.copy2(path, dest / path.name)
-
-    for path in [SELF_PACKAGE_JSON]:
-        shutil.copy2(path, js_dest / path.name)
+    all_dest = {
+        dest: [SELF_DODO, SELF_PPT],
+        dest / "js": [SELF_PACKAGE_JSON],
+        dest / "lite": [SELF_LITE_CONFIG],
+    }
+    for dest_parent, paths in all_dest.items():
+        for path in paths:
+            dest_parent.mkdir(exist_ok=True, parents=True)
+            shutil.copy2(path, dest_parent / path.name)
 
     old_cwd = Path.cwd()
     os.chdir(str(dest))
     yield dest
     os.chdir(str(old_cwd))
     shutil.rmtree(dest, ignore_errors=True)
 
@@ -131,7 +136,25 @@
         ppt.write_text(ppt_text, encoding="utf-8")
         return ppt
 
     old_cwd = Path.cwd()
     os.chdir(str(tmp_path))
     yield make_pyproject_toml
     os.chdir(str(old_cwd))
+
+
+@pytest.fixture()
+def a_package_json_with(
+    a_pyproject_with: TPyprojectMaker,
+) -> Callable[[Dict[str, Any]], Path]:
+    """Build a package.json (and py_project.toml that refers to it)."""
+
+    def with_pj(doitoml: Dict[str, Any]) -> Path:
+        ppt = a_pyproject_with({"config_paths": ["package.json"]})
+        pj = ppt.parent / "package.json"
+        pj.write_text(
+            json.dumps({"doitoml": {**doitoml, "prefix": "pj"}}),
+            encoding="utf-8",
+        )
+        return pj
+
+    return with_pj
```

### Comparing `doitoml-0.1.1/test/test_actors.py` & `doitoml-0.2.0/test/test_actors.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/test/test_config.py` & `doitoml-0.2.0/test/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 @pytest.mark.parametrize(
     ("expected", "message", "items"),
     [
         (UnresolvedError, "resolve environment", {"env": {"a": "${b}"}}),
         (UnresolvedError, "resolve paths", {"paths": {"a": ["::b"]}}),
-        (UnresolvedError, "resolve commands", {"tokens": {"a": ["::b"]}}),
+        (UnresolvedError, "resolve tokens", {"tokens": {"a": ["::b"]}}),
         (ConfigError, "not a dict", {"tasks": {"a": []}}),
         (UnresolvedError, "paths", {"tasks": {"a": {"actions": [["::b"]]}}}),
         (
             UnresolvedError,
             "paths",
             {"tasks": {"a": {"actions": [["::b"]], "file_dep": ["::b"]}}},
         ),
```

### Comparing `doitoml-0.1.1/test/test_dsl.py` & `doitoml-0.2.0/test/test_dsl.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/test/test_examples.py` & `doitoml-0.2.0/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/test/test_parse_fails.py` & `doitoml-0.2.0/test/test_parse_fails.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/test/test_self.py` & `doitoml-0.2.0/test/test_self.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/test/test_templaters.py` & `doitoml-0.2.0/test/test_templaters.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/test/test_updaters.py` & `doitoml-0.2.0/test/test_updaters.py`

 * *Files identical despite different names*

### Comparing `doitoml-0.1.1/PKG-INFO` & `doitoml-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doitoml
-Version: 0.1.1
+Version: 0.2.0
 Summary: Load declarative tasks for doit from TOML, JSON, YAML, and other files.
 Author-email: doitoml contributors <deathbeds@googlegroups.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -14,24 +14,32 @@
 Requires-Dist: doitoml[json-e] ; extra == "all"
 Requires-Dist: doitoml[jinja2] ; extra == "all"
 Requires-Dist: doitoml[jsonschema] ; extra == "all"
 Requires-Dist: doitoml[pyyaml] ; extra == "all"
 Requires-Dist: jinja2 >=3 ; extra == "jinja2"
 Requires-Dist: json-e >=4 ; extra == "json-e"
 Requires-Dist: jsonschema >=4 ; extra == "jsonschema"
+Requires-Dist: build ; extra == "test"
+Requires-Dist: pytest-console-scripts ; extra == "test"
+Requires-Dist: pytest-cov ; extra == "test"
+Requires-Dist: pytest-html-report ; extra == "test"
+Requires-Dist: pytest-json-report ; extra == "test"
+Requires-Dist: pytest-xdist ; extra == "test"
+Requires-Dist: tomli-w ; extra == "test"
 Requires-Dist: pyyaml >=5 ; extra == "yaml"
 Project-URL: Bug Tracker, https://github.com/deathbeds/doitoml/issues
 Project-URL: Changelog, https://github.com/deathbeds/doitoml/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://doitoml.rtfd.io
 Project-URL: PyPI, https://pypi.org/project/doitoml
 Project-URL: Source, https://github.com/deathbeds/doitoml/tree/main
 Provides-Extra: all
 Provides-Extra: jinja2
 Provides-Extra: json-e
 Provides-Extra: jsonschema
+Provides-Extra: test
 Provides-Extra: yaml
 
 # `doitoml`
 
 > Load declarative tasks for [doit] from TOML, JSON, YAML, and other files.
 
 |            docs             |                                          install                                           |                build                 |
```

