# Comparing `tmp/dbt-ai-0.1.2a0.tar.gz` & `tmp/dbt-ai-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-ai-0.1.2a0.tar", last modified: Sun May  7 12:31:04 2023, max compression
+gzip compressed data, was "dbt-ai-0.1.3a0.tar", last modified: Sun May  7 12:33:19 2023, max compression
```

## Comparing `dbt-ai-0.1.2a0.tar` & `dbt-ai-0.1.3a0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:31:04.097895 dbt-ai-0.1.2a0/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1069 2023-05-07 00:28:17.000000 dbt-ai-0.1.2a0/LICENSE
--rw-r--r--   0 armalite  (1000) armalite  (1000)       71 2023-05-06 13:04:03.000000 dbt-ai-0.1.2a0/MANIFEST.in
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3428 2023-05-07 12:31:04.097895 dbt-ai-0.1.2a0/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3226 2023-05-07 12:28:55.000000 dbt-ai-0.1.2a0/README.md
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:31:04.097895 dbt-ai-0.1.2a0/dbt_ai/
--rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.1.2a0/dbt_ai/__init__.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     4413 2023-05-07 12:22:42.000000 dbt-ai-0.1.2a0/dbt_ai/ai.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     8111 2023-05-07 12:28:33.000000 dbt-ai-0.1.2a0/dbt_ai/dbt.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)      565 2023-05-07 06:43:19.000000 dbt-ai-0.1.2a0/dbt_ai/helper.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1698 2023-05-07 12:04:25.000000 dbt-ai-0.1.2a0/dbt_ai/main.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.1.2a0/dbt_ai/py.typed
--rw-r--r--   0 armalite  (1000) armalite  (1000)      811 2023-05-06 13:18:50.000000 dbt-ai-0.1.2a0/dbt_ai/report.py
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:31:04.097895 dbt-ai-0.1.2a0/dbt_ai/templates/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3094 2023-05-06 13:45:28.000000 dbt-ai-0.1.2a0/dbt_ai/templates/report_template.html
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:31:04.097895 dbt-ai-0.1.2a0/dbt_ai.egg-info/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3428 2023-05-07 12:31:04.000000 dbt-ai-0.1.2a0/dbt_ai.egg-info/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)      384 2023-05-07 12:31:04.000000 dbt-ai-0.1.2a0/dbt_ai.egg-info/SOURCES.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-07 12:31:04.000000 dbt-ai-0.1.2a0/dbt_ai.egg-info/dependency_links.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       44 2023-05-07 12:31:04.000000 dbt-ai-0.1.2a0/dbt_ai.egg-info/entry_points.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)      193 2023-05-07 12:31:04.000000 dbt-ai-0.1.2a0/dbt_ai.egg-info/requires.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-07 12:31:04.000000 dbt-ai-0.1.2a0/dbt_ai.egg-info/top_level.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1625 2023-05-07 12:28:59.000000 dbt-ai-0.1.2a0/pyproject.toml
--rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-07 12:31:04.097895 dbt-ai-0.1.2a0/setup.cfg
--rw-r--r--   0 armalite  (1000) armalite  (1000)      144 2023-05-06 13:15:40.000000 dbt-ai-0.1.2a0/setup.py
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:33:19.557895 dbt-ai-0.1.3a0/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1069 2023-05-07 00:28:17.000000 dbt-ai-0.1.3a0/LICENSE
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       71 2023-05-06 13:04:03.000000 dbt-ai-0.1.3a0/MANIFEST.in
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     3428 2023-05-07 12:33:19.557895 dbt-ai-0.1.3a0/PKG-INFO
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     3226 2023-05-07 12:32:37.000000 dbt-ai-0.1.3a0/README.md
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:33:19.557895 dbt-ai-0.1.3a0/dbt_ai/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.1.3a0/dbt_ai/__init__.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     4413 2023-05-07 12:22:42.000000 dbt-ai-0.1.3a0/dbt_ai/ai.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     8097 2023-05-07 12:33:03.000000 dbt-ai-0.1.3a0/dbt_ai/dbt.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      565 2023-05-07 06:43:19.000000 dbt-ai-0.1.3a0/dbt_ai/helper.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1698 2023-05-07 12:04:25.000000 dbt-ai-0.1.3a0/dbt_ai/main.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.1.3a0/dbt_ai/py.typed
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      811 2023-05-06 13:18:50.000000 dbt-ai-0.1.3a0/dbt_ai/report.py
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:33:19.557895 dbt-ai-0.1.3a0/dbt_ai/templates/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     3094 2023-05-06 13:45:28.000000 dbt-ai-0.1.3a0/dbt_ai/templates/report_template.html
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:33:19.557895 dbt-ai-0.1.3a0/dbt_ai.egg-info/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     3428 2023-05-07 12:33:19.000000 dbt-ai-0.1.3a0/dbt_ai.egg-info/PKG-INFO
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      384 2023-05-07 12:33:19.000000 dbt-ai-0.1.3a0/dbt_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-07 12:33:19.000000 dbt-ai-0.1.3a0/dbt_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       44 2023-05-07 12:33:19.000000 dbt-ai-0.1.3a0/dbt_ai.egg-info/entry_points.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      193 2023-05-07 12:33:19.000000 dbt-ai-0.1.3a0/dbt_ai.egg-info/requires.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-07 12:33:19.000000 dbt-ai-0.1.3a0/dbt_ai.egg-info/top_level.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1625 2023-05-07 12:32:39.000000 dbt-ai-0.1.3a0/pyproject.toml
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-07 12:33:19.557895 dbt-ai-0.1.3a0/setup.cfg
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      144 2023-05-06 13:15:40.000000 dbt-ai-0.1.3a0/setup.py
```

### Comparing `dbt-ai-0.1.2a0/LICENSE` & `dbt-ai-0.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.2a0/PKG-INFO` & `dbt-ai-0.1.3a0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-Metadata-Version: 2.1
-Name: dbt-ai
-Version: 0.1.2a0
-Summary: AI powered DBT helper application
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # DBT AI
 
 This application provides AI generated recommendations on how to improve your [DBT](https://www.getdbt.com/) models.
 
 ## Features
  - Scans all dbt models and generates a report containing recommendations for each model
  - Lists dbt models that are missing associated metadata e.g. in a `schema.yml` file or equivalent
  - Use AI to generate DBT models for you based on a prompt
  - DBT model lineage description is listed in the terminal (more features coming soon)
 
 ## Installation
 You can install the application here
 ```bash
-pip install dbt-ai==0.1.2a0
+pip install dbt-ai==0.1.3a0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key.
```

### Comparing `dbt-ai-0.1.2a0/README.md` & `dbt-ai-0.1.3a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,30 @@
+Metadata-Version: 2.1
+Name: dbt-ai
+Version: 0.1.3a0
+Summary: AI powered DBT helper application
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # DBT AI
 
 This application provides AI generated recommendations on how to improve your [DBT](https://www.getdbt.com/) models.
 
 ## Features
  - Scans all dbt models and generates a report containing recommendations for each model
  - Lists dbt models that are missing associated metadata e.g. in a `schema.yml` file or equivalent
  - Use AI to generate DBT models for you based on a prompt
  - DBT model lineage description is listed in the terminal (more features coming soon)
 
 ## Installation
 You can install the application here
 ```bash
-pip install dbt-ai==0.1.2a0
+pip install dbt-ai==0.1.3a0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key.
```

### Comparing `dbt-ai-0.1.2a0/dbt_ai/ai.py` & `dbt-ai-0.1.3a0/dbt_ai/ai.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.2a0/dbt_ai/dbt.py` & `dbt-ai-0.1.3a0/dbt_ai/dbt.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
             with open(sources_yml_path, "r") as f:
                 sources_yml_content = f.read()
         except FileNotFoundError:
             print("sources.yml not found. Proceeding with an empty sources file.")
             sources_yml_content = None
         return sources_yml_content
 
-
     def get_model_refs(self, model_file_path: str) -> list:
         with open(model_file_path, "r") as f:
             content = f.read()
 
         refs = re.findall(r"ref\(['\"]([\w\.]+)['\"]\)", content)
 
         return refs
@@ -193,15 +192,15 @@
         )
 
         fig.show()
 
     def create_dbt_models(self, prompt: str) -> None:
         print(f"Attempting to create dbt models based on prompt")
         sources_yml = self.sources_yml_content if self.sources_yml_content else ""
-        response = generate_models(prompt, self.sources_yml_content)
+        response = generate_models(prompt, sources_yml)
 
         model_delimiter = "===\n\n"
         response_lines = response[0].split(model_delimiter)
 
         for i, model_str in enumerate(response_lines):
             if not model_str.strip():
                 continue
```

### Comparing `dbt-ai-0.1.2a0/dbt_ai/helper.py` & `dbt-ai-0.1.3a0/dbt_ai/helper.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.2a0/dbt_ai/main.py` & `dbt-ai-0.1.3a0/dbt_ai/main.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.2a0/dbt_ai/report.py` & `dbt-ai-0.1.3a0/dbt_ai/report.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.2a0/dbt_ai/templates/report_template.html` & `dbt-ai-0.1.3a0/dbt_ai/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.2a0/dbt_ai.egg-info/PKG-INFO` & `dbt-ai-0.1.3a0/dbt_ai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.1.2a0
+Version: 0.1.3a0
 Summary: AI powered DBT helper application
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DBT AI
@@ -16,15 +16,15 @@
  - Lists dbt models that are missing associated metadata e.g. in a `schema.yml` file or equivalent
  - Use AI to generate DBT models for you based on a prompt
  - DBT model lineage description is listed in the terminal (more features coming soon)
 
 ## Installation
 You can install the application here
 ```bash
-pip install dbt-ai==0.1.2a0
+pip install dbt-ai==0.1.3a0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key.
```

### Comparing `dbt-ai-0.1.2a0/pyproject.toml` & `dbt-ai-0.1.3a0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dbt-ai"
 description = "AI powered DBT helper application"
-version = "0.1.2-alpha"
+version = "0.1.3-alpha"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "dbt-snowflake~=1.4",
     "openai~=0.27",
     "pyyaml~=6.0",
     "markdown2~=2.4",
```

