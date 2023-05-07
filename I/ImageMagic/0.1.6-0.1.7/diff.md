# Comparing `tmp/ImageMagic-0.1.6.tar.gz` & `tmp/ImageMagic-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImageMagic-0.1.6.tar", last modified: Fri May  5 10:55:03 2023, max compression
+gzip compressed data, was "ImageMagic-0.1.7.tar", last modified: Sun May  7 01:24:37 2023, max compression
```

## Comparing `ImageMagic-0.1.6.tar` & `ImageMagic-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 10:55:03.106652 ImageMagic-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-05-05 10:55:03.091027 ImageMagic-0.1.6/ImageMagic/
--rw-rw-rw-   0        0        0     6184 2023-05-04 12:40:18.000000 ImageMagic-0.1.6/ImageMagic/Aocr.py
--rw-rw-rw-   0        0        0    11530 2023-05-05 10:43:04.000000 ImageMagic-0.1.6/ImageMagic/Image.py
--rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.1.6/ImageMagic/_Atesseract.py
--rw-rw-rw-   0        0        0      260 2023-05-04 12:55:21.000000 ImageMagic-0.1.6/ImageMagic/__init__.py
--rw-rw-rw-   0        0        0       85 2023-05-05 10:54:35.000000 ImageMagic-0.1.6/ImageMagic/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:55:03.106652 ImageMagic-0.1.6/ImageMagic.egg-info/
--rw-rw-rw-   0        0        0      500 2023-05-05 10:55:02.000000 ImageMagic-0.1.6/ImageMagic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-05-05 10:55:03.000000 ImageMagic-0.1.6/ImageMagic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 10:55:02.000000 ImageMagic-0.1.6/ImageMagic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-05 10:55:02.000000 ImageMagic-0.1.6/ImageMagic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-05 10:55:02.000000 ImageMagic-0.1.6/ImageMagic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      500 2023-05-05 10:55:03.106652 ImageMagic-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1096 2023-05-05 10:54:35.000000 ImageMagic-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 10:55:03.106652 ImageMagic-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      778 2023-05-05 10:53:04.000000 ImageMagic-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:24:37.957534 ImageMagic-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-05-07 01:24:37.941909 ImageMagic-0.1.7/ImageMagic/
+-rw-rw-rw-   0        0        0     6237 2023-05-07 00:54:28.000000 ImageMagic-0.1.7/ImageMagic/Aocr.py
+-rw-rw-rw-   0        0        0    13766 2023-05-07 01:13:22.000000 ImageMagic-0.1.7/ImageMagic/Image.py
+-rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.1.7/ImageMagic/_Atesseract.py
+-rw-rw-rw-   0        0        0      260 2023-05-04 12:55:21.000000 ImageMagic-0.1.7/ImageMagic/__init__.py
+-rw-rw-rw-   0        0        0       85 2023-05-07 01:24:05.000000 ImageMagic-0.1.7/ImageMagic/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:24:37.957534 ImageMagic-0.1.7/ImageMagic.egg-info/
+-rw-rw-rw-   0        0        0      500 2023-05-07 01:24:37.000000 ImageMagic-0.1.7/ImageMagic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-05-07 01:24:37.000000 ImageMagic-0.1.7/ImageMagic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 01:24:37.000000 ImageMagic-0.1.7/ImageMagic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-07 01:24:37.000000 ImageMagic-0.1.7/ImageMagic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 01:24:37.000000 ImageMagic-0.1.7/ImageMagic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      500 2023-05-07 01:24:37.957534 ImageMagic-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1231 2023-05-06 11:02:24.000000 ImageMagic-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 01:24:37.957534 ImageMagic-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-05-06 05:17:18.000000 ImageMagic-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:24:37.957534 ImageMagic-0.1.7/test/
+-rw-rw-rw-   0        0        0     1286 2023-05-07 01:21:31.000000 ImageMagic-0.1.7/test/test.py
```

### Comparing `ImageMagic-0.1.6/ImageMagic/Aocr.py` & `ImageMagic-0.1.7/ImageMagic/Aocr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from ImageMagic._Atesseract import *
+from . import _Atesseract as tess
 from PIL import Image
 
 
 
-def image_to_text(filePath,lang='chi_sim',config='',nice=0,output_type=Output.STRING,timeout=0,):
+def image_to_text(filePath,lang='chi_sim',config='',nice=0,output_type=tess.Output.STRING,timeout=0,):
 
     """
     Gets the text content of the picture
     Args:
         filePath: Image path
         lang: The language of the image text, multi-language please use the plus sign, e.g: 'chi_sim+eng'
         config: Any other custom configuration flags that cannot be used by the Aocr function
@@ -16,33 +16,33 @@
         timeout: The length of the timeout
 
     Returns:
         Text content
     """
 
     image = Image.open(filePath)
