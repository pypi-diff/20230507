# Comparing `tmp/cursesplus-2.0.3.tar.gz` & `tmp/cursesplus-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.0.3.tar", last modified: Sun Apr 16 17:47:53 2023, max compression
+gzip compressed data, was "cursesplus-2.0.4.tar", last modified: Sat May  6 22:18:21 2023, max compression
```

## Comparing `cursesplus-2.0.3.tar` & `cursesplus-2.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-16 17:47:53.832487 cursesplus-2.0.3/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.0.3/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1624 2023-04-16 17:47:53.832487 cursesplus-2.0.3/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1021 2023-04-16 17:47:37.000000 cursesplus-2.0.3/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-04-16 17:47:19.000000 cursesplus-2.0.3/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-04-16 17:47:53.832487 cursesplus-2.0.3/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-16 17:47:53.812487 cursesplus-2.0.3/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      555 2023-04-07 16:31:31.000000 cursesplus-2.0.3/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-16 17:47:53.822487 cursesplus-2.0.3/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.0.3/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.0.3/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11982 2023-04-16 17:46:39.000000 cursesplus-2.0.3/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.0.3/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-16 17:47:53.822487 cursesplus-2.0.3/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1624 2023-04-16 17:47:53.000000 cursesplus-2.0.3/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-04-16 17:47:53.000000 cursesplus-2.0.3/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-04-16 17:47:53.000000 cursesplus-2.0.3/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-04-16 17:47:53.000000 cursesplus-2.0.3/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-06 22:18:21.432831 cursesplus-2.0.4/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.0.4/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1614 2023-05-06 22:18:21.432831 cursesplus-2.0.4/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1011 2023-05-06 21:53:22.000000 cursesplus-2.0.4/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-05-06 21:51:19.000000 cursesplus-2.0.4/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-05-06 22:18:21.432831 cursesplus-2.0.4/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-06 22:18:21.422831 cursesplus-2.0.4/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      283 2023-05-06 21:59:53.000000 cursesplus-2.0.4/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-06 22:18:21.422831 cursesplus-2.0.4/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.0.4/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.0.4/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    13100 2023-05-06 22:12:50.000000 cursesplus-2.0.4/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.0.4/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-05-06 22:18:21.432831 cursesplus-2.0.4/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1614 2023-05-06 22:18:21.000000 cursesplus-2.0.4/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-05-06 22:18:21.000000 cursesplus-2.0.4/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-05-06 22:18:21.000000 cursesplus-2.0.4/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-05-06 22:18:21.000000 cursesplus-2.0.4/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.0.3/LICENSE` & `cursesplus-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.3/PKG-INFO` & `cursesplus-2.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.0.3
+Version: 2.0.4
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,17 +36,17 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
-### Version 2.0.3
+### Version 2.0.4
 
-Huge performance improvements to filedialog
+More features added to filedialog
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
 -Rewrite colour system. load_colours() is now nonexistent.
 -Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
```

### Comparing `cursesplus-2.0.3/README.md` & `cursesplus-2.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
-### Version 2.0.3
+### Version 2.0.4
 
-Huge performance improvements to filedialog
+More features added to filedialog
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
 -Rewrite colour system. load_colours() is now nonexistent.
 -Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
```

### Comparing `cursesplus-2.0.3/pyproject.toml` & `cursesplus-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.0.3"
+version = "2.0.4"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.0.3/src/cursesplus/__init__.py` & `cursesplus-2.0.4/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.3/src/cursesplus/cp.py` & `cursesplus-2.0.4/src/cursesplus/cp.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.3/src/cursesplus/filedialog.py` & `cursesplus-2.0.4/src/cursesplus/filedialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import cp
+from . import cp, messagebox
 import os
 import glob
 from datetime import datetime
 
 def parse_size(data: int) -> str:
     """Internal Function to change an int to a data string size ex 1000000 -> 1 MB"""
     result = "???"
@@ -147,16 +147,27 @@
         elif ch == cp.curses.KEY_SLEFT or ch == 98:
             directory = "/".join(directory.split("/")[0:-1])
             selected = 0
             yoffset = 0
             refresh = True
             if directory == "":
                 directory = "/"
+        elif ch == 114:
+            refresh = True#Refresh files list
+        elif ch == 108:
+            npath = cp.cursesinput(stdscr,"Please enter new path").replace("\n","")
+            if os.path.isdir(npath):
+                directory = npath
+                selected = 0
+                yoffset = 0
+                refresh = True
+            else:
+                messagebox.showwarning(stdscr,["Path does not exist"])
         elif ch == 104:
