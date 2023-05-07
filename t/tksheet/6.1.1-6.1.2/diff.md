# Comparing `tmp/tksheet-6.1.1.tar.gz` & `tmp/tksheet-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.1.1.tar", last modified: Sat May  6 18:18:43 2023, max compression
+gzip compressed data, was "tksheet-6.1.2.tar", last modified: Sun May  7 09:22:39 2023, max compression
```

## Comparing `tksheet-6.1.1.tar` & `tksheet-6.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:18:43.812937 tksheet-6.1.1/
--rw-rw-rw-   0        0        0     1101 2023-05-06 15:11:23.000000 tksheet-6.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3548 2023-05-06 18:18:43.812937 tksheet-6.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2898 2023-05-06 15:11:23.000000 tksheet-6.1.1/README.md
--rw-rw-rw-   0        0        0       86 2023-05-06 18:18:43.828574 tksheet-6.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-05-06 15:12:58.000000 tksheet-6.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:18:43.812937 tksheet-6.1.1/tksheet/
--rw-rw-rw-   0        0        0      344 2023-05-06 15:11:23.000000 tksheet-6.1.1/tksheet/__init__.py
--rw-rw-rw-   0        0        0   169752 2023-05-06 15:11:23.000000 tksheet-6.1.1/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   117473 2023-05-06 15:11:24.000000 tksheet-6.1.1/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0     8893 2023-05-06 15:11:24.000000 tksheet-6.1.1/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   346731 2023-05-06 18:11:05.000000 tksheet-6.1.1/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12757 2023-05-06 15:11:24.000000 tksheet-6.1.1/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0   113971 2023-05-06 15:11:24.000000 tksheet-6.1.1/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5789 2023-05-06 15:11:24.000000 tksheet-6.1.1/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    59987 2023-05-06 15:11:24.000000 tksheet-6.1.1/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:18:43.812937 tksheet-6.1.1/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3548 2023-05-06 18:18:43.000000 tksheet-6.1.1/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-05-06 18:18:43.000000 tksheet-6.1.1/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:18:43.000000 tksheet-6.1.1/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 18:18:43.000000 tksheet-6.1.1/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 09:22:39.860341 tksheet-6.1.2/
+-rw-rw-rw-   0        0        0     1101 2023-05-07 08:33:24.000000 tksheet-6.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3548 2023-05-07 09:22:39.860341 tksheet-6.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2898 2023-05-07 08:33:24.000000 tksheet-6.1.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-07 09:22:39.861343 tksheet-6.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-05-07 08:49:30.000000 tksheet-6.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:22:39.850823 tksheet-6.1.2/tksheet/
+-rw-rw-rw-   0        0        0      344 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   169752 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   117473 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0     8893 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   348717 2023-05-07 09:18:51.000000 tksheet-6.1.2/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12757 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0   113955 2023-05-07 09:10:20.000000 tksheet-6.1.2/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5789 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    59987 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:22:39.859338 tksheet-6.1.2/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3548 2023-05-07 09:22:39.000000 tksheet-6.1.2/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-05-07 09:22:39.000000 tksheet-6.1.2/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 09:22:39.000000 tksheet-6.1.2/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-07 09:22:39.000000 tksheet-6.1.2/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.1.1/LICENSE.txt` & `tksheet-6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.1/PKG-INFO` & `tksheet-6.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.1
+Version: 6.1.2
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.1.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.2.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tksheet-6.1.1/README.md` & `tksheet-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.1/setup.py` & `tksheet-6.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.1.1',
+  version = '6.1.2',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.1.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.2.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.1.1/tksheet/_tksheet.py` & `tksheet-6.1.2/tksheet/_tksheet.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.1/tksheet/_tksheet_column_headers.py` & `tksheet-6.1.2/tksheet/_tksheet_column_headers.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.1/tksheet/_tksheet_formatters.py` & `tksheet-6.1.2/tksheet/_tksheet_formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.1/tksheet/_tksheet_main_table.py` & `tksheet-6.1.2/tksheet/_tksheet_main_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,15 +515,19 @@
                     except Exception:
                         return
                 for rn in range(maxrows):
                     row = []
                     for r1, c1, r2, c2 in boxes:
                         if r2 - r1 < maxrows:
                             continue
