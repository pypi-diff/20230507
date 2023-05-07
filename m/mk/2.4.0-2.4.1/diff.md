# Comparing `tmp/mk-2.4.0.tar.gz` & `tmp/mk-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mk-2.4.0.tar", last modified: Thu Apr  6 11:35:50 2023, max compression
+gzip compressed data, was "mk-2.4.1.tar", last modified: Sun May  7 09:14:20 2023, max compression
```

## Comparing `mk-2.4.0.tar` & `mk-2.4.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.509682 mk-2.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.493682 mk-2.4.0/.config/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-06 11:35:19.000000 mk-2.4.0/.config/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-06 11:35:19.000000 mk-2.4.0/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-06 11:35:19.000000 mk-2.4.0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-06 11:35:19.000000 mk-2.4.0/.config/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-06 11:35:19.000000 mk-2.4.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.493682 mk-2.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-06 11:35:19.000000 mk-2.4.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-06 11:35:19.000000 mk-2.4.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-06 11:35:19.000000 mk-2.4.0/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-06 11:35:19.000000 mk-2.4.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-06 11:35:19.000000 mk-2.4.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.493682 mk-2.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-06 11:35:19.000000 mk-2.4.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-06 11:35:19.000000 mk-2.4.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-06 11:35:19.000000 mk-2.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-06 11:35:19.000000 mk-2.4.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-06 11:35:19.000000 mk-2.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-06 11:35:19.000000 mk-2.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-06 11:35:19.000000 mk-2.4.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.493682 mk-2.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-06 11:35:19.000000 mk-2.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-06 11:35:19.000000 mk-2.4.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-06 11:35:19.000000 mk-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-06 11:35:19.000000 mk-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-06 11:35:50.505682 mk-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-06 11:35:19.000000 mk-2.4.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.497682 mk-2.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.497682 mk-2.4.0/docs/.overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-06 11:35:19.000000 mk-2.4.0/docs/.overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-04-06 11:35:19.000000 mk-2.4.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.497682 mk-2.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-04-06 11:35:19.000000 mk-2.4.0/docs/images/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    31065 2023-04-06 11:35:19.000000 mk-2.4.0/docs/images/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-06 11:35:19.000000 mk-2.4.0/docs/images/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-06 11:35:19.000000 mk-2.4.0/docs/images/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-06 11:35:19.000000 mk-2.4.0/docs/images/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-06 11:35:19.000000 mk-2.4.0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    22103 2023-04-06 11:35:19.000000 mk-2.4.0/docs/images/logo.afdesign
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-06 11:35:19.000000 mk-2.4.0/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-06 11:35:19.000000 mk-2.4.0/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110782 2023-04-06 11:35:19.000000 mk-2.4.0/docs/images/mk-social-preview.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.497682 mk-2.4.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-06 11:35:19.000000 mk-2.4.0/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-06 11:35:19.000000 mk-2.4.0/docs/tools.md
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-06 11:35:19.000000 mk-2.4.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-06 11:35:19.000000 mk-2.4.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.497682 mk-2.4.0/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-06 11:35:19.000000 mk-2.4.0/playbooks/example-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-06 11:35:19.000000 mk-2.4.0/playbooks/test-integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-06 11:35:19.000000 mk-2.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.489682 mk-2.4.0/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.497682 mk-2.4.0/samples/deep/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-06 11:35:19.000000 mk-2.4.0/samples/deep/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.501682 mk-2.4.0/samples/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-06 11:35:19.000000 mk-2.4.0/samples/integration/ansible-lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-06 11:35:19.000000 mk-2.4.0/samples/integration/cookiecutter.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-06 11:35:19.000000 mk-2.4.0/samples/integration/flask-babel.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-06 11:35:19.000000 mk-2.4.0/samples/integration/podman.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-06 11:35:19.000000 mk-2.4.0/samples/integration/typeshed.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 11:35:50.509682 mk-2.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.489682 mk-2.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.501682 mk-2.4.0/src/mk/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/_typer.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-06 11:35:50.000000 mk-2.4.0/src/mk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.505682 mk-2.4.0/src/mk/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/tools/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/tools/cmake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/tools/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/tools/make.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/tools/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/tools/pre_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/tools/py_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/tools/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/tools/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/tools/taskfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-06 11:35:19.000000 mk-2.4.0/src/mk/tools/tox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.501682 mk-2.4.0/src/mk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-06 11:35:50.000000 mk-2.4.0/src/mk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-06 11:35:50.000000 mk-2.4.0/src/mk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 11:35:50.000000 mk-2.4.0/src/mk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-06 11:35:50.000000 mk-2.4.0/src/mk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-06 11:35:50.000000 mk-2.4.0/src/mk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-06 11:35:50.000000 mk-2.4.0/src/mk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.505682 mk-2.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-06 11:35:19.000000 mk-2.4.0/test/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:35:50.505682 mk-2.4.0/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)       21 2023-04-06 11:35:19.000000 mk-2.4.0/tools/example-shell.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-06 11:35:19.000000 mk-2.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.731895 mk-2.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.711895 mk-2.4.1/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-07 09:13:38.000000 mk-2.4.1/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-07 09:13:38.000000 mk-2.4.1/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-07 09:13:38.000000 mk-2.4.1/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-07 09:13:38.000000 mk-2.4.1/.config/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-07 09:13:38.000000 mk-2.4.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.711895 mk-2.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 09:13:38.000000 mk-2.4.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 09:13:38.000000 mk-2.4.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-07 09:13:38.000000 mk-2.4.1/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-07 09:13:38.000000 mk-2.4.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 09:13:38.000000 mk-2.4.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.715895 mk-2.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-07 09:13:38.000000 mk-2.4.1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-07 09:13:38.000000 mk-2.4.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-07 09:13:38.000000 mk-2.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-07 09:13:38.000000 mk-2.4.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-07 09:13:38.000000 mk-2.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-07 09:13:38.000000 mk-2.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-07 09:13:38.000000 mk-2.4.1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.715895 mk-2.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-07 09:13:38.000000 mk-2.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-07 09:13:38.000000 mk-2.4.1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-07 09:13:38.000000 mk-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-07 09:13:38.000000 mk-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-07 09:14:20.731895 mk-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 09:13:38.000000 mk-2.4.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.715895 mk-2.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.715895 mk-2.4.1/docs/.overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-07 09:13:38.000000 mk-2.4.1/docs/.overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-07 09:13:38.000000 mk-2.4.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.715895 mk-2.4.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-07 09:13:38.000000 mk-2.4.1/docs/images/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31065 2023-05-07 09:13:38.000000 mk-2.4.1/docs/images/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-05-07 09:13:38.000000 mk-2.4.1/docs/images/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-07 09:13:38.000000 mk-2.4.1/docs/images/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-07 09:13:38.000000 mk-2.4.1/docs/images/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-07 09:13:38.000000 mk-2.4.1/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    22103 2023-05-07 09:13:38.000000 mk-2.4.1/docs/images/logo.afdesign
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-07 09:13:38.000000 mk-2.4.1/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-07 09:13:38.000000 mk-2.4.1/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110782 2023-05-07 09:13:38.000000 mk-2.4.1/docs/images/mk-social-preview.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.715895 mk-2.4.1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-07 09:13:38.000000 mk-2.4.1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-07 09:13:38.000000 mk-2.4.1/docs/tools.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-07 09:13:38.000000 mk-2.4.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-07 09:13:38.000000 mk-2.4.1/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.715895 mk-2.4.1/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 09:13:38.000000 mk-2.4.1/playbooks/example-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-07 09:13:38.000000 mk-2.4.1/playbooks/test-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-07 09:13:38.000000 mk-2.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.707895 mk-2.4.1/samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.715895 mk-2.4.1/samples/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-07 09:13:38.000000 mk-2.4.1/samples/deep/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.719895 mk-2.4.1/samples/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-07 09:13:38.000000 mk-2.4.1/samples/integration/ansible-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-07 09:13:38.000000 mk-2.4.1/samples/integration/cookiecutter.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 09:13:38.000000 mk-2.4.1/samples/integration/flask-babel.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-07 09:13:38.000000 mk-2.4.1/samples/integration/podman.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-07 09:13:38.000000 mk-2.4.1/samples/integration/typeshed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 09:14:20.731895 mk-2.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.707895 mk-2.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.719895 mk-2.4.1/src/mk/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/_typer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 09:14:20.000000 mk-2.4.1/src/mk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.727895 mk-2.4.1/src/mk/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/tools/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/tools/cmake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/tools/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/tools/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/tools/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/tools/pre_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/tools/py_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/tools/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/tools/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/tools/taskfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-07 09:13:38.000000 mk-2.4.1/src/mk/tools/tox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.723895 mk-2.4.1/src/mk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-07 09:14:20.000000 mk-2.4.1/src/mk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-07 09:14:20.000000 mk-2.4.1/src/mk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:14:20.000000 mk-2.4.1/src/mk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-07 09:14:20.000000 mk-2.4.1/src/mk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-07 09:14:20.000000 mk-2.4.1/src/mk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-07 09:14:20.000000 mk-2.4.1/src/mk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.731895 mk-2.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-07 09:13:38.000000 mk-2.4.1/test/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:14:20.731895 mk-2.4.1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       21 2023-05-07 09:13:38.000000 mk-2.4.1/tools/example-shell.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-07 09:13:38.000000 mk-2.4.1/tox.ini
```

### Comparing `mk-2.4.0/.config/requirements.txt` & `mk-2.4.1/.config/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 colorama==0.4.6
 cryptography==39.0.2
 diskcache==5.4.0
 docutils==0.19
 gitdb==4.0.10
 gitpython==3.1.31
 idna==3.4
