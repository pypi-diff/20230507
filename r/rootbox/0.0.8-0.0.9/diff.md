# Comparing `tmp/rootbox-0.0.8.tar.gz` & `tmp/rootbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootbox-0.0.8.tar", last modified: Fri Apr 14 17:50:05 2023, max compression
+gzip compressed data, was "rootbox-0.0.9.tar", last modified: Sat Apr 22 10:15:03 2023, max compression
```

## Comparing `rootbox-0.0.8.tar` & `rootbox-0.0.9.tar`

### file list

```diff
@@ -1,66 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.226235 rootbox-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.218235 rootbox-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-14 17:49:59.000000 rootbox-0.0.8/.github/workflows/multi-test.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-04-14 17:49:59.000000 rootbox-0.0.8/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-04-14 17:49:59.000000 rootbox-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-04-14 17:49:59.000000 rootbox-0.0.8/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-04-14 17:49:59.000000 rootbox-0.0.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (122)      449 2023-04-14 17:49:59.000000 rootbox-0.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-04-14 17:49:59.000000 rootbox-0.0.8/CREDITS.md
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-14 17:49:59.000000 rootbox-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-14 17:49:59.000000 rootbox-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-14 17:50:05.226235 rootbox-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-04-14 17:49:59.000000 rootbox-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-14 17:49:59.000000 rootbox-0.0.8/docs/LXC.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/docs/img/
--rwxr-xr-x   0 runner    (1001) docker     (122)    24714 2023-04-14 17:49:59.000000 rootbox-0.0.8/docs/img/rootbox_0.0.8.png
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-14 17:49:59.000000 rootbox-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-04-14 17:49:59.000000 rootbox-0.0.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-14 17:49:59.000000 rootbox-0.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/rootbox/
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/rootbox/cli/
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/cli/cmd_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/cli/cmd_exec.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/cli/cmd_lxc.py
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/cli/cmd_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/cli/cmd_run.py
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/colorhelper.py
--rw-r--r--   0 runner    (1001) docker     (122)      793 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/download.py
--rw-r--r--   0 runner    (1001) docker     (122)      985 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/enter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.226235 rootbox-0.0.8/rootbox/images/
--rw-r--r--   0 runner    (1001) docker     (122)     1103 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/images/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/images/lxc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/images_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/mount.py
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/path.py
--rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/process.py
--rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/rootfs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/shell.py
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/size.py
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/socket.py
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/tar.py
--rw-r--r--   0 runner    (1001) docker     (122)     1142 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/unshare.py
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/verbose.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/rootbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.226235 rootbox-0.0.8/samples/
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-14 17:49:59.000000 rootbox-0.0.8/samples/test.py
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-14 17:50:05.226235 rootbox-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-14 17:49:59.000000 rootbox-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.226235 rootbox-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      613 2023-04-14 17:49:59.000000 rootbox-0.0.8/tests/test_cmd_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-04-14 17:49:59.000000 rootbox-0.0.8/tests/test_image_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-14 17:49:59.000000 rootbox-0.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.275191 rootbox-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.263191 rootbox-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.271191 rootbox-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      423 2023-04-22 10:14:56.000000 rootbox-0.0.9/.github/workflows/gh-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-22 10:14:56.000000 rootbox-0.0.9/.github/workflows/multi-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      863 2023-04-22 10:14:56.000000 rootbox-0.0.9/.github/workflows/pypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-04-22 10:14:56.000000 rootbox-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-04-22 10:14:56.000000 rootbox-0.0.9/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.271191 rootbox-0.0.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-04-22 10:14:56.000000 rootbox-0.0.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-22 10:14:56.000000 rootbox-0.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-22 10:14:56.000000 rootbox-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-22 10:14:56.000000 rootbox-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-22 10:15:03.275191 rootbox-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-04-22 10:14:56.000000 rootbox-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.271191 rootbox-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-22 10:14:56.000000 rootbox-0.0.9/docs/LXC.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.271191 rootbox-0.0.9/docs/img/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    24714 2023-04-22 10:14:56.000000 rootbox-0.0.9/docs/img/rootbox_0.0.8.png
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-22 10:14:56.000000 rootbox-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-04-22 10:14:56.000000 rootbox-0.0.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-22 10:14:56.000000 rootbox-0.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.271191 rootbox-0.0.9/rootbox/
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.275191 rootbox-0.0.9/rootbox/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/cli/cmd_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/cli/cmd_exec.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/cli/cmd_lxc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/cli/cmd_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/cli/cmd_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/colorhelper.py
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)      985 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/enter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.275191 rootbox-0.0.9/rootbox/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/images/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/images/lxc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/images_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/mount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/mount_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/process.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/rootfs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.275191 rootbox-0.0.9/rootbox/shell/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/shell/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/shell/systeminfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/size.py
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/socket.py
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/tar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1142 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/unshare.py
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-22 10:14:56.000000 rootbox-0.0.9/rootbox/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-22 10:15:03.000000 rootbox-0.0.9/rootbox/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.271191 rootbox-0.0.9/rootbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-22 10:15:03.000000 rootbox-0.0.9/rootbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-04-22 10:15:03.000000 rootbox-0.0.9/rootbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-22 10:15:03.000000 rootbox-0.0.9/rootbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-22 10:15:03.000000 rootbox-0.0.9/rootbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-22 10:15:03.000000 rootbox-0.0.9/rootbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-22 10:15:03.000000 rootbox-0.0.9/rootbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.275191 rootbox-0.0.9/samples/
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-22 10:14:56.000000 rootbox-0.0.9/samples/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-22 10:15:03.275191 rootbox-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-22 10:14:56.000000 rootbox-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 10:15:03.275191 rootbox-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-04-22 10:14:56.000000 rootbox-0.0.9/tests/test_cmd_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-04-22 10:14:56.000000 rootbox-0.0.9/tests/test_image_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      288 2023-04-22 10:14:56.000000 rootbox-0.0.9/tests/test_mount_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-22 10:14:56.000000 rootbox-0.0.9/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-22 10:14:56.000000 rootbox-0.0.9/tox.ini
```

### Comparing `rootbox-0.0.8/.github/workflows/multi-test.yaml` & `rootbox-0.0.9/.github/workflows/multi-test.yaml`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/.github/workflows/release.yaml` & `rootbox-0.0.9/.github/workflows/pypi-release.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -22,22 +22,10 @@
         run: python -m pip install --upgrade pip setuptools wheel
 
       - name: Build a binary wheel and a source tarball
         run: python setup.py sdist bdist_wheel
 
       - name: Publish distribution 📦 to PyPI
         if: startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
-
-  # https://github.com/softprops/action-gh-release
-  create-release:
-    runs-on: ubuntu-latest
-    permissions:
-      contents: write
-    steps:
-    - uses: actions/checkout@v3
-    - name: Release
-      uses: softprops/action-gh-release@v1
-      with:
-        body_path: ${{ github.workspace }}/CHANGELOG.md
```