-    text = imageToString(image,lang=lang,config=config,nice=nice,output_type=output_type,timeout=timeout)
+    text = tess.imageToString(image,lang=lang,config=config,nice=nice,output_type=output_type,timeout=timeout)
     return text
 
 
 def check_languages(config=''):
 
     """
     Gets the installed languages
     Args:
         config: Any other custom configuration flags that cannot be used by the Aocr function
 
     Returns:
         Supported languages
     """
-    languages = getLanguages(config=config)
+    languages = tess.getLanguages(config=config)
     return languages
 
 
-def get_image_boxs(filePath,lang='chi_sim',config='',nice=0,output_type=Output.STRING,timeout=0):
+def get_image_boxs(filePath,lang='chi_sim',config='',nice=0,output_type=tess.Output.STRING,timeout=0):
 
     """
     Gets an estimate of the picture bounding box
     Args:
         filePath: Image path
         lang: The language of the image text, multi-language please use the plus sign, e.g: 'chi_sim+eng'
         config: Any other custom configuration flags that cannot be used by the Aocr function
@@ -50,19 +50,19 @@
         output_type: Output type, defaulting to string type | including BYTES, DATAFRAME, DICT, STRING
         timeout: The length of the timeout
 
     Returns:
         Border estimate
     """
     image = Image.open(filePath)
-    boxs = imageToBoxes(image,lang=lang,config=config,nice=nice,output_type=output_type,timeout=timeout)
+    boxs = tess.imageToBoxes(image,lang=lang,config=config,nice=nice,output_type=output_type,timeout=timeout)
     return boxs
 
 
-def get_image_osd(filePath,lang='chi_sim',config='',nice=0,output_type=Output.STRING,timeout=0):
+def get_image_osd(filePath,lang='chi_sim',config='',nice=0,output_type=tess.Output.STRING,timeout=0):
 
     """
     Get information about orientation and script detection
     Args:
         filePath: Image path
         lang: The language of the image text, multi-language please use the plus sign, e.g: 'chi_sim+eng'
         config: Any other custom configuration flags that cannot be used by the Aocr function
@@ -71,19 +71,19 @@
         timeout: The length of the timeout
 
     Returns:
         Direction and script detection information
     """
 
     image = Image.open(filePath)
-    osd = imageToOsd(image,lang=lang,config=config,nice=nice,output_type=output_type,timeout=timeout)
+    osd = tess.imageToOsd(image,lang=lang,config=config,nice=nice,output_type=output_type,timeout=timeout)
     return osd
 
 
-def get_image_data(filePath,lang='chi_sim',config='',nice=0,output_type=Output.STRING,timeout=0):
+def get_image_data(filePath,lang='chi_sim',config='',nice=0,output_type=tess.Output.STRING,timeout=0):
 
     """
     Get image details, including boxes, confidence, line numbers, and page numbers.
     Requires Tesseract 3.05+
     Args:
         filePath: Image path
         lang: The language of the image text, multi-language please use the plus sign, e.g: 'chi_sim+eng'
@@ -93,15 +93,15 @@
         timeout: The length of the timeout
 
     Returns:
         Detailed data for the picture, including boxes, confidence, line numbers, and page numbers
     """
 
     image = Image.open(filePath)
-    data = imageToData(image,lang=lang,config=config,nice=nice,output_type=output_type,timeout=timeout)
+    data = tess.imageToData(image,lang=lang,config=config,nice=nice,output_type=output_type,timeout=timeout)
     return data
 
 
 def image_to_pdf(imagePath,savePath,lang='chi_sim',config='',nice=0,timeout=0):
 
     """
     Convert images into searchable PDF files
@@ -113,15 +113,15 @@
         nice: Modify the processor priority that Tesseract runs, which Windows does not support
         timeout: The length of the timeout
 
     Returns:
         None
     """
 
-    pdf = imageToPdfOrHocr(imagePath,lang=lang,config=config,nice=nice,extension='pdf',timeout=timeout)
+    pdf = tess.imageToPdfOrHocr(imagePath,lang=lang,config=config,nice=nice,extension='pdf',timeout=timeout)
     with open(savePath,'wb') as f:
         f.write(pdf)
 
 def image_to_hocr(filePath,lang='chi_sim',config='',nice=0,timeout=0):
 
     """
     Get the HOCR output
@@ -132,15 +132,15 @@
         nice: Modify the processor priority that Tesseract runs, which Windows does not support
         timeout: The length of the timeout
 
     Returns:
         HOCR
     """
 
