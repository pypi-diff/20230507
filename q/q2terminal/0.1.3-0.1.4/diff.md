# Comparing `tmp/q2terminal-0.1.3.tar.gz` & `tmp/q2terminal-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2terminal-0.1.3.tar", max compression
+gzip compressed data, was "q2terminal-0.1.4.tar", max compression
```

## Comparing `q2terminal-0.1.3.tar` & `q2terminal-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      384 2023-05-05 22:11:21.873710 q2terminal-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2179 2023-05-05 22:10:55.399583 q2terminal-0.1.3/q2terminal/q2terminal.py
--rw-r--r--   0        0        0       21 2023-05-05 22:11:25.817906 q2terminal-0.1.3/q2terminal/version.py
--rw-r--r--   0        0        0       51 2023-05-05 22:03:50.967499 q2terminal-0.1.3/README.md
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 q2terminal-0.1.3/setup.py
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 q2terminal-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      384 2023-05-06 01:23:50.936394 q2terminal-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2428 2023-05-06 00:51:24.762775 q2terminal-0.1.4/q2terminal/q2terminal.py
+-rw-r--r--   0        0        0       21 2023-05-06 01:23:55.232494 q2terminal-0.1.4/q2terminal/version.py
+-rw-r--r--   0        0        0      353 2023-05-05 22:13:48.919889 q2terminal-0.1.4/README.md
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 q2terminal-0.1.4/setup.py
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 q2terminal-0.1.4/PKG-INFO
```

### Comparing `q2terminal-0.1.3/q2terminal/q2terminal.py` & `q2terminal-0.1.4/q2terminal/q2terminal.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,59 +3,64 @@
 from time import ctime
 
 
 class Q2Terminal:
     def __init__(self, terminal=None, echo=False, callback=None):
         self.echo = False
         self.callback = None
+        self.shell = False
         if terminal is None:
             if "win32" in sys.platform:
                 terminal = "powershell"
-            elif "darwin":
+            elif "darwin" in sys.platform:
                 terminal = "zsh"
             else:
-                terminal = "bash"
+                terminal = "/bin/bash"
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
         self.exit_code = None
 
     def run(self, cmd="", echo=False, callback=None):
         if echo or self.echo:
             print(f"{ctime()}> {cmd}>")
         _callback = callback if callback else self.callback
         self.exit_code = None
-        cmd = f"{cmd};$?;echo q2eoc\n"
+        cmd = f"{cmd}; echo $?;echo q2eoc\n"
         self.proc.stdin.writelines([bytes(cmd, "utf8")])
         self.proc.stdin.flush()
         rez = []
-        first_line = True
+        # skip first line of output for Windows powershell
+        first_line = True if "win32" in sys.platform else False
         while self.proc.poll() is None:
             line = self.proc.stdout.readline().decode("utf8").rstrip()
             if not line:
                 continue
             if first_line:
                 first_line = False
                 continue
 
             if line.strip() == "q2eoc":
                 if rez:
                     self.exit_code = rez.pop().strip()
                     if self.exit_code.isdigit():
                         self.exit_code = int(self.exit_code)
                     elif self.exit_code == "True":
-                        self.exit_code = True
+                        self.exit_code = 0
                     elif self.exit_code == "False":
-                        self.exit_code = False
+                        self.exit_code = 1
                 break
             elif line == "":
                 continue
             else:
                 rez.append(line)
                 if echo or self.echo:
                     print(f"{ctime()}: {line}")
```

