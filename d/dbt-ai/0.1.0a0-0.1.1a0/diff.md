# Comparing `tmp/dbt-ai-0.1.0a0.tar.gz` & `tmp/dbt-ai-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-ai-0.1.0a0.tar", last modified: Sun May  7 12:02:55 2023, max compression
+gzip compressed data, was "dbt-ai-0.1.1a0.tar", last modified: Sun May  7 12:24:23 2023, max compression
```

## Comparing `dbt-ai-0.1.0a0.tar` & `dbt-ai-0.1.1a0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:02:55.457895 dbt-ai-0.1.0a0/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1069 2023-05-07 00:28:17.000000 dbt-ai-0.1.0a0/LICENSE
--rw-r--r--   0 armalite  (1000) armalite  (1000)       71 2023-05-06 13:04:03.000000 dbt-ai-0.1.0a0/MANIFEST.in
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3429 2023-05-07 12:02:55.457895 dbt-ai-0.1.0a0/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3227 2023-05-07 12:02:14.000000 dbt-ai-0.1.0a0/README.md
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:02:55.457895 dbt-ai-0.1.0a0/dbt_ai/
--rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.1.0a0/dbt_ai/__init__.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     4420 2023-05-07 11:42:35.000000 dbt-ai-0.1.0a0/dbt_ai/ai.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     7893 2023-05-07 11:51:30.000000 dbt-ai-0.1.0a0/dbt_ai/dbt.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)      565 2023-05-07 06:43:19.000000 dbt-ai-0.1.0a0/dbt_ai/helper.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1699 2023-05-07 12:01:28.000000 dbt-ai-0.1.0a0/dbt_ai/main.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.1.0a0/dbt_ai/py.typed
--rw-r--r--   0 armalite  (1000) armalite  (1000)      811 2023-05-06 13:18:50.000000 dbt-ai-0.1.0a0/dbt_ai/report.py
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:02:55.457895 dbt-ai-0.1.0a0/dbt_ai/templates/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3094 2023-05-06 13:45:28.000000 dbt-ai-0.1.0a0/dbt_ai/templates/report_template.html
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:02:55.457895 dbt-ai-0.1.0a0/dbt_ai.egg-info/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3429 2023-05-07 12:02:55.000000 dbt-ai-0.1.0a0/dbt_ai.egg-info/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)      384 2023-05-07 12:02:55.000000 dbt-ai-0.1.0a0/dbt_ai.egg-info/SOURCES.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-07 12:02:55.000000 dbt-ai-0.1.0a0/dbt_ai.egg-info/dependency_links.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       44 2023-05-07 12:02:55.000000 dbt-ai-0.1.0a0/dbt_ai.egg-info/entry_points.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)      193 2023-05-07 12:02:55.000000 dbt-ai-0.1.0a0/dbt_ai.egg-info/requires.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-07 12:02:55.000000 dbt-ai-0.1.0a0/dbt_ai.egg-info/top_level.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1625 2023-05-07 12:02:29.000000 dbt-ai-0.1.0a0/pyproject.toml
--rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-07 12:02:55.457895 dbt-ai-0.1.0a0/setup.cfg
--rw-r--r--   0 armalite  (1000) armalite  (1000)      144 2023-05-06 13:15:40.000000 dbt-ai-0.1.0a0/setup.py
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:24:23.267895 dbt-ai-0.1.1a0/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1069 2023-05-07 00:28:17.000000 dbt-ai-0.1.1a0/LICENSE
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       71 2023-05-06 13:04:03.000000 dbt-ai-0.1.1a0/MANIFEST.in
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     3429 2023-05-07 12:24:23.267895 dbt-ai-0.1.1a0/PKG-INFO
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     3227 2023-05-07 12:24:03.000000 dbt-ai-0.1.1a0/README.md
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:24:23.267895 dbt-ai-0.1.1a0/dbt_ai/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.1.1a0/dbt_ai/__init__.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     4413 2023-05-07 12:22:42.000000 dbt-ai-0.1.1a0/dbt_ai/ai.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     7850 2023-05-07 12:04:25.000000 dbt-ai-0.1.1a0/dbt_ai/dbt.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      565 2023-05-07 06:43:19.000000 dbt-ai-0.1.1a0/dbt_ai/helper.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1698 2023-05-07 12:04:25.000000 dbt-ai-0.1.1a0/dbt_ai/main.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.1.1a0/dbt_ai/py.typed
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      811 2023-05-06 13:18:50.000000 dbt-ai-0.1.1a0/dbt_ai/report.py
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:24:23.267895 dbt-ai-0.1.1a0/dbt_ai/templates/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     3094 2023-05-06 13:45:28.000000 dbt-ai-0.1.1a0/dbt_ai/templates/report_template.html
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:24:23.267895 dbt-ai-0.1.1a0/dbt_ai.egg-info/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     3429 2023-05-07 12:24:23.000000 dbt-ai-0.1.1a0/dbt_ai.egg-info/PKG-INFO
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      384 2023-05-07 12:24:23.000000 dbt-ai-0.1.1a0/dbt_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-07 12:24:23.000000 dbt-ai-0.1.1a0/dbt_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       44 2023-05-07 12:24:23.000000 dbt-ai-0.1.1a0/dbt_ai.egg-info/entry_points.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      193 2023-05-07 12:24:23.000000 dbt-ai-0.1.1a0/dbt_ai.egg-info/requires.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-07 12:24:23.000000 dbt-ai-0.1.1a0/dbt_ai.egg-info/top_level.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1625 2023-05-07 12:24:09.000000 dbt-ai-0.1.1a0/pyproject.toml
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-07 12:24:23.267895 dbt-ai-0.1.1a0/setup.cfg
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      144 2023-05-06 13:15:40.000000 dbt-ai-0.1.1a0/setup.py
```

### Comparing `dbt-ai-0.1.0a0/LICENSE` & `dbt-ai-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.0a0/PKG-INFO` & `dbt-ai-0.1.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.1.0a0
+Version: 0.1.1a0
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
-pip install dbt-ai==0.1.0a0
+pip install dbt-ai==0.1.1a0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key.
```

### Comparing `dbt-ai-0.1.0a0/README.md` & `dbt-ai-0.1.1a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  - Lists dbt models that are missing associated metadata e.g. in a `schema.yml` file or equivalent
  - Use AI to generate DBT models for you based on a prompt
  - DBT model lineage description is listed in the terminal (more features coming soon)
 
 ## Installation
 You can install the application here
 ```bash
-pip install dbt-ai==0.1.0a0
+pip install dbt-ai==0.1.1a0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key.
```