-                        datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
+                        datarn = (
+                            (r1 + rn)
+                            if self.all_rows_displayed
+                            else self.displayed_rows[r1 + rn]
+                        )
                         for c in range(c1, c2):
                             datacn = (
                                 c
                                 if self.all_columns_displayed
                                 else self.displayed_columns[c]
                             )
                             row.append(self.get_cell_clipboard(datarn, datacn))
@@ -539,15 +543,19 @@
                             )
                         )
                     except Exception:
                         return
                 for r1, c1, r2, c2 in boxes:
                     for rn in range(r2 - r1):
                         row = []
-                        datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
+                        datarn = (
+                            (r1 + rn)
+                            if self.all_rows_displayed
+                            else self.displayed_rows[r1 + rn]
+                        )
                         for c in range(c1, c2):
                             datacn = (
                                 c
                                 if self.all_columns_displayed
                                 else self.displayed_columns[c]
                             )
                             row.append(self.get_cell_clipboard(datarn, datacn))
@@ -590,29 +598,37 @@
                 except Exception:
                     return
             for rn in range(maxrows):
                 row = []
                 for r1, c1, r2, c2 in boxes:
                     if r2 - r1 < maxrows:
                         continue
-                    datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
+                    datarn = (
+                        (r1 + rn)
+                        if self.all_rows_displayed
+                        else self.displayed_rows[r1 + rn]
+                    )
                     for c in range(c1, c2):
                         datacn = (
                             c
                             if self.all_columns_displayed
                             else self.displayed_columns[c]
                         )
                         row.append(self.get_cell_clipboard(datarn, datacn))
                 writer.writerow(row)
                 rows.append(row)
             for rn in range(maxrows):
                 for r1, c1, r2, c2 in boxes:
                     if r2 - r1 < maxrows:
                         continue
-                    datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
+                    datarn = (
+                        (r1 + rn)
+                        if self.all_rows_displayed
+                        else self.displayed_rows[r1 + rn]
+                    )
                     for c in range(c1, c2):
                         datacn = (
                             c
                             if self.all_columns_displayed
                             else self.displayed_columns[c]
                         )
                         if self.input_valid_for_cell(datarn, datacn, ""):
@@ -630,27 +646,35 @@
                         CtrlKeyEvent("begin_ctrl_x", boxes, currently_selected, tuple())
                     )
                 except Exception:
                     return
             for r1, c1, r2, c2 in boxes:
                 for rn in range(r2 - r1):
                     row = []
-                    datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
+                    datarn = (
+                        (r1 + rn)
+                        if self.all_rows_displayed
+                        else self.displayed_rows[r1 + rn]
+                    )
                     for c in range(c1, c2):
                         datacn = (
                             c
                             if self.all_columns_displayed
                             else self.displayed_columns[c]
                         )
                         row.append(self.get_cell_data(datarn, datacn))
                     writer.writerow(row)
                     rows.append(row)
             for r1, c1, r2, c2 in boxes:
                 for rn in range(r2 - r1):
-                    datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
+                    datarn = (
+                        (r1 + rn)
+                        if self.all_rows_displayed
+                        else self.displayed_rows[r1 + rn]
+                    )
                     for c in range(c1, c2):
                         datacn = (
                             c
                             if self.all_columns_displayed
                             else self.displayed_columns[c]
                         )
                         if self.input_valid_for_cell(datarn, datacn, ""):
@@ -966,51 +990,66 @@
             if to_move_min > c:
                 cws[c:c] = cws[to_move_min:to_move_max]
                 cws[to_move_max:to_del] = []
             else:
                 cws[c + 1 : c + 1] = cws[to_move_min:to_move_max]
                 cws[to_move_min:to_move_max] = []
             self.col_positions = list(accumulate(chain([0], (width for width in cws))))