-importlib-metadata==6.1.0
+importlib-metadata==6.2.0
 jaraco-classes==3.2.3
 jeepney==0.8.0
 keyring==23.13.1
 markdown-it-py==2.2.0
 mdurl==0.1.2
 more-itertools==9.1.0
 packaging==23.0
```

### Comparing `mk-2.4.0/.github/workflows/release.yml` & `mk-2.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/.github/workflows/tox.yml` & `mk-2.4.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/.pre-commit-config.yaml` & `mk-2.4.1/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 ---
 ci:
   skip: [markdownlint_docker]
 repos:
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.264"
+    hooks:
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
         always_run: true
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
           - prettier-plugin-sort-json
   - repo: https://github.com/markdownlint/markdownlint.git
     rev: v0.12.0
     hooks:
       - id: markdownlint_docker
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        args:
-          # https://github.com/pre-commit/mirrors-isort/issues/9#issuecomment-624404082
-          - --filter-files
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         args: [--safe]
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
@@ -35,32 +33,23 @@
       - id: trailing-whitespace
       - id: mixed-line-ending
       - id: check-byte-order-marker
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
         language_version: python3
-  - repo: https://github.com/pycqa/flake8.git
-    rev: 6.0.0
-    hooks:
-      - id: flake8
-        additional_dependencies:
-          - flake8-absolute-import
-          - flake8-black>=0.1.1
-          - flake8-docstrings>=1.5.0
-        language_version: python3
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.30.0
+    rev: v1.31.0
     hooks:
       - id: yamllint
         files: \.(yaml|yml)$
         types: [file, yaml]
         entry: yamllint --strict
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.2.0
     hooks:
       - id: mypy
         # mypy args needed in order to match mypy cli behavior
         args: ["--python-version", "3.8"]
         entry: mypy src/
         pass_filenames: false
         additional_dependencies:
```

### Comparing `mk-2.4.0/LICENSE` & `mk-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/PKG-INFO` & `mk-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mk
-Version: 2.4.0
+Version: 2.4.1
 Summary: mk
 Author-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/pycontribs/mk
 Project-URL: repository, https://github.com/pycontribs/mk
 Project-URL: changelog, https://github.com/pycontribs/mk/releases
 Keywords: mk
```

### Comparing `mk-2.4.0/docs/README.md` & `mk-2.4.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/docs/images/android-chrome-192x192.png` & `mk-2.4.1/docs/images/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/docs/images/android-chrome-512x512.png` & `mk-2.4.1/docs/images/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/docs/images/apple-touch-icon.png` & `mk-2.4.1/docs/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/docs/images/favicon-32x32.png` & `mk-2.4.1/docs/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/docs/images/favicon.ico` & `mk-2.4.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/docs/images/logo.afdesign` & `mk-2.4.1/docs/images/logo.afdesign`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/docs/images/logo.png` & `mk-2.4.1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/docs/images/logo.svg` & `mk-2.4.1/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/docs/images/mk-social-preview.png` & `mk-2.4.1/docs/images/mk-social-preview.png`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/docs/stylesheets/extra.css` & `mk-2.4.1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/docs/tools.md` & `mk-2.4.1/docs/tools.md`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/mkdocs.yml` & `mk-2.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/mypy.ini` & `mk-2.4.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/playbooks/test-integration.yml` & `mk-2.4.1/playbooks/test-integration.yml`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/pyproject.toml` & `mk-2.4.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -81,14 +81,21 @@
 # During development we might remove code (files) with coverage data, and we dont want to fail:
 ignore_errors = true
 show_missing = true
 
 [tool.isort]
 profile = "black"
 
+[tool.mypy]
+python_version = 3.9
+strict = true
+color_output = true
+error_summary = true
+no_incremental = true
+
 [tool.pylint."MESSAGES CONTROL"]
 # increase from default is 50 which is too aggressive
 max-statements = 60
 disable = [
   # Disabled on purpose (explain in comment)
   "line-too-long", # black managed
   "wrong-import-position", # isort managed
@@ -99,14 +106,49 @@
   "missing-function-docstring",
   "missing-module-docstring",
   "no-value-for-parameter",
   "not-an-iterable",
   "too-few-public-methods",
 ]
 
+[tool.ruff]
+ignore = [
+  # temporary disabled until we fix them:
+  "ANN",
+  "B",
+  "T",
+  "D",
+  "E",
+  "PT",
+  "ERA",
+  "PTH",
+  "C901",
+  "ARG",
+  "FBT",
+  "SIM",
+  "PGH",
+  "TCH",
+  "PLR",
+  "INP",
+  "RET",
+]
+select = ["ALL"]
+target-version = "py39"
+# Same as Black.
+line-length = 88
+
+[tool.ruff.flake8-pytest-style]
+parametrize-values-type = "tuple"
+
+[tool.ruff.isort]
+known-first-party = ["mk"]
+
+[tool.ruff.per-file-ignores]
+"test/**/*.py" = ["S"]
+
 [tool.setuptools.dynamic]
 optional-dependencies.test = { file = [".config/requirements-test.txt"] }
 optional-dependencies.docs = { file = [".config/requirements-docs.txt"] }
 dependencies = { file = [".config/requirements.in"] }
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
```

### Comparing `mk-2.4.0/src/mk/__main__.py` & `mk-2.4.1/src/mk/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,58 +1,72 @@
 """Main module."""
+from __future__ import annotations
+
 import argparse
 import itertools
 import logging
 import os
 import shlex
-from typing import Any, Dict, List
+from typing import Any
 
 import typer
 from rich.console import Console
 from rich.logging import RichHandler
 
 from mk import __version__
 from mk._typer import CustomTyper
 from mk.ctx import ctx
 
-handlers: List[logging.Handler]
+handlers: list[logging.Handler]
 console_err = Console(stderr=True)
 app = CustomTyper(width=console_err.width, rich_markup_mode="rich")
 
 if "_MK_COMPLETE" in os.environ:
     level = logging.CRITICAL
     handlers = [logging.NullHandler()]
 else:
     level = logging.DEBUG
     handlers = [
-        RichHandler(console=console_err, show_time=False, show_path=False, markup=False)
+        RichHandler(
+            console=console_err,
+            show_time=False,
+            show_path=False,
+            markup=False,
+        ),
     ]
 
 logging.basicConfig(
     level=logging.WARNING,
     format="%(message)s",
     handlers=handlers,
 )
 
 
 def version_callback(value: bool) -> None:
     if value:
         typer.echo(f"mk {__version__}")
-        raise typer.Exit()
+        raise typer.Exit
 
 
 @app.callback(invoke_without_command=True)
 def main(
     click_ctx: typer.Context,
     # pylint: disable=unused-argument
     version: bool = typer.Option(
-        None, "--version", callback=version_callback, is_eager=True
-    ),  # noqa: B008
+        None,
+        "--version",
+        callback=version_callback,
+        is_eager=True,
+    ),
     verbose: int = typer.Option(
-        0, "--verbose", "-v", count=True, help="Increase verbosity."
+        0,
+        "--verbose",
+        "-v",
+        count=True,
+        help="Increase verbosity.",
     ),
 ) -> None:
     # enforce coloring because some tools like npm may auto disable it due to
     # the lack of real tty.
     os.environ["FORCE_COLOR"] = os.environ.get("FORCE_COLOR", "true")
 
     # click_ctx.invoked_subcommand can be the command or None
