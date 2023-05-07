# Comparing `tmp/dbt-ai-0.0.8a0.tar.gz` & `tmp/dbt-ai-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-ai-0.0.8a0.tar", last modified: Sat May  6 13:05:57 2023, max compression
+gzip compressed data, was "dbt-ai-0.0.9a0.tar", last modified: Sat May  6 13:35:27 2023, max compression
```

## Comparing `dbt-ai-0.0.8a0.tar` & `dbt-ai-0.0.9a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 13:05:57.757895 dbt-ai-0.0.8a0/
--rw-r--r--   0 armalite  (1000) armalite  (1000)       71 2023-05-06 13:04:03.000000 dbt-ai-0.0.8a0/MANIFEST.in
--rw-r--r--   0 armalite  (1000) armalite  (1000)     2004 2023-05-06 13:05:57.757895 dbt-ai-0.0.8a0/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1824 2023-05-06 13:05:14.000000 dbt-ai-0.0.8a0/README.md
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 13:05:57.757895 dbt-ai-0.0.8a0/dbt_ai/
--rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.0.8a0/dbt_ai/__init__.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1135 2023-05-06 10:40:22.000000 dbt-ai-0.0.8a0/dbt_ai/ai.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     2633 2023-05-06 09:35:47.000000 dbt-ai-0.0.8a0/dbt_ai/dbt.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)      528 2023-05-06 08:28:32.000000 dbt-ai-0.0.8a0/dbt_ai/helper.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1135 2023-05-06 09:36:12.000000 dbt-ai-0.0.8a0/dbt_ai/main.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.0.8a0/dbt_ai/py.typed
--rw-r--r--   0 armalite  (1000) armalite  (1000)      795 2023-05-06 12:58:28.000000 dbt-ai-0.0.8a0/dbt_ai/report.py
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 13:05:57.757895 dbt-ai-0.0.8a0/dbt_ai/templates/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3099 2023-05-06 10:46:28.000000 dbt-ai-0.0.8a0/dbt_ai/templates/report_template.html
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 13:05:57.757895 dbt-ai-0.0.8a0/dbt_ai.egg-info/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     2004 2023-05-06 13:05:57.000000 dbt-ai-0.0.8a0/dbt_ai.egg-info/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)      376 2023-05-06 13:05:57.000000 dbt-ai-0.0.8a0/dbt_ai.egg-info/SOURCES.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-06 13:05:57.000000 dbt-ai-0.0.8a0/dbt_ai.egg-info/dependency_links.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       44 2023-05-06 13:05:57.000000 dbt-ai-0.0.8a0/dbt_ai.egg-info/entry_points.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)      155 2023-05-06 13:05:57.000000 dbt-ai-0.0.8a0/dbt_ai.egg-info/requires.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-06 13:05:57.000000 dbt-ai-0.0.8a0/dbt_ai.egg-info/top_level.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1542 2023-05-06 13:05:47.000000 dbt-ai-0.0.8a0/pyproject.toml
--rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-06 13:05:57.757895 dbt-ai-0.0.8a0/setup.cfg
--rw-r--r--   0 armalite  (1000) armalite  (1000)      165 2023-05-06 12:18:31.000000 dbt-ai-0.0.8a0/setup.py
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 13:35:27.417895 dbt-ai-0.0.9a0/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       71 2023-05-06 13:04:03.000000 dbt-ai-0.0.9a0/MANIFEST.in
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     2006 2023-05-06 13:35:27.417895 dbt-ai-0.0.9a0/PKG-INFO
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1826 2023-05-06 13:35:04.000000 dbt-ai-0.0.9a0/README.md
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 13:35:27.417895 dbt-ai-0.0.9a0/dbt_ai/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.0.9a0/dbt_ai/__init__.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1198 2023-05-06 13:16:42.000000 dbt-ai-0.0.9a0/dbt_ai/ai.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     2650 2023-05-06 13:18:01.000000 dbt-ai-0.0.9a0/dbt_ai/dbt.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      555 2023-05-06 13:20:07.000000 dbt-ai-0.0.9a0/dbt_ai/helper.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1135 2023-05-06 13:15:40.000000 dbt-ai-0.0.9a0/dbt_ai/main.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.0.9a0/dbt_ai/py.typed
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      811 2023-05-06 13:18:50.000000 dbt-ai-0.0.9a0/dbt_ai/report.py
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 13:35:27.417895 dbt-ai-0.0.9a0/dbt_ai/templates/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     3099 2023-05-06 10:46:28.000000 dbt-ai-0.0.9a0/dbt_ai/templates/report_template.html
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-06 13:35:27.417895 dbt-ai-0.0.9a0/dbt_ai.egg-info/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     2006 2023-05-06 13:35:27.000000 dbt-ai-0.0.9a0/dbt_ai.egg-info/PKG-INFO
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      376 2023-05-06 13:35:27.000000 dbt-ai-0.0.9a0/dbt_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-06 13:35:27.000000 dbt-ai-0.0.9a0/dbt_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       44 2023-05-06 13:35:27.000000 dbt-ai-0.0.9a0/dbt_ai.egg-info/entry_points.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      155 2023-05-06 13:35:27.000000 dbt-ai-0.0.9a0/dbt_ai.egg-info/requires.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-06 13:35:27.000000 dbt-ai-0.0.9a0/dbt_ai.egg-info/top_level.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1566 2023-05-06 13:35:13.000000 dbt-ai-0.0.9a0/pyproject.toml
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-06 13:35:27.417895 dbt-ai-0.0.9a0/setup.cfg
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      144 2023-05-06 13:15:40.000000 dbt-ai-0.0.9a0/setup.py
```

### Comparing `dbt-ai-0.0.8a0/PKG-INFO` & `dbt-ai-0.0.9a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.0.8a0
+Version: 0.0.9a0
 Summary: AI powered DBT helper application
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # DBT AI
 
 This application helps you improve your dbt models by providing suggestions using the OpenAI GPT-3.5 model.
 
 ## Installation
 You can install the application here
 ```bash
-pip install dbt-ai==0.0.8a0
+pip install dbt-ai==0.0.9a0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key. 
@@ -38,14 +38,14 @@
     dbt-ai path/to/dbt/project
 ```
 
 Please allow some time for the AI model to process your dbt models. The application will process all dbt model files in your project and generate an HTML report with suggestions for each model. The report will be saved as dbt_model_suggestions.html within the dbt project directory. Upon generation of the report, it will be opened in a new browser tab.
 
 ## Generated Report
 This shows an example of a report generated from a DBT project containing 3 models
