# Comparing `tmp/korcen-0.3.4.tar.gz` & `tmp/korcen-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "korcen-0.3.4.tar", last modified: Fri May  5 06:12:15 2023, max compression
+gzip compressed data, was "korcen-0.3.5.tar", last modified: Sun May  7 13:40:07 2023, max compression
```

## Comparing `korcen-0.3.4.tar` & `korcen-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 06:12:15.202695 korcen-0.3.4/
--rw-rw-rw-   0        0        0      402 2023-05-05 06:12:15.200693 korcen-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-05-08 14:04:20.000000 korcen-0.3.4/README
-drwxrwxrwx   0        0        0        0 2023-05-05 06:12:15.176698 korcen-0.3.4/korcen/
--rw-rw-rw-   0        0        0      407 2023-02-08 16:18:28.000000 korcen-0.3.4/korcen/__init__.py
--rw-rw-rw-   0        0        0   149059 2023-05-05 05:58:09.000000 korcen-0.3.4/korcen/korcen.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:12:15.197696 korcen-0.3.4/korcen.egg-info/
--rw-rw-rw-   0        0        0      402 2023-05-05 06:12:14.000000 korcen-0.3.4/korcen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-05 06:12:15.000000 korcen-0.3.4/korcen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 06:12:14.000000 korcen-0.3.4/korcen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-05 06:12:14.000000 korcen-0.3.4/korcen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 06:12:14.000000 korcen-0.3.4/korcen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 06:12:15.202695 korcen-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-05-05 06:12:05.000000 korcen-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:40:07.823063 korcen-0.3.5/
+-rw-rw-rw-   0        0        0      402 2023-05-07 13:40:07.822064 korcen-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-05-08 14:04:20.000000 korcen-0.3.5/README
+drwxrwxrwx   0        0        0        0 2023-05-07 13:40:07.796871 korcen-0.3.5/korcen/
+-rw-rw-rw-   0        0        0      407 2023-02-08 16:18:28.000000 korcen-0.3.5/korcen/__init__.py
+-rw-rw-rw-   0        0        0   148973 2023-05-07 13:39:53.000000 korcen-0.3.5/korcen/korcen.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:40:07.818066 korcen-0.3.5/korcen.egg-info/
+-rw-rw-rw-   0        0        0      402 2023-05-07 13:40:07.000000 korcen-0.3.5/korcen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-05-07 13:40:07.000000 korcen-0.3.5/korcen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 13:40:07.000000 korcen-0.3.5/korcen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-07 13:40:07.000000 korcen-0.3.5/korcen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 13:40:07.000000 korcen-0.3.5/korcen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 13:40:07.823063 korcen-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-05-07 13:40:01.000000 korcen-0.3.5/setup.py
```

### Comparing `korcen-0.3.4/korcen/korcen.py` & `korcen-0.3.5/korcen/korcen.py`

 * *Files 0% similar despite different names*

```diff
@@ -806,15 +806,14 @@
     text = re.sub('[^a-z]', '', text)
     sex = ["sex", "s스", "x스", "se스", "se스", "s스",
             "ㅅㅅ", "s하고e싶다x", "ㅅㅔㅅㄱ", "이=스", "ㅇl=스"]
     for i in sex:
         if i in text:
             return True
     text = re.sub(r'\^', 'ㅅ', newtext)
-    text = re.sub('sex', '섹스', text)
     text = re.sub('엑', '', text)
     text = re.sub('0ㅑ', '야', text)
     text = re.sub("[^ㄱ-힣]", "", text)
     sex = ["ㅅㅔㄱ스", "섹ㅅ", "ㅅ스", "세ㄱㅅ", "ㅅㅔㄱㅅ"]
     for i in sex:
         if i in text:
             return True
@@ -1950,15 +1949,14 @@
     text = re.sub('[^a-z]', '', text)
     sex = ["sex", "s스", "x스", "se스", "se스", "s스",
             "ㅅㅅ", "s하고e싶다x", "ㅅㅔㅅㄱ", "이=스", "ㅇl=스"]
     for i in sex:
         if i in text:
             return True
     text = re.sub(r'\^', 'ㅅ', newtext)
-    text = re.sub('sex', '섹스', text)
     text = re.sub('엑', '', text)
     text = re.sub('0ㅑ', '야', text)
     text = re.sub("[^ㄱ-힣]", "", text)
     sex = ["ㅅㅔㄱ스", "섹ㅅ", "ㅅ스", "세ㄱㅅ", "ㅅㅔㄱㅅ"]
     for i in sex:
         if i in text:
             return True
@@ -2505,8 +2503,8 @@
 #   | | (_| | | | | (_| | |_
 #   |_|\__,_|_| |_|\__,_|\__|
 
 if __name__ == "__main__":
     cache_size = 2
     while True:
         text = input()
-        print(check(text, 1))
+        print(check(text, 1))
```

### Comparing `korcen-0.3.4/setup.py` & `korcen-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="korcen",  # Replace with your own PyPI username(id)
-    version="0.3.4",
+    version="0.3.5",
     author="Tanat",
     author_email="shrbwjd05@naver.com",
     description="한국어 비속어 검열",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KR-korcen/korcen",
     packages=setuptools.find_packages(),
```

