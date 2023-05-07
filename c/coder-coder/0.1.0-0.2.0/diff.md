# Comparing `tmp/coder_coder-0.1.0.tar.gz` & `tmp/coder_coder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coder_coder-0.1.0.tar", max compression
+gzip compressed data, was "coder_coder-0.2.0.tar", max compression
```

## Comparing `coder_coder-0.1.0.tar` & `coder_coder-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-28 01:18:29.778471 coder_coder-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-28 01:18:29.778418 coder_coder-0.1.0/coder_coder/__init__.py
--rw-r--r--   0        0        0     8845 2023-05-06 17:09:20.222938 coder_coder-0.1.0/coder_coder/cli.py
--rw-r--r--   0        0        0     1399 2023-05-06 01:03:12.267329 coder_coder-0.1.0/coder_coder/content.py
--rw-r--r--   0        0        0     2381 2023-05-06 19:32:44.634729 coder_coder-0.1.0/coder_coder/main.py
--rw-r--r--   0        0        0      543 2023-05-06 19:36:29.570956 coder_coder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 coder_coder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-05-07 00:14:21.467321 coder_coder-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 01:18:29.778418 coder_coder-0.2.0/coder_coder/__init__.py
+-rw-r--r--   0        0        0     8845 2023-05-06 17:09:20.222938 coder_coder-0.2.0/coder_coder/cli.py
+-rw-r--r--   0        0        0     1399 2023-05-06 01:03:12.267329 coder_coder-0.2.0/coder_coder/content.py
+-rw-r--r--   0        0        0     3614 2023-05-06 20:44:18.429199 coder_coder-0.2.0/coder_coder/main.py
+-rw-r--r--   0        0        0      543 2023-05-07 00:34:26.571293 coder_coder-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 coder_coder-0.2.0/PKG-INFO
```

### Comparing `coder_coder-0.1.0/coder_coder/cli.py` & `coder_coder-0.2.0/coder_coder/cli.py`

 * *Files identical despite different names*

### Comparing `coder_coder-0.1.0/coder_coder/content.py` & `coder_coder-0.2.0/coder_coder/content.py`

 * *Files identical despite different names*

### Comparing `coder_coder-0.1.0/coder_coder/main.py` & `coder_coder-0.2.0/coder_coder/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,43 @@
 import json
-import math
 import os
-import time
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Any
 
 import typer
 
 import openai
 from dotenv import load_dotenv
 
-load_dotenv(Path(__file__).parent.parent / "env" /".env")
-openai.api_key = os.environ["OPENAI_API_KEY"]  # supply your API key however you choose
-openai.organization = os.environ["OPENAI_ORG_ID"]  # supply your organization key however you choose
+coder_env = Path.home() / ".coder_code"
+if not coder_env.exists():
+    coder_env.mkdir()
 
 
+def load_config():
+    config_file = coder_env / "config.json"
+    if config_file.exists():
+        with open(config_file, "r") as f:
+            config = json.load(f)
+    else:
+        config = {"text_model": "gpt-4"}
+    for k, v in config.items():
+        os.environ[k] = v
+    return config
+
+def save_config(config):
+    config_file = coder_env / "config.json"
+    with open(config_file, "w") as f:
+        json.dump(config, f)
+
+
+CONFIG = load_config()
+openai.api_key = os.environ["OPENAI_API_KEY"]
+openai.organization = os.environ["OPENAI_ORG_ID"]
+
 app = typer.Typer()
 
 
 @app.callback()
 def callback():
     """
     Awesome Portal Gun
@@ -37,38 +56,64 @@
         with open(in_file, "r") as f:
             existing_code = f.read()
         prompt = f"""Given this existing code {existing_code}. Write code to {user_prompt}. 
         Use or rewrite the existing code in a logical way without losing any of the functionality of the existing code.
          Output code only. No description."""
     else:
         prompt = f"Write code to {user_prompt}. Output the code only. No description."
-    completion = openai.ChatCompletion.create(model="gpt-4", messages=[{"role": "user", "content": prompt}])
+    completion = openai.ChatCompletion.create(model=CONFIG["text_model"], messages=[{"role": "user", "content": prompt}])
     text_response = completion.choices[0].message.content
     typer.echo(text_response)
     if out_file:
         with open(out_file, "w") as f:
             f.write(text_response)
 
 
 @app.command()
+def document(in_file: Optional[str] = typer.Argument(...)):
+    typer.echo(f"Documenting: {in_file}")
+    prompt = f"""Write documentation for the following code: {in_file}"""
+    completion = openai.ChatCompletion.create(model=CONFIG["text_model"], messages=[{"role": "user", "content": prompt}])
+    text_response = completion.choices[0].message.content
+    typer.echo(text_response)
+
+
+@app.command()
 def plan(user_prompt: str = typer.Argument(...),
          out_file: Optional[str] = typer.Option(None)):
+    typer.echo(f"Planning: {user_prompt}")
     prompt = f"""
 Develop a plan for the following goal: {user_prompt}
 """
-    completion = openai.ChatCompletion.create(model="gpt-4", messages=[{"role": "user", "content": prompt}])
+    completion = openai.ChatCompletion.create(model=CONFIG["text_model"], messages=[{"role": "user", "content": prompt}])
     text_response = completion.choices[0].message.content
     typer.echo(text_response)
     if out_file:
         with open(out_file, "w") as f:
             f.write(text_response)
 
 
 @app.command()
 def prompt(user_prompt: str = typer.Argument(...),
          out_file: Optional[str] = typer.Option(None)):
-    completion = openai.ChatCompletion.create(model="gpt-4", messages=[{"role": "user", "content": user_prompt}])
+    typer.echo(f"Prompting: {user_prompt}")
+    completion = openai.ChatCompletion.create(model=CONFIG["text_model"], messages=[{"role": "user", "content": user_prompt}])
     text_response = completion.choices[0].message.content
     typer.echo(text_response)
     if out_file:
         with open(out_file, "w") as f:
             f.write(text_response)
+
+
+@app.command()
+def set_config(key: str = typer.Argument(...),
+               value: str = typer.Argument(...)):
+    CONFIG[key] = value
+    save_config(CONFIG)
+
+
+@app.command()
+def get_config(key: str = typer.Option(default=None)):
+    if key is not None:
+        typer.echo(CONFIG[key])
+    else:
+        typer.echo(CONFIG)
```

### Comparing `coder_coder-0.1.0/pyproject.toml` & `coder_coder-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coder-coder"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Kevin Fortier <kevin.r.fortier@gmail.com>"]
 readme = "README.md"
 packages = [{include = "coder_coder"}]
 
 [tool.poetry.scripts]
 coder = "coder_coder.main:app"
```