### Comparing `dbt-ai-0.1.0a0/dbt_ai/ai.py` & `dbt-ai-0.1.1a0/dbt_ai/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,25 +61,24 @@
     # Generate response using OpenAI API
     response = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         messages=[
             {
                 "role": "system",
                 "content": "You are a helpful assistant that will write dbt models based on the provided prompt. The prompt includes useful information such as the contents of the sources.yml file. \
-             If the logic needs to be split into multiple dbt models, please delimit the contents of each model with '===', which will be used to split the data to write into separate sql files later. \
-                Do not put any explanations. Each model content should be divided with a === so that splitting by === would divide the 3 models. The first line in the split model should have a 'model_name: modelname' with the actual model name. \
-                    The following lines after the model name should be the sql content with NO codeblock syntax. The last line of that model file should be the line prior to the next === \
+                If the logic needs to be split into multiple dbt models, please delimit the contents of each model with '===', which will be used to split the data to write into separate sql files later. \
+                Do not put any explanations. Each model content should be divided with a === so that splitting by === would divide the models. The first line in the split model should have a 'model_name: modelname' with the actual model name. \
+                The following lines after the model name should be the sql content with NO codeblock syntax. The last line of that model file should be the line prior to the next === \
                 The user will likely provide enough information such as any join requirements, or aggregation requirements so use this information to correctly structure your dbt model queries.",
             },
             {"role": "user", "content": prompt_with_sources},
         ],
         max_tokens=400,
         n=1,
         stop=None,
         temperature=0,
     )
 
     # Extract the models from the response
     models = response.choices[0].message["content"].split("MODEL:")
