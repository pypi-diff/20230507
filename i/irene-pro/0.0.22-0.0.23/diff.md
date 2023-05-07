# Comparing `tmp/irene_pro-0.0.22.tar.gz` & `tmp/irene_pro-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.22.tar", last modified: Thu May  4 13:32:25 2023, max compression
+gzip compressed data, was "irene_pro-0.0.23.tar", last modified: Sun May  7 10:59:43 2023, max compression
```

## Comparing `irene_pro-0.0.22.tar` & `irene_pro-0.0.23.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 13:32:25.505220 irene_pro-0.0.22/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.22/LICENSE
--rw-rw-rw-   0        0        0        0 2023-05-04 09:36:27.000000 irene_pro-0.0.22/MANIFEST.in
--rw-rw-rw-   0        0        0     1182 2023-05-04 13:32:25.500234 irene_pro-0.0.22/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-05-04 10:12:36.000000 irene_pro-0.0.22/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 13:32:25.474303 irene_pro-0.0.22/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.22/irene_pro/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-04 09:32:48.000000 irene_pro-0.0.22/irene_pro/logic.py
--rw-rw-rw-   0        0        0    21669 2023-05-04 10:00:25.000000 irene_pro-0.0.22/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:32:25.494250 irene_pro-0.0.22/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1182 2023-05-04 13:32:25.000000 irene_pro-0.0.22/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-04 13:32:25.000000 irene_pro-0.0.22/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 13:32:25.000000 irene_pro-0.0.22/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-04 13:32:25.000000 irene_pro-0.0.22/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 13:32:25.000000 irene_pro-0.0.22/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 13:32:25.508221 irene_pro-0.0.22/setup.cfg
--rw-rw-rw-   0        0        0     1146 2023-05-04 13:32:01.000000 irene_pro-0.0.22/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 10:59:43.306898 irene_pro-0.0.23/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.23/LICENSE
+-rw-rw-rw-   0        0        0     2406 2023-05-07 10:59:43.303902 irene_pro-0.0.23/PKG-INFO
+-rw-rw-rw-   0        0        0     1827 2023-05-07 10:49:50.000000 irene_pro-0.0.23/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 10:59:43.274980 irene_pro-0.0.23/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 07:11:13.000000 irene_pro-0.0.23/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0    24162 2023-05-07 10:44:54.000000 irene_pro-0.0.23/irene_pro/gui.py
+-rw-rw-rw-   0        0        0    11620 2023-05-01 10:00:44.000000 irene_pro-0.0.23/irene_pro/others.py
+drwxrwxrwx   0        0        0        0 2023-05-07 10:59:43.299914 irene_pro-0.0.23/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     2406 2023-05-07 10:59:43.000000 irene_pro-0.0.23/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-07 10:59:43.000000 irene_pro-0.0.23/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 10:59:43.000000 irene_pro-0.0.23/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-07 10:59:43.000000 irene_pro-0.0.23/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-07 10:59:43.000000 irene_pro-0.0.23/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 10:59:43.307929 irene_pro-0.0.23/setup.cfg
+-rw-rw-rw-   0        0        0     2370 2023-05-07 10:58:51.000000 irene_pro-0.0.23/setup.py
```

### Comparing `irene_pro-0.0.22/irene_pro/widgets.py` & `irene_pro-0.0.23/irene_pro/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 from tkinter import *
 from tkinter import ttk, filedialog
 import re, random
 from win32api import GetSystemMetrics as ruler
 from math import ceil
 import cv2
-import pyperclip as copier
 from tkcalendar import Calendar
 import ttkthemes
+from others import *
 
 s_width = ruler(0)
 s_height = ruler(1)
 
 
 def w(width:float):
     ratio = width / 1366
@@ -397,20 +397,14 @@
             if found_num:
                 text = master['bg'][:master['bg'].index(found_num[0])]
                 num = int(master['bg'][master['bg'].index(found_num[0]):]) - 3
                 self.config(bg = text+str(num))
         except TypeError:
             pass
 
