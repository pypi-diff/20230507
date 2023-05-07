# Comparing `tmp/extended_tk-0.13.0-py3-none-any.whl.zip` & `tmp/extended_tk-0.14.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7206 bytes, number of entries: 7
+Zip file size: 8060 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat     9452 b- defN 23-Apr-24 19:44 TkPlus/__init__.py
--rw-rw-rw-  2.0 fat     9977 b- defN 23-May-05 10:40 extended_tk/__init__.py
--rw-rw-rw-  2.0 fat      243 b- defN 23-May-05 11:48 extended_tk-0.13.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      717 b- defN 23-May-05 11:48 extended_tk-0.13.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-05 11:48 extended_tk-0.13.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-05 11:48 extended_tk-0.13.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      564 b- defN 23-May-05 11:48 extended_tk-0.13.0.dist-info/RECORD
-7 files, 21057 bytes uncompressed, 6202 bytes compressed:  70.5%
+-rw-rw-rw-  2.0 fat    10837 b- defN 23-May-07 11:32 extended_tk/__init__.py
+-rw-rw-rw-  2.0 fat      243 b- defN 23-May-07 11:43 extended_tk-0.14.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2252 b- defN 23-May-07 11:43 extended_tk-0.14.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 11:43 extended_tk-0.14.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-07 11:43 extended_tk-0.14.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      566 b- defN 23-May-07 11:43 extended_tk-0.14.0.dist-info/RECORD
+7 files, 23454 bytes uncompressed, 7056 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: TkPlus/__init__.py
 Comment: 
 
 Filename: extended_tk/__init__.py
 Comment: 
 
-Filename: extended_tk-0.13.0.dist-info/LICENSE
+Filename: extended_tk-0.14.0.dist-info/LICENSE
 Comment: 
 
-Filename: extended_tk-0.13.0.dist-info/METADATA
+Filename: extended_tk-0.14.0.dist-info/METADATA
 Comment: 
 
-Filename: extended_tk-0.13.0.dist-info/WHEEL
+Filename: extended_tk-0.14.0.dist-info/WHEEL
 Comment: 
 
-Filename: extended_tk-0.13.0.dist-info/top_level.txt
+Filename: extended_tk-0.14.0.dist-info/top_level.txt
 Comment: 
 
-Filename: extended_tk-0.13.0.dist-info/RECORD
+Filename: extended_tk-0.14.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## extended_tk/__init__.py

```diff
@@ -9,16 +9,17 @@
 # __MAIN CODE__ #
 class Add_Delete(Button):
     '''
     Creates a button pair to add or delete a copy of the row
     in which they are placed.
     ONLY WITH GRID!!
     '''
-    def __init__(self, master, scale=1, min_row=1, max_row=-1, textFont='Bell MT', textSize=10):
+    def __init__(self, master, scale=1, min_row=1, max_row=-1, textFont='Bell MT', textSize=10, extra:tuple=()):
         Button.__init__(self, master)
+        self.__extra = extra
         self.__min = min_row
         self.__max = max_row
         self.__row = self.master.grid_size()[1]
         self.__dic = self.master.__dict__['children'].values()
         self.add = Button(
             master, text='+',
             font=(textFont, int(textSize*scale)),
@@ -29,14 +30,33 @@
             master, text='-',
             font=(textFont, int((textSize)*scale)),
             state=DISABLED, width=self.add['width'],
             command=self.__del_row
         )
         self.delete.grid(row=master.grid_size()[1]-1, column=master.grid_size()[0]+1)
         
+    def add_extra(self, *args):
+        self.__extra = args
+        
+    def __move_down(self):
+        for item in self.__extra:
+            for info in item.grid_info():
+                if info == 'row':
+                    item.grid({'row': item.grid_info()[info]+1})
+                else:
+                    item.grid({info: item.grid_info()[info]})
+    
+    def __move_up(self):
+        for item in self.__extra:
+            for info in item.grid_info():
+                if info == 'row':
+                    item.grid({'row': item.grid_info()[info]-1})
+                else:
+                    item.grid({info: item.grid_info()[info]})
+        
     def __copiable(self, item):
         no_copy = [Button, Frame]
         for type in no_copy:
             if isinstance(item, type):
                 return False
         return True
             
@@ -65,14 +85,16 @@
         self.add.grid(row=self.__row)
         self.delete.grid(row=self.__row)
         self.__row = self.master.grid_size()[1]
         if self.__row >= self.__min:
             self.delete.config(state=NORMAL)
         if self.__row == self.__max and self.__max != -1:
             self.add.config(state=DISABLED)
+        if not len(self.__extra) == 0:
+            self.__move_down()
         
     def __del_row(self):
         '''
         Deletes the current row of items.
         '''
         to_delete = [i for i in self.__dic if not isinstance(i, Button) and i.grid_info()['row']==self.__row-1]
         for item in to_delete:
@@ -80,14 +102,16 @@
         self.add.grid(row=self.__row-2)
         self.delete.grid(row=self.__row-2)
         self.__row = self.master.grid_size()[1]
         if self.__row <= self.__min:
             self.delete.config(state=DISABLED)
         if self.__row < self.__max:
             self.add.config(state=NORMAL)
+        if not len(self.__extra) == 0:
+            self.__move_up()
 
 class Checkbox(Checkbutton):
     '''
     A simplified CheckBox with a simply usage to set active or
     inactive some features.
     '''
```