### Comparing `rootbox-0.0.8/.gitignore` & `rootbox-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/.pre-commit-config.yaml` & `rootbox-0.0.9/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -36,16 +36,15 @@
 
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
     rev: 'v0.0.259'
     hooks:
     - id: ruff
 
-# - repo: local
-#   hooks:
-#     -   id: tox-on-python3.8
-#         name: Run tox in Python 3.8 using rootbox
-#         entry:
-#             python -m rootbox run docker:python:3.8-alpine
-#              "apk add git && pip install tox && tox"
-#         language: system
-#         pass_filenames: false
+- repo: local
+  hooks:
+    -   id: run-pytest
+        name: Run tests using pytest
+        entry:
+            python -m pytest
+        language: system
+        pass_filenames: false
```

### Comparing `rootbox-0.0.8/LICENSE` & `rootbox-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/PKG-INFO` & `rootbox-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Portable reproducible environments for Linux applications
 Home-page: https://github.com/joaompinto/rootbox
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rootbox-0.0.8/README.md` & `rootbox-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/docs/LXC.md` & `rootbox-0.0.9/docs/LXC.md`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/docs/img/rootbox_0.0.8.png` & `rootbox-0.0.9/docs/img/rootbox_0.0.8.png`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/__main__.py` & `rootbox-0.0.9/rootbox/__main__.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/cli/cmd_create.py` & `rootbox-0.0.9/rootbox/cli/cmd_create.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/cli/cmd_pull.py` & `rootbox-0.0.9/rootbox/cli/cmd_pull.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/cli/cmd_run.py` & `rootbox-0.0.9/rootbox/cli/cmd_run.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,56 @@
 """  Create a new environment  """