-    hocr = imageToPdfOrHocr(filePath,lang=lang,config=config,extension='hocr',nice=nice,timeout=timeout)
+    hocr = tess.imageToPdfOrHocr(filePath,lang=lang,config=config,extension='hocr',nice=nice,timeout=timeout)
     return hocr
 
 def image_to_AltoXml(filePath,lang='chi_sim',config='',nice=0,timeout=0):
 
     """
     Returns the result of a Tesseract OCR run on the provided image to ALTO XML
     Args:
@@ -150,10 +150,9 @@
         nice: Modify the processor priority that Tesseract runs, which Windows does not support
         timeout: The length of the timeout
 
     Returns:
         Returns the result of a Tesseract OCR run on the provided image to ALTO XML
     """
 
-    xml = imageToAltoXml(filePath,lang=lang,config=config,nice=nice,timeout=timeout)
-    return xml
-
+    xml = tess.imageToAltoXml(filePath,lang=lang,config=config,nice=nice,timeout=timeout)
+    return xml
```

### Comparing `ImageMagic-0.1.6/ImageMagic/Image.py` & `ImageMagic-0.1.7/ImageMagic/Image.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import hashlib
 import hmac
 import base64
 import time
 import os
 from loguru import logger
 import shutil
-
+import struct
 
 #They are used in the Audio class
 RESULT = None
 ANSWER = None
 
 
 def word_to_image(text, path, fontPath=r'C:\Windows\Fonts\STXIHEI.TTF', LinesWords=14, fontsize=45, type='png', color=(255, 255, 255)):
@@ -151,14 +151,96 @@
     if new_width is None and new_height is None:
         img = img.resize((int(width),int(height)),PILImage.Resampling.LANCZOS)
     else:
         img = img.resize((int(new_width),int(new_height)),PILImage.Resampling.LANCZOS)
     img.save(savePath)
 
 
