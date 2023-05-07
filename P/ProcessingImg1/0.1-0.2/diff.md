# Comparing `tmp/ProcessingImg1-0.1.tar.gz` & `tmp/ProcessingImg1-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProcessingImg1-0.1.tar", last modified: Fri May  5 19:36:42 2023, max compression
+gzip compressed data, was "ProcessingImg1-0.2.tar", last modified: Sun May  7 13:30:46 2023, max compression
```

## Comparing `ProcessingImg1-0.1.tar` & `ProcessingImg1-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:36:42.412020 ProcessingImg1-0.1/
--rw-rw-rw-   0        0        0       46 2023-05-05 19:12:48.000000 ProcessingImg1-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      419 2023-05-05 19:36:42.412020 ProcessingImg1-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 19:36:42.406381 ProcessingImg1-0.1/ProcessingImg1.egg-info/
--rw-rw-rw-   0        0        0      419 2023-05-05 19:36:42.000000 ProcessingImg1-0.1/ProcessingImg1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-05 19:36:42.000000 ProcessingImg1-0.1/ProcessingImg1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:36:42.000000 ProcessingImg1-0.1/ProcessingImg1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-05 19:36:42.000000 ProcessingImg1-0.1/ProcessingImg1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3213 2023-05-05 19:12:45.000000 ProcessingImg1-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 19:36:42.408030 ProcessingImg1-0.1/organize/
--rw-rw-rw-   0        0        0     4771 2023-05-05 19:12:43.000000 ProcessingImg1-0.1/organize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:36:42.410026 ProcessingImg1-0.1/processing/
--rw-rw-rw-   0        0        0    13744 2023-05-05 18:49:37.000000 ProcessingImg1-0.1/processing/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-05 19:36:42.412020 ProcessingImg1-0.1/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-05-05 19:35:59.000000 ProcessingImg1-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:30:46.480398 ProcessingImg1-0.2/
+-rw-rw-rw-   0        0        0       46 2023-05-07 13:26:18.000000 ProcessingImg1-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      825 2023-05-07 13:30:46.480398 ProcessingImg1-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-07 13:30:46.473416 ProcessingImg1-0.2/ProcessingImg1.egg-info/
+-rw-rw-rw-   0        0        0      825 2023-05-07 13:30:46.000000 ProcessingImg1-0.2/ProcessingImg1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-07 13:30:46.000000 ProcessingImg1-0.2/ProcessingImg1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 13:30:46.000000 ProcessingImg1-0.2/ProcessingImg1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-07 13:30:46.000000 ProcessingImg1-0.2/ProcessingImg1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4443 2023-05-07 13:16:05.000000 ProcessingImg1-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 13:30:46.474413 ProcessingImg1-0.2/organize/
+-rw-rw-rw-   0        0        0     4469 2023-05-07 13:26:48.000000 ProcessingImg1-0.2/organize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:30:46.476434 ProcessingImg1-0.2/processing/
+-rw-rw-rw-   0        0        0    14855 2023-05-07 13:26:37.000000 ProcessingImg1-0.2/processing/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-07 13:30:46.481394 ProcessingImg1-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1007 2023-05-07 13:25:07.000000 ProcessingImg1-0.2/setup.py
```

### Comparing `ProcessingImg1-0.1/README.md` & `ProcessingImg1-0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-# Proc_Image
+# ProcessingImg1
 Small and simple image processing library
 
 # How to Install The Library?
-## pip install ProcImage
+## pip install ProcessingImg1
 
 ## First, this is a simple and compact package for image processing and hardware management developed using the Pillow package
 ------------------------
 
-* First: This package contains two volumes, the first folder is called *Image_* This folder contains a file called *image_processing.py* and this file is for image processing
 
---------------------
 
-
-* Secondly: The second folder is called *organize* and this folder contains a file called *organize_hard.py* for organizing the  that arranges the pictures, folders, applications, etc... It arranges and organizes them well and neatly.
-
-
-
-1- Now: We start giving examples of the folder *Image_* We agree that this folder contains a Python file named *processing_image.py* and this file contains several functions. We will now give examples of these functions in this file.
+1- Now: We start giving examples of the folder *processing* We agree that this folder contains a Python file named *__init__.py* and this file contains several functions. We will now give examples of these functions in this file.
 
 
 ## Let's take an example : about the function <font color='red'>get_list(path)</font> it takes the path of a folder and then returns all the images as a table
 
 
 ```python
 from processing import ImageProcessing
@@ -48,15 +41,15 @@
 
 ##### ['33.jpg', 'A.jpg', 'aesthetic-ocean-cell-phone-art-94x4pcvrtazi8upm.jpg', 'palm-tree-1.jpg', 'rr.jpg', 'test.jpg', 'test1.jpg', 'veidz.jpg']
 
 -----
 # Example Two
 
 ### The first function <font color='red'>get_list_sorted(main_path , answer)</font> takes the full path of the target image folder,
-###and takes the user's answer, in order to arrange the images in ascending or descending order. In the entered folder
+and takes the user's answer, in order to arrange the images in ascending or descending order. In the entered folder
 
 
 ```python
 from processing import ImageProcessing
 my_object = ImageProcessing()
 
 print(my_object.get_list_sorted(r"C:\Users\Alaa\Pictures",False))
@@ -85,9 +78,52 @@
 
 ##### name Image :A.jpg
 ##### total dimensions :6400 Pixel
 ##### Location :C:\Users\Alaa\Pictures
 ----
 
 