@@ -68,39 +82,46 @@
 @app.command()
 def commands() -> None:
     """List all commands available."""
     for action in ctx.runner.actions:
         print(action.name)
 
 
-def cli() -> None:
+def cli() -> None:  # pylint: disable=too-many-locals
     parser = argparse.ArgumentParser(
         description="Preprocess arguments to set log level.",
         add_help=False,
     )
     parser.add_argument(
-        "-v", "--verbose", action="append_const", const=1, dest="verbosity"
+        "-v",
+        "--verbose",
+        action="append_const",
+        const=1,
+        dest="verbosity",
     )
     opt, _ = parser.parse_known_args()
     opt.verbosity = 0 if opt.verbosity is None else sum(opt.verbosity)
     if opt.verbosity:
         log_level = logging.INFO if opt.verbosity == 1 else logging.DEBUG
         logging.getLogger().setLevel(log_level)
-        logging.log(level=log_level, msg=f"Reconfigured logging level to {log_level}")
+        msg = f"Reconfigured logging level to {log_level}"
+        logging.log(level=log_level, msg=msg)
 
     existing_commands = []
     for command_info in app.registered_commands:
         command = typer.main.get_command_from_info(
-            command_info, pretty_exceptions_short=False, rich_markup_mode="rich"
+            command_info,
+            pretty_exceptions_short=False,
+            rich_markup_mode="rich",
         )
         existing_commands.append(command.name)
 
     # command = get_command_from_info(command_info=command_info)
 
-    action_map: Dict[str, Any] = {}
+    action_map: dict[str, Any] = {}
     for action in ctx.runner.actions:
         # Currently we rename action that overlap but in the future we may
         # want to allow one to shadow others or we may want to chain them
         # under a single name.
         action_name = action.name
         counter = itertools.count(2)
         while action_name in existing_commands:
@@ -131,17 +152,17 @@
         action_map[action_name] = action
         existing_commands.append(action_name)
     # Add aliases for 1-3 letter commands
     for alias_len in (1, 2, 3):
         for x, action in action_map.items():
             alias = x[0:alias_len]
             # pylint: disable=consider-iterating-dictionary
-            if alias in action_map.keys():
+            if alias in action_map:
                 continue
-            if sum(1 for name in action_map.keys() if name.startswith(alias)) == 1:
+            if sum(1 for name in action_map if name.startswith(alias)) == 1:
                 app.command(
                     name=alias,
                     short_help=f"Alias for [dim]mk {x}[/dim]",
                     rich_help_panel="aliases",
                     hidden=bool(opt.verbosity < 1),
                 )(action.run)
```

### Comparing `mk-2.4.0/src/mk/_typer.py` & `mk-2.4.1/src/mk/_typer.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,9 +25,12 @@
         self,
         *args,
         cls=None,
         context_settings={"help_option_names": ["-h", "--help"]},
         **kwargs,
     ):
         return super().command(
-            *args, cls=cls, context_settings=context_settings, **kwargs
+            *args,
+            cls=cls,
+            context_settings=context_settings,
+            **kwargs,
         )
```

### Comparing `mk-2.4.0/src/mk/runner.py` & `mk-2.4.1/src/mk/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+from __future__ import annotations
+
 import hashlib
 import logging
 import sys
 
 try:
     from functools import cached_property
 except ImportError:
     from cached_property import cached_property  # type: ignore
 
 from pathlib import Path
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from mk.tools import Action
 
 import pluggy
 from diskcache import Cache
 from git import Repo
 from git.exc import GitError
 
 
 class Runner:
     def __init__(self) -> None:
-        self.root: Optional[Path] = None
+        self.root: Path | None = None
         try:
             self.repo = Repo(".", search_parent_directories=True)
         except GitError:
             logging.fatal("Current version of mk works only within git repos.")
             self.repo = None
             return
         self.branch = ""
@@ -34,29 +36,29 @@
                 self.branch = self.repo.active_branch.name
                 logging.info("Detected active branch '%s'", self.branch)
             except TypeError:
                 logging.warning("No branch detected.")
 
         self.root = Path(self.repo.working_dir)
         hash_key = f"{sys.version_info.major}{sys.version_info.minor}{self.root}"
-        self.hash = hashlib.sha1(hash_key.encode("UTF-8")).hexdigest()[:5]
+        self.hash = hashlib.sha256(hash_key.encode("UTF-8")).hexdigest()[:5]
         self.cache = Cache(f"~/.cache/mk.{self.hash}/")
 
         if self.repo.is_dirty():
             logging.warning("Repo is dirty on %s", self.repo.active_branch)
 
     @cached_property
     def pm(self) -> pluggy.PluginManager:
         """Plugin manager."""
         pm = pluggy.PluginManager("mk_tools")
         pm.load_setuptools_entrypoints("mk_tools")
         return pm
 
     @cached_property
-    def actions(self) -> List["Action"]:
+    def actions(self) -> list[Action]:
         """List of discovered actions."""
         if not self.root:
             return []
 
         _actions = []
         for _, cls_name in self.pm.list_name_plugin():
             c = cls_name()
```

### Comparing `mk-2.4.0/src/mk/tools/ansible.py` & `mk-2.4.1/src/mk/tools/shell.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,45 @@
+from __future__ import annotations
+
 import glob
 import os
 from pathlib import Path
