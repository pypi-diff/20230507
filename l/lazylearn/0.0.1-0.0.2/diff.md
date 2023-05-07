# Comparing `tmp/lazylearn-0.0.1.tar.gz` & `tmp/lazylearn-0.0.2.tar.gz`

## Comparing `lazylearn-0.0.1.tar` & `lazylearn-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,35 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 lazylearn-0.0.1/Pipfile
--rw-r--r--   0        0        0    14496 2020-02-02 00:00:00.000000 lazylearn-0.0.1/Pipfile.lock
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 lazylearn-0.0.1/.github/workflows/verify.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.1/python/src/easylearn/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.1/python/src/easylearn/ingestion/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.1/python/src/easylearn/models/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 lazylearn-0.0.1/python/src/easylearn/models/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.1/python/src/easylearn/pipeline/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 lazylearn-0.0.1/python/src/test/test_mock.py
--rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 lazylearn-0.0.1/shell/check.sh
--rwxr-xr-x   0        0        0      372 2020-02-02 00:00:00.000000 lazylearn-0.0.1/shell/tidy.sh
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 lazylearn-0.0.1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 lazylearn-0.0.1/LICENSE
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 lazylearn-0.0.1/README.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 lazylearn-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 lazylearn-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 lazylearn-0.0.2/Pipfile
+-rw-r--r--   0        0        0    74533 2020-02-02 00:00:00.000000 lazylearn-0.0.2/Pipfile.lock
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 lazylearn-0.0.2/.github/workflows/verify.yaml
+-rw-r--r--   0        0        0    59514 2020-02-02 00:00:00.000000 lazylearn-0.0.2/doc/logo/grayscale_transparent.png
+-rw-r--r--   0        0        0    62685 2020-02-02 00:00:00.000000 lazylearn-0.0.2/doc/logo/original.png
+-rw-r--r--   0        0        0    66560 2020-02-02 00:00:00.000000 lazylearn-0.0.2/doc/logo/transparent.png
+-rw-r--r--   0        0        0    71882 2020-02-02 00:00:00.000000 lazylearn-0.0.2/doc/logo/transparent_small.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/__init__.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/lazylearn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/errors/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/errors/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/ingestion/__init__.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline_steps/__init__.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline_steps/data_parser_step.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline_steps/interpreter_step.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline_steps/summary_stats_step.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/models/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/models/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/pipeline/__init__.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/pipeline/pipeline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/preprocessing/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/preprocessing/encoding/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/preprocessing/encoding/encoders.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/test/test_mock.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/test/ingestion/ingestion_pipeline_steps/test_data_parser_step.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/test/ingestion/ingestion_pipeline_steps/test_interpreter_step.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/test/ingestion/ingestion_pipeline_steps/test_summary_stats_step.py
+-rwxr-xr-x   0        0        0      743 2020-02-02 00:00:00.000000 lazylearn-0.0.2/shell/check.sh
+-rwxr-xr-x   0        0        0      382 2020-02-02 00:00:00.000000 lazylearn-0.0.2/shell/tidy.sh
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 lazylearn-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 lazylearn-0.0.2/LICENSE
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 lazylearn-0.0.2/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 lazylearn-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 lazylearn-0.0.2/PKG-INFO
```

### Comparing `lazylearn-0.0.1/.github/workflows/verify.yaml` & `lazylearn-0.0.2/.github/workflows/verify.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: Linting & Testing
 
 on:
   pull_request:
 
 env:
-  PYTHONPATH: ./python/src/main/
+  PYTHONPATH: ./python/src/lazylearn/
 
 jobs:
   testing:
     runs-on: ubuntu-latest
     steps:
       - name: "Checkout"
         uses: actions/checkout@v3
@@ -50,16 +50,16 @@
 
       - name: Install linters
         run: |
           pip install black isort flake8
 
       - name: black
         run: |
-          python -m black --check python/src/main/
+          python -m black --check python/src/lazylearn/
 
       - name: isort
         run: |
