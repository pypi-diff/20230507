# Comparing `tmp/genv-0.6.0.tar.gz` & `tmp/genv-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genv-0.6.0.tar", last modified: Wed Mar 15 09:15:00 2023, max compression
+gzip compressed data, was "genv-0.9.0.tar", last modified: Mon May  1 06:07:49 2023, max compression
```

## Comparing `genv-0.6.0.tar` & `genv-0.9.0.tar`

### file list

```diff
@@ -1,42 +1,61 @@
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-03-15 09:15:00.183185 genv-0.6.0/
--rw-r--r--   0 raz       (1001) raz       (1001)     4203 2023-03-15 09:15:00.183185 genv-0.6.0/PKG-INFO
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-03-15 09:15:00.180185 genv-0.6.0/genv/
--rw-r--r--   0 raz       (1001) raz       (1001)      250 2023-02-21 07:32:46.000000 genv-0.6.0/genv/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4246 2023-02-19 16:46:14.000000 genv-0.6.0/genv/devices.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-03-15 09:15:00.181185 genv-0.6.0/genv/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)      103 2023-02-19 16:28:43.000000 genv-0.6.0/genv/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1311 2023-02-19 16:28:43.000000 genv-0.6.0/genv/enforce/execute.py
--rw-r--r--   0 raz       (1001) raz       (1001)      298 2023-02-19 16:28:43.000000 genv-0.6.0/genv/enforce/report.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-03-15 09:15:00.182185 genv-0.6.0/genv/enforce/rules/
--rw-r--r--   0 raz       (1001) raz       (1001)      176 2023-02-19 16:28:43.000000 genv-0.6.0/genv/enforce/rules/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      851 2023-02-19 16:28:43.000000 genv-0.6.0/genv/enforce/rules/env_devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1379 2023-02-19 16:28:43.000000 genv-0.6.0/genv/enforce/rules/env_memory.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1342 2023-02-19 16:28:43.000000 genv-0.6.0/genv/enforce/rules/max_devices_per_user.py
--rw-r--r--   0 raz       (1001) raz       (1001)      526 2023-02-19 16:28:43.000000 genv-0.6.0/genv/enforce/rules/non_env_processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1136 2023-02-19 16:28:43.000000 genv-0.6.0/genv/enforce/survey.py
--rw-r--r--   0 raz       (1001) raz       (1001)     5124 2023-03-15 09:12:29.000000 genv-0.6.0/genv/envs.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1316 2023-02-19 16:28:43.000000 genv-0.6.0/genv/json_.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1704 2023-02-19 16:46:14.000000 genv-0.6.0/genv/nvidia_smi.py
--rw-r--r--   0 raz       (1001) raz       (1001)     2584 2023-03-15 09:12:19.000000 genv-0.6.0/genv/os_.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1253 2023-03-15 09:12:19.000000 genv-0.6.0/genv/poll.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4347 2023-02-19 16:46:14.000000 genv-0.6.0/genv/processes.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-03-15 09:15:00.183185 genv-0.6.0/genv/remote/
--rw-r--r--   0 raz       (1001) raz       (1001)      162 2023-02-19 16:28:43.000000 genv-0.6.0/genv/remote/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      379 2023-02-19 16:28:43.000000 genv-0.6.0/genv/remote/devices.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-03-15 09:15:00.183185 genv-0.6.0/genv/remote/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)       29 2023-02-13 23:02:53.000000 genv-0.6.0/genv/remote/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      640 2023-02-19 16:28:43.000000 genv-0.6.0/genv/remote/enforce/execute.py
--rw-r--r--   0 raz       (1001) raz       (1001)      378 2023-02-19 16:28:43.000000 genv-0.6.0/genv/remote/envs.py
--rw-r--r--   0 raz       (1001) raz       (1001)      383 2023-02-19 16:28:43.000000 genv-0.6.0/genv/remote/processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)      825 2023-02-19 16:28:43.000000 genv-0.6.0/genv/remote/snapshot.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4115 2023-02-19 17:11:13.000000 genv-0.6.0/genv/remote/ssh.py
--rw-r--r--   0 raz       (1001) raz       (1001)      515 2023-02-19 16:28:43.000000 genv-0.6.0/genv/remote/utils.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1200 2023-03-15 09:12:29.000000 genv-0.6.0/genv/snapshot.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3693 2023-02-19 16:28:43.000000 genv-0.6.0/genv/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-03-15 09:15:00.181185 genv-0.6.0/genv.egg-info/
--rw-r--r--   0 raz       (1001) raz       (1001)     4203 2023-03-15 09:15:00.000000 genv-0.6.0/genv.egg-info/PKG-INFO
--rw-r--r--   0 raz       (1001) raz       (1001)      768 2023-03-15 09:15:00.000000 genv-0.6.0/genv.egg-info/SOURCES.txt
--rw-r--r--   0 raz       (1001) raz       (1001)        1 2023-03-15 09:15:00.000000 genv-0.6.0/genv.egg-info/dependency_links.txt
--rw-r--r--   0 raz       (1001) raz       (1001)        5 2023-03-15 09:15:00.000000 genv-0.6.0/genv.egg-info/top_level.txt
--rw-r--r--   0 raz       (1001) raz       (1001)       38 2023-03-15 09:15:00.183185 genv-0.6.0/setup.cfg
--rw-r--r--   0 raz       (1001) raz       (1001)      622 2023-03-15 09:14:57.000000 genv-0.6.0/setup.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.421188 genv-0.9.0/
+-rw-r--r--   0 raz       (1001) raz       (1001)     4737 2023-05-01 06:07:49.421188 genv-0.9.0/PKG-INFO
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.417188 genv-0.9.0/genv/
+-rw-r--r--   0 raz       (1001) raz       (1001)      268 2023-04-30 14:04:42.000000 genv-0.9.0/genv/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     8607 2023-04-30 14:04:42.000000 genv-0.9.0/genv/devices.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.418188 genv-0.9.0/genv/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)      103 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1311 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/execute.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      298 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/report.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.418188 genv-0.9.0/genv/enforce/rules/
+-rw-r--r--   0 raz       (1001) raz       (1001)      176 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/rules/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      851 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/rules/env_devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1379 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/rules/env_memory.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1342 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/rules/max_devices_per_user.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      629 2023-04-13 08:09:45.000000 genv-0.9.0/genv/enforce/rules/non_env_processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1136 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/survey.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.418188 genv-0.9.0/genv/env/
+-rw-r--r--   0 raz       (1001) raz       (1001)      227 2023-04-30 14:04:42.000000 genv-0.9.0/genv/env/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      995 2023-04-30 14:04:42.000000 genv-0.9.0/genv/env/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     6009 2023-04-13 08:09:45.000000 genv-0.9.0/genv/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1348 2023-04-30 14:04:42.000000 genv-0.9.0/genv/json_.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.419188 genv-0.9.0/genv/metrics/
+-rw-r--r--   0 raz       (1001) raz       (1001)      184 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3109 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/collection.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1797 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/metric.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     2663 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/publisher.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      443 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/spec.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3605 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/specs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      157 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/type.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1438 2023-04-04 06:42:45.000000 genv-0.9.0/genv/nvidia_smi.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4311 2023-04-30 14:04:44.000000 genv-0.9.0/genv/os_.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1253 2023-04-17 10:27:35.000000 genv-0.9.0/genv/poll.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4347 2023-04-03 12:05:14.000000 genv-0.9.0/genv/processes.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.420188 genv-0.9.0/genv/remote/
+-rw-r--r--   0 raz       (1001) raz       (1001)      162 2023-03-30 12:58:17.000000 genv-0.9.0/genv/remote/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      379 2023-02-19 16:28:43.000000 genv-0.9.0/genv/remote/devices.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.420188 genv-0.9.0/genv/remote/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       29 2023-02-13 23:02:53.000000 genv-0.9.0/genv/remote/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      640 2023-02-19 16:28:43.000000 genv-0.9.0/genv/remote/enforce/execute.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      378 2023-02-19 16:28:43.000000 genv-0.9.0/genv/remote/envs.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.420188 genv-0.9.0/genv/remote/metrics/
+-rw-r--r--   0 raz       (1001) raz       (1001)       35 2023-04-04 06:42:45.000000 genv-0.9.0/genv/remote/metrics/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1730 2023-04-04 06:42:45.000000 genv-0.9.0/genv/remote/metrics/collection.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      383 2023-02-19 16:28:43.000000 genv-0.9.0/genv/remote/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      825 2023-03-30 12:58:17.000000 genv-0.9.0/genv/remote/snapshot.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3179 2023-04-04 06:42:45.000000 genv-0.9.0/genv/remote/ssh.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      515 2023-02-19 16:28:43.000000 genv-0.9.0/genv/remote/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.421188 genv-0.9.0/genv/runners/
+-rw-r--r--   0 raz       (1001) raz       (1001)       59 2023-04-04 06:42:45.000000 genv-0.9.0/genv/runners/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      687 2023-04-04 06:42:45.000000 genv-0.9.0/genv/runners/local.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     2046 2023-04-04 06:42:45.000000 genv-0.9.0/genv/runners/runner.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     2425 2023-04-04 06:42:45.000000 genv-0.9.0/genv/runners/ssh.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1499 2023-04-04 06:42:45.000000 genv-0.9.0/genv/snapshot.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4069 2023-04-30 14:04:42.000000 genv-0.9.0/genv/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.417188 genv-0.9.0/genv.egg-info/
+-rw-r--r--   0 raz       (1001) raz       (1001)     4737 2023-05-01 06:07:49.000000 genv-0.9.0/genv.egg-info/PKG-INFO
+-rw-r--r--   0 raz       (1001) raz       (1001)     1130 2023-05-01 06:07:49.000000 genv-0.9.0/genv.egg-info/SOURCES.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)        1 2023-05-01 06:07:49.000000 genv-0.9.0/genv.egg-info/dependency_links.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)        5 2023-05-01 06:07:49.000000 genv-0.9.0/genv.egg-info/top_level.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)       38 2023-05-01 06:07:49.421188 genv-0.9.0/setup.cfg
+-rw-r--r--   0 raz       (1001) raz       (1001)      622 2023-05-01 06:01:25.000000 genv-0.9.0/setup.py
```

### Comparing `genv-0.6.0/PKG-INFO` & `genv-0.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,63 @@
 Metadata-Version: 2.1
 Name: genv
