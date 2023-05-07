# Comparing `tmp/xpanther-1.0.5.tar.gz` & `tmp/xpanther-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpanther-1.0.5.tar", last modified: Wed Apr 26 14:43:47 2023, max compression
+gzip compressed data, was "xpanther-1.0.6.tar", last modified: Sun May  7 13:46:10 2023, max compression
```

## Comparing `xpanther-1.0.5.tar` & `xpanther-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 14:43:47.593200 xpanther-1.0.5/
--rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     5863 2023-04-26 14:43:47.593200 xpanther-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5386 2023-02-19 14:07:14.000000 xpanther-1.0.5/README.md
--rw-rw-rw-   0        0        0      633 2023-04-26 14:42:52.000000 xpanther-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 14:43:47.593200 xpanther-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 14:43:47.538584 xpanther-1.0.5/xpanther/
--rw-rw-rw-   0        0        0       79 2023-04-26 14:42:52.000000 xpanther-1.0.5/xpanther/__init__.py
--rw-rw-rw-   0        0        0    20075 2023-04-26 14:42:52.000000 xpanther-1.0.5/xpanther/main.py
--rw-rw-rw-   0        0        0     2467 2023-02-19 14:05:11.000000 xpanther-1.0.5/xpanther/main_ide.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:43:47.593200 xpanther-1.0.5/xpanther.egg-info/
--rw-rw-rw-   0        0        0     5863 2023-04-26 14:43:47.000000 xpanther-1.0.5/xpanther.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-04-26 14:43:47.000000 xpanther-1.0.5/xpanther.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 14:43:47.000000 xpanther-1.0.5/xpanther.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-26 14:43:47.000000 xpanther-1.0.5/xpanther.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-26 14:43:47.000000 xpanther-1.0.5/xpanther.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 13:46:10.819241 xpanther-1.0.6/
+-rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5854 2023-05-07 13:46:10.819241 xpanther-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5386 2023-02-19 14:07:14.000000 xpanther-1.0.6/README.md
+-rw-rw-rw-   0        0        0      624 2023-05-07 13:45:42.000000 xpanther-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 13:46:10.819241 xpanther-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 13:46:10.777985 xpanther-1.0.6/xpanther/
+-rw-rw-rw-   0        0        0       79 2023-05-07 13:19:03.000000 xpanther-1.0.6/xpanther/__init__.py
+-rw-rw-rw-   0        0        0    19992 2023-05-07 13:42:55.000000 xpanther-1.0.6/xpanther/main.py
+-rw-rw-rw-   0        0        0     2641 2023-05-07 13:40:55.000000 xpanther-1.0.6/xpanther/main_ide.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:46:10.819241 xpanther-1.0.6/xpanther.egg-info/
+-rw-rw-rw-   0        0        0     5854 2023-05-07 13:46:10.000000 xpanther-1.0.6/xpanther.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-07 13:46:10.000000 xpanther-1.0.6/xpanther.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 13:46:10.000000 xpanther-1.0.6/xpanther.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-07 13:46:10.000000 xpanther-1.0.6/xpanther.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 13:46:10.000000 xpanther-1.0.6/xpanther.egg-info/top_level.txt
```

### Comparing `xpanther-1.0.5/LICENSE` & `xpanther-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xpanther-1.0.5/PKG-INFO` & `xpanther-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.0.5
-Summary: Find unique relative xpath of any html/xml element
+Version: 1.0.6
+Summary: Find Unique Xpath of any HTML/XML element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `xpanther-1.0.5/README.md` & `xpanther-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `xpanther-1.0.5/pyproject.toml` & `xpanther-1.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xpanther"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
-description = "Find unique relative xpath of any html/xml element"
+description = "Find Unique Xpath of any HTML/XML element"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "bs4 >= 0.0.1",
     "selenium >= 4.9.0",
 ]
 classifiers = [
```

### Comparing `xpanther-1.0.5/xpanther/main.py` & `xpanther-1.0.6/xpanther/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import re
 import requests
 from itertools import combinations
 from collections import Counter
 from bs4 import BeautifulSoup
 
-# TODO # 1: FINAL --- Print the output ready in various forms for multiple platforms and languages.
-
 
 class XPanther:
     def __init__(self, DOM, xml=False, pre_formatted=False, url_input=False, child_method=True, print_output=True,
                  no_digits=False, show_all=False, speed='normal'):
         self.__dom = DOM
         self.__keys = []
         self.__formatted_html_lines = []
@@ -27,22 +25,22 @@
         self.__url_input = url_input
         self.__show_all = show_all
         self.__print_output = print_output
         self.__speed = speed
 
     def capture(self, target):
         program_return = []
-        formatted_HTML = self.__format_HTML(self.__dom)
+        formatted_HTML = self.__format_html(self.__dom)
         element_regex, attr_regex, closing_tag_regex = self.__regex_distributor(formatted_HTML)
 
-        self.__process_HTML(formatted_HTML, element_regex, attr_regex, closing_tag_regex)
+        self.__process_html(formatted_HTML, element_regex, attr_regex, closing_tag_regex)
 
         if type(target) == str and re.match(element_regex, target):
             list_of_occurrences = []
-            formatted_element = self.__format_HTML(target, format_override=True)
+            formatted_element = self.__format_html(target, format_override=True)
 
             for line in formatted_element:
                 if re.match(closing_tag_regex, line.lstrip()):
                     pass
                 else:
                     if self.__xml:
                         if not self.__pre_formatted:
@@ -122,22 +120,22 @@
                 return False
         else:
             self.__print('Invalid Input or not proper element!')
             return False
 
     def __controller(self, target_elements):
         if unique_elements := self.__find_unique_elements(target_elements):
-            if xpath := self.__find_XPATH(unique_elements, target_elements):
+            if xpath := self.__find_xpath(unique_elements, target_elements):
                 return xpath
         else:
             cut_down_elements = self.__select_attribute_pool_size(target_elements)
             target_elements = cut_down_elements
             if all_combinations := self.__find_combinations(target_elements):
                 if indicators := self.__find_unique_combinations(all_combinations[0], all_combinations[1]):
-                    if xpath := self.__find_XPATH(indicators, target_elements):
+                    if xpath := self.__find_xpath(indicators, target_elements):
                         return xpath
                 else:
                     if not self.__child_method_ban:
                         if self.__child_method:
                             if result := self.__child_control(self.__target):
                                 return result
                             else:
@@ -148,24 +146,24 @@
                         if not self.__child_method:
                             return self.__checking_parent(target_elements)
                     else:
                         return self.__checking_parent(target_elements)
             else:
                 return False
 
-    def __format_HTML(self, input, format_override=False):
+    def __format_html(self, input_html, format_override=False):
         parser = 'html.parser'
         if self.__xml:
             parser = 'xml'
-        HTML = input
+        HTML = input_html
         if not format_override:
             if not self.__url_input:
-                if '<' and '>' not in input:
+                if '<' and '>' not in input_html:
                     try:
-                        with open(input, 'r', encoding='utf-8', errors='ignore') as textfile:
+                        with open(input_html, 'r', encoding='utf-8', errors='ignore') as textfile:
                             HTML = textfile.read()
                     except FileNotFoundError:
                         self.__print('File Not Found !')
                     except OSError as o:
                         self.__print(o)
             else:
                 HTML = requests.get(self.__dom).text
@@ -176,15 +174,15 @@
             except Exception as e:
                 self.__print(e)
             if self.__xml:
                 formatted_HTML.pop(0)
 
         return formatted_HTML
 
-    def __process_HTML(self, formatted_HTML, element_regex, attr_regex, closing_tag_regex):
+    def __process_html(self, formatted_HTML, element_regex, attr_regex, closing_tag_regex):
         index = 0
         for line in formatted_HTML:
             if re.match(closing_tag_regex, line.lstrip()):
                 pass
             else:
                 self.__formatted_html_lines.append(line.lstrip())
                 elements = re.findall(element_regex, line)
@@ -284,15 +282,15 @@
             speed = 15
         elif type(self.__speed) == int and int(self.__speed) <= 50:
             speed = self.__speed
         else:
             speed = 25
         return [elements[0][:speed], elements[1], elements[2]]
 
-    def __format_XPATH(self, unique_elements, all_elements):
+    def __format_xpath(self, unique_elements, all_elements):
         combination = False
         if self.__identifier_method == 'combination':
             combination = True
 
         child_index_xpath = ''
         parent_hierarchy = ''
         tag = all_elements[0][0]
@@ -349,16 +347,16 @@
                 if not self.__show_all:
                     return final_Xpath
             return True
         else:
             self.__print(f'Element\'s --{all_elements[0]}-- format is not normal !')
             return False
 
-    def __find_XPATH(self, unique_elements, target_elements):
-        if result := self.__format_XPATH(unique_elements, target_elements):
+    def __find_xpath(self, unique_elements, target_elements):
+        if result := self.__format_xpath(unique_elements, target_elements):
             self.__gen = []
             self.__children_index = []
             return result
 
     def __find_parent(self, element):
         target_index = element[2]
         child_index = 0
```

### Comparing `xpanther-1.0.5/xpanther/main_ide.py` & `xpanther-1.0.6/xpanther/main_ide.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # TODO # 2: iFrames are not supported
 # TODO # 3: This should be done with GUI.
 
 
 class XPantherIDE:
     def __init__(self, page_url):
         self.__driver = webdriver.Chrome()
-        self.__element_list = []
         self.__page_url = page_url
 
     def start(self):
         program_return = []
         self.__driver.get(self.__page_url)
         event_js = '''
         var array_events = []
@@ -27,35 +26,40 @@
         var registerUrl = (e) => {
             array_events.push(document.documentElement.outerHTML)
             }
             
         getElementHtml = document.addEventListener("click", registerOuterHtml, true)
         getDOMHtml = document.addEventListener("click", registerUrl, true)
         '''
-        return_js = '''return window.array_events'''
+        return_js = '''
+        function get_value() {
+            var result = window.array_events;
+            window.array_events = [];
+            return result;
+            }
+        return get_value()'''
         self.__driver.set_script_timeout(10000)
         self.__driver.execute_script(event_js)
+        current_url = self.__driver.current_url
         try:
-            for _ in range(1800):
-                if array_events := self.__driver.execute_script(return_js):
-                    if array_events[-2:] not in program_return:
-                        program_return.append(array_events[-2:])
-                else:
-                    try:
-                        WebDriverWait(self.__driver, 0.1).until(
-                            lambda driver: self.__driver.current_url != self.__page_url)
-                    except TimeoutException:
-                        pass
-                    else:
-                        self.__page_url = self.__driver.current_url
+            for _ in range(1000):
+                try:
+                    if (new_url := self.__driver.current_url) != current_url:
+                        current_url = new_url
                         self.__driver.execute_script(event_js)
+                    return_value = WebDriverWait(self.__driver, 1).until(lambda driver: self.__driver.execute_script(return_js))
+                    program_return += [[value, html] for value, html in zip(return_value[::2], return_value[1::2]) if value not in (element[0] for element in program_return)]
+                except TimeoutException:
+                    pass
         except WebDriverException:
             pass
         finally:
             index = 1
             if program_return:
                 for click in program_return:
                     print("\033[91m {}\033[00m".format(f'\n#{index} CLICK SELECTION:'))
                     XPanther(click[1]).capture(click[0])
                     index += 1
+                return True
             else:
                 print('No click was registered!')
+                return False
```

### Comparing `xpanther-1.0.5/xpanther.egg-info/PKG-INFO` & `xpanther-1.0.6/xpanther.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.0.5
-Summary: Find unique relative xpath of any html/xml element
+Version: 1.0.6
+Summary: Find Unique Xpath of any HTML/XML element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

