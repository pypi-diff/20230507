# Comparing `tmp/impose_cli-0.0.13.tar.gz` & `tmp/impose_cli-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose_cli-0.0.13.tar", last modified: Sun May  7 16:03:53 2023, max compression
+gzip compressed data, was "impose_cli-0.0.14.tar", last modified: Sun May  7 16:32:03 2023, max compression
```

## Comparing `impose_cli-0.0.13.tar` & `impose_cli-0.0.14.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 16:03:53.347193 impose_cli-0.0.13/
--rw-r--r--   0 samuelchai   (501) staff       (20)      179 2023-05-07 16:03:53.347094 impose_cli-0.0.13/PKG-INFO
--rw-r--r--   0 samuelchai   (501) staff       (20)      379 2023-05-07 15:18:12.000000 impose_cli-0.0.13/README.md
-drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 16:03:53.346211 impose_cli-0.0.13/impose_cli/
--rw-r--r--   0 samuelchai   (501) staff       (20)       52 2023-05-07 16:03:24.000000 impose_cli-0.0.13/impose_cli/__init__.py
--rw-r--r--   0 samuelchai   (501) staff       (20)     4398 2023-05-07 15:18:12.000000 impose_cli-0.0.13/impose_cli/impose_cli.py
-drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 16:03:53.346924 impose_cli-0.0.13/impose_cli.egg-info/
--rw-r--r--   0 samuelchai   (501) staff       (20)      179 2023-05-07 16:03:53.000000 impose_cli-0.0.13/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 samuelchai   (501) staff       (20)      235 2023-05-07 16:03:53.000000 impose_cli-0.0.13/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 16:03:53.000000 impose_cli-0.0.13/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)        6 2023-05-07 16:03:53.000000 impose_cli-0.0.13/impose_cli.egg-info/requires.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)       11 2023-05-07 16:03:53.000000 impose_cli-0.0.13/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)       38 2023-05-07 16:03:53.347237 impose_cli-0.0.13/setup.cfg
--rw-r--r--   0 samuelchai   (501) staff       (20)      378 2023-05-07 16:02:45.000000 impose_cli-0.0.13/setup.py
+drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 16:32:03.988860 impose_cli-0.0.14/
+-rw-r--r--   0 samuelchai   (501) staff       (20)      179 2023-05-07 16:32:03.988763 impose_cli-0.0.14/PKG-INFO
+-rw-r--r--   0 samuelchai   (501) staff       (20)      379 2023-05-07 15:18:12.000000 impose_cli-0.0.14/README.md
+drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 16:32:03.988066 impose_cli-0.0.14/impose_cli/
+-rw-r--r--   0 samuelchai   (501) staff       (20)       52 2023-05-07 16:03:24.000000 impose_cli-0.0.14/impose_cli/__init__.py
+-rw-r--r--   0 samuelchai   (501) staff       (20)     4422 2023-05-07 16:29:47.000000 impose_cli-0.0.14/impose_cli/impose_cli.py
+drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 16:32:03.988606 impose_cli-0.0.14/impose_cli.egg-info/
+-rw-r--r--   0 samuelchai   (501) staff       (20)      179 2023-05-07 16:32:03.000000 impose_cli-0.0.14/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 samuelchai   (501) staff       (20)      235 2023-05-07 16:32:03.000000 impose_cli-0.0.14/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 16:32:03.000000 impose_cli-0.0.14/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)        6 2023-05-07 16:32:03.000000 impose_cli-0.0.14/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)       11 2023-05-07 16:32:03.000000 impose_cli-0.0.14/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)       38 2023-05-07 16:32:03.988893 impose_cli-0.0.14/setup.cfg
+-rw-r--r--   0 samuelchai   (501) staff       (20)      378 2023-05-07 16:30:34.000000 impose_cli-0.0.14/setup.py
```

### Comparing `impose_cli-0.0.13/impose_cli/impose_cli.py` & `impose_cli-0.0.14/impose_cli/impose_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         spec.loader.exec_module(module)
         return module
 
     def analyze_functions(module, function):
         signature = sig(getattr(module, function))
         parameters = signature.parameters
         args_with_defaults = [(p.name, p.annotation if p.annotation.__name__ != '_empty' else None) for p in parameters.values() if p.default != Parameter.empty]
-        args_without_defaults = [(p.name, p.annotation if p.annotation.__name__ != '_empty' else None) for p in parameters.values() if p.default == Parameter.empty]
+        args_without_defaults = [(p.name, p.annotation if p.annotation.__name__ != '_empty' else None) for p in parameters.values() if p.default == Parameter.empty and p.default is not None]
         return args_without_defaults, args_with_defaults
 
     def create_dynamic_group(group_name, command_list):
         dynamic_group = click.Group(name=group_name)
 
         for cmd in command_list:
             dynamic_command = click.Command(name=cmd['name'].replace('_', '-'), callback=cmd['callback'])
@@ -75,15 +75,15 @@
                     dynamic_command.params.append(click.Argument((arg_name,), type=arg[1]))
                 else:
                     dynamic_command.params.append(click.Argument((arg_name,)))
 
             for opt in cmd['options']:
                 opt_name = opt[0].replace('_', '-')
                 if opt[1] is not None:
-                    dynamic_command.params.append(click.Argument((f"--{opt_name}",), type=opt[1]))
+                    dynamic_command.params.append(click.Option((f"--{opt_name}",), type=opt[1]))
                 else:
                     dynamic_command.params.append(click.Option((f"--{opt_name}",)))
 
             dynamic_group.add_command(dynamic_command)
 
         return dynamic_group
```

