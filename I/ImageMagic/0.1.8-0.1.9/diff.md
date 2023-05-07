# Comparing `tmp/ImageMagic-0.1.8.tar.gz` & `tmp/ImageMagic-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImageMagic-0.1.8.tar", last modified: Sun May  7 01:47:02 2023, max compression
+gzip compressed data, was "ImageMagic-0.1.9.tar", last modified: Sun May  7 05:16:23 2023, max compression
```

## Comparing `ImageMagic-0.1.8.tar` & `ImageMagic-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 01:47:02.358485 ImageMagic-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-05-07 01:47:02.342857 ImageMagic-0.1.8/ImageMagic/
--rw-rw-rw-   0        0        0     6237 2023-05-07 00:54:28.000000 ImageMagic-0.1.8/ImageMagic/Aocr.py
--rw-rw-rw-   0        0        0    13766 2023-05-07 01:13:22.000000 ImageMagic-0.1.8/ImageMagic/Image.py
--rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.1.8/ImageMagic/_Atesseract.py
--rw-rw-rw-   0        0        0      260 2023-05-04 12:55:21.000000 ImageMagic-0.1.8/ImageMagic/__init__.py
--rw-rw-rw-   0        0        0       85 2023-05-07 01:46:11.000000 ImageMagic-0.1.8/ImageMagic/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-07 01:47:02.358485 ImageMagic-0.1.8/ImageMagic.egg-info/
--rw-rw-rw-   0        0        0      500 2023-05-07 01:47:02.000000 ImageMagic-0.1.8/ImageMagic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-05-07 01:47:02.000000 ImageMagic-0.1.8/ImageMagic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 01:47:02.000000 ImageMagic-0.1.8/ImageMagic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-07 01:47:02.000000 ImageMagic-0.1.8/ImageMagic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-07 01:47:02.000000 ImageMagic-0.1.8/ImageMagic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      500 2023-05-07 01:47:02.358485 ImageMagic-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1231 2023-05-06 11:02:24.000000 ImageMagic-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-07 01:47:02.358485 ImageMagic-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      792 2023-05-07 01:41:00.000000 ImageMagic-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 01:47:02.358485 ImageMagic-0.1.8/test/
--rw-rw-rw-   0        0        0       26 2023-05-06 05:17:57.000000 ImageMagic-0.1.8/test/__init__.py
--rw-rw-rw-   0        0        0     1286 2023-05-07 01:21:31.000000 ImageMagic-0.1.8/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-07 05:16:23.429719 ImageMagic-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-05-07 05:16:23.398468 ImageMagic-0.1.9/ImageMagic/
+-rw-rw-rw-   0        0        0     6237 2023-05-07 00:54:28.000000 ImageMagic-0.1.9/ImageMagic/Aocr.py
+-rw-rw-rw-   0        0        0    15057 2023-05-07 05:10:59.000000 ImageMagic-0.1.9/ImageMagic/Image.py
+-rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.1.9/ImageMagic/_Atesseract.py
+-rw-rw-rw-   0        0        0      260 2023-05-04 12:55:21.000000 ImageMagic-0.1.9/ImageMagic/__init__.py
+-rw-rw-rw-   0        0        0       85 2023-05-07 05:12:37.000000 ImageMagic-0.1.9/ImageMagic/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-07 05:16:23.414092 ImageMagic-0.1.9/ImageMagic.egg-info/
+-rw-rw-rw-   0        0        0      500 2023-05-07 05:16:23.000000 ImageMagic-0.1.9/ImageMagic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-05-07 05:16:23.000000 ImageMagic-0.1.9/ImageMagic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 05:16:23.000000 ImageMagic-0.1.9/ImageMagic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-07 05:16:23.000000 ImageMagic-0.1.9/ImageMagic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-07 05:16:23.000000 ImageMagic-0.1.9/ImageMagic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      500 2023-05-07 05:16:23.429719 ImageMagic-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1231 2023-05-06 11:02:24.000000 ImageMagic-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 05:16:23.429719 ImageMagic-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-05-07 01:41:00.000000 ImageMagic-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 05:16:23.414092 ImageMagic-0.1.9/test/
+-rw-rw-rw-   0        0        0       26 2023-05-06 05:17:57.000000 ImageMagic-0.1.9/test/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-05-07 05:15:55.000000 ImageMagic-0.1.9/test/test.py
```

### Comparing `ImageMagic-0.1.8/ImageMagic/Aocr.py` & `ImageMagic-0.1.9/ImageMagic/Aocr.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.8/ImageMagic/Image.py` & `ImageMagic-0.1.9/ImageMagic/Image.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import hashlib
 import hmac
 import base64
 import time
 import os
 from loguru import logger
 import shutil
-import struct
+import numpy as np
 
 #They are used in the Audio class
 RESULT = None
 ANSWER = None
 
 
 def word_to_image(text, path, fontPath=r'C:\Windows\Fonts\STXIHEI.TTF', LinesWords=14, fontsize=45, type='png', color=(255, 255, 255)):