-![](images/ai_generated_dbt_report.png?raw=true)
+![](images/ai_generated_dbt_report_1.png?raw=true)
 
 
 ## Contributing
 We welcome contributions to the project! Please feel free to open issues or submit pull requests with your improvements and suggestions.
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) to get started and develop in this repo.
```

### Comparing `dbt-ai-0.0.8a0/README.md` & `dbt-ai-0.0.9a0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # DBT AI
 
 This application helps you improve your dbt models by providing suggestions using the OpenAI GPT-3.5 model.
 
 ## Installation
 You can install the application here
 ```bash
-pip install dbt-ai==0.0.8a0
+pip install dbt-ai==0.0.9a0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key. 
@@ -30,14 +30,14 @@
     dbt-ai path/to/dbt/project
 ```
 
 Please allow some time for the AI model to process your dbt models. The application will process all dbt model files in your project and generate an HTML report with suggestions for each model. The report will be saved as dbt_model_suggestions.html within the dbt project directory. Upon generation of the report, it will be opened in a new browser tab.
 
 ## Generated Report
 This shows an example of a report generated from a DBT project containing 3 models
-![](images/ai_generated_dbt_report.png?raw=true)
+![](images/ai_generated_dbt_report_1.png?raw=true)
 
 
 ## Contributing
 We welcome contributions to the project! Please feel free to open issues or submit pull requests with your improvements and suggestions.
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) to get started and develop in this repo.
```

### Comparing `dbt-ai-0.0.8a0/dbt_ai/ai.py` & `dbt-ai-0.0.9a0/dbt_ai/ai.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+# flake8: noqa
+
 import openai
 
 
 def generate_response(prompt) -> list:
     response = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         messages=[
-            {"role": "system", "content": "You are a helpful assistant that suggests improvements to dbt models. \
+            {
+                "role": "system",
+                "content": "You are a helpful assistant that suggests improvements to dbt models. \
             For the suggestions for each model you provide, simply start it with 'Suggestions for model <model name>' \
             followed by a new line. Surround the model name with ` so it is rendered like code and that underscores in the name dont get rendered. \
             Keep your suggestions fairly concise and easy to read. Order your suggestions in a logical order. \
             Add a new line in between list entries in your suggestions to help the application render it in html more nicely. Make sure \
             this is done for all the model suggestions. Favor using new lines for every point - do not randomize the formatting. \
-             "},
+             ",
+            },
             {"role": "user", "content": prompt},
         ],
         max_tokens=400,
         n=1,
         stop=None,
         temperature=0,
     )