-Version: 0.6.0
+Version: 0.9.0
 Summary: GPU Environment Management
 Home-page: https://github.com/run-ai/genv
 Author: Run:AI
 Author-email: pypi@run.ai
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="images/genv blade landscape black@4x.png#gh-light-mode-only" width="600" alt="genv"/>
   <img src="images/genv blade landscape white@4x.png#gh-dark-mode-only" width="600" alt="genv"/>
 </p>
 
-# genv (GPU Environment Management) [![Join the community at (https://discord.gg/zN3Q9pQAuT)](https://img.shields.io/badge/Discord-genv-7289da?logo=discord)](https://discord.gg/zN3Q9pQAuT) [![Join the chat at https://gitter.im/run-ai-genv/community](https://badges.gitter.im/run-ai-genv/community.svg)](https://gitter.im/run-ai-genv/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+# Genv (GPU Environment Management) [![Join the community at (https://discord.gg/zN3Q9pQAuT)](https://img.shields.io/badge/Discord-genv-7289da?logo=discord)](https://discord.gg/zN3Q9pQAuT)
 
-
-*genv* lets you easily control, configure and monitor the GPU resources that you are using.
+Genv lets you easily control, configure and monitor the GPU resources that you are using.
 
 It is intendend to ease up the process of GPU allocation for data scientists without code changes 💪🏻
 
 This project was highly inspired by [pyenv](https://github.com/pyenv/pyenv) and other version, package and environment management software like [Conda](https://docs.conda.io/projects/conda/en/latest/), [nvm](https://github.com/nvm-sh/nvm), [rbenv](https://github.com/rbenv/rbenv).
 
 ![Example](images/example.png)
 
-## 🔥 Why You Should use *genv*
-
-Because with *genv*, you will:
+## 🔥 Why Genv?
 
 - Easily share GPUs with your teammates
 - Find available GPUs for you to use - on-prem or on cloud via remote access
 - Pool the GPUs from multiple machines, allocate the available machine without SSH-ing every one of them
 - Switch between GPUs without code changes
 - Reserve GPU resources for as long as you use them with no one else hijacking them
 - Reproduce your experiment environment easily
 - Save time while collaborating
 
 Plus, it's 100% free and gets installed before you can say Jack Robinson.
 
+## Documentation
+
+Check out the Genv [documentation site](https://docs.genv.dev).
+
+
+## 🏃🏻 Join us in the AI Infrastructure Club!
+
+[<img src="https://img.shields.io/badge/Discord-Join%20the%20community!-7289da?style=for-the-badge&logo=discord&logoColor=7289da" height="30" />](https://discord.gg/zN3Q9pQAuT)
+
+Looking for a place to discuss best practices, discover new tools, and exchange ideas about how to make the most out of our GPUs without losing time? Join the Discord server with the creators of Genv and [*rntop*](https://github.com/run-ai/rntop) - start building your models faster!
+
+- Installation and setup support as well as best practice tips and tricks directly for your use-case
+- Discuss possible features
+- Monthly Beers with Engineers sessions with amazing guests
+- Networking events
+- and many more...
+
 ## 🎉 Simple Integration & Usage with your fav IDE
 
 
 Integration with VSCode [(Take me to the installation guide!)](https://github.com/run-ai/vscode-genv) |
 :-------------------------:|
 <img src="images/overview.gif" width="800" alt="genv vscode"/> |
 
@@ -53,33 +67,43 @@
 :-------------------------:|
 <img src="images/overview_jupyterlab.gif" width="800" alt="genv jupyterlab"/> |
 
 
 
 A PyCharm integration is also in our roadmap so stay tuned!
 
-## Documentation
-
-Check out the genv [documentation site](https://run-ai.github.io/genv).
-
-
-## 🏃🏻 Be an early runner in the AI Infrastructure Club!
-
-[<img src="https://img.shields.io/badge/Discord-Join%20the%20community!-7289da?style=for-the-badge&logo=discord&logoColor=7289da" height="30" />](https://discord.gg/zN3Q9pQAuT)
-
-Looking for a place to discuss best practices, discover new tools, and exchange ideas about how to make the most out of our GPUs without losing time? Join the Discord server with the creators of *genv* and [*rntop*](https://github.com/run-ai/rntop) - start building your models faster!
-
-- Installation and setup support as well as best practice tips and tricks directly for your use-case
-- Discuss possible features
-- Monthly Beers with Engineers sessions with amazing guests
-- Networking events 
-- and many more...
-
-## 🏆 Special Thanks for Runners
-
-- You could be mentioned here! Submit a feature request to be featured here 💥
 
 ## License
-The genv software is Copyright 2022 [Run.ai Labs, Ltd.].
+The Genv software is Copyright 2022 [Run.ai Labs, Ltd.].
 The software is licensed by Run.ai under the AGPLv3 license.
 Please note that Run.ai’s intention in licensing the software are that the obligations of licensee pursuant to the AGPLv3 license should be interpreted broadly.
 For example, Run.ai’s intention is that the terms “work based on the Program” in Section 0 of the AGPLv3 license, and “Corresponding Source” in Section 1 of the AGPLv3 license, should be interpreted as broadly as possible to the extent permitted under applicable law.
+
+Genv Remote vs. Run.ai
+----------------------
+1. containers vs environments
+2. SSH vs k8s
+3. interception- vs monitoring-based enfircements
+4. non-centralized (no load balancing)
+5. no advanced user roles (everyone can list envs and devices)
+6. shim-based visualization vs. interception-based virtualization
+7. environment must fit in a node vs. multi-node workload
+8. no compute mgmt
+
+
+QUOTA:
+-----
+system:
+    [V] (nvidia-smi)      non env processes
+    [V] (nvidia-smi)      processes from envs on non-attached devices
+    [ ] (envs.json)       timeout
+
+resources:
+    [V] (devices.json)    num of attached devices
+
+    (later...)
+    [ ] (nvidia-smi)      num of processes (as an alternative to compute mgmt)
+    [ ] (envs.json)       num of active envs
+    [ ] (envs.json)       num of machines with active envs
+    [ ] (nvidia-smi)      amount of GPU memory (per device/total)
+
+https://grafana.com/docs/grafana/latest/cli/#override-homepath-value
```

### Comparing `genv-0.6.0/genv/devices.py` & `genv-0.9.0/genv/processes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,151 +1,164 @@
+import asyncio
 from dataclasses import dataclass
-import subprocess
-from typing import Dict, Iterable, Optional
+import sys
+from typing import Iterable, Optional
 
-
-# NOTE(raz): This should be the layer that queries and controls the state of Genv regarding devices.
-# Currently, it relies on executing the device manager executable of Genv, as this is where the logic is implemented.
-# This however should be done oppositely.
-# The entire logic that queries and controls devices.json should be implemented here, and the device manager executable
-# should use methods from here.
-# It should take the Genv lock for the atomicity of the transaction, and print output as needed.
-# The current architecture has an inherent potential deadlock because each manager locks a different lock, and might
-# call the other manager.
+from . import nvidia_smi
+from . import os_
+from . import utils
 
 
 @dataclass
-class Device:
-    index: int
-    eids: Iterable[str]
+class Process:
+    """
+    A compute running process either from an environment or not.
+    """
+
+    @dataclass
+    class Usage:
+        """
+        The GPU index and amount of GPU memory used by the process.
+        """
+
+        index: int
+        gpu_memory: str
+
+        @property
+        def bytes(self) -> int:
+            return utils.memory_to_bytes(self.gpu_memory)
+
+    pid: int
+    used_gpu_memory: Iterable[Usage]
+    eid: Optional[str]
 
     @property
-    def attached(self) -> bool:
-        return len(self.eids) > 0
+    def indices(self) -> Iterable[int]:
+        return [usage.index for usage in self.used_gpu_memory]
 
     @property
-    def detached(self) -> bool:
-        return len(self.eids) == 0
+    def total_bytes(self) -> int:
+        return sum(usage.bytes for usage in self.used_gpu_memory)
+
+    def __hash__(self) -> int:
+        return self.pid.__hash__()
+
+    def filter(self, *, index: int):
+        """
+        Returns a new process with information only of the given device index.
+        """
+        return Process(
+            self.pid,
+            [usage for usage in self.used_gpu_memory if usage.index == index],
+            self.eid,
+        )
 
-    def filter(self, *, eids: Iterable[str]):
+    @staticmethod
+    def eid(pid: int) -> Optional[str]:
         """
-        Returns a new device with only the given environment identifiers.
+        Returns the environment identifier of the process with the given pid.
+        Returns None if the process is not running in an environment or if it could not be queried.
         """
-        return Device(self.index, [eid for eid in self.eids if eid in eids])
+        try:
+            return os_.get_process_environ(pid).get("GENV_ENVIRONMENT_ID")
+        except PermissionError:
+            print(
+                f"[WARNING] Not enough permissions to query environment of process {pid}",
+                file=sys.stderr,
+            )
+        except FileNotFoundError:
+            print(f"[DEBUG] Process {pid} already terminated", file=sys.stderr)
 
 
 @dataclass
 class Snapshot:
     """
-    A snapshot of devices.
+    A snapshot of running processes.
     """
 
-    devices: Iterable[Device]
+    processes: Iterable[Process]
 
     @property
-    def indices(self) -> Iterable[int]:
-        return [device.index for device in self.devices]
+    def pids(self) -> Iterable[int]:
+        return [process.pid for process in self.processes]
 
     def __iter__(self):
-        return self.devices.__iter__()
+        return self.processes.__iter__()
 
     def __len__(self):
-        return self.devices.__len__()
+        return self.processes.__len__()
 
-    def __getitem__(self, index: int) -> Device:
-        return next(device for device in self.devices if device.index == index)
+    def __getitem__(self, pid: int) -> Process:
+        return next(process for process in self.processes if process.pid == pid)
 
     def filter(
         self,
         deep: bool = True,
         *,
-        indices: Optional[Iterable[int]] = None,
+        pids: Optional[Iterable[int]] = None,
         eid: Optional[str] = None,
         eids: Optional[Iterable[str]] = None,
-        attached: Optional[bool] = None,
+        index: Optional[int] = None,
     ):
         """
         Returns a new filtered snapshot.
 
         :param deep: Perform deep filtering
-        :param indices: Device indices to keep
+        :param pids: Process identifiers to keep
         :param eid: Environment identifier to keep
         :param eids: Environment identifiers to keep
-        :param attached: Keep only devices with environments attached or not
+        :param username: Username to keep
         """
         if eids:
             eids = set(eids)
 
         if eid:
             if not eids:
                 eids = set()
 
             eids.add(eid)
 
-        devices = self.devices
+        processes = self.processes
 
-        if indices is not None:
-            devices = [device for device in devices if device.index in indices]
+        if pids is not None:
+            processes = [process for process in processes if process.pid in pids]
 
         if eids is not None:
-            if deep:
-                devices = [device.filter(eids=eids) for device in devices]
-
-            devices = [
-                device
-                for device in devices
-                if any((eid in eids) for eid in device.eids)
-            ]
-
-        if attached is not None:
-            if attached:
-                devices = [device for device in devices if device.attached]
-            else:
-                devices = [device for device in devices if device.detached]
-
-        return Snapshot(devices)
+            processes = [process for process in processes if process.eid in eids]
 
+        if index is not None:
+            if deep:
+                processes = [process.filter(index=index) for process in processes]
 
-def snapshot() -> Snapshot:
-    return Snapshot([Device(index, d["eids"]) for index, d in ps().items()])
+            processes = [process for process in processes if index in process.indices]
 
+        return Snapshot(processes)
 
-def ps() -> Dict[int, Iterable[str]]:
-    """
-    Returns information about device and active attachments.
 
-    :return: A mapping between device index and all attached environment identifiers
+async def snapshot() -> Snapshot:
     """
-    devices = dict()
-
-    for line in (
-        subprocess.check_output(
-            "genv exec devices ps --no-header --format csv", shell=True
-        )
-        .decode("utf-8")
-        .strip()
-        .splitlines()
-    ):
-        index, eid, _, _ = line.split(",")
-        index = int(index)
-
-        if index not in devices:
-            devices[index] = {"eids": []}
-
-        if eid:
-            devices[index]["eids"].append(eid)
-
-    return devices
-
-
-def detach(eid: str, index: int) -> None:
+    Returns a snapshot of all running compute processes.
     """
-    Detaches an environment from a device.
+    uuids, apps = await asyncio.gather(
+        nvidia_smi.device_uuids(), nvidia_smi.compute_apps()
+    )
 
-    :param eid: Environment identifier
-    :param index: Device index
-    :return: None
-    """
-    # TODO(raz): support detaching from multiple devices at the same time
-    subprocess.check_call(
-        f"genv exec devices detach --quiet --eid {eid} --index {index}", shell=True
+    pid_to_apps = {
+        pid: [app for app in apps if app["pid"] == pid]
+        for pid in set(app["pid"] for app in apps)
+    }
+
+    return Snapshot(
+        [
+            Process(
+                pid=pid,
+                used_gpu_memory=[
+                    Process.Usage(
+                        index=uuids[app["gpu_uuid"]], gpu_memory=app["used_gpu_memory"]
+                    )
+                    for app in apps
+                ],
+                eid=Process.eid(pid),
+            )
+            for pid, apps in pid_to_apps.items()
+        ]
     )
```

### Comparing `genv-0.6.0/genv/enforce/execute.py` & `genv-0.9.0/genv/enforce/execute.py`

 * *Files identical despite different names*

### Comparing `genv-0.6.0/genv/enforce/rules/env_devices.py` & `genv-0.9.0/genv/enforce/rules/env_devices.py`

 * *Files identical despite different names*

### Comparing `genv-0.6.0/genv/enforce/rules/env_memory.py` & `genv-0.9.0/genv/enforce/rules/env_memory.py`

 * *Files identical despite different names*

### Comparing `genv-0.6.0/genv/enforce/rules/max_devices_per_user.py` & `genv-0.9.0/genv/enforce/rules/max_devices_per_user.py`

 * *Files identical despite different names*

### Comparing `genv-0.6.0/genv/enforce/rules/non_env_processes.py` & `genv-0.9.0/genv/enforce/rules/non_env_processes.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 def non_env_processes(*surveys: Survey) -> None:
     """
     Terminates processes that are not running in environments.
     """
     for survey in surveys:
         for process in survey.snapshot.processes:
             if process.eid is not None:
+                # TODO(raz): should we make sure that the environment actually exists in the snapshot?
                 continue
 
             print(
                 f"{f'[{survey.hostname}] ' if survey.hostname else ''}"
                 f"Process {process.pid} is not running in a GPU environment"
             )
```

### Comparing `genv-0.6.0/genv/enforce/survey.py` & `genv-0.9.0/genv/enforce/survey.py`

 * *Files identical despite different names*

### Comparing `genv-0.6.0/genv/envs.py` & `genv-0.9.0/genv/envs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 import subprocess
-from typing import Dict, Iterable, Optional, Union
+from typing import Any, Dict, Iterable, Optional, Union
 
 from . import utils
 
 # NOTE(raz): This should be the layer that queries and controls the state of Genv regarding active environments.
 # Currently, it relies on executing the environment manager executable of Genv, as this is where the logic is implemented.
 # This however should be done oppositely.
 # The entire logic that queries and controls envs.json should be implemented here, and the environment manager executable
@@ -44,14 +44,18 @@
 
     envs: Iterable[Env]
 
     @property
     def eids(self) -> Iterable[str]:
         return [env.eid for env in self.envs]
 
+    @property
+    def usernames(self) -> Iterable[str]:
+        return set(env.username for env in self.envs if env.username)
+
     def __iter__(self):
         return self.envs.__iter__()
 
     def __len__(self):
         return self.envs.__len__()
 
     def __getitem__(self, eid: str) -> Env:
@@ -171,15 +175,49 @@
     :return: A mapping from environment identifier to its configured name or None if not configured.
     """
     return {
         eid: (name or None) for eid, name in query("config.name", eids=True).items()
     }
 
 
+def gpus(eid: str) -> Optional[int]:
+    """
+    Returns the configured device count an environment.
+    """
+    s = query("config.gpus", eid=eid)
+
+    return int(s) if s else None
+
+
 def gpu_memory(eid: str) -> Optional[str]:
     """
     Returns the configured amount of GPU memory of an environment.
 
     :param eid: Environment to query
     :return: The configured amount of GPU memory or None if not configured
     """
     return query("config.gpu_memory", eid=eid) or None
+
+
+def activate(eid: str, uid: int, pid: int) -> None:
+    """
+    Activates an environment.
+    """
+    subprocess.check_output(
+        f"genv exec envs activate --eid {eid} --uid {uid} --pid {pid}",
+        shell=True,
+    )
+
+
+def configure(eid: str, command: str, value: Any) -> None:
+    """
+    Configures an environment.
+    """
+    ARGUMENTS = {
+        "gpus": "--count",
+        "gpu-memory": "--gpu-memory",
+    }
+
+    subprocess.check_output(
+        f"genv exec envs config --eid {eid} {command} {ARGUMENTS[command]} {str(value)}",
+        shell=True,
+    )
```

### Comparing `genv-0.6.0/genv/json_.py` & `genv-0.9.0/genv/json_.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from . import processes
 from .snapshot import Snapshot
 from .enforce import Report
 
 # TODO(raz): test here that all types have a different set of keys for creation
 Types = [
     devices.Device,
+    devices.Device.Attachement,
     devices.Snapshot,
     envs.Env,
     envs.Env.Config,
     envs.Snapshot,
     processes.Process,
     processes.Process.Usage,
     processes.Snapshot,
```

### Comparing `genv-0.6.0/genv/poll.py` & `genv-0.9.0/genv/poll.py`

 * *Files identical despite different names*

### Comparing `genv-0.6.0/genv/remote/enforce/execute.py` & `genv-0.9.0/genv/remote/enforce/execute.py`

 * *Files identical despite different names*

### Comparing `genv-0.6.0/genv/remote/snapshot.py` & `genv-0.9.0/genv/remote/snapshot.py`

 * *Files identical despite different names*

### Comparing `genv-0.6.0/genv/remote/ssh.py` & `genv-0.9.0/genv/remote/ssh.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from dataclasses import dataclass
-import os
 import sys
 from typing import Any, Callable, Iterable, Optional, Tuple
 
 from .utils import reprint
+from ..runners.ssh import SshRunner
 
 
 @dataclass
 class Host:
     """
     Host configuration.
 
@@ -45,85 +45,43 @@
     :param sudo: Run command as root using sudo
     """
 
     args: Iterable[str]
     sudo: bool = False
 
 
-async def start(host: Host, command: Command, stdin: int) -> asyncio.subprocess.Process:
-    """
-    Starts a background process that runs a Genv command on a remote host over SSH.
-
-    :param host: Host configuration
-    :param command: Genv command specification
-    :param stdin: Standard input
-
-    :return: Returns the SSH process
-    """
-    args = []
-
-    if host.timeout is not None:
-        args.append(f"-o ConnectTimeout={host.timeout}")
-
-    path = f"$PATH:{host.root}/bin"
-
-    # add development shims to remote $PATH if in the local $PATH
-    if os.path.realpath(os.path.join(os.environ["GENV_ROOT"], "devel/shims")) in [
-        os.path.realpath(path) for path in os.environ["PATH"].split(":")
-    ]:
-        path = f"{path}:{host.root}/devel/shims"
-
-    cmd = f'env PATH="{path}" genv {" ".join(command.args)}'
-
-    if command.sudo:
-        cmd = f"sudo {cmd}"
-
-    return await asyncio.create_subprocess_exec(
-        "ssh",
-        *args,
-        host.hostname,
-        cmd,
-        stdin=stdin,
-        stdout=asyncio.subprocess.PIPE,
-        stderr=asyncio.subprocess.PIPE,
-    )
-
-
 async def run(
     config: Config, command: Command, stdins: Optional[Iterable[str]] = None
 ) -> Tuple[Iterable[Host], Iterable[str]]:
     """
     Runs a Genv command on multiple hosts over SSH.
     Waits for the command to finish on all hosts.
     Raises 'RuntimeError' if failed to connect to any of the hosts and 'config.throw_on_error' is True.
 
     :param config: Execution configuration
     :param command: Genv command specification
     :param stdins: Input to send per host
 
     :return: Returns the hosts that succeeded and their standard outputs
     """
-    processes = [
-        await start(
-            host,
-            command,
-            asyncio.subprocess.PIPE if stdins else asyncio.subprocess.DEVNULL,
-        )
-        for host in config.hosts
-    ]
+    ssh_runners_and_inputs = []
+    for host, stdin in zip(config.hosts, stdins or [None for _ in config.hosts]):
+        ssh_runner = SshRunner(host.hostname, host.timeout, {'PATH': SshRunner.calc_remote_path_env(host.root)})
+        ssh_runners_and_inputs.append((ssh_runner, stdin))
 
-    outputs = await asyncio.gather(
+    ssh_outputs = await asyncio.gather(
         *(
-            process.communicate(stdin.encode("utf-8") if stdin else None)
-            for process, stdin in zip(processes, stdins or [None for _ in config.hosts])
+            ssh_runner.run("genv", *command.args, stdin=stdin, sudo=command.sudo)
+            for ssh_runner, stdin in ssh_runners_and_inputs
         )
     )
 
-    stdouts = [stdout.decode("utf-8").strip() for stdout, _ in outputs]
-    stderrs = [stderr.decode("utf-8").strip() for _, stderr in outputs]
+    processes = [runner_output.command_process for runner_output in ssh_outputs]
+    stdouts = [runner_output.stdout for runner_output in ssh_outputs]
+    stderrs = [runner_output.stderr for runner_output in ssh_outputs]
 
     def filter(
         objs: Iterable[Any], pred: Callable[[asyncio.subprocess.Process], bool]
     ) -> Iterable[Any]:
         return [obj for process, obj in zip(processes, objs) if pred(process)]
 
     def succeeded(objs: Iterable[Any]) -> Iterable[Any]:
```

### Comparing `genv-0.6.0/genv/remote/utils.py` & `genv-0.9.0/genv/remote/utils.py`

 * *Files identical despite different names*

### Comparing `genv-0.6.0/genv/utils.py` & `genv-0.9.0/genv/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 from contextlib import contextmanager
 from datetime import datetime
 import json
 import os
-from pathlib import Path
-from typing import Callable, Dict, Optional, Union
+from typing import Any, Callable, Dict, Optional, Type, Union
 
-from .os_ import Umask, Flock
+from .os_ import access_lock
 
 DATETIME_FMT = "%d/%m/%Y %H:%M:%S"
 MEMORY_TO_BYTES_MULTIPLIERS_DICT = {
     "b": 1,
     "k": 1000,
     "m": 1000 * 1000,
     "g": 1000 * 1000 * 1000,
     "ki": 1024,
     "mi": 1024 * 1024,
     "gi": 1024 * 1024 * 1024,
 }
 
 
+def get_temp_file_path(filename: str) -> str:
+    """
+    Returns the path of a file with the provided name in the Genv temporary directory.
+    """
+    return os.path.join(os.environ.get("GENV_TMPDIR", "/var/tmp/genv"), filename)
+
+
 @contextmanager
 def access_json(
     filename: str,
     factory: Callable[[], Dict],
     *,
-    convert: Optional[Callable[[Dict], None]] = None,
+    convert: Optional[Callable[[Any], Any]] = None,
     reset: bool = False,
+    json_decoder: Optional[Type[json.JSONDecoder]] = None,
+    json_encoder: Optional[Type[json.JSONEncoder]] = None,
 ):
     """
     This function returns a json object representing a genv state data.
     The state object will either be created or loaded from a cache file, and updated with the correct data.
     At the end of the caller process, the state object will be writen into the cache file.
 
 
@@ -37,35 +45,34 @@
             The base path of the file is either GENV_TMPDIR (if defined) or /var/tmp/genv.
     :param factory: A function creating a "clean" instance of the state object
     :param convert: A convertor function mutating the state object
                      to the correct form (backward compatibility / updating)
     :param reset: If the reset flag is on,
     :return:
     """
-    path = os.path.join(os.environ.get("GENV_TMPDIR", "/var/tmp/genv"), filename)
-
-    with Umask(0):
-        Path(path).parent.mkdir(parents=True, exist_ok=True, mode=0o777)
+    path = get_temp_file_path(filename)
 
-        with Flock(f"{path}.lock", 0o666):
-            if os.path.exists(path) and not reset:
-                with open(path) as f:
-                    o = json.load(f)
-
-                    if convert:
-                        convert(o)
-            else:
-                o = factory()
-
-            yield o
-
-            with open(
-                path, "w", opener=lambda path, flags: os.open(path, flags, 0o666)
-            ) as f:
-                json.dump(o, f, indent=4)
+    with access_lock(f"{path}.lock"):
+        if os.path.exists(path) and not reset:
+            with open(path) as f:
+                o = json.load(f, cls=json_decoder)
+
+                if convert:
+                    o = convert(o)
+        else:
+            o = factory()
+
+        yield o
+
+        # TODO(raz): are probably relying on the umask being set to 0 thanks to access_lock().
+        # this is not part of the API of the method so we probably need to do it here as well.
+        with open(
+            path, "w", opener=lambda path, flags: os.open(path, flags, 0o666)
+        ) as f:
+            json.dump(o, f, cls=json_encoder, indent=2)
 
 
 def memory_to_bytes(cap: str) -> int:
     """
     Convert memory string to an integer value in bytes.
     """
     for unit, multiplier in MEMORY_TO_BYTES_MULTIPLIERS_DICT.items():
```

### Comparing `genv-0.6.0/genv.egg-info/PKG-INFO` & `genv-0.9.0/genv.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,63 @@
 Metadata-Version: 2.1
 Name: genv
-Version: 0.6.0
+Version: 0.9.0
 Summary: GPU Environment Management
 Home-page: https://github.com/run-ai/genv
 Author: Run:AI
 Author-email: pypi@run.ai
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="images/genv blade landscape black@4x.png#gh-light-mode-only" width="600" alt="genv"/>
   <img src="images/genv blade landscape white@4x.png#gh-dark-mode-only" width="600" alt="genv"/>
 </p>
 
-# genv (GPU Environment Management) [![Join the community at (https://discord.gg/zN3Q9pQAuT)](https://img.shields.io/badge/Discord-genv-7289da?logo=discord)](https://discord.gg/zN3Q9pQAuT) [![Join the chat at https://gitter.im/run-ai-genv/community](https://badges.gitter.im/run-ai-genv/community.svg)](https://gitter.im/run-ai-genv/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+# Genv (GPU Environment Management) [![Join the community at (https://discord.gg/zN3Q9pQAuT)](https://img.shields.io/badge/Discord-genv-7289da?logo=discord)](https://discord.gg/zN3Q9pQAuT)
 
-
-*genv* lets you easily control, configure and monitor the GPU resources that you are using.
+Genv lets you easily control, configure and monitor the GPU resources that you are using.
 
 It is intendend to ease up the process of GPU allocation for data scientists without code changes 💪🏻
 
 This project was highly inspired by [pyenv](https://github.com/pyenv/pyenv) and other version, package and environment management software like [Conda](https://docs.conda.io/projects/conda/en/latest/), [nvm](https://github.com/nvm-sh/nvm), [rbenv](https://github.com/rbenv/rbenv).
 
 ![Example](images/example.png)
 
-## 🔥 Why You Should use *genv*
-
-Because with *genv*, you will:
+## 🔥 Why Genv?
 
 - Easily share GPUs with your teammates
 - Find available GPUs for you to use - on-prem or on cloud via remote access
 - Pool the GPUs from multiple machines, allocate the available machine without SSH-ing every one of them
 - Switch between GPUs without code changes
 - Reserve GPU resources for as long as you use them with no one else hijacking them
 - Reproduce your experiment environment easily
 - Save time while collaborating
 
 Plus, it's 100% free and gets installed before you can say Jack Robinson.
 
+## Documentation
+
+Check out the Genv [documentation site](https://docs.genv.dev).
+
+
+## 🏃🏻 Join us in the AI Infrastructure Club!
+
+[<img src="https://img.shields.io/badge/Discord-Join%20the%20community!-7289da?style=for-the-badge&logo=discord&logoColor=7289da" height="30" />](https://discord.gg/zN3Q9pQAuT)
+
+Looking for a place to discuss best practices, discover new tools, and exchange ideas about how to make the most out of our GPUs without losing time? Join the Discord server with the creators of Genv and [*rntop*](https://github.com/run-ai/rntop) - start building your models faster!
+
+- Installation and setup support as well as best practice tips and tricks directly for your use-case
+- Discuss possible features
+- Monthly Beers with Engineers sessions with amazing guests
+- Networking events
+- and many more...
+
 ## 🎉 Simple Integration & Usage with your fav IDE
 
 
 Integration with VSCode [(Take me to the installation guide!)](https://github.com/run-ai/vscode-genv) |
 :-------------------------:|
 <img src="images/overview.gif" width="800" alt="genv vscode"/> |
 
@@ -53,33 +67,43 @@
 :-------------------------:|
 <img src="images/overview_jupyterlab.gif" width="800" alt="genv jupyterlab"/> |
 
 
 
 A PyCharm integration is also in our roadmap so stay tuned!
 
-## Documentation
-
-Check out the genv [documentation site](https://run-ai.github.io/genv).
-
-
-## 🏃🏻 Be an early runner in the AI Infrastructure Club!
-
-[<img src="https://img.shields.io/badge/Discord-Join%20the%20community!-7289da?style=for-the-badge&logo=discord&logoColor=7289da" height="30" />](https://discord.gg/zN3Q9pQAuT)
-
-Looking for a place to discuss best practices, discover new tools, and exchange ideas about how to make the most out of our GPUs without losing time? Join the Discord server with the creators of *genv* and [*rntop*](https://github.com/run-ai/rntop) - start building your models faster!
-
-- Installation and setup support as well as best practice tips and tricks directly for your use-case
-- Discuss possible features
-- Monthly Beers with Engineers sessions with amazing guests
-- Networking events 
-- and many more...
-
-## 🏆 Special Thanks for Runners
-
-- You could be mentioned here! Submit a feature request to be featured here 💥
 
 ## License
-The genv software is Copyright 2022 [Run.ai Labs, Ltd.].
+The Genv software is Copyright 2022 [Run.ai Labs, Ltd.].
 The software is licensed by Run.ai under the AGPLv3 license.
 Please note that Run.ai’s intention in licensing the software are that the obligations of licensee pursuant to the AGPLv3 license should be interpreted broadly.
 For example, Run.ai’s intention is that the terms “work based on the Program” in Section 0 of the AGPLv3 license, and “Corresponding Source” in Section 1 of the AGPLv3 license, should be interpreted as broadly as possible to the extent permitted under applicable law.
+
+Genv Remote vs. Run.ai
+----------------------
+1. containers vs environments
+2. SSH vs k8s
+3. interception- vs monitoring-based enfircements
+4. non-centralized (no load balancing)
+5. no advanced user roles (everyone can list envs and devices)
+6. shim-based visualization vs. interception-based virtualization
+7. environment must fit in a node vs. multi-node workload
+8. no compute mgmt
+
+
+QUOTA:
+-----
+system:
+    [V] (nvidia-smi)      non env processes
+    [V] (nvidia-smi)      processes from envs on non-attached devices
+    [ ] (envs.json)       timeout
+
+resources:
+    [V] (devices.json)    num of attached devices
+
+    (later...)
+    [ ] (nvidia-smi)      num of processes (as an alternative to compute mgmt)
+    [ ] (envs.json)       num of active envs
+    [ ] (envs.json)       num of machines with active envs
+    [ ] (nvidia-smi)      amount of GPU memory (per device/total)
+
+https://grafana.com/docs/grafana/latest/cli/#override-homepath-value
```

### Comparing `genv-0.6.0/setup.py` & `genv-0.9.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("../README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="genv",
-    version="0.6.0",
+    version="0.9.0",
     author="Run:AI",
     author_email="pypi@run.ai",
     description="GPU Environment Management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/run-ai/genv",
     packages=setuptools.find_packages(),
```