-
+    #文字转图片
     """
     Let the text you enter appear on an image,
     Your text word count should preferably be greater than or equal to 10!（In cases where you use the default font size）
     Args:
         text: Your text content
         path: The path where the picture is saved,You will also need to write the full name of your file (including the suffix!).
         fontPath: Font path
@@ -60,15 +60,15 @@
     except FileNotFoundError as error:
         logger.error(f'Please check your file path, you need to enter a full path, including your file name (even the suffix!).\nerror:{error}')
 
     os.remove('temp.txt')
 
 
 def audio_to_image(appid,key,audioPath,imagePath,fontPath=r'C:\Windows\Fonts\STXIHEI.TTF'):
-
+    #音频转图片
     """
     Supports WAV, FLAC, OPUS, M4A, MP3 format audio files,
     Convert audio content into pictures, do you find this method a bit strange?
     Yes, it is the stitching of two other methods! You can use it according to your interests.
     Args:
         appid: your appid from https://console.xfyun.cn/services/lfasr
         key: your secretKey from https://console.xfyun.cn/services/lfasr
@@ -86,15 +86,15 @@
     try:
         word_to_image(get_text,imagePath,fontPath)
     except FileNotFoundError as error:
         logger.error(f'Please check your file path, you need to enter a full path, including your file name (even the suffix!).\nerror:{error}')
 
 
 def convert(originFilePath,format,savePath,mode=None):
-
+    #图片格式转换
     """
     Picture format conversion, the current version supports all possible conversions between "L", "RGB" and "CMYK".
     Args:
         originFilePath: Path to the original file (full path,Includes suffix)
         format: Target format (the format you want)
         savePath: The converted save path, including the file name and even the suffix
         mode: Conversion mode
@@ -104,15 +104,15 @@
     """
 
     image = PILImage.open(originFilePath).convert(mode=mode)
     image.save(savePath,format=format)
 
 
 def equal_scale_image(filePath,savePath,multiple=1):
-
+    #图片等比例变化
     """
     Change your image in equal proportions
     Args:
         filePath: Original file path
         savePath: The path to the save
         multiple: The multiplier of the change
 
@@ -124,15 +124,15 @@
     width = img.size[0]
     height = img.size[1]
     img = img.resize((int(width * multiple), int(height * multiple)), PILImage.Resampling.LANCZOS)
     img.save(savePath)
 
 
 def customize_image(filePath,savePath,new_width=None,new_height=None):
-
+    #自定义图片分辨率
     """
     Custom image size (if no input is used, the original parameter will be used)
     Args:
         filePath: Original file path
         savePath: The path to the save
         new_width: width
         new_height: height
@@ -151,66 +151,105 @@
     if new_width is None and new_height is None:
         img = img.resize((int(width),int(height)),PILImage.Resampling.LANCZOS)
     else:
         img = img.resize((int(new_width),int(new_height)),PILImage.Resampling.LANCZOS)
     img.save(savePath)
 
 
-def get_image_hash(image_path):
-
+def lbp_image_hash(imagePath):
+    #哈希局部二值算法
     """
-    Gets the hash value of the image
+    The local binary algorithm calculates the hash value.
     Args:
-        image_path: Image path
+        imagePath: Image path
 
     Returns:
         The hash of the image (consisting of 0 and 1)
     """
 
-    img = PILImage.open(image_path)
-    w = img.size[0]
-    h = img.size[1]
-    img.close() #关闭img，释放资源
-
-    # 打开图像文件
-    with open(image_path, "rb") as f:
-        data = f.read()
-    # 解析图像头信息
-    width, height = struct.unpack('>II', data[16:24])
-    pixel_data = data[24:]
-
-    # 调整图像大小
-    if w > width or h > height:
-        raise ValueError("Invalid size")
-    xstep = width // w
-    ystep = height // h
-
-    # 计算像素均值并生成哈希值
-    pixels = []
-    for y in range(h):
-        for x in range(w):
-            pixel = pixel_data[((y * ystep) * width + (x * xstep)) * 3:((y * ystep) * width + (x * xstep)) * 3 + 3]
-            pixels.append(sum(pixel) / 3)
-
-    # 计算平均像素值
-    avg_pixel = sum(pixels) / len(pixels)
+    # 打开图像并转换为灰度图像
+    with PILImage.open(imagePath) as img:
+        gray_img = img.convert('L')
+
+    # 缩放图像为8x8大小
+    small_img = gray_img.resize((8, 8), resample=PILImage.Resampling.BILINEAR)
+
+    # 计算每个像素的平均值
+    pixels = list(small_img.getdata())
+    avg_pixel = sum(pixels) // 64
 
-    # 生成哈希值
-    hash_value = ""
+    # 将像素值转换为二进制哈希值
+    binary_hash = ''
     for pixel in pixels:
-        if pixel > avg_pixel:
-            hash_value += "1"
+        if pixel >= avg_pixel:
+            binary_hash += '1'
         else:
-            hash_value += "0"
+            binary_hash += '0'
+
+    return binary_hash
+
+
+def p_image_hash(imagePath):
+    #哈希感知算法
+    """
+    Use Perceptual Hash computation to get the image hash.
+    Args:
+        imagePath: image path
+
+    Returns:
+        Image hash value.
+    """
+
+    image = PILImage.open(imagePath).convert('L')
+    # 缩放图像为8x8的尺寸
+    image = image.resize((8, 8), PILImage.Resampling.LANCZOS)
+    # 将图像转换为numpy数组
+    pixels = np.array(image.getdata()).reshape((8, 8))
+    # 计算像素平均值
+    avg_pixel = pixels.mean()
+    # 将像素值与平均值进行比较，生成64位哈希值
+    hash_value = 0
+    for row in range(8):
+        for col in range(8):
+            if pixels[row, col] > avg_pixel:
+                hash_value |= 1 << (row * 8 + col)
     return hash_value
 
-def remove_same_images(directoryPath):
 
+def average_image_hash(imagePath):
+    #哈希平均算法
     """
-    Delete the same images in the directory, and calculate the hash value of the images to identify whether the pictures are the same.
+    The image hash is obtained using the average hash algorithm.
+
+    Args:
+        imagePath: image path.
+    Returns:
+        image hash.
+    """
+
+    hash_size = 8
+    # 加载图像并调整大小
+    with PILImage.open(imagePath) as image:
+        image = image.convert('L').resize((hash_size, hash_size), PILImage.Resampling.LANCZOS)
+
+    # 计算平均灰度值
+    pixels = list(image.getdata())
+    avg = sum(pixels) / len(pixels)
+
+    # 将像素值与平均值进行比较并生成哈希值
+    bits = "".join(['1' if pixel > avg else '0' for pixel in pixels])
+    hash_value = int(bits, 2)
+
+    return hash_value
+
+
+def remove_same_images(directoryPath):
+    #移除相同图片
+    """
+    Delete the same image in the directory and keep only one picture (using local binary value algorithm).
     Supports jpg, png, bmp, webp, jpeg, gif, svg, tif, tiff.
     Args:
         directoryPath: The file directory path
 
     Returns:
         None
     """
@@ -221,28 +260,28 @@
     # 遍历目录中的所有图像
     for filename in os.listdir(directoryPath):
         if not filename.endswith((".jpg", ".png", ".bmp",".webp",".jpeg",".gif","svg","tif","tiff")):
             continue
         filepath = os.path.join(directoryPath, filename)
 
         # 计算图像哈希值
-        hash_value = get_image_hash(filepath)
+        hash_value = lbp_image_hash(filepath)
 
         # 如果哈希值已经存在，则删除图像
         if hash_value in hashes:
             logger.info(f"Removing duplicate image: {filepath}")
             os.remove(filepath)
         else:
             hashes[hash_value] = filepath
 
     logger.info("Done removing duplicate images.")
 
 
 def categorize_image(filePath):
-
+    #图片分类
     """
     Categorize your images, support jpg, jpeg, png, webp, bmp, tif, tiff, gif, svg, wmf
     Args:
         filePath: Your folder path
 
     Returns:
         None
@@ -304,15 +343,15 @@
                 os.makedirs(f'{filePath}/another')
             except FileExistsError:
                 pass
             shutil.copy(os.path.join(filePath,filename),f'{filePath}/another')
 
 
 class Audio:
-
+    #音频类
     """
     You need to pass in the appid, secret-key, and path to the audio file
     """
 
     def __init__(self,appid,key,upload_file_path):
 
         """
@@ -370,15 +409,15 @@
         response = requests.post(self.__uploadlinks,params=data,headers=self.__header,data=documents)
         result = json.loads(response.text)
         #print(result)
         return result
 
 
     def voice_to_word(self):
-
+        #音频转文字
         """
         Audio to text,Supports WAV, FLAC, OPUS, M4A, MP3 format audio files,
         If you call this method, you need to pass parameters in the class
         Returns:
             A list of results
         """
```

### Comparing `ImageMagic-0.1.8/ImageMagic/_Atesseract.py` & `ImageMagic-0.1.9/ImageMagic/_Atesseract.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.8/LICENSE` & `ImageMagic-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.8/README.md` & `ImageMagic-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.8/setup.py` & `ImageMagic-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.8/test/test.py` & `ImageMagic-0.1.9/test/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,13 +46,23 @@
 '''
 
 '''
 lang = Aocr.check_languages()
 print(lang)
 '''
 
+#Image.remove_same_images('./images')
+
 '''
-hash = Image.get_image_hash('./images/test.png')
+hash = Image.lbp_image_hash('./images/test.png')
 print(hash)
 '''
 
-#Image.remove_same_images('./images')
+'''
+hash = Image.p_image_hash('./images/test.png')
+print(hash)
+'''
+
+'''
+hash = Image.average_image_hash('./images/test.png')
+print(hash)
+'''
```