-from typing import List, Optional
 
 from mk.exec import run_or_fail
 from mk.tools import Action, Tool
 
 
-class AnsibleTool(Tool):
-    name = "ansible"
+class ShellTool(Tool):
+    name = "shell"
 
-    def run(self, action: Optional[Action] = None):
+    def run(self, action: Action | None = None) -> None:
         if action and action.filename:
-            run_or_fail(
-                ["ansible-playbook", "-vv", action.filename],
-                tee=True,
-                env_overrides={"ANSIBLE_FORCE_COLOR": "1"},
-            )
+            run_or_fail(f"./{action.filename}", tee=True)
 
     def is_present(self, path: Path) -> bool:
-        if os.path.isdir(os.path.join(path, "playbooks")):
-            return True
-        return False
-
-    def actions(self) -> List[Action]:
-        actions: List[Action] = []
-        for filename in glob.glob("playbooks/*.yml"):
-            name = os.path.splitext(os.path.basename(filename))[0]
-            actions.append(
-                Action(
-                    name=name,
-                    description=f"[dim]ansible-playbook {filename}[/dim]",
-                    tool=self,
-                    filename=filename,
+        return True
+
+    def actions(self) -> list[Action]:
+        actions: list[Action] = []
+        exclude_list = ["setup.py"]
+        for filename in [
+            *glob.glob("*"),
+            *glob.glob("tools/*.*"),
+            *glob.glob("bin/*.*"),
+            *glob.glob("scripts/*.*"),
+        ]:
+            if (
+                os.path.isfile(filename)
+                and os.access(filename, os.X_OK)
+                and filename not in exclude_list
+                and not filename.endswith(".so")
+            ):
+                name = os.path.splitext(os.path.basename(filename))[0]
+                actions.append(
+                    Action(
+                        name=name,
+                        description=f"[dim]./{filename}[/dim]",
+                        tool=self,
+                        filename=filename,
+                    ),
                 )
-            )
         return actions
```

### Comparing `mk-2.4.0/src/mk/tools/cmake.py` & `mk-2.4.1/src/mk/tools/cmake.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+from __future__ import annotations
+
 import logging
 import os
 import shutil
 from pathlib import Path
-from typing import List, Optional
 
 from mk.exec import run_or_fail
 from mk.tools import Action, Tool
 
 
 class CMakeTool(Tool):
     name = "cmake"
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(self)
-        self.configfile = None
-        self._is_present = None
+        self.configfile: str | None = None
+        self._is_present: bool | None = None
 
-    def run(self, action: Optional[Action] = None) -> None:
+    def run(self, action: Action | None = None) -> None:
         cmd = ["cmake"]
         if action:
             cmd.append(action.name)
         run_or_fail(cmd, tee=True)
 
     def is_present(self, path: Path) -> bool:
         if self._is_present is not None:
@@ -28,23 +29,23 @@
         self._is_present = False
         for name in ["CMakeLists.txt"]:
             configfile = os.path.join(path, name)
             if os.path.isfile(configfile):
                 self.configfile = configfile
                 if not shutil.which("cmake"):
                     logging.warning(
-                        "Unable to find cmake tool. See https://cmake.org/download/"
+                        "Unable to find cmake tool. See https://cmake.org/download/",
                     )
                     self._is_present = False
                     break
                 logging.warning(
-                    "cmake is not fully supported yet by mk. See https://github.com/pycontribs/mk/issues/135"
+                    "cmake is not fully supported yet by mk. See https://github.com/pycontribs/mk/issues/135",
                 )
                 self._is_present = True
                 break
-        return self._is_present
+        return bool(self._is_present)
 
-    def actions(self) -> List[Action]:
+    def actions(self) -> list[Action]:
         actions = []
         if self.is_present(Path(".")):
             actions.append(Action(name=".", tool=self, description="Run 'cmake .'"))
         return actions
```

### Comparing `mk-2.4.0/src/mk/tools/git.py` & `mk-2.4.1/src/mk/tools/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 """Expose features related to git repositories."""
 from __future__ import annotations
 
 import logging
 import shutil
 import sys
 from pathlib import Path
-from typing import List, Optional
 
 from mk.ctx import ctx
 from mk.exec import fail, run_or_fail
 from mk.tools import Action, Tool
 
 
 class GitTool(Tool):
     name = "git"
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(self)
 
-    def run(self, action: Optional[Action] = None) -> None:
+    def run(self, action: Action | None = None) -> None:
         if action and action.name == "up":
             self.up()
         else:
-            raise NotImplementedError(f"Action {action} is not supported.")
+            msg = f"Action {action} is not supported."
+            raise NotImplementedError(msg)
 
     def is_present(self, path: Path) -> bool:
         if not shutil.which("gh"):
             logging.warning("Unable to find gh tool. See https://cli.github.com/")
             return False
         return True
 
-    def actions(self) -> List[Action]:
-        actions: List[Action] = []
+    def actions(self) -> list[Action]:
+        actions: list[Action] = []
         if ctx.runner.branch not in ["main", "master"]:
             if self.is_present(self.path):
                 actions.append(
                     Action(
                         name="up",
                         description="Upload current change by creating or updating a CR/PR.",
                         tool=self,
-                    )
+                    ),
                 )
         else:
             logging.info(
-                "Not adding 'up' action as it does not work when current branch is main/master"
+                "Not adding 'up' action as it does not work when current branch is main/master",
             )
         return actions
 
     # pylint: disable=too-many-branches
     def up(self):
         repo = ctx.runner.repo
         if not repo or repo.is_dirty():