```

### Comparing `dbt-ai-0.0.8a0/dbt_ai/dbt.py` & `dbt-ai-0.0.9a0/dbt_ai/dbt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 import glob
 import os
 
 import yaml
 
 from dbt_ai.ai import generate_response
-from dbt_ai.helper import find_yaml_files, format_suggestion
+from dbt_ai.helper import find_yaml_files
 
 
 class DbtModelProcessor:
     """Class containing functions to process and analyse a DBT project"""
 
-    def __init__(self, dbt_project_path):
+    def __init__(self, dbt_project_path) -> None:
         self.dbt_project_path = dbt_project_path
         self.yaml_files = find_yaml_files(dbt_project_path)
         self.api_key_available = bool(os.getenv("OPENAI_API_KEY"))
         if not self.api_key_available:
             print("Warning: OPENAI_API_KEY is not set. Suggestion features will be unavailable.")
 
-    def suggest_dbt_model_improvements(self, file_path, model_name) -> list:
+    def suggest_dbt_model_improvements(self, file_path: str, model_name: str) -> list:
         with open(file_path, "r") as f:
             content = f.read()
         prompt = f"Given the following dbt model {model_name}:\n\n{content}\n\nPlease provide suggestions on how to improve this model in terms of syntax, code structure and dbt best practices such as using ref instead of hardcoding table names:"
         response = generate_response(prompt)
         return response
 
-    def model_has_metadata(self, model_name) -> bool:
+    def model_has_metadata(self, model_name: str) -> bool:
         for yaml_file in self.yaml_files:
             with open(yaml_file, "r") as f:
                 try:
                     yaml_content = yaml.safe_load(f)
 
                     if yaml_content:
                         for item in yaml_content.get("models", []):
                             if isinstance(item, dict) and item.get("name") == model_name:
                                 return True
                 except yaml.YAMLError as e:
                     print(f"Error parsing YAML file {yaml_file}: {e}")
 
         return False
 
-    def process_model(self, model_file) -> dict:
+    def process_model(self, model_file: str) -> dict:
         model_name = os.path.basename(model_file).replace(".sql", "")
 
         has_metadata = self.model_has_metadata(model_name)
         if self.api_key_available:
             raw_suggestion = self.suggest_dbt_model_improvements(model_file, model_name)
         else:
             raw_suggestion = ""
 
         return {
             "model_name": model_name,
             "metadata_exists": has_metadata,
             "suggestions": raw_suggestion,
         }
 
-    def process_dbt_models(self):
+    def process_dbt_models(self):  # flake8: noqa
         model_files = glob.glob(os.path.join(self.dbt_project_path, "models/**/*.sql"), recursive=True)
         models = [self.process_model(model_file) for model_file in model_files]
         missing_metadata = []
 
         # Check for models without metadata
         for model in models:
-            if not model['metadata_exists']:
-                missing_metadata.append(model['model_name'])
-        
+            if not model["metadata_exists"]:
+                missing_metadata.append(model["model_name"])
+
         return models, missing_metadata
```

### Comparing `dbt-ai-0.0.8a0/dbt_ai/helper.py` & `dbt-ai-0.0.9a0/dbt_ai/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+# flake8: noqa
+
 import glob
-import os
 import html
+import os
 
 
-def find_yaml_files(dbt_project_path):
+def find_yaml_files(dbt_project_path: str):
     yaml_files = glob.glob(os.path.join(dbt_project_path, "**/*.yml"), recursive=True)
     yaml_files.extend(glob.glob(os.path.join(dbt_project_path, "**/*.yaml"), recursive=True))
     return yaml_files
 
 