-          python -m isort python/src/main/ --multi-line 3 --profile black --check
+          python -m isort python/src/lazylearn/ --multi-line 3 --profile black --check
 
       - name: flake8
         run: |
-          python -m flake8 python/src/main/
+          python -m flake8 python/src/lazylearn/
```

### Comparing `lazylearn-0.0.1/shell/check.sh` & `lazylearn-0.0.2/shell/check.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/bin/bash
 #
 # Perform code style checks of the Python code.
 export PIPENV_VERBOSITY=-1
 set -e
 
 echo "--- black ---"
-pipenv run black --line-length 88 --check python/src/easy-learn/
+pipenv run black --line-length 88 --check python/src/lazylearn/
 pipenv run black --line-length 88 --check python/src/test/
 echo "--- isort ---"
-pipenv run isort python/src/easy-learn/ --multi-line 3 --profile black --check
+pipenv run isort python/src/lazylearn/ --multi-line 3 --profile black --check
 pipenv run isort python/src/test/ --multi-line 3 --profile black --check
 echo "--- flake8 ---"
-pipenv run flake8 python/src/easy-learn/
+pipenv run flake8 python/src/lazylearn/
 pipenv run flake8 python/src/test/
 echo "--- pytest ---"
 if [[ "$OSTYPE" == "msys" ]]; then
-  PYTHONPATH="./python/src/main;$PYTHONPATH" pipenv run pytest python/src/test/
+  PYTHONPATH="./python/src/lazylearn;$PYTHONPATH" pipenv run pytest python/src/test/
 else
-  PYTHONPATH=./python/src/main:$PYTHONPATH pipenv run pytest python/src/test/
+  PYTHONPATH=./python/src/lazylearn:$PYTHONPATH pipenv run pytest python/src/test/
 fi
```

### Comparing `lazylearn-0.0.1/.gitignore` & `lazylearn-0.0.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 # macos
 .DS_Store
 
 # JetBrains
 .idea
 
+# local
+notebooks/
+
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
```

### Comparing `lazylearn-0.0.1/LICENSE` & `lazylearn-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.1/PKG-INFO` & `lazylearn-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,42 @@
 Metadata-Version: 2.1
 Name: lazylearn
-Version: 0.0.1
-Summary: A small example package
-Project-URL: Homepage, https://github.com/pypa/sampleproject
+Version: 0.0.2
+Summary: lazy-learn is a high-level Python interface for automated machine learning (AutoML) for the lazy data scientist. While there are many AutoML libraries available each typically solves a niche area of the overall ML pipeline without providing a covering and approachable end-to-end system. lazy-learn aims at providing the most approachable and fastest access to building baseline models.
+Project-URL: Homepage, https://github.com/frederikhoengaard/lazy-learn
 Author-email: "Frederik P. Høngaard" <mail@frederikhoengaard.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# easy-learn
 
----
+<img width="500" src="doc/logo/transparent_small.png">
 
-## About
+**lazy-learn** is a high-level Python interface for automated machine learning (AutoML). While there are many AutoML libraries available each typically solves a niche area of the overall ML pipeline without providing a covering and approachable end-to-end system.
 
-easy-learn is a high-level Python interface for automated machine learning (AutoML). While there are many AutoML libraries available each typically solves a niche area of the overall ML pipeline without providing a covering and approachable end-to-end system.
-
-The aim of easy-learn is exactly that. Given a dataset, easy-learn will analyse types and distributions of attributes, preprocess, feature-engineer and ultimately train models to be used for further evaluation or inference. 
+The aim of lazy-learn is exactly that. Given a dataset, easy-learn will analyse types and distributions of attributes, preprocess, feature-engineer and ultimately train models to be used for further evaluation or inference. 
 
 ## Usage
 
+Using lazy-learn revolves around the `LazyLearner` class. You can think of it as a kind of project, and it is the wrapper for any experiment within lazy-learn.
+
+## Installation
+
+### Dependencies
+
+lazy-learn requires:
+
+- pandas
+- scikit-learn
+
+### User Installation 
+```
+pip install lazy-learn
+```
+
+## Help and Support
+### Documentation
+
+### Citation
```