@@ -64,38 +64,39 @@
                     "Uploading from default branch is not allowed in order to avoid accidents.",
                     2,
                 )
 
             remotes = {r.name for r in repo.remotes}
             if not {"origin", "upstream"}.issubset(remotes):
                 logging.debug(
-                    "Assuring you have two remotes, your fork as [blue]origin[/] and [blue]upstream[/]"
+                    "Assuring you have two remotes, your fork as [blue]origin[/] and [blue]upstream[/]",
                 )
                 run_or_fail(["gh", "repo", "fork", "--remote=true"], tee=True)
                 remotes = {r.name for r in repo.remotes}
             if "upstream" not in remotes:
                 fail("Failed to create upstream")
 
             if tracking_branch is None:
                 logging.debug("We do not have atracking branch")
             else:
                 logging.debug("Performing a git push")
 
             logging.debug("Doing a git push")
             run_or_fail(
-                ["git", "push", "--force-with-lease", "-u", "origin", "HEAD"], tee=False
+                ["git", "push", "--force-with-lease", "-u", "origin", "HEAD"],
+                tee=False,
             )
 
             # github for the moment
             # https://github.com/cli/cli/issues/1718
 
             # --web option is of not use because it happens too soon, confusing github
             logging.debug("Tryging to detect if there are existing PRs open")
             result = run_or_fail(
-                ["gh", "pr", "list", "-S", f"head:{repo.active_branch}"]
+                ["gh", "pr", "list", "-S", f"head:{repo.active_branch}"],
             )
             if result.returncode == 0:
                 pr_list = []
                 if result.stdout:
                     for line in result.stdout.splitlines():
                         pr_list.append(line.split("\t")[0])
                 if len(pr_list) == 0:
@@ -114,14 +115,15 @@
                         "--body",
                         body,
                     ]
                     result = run_or_fail(cmd, tee=True)
                     logging.debug(result.stdout)
                 elif len(pr_list) == 1:
                     logging.debug(
-                        "PR #%s already exists, no need to create new one.", pr_list[0]
+                        "PR #%s already exists, no need to create new one.",
+                        pr_list[0],
                     )
                 else:
                     logging.warning(
                         "Unable to decide which PR to use when multiple are found: %s",
                         pr_list,
                     )
```

### Comparing `mk-2.4.0/src/mk/tools/make.py` & `mk-2.4.1/src/mk/tools/make.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,48 @@
+from __future__ import annotations
+
 import os
 import re
 from pathlib import Path
-from typing import List, Optional
 
 from mk.exec import run_or_fail
 from mk.tools import Action, Tool
 
 
 class MakeTool(Tool):
     name = "make"
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(self)
-        self.makefile = None
+        self.makefile: str | None = None
 
-    def run(self, action: Optional[Action] = None) -> None:
+    def run(self, action: Action | None = None) -> None:
         cmd = ["make"]
         if action:
             cmd.append(action.name)
         run_or_fail(cmd, tee=True)
 
     def is_present(self, path: Path) -> bool:
         for name in ["Makefile", "makefile", "GNUmakefile"]:
             makefile = os.path.join(path, name)
             if os.path.isfile(makefile):
                 self.makefile = makefile
                 return True
         return False
 
-    def actions(self) -> List[Action]:
+    def actions(self) -> list[Action]:
         actions = []
-
-        with open(self.makefile, "r", encoding="utf-8") as file:
+        if not self.makefile:
+            msg = "Makefile not found"
+            raise RuntimeError(msg)
+        with open(self.makefile, encoding="utf-8") as file:
             for line in file.readlines():
                 # Current implementation assumes that descriptions are added
                 # using double ## after the target name.
                 # Inspired by https://github.com/containers/podman/blob/master/Makefile#L127
                 match = re.match(r"^([a-zA-Z_-]+):.*?## (.*)$$", line)
                 if match:
                     target, description = match.groups()
                     actions.append(
-                        Action(name=target, tool=self, description=description)
+                        Action(name=target, tool=self, description=description),
                     )
         return actions
```

### Comparing `mk-2.4.0/src/mk/tools/node.py` & `mk-2.4.1/src/mk/tools/node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
+
 import json
 from pathlib import Path
-from typing import List, Optional
 
 from mk.exec import run, run_or_fail
 from mk.tools import Action, Tool
 
 
 class NodeTool(Tool):
     name = "node"
@@ -12,46 +13,43 @@
     def __init__(self, path=".") -> None:
         super().__init__(path=path)
         cmd = ["git", "ls-files", "**/package.json", "package.json"]
         result = run(cmd)
         if result.returncode != 0 or not result.stdout:
             self.present = False
             return
-        self._actions: List[Action] = []
+        self._actions: list[Action] = []
         for line in result.stdout.split():
             # we consider only up to one level deep files
             if line.count("/") > 1:
                 continue
             parts = line.split("/")
-            if len(parts) == 1:
-                cwd = None
-            else:
-                cwd = parts[0]
-            with open(line, "r", encoding="utf-8") as package_json:
+            cwd = None if len(parts) == 1 else parts[0]
+            with open(line, encoding="utf-8") as package_json:
                 data = json.load(package_json)
                 if "scripts" in data:
-                    for k in data["scripts"].keys():
+                    for k in data["scripts"]:
                         self._actions.append(
                             Action(
                                 name=k,
                                 tool=self,
                                 description=data["scripts"][k],
                                 args=[k],
                                 cwd=cwd,
-                            )
+                            ),
                         )
         self.present = bool(self._actions)
 
     def is_present(self, path: Path) -> bool:
         return self.present
 
-    def actions(self) -> List[Action]:
+    def actions(self) -> list[Action]:
         return self._actions
 