+def get_image_hash(image_path):
+
+    """
+    Gets the hash value of the image
+    Args:
+        image_path: Image path
+
+    Returns:
+        The hash of the image (consisting of 0 and 1)
+    """
+
+    img = PILImage.open(image_path)
+    w = img.size[0]
+    h = img.size[1]
+    img.close() #关闭img，释放资源
+
+    # 打开图像文件
+    with open(image_path, "rb") as f:
+        data = f.read()
+    # 解析图像头信息
+    width, height = struct.unpack('>II', data[16:24])
+    pixel_data = data[24:]
+
+    # 调整图像大小
+    if w > width or h > height:
+        raise ValueError("Invalid size")
+    xstep = width // w
+    ystep = height // h
+
+    # 计算像素均值并生成哈希值
+    pixels = []
+    for y in range(h):
+        for x in range(w):
+            pixel = pixel_data[((y * ystep) * width + (x * xstep)) * 3:((y * ystep) * width + (x * xstep)) * 3 + 3]
+            pixels.append(sum(pixel) / 3)
+
+    # 计算平均像素值
+    avg_pixel = sum(pixels) / len(pixels)
+
+    # 生成哈希值
+    hash_value = ""
+    for pixel in pixels:
+        if pixel > avg_pixel:
+            hash_value += "1"
+        else:
+            hash_value += "0"
+    return hash_value
+
+def remove_same_images(directoryPath):
+
+    """
+    Delete the same images in the directory, and calculate the hash value of the images to identify whether the pictures are the same.
+    Supports jpg, png, bmp, webp, jpeg, gif, svg, tif, tiff.
+    Args:
+        directoryPath: The file directory path
+
+    Returns:
+        None
+    """
+
+    # 保存图像哈希值和路径
+    hashes = {}
+
+    # 遍历目录中的所有图像
+    for filename in os.listdir(directoryPath):
+        if not filename.endswith((".jpg", ".png", ".bmp",".webp",".jpeg",".gif","svg","tif","tiff")):
+            continue
+        filepath = os.path.join(directoryPath, filename)
+
+        # 计算图像哈希值
+        hash_value = get_image_hash(filepath)
+
+        # 如果哈希值已经存在，则删除图像
+        if hash_value in hashes:
+            logger.info(f"Removing duplicate image: {filepath}")
+            os.remove(filepath)
+        else:
+            hashes[hash_value] = filepath
+
+    logger.info("Done removing duplicate images.")
+
+
 def categorize_image(filePath):
 
     """
     Categorize your images, support jpg, jpeg, png, webp, bmp, tif, tiff, gif, svg, wmf
     Args:
         filePath: Your folder path
 
@@ -168,63 +250,63 @@
 
     for filename in os.listdir(filePath):
         ext = os.path.splitext(filename)[1].lower()
 
         if ext == ".png":
             try:
                 os.makedirs(f'{filePath}/png')
-            except FileExistsError as error:
+            except FileExistsError:
                 pass
             shutil.copy(os.path.join(filePath, filename), f'{filePath}/png')
         elif ext == ".jpg" or ext == 'jpeg':
             try:
                 os.makedirs(f'{filePath}/jpg')
-            except FileExistsError as error:
+            except FileExistsError:
                 pass
             shutil.copy(os.path.join(filePath, filename), f'{filePath}/jpg')
         elif ext == '.webp':
             try:
                 os.makedirs(f'{filePath}/webp')
-            except FileExistsError as error:
+            except FileExistsError:
                 pass
             shutil.copy(os.path.join(filePath, filename), f'{filePath}/webp')
         elif ext == 'bmp':
             try:
                 os.makedirs(f'{filePath}/bmp')
-            except FileExistsError as error:
+            except FileExistsError:
                 pass
             shutil.copy(os.path.join(filePath,filename),f'{filePath}/bmp')
         elif ext == 'tif' or ext == 'tiff':
             try:
                 os.makedirs(f'{filePath}/tif')
-            except FileExistsError as error:
+            except FileExistsError:
                 pass
             shutil.copy(os.path.join(filePath,filename),f'{filePath}/tif')
         elif ext == 'gif':
             try:
                 os.makedirs(f'{filePath}/gif')
-            except FileExistsError as error:
+            except FileExistsError:
                 pass
             shutil.copy(os.path.join(filePath,filename),f'{filePath}/gif')
         elif ext == 'svg':
             try:
                 os.makedirs(f'{filePath}/svg')
-            except FileExistsError as error:
+            except FileExistsError:
                 pass
             shutil.copy(os.path.join(filePath,filename),f'{filePath}/svg')
         elif ext == 'wmf':
             try:
                 os.makedirs(f'{filePath}/wmf')
-            except FileExistsError as error:
+            except FileExistsError:
                 pass
             shutil.copy(os.path.join(filePath,filename),f'{filePath}/wmf')
         else:
             try:
                 os.makedirs(f'{filePath}/another')
-            except FileExistsError as error:
+            except FileExistsError:
                 pass
             shutil.copy(os.path.join(filePath,filename),f'{filePath}/another')
 
 
 class Audio:
 
     """
```

### Comparing `ImageMagic-0.1.6/ImageMagic/_Atesseract.py` & `ImageMagic-0.1.7/ImageMagic/_Atesseract.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.6/LICENSE` & `ImageMagic-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.6/README.md` & `ImageMagic-0.1.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 1. 使用pip下载
 ```
 pip install ImageMagic
 ```
 
 2. 或者，你也可以从[源](https://github.com/asxez/ImageMagic)进行构建
 
+# 文档
+[文档](https://www.asxe.vip/2023/05/05/ImageMagic%E7%9A%84API%E6%96%87%E6%A1%A3(%E4%B8%AD%E8%8B%B1%E6%96%87%E7%89%88)/)
+
 # 依赖
   - [PIL](https://github.com/python-pillow/Pillow)
   - [Tesseract-OCR](https://tesseract-ocr.github.io/tessdoc/Installation.html)
   - [numpy](https://github.com/numpy/numpy)
   - [pandas](https://github.com/pandas-dev/pandas)
   - ……
```

### Comparing `ImageMagic-0.1.6/setup.py` & `ImageMagic-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages
 from ImageMagic import _version
 
 setup(
     name='ImageMagic',
     version=_version.__version__,
-    packages=find_packages(),
+    packages=find_packages(exclude='test*'),
     url='https://github.com/asxez/ImageMagic',
     license='GNU GPL 3.0',
     author='asxe',
     author_email='2973918177@qq.com',
     description='图像处理库（包括但不限于图像）【Image processing libraries (including but not limited to images)】',
     long_description='It is a neat image processing library, and you can even achieve what you want with just one line of code, such as text-to-image or image content recognition (OCR), and more!',
     install_requires=[
```