-        if c + num_cols > len(self.col_positions):
-            new_selected = tuple(
-                range(
-                    len(self.col_positions) - 1 - num_cols, len(self.col_positions) - 1
-                )
-            )
-            if create_selections and index_type == "displayed":
-                self.create_selected(
-                    0,
-                    len(self.col_positions) - 1 - num_cols,
-                    len(self.row_positions) - 1,
-                    len(self.col_positions) - 1,
-                    "columns",
-                )
-        else:
-            if to_move_min > c:
-                new_selected = tuple(range(c, c + num_cols))
-                if create_selections and index_type == "displayed":
-                    self.create_selected(
-                        0, c, len(self.row_positions) - 1, c + num_cols, "columns"
+            if c + num_cols > len(self.col_positions):
+                new_selected = tuple(
+                    range(
+                        len(self.col_positions) - 1 - num_cols,
+                        len(self.col_positions) - 1,
                     )
-            else:
-                new_selected = tuple(range(c + 1 - num_cols, c + 1))
-                if create_selections and index_type == "displayed":
+                )
+                if create_selections:
                     self.create_selected(
                         0,
-                        c + 1 - num_cols,
+                        len(self.col_positions) - 1 - num_cols,
                         len(self.row_positions) - 1,
-                        c + 1,
+                        len(self.col_positions) - 1,
                         "columns",
                     )
-        if create_selections and index_type == "displayed":
-            self.set_currently_selected(0, int(new_selected[0]), type_="column")
+            else:
+                if to_move_min > c:
+                    new_selected = tuple(range(c, c + num_cols))
+                    if create_selections:
+                        self.create_selected(
+                            0, c, len(self.row_positions) - 1, c + num_cols, "columns"
+                        )
+                else:
+                    new_selected = tuple(range(c + 1 - num_cols, c + 1))
+                    if create_selections:
+                        self.create_selected(
+                            0,
+                            c + 1 - num_cols,
+                            len(self.row_positions) - 1,
+                            c + 1,
+                            "columns",
+                        )
+        elif index_type == "data":
+            if to_move_min > c:
+                new_selected = tuple(range(c, c + num_cols))
+            else:
+                new_selected = tuple(range(c + 1 - num_cols, c + 1))
         newcolsdct = {t1: t2 for t1, t2 in zip(orig_selected, new_selected)}
         if self.all_columns_displayed or index_type != "displayed":
             dispset = {}
             if to_move_min > c:
+                if move_data:
+                    extend_idx = to_move_max - 1
+                    for rn in range(len(self.data)):
+                        if to_move_max > len(self.data[rn]):
+                            self.fix_row_len(rn, extend_idx)
+                        self.data[rn][c:c] = self.data[rn][to_move_min:to_move_max]
+                        self.data[rn][to_move_max:to_del] = []
+                    self.CH.fix_header(extend_idx)
+                    if isinstance(self._headers, list) and self._headers:
+                        self._headers[c:c] = self._headers[to_move_min:to_move_max]
+                        self._headers[to_move_max:to_del] = []
                 self.CH.cell_options = {
                     newcolsdct[k]
                     if k in newcolsdct
                     else k + num_cols
                     if k < to_move_min and k >= c
                     else k: v
                     for k, v in self.CH.cell_options.items()
@@ -1027,35 +1066,36 @@
                     newcolsdct[k]
                     if k in newcolsdct
                     else k + num_cols
                     if k < to_move_min and k >= c
                     else k: v
                     for k, v in self.col_options.items()
                 }
-                if move_data:
-                    for rn in range(len(self.data)):
-                        if to_move_max >= len(self.data[rn]):
-                            self.fix_row_len(rn, to_move_max)
-                        self.data[rn][c:c] = self.data[rn][to_move_min:to_move_max]
-                        self.data[rn][to_move_max:to_del] = []
-                    self.CH.fix_header(to_move_max)
-                    if isinstance(self._headers, list) and self._headers:
-                        self._headers[c:c] = self._headers[to_move_min:to_move_max]
-                        self._headers[to_move_max:to_del] = []
                 if index_type != "displayed":
                     self.displayed_columns = sorted(
                         int(newcolsdct[k])
                         if k in newcolsdct
                         else k + num_cols
                         if k < to_move_min and k >= c
                         else int(k)
                         for k in self.displayed_columns
                     )
             else:
                 c += 1
+                if move_data:
+                    extend_idx = c - 1
+                    for rn in range(len(self.data)):
+                        if c > len(self.data[rn]):
+                            self.fix_row_len(rn, extend_idx)
+                        self.data[rn][c:c] = self.data[rn][to_move_min:to_move_max]
+                        self.data[rn][to_move_min:to_move_max] = []
+                    self.CH.fix_header(extend_idx)
+                    if isinstance(self._headers, list) and self._headers:
+                        self._headers[c:c] = self._headers[to_move_min:to_move_max]
+                        self._headers[to_move_min:to_move_max] = []
                 self.CH.cell_options = {
                     newcolsdct[k]
                     if k in newcolsdct
                     else k - num_cols
                     if k < c and k > to_move_min
                     else k: v
                     for k, v in self.CH.cell_options.items()
@@ -1072,81 +1112,58 @@
                     newcolsdct[k]
                     if k in newcolsdct
                     else k - num_cols
                     if k < c and k > to_move_min
                     else k: v
                     for k, v in self.col_options.items()
                 }
-                if move_data:
-                    for rn in range(len(self.data)):
-                        if c >= len(self.data[rn]):
-                            self.fix_row_len(rn, c)
-                        self.data[rn][c:c] = self.data[rn][to_move_min:to_move_max]
-                        self.data[rn][to_move_min:to_move_max] = []
-                    self.CH.fix_header(c)
-                    if isinstance(self._headers, list) and self._headers:
-                        self._headers[c:c] = self._headers[to_move_min:to_move_max]
-                        self._headers[to_move_min:to_move_max] = []
                 if index_type != "displayed":
                     self.displayed_columns = sorted(
                         int(newcolsdct[k])
                         if k in newcolsdct
                         else k - num_cols
                         if k < c and k > to_move_min
                         else int(k)
                         for k in self.displayed_columns
                     )
         else:
             # moves data around, not displayed columns indexes
             # which remain sorted and the same after drop and drop
             if to_move_min > c:
                 dispset = {
-                    b: a
+                    a: b
                     for a, b in zip(
                         self.displayed_columns,
                         (
                             self.displayed_columns[:c]
                             + self.displayed_columns[
                                 to_move_min : to_move_min + num_cols
                             ]
                             + self.displayed_columns[c:to_move_min]
                             + self.displayed_columns[to_move_min + num_cols :]
                         ),
                     )
                 }
             else:
                 dispset = {
-                    b: a
+                    a: b
                     for a, b in zip(
                         self.displayed_columns,
                         (
                             self.displayed_columns[:to_move_min]
                             + self.displayed_columns[to_move_min + num_cols : c + 1]
                             + self.displayed_columns[
                                 to_move_min : to_move_min + num_cols
                             ]
                             + self.displayed_columns[c + 1 :]
                         ),
                     )
                 }
             # has to pick up elements from all over the place in the original row
             # building an entirely new row is best due to permutations of hidden columns
-            self.CH.cell_options = {
-                dispset[k] if k in dispset else k: v
-                for k, v in self.CH.cell_options.items()
-            }
-            self.cell_options = {
-                (k[0], dispset[k[1]]) if k[1] in dispset else k: v
-                for k, v in self.cell_options.items()
-            }
-            self.col_options = {
-                dispset[k] if k in dispset else k: v
-                for k, v in self.col_options.items()
-            }
-            dispset = {b: a for a, b in dispset.items()}
             if move_data:
                 max_len = max(chain(dispset, dispset.values())) + 1
                 max_idx = max_len - 1
                 for rn in range(len(self.data)):
                     if max_len > len(self.data[rn]):
                         self.fix_row_len(rn, max_idx)
                     new = []
@@ -1173,14 +1190,27 @@
                             done.add(idx)
                         elif idx not in done:
                             new.append(self._headers[idx])
                             idx += 1
                         else:
                             idx += 1
                     self._headers = new
+                dispset = {b: a for a, b in dispset.items()}
+                self.CH.cell_options = {
+                    dispset[k] if k in dispset else k: v
+                    for k, v in self.CH.cell_options.items()
+                }
+                self.cell_options = {
+                    (k[0], dispset[k[1]]) if k[1] in dispset else k: v
+                    for k, v in self.cell_options.items()
+                }
+                self.col_options = {
+                    dispset[k] if k in dispset else k: v
+                    for k, v in self.col_options.items()
+                }
         return new_selected, {b: a for a, b in dispset.items()}
 
     def move_rows_adjust_options_dict(
         self,
         row,
         to_move_min,
         num_rows,
@@ -1206,47 +1236,65 @@
                 rhs[to_move_max:to_del] = []
             else:
                 rhs[r + 1 : r + 1] = rhs[to_move_min:to_move_max]
                 rhs[to_move_min:to_move_max] = []
             self.row_positions = list(
                 accumulate(chain([0], (height for height in rhs)))
             )
-        if r + num_rows > len(self.row_positions):
-            new_selected = tuple(
-                range(
-                    len(self.row_positions) - 1 - num_rows, len(self.row_positions) - 1
-                )
-            )
-            if create_selections and index_type == "displayed":
-                self.create_selected(
-                    len(self.row_positions) - 1 - num_rows,
-                    0,
-                    len(self.row_positions) - 1,
-                    len(self.col_positions) - 1,
-                    "rows",
+            if r + num_rows > len(self.row_positions):
+                new_selected = tuple(
+                    range(
+                        len(self.row_positions) - 1 - num_rows,
+                        len(self.row_positions) - 1,
+                    )
                 )
-        else:
-            if to_move_min > r:
-                new_selected = tuple(range(r, r + num_rows))
-                if create_selections and index_type == "displayed":
+                if create_selections:
                     self.create_selected(
-                        r, 0, r + num_rows, len(self.col_positions) - 1, "rows"
+                        len(self.row_positions) - 1 - num_rows,
+                        0,
+                        len(self.row_positions) - 1,
+                        len(self.col_positions) - 1,
+                        "rows",
                     )
             else:
+                if to_move_min > r:
+                    new_selected = tuple(range(r, r + num_rows))
+                    if create_selections:
+                        self.create_selected(
+                            r, 0, r + num_rows, len(self.col_positions) - 1, "rows"
+                        )
+                else:
+                    new_selected = tuple(range(r + 1 - num_rows, r + 1))
+                    if create_selections:
+                        self.create_selected(
+                            r + 1 - num_rows,
+                            0,
+                            r + 1,
+                            len(self.col_positions) - 1,
+                            "rows",
+                        )
+        elif index_type == "data":
+            if to_move_min > r:
+                new_selected = tuple(range(r, r + num_rows))
+            else:
                 new_selected = tuple(range(r + 1 - num_rows, r + 1))
-                if create_selections and index_type == "displayed":
-                    self.create_selected(
-                        r + 1 - num_rows, 0, r + 1, len(self.col_positions) - 1, "rows"
-                    )
-        if create_selections and index_type == "displayed":
-            self.set_currently_selected(int(new_selected[0]), 0, type_="row")
         newrowsdct = {t1: t2 for t1, t2 in zip(orig_selected, new_selected)}
         if self.all_rows_displayed or index_type != "displayed":
             dispset = {}
             if to_move_min > r:
+                if move_data:
+                    extend_idx = to_move_max - 1
+                    if to_move_max > len(self.data):
+                        self.fix_data_len(extend_idx)
+                    self.data[r:r] = self.data[to_move_min:to_move_max]
+                    self.data[to_move_max:to_del] = []
+                    self.RI.fix_index(extend_idx)
+                    if isinstance(self._row_index, list) and self._row_index:
+                        self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
+                        self._row_index[to_move_max:to_del] = []
                 self.RI.cell_options = {
                     newrowsdct[k]
                     if k in newrowsdct
                     else k + num_rows
                     if k < to_move_min and k >= r
                     else k: v
                     for k, v in self.RI.cell_options.items()
@@ -1263,32 +1311,35 @@
                     newrowsdct[k]
                     if k in newrowsdct
                     else k + num_rows
                     if k < to_move_min and k >= r
                     else k: v
                     for k, v in self.row_options.items()
                 }
-                if move_data:
-                    self.data[r:r] = self.data[to_move_min:to_move_max]
-                    self.data[to_move_max:to_del] = []
-                    self.RI.fix_index(to_move_max)
-                    if isinstance(self._row_index, list) and self._row_index:
-                        self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
-                        self._row_index[to_move_max:to_del] = []
                 if index_type != "displayed":
                     self.displayed_rows = sorted(
                         int(newrowsdct[k])
                         if k in newrowsdct
                         else k + num_rows
                         if k < to_move_min and k >= r
                         else int(k)
                         for k in self.displayed_rows
                     )
             else:
                 r += 1
+                if move_data:
+                    extend_idx = r - 1
+                    if r > len(self.data):
+                        self.fix_data_len(extend_idx)
+                    self.data[r:r] = self.data[to_move_min:to_move_max]
+                    self.data[to_move_min:to_move_max] = []
+                    self.RI.fix_index(extend_idx)
+                    if isinstance(self._row_index, list) and self._row_index:
+                        self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
+                        self._row_index[to_move_min:to_move_max] = []
                 self.RI.cell_options = {
                     newrowsdct[k]
                     if k in newrowsdct
                     else k - num_rows
                     if k < r and k > to_move_min
                     else k: v
                     for k, v in self.RI.cell_options.items()
@@ -1305,74 +1356,54 @@
                     newrowsdct[k]
                     if k in newrowsdct
                     else k - num_rows
                     if k < r and k > to_move_min
                     else k: v
                     for k, v in self.row_options.items()
                 }
-                if move_data:
-                    self.data[r:r] = self.data[to_move_min:to_move_max]
-                    self.data[to_move_min:to_move_max] = []
-                    self.RI.fix_index(r)
-                    if isinstance(self._row_index, list) and self._row_index:
-                        self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
-                        self._row_index[to_move_min:to_move_max] = []
                 if index_type != "displayed":
                     self.displayed_rows = sorted(
                         int(newrowsdct[k])
                         if k in newrowsdct
                         else k - num_rows
                         if k < r and k > to_move_min
                         else int(k)
                         for k in self.displayed_rows
                     )
         else:
             # moves data around, not displayed rows indexes
             # which remain sorted and the same after drop and drop
             if to_move_min > r:
                 dispset = {
-                    b: a
+                    a: b
                     for a, b in zip(
                         self.displayed_rows,
                         (
                             self.displayed_rows[:r]
                             + self.displayed_rows[to_move_min : to_move_min + num_rows]
                             + self.displayed_rows[r:to_move_min]
                             + self.displayed_rows[to_move_min + num_rows :]
                         ),
                     )
                 }
             else:
                 dispset = {
-                    b: a
+                    a: b
                     for a, b in zip(
                         self.displayed_rows,
                         (
                             self.displayed_rows[:to_move_min]
                             + self.displayed_rows[to_move_min + num_rows : r + 1]
                             + self.displayed_rows[to_move_min : to_move_min + num_rows]
                             + self.displayed_rows[r + 1 :]
                         ),
                     )
                 }
             # has to pick up rows from all over the place in the original sheet
             # building an entirely new sheet is best due to permutations of hidden rows
-            self.RI.cell_options = {
-                dispset[k] if k in dispset else k: v
-                for k, v in self.RI.cell_options.items()
-            }
-            self.cell_options = {
-                (dispset[k[0]], k[1]) if k[0] in dispset else k: v
-                for k, v in self.cell_options.items()
-            }
-            self.row_options = {
-                dispset[k] if k in dispset else k: v
-                for k, v in self.row_options.items()
-            }
-            dispset = {b: a for a, b in dispset.items()}
             if move_data:
                 max_len = max(chain(dispset, dispset.values())) + 1
                 if len(self.data) < max_len:
                     self.fix_data_len(max_len - 1)
                 new = []
                 idx = 0
                 done = set()
@@ -1397,14 +1428,27 @@
                             done.add(idx)
                         elif idx not in done:
                             new.append(self._row_index[idx])
                             idx += 1
                         else:
                             idx += 1
                     self._row_index = new
+                dispset = {b: a for a, b in dispset.items()}
+                self.RI.cell_options = {
+                    dispset[k] if k in dispset else k: v
+                    for k, v in self.RI.cell_options.items()
+                }
+                self.cell_options = {
+                    (dispset[k[0]], k[1]) if k[0] in dispset else k: v
+                    for k, v in self.cell_options.items()
+                }
+                self.row_options = {
+                    dispset[k] if k in dispset else k: v
+                    for k, v in self.row_options.items()
+                }
         return new_selected, {b: a for a, b in dispset.items()}
 
     def ctrl_z(self, event=None):
         if not self.undo_storage:
             return
         if not isinstance(self.undo_storage[-1], (tuple, dict)):
             undo_storage = pickle.loads(zlib.decompress(self.undo_storage[-1]))
@@ -1490,22 +1534,40 @@
         elif undo_storage[0] == "move_cols":
             c = undo_storage[1][0]
             to_move_min = undo_storage[2][0]
             totalcols = len(undo_storage[2])
             if to_move_min < c:
                 c += totalcols - 1
             self.move_columns_adjust_options_dict(c, to_move_min, totalcols)
+            self.see(
+                r=0,
+                c=c,
+                keep_yscroll=False,
+                keep_xscroll=False,
+                bottom_right_corner=False,
+                check_cell_visibility=True,
+                redraw=False,
+            )
 
         elif undo_storage[0] == "move_rows":
             r = undo_storage[1][0]
             to_move_min = undo_storage[2][0]
             totalrows = len(undo_storage[2])
             if to_move_min < r:
                 r += totalrows - 1
             self.move_rows_adjust_options_dict(r, to_move_min, totalrows)
+            self.see(
+                r=r,
+                c=0,
+                keep_yscroll=False,
+                keep_xscroll=False,
+                bottom_right_corner=False,
+                check_cell_visibility=True,
+                redraw=False,
+            )
 
         elif undo_storage[0] == "insert_rows":
             self.displayed_rows = undo_storage[1]["displayed_rows"]
             self.data[
                 undo_storage[1]["data_row_num"] : undo_storage[1]["data_row_num"]
                 + undo_storage[1]["numrows"]
             ] = []
@@ -3185,27 +3247,27 @@
             c = self.identify_col(x=event.x)
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
                 self.toggle_select_cell(r, c, redraw=True)
         elif (
             self.RI.width_resizing_enabled
             and self.show_index
             and self.RI.rsz_h is None
-            and self.RI.rsz_w == True
+            and self.RI.rsz_w
         ):
             self.RI.currently_resizing_width = True
             self.new_row_width = self.RI.current_width + event.x
             x = self.canvasx(event.x)
             self.create_resize_line(
                 x, y1, x, y2, width=1, fill=self.RI.resizing_line_fg, tag="rwl"
             )
         elif (
             self.CH.height_resizing_enabled
             and self.show_header
             and self.CH.rsz_w is None
-            and self.CH.rsz_h == True
+            and self.CH.rsz_h
         ):
             self.CH.currently_resizing_height = True
             self.new_header_height = self.CH.current_height + event.y
             y = self.canvasy(event.y)
             self.create_resize_line(
                 x1, y, x2, y, width=1, fill=self.RI.resizing_line_fg, tag="rhl"
             )
@@ -7306,30 +7368,34 @@
     def get_empty_row_seq(self, datarn, end, start=0, r_ops=True, c_ops=True):
         return [
             self.get_value_for_empty_cell(datarn, datacn, r_ops=r_ops, c_ops=c_ops)
             for datacn in range(start, end)
         ]
 
     def fix_row_len(self, datarn, datacn):
-        self.data[datarn].extend(self.get_empty_row_seq(datarn, 
-                                                        end = datacn + 1, 
-                                                        start = len(self.data[datarn])))
+        self.data[datarn].extend(
+            self.get_empty_row_seq(datarn, end=datacn + 1, start=len(self.data[datarn]))
+        )
 
     def fix_row_values(self, datarn, start=None, end=None):
         if datarn < len(self.data):
             for datacn, v in enumerate(islice(self.data[datarn], start, end)):
                 if not self.input_valid_for_cell(datarn, datacn, v):
                     self.data[datarn][datacn] = self.get_value_for_empty_cell(
                         datarn, datacn
                     )
 
     def fix_data_len(self, datarn, datacn):
         ncols = self.total_data_cols() if datacn is None else datacn + 1
-        self.data.extend([self.get_empty_row_seq(rn, end = ncols, start = 0) 
-                          for rn in range(len(self.data), datarn + 1)])
+        self.data.extend(
+            [
+                self.get_empty_row_seq(rn, end=ncols, start=0)
+                for rn in range(len(self.data), datarn + 1)
+            ]
+        )
 
     # internal event use
     def click_checkbox(self, r, c, datarn=None, datacn=None, undo=True, redraw=True):
         if datarn is None:
             datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         if datacn is None:
             datacn = c if self.all_columns_displayed else self.displayed_columns[c]
@@ -7461,15 +7527,15 @@
             else ""
         )
         for datarn in range(self.total_data_rows()):
             self.set_cell_data(datarn, datacn, value)
 
     def dropdown_sheet(self, **kwargs):
         if "dropdown" in self.options or "checkbox" in self.options:
-            self.delete_cell_options_dropdown_and_checkbox(datarn, datacn)
+            self.delete_options_dropdown_and_checkbox()
         self.options["dropdown"] = get_dropdown_dict(**kwargs)
         value = (
             kwargs["set_value"]
             if kwargs["set_value"] is not None
             else kwargs["values"][0]
             if kwargs["values"]
             else ""
```

### Comparing `tksheet-6.1.1/tksheet/_tksheet_other_classes.py` & `tksheet-6.1.2/tksheet/_tksheet_other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.1/tksheet/_tksheet_row_index.py` & `tksheet-6.1.2/tksheet/_tksheet_row_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
             self.MT.main_table_redraw_grid_and_text(
                 redraw_header=True, redraw_row_index=True
             )
             if self.row_height_resize_func is not None and old_height != new_height:
                 self.row_height_resize_func(
                     ResizeEvent("row_height_resize", row, old_height, new_height)
                 )
-        elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w == True:
+        elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w:
             self.set_width_of_index_to_text()
         elif self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
             r = self.MT.identify_row(y=event.y)
             if r < len(self.MT.row_positions) - 1:
                 if self.MT.single_selection_enabled:
                     self.select_row(r, redraw=True)
                 elif self.MT.toggle_selection_enabled:
@@ -453,15 +453,15 @@
                 width=1,
                 fill=self.resizing_line_fg,
                 tag="rhl2",
             )
             self.MT.create_resize_line(
                 x1, line2y, x2, line2y, width=1, fill=self.resizing_line_fg, tag="rhl2"
             )
-        elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w == True:
+        elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w:
             self.currently_resizing_width = True
             x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
             x = int(event.x)
             if x < self.MT.min_column_width:
                 x = int(self.MT.min_column_width)
             self.new_row_width = x
             self.create_resize_line(
```

### Comparing `tksheet-6.1.1/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.1.2/tksheet/_tksheet_top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.1/tksheet/_tksheet_vars.py` & `tksheet-6.1.2/tksheet/_tksheet_vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.1/tksheet.egg-info/PKG-INFO` & `tksheet-6.1.2/tksheet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.1
+Version: 6.1.2
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.1.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.2.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