-    def run(self, action: Optional[Action] = None) -> None:
+    def run(self, action: Action | None = None) -> None:
         if not action:
             cmd = ["npm", "run"]
             cwd = None
         else:
             cmd = ["npm", "run", action.name]
             cwd = action.cwd
         run_or_fail(cmd, cwd=cwd, tee=True)
```

### Comparing `mk-2.4.0/src/mk/tools/pre_commit.py` & `mk-2.4.1/src/mk/tools/pre_commit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+from __future__ import annotations
+
 import os
 from pathlib import Path
-from typing import List, Optional
 
 from mk.exec import run_or_fail
 from mk.tools import Action, Tool
 
 
 class PreCommitTool(Tool):
     name = "pre-commit"
 
-    def run(self, action: Optional[Action] = None):
+    def run(self, action: Action | None = None):
         run_or_fail(["pre-commit", "run", "-a"], tee=True)
 
     def is_present(self, path: Path) -> bool:
         if os.path.isfile(os.path.join(path, ".pre-commit-config.yaml")):
             return True
         return False
 
-    def actions(self) -> List[Action]:
+    def actions(self) -> list[Action]:
         return [
-            Action(name="lint", description="[dim]pre-commit run -a[/dim]", tool=self)
+            Action(name="lint", description="[dim]pre-commit run -a[/dim]", tool=self),
         ]
```

### Comparing `mk-2.4.0/src/mk/tools/py_package.py` & `mk-2.4.1/src/mk/tools/py_package.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from __future__ import annotations
+
 import logging
 import sys
 from pathlib import Path
-from typing import List, Optional
 
 from mk.exec import run_or_fail
 from mk.loaders import load_toml
 from mk.tools import Action, Tool
 
 
 class PyPackageTool(Tool):
@@ -13,66 +14,68 @@
 
     name = "pip"
 
     def __init__(self) -> None:
         super().__init__(self)
         self.pkg_name = ""
 
-    def run(self, action: Optional[Action] = None) -> None:
+    def run(self, action: Action | None = None) -> None:
         if not action:
             return
         if action.name in ["build", "install", "uninstall"]:
             cmd = action.args
             run_or_fail(cmd, tee=True)
             run_or_fail(f"{sys.executable} -m twine check dist/*", tee=True)
         else:
-            raise NotImplementedError(f"Action {action.name} not implemented")
+            msg = f"Action {action.name} not implemented"
+            raise NotImplementedError(msg)
 
     def is_present(self, path: Path) -> bool:
         data = load_toml(path / "pyproject.toml")
         self.pkg_name = (
             data.get("project", {}).get("name", "")
             or data.get("tool", {})
             .get("flit", {})
             .get("metadata", {})
             .get("module", "")
             or data.get("tool", {}).get("poetry", {}).get("name", "")
         )
         if not self.pkg_name:
             if (path / "setup.py").exists():
                 self.pkg_name = run_or_fail(
-                    [sys.executable, "setup.py", "--name"], tee=False
+                    [sys.executable, "setup.py", "--name"],
+                    tee=False,
                 ).stdout.strip()
                 return True
             if (path / "setup.cfg").exists():
                 return True
             return False
         return True
 
-    def actions(self) -> List[Action]:
-        actions: List[Action] = []
+    def actions(self) -> list[Action]:
+        actions: list[Action] = []
         if not self.is_present(Path(".")):
             return actions
 
         actions.append(
             Action(
                 name="install",
                 tool=self,
                 description="Use pip to install the current package for current user.",
                 args=["pip3", "install", "-e", "."],
-            )
+            ),
         )
         if self.pkg_name:
             actions.append(
                 Action(
                     name="uninstall",
                     tool=self,
                     description="Use pip to uninstall the current package.",
                     args=["pip3", "uninstall", self.pkg_name],
-                )
+                ),
             )
         try:
             # pylint: disable=import-outside-toplevel,unused-import
             import build  # noqa: F401
 
             actions.append(
                 Action(
@@ -84,15 +87,15 @@
                         "-m",
                         "build",
                         "--sdist",
                         "--wheel",
                         "--outdir",
                         "dist",
                     ],
-                )
+                ),
             )
         except ImportError:
             logging.warning(
-                "Python 'build' package not found, unable to provide build action."
+                "Python 'build' package not found, unable to provide build action.",
             )
 
         return actions
```

### Comparing `mk-2.4.0/src/mk/tools/pytest.py` & `mk-2.4.1/src/mk/tools/pytest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+from __future__ import annotations
+
 import os
 import sys
 from pathlib import Path
-from typing import List, Optional
 
 from mk.exec import run_or_fail
 from mk.loaders import load_toml
 from mk.tools import Action, Tool
 
 
 class PyTestTool(Tool):
     """Expose test command if pytest config is detected."""
 
     name = "pytest"
 
     def __init__(self) -> None:
         super().__init__(self)
 
-    def run(self, action: Optional[Action] = None) -> None:
+    def run(self, action: Action | None = None) -> None:
         if not action:
             return
         if action.name == "test":
             cmd = [sys.executable, "-m", "pytest"]
             run_or_fail(cmd, tee=True)
         return
 
@@ -28,18 +29,18 @@
         if os.path.isfile(path / "pytest.ini"):
             return True
         data = load_toml(path / "pyproject.toml")
         if data and data.get("tool", {}).get("pytest"):
             return True
         return False
 
-    def actions(self) -> List[Action]:
+    def actions(self) -> list[Action]:
         actions = []
         actions.append(
             Action(
                 name="test",
                 tool=self,
                 description="Run pytest",
-            )
+            ),
         )
 
         return actions