-def format_suggestion(suggestion):
+def format_suggestion(suggestion: str):
     html_suggestion = ""
 
     escaped_suggestion = html.escape(suggestion)
     formatted_suggestion = escaped_suggestion.replace("\n", "<br>")
     html_suggestion = formatted_suggestion
 
-    return html_suggestion
+    return html_suggestion
```

### Comparing `dbt-ai-0.0.8a0/dbt_ai/main.py` & `dbt-ai-0.0.9a0/dbt_ai/main.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import os
 
 from dbt_ai.dbt import DbtModelProcessor
 from dbt_ai.report import generate_html_report
 
+
 def main() -> None:
     parser = argparse.ArgumentParser(
         description="Generate improvement suggestions and check metadata coverage for dbt models"
     )
     parser.add_argument("dbt_project_path", help="Path to the dbt project directory")
     args = parser.parse_args()
 
@@ -25,10 +26,9 @@
         print("\nThe following models are missing metadata:")
         for model_name in models_without_metadata:
             print(f"  - {model_name}")
     else:
         print("\nAll models have associated metadata.")
 
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `dbt-ai-0.0.8a0/dbt_ai/report.py` & `dbt-ai-0.0.9a0/dbt_ai/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from jinja2 import Environment, FileSystemLoader
-import webbrowser 
-import markdown2
+# flake8: noqa
+
 import os
+import webbrowser
+
+import markdown2
+from jinja2 import Environment, FileSystemLoader
 
 
 def markdown_filter(value):
     return markdown2.markdown(value, extras=["fenced-code-blocks"])
 
 
 def generate_html_report(models, output_path, missing_metadata: list[str]):
     template_path = os.path.join(os.path.dirname(__file__), "templates", "report_template.html")
     env = Environment(loader=FileSystemLoader(os.path.dirname(template_path)))
-    env.filters['markdown'] = markdown_filter
+    env.filters["markdown"] = markdown_filter
     template = env.get_template(os.path.basename(template_path))
 
     rendered_report = template.render(models=models, missing_metadata=missing_metadata)
     with open(output_path, "w") as f:
         f.write(rendered_report)
 
     # Open the report in a new browser tab
```

### Comparing `dbt-ai-0.0.8a0/dbt_ai/templates/report_template.html` & `dbt-ai-0.0.9a0/dbt_ai/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.0.8a0/dbt_ai.egg-info/PKG-INFO` & `dbt-ai-0.0.9a0/dbt_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.0.8a0
+Version: 0.0.9a0
 Summary: AI powered DBT helper application
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # DBT AI
 
 This application helps you improve your dbt models by providing suggestions using the OpenAI GPT-3.5 model.
 
 ## Installation
 You can install the application here
 ```bash
-pip install dbt-ai==0.0.8a0
+pip install dbt-ai==0.0.9a0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
  - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key. 
@@ -38,14 +38,14 @@
     dbt-ai path/to/dbt/project
 ```
 
 Please allow some time for the AI model to process your dbt models. The application will process all dbt model files in your project and generate an HTML report with suggestions for each model. The report will be saved as dbt_model_suggestions.html within the dbt project directory. Upon generation of the report, it will be opened in a new browser tab.
 
 ## Generated Report
 This shows an example of a report generated from a DBT project containing 3 models
-![](images/ai_generated_dbt_report.png?raw=true)
+![](images/ai_generated_dbt_report_1.png?raw=true)
 
 
 ## Contributing
 We welcome contributions to the project! Please feel free to open issues or submit pull requests with your improvements and suggestions.
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) to get started and develop in this repo.
```

### Comparing `dbt-ai-0.0.8a0/pyproject.toml` & `dbt-ai-0.0.9a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dbt-ai"
 description = "AI powered DBT helper application"
-version = "0.0.8-alpha"
+version = "0.0.9-alpha"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "dbt-snowflake~=1.4",
     "openai~=0.27",
     "pyyaml~=6.0",
     "markdown2~=2.4",
@@ -28,14 +28,15 @@
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["tests*"]
 
 # use PyCharm default line length of 120
 [tool.black]
 line-length = 120
+exclude = "conftest.py"
 
 [tool.ruff]
 line-length = 120
 
 # rules to enable/ignore
 select = [
     # pyflakes
```

