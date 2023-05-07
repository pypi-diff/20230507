# Comparing `tmp/rekono-cli-1.1.0.tar.gz` & `tmp/rekono-cli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rekono-cli-1.1.0.tar", last modified: Wed Jan 11 17:44:10 2023, max compression
+gzip compressed data, was "dist/rekono-cli-2.0.0.tar", last modified: Sun May  7 11:50:31 2023, max compression
```

## Comparing `rekono-cli-1.1.0.tar` & `rekono-cli-2.0.0.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:44:10.000000 rekono-cli-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-01-11 17:44:10.000000 rekono-cli-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:44:10.000000 rekono-cli-1.1.0/rekono/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:44:10.000000 rekono-cli-1.1.0/rekono/api/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/api/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/api/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:44:10.000000 rekono-cli-1.1.0/rekono/installation/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/installation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/installation/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/installation/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/installation/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/installation/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/installation/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/installation/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:44:10.000000 rekono-cli-1.1.0/rekono/services/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/services/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/services/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/services/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:44:10.000000 rekono-cli-1.1.0/rekono/services/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/services/templates/rekono.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:44:10.000000 rekono-cli-1.1.0/rekono/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:44:10.000000 rekono-cli-1.1.0/rekono/utils/linux/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/utils/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/utils/linux/apt.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/utils/linux/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/utils/linux/systemctl.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/utils/linux/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/utils/linux/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/rekono/utils/source_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:44:10.000000 rekono-cli-1.1.0/rekono_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-01-11 17:44:09.000000 rekono-cli-1.1.0/rekono_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-01-11 17:44:10.000000 rekono-cli-1.1.0/rekono_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 17:44:09.000000 rekono-cli-1.1.0/rekono_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-11 17:44:09.000000 rekono-cli-1.1.0/rekono_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-11 17:44:09.000000 rekono-cli-1.1.0/rekono_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-11 17:44:09.000000 rekono-cli-1.1.0/rekono_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 17:44:10.000000 rekono-cli-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-01-11 17:43:46.000000 rekono-cli-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/authentications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/findings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/target_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/wordlists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono/framework/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/commands/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/commands/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/setup.py
```

### Comparing `rekono-cli-1.1.0/setup.py` & `rekono-cli-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 
 import pkg_resources
 from setuptools import find_packages, setup
 
 from rekono import VERSION
 
 current_directory = os.path.dirname(os.path.realpath(__file__))
-with open(os.path.join(current_directory, 'README.md'), 'r') as readme:
+with open(os.path.join(current_directory, '..', 'README.md'), 'r') as readme:
     long_description = readme.read()
 
 with open(os.path.join(current_directory, 'requirements.txt'), 'r') as requirements:
     install_requires = [str(req) for req in pkg_resources.parse_requirements(requirements)]
 
 setup(
     name='rekono-cli',
-    packages=find_packages(),
+    packages=find_packages(exclude=['tests']),
     version=VERSION,
-    description='CLI to manage Rekono',
+    description='CLI to make requests to Rekono API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Pablo Santiago López',
     url='https://github.com/pablosnt/rekono-cli',
     keywords=['automation', 'pentesting', 'security', 'cli', 'rekono'],
     include_package_data=True,
     install_requires=install_requires,
     python_requires='>=3.7',
     entry_points='''
         [console_scripts]
-        rekono=rekono.main:rekono
+        rekono-cli=rekono.main:rekono
     ''',
     project_urls={
         'Rekono': 'https://github.com/pablosnt/rekono',
         'Rekono CLI': 'https://github.com/pablosnt/rekono-cli',
     }
 )
```