-            cp.displaymsg(stdscr,["List of Keybinds","Down Arrow: Scroll down","Up Arrow: Scroll up","Left Arrow: Scroll left","Right Arrow: Scroll right","Shift-left arrow: Move up to parent Directory","Enter: Open/select","F: Change filter"])
+            cp.displaymsg(stdscr,["List of Keybinds","Down Arrow: Scroll down","Up Arrow: Scroll up","Left Arrow: Scroll left","Right Arrow: Scroll right","Shift-left arrow: Move up to parent Directory","Enter: Open/select","F: Change filter","L: Change location"])
 
         #masterlist.clear()
 
 def openfilesdialog(stdscr,title: str = "Please choose a file",filter: str = [["*","All Files"]],directory: str = os.getcwd()) -> list:
     """Start a filedialog to select multiple files. title is the prompt the user recieves. filter is the file filter. The filter syntax is the same as TK syntax. The first
     filter provided is the main filter. 
     Filter Syntax: 
@@ -171,35 +182,40 @@
     xoffset: int = 0
     yoffset: int = 0
     activefilter: int = 0
     selected: int = 0
     chosen: list[str] = []
     chosen.append(" ")
     chosen.clear()
+    update = True
+    masterlist: list = list[Fileobj]
     while True:
-        masterlist: list = list[Fileobj]
+        
         mx,my = os.get_terminal_size()
         MAXNL = mx - 33
         stdscr.clear()
         cp.rectangle(stdscr,2,0,my-2,mx-1)
         cp.filline(stdscr,0,cp.set_color(cp.BLUE,cp.WHITE))
         cp.filline(stdscr,1,cp.set_color(cp.GREEN,cp.WHITE))
         cp.filline(stdscr,my-2,cp.set_color(cp.WHITE,cp.BLACK))
         cp.filline(stdscr,my-1,cp.set_color(cp.RED,cp.WHITE))
         topline = "Name"+" "*(MAXNL-4)+"|"+"Size     "+"|Date Modified"
         topline = topline+(mx-2-len(topline))*" "
-        directories = [directory+"/"+l for l in os.listdir(directory) if os.path.isdir(directory+"/"+l)]
-        if filter[activefilter][0] == "*":
-            files = [directory+"/"+l for l in os.listdir(directory) if os.path.isfile(directory+"/"+l)]
-        else:
-            files = glob.glob(directory+"/"+filter[activefilter][0])
-        directories.sort()
-        files.sort()
-        #displaymsg(stdscr,directories+files)
-        masterlist = [Fileobj(f) for f in (directories+files)]
+        if update:
+            #masterlist.clear()
+            directories = [directory+"/"+l for l in os.listdir(directory) if os.path.isdir(directory+"/"+l)]
+            if filter[activefilter][0] == "*":
+                files = [directory+"/"+l for l in os.listdir(directory) if os.path.isfile(directory+"/"+l)]
+            else:
+                files = glob.glob(directory+"/"+filter[activefilter][0])
+            directories.sort()
+            files.sort()
+            #displaymsg(stdscr,directories+files)
+            masterlist = [Fileobj(f) for f in (directories+files)]
+        update = False
         stdscr.addstr(0,0,title+"|H for Help|Press Shift-Left Arrow to move up directory"[0:mx],cp.set_colour(cp.BLUE,cp.WHITE))
         stdscr.addstr(1,0,directory[xoffset:xoffset+mx],cp.set_colour(cp.GREEN,cp.WHITE))
         stdscr.addstr(my-2,0,f"{filter[activefilter][1]} ({filter[activefilter][0]}) [{len(masterlist)} objects found]"[0:mx],cp.set_colour(cp.WHITE,cp.BLACK))
         stdscr.addstr(2,1,topline[0:mx-1])
         
         try:
             stdscr.addstr(my-1,0,str(chosen)[xoffset:xoffset+mx],cp.set_colour(cp.RED,cp.WHITE))
@@ -245,31 +261,44 @@
             selected = 0
             yoffset = 0
         elif ch == cp.curses.KEY_ENTER or ch == 10 or ch == 13:
             if masterlist[selected].isdir:
                 directory = masterlist[selected].path
                 selected = 0
                 yoffset = 0
+                update = True
             else:
                 chosen.clear()
                 chosen.append(masterlist[selected].path)
         elif ch == 115:
             #s for add to selection
             if not masterlist[selected].isdir:
                 if masterlist[selected].path in chosen:
                     chosen.remove(masterlist[selected].path)
                 else:
                     chosen.append(masterlist[selected].path)
         elif ch == cp.curses.KEY_SLEFT or ch == 98:
             directory = "/".join(directory.split("/")[0:-1])
             selected = 0
             yoffset = 0
+            update = True
             if directory == "":
                 directory = "/"
+        elif ch == 114:
+            update = True#Refresh files list
         elif ch == 100 or cp.curses.keyname(ch).decode() == "^X":
             return [c for c in chosen if os.path.isfile(c) and c.replace(" ","") != ""]#Only return files that still exist
         elif ch == 99:
             chosen.clear()
+        elif ch == 108:
+            npath = cp.cursesinput(stdscr,"Please enter new path").replace("\n","")
+            if os.path.isdir(npath):
+                directory = npath
+                selected = 0
+                yoffset = 0
+                update = True
+            else:
+                messagebox.showwarning(stdscr,["Path does not exist"])
         elif ch == 104:
-            cp.displaymsg(stdscr,["List of Keybinds","Down Arrow: Scroll down","Up Arrow: Scroll up","Left Arrow: Scroll left","Right Arrow: Scroll right","Shift-left arrow: Move up to parent Directory","Enter: Open/select","F: Change filter","S: Append / Remove from selection","D/Ctrl-X: Done","C: Clear selection"])
+            cp.displaymsg(stdscr,["List of Keybinds","Down Arrow: Scroll down","Up Arrow: Scroll up","Left Arrow: Scroll left","Right Arrow: Scroll right","Shift-left arrow: Move up to parent Directory","Enter: Open/select","F: Change filter","S: Append / Remove from selection","D/Ctrl-X: Done","C: Clear selection","R: Refresh files list","L: Change location"])
 
-        masterlist.clear()
+        #masterlist.clear()
```

### Comparing `cursesplus-2.0.3/src/cursesplus/messagebox.py` & `cursesplus-2.0.4/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.3/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.0.4/src/cursesplus.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.0.3
+Version: 2.0.4
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,17 +36,17 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
-### Version 2.0.3
+### Version 2.0.4
 
-Huge performance improvements to filedialog
+More features added to filedialog
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
 -Rewrite colour system. load_colours() is now nonexistent.
 -Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
```