+import os
+import tarfile
+from pathlib import Path
 from typing import Optional
 
 import typer
 
 from ..download import download_image
 from ..images import parse_image_url
+from ..mount_checker import MountChecker
 from ..rootfs import prepare_rootfs
-from ..shell import raw_execute, shell_execute
+from ..shell.execute import execute
 from ..unshare import CLONE_NEWNET, unshare
 
 
 def run(
     image_name: str = typer.Argument(...),
     no_shell: bool = typer.Option(False, "--no-sh", "--no-shell"),
     no_net: bool = typer.Option(
         False, "--no-network", "-N", help="Disable network in the container"
     ),
+    ram_disk_size: Optional[int] = typer.Option(
+        1, "--ram-disk", "-r", help="Size of the ram disk (GBs)"
+    ),
     command: Optional[str] = typer.Argument(None, help="Command to be run"),
     only_from_cache: bool = typer.Option(False, "--only-from-cache"),
+    tar_file: Optional[Path] = typer.Option(None, "--tar-file", "-t"),
 ):
     if no_shell and command == "/bin/sh":
         raise typer.BadParameter("--no-shell was provided but no command was given")
 
     image = parse_image_url(image_name)
-    image_fname = download_image(image, only_from_cache=only_from_cache)
-    mount_dir = prepare_rootfs(image_fname, in_memory=True, perform_chroot=True)
+    if isinstance(image, Path):
+        image_fname = image
+        image_prompt_name = f"file:{image.name}"
+    else:
+        image_fname = download_image(image, only_from_cache=only_from_cache)
+        image_prompt_name = image_name
+    mount_dir = prepare_rootfs(image_fname, ram_disk_size, perform_chroot=True)
+
     if no_net:
         unshare(CLONE_NEWNET)
-    if no_shell:
-        raw_execute(image_name, mount_dir, command)
-    else:
-        shell_execute(image_name, mount_dir, command)
+    execute(image_prompt_name, mount_dir, command, use_shell=not no_shell)
+    MountChecker.read_mounts()
+    os.chroot("/host_root")
+    if tar_file:
+        with tarfile.open(tar_file, "w:gz") as tar:
+            tar.add(
+                mount_dir, arcname="./", filter=filter_out_other_mounts, recursive=True
+            )
+
+
+def filter_out_other_mounts(tarinfo: tarfile.TarInfo):
+    if MountChecker.is_on_mount_dir(tarinfo.name):
+        return tarinfo
```

### Comparing `rootbox-0.0.8/rootbox/colorhelper.py` & `rootbox-0.0.9/rootbox/colorhelper.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/download.py` & `rootbox-0.0.9/rootbox/download.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/enter.py` & `rootbox-0.0.9/rootbox/enter.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/http.py` & `rootbox-0.0.9/rootbox/http.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/images/__init__.py` & `rootbox-0.0.9/rootbox/images/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 from typing import Union
 
 import typer
 