```

### Comparing `mk-2.4.0/src/mk/tools/taskfile.py` & `mk-2.4.1/src/mk/tools/taskfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from __future__ import annotations
+
 import json
 import logging
 import os
 import shutil
 import sys
 from pathlib import Path
-from typing import List, Optional
 
 from mk.exec import run_or_fail
 from mk.tools import Action, Tool
 
 
 class TaskfileTool(Tool):
     name = "taskfile"
@@ -21,22 +22,22 @@
     def is_present(self, path: Path) -> bool:
         if os.path.isfile(os.path.join(path, "taskfile.yml")):
             # On some Linux distros might be exposed as taskfile in order to
             # avoid clashing with the other Task Warrior executable https://taskwarrior.org/
             self.executable = shutil.which("taskfile") or shutil.which("task") or ""
             if not self.executable:
                 logging.error(
-                    "taskfile.yml config found but the tool is not installed. See https://taskfile.dev/installation/"
+                    "taskfile.yml config found but the tool is not installed. See https://taskfile.dev/installation/",
                 )
                 sys.exit(1)
             return True
         return False
 
-    def actions(self) -> List[Action]:
-        actions: List[Action] = []
+    def actions(self) -> list[Action]:
+        actions: list[Action] = []
         tasks_json = (
             run_or_fail(
                 ["task", "--list", "--json"],
                 tee=False,
             ).stdout
             or ""
         )
@@ -47,17 +48,14 @@
                 desc += task["summary"]
             actions.append(
                 Action(
                     name=task["name"],
                     tool=self,
                     description=desc,
                     args=[task["name"]],
-                )
+                ),
             )
         return actions
 
-    def run(self, action: Optional[Action] = None) -> None:
-        if not action:
-            cmd = ["task"]
-        else:
-            cmd = ["task", action.name]
+    def run(self, action: Action | None = None) -> None:
+        cmd = ["task"] if not action else ["task", action.name]
         run_or_fail(cmd, tee=True)
```

### Comparing `mk-2.4.0/src/mk/tools/tox.py` & `mk-2.4.1/src/mk/tools/tox.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 """Implementation of the tox tool support."""
+from __future__ import annotations
+
 import logging
 import os
 import re
 import shlex
 import sys
 from configparser import ConfigParser, ParsingError
 from pathlib import Path
-from typing import List, Optional
 
 from mk.exec import run_or_fail
 from mk.text import strip_ansi_escape
 from mk.tools import Action, Tool
 
 
 class ToxTool(Tool):
     name = "tox"
 
     def is_present(self, path: Path) -> bool:
         if os.path.isfile(os.path.join(path, "tox.ini")):
             return True
         return False
 
-    def actions(self) -> List[Action]:
+    def actions(self) -> list[Action]:
         # -a is not supported by tox4!
-        actions: List[Action] = []
+        actions: list[Action] = []
         cp = ConfigParser(strict=False, interpolation=None)
         env_overrides = {"PY_COLORS": "0"}
         result = run_or_fail(
             ["tox", "-qq", "--colored", "no", "--hashseed", "1", "--showconfig"],
             env_overrides=env_overrides,
             tee=False,
         )
         tox_cfg = result.stdout or ""
 
         # workaround for https://github.com/tox-dev/tox/issues/2030
         # we remove all lines starting with .tox from output
         tox_cfg = re.sub(
-            r"^\.tox[^\r\n]*\n$", "", strip_ansi_escape(tox_cfg), re.MULTILINE
+            r"^\.tox[^\r\n]*\n$",
+            "",
+            strip_ansi_escape(tox_cfg),
+            re.MULTILINE,
         )
 
         # now tox_cfg should have a valid ini content
         try:
             cp.read_string(tox_cfg)
         except ParsingError:
             logging.fatal(
-                "Unable to parse tox output from command: %s", shlex.join(result.args)
+                "Unable to parse tox output from command: %s",
+                shlex.join(result.args),
             )
             print(tox_cfg, file=sys.stderr)
             sys.exit(22)
         for section in cp.sections():
             if section.startswith("testenv:"):
                 _, env_name = section.split(":")
                 # we ignore hidden envs like implicit .pkg:
                 if not env_name.startswith("."):
                     actions.append(
                         Action(
                             name=env_name,
                             tool=self,
                             description=cp[section]["description"],
                             args=[env_name],
-                        )
+                        ),
                     )
 
         return actions
 
-    def run(self, action: Optional[Action] = None) -> None:
-        if not action:
-            cmd = ["tox"]
-        else:
-            cmd = ["tox", "-e", action.name]
+    def run(self, action: Action | None = None) -> None:
+        cmd = ["tox"] if not action else ["tox", "-e", action.name]
         run_or_fail(cmd, tee=True)
```

### Comparing `mk-2.4.0/src/mk.egg-info/PKG-INFO` & `mk-2.4.1/src/mk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mk
-Version: 2.4.0
+Version: 2.4.1
 Summary: mk
 Author-email: Sorin Sbarnea <sorin.sbarnea@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/pycontribs/mk
 Project-URL: repository, https://github.com/pycontribs/mk
 Project-URL: changelog, https://github.com/pycontribs/mk/releases
 Keywords: mk
```

### Comparing `mk-2.4.0/src/mk.egg-info/SOURCES.txt` & `mk-2.4.1/src/mk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/src/mk.egg-info/requires.txt` & `mk-2.4.1/src/mk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/test/test_cli.py` & `mk-2.4.1/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `mk-2.4.0/tox.ini` & `mk-2.4.1/tox.ini`

 * *Files identical despite different names*