-def clipboard(data = None, action = None):
-    if action == "copy" and data:
-        copier.copy(data)
-    elif action == "paste":
-        return copier.paste()
-
 class spinbox(ttk.Spinbox):
     def __init__(self, master, **kwargs):
         super().__init__(master =master, **kwargs)
 
 class calendar(Calendar):
     def __init__(self, master, global_date_holder:Variable, date_holder_widget = None, create_toplevel = False, **kw):
         super().__init__(master = master, **kw)
@@ -422,16 +416,14 @@
             self.datetime_fr = lframe(self.master)
             self.datetime_fr.pack(side=RIGHT, padx = w(2))
         else:
             # CREATE TOPLEVEL WINDOW TO HOLD THE CALENDAR AND THE TIME SELECTOR
             self.datetime_fr = Toplevel()
             self.datetime_fr.title("Select time and date")
             self.datetime_fr.geometry(f'{w(250)}x{h(480)}')
-            # self.datetime_fr.resizable(False, False)
-            self.datetime_fr.iconbitmap("images/clock.ico")
             self.datetime_fr.resizable(False, False)
         
         # MAKE CALENDAR
         self.make_cal()
 
     def make_cal(self):
         self.datetime_fr1 = lframe(self.datetime_fr)
@@ -512,8 +504,100 @@
     
     def browse_path(self, dir_holder = None):
         dir = filedialog.askdirectory()
         if dir_holder:
             dir_holder.delete(0, END)
             dir_holder.insert(END, dir)
         else:
-            return dir
+            return dir
+
+# PROGRESSBAR
+class Progress(ttk.Progressbar):
+    def __init__(self, master, max = 100, **kwargs):
+        """max: is the max length to which the progressbar will automatically be destroyed when reached"""
+        super().__init__(master=master)
+        self.master = master
+        self.max = max
+        
+    def step(self, value):
+        import time
+        self['value'] = value
+        self.master.update_idletasks()
+        if value == self.max:
+            self.master.destroy()
+        time.sleep(1)
+
+# ======= SCALE===========================================================
+class scaler(ttk.Scale):
+    def __init__(self, master,start, end, selected_displayer:Label, return_float = True, **kwargs):
+        """selected_displayer: the label to display the selected value from scale
+        return_float: by default, it returns float value, you can return integers but setting to False"""
+        super().__init__(master=master, from_ = start, to=end, **kwargs)
+        
+        self.displayer = selected_displayer
+        self.return_float_value = return_float
+        self.selected_value = None
+        self.config(command=self.display)
+
+    def display(self, value):
+        if not self.return_float_value:
+            value = int(float(value))
+        self.displayer.config(text=value)
+        self.selected_value = value
+    
+    def get_value(self):
+        """get the selected value from the scale so that you can use it in other side"""
+        return self.selected_value
+
+
+def separate(numbers):
+    floating = []
+    new_str = ""
+    float_pos = 0
+    decision = ""
+    sign_negative = ""
+    str_num = str(numbers)
+    listed = [i for i in str_num]
+    original = listed
+
+    try:
+        if "." in str_num:
+            float_pos += original.index(".")
+            decision += "point"
+            floating = listed[float_pos:]
+        if "-" in str_num:
+            listed.remove("-")
+            sign_negative += "negative"
+
+    except Exception:
+        pass
+
+    if decision == "point":
+        listed = listed[:float_pos]
+
+    if len(listed) > 3 and len(listed) < 7:
+        try:
+            position = len(listed) - 3
+            listed.insert(position, " ")
+        except Exception:
+            pass
+
+    elif len(listed) == 7:
+        listed.insert(1, " ")
+        listed.insert(5, " ")
+
+    elif len(listed) == 8:
+        listed.insert(2, " ")
+        listed.insert(6, " ")
+
+    elif len(listed) == 9:
+        listed.insert(3, " ")
+        listed.insert(7, " ")
+
+    if sign_negative == "negative":
+        new_str += "-"
+    for j in listed:
+        new_str += j
+    if len(floating) > 0:
+        for k in floating:
+            new_str += k
+    return new_str
```