-from .docker import DockerImage, parse_docker_url
+from .docker import DockerImage
+from .docker import parse_image_url as parse_docker_url
 from .lxc import LXCImage
 
 
 def local_url(path: str) -> Path:
     return Path(path)
 
 
@@ -29,11 +30,11 @@
         return local_url(image_url)
 
     handler, url = image_url.split(":", 1)
 
     if handler == "lxc":
         return LXCImage(*url.split(":"))
     if handler == "docker":
-        return parse_docker_url(url)
+        return DockerImage(*parse_docker_url(url))
     raise typer.BadParameter(
         f"Unknown image handler '{handler}', images must be prefixed with 'lxc:' or 'docker:"
     )
```

### Comparing `rootbox-0.0.8/rootbox/images/docker.py` & `rootbox-0.0.9/rootbox/images/docker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 from os import environ
 from tempfile import NamedTemporaryFile
 
-from drclient.cli.cmd_pull import pull
+from drclient.image import parse_image_url as docker_parse_image_url
+from drclient.image import pull_image
 
 DEFAULT_REGISTRY = environ.get("DOCKER_REGISTRY", "registry-1.docker.io")
 
 
 @dataclass
 class DockerImage:
     registry: str
@@ -25,32 +26,21 @@
     source_reference = f"{registry}/{repository}:{tag}"
     return download(source_reference)
 
 
 def download(image_url):
     # Check if image is on cache
     with NamedTemporaryFile(delete=False) as tmp_file:
-        pull(image_url, tar_file=tmp_file.name, output_directory=None)
+        pull_image(image_url, tar_file=tmp_file.name, output_directory=None)
         tmp_file.flush()
     return tmp_file.name
 
 
-def parse_docker_url(image_name: str) -> tuple:
-    registry = DEFAULT_REGISTRY
-    tag = "latest"
-    if "/" in image_name:
-        first_part, other_parts = image_name.split("/", 1)
-        if "." in first_part:
-            image_name = other_parts
-            registry = f"{first_part}"
-    else:
-        image_name = f"library/{image_name}"
-    if ":" in image_name:
-        image_name, tag = image_name.split(":")
-    return DockerImage(registry, image_name, tag)
+def parse_image_url(image_url: str) -> DockerImage:
+    return docker_parse_image_url(image_url)
 
 
 def url_to_filename(url: str):
     """Convert url to filename"""
     url = url.replace("://", "_")
     url = url.replace("/", "_")
     url = url.replace(":", "_")
```

### Comparing `rootbox-0.0.8/rootbox/images/lxc.py` & `rootbox-0.0.9/rootbox/images/lxc.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/images_cache.py` & `rootbox-0.0.9/rootbox/images_cache.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/mount.py` & `rootbox-0.0.9/rootbox/mount.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/process.py` & `rootbox-0.0.9/rootbox/process.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/rootfs.py` & `rootbox-0.0.9/rootbox/rootfs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 
 from .mount import MS_BIND, MS_PRIVATE, MS_REC, mount
 from .path import path_is_parent
 from .tar import extract_tar
 from .unshare import setup_user_level_root
 
 STD_MOUNTS = [
+    ("/", "host_root/", None, MS_BIND | MS_REC),
     ("/proc", "proc/", None, MS_BIND | MS_REC),
     ("/dev", "dev/", None, MS_BIND | MS_REC),
     ("/sys", "sys/", None, MS_BIND | MS_REC),
     ("tmpfs", "run/", "tmpfs"),
 ]
 
 
-def prepare_rootfs(
-    rootfs_filename: Path, in_memory: bool = True, perform_chroot=True
-) -> Path:
+def prepare_rootfs(rootfs_filename: Path, ram_disk_size, perform_chroot=True) -> Path:
     """Preate a new root mount directory"""
     setup_user_level_root()
     current_path = os.getcwd()
     restore_path = None
     if path_is_parent(os.path.expanduser("~"), current_path):
         restore_path = current_path
 
     mount(None, "/", None, MS_REC | MS_PRIVATE)
     mount_dir = Path(mkdtemp())