+----
+
+### Referring to the example of the convert_image function, the function that converts an image from a PNG or other extension into a thumbnail with the ICO file extension
+
+```python
+from processing import ImageProcessing
+result = ImageProcessing.convert_image(path="C:\\Alaa.png" , extension=".jpg", size=(50, 50))
+
+
+
+```
+
+---
+
+```python
+    @staticmethod
+    def convert_image(**kwargs):
+        """Convert the image to a thumbnail with ICO File extension"""
+        try:
+            path = kwargs.get('path')
+            extension = kwargs.get('extension')
+            size = kwargs.get('size')
+
+            if not os.path.exists(path):
+                raise FileNotFoundError("The path is wrong, please check it :{}".format(path))
+            elif os.path.isfile(path) and os.path.splitext(path)[1] != extension:
+                raise TypeError("The file type is wrong, please check it :{}".format(extension))
+            else:
+                list_extension = ["path" , "extension" , "size"]
+                for (check_key) in list_extension :
+                    if check_key not in kwargs.keys():
+                        raise KeyError("The key is wrong, you must write the keys correctly (path),(extension),(size)")
+
+                with Image.open(path) as image:
+                    image.thumbnail(size, Image.Resampling.BICUBIC)
+                    image.save(os.path.splitext(path)[0] + '.ico', format='ICO')
+
+                print("The image has been successfully saved in place :{}".format(os.path.splitext(path)[0] + '.ico', format='ICO'))
+
+        except Exception as error:
+            return error
+
+```
 ![Developer](https://lh3.googleusercontent.com/ogw/ADea4I69npfzwotm16-3HpRfSP4VbW87nXPfi5b8FD-mNu4=s32-c-mo)
 ["Developer"](https://www.facebook.com/alaa.jassim.mohammed)
```

### Comparing `ProcessingImg1-0.1/organize/__init__.py` & `ProcessingImg1-0.2/organize/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 
 
+
+
 """
 -1 The first function: images arranges the images and then add them in 
 a new folder. This function takes the path of the images folder + the name 
 of the new folder in which all images will be added.
 
 -2 The first function: files arranges files of all kinds and then add them in 
 a new folder. This function takes the path of the files 
@@ -22,19 +24,16 @@
 all kinds and then add them in a new folder and this function 
 takes the path of the applications folder + the name of the new folder in which all files and applications will be added
 """
 
 import os , shutil
 class Organize:
 	""" Hardware Regulation """
-	def __init__(self):
-		self.condition = False
-
-	def images(self,currnet_path ,new_folder):
-		""" The function responsible for organizing the images git full path dir"""
+	@staticmethod
+	def images(currnet_path , new_folder):
 		try :
 			if not os.path.isdir(currnet_path):
 				raise FileNotFoundError("Path not found :{}".format(currnet_path))
 
 			for filename in os.listdir(currnet_path):
 				if filename.endswith((
 						".png" , ".jpg" , ".jpeg" , ".gif" ,
@@ -47,16 +46,19 @@
 						os.mkdir(new_folder)
 					shutil.copy(currnet_path + '\\' + filename , new_folder)
 					os.remove(currnet_path + '\\' + filename)
 		except Exception as error:
 			return error
 
 
-	def files(self,currnet_path ,new_folder):
-		""" This function organizes files git currnet path And git new folder """
+
+
+
+	@staticmethod
+	def files(currnet_path,new_folder):
 		try :
 			if not os.path.isdir(currnet_path):
 				raise FileNotFoundError("Path not found :{}".format(currnet_path))
 
 			for filename in os.listdir(currnet_path):
 				if filename.endswith((
 						".txt" , ".pdf" , ".py" , ".css" ,
@@ -69,16 +71,18 @@
 						os.mkdir(new_folder)
 					shutil.copy(currnet_path + '\\' + filename , new_folder)
 					os.remove(currnet_path + '\\' + filename)
 		except Exception as error:
 			return error
 
 
+ 
 
-	def videos(self,currnet_path ,new_folder):
+	@staticmethod
+	def videos(currnet_path ,new_folder):
 		""" This function organizes Videos git currnet path And git new folder """
 		try :
 			if not os.path.isdir(currnet_path):
 				raise FileNotFoundError("Path not found :{}".format(currnet_path))
 
 			for filename in os.listdir(currnet_path):
 				if filename.endswith((
@@ -91,17 +95,16 @@
 					if not os.path.exists(new_folder):
 						os.mkdir(new_folder)
 					shutil.copy(currnet_path + '\\' + filename , new_folder)
 					os.remove(currnet_path + '\\' + filename)
 		except Exception as error:
 			return error
 
-
-	def music(self,currnet_path ,new_folder):
-		""" This function organizes Music git currnet path And git new folder """
+	@staticmethod
+	def music(currnet_path ,new_folder):
 		try :
 			if not os.path.isdir(currnet_path):
 				raise FileNotFoundError("Path not found :{}".format(currnet_path))
 
 			for filename in os.listdir(currnet_path):
 				if filename.endswith((
 						".webm" , ".mpg" , ".mp2" , ".mpe" ,
@@ -114,16 +117,16 @@
 						os.mkdir(new_folder)
 					shutil.copy(currnet_path + '\\' + filename , new_folder)
 					os.remove(currnet_path + '\\' + filename)
 		except Exception as error:
 			return error
 
 
-	def applications(self,currnet_path ,new_folder):
-		""" This function organizes Applications git currnet path And git new folder """
+	@staticmethod
+	def applications(currnet_path,new_folder):
 		try :
 			if not os.path.isdir(currnet_path):
 				raise FileNotFoundError("Path not found :{}".format(currnet_path))
 
 			for filename in os.listdir(currnet_path):
 				if filename.endswith((".exe",".dmp")):
```

