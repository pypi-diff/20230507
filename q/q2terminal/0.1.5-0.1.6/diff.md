# Comparing `tmp/q2terminal-0.1.5.tar.gz` & `tmp/q2terminal-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2terminal-0.1.5.tar", max compression
+gzip compressed data, was "q2terminal-0.1.6.tar", max compression
```

## Comparing `q2terminal-0.1.5.tar` & `q2terminal-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      384 2023-05-06 22:30:03.816197 q2terminal-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2292 2023-05-06 22:00:43.945875 q2terminal-0.1.5/q2terminal/q2terminal.py
--rw-r--r--   0        0        0       21 2023-05-06 22:30:07.307111 q2terminal-0.1.5/q2terminal/version.py
--rw-r--r--   0        0        0      523 2023-05-06 22:10:01.827611 q2terminal-0.1.5/README.md
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 q2terminal-0.1.5/setup.py
--rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 q2terminal-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      384 2023-05-07 20:23:34.343483 q2terminal-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2424 2023-05-07 20:22:00.315642 q2terminal-0.1.6/q2terminal/q2terminal.py
+-rw-r--r--   0        0        0       21 2023-05-07 20:23:36.403703 q2terminal-0.1.6/q2terminal/version.py
+-rw-r--r--   0        0        0      523 2023-05-06 22:10:01.827611 q2terminal-0.1.6/README.md
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 q2terminal-0.1.6/setup.py
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 q2terminal-0.1.6/PKG-INFO
```

### Comparing `q2terminal-0.1.5/q2terminal/q2terminal.py` & `q2terminal-0.1.6/q2terminal/q2terminal.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,23 +3,27 @@
 from time import ctime
 
 
 class Q2Terminal:
     def __init__(self, terminal=None, echo=False, callback=None):
         self.echo = False
         self.callback = None
+        self.shell = False
         if terminal is None:
             if "win32" in sys.platform:
                 terminal = "powershell"
             elif "darwin" in sys.platform:
                 terminal = "zsh"
             else:
                 terminal = "bash"
+        if "win32" not in sys.platform:
+            self.shell = True
         self.proc = Popen(
             [terminal],
+            shell=self.shell,
             stdin=PIPE,
             stdout=PIPE,
             stderr=STDOUT,
         )
         self.run("echo 0")
         self.echo = echo
         self.callback = callback
@@ -55,15 +59,15 @@
                         self.exit_code = 1
                 break
             elif line == "":
                 continue
             else:
                 rez.append(line)
                 if echo or self.echo:
-                    print(f"{ctime()}: {line}")
+                    print(f"{ctime()}:\t{line}")
                 if callable(_callback):
                     callback(line)
 
         return rez
 
     def close(self):
         self.proc.terminate()
```

### Comparing `q2terminal-0.1.5/README.md` & `q2terminal-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `q2terminal-0.1.5/setup.py` & `q2terminal-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['q2terminal']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'q2terminal',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': '',
     'long_description': '[![Python application](https://github.com/AndreiPuchko/q2terminal/actions/workflows/main.yml/badge.svg)](https://github.com/AndreiPuchko/q2terminal/actions/workflows/main.yml)\n# Interaction with a terminal session\n\n```python\nfrom q2terminal.q2terminal import Q2Terminal\nimport sys\n\nt = Q2Terminal()\nt.run("programm", echo=True)\nassert t.exit_code != 0\n\nassert t.run("$q2 = 123") == []\nassert t.run("echo $q2") == ["123"]\n\n\nif "win32" in sys.platform:\n    t.run("notepad")\n    assert t.exit_code == 0\n```\n',
     'author': 'Andrei Puchko',
     'author_email': 'andrei.puchko@gmx.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `q2terminal-0.1.5/PKG-INFO` & `q2terminal-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2terminal
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