-    if in_memory:
-        mount("tmpfs", mount_dir, "tmpfs", options="size=1G")
+    if ram_disk_size:
+        mount("tmpfs", mount_dir, "tmpfs", options=f"size={ram_disk_size}G")
     if ".tar" in rootfs_filename.suffixes:
         extract_tar(rootfs_filename, mount_dir)
     else:
         raise NotImplementedError(f"Unsupported rootfs format: {rootfs_filename}")
     os.chdir(mount_dir)
     for mount_args in STD_MOUNTS:
         os.makedirs(mount_args[1], exist_ok=True)
         mount(*mount_args)
     resolv_conf = Path(f"{mount_dir}/etc/resolv.conf")
     if resolv_conf.is_symlink():
         resolv_conf.unlink()
     if Path(mount_dir, "etc").exists():
         resolv_conf.touch()
         mount("/etc/resolv.conf", f"{mount_dir}/etc/resolv.conf", None, MS_BIND)
+
     if perform_chroot:
         if restore_path:
             target_restore_path = Path(mount_dir, restore_path[1:])
             target_restore_path.mkdir(parents=True)
             mount(restore_path, target_restore_path, None, MS_BIND | MS_REC)
         else:
             target_restore_path = "/"
```

### Comparing `rootbox-0.0.8/rootbox/size.py` & `rootbox-0.0.9/rootbox/size.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/socket.py` & `rootbox-0.0.9/rootbox/socket.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox/unshare.py` & `rootbox-0.0.9/rootbox/unshare.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/rootbox.egg-info/PKG-INFO` & `rootbox-0.0.9/rootbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Portable reproducible environments for Linux applications
 Home-page: https://github.com/joaompinto/rootbox
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rootbox-0.0.8/rootbox.egg-info/SOURCES.txt` & `rootbox-0.0.9/rootbox.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
-CREDITS.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
+.github/workflows/gh-release.yaml
 .github/workflows/multi-test.yaml
-.github/workflows/release.yaml
+.github/workflows/pypi-release.yaml
 .vscode/settings.json
 docs/LXC.md
 docs/img/rootbox_0.0.8.png
 rootbox/__main__.py
 rootbox/colorhelper.py
 rootbox/download.py
 rootbox/enter.py
 rootbox/http.py
 rootbox/images_cache.py
 rootbox/mount.py
+rootbox/mount_checker.py
 rootbox/path.py
 rootbox/process.py
 rootbox/rootfs.py
-rootbox/shell.py
 rootbox/size.py
 rootbox/socket.py
 rootbox/tar.py
 rootbox/unshare.py
 rootbox/verbose.py
 rootbox/version.py
 rootbox.egg-info/PKG-INFO
@@ -44,10 +44,15 @@
 rootbox/cli/cmd_lxc.py
 rootbox/cli/cmd_pull.py
 rootbox/cli/cmd_run.py
 rootbox/cli/main.py
 rootbox/images/__init__.py
 rootbox/images/docker.py
 rootbox/images/lxc.py
+rootbox/shell/__init__.py
+rootbox/shell/execute.py
+rootbox/shell/systeminfo.py
 samples/test.py
 tests/test_cmd_pull.py
-tests/test_image_url.py
+tests/test_image_url.py
+tests/test_mount_checker.py
+tests/test_path.py
```

### Comparing `rootbox-0.0.8/samples/test.py` & `rootbox-0.0.9/samples/test.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/setup.py` & `rootbox-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/tests/test_cmd_pull.py` & `rootbox-0.0.9/tests/test_cmd_pull.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.8/tests/test_image_url.py` & `rootbox-0.0.9/tests/test_image_url.py`

 * *Files identical despite different names*