-    #print(models)
-    return models 
-    
+    # print(models)
+    return models
```

### Comparing `dbt-ai-0.1.0a0/dbt_ai/dbt.py` & `dbt-ai-0.1.1a0/dbt_ai/dbt.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,16 @@
         self.yaml_files = find_yaml_files(dbt_project_path)
         self.api_key_available = bool(os.getenv("OPENAI_API_KEY"))
         self.sources_yml_content = self.read_sources_yml(dbt_project_path)
         if not self.api_key_available:
             print("Warning: OPENAI_API_KEY is not set. Suggestion features will be unavailable.")
 
     def read_sources_yml(self, dbt_project_path: str):
-        sources_yml_path = os.path.join(dbt_project_path, 'models', 'sources.yml')
-        with open(sources_yml_path, 'r') as f:
+        sources_yml_path = os.path.join(dbt_project_path, "models", "sources.yml")
+        with open(sources_yml_path, "r") as f:
             sources_yml_content = f.read()
         return sources_yml_content
 
     def get_model_refs(self, model_file_path: str) -> list:
         with open(model_file_path, "r") as f:
             content = f.read()
 
@@ -188,38 +188,24 @@
         )
 
         fig.show()
 
     def create_dbt_models(self, prompt: str) -> None:
         print(f"Attempting to create dbt models based on prompt")
         response = generate_models(prompt, self.sources_yml_content)
-        
+
         model_delimiter = "===\n\n"
         response_lines = response[0].split(model_delimiter)
 
         for i, model_str in enumerate(response_lines):
             if not model_str.strip():
                 continue
-                
+
             model_lines = model_str.strip().split("\n")
             model_name = model_lines[0].split(":")[-1].strip()
             model_content = "\n".join(model_lines[1:])
             model_content = model_content.replace("===", "")
 
             model_path = os.path.join(self.dbt_project_path, "models", f"{model_name}.sql")
             with open(model_path, "w") as f:
                 f.write(model_content.strip())
             print(f"Created model file: {model_path}")
-
-
-
-
-
-
-
-
-
-
-
-
-
-
```

### Comparing `dbt-ai-0.1.0a0/dbt_ai/helper.py` & `dbt-ai-0.1.1a0/dbt_ai/helper.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.0a0/dbt_ai/main.py` & `dbt-ai-0.1.1a0/dbt_ai/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,10 +42,9 @@
             print("\nAll models have associated metadata.")
     else:
         processor = DbtModelProcessor(args.dbt_project_path)
         prompt = args.create_models
         processor.create_dbt_models(prompt)
 
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `dbt-ai-0.1.0a0/dbt_ai/report.py` & `dbt-ai-0.1.1a0/dbt_ai/report.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.0a0/dbt_ai/templates/report_template.html` & `dbt-ai-0.1.1a0/dbt_ai/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.0a0/dbt_ai.egg-info/PKG-INFO` & `dbt-ai-0.1.1a0/dbt_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.1.0a0
+Version: 0.1.1a0
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
-pip install dbt-ai==0.1.0a0
+pip install dbt-ai==0.1.1a0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key.
```

### Comparing `dbt-ai-0.1.0a0/pyproject.toml` & `dbt-ai-0.1.1a0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dbt-ai"
 description = "AI powered DBT helper application"
-version = "0.1.0-alpha"
+version = "0.1.1-alpha"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "dbt-snowflake~=1.4",
     "openai~=0.27",
     "pyyaml~=6.0",
     "markdown2~=2.4",
```

