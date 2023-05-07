# Comparing `tmp/cursesplus-2.0.4.tar.gz` & `tmp/cursesplus-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.0.4.tar", last modified: Sat May  6 22:18:21 2023, max compression
+gzip compressed data, was "cursesplus-2.0.5.tar", last modified: Sun May  7 14:43:54 2023, max compression
```

## Comparing `cursesplus-2.0.4.tar` & `cursesplus-2.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-06 22:18:21.432831 cursesplus-2.0.4/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.0.4/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1614 2023-05-06 22:18:21.432831 cursesplus-2.0.4/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1011 2023-05-06 21:53:22.000000 cursesplus-2.0.4/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-05-06 21:51:19.000000 cursesplus-2.0.4/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-06 22:18:21.432831 cursesplus-2.0.4/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-06 22:18:21.422831 cursesplus-2.0.4/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      283 2023-05-06 21:59:53.000000 cursesplus-2.0.4/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-06 22:18:21.422831 cursesplus-2.0.4/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.0.4/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.0.4/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    13100 2023-05-06 22:12:50.000000 cursesplus-2.0.4/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.0.4/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-06 22:18:21.432831 cursesplus-2.0.4/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1614 2023-05-06 22:18:21.000000 cursesplus-2.0.4/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-06 22:18:21.000000 cursesplus-2.0.4/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-06 22:18:21.000000 cursesplus-2.0.4/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-06 22:18:21.000000 cursesplus-2.0.4/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-07 14:43:54.214818 cursesplus-2.0.5/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.0.5/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1667 2023-05-07 14:43:54.214818 cursesplus-2.0.5/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1064 2023-05-07 14:40:15.000000 cursesplus-2.0.5/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-05-07 14:39:51.000000 cursesplus-2.0.5/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-07 14:43:54.214818 cursesplus-2.0.5/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-07 14:43:54.204818 cursesplus-2.0.5/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      283 2023-05-06 21:59:53.000000 cursesplus-2.0.5/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-07 14:43:54.214818 cursesplus-2.0.5/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.0.5/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.0.5/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    13128 2023-05-07 14:43:34.000000 cursesplus-2.0.5/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.0.5/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-07 14:43:54.214818 cursesplus-2.0.5/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1667 2023-05-07 14:43:54.000000 cursesplus-2.0.5/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-07 14:43:54.000000 cursesplus-2.0.5/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-07 14:43:54.000000 cursesplus-2.0.5/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-07 14:43:54.000000 cursesplus-2.0.5/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.0.4/LICENSE` & `cursesplus-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.4/PKG-INFO` & `cursesplus-2.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.0.4
+Version: 2.0.5
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,18 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
+### Version 2.0.5
+
+Fix small bug in Manjaro Konsole
+
 ### Version 2.0.4
 
 More features added to filedialog
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
```

### Comparing `cursesplus-2.0.4/README.md` & `cursesplus-2.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
+### Version 2.0.5
+
+Fix small bug in Manjaro Konsole
+
 ### Version 2.0.4
 
 More features added to filedialog
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
```

### Comparing `cursesplus-2.0.4/pyproject.toml` & `cursesplus-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.0.4"
+version = "2.0.5"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.0.4/src/cursesplus/__init__.py` & `cursesplus-2.0.5/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.4/src/cursesplus/cp.py` & `cursesplus-2.0.5/src/cursesplus/cp.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.4/src/cursesplus/filedialog.py` & `cursesplus-2.0.5/src/cursesplus/filedialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             wstr += " "*(MAXNL-len(wstr)+1)
             wstr += fileobjects.sizestr
             wstr += " "*(10-len(fileobjects.sizestr))
             wstr += fileobjects.date
             if selected == ind:
                 stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.MAGENTA))
             elif fileobjects.isdir:
-                stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.BLUE))
+                stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.CYAN))
             else:
                 stdscr.addstr(3+indx,1,wstr)
             ind += 1
             indx += 1#Inc both
 
         
         stdscr.refresh()
@@ -228,17 +228,17 @@
             wstr += " "*(MAXNL-len(wstr)+1)
             wstr += fileobjects.sizestr
             wstr += " "*(10-len(fileobjects.sizestr))
             wstr += fileobjects.date
             if selected == ind:
                 stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.MAGENTA))
             elif fileobjects.isdir:
-                stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.BLUE))
-            elif fileobjects.path in chosen:
                 stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.CYAN))
+            elif fileobjects.path in chosen:
+                stdscr.addstr(3+indx,1,wstr,cp.set_colour(cp.BLACK,cp.YELLOW))
             else:
                 stdscr.addstr(3+indx,1,wstr)
             ind += 1
             indx += 1#Inc both
 
         
         stdscr.refresh()
@@ -256,14 +256,15 @@
             if selected - yoffset > my - 7:
                 yoffset += 1
             selected += 1
         elif ch == 102:
             activefilter = cp.displayops(stdscr,[f"{f[1]} ({f[0]})" for f in filter],"Please choose a filter")
             selected = 0
             yoffset = 0
+            update = True
         elif ch == cp.curses.KEY_ENTER or ch == 10 or ch == 13:
             if masterlist[selected].isdir:
                 directory = masterlist[selected].path
                 selected = 0
                 yoffset = 0
                 update = True
             else:
```

### Comparing `cursesplus-2.0.4/src/cursesplus/messagebox.py` & `cursesplus-2.0.5/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.4/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.0.5/src/cursesplus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.0.4
+Version: 2.0.5
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,18 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
+### Version 2.0.5
+
+Fix small bug in Manjaro Konsole
+
 ### Version 2.0.4
 
 More features added to filedialog
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
```

