# Comparing `tmp/thera-py-0.4.0.tar.gz` & `tmp/thera-py-0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thera-py-0.4.0.tar", last modified: Wed Jan 11 19:02:49 2023, max compression
+gzip compressed data, was "thera-py-0.4.dev0.tar", last modified: Sun Oct  2 20:50:34 2022, max compression
```

## Comparing `thera-py-0.4.0.tar` & `thera-py-0.4.dev0.tar`

### file list

```diff
@@ -1,37 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:02:49.356951 thera-py-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-11 19:02:44.000000 thera-py-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-01-11 19:02:49.356951 thera-py-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-01-11 19:02:44.000000 thera-py-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-11 19:02:44.000000 thera-py-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-01-11 19:02:49.356951 thera-py-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-11 19:02:44.000000 thera-py-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:02:49.352951 thera-py-0.4.0/thera_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-01-11 19:02:49.000000 thera-py-0.4.0/thera_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-11 19:02:49.000000 thera-py-0.4.0/thera_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 19:02:49.000000 thera-py-0.4.0/thera_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 19:02:49.000000 thera-py-0.4.0/thera_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-01-11 19:02:49.000000 thera-py-0.4.0/thera_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-11 19:02:49.000000 thera-py-0.4.0/thera_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:02:49.356951 thera-py-0.4.0/therapy/
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:02:49.356951 thera-py-0.4.0/therapy/etl/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/chembl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/chemidplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/drugbank.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/drugsatfda.py
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/guidetopharmacology.py
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/hemonc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/ncit.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/rules.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/rxnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/etl/wikidata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    29298 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    36896 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-11 19:02:44.000000 thera-py-0.4.0/therapy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 20:50:34.211768 thera-py-0.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (121)     6161 2022-10-02 20:50:34.211768 thera-py-0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5820 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-10-02 20:50:34.211768 thera-py-0.4.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 20:50:34.207768 thera-py-0.4.dev0/thera_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6161 2022-10-02 20:50:34.000000 thera-py-0.4.dev0/thera_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2022-10-02 20:50:34.000000 thera-py-0.4.dev0/thera_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-02 20:50:34.000000 thera-py-0.4.dev0/thera_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-02 20:50:34.000000 thera-py-0.4.dev0/thera_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-10-02 20:50:34.000000 thera-py-0.4.dev0/thera_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-02 20:50:34.000000 thera-py-0.4.dev0/thera_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 20:50:34.211768 thera-py-0.4.dev0/therapy/
+-rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12093 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15544 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/database.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 20:50:34.211768 thera-py-0.4.dev0/therapy/etl/
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12914 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/etl/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8149 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/etl/chembl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4799 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/etl/chemidplus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3064 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/etl/drugbank.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6692 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/etl/drugsatfda.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10006 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/etl/guidetopharmacology.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12689 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/etl/hemonc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11686 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/etl/merge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7604 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/etl/ncit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14844 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/etl/rxnorm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6060 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/etl/wikidata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7156 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29298 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/query.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37523 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-02 20:50:25.000000 thera-py-0.4.dev0/therapy/version.py
```

### Comparing `thera-py-0.4.0/PKG-INFO` & `thera-py-0.4.dev0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: thera-py
-Version: 0.4.0
+Version: 0.4.dev0
 Summary: VICC normalization routine for therapies
 Home-page: https://github.com/cancervariants/therapy-normalization
 Author: VICC
 Author-email: help@cancervariants.org
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE
+Provides-Extra: dev
 
 # Therapy Normalization
 Services and guidelines for normalizing drug (and non-drug therapy) terms
 
 ## Developer instructions
 The following sections include instructions specifically for developers.
 
@@ -51,28 +49,26 @@
 
 ```commandline
 pre-commit install
 ```
 
 ### Running tests
 
-Unit tests are provided via pytest.
+Unit tests are run with pytest.
 
 ```commandline
 pipenv run pytest
 ```
 
-By default, tests will employ an existing DynamoDB database. For test environments where this is unavailable (e.g. in CI), the `THERAPY_TEST` environment variable can be set to initialize a local DynamoDB instance with miniature versions of input data files before tests are executed.
+We also provide [Tox](https://tox.wiki/en/latest/index.html) settings to test in multiple environments and check for proper type annotations and code style. If interpreters for Python 3.8 and Python 3.9 are present, the following will run all tests for all environments:
 
 ```commandline
-export THERAPY_TEST=true
+tox
 ```
 
-Sometimes, sources will update their data, and our test fixtures and data will become incorrect. The `tests/scripts/` subdirectory includes scripts to rebuild data files, although most fixtures will need to be updated manually.
-
 ### Updating the database
 
 Before you use the CLI to update the database, run the following in a separate terminal to start DynamoDB on `port 8000`:
 
 ```
 java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
 ```
@@ -174,18 +170,7 @@
 ```commandline
 uvicorn therapy.main:app --reload
 ```
 
 Next, view the OpenAPI docs on your local machine:
 
 http://127.0.0.1:8000/therapy
-
-
-### FAQ
-
-**A data import method raised a SourceFormatException instance. How do I proceed?**
-
-TheraPy will automatically try to acquire the latest version of data for each source, but sometimes, sources alter the structure of their data (e.g. adding or removing CSV columns). If you encounter a SourceFormatException while importing data, please notify us by creating a new [issue](https://github.com/cancervariants/therapy-normalization/issues) if one doesn't already exist, and we will attempt to resolve it.
-
-In the meantime, you can force TheraPy to use an older data release by removing the incompatible version from the source data folder, manually downloading and replacing it with an older version of the data per the structure described above, and calling the CLI with the `--use_existing` argument.
-
-
```

### Comparing `thera-py-0.4.0/README.md` & `thera-py-0.4.dev0/thera_py.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: thera-py
+Version: 0.4.dev0
+Summary: VICC normalization routine for therapies
+Home-page: https://github.com/cancervariants/therapy-normalization
+Author: VICC
+Author-email: help@cancervariants.org
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+
 # Therapy Normalization
 Services and guidelines for normalizing drug (and non-drug therapy) terms
 
 ## Developer instructions
 The following sections include instructions specifically for developers.
 
 ### Installation
@@ -36,28 +49,26 @@
 
 ```commandline
 pre-commit install
 ```
 
 ### Running tests
 
-Unit tests are provided via pytest.
+Unit tests are run with pytest.
 
 ```commandline
 pipenv run pytest
 ```
 
-By default, tests will employ an existing DynamoDB database. For test environments where this is unavailable (e.g. in CI), the `THERAPY_TEST` environment variable can be set to initialize a local DynamoDB instance with miniature versions of input data files before tests are executed.
+We also provide [Tox](https://tox.wiki/en/latest/index.html) settings to test in multiple environments and check for proper type annotations and code style. If interpreters for Python 3.8 and Python 3.9 are present, the following will run all tests for all environments:
 
 ```commandline
-export THERAPY_TEST=true
+tox
 ```
 
-Sometimes, sources will update their data, and our test fixtures and data will become incorrect. The `tests/scripts/` subdirectory includes scripts to rebuild data files, although most fixtures will need to be updated manually.
-
 ### Updating the database
 
 Before you use the CLI to update the database, run the following in a separate terminal to start DynamoDB on `port 8000`:
 
 ```
 java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
 ```
@@ -159,16 +170,7 @@
 ```commandline
 uvicorn therapy.main:app --reload
 ```
 
 Next, view the OpenAPI docs on your local machine:
 
 http://127.0.0.1:8000/therapy
-
-
-### FAQ
-
-**A data import method raised a SourceFormatException instance. How do I proceed?**
-
-TheraPy will automatically try to acquire the latest version of data for each source, but sometimes, sources alter the structure of their data (e.g. adding or removing CSV columns). If you encounter a SourceFormatException while importing data, please notify us by creating a new [issue](https://github.com/cancervariants/therapy-normalization/issues) if one doesn't already exist, and we will attempt to resolve it.
-
-In the meantime, you can force TheraPy to use an older data release by removing the incompatible version from the source data folder, manually downloading and replacing it with an older version of the data per the structure described above, and calling the CLI with the `--use_existing` argument.
```

### Comparing `thera-py-0.4.0/setup.cfg` & `thera-py-0.4.dev0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -10,52 +10,55 @@
 
 [options]
 packages = find:
 python_requires = >=3.8
 zip_safe = False
 include_package_data = True
 install_requires = 
-	pydantic >=1.8.2
 	fastapi >= 0.72.0
-	click
+	urllib3 >= 1.26.5
 	uvicorn
+	uvloop
+	websockets >= 9.1
+	click
+	lxml >= 4.6.5
 	boto3
+	cython
+	owlready2
+	pyparsing == 2.4.7
+	rdflib
+	wikibaseintegrator >= 0.12.0
+	bs4
+	pyyaml
+	pydantic >=1.8.2
+	chembl-downloader
+	pystow
+	bioversions >= 0.4.3
+	disease-normalizer >= 0.2.14
 	ga4gh.vrsatile.pydantic >= 0.1.dev3
 
-[options.package_data]
-therapy = 
-	etl/*
-
 [options.extras_require]
 test = 
+	tox
 	pytest
 	pytest-cov
 dev = 
-	disease-normalizer >= 0.3.1
-	owlready2
-	rdflib
-	wikibaseintegrator >= 0.12.0
-	chembl-downloader
-	bioversions >= 0.4.3
-	ipykernel
 	pre-commit
 	tox
 	flake8
 	flake8-docstrings
 	flake8-quotes
 	flake8-import-order
 	flake8-annotations
 	mypy
 	types-requests
 	types-pyyaml
-	lxml
-	xmlformatter
 
 [tool:pytest]
-addopts = --ignore setup.py --ignore=analysis/ --cov-report term-missing --cov=therapy
+addopts = --ignore setup.py --ignore=codebuild/ --ignore=analysis/ --ignore=dynamodb_revisions/ --doctest-modules --cov-report term-missing --cov .
 
 [mypy]
 plugins = pydantic.mypy
 ignore_missing_imports = True
 
 [coverage:run]
 source =
```

### Comparing `thera-py-0.4.0/thera_py.egg-info/PKG-INFO` & `thera-py-0.4.dev0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: thera-py
-Version: 0.4.0
-Summary: VICC normalization routine for therapies
-Home-page: https://github.com/cancervariants/therapy-normalization
-Author: VICC
-Author-email: help@cancervariants.org
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 # Therapy Normalization
 Services and guidelines for normalizing drug (and non-drug therapy) terms
 
 ## Developer instructions
 The following sections include instructions specifically for developers.
 
 ### Installation
@@ -51,28 +36,26 @@
 
 ```commandline
 pre-commit install
 ```
 
 ### Running tests
 
-Unit tests are provided via pytest.
+Unit tests are run with pytest.
 
 ```commandline
 pipenv run pytest
 ```
 
-By default, tests will employ an existing DynamoDB database. For test environments where this is unavailable (e.g. in CI), the `THERAPY_TEST` environment variable can be set to initialize a local DynamoDB instance with miniature versions of input data files before tests are executed.
+We also provide [Tox](https://tox.wiki/en/latest/index.html) settings to test in multiple environments and check for proper type annotations and code style. If interpreters for Python 3.8 and Python 3.9 are present, the following will run all tests for all environments:
 
 ```commandline
-export THERAPY_TEST=true
+tox
 ```
 
-Sometimes, sources will update their data, and our test fixtures and data will become incorrect. The `tests/scripts/` subdirectory includes scripts to rebuild data files, although most fixtures will need to be updated manually.
-
 ### Updating the database
 
 Before you use the CLI to update the database, run the following in a separate terminal to start DynamoDB on `port 8000`:
 
 ```
 java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
 ```
@@ -174,18 +157,7 @@
 ```commandline
 uvicorn therapy.main:app --reload
 ```
 
 Next, view the OpenAPI docs on your local machine:
 
 http://127.0.0.1:8000/therapy
-
-
-### FAQ
-
-**A data import method raised a SourceFormatException instance. How do I proceed?**
-
-TheraPy will automatically try to acquire the latest version of data for each source, but sometimes, sources alter the structure of their data (e.g. adding or removing CSV columns). If you encounter a SourceFormatException while importing data, please notify us by creating a new [issue](https://github.com/cancervariants/therapy-normalization/issues) if one doesn't already exist, and we will attempt to resolve it.
-
-In the meantime, you can force TheraPy to use an older data release by removing the incompatible version from the source data folder, manually downloading and replacing it with an older version of the data per the structure described above, and calling the CLI with the `--use_existing` argument.
-
-
```

### Comparing `thera-py-0.4.0/thera_py.egg-info/SOURCES.txt` & `thera-py-0.4.dev0/thera_py.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 thera_py.egg-info/PKG-INFO
 thera_py.egg-info/SOURCES.txt
 thera_py.egg-info/dependency_links.txt
@@ -22,11 +21,9 @@
 therapy/etl/chemidplus.py
 therapy/etl/drugbank.py
 therapy/etl/drugsatfda.py
 therapy/etl/guidetopharmacology.py
 therapy/etl/hemonc.py
 therapy/etl/merge.py
 therapy/etl/ncit.py
-therapy/etl/rules.csv
-therapy/etl/rules.py
 therapy/etl/rxnorm.py
 therapy/etl/wikidata.py
```

### Comparing `thera-py-0.4.0/therapy/__init__.py` & `thera-py-0.4.dev0/therapy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,7 +50,13 @@
 )
 
 # Sources that we import directly
 XREF_SOURCES = {source for source in SourceName.__members__}
 
 # Sources that are found in data from imported sources
 ASSOC_WITH_SOURCES = {source for source in NamespacePrefix.__members__} - XREF_SOURCES
+
+from therapy.etl import ChEMBL, Wikidata, DrugBank, NCIt, ChemIDplus, RxNorm, HemOnc, GuideToPHARMACOLOGY, DrugsAtFDA  # noqa: E402, E501, I202
+
+# used to get source class name from string
+SOURCES_CLASS = \
+    {s.value.lower(): eval(s.value) for s in SourceName.__members__.values()}
```

### Comparing `thera-py-0.4.0/therapy/cli.py` & `thera-py-0.4.dev0/therapy/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 import click
 from botocore.exceptions import ClientError
 from boto3.dynamodb.conditions import Key
 from disease.database import Database as DiseaseDatabase
 from disease.cli import CLI as DiseaseCLI
 from disease.schemas import SourceName as DiseaseSources
 
-from therapy import SOURCES
+from therapy import SOURCES_CLASS, SOURCES
 from therapy.schemas import SourceName
-from therapy.database import Database, confirm_aws_db_use, SKIP_AWS_DB_ENV_NAME, \
-    VALID_AWS_ENV_NAMES, AWS_ENV_VAR_NAME
-from therapy.etl import ChEMBL, Wikidata, DrugBank, NCIt, ChemIDplus, RxNorm, HemOnc, GuideToPHARMACOLOGY, DrugsAtFDA  # noqa: F401, E501
+from therapy.database import Database, confirm_aws_db_use
 from therapy.etl.merge import Merge
 
 logger = logging.getLogger("therapy")
 logger.setLevel(logging.DEBUG)
 
 
 class CLI:
@@ -28,18 +26,17 @@
     @staticmethod
     @click.command()
     @click.option(
         "--normalizer",
         help="The normalizer(s) you wish to update separated by spaces."
     )
     @click.option(
-        "--aws_instance",
+        "--prod",
         is_flag=True,
-        help=" Must be `Dev`, `Staging`, or `Prod`. This determines the AWS instance to"
-             " use. `Dev` uses nonprod. `Staging` and `Prod` uses prod."
+        help="Working in production environment."
     )
     @click.option(
         "--db_url",
         help="URL endpoint for the application database."
     )
     @click.option(
         "--update_all",
@@ -53,36 +50,35 @@
     )
     @click.option(
         "--use_existing",
         is_flag=True,
         default=False,
         help="Use most recent existing source data instead of fetching latest version"
     )
-    def update_normalizer_db(normalizer: str, aws_instance: str, db_url: str,
+    def update_normalizer_db(normalizer: str, prod: bool, db_url: str,
                              update_all: bool, update_merged: bool,
                              use_existing: bool) -> None:
         """Update selected normalizer source(s) in the therapy database.
         \f  # noqa: D301
         :param str normalizer: comma-separated string listing source names
-        :param str aws_instance: The AWS environment name.
-            Must be one of: `Dev`, `Staging`, or `Prod`
+        :param bool prod: if true, utilize production environment settings
         :param str db_url: DynamoDB endpoint URL (usually only needed locally)
         :param bool update_all: if true, update all sources
         :param bool update_merged: if true, update normalized group results
         :param bool use_existing: if true, don't try to fetch latest source data
         """
-        # If SKIP_AWS_CONFIRMATION is accidentally set, we should verify that the
-        # aws instance should actually be used
-        invalid_aws_msg = f"{AWS_ENV_VAR_NAME} must be set to one of {VALID_AWS_ENV_NAMES}"  # noqa: E501
-        aws_env_name = environ.get(AWS_ENV_VAR_NAME) or aws_instance
-        if aws_env_name:
-            assert aws_env_name in VALID_AWS_ENV_NAMES, invalid_aws_msg
-            environ[AWS_ENV_VAR_NAME] = aws_env_name
-            confirm_aws_db_use(aws_env_name.upper())
-            environ[SKIP_AWS_DB_ENV_NAME] = "true"  # this is already checked above
+        # Sometimes THERAPY_NORM_EB_PROD is accidentally set. We should verify that
+        # it should actually be used in CLI
+        if "THERAPY_NORM_EB_PROD" in environ:
+            confirm_aws_db_use("PROD")
+
+        endpoint_url = None
+        if prod:
+            environ["THERAPY_NORM_PROD"] = "TRUE"
+            environ["DISEASE_NORM_PROD"] = "TRUE"
             db: Database = Database()
         else:
             if db_url:
                 endpoint_url = db_url
             elif "THERAPY_NORM_DB_URL" in environ.keys():
                 endpoint_url = environ["THERAPY_NORM_DB_URL"]
             else:
@@ -164,19 +160,14 @@
         :param Database db: database instance to use
         :param bool update_merged: if true, store concept IDs as they're processed and
             produce normalized records
         :param bool use_existing: if true, don't try to fetch latest source data in
             source perform_etl methods
         """
         processed_ids = list()
-
-        # used to get source class name from string
-        SOURCES_CLASS = \
-            {s.value.lower(): eval(s.value) for s in SourceName.__members__.values()}
-
         for n in normalizers:
             msg = f"Deleting {n}..."
             click.echo(f"\n{msg}")
             logger.info(msg)
 
             start_delete = timer()
             CLI()._delete_data(n, db)
```

### Comparing `thera-py-0.4.0/therapy/database.py` & `thera-py-0.4.dev0/therapy/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,30 @@
 """This module creates the database."""
 from os import environ
 from typing import Optional, Dict, List, Any
-from enum import Enum
 import logging
 import sys
 import atexit
 
 import click
 import boto3
 from boto3.dynamodb.conditions import Key
 from botocore.exceptions import ClientError
 
 from therapy import PREFIX_LOOKUP
 
 logger = logging.getLogger("therapy")
 logger.setLevel(logging.DEBUG)
 
-# can be set to either `Dev`, `Staging`, or `Prod`
-# ONLY set when wanting to access aws instance
-AWS_ENV_VAR_NAME = "THERAPY_NORM_ENV"
-
-# Set to "true" if want to skip db confirmation check. Should ONLY be used for
-# deployment needs
-SKIP_AWS_DB_ENV_NAME = "SKIP_AWS_CONFIRMATION"
-
-
-class AwsEnvName(str, Enum):
-    """AWS environment name that is being used"""
-
-    DEVELOPMENT = "Dev"
-    STAGING = "Staging"
-    PRODUCTION = "Prod"
-
-
-VALID_AWS_ENV_NAMES = {v.value for v in AwsEnvName.__members__.values()}
-
-
-class DatabaseException(Exception):
-    """Create custom class for handling database exceptions"""
-
-    pass
-
 
 def confirm_aws_db_use(env_name: str) -> None:
     """Check to ensure that AWS instance should actually be used."""
     if click.confirm(f"Are you sure you want to use the AWS {env_name} database?",
                      default=False):
-        click.echo(f"***THERAPY AWS {env_name.upper()} DATABASE IN USE***")
+        click.echo(f"***THERAPY {env_name.upper()} DATABASE IN USE***")
     else:
         click.echo("Exiting.")
         sys.exit()
 
 
 class Database:
     """The database class."""
@@ -60,30 +34,45 @@
 
         :param str db_url: database endpoint URL to connect to
         :param str region_name: AWS region name to use
         """
         therapy_concepts_table = "therapy_concepts"  # default
         therapy_metadata_table = "therapy_metadata"  # default
 
-        if AWS_ENV_VAR_NAME in environ:
-            aws_env = environ[AWS_ENV_VAR_NAME]
-            if aws_env not in VALID_AWS_ENV_NAMES:
-                raise DatabaseException(f"{AWS_ENV_VAR_NAME} must be one of {VALID_AWS_ENV_NAMES}")  # noqa: E501
-
-            skip_confirmation = environ.get(SKIP_AWS_DB_ENV_NAME)
-            if (not skip_confirmation) or (skip_confirmation and skip_confirmation != "true"):  # noqa: E501
-                confirm_aws_db_use(environ[AWS_ENV_VAR_NAME])
+        if "THERAPY_NORM_PROD" in environ or "THERAPY_NORM_EB_PROD" in environ:
+            boto_params = {
+                "region_name": region_name
+            }
+            self.endpoint_url = ""
+            if "THERAPY_NORM_PROD" in environ:
+                environ["DISEASE_NORM_PROD"] = "true"
+            if "THERAPY_NORM_EB_PROD" in environ:
+                environ["DISEASE_NORM_EB_PROD"] = "true"
+            else:
+                # EB Instance should not have to confirm.
+                # This is used only for using production via CLI
+                if click.confirm("Are you sure you want to use the "
+                                 "production database?", default=False):
+                    click.echo("***THERAPY PRODUCTION DATABASE IN USE***")
+                else:
+                    click.echo("Exiting.")
+                    sys.exit()
+        elif "THERAPY_NORM_NONPROD" in environ:
+            # This is a nonprod table. Only to be used for creating backups which
+            # prod will restore. Will need to manually delete / create this table
+            # on an as needed basis.
+            therapy_concepts_table = "therapy_concepts_nonprod"
+            therapy_metadata_table = "therapy_metadata_nonprod"
 
             boto_params = {
                 "region_name": region_name
             }
 
-            if aws_env == AwsEnvName.DEVELOPMENT:
-                therapy_concepts_table = "therapy_concepts_nonprod"
-                therapy_metadata_table = "therapy_metadata_nonprod"
+            # This is used only for updating nonprod via CLI
+            confirm_aws_db_use("NONPROD")
         else:
             if db_url:
                 self.endpoint_url = db_url
             elif "THERAPY_NORM_DB_URL" in environ:
                 self.endpoint_url = environ["THERAPY_NORM_DB_URL"]
             else:
                 self.endpoint_url = "http://localhost:8000"
@@ -96,15 +85,17 @@
                 "endpoint_url": self.endpoint_url
             }
 
         self.dynamodb = boto3.resource("dynamodb", **boto_params)
         self.dynamodb_client = boto3.client("dynamodb", **boto_params)
 
         # Only create tables for local instance
-        if not {AWS_ENV_VAR_NAME} & set(environ):
+        envs_do_not_create_tables = {"THERAPY_NORM_PROD", "THERAPY_NORM_EB_PROD",
+                                     "THERAPY_NORM_NONPROD"}
+        if not set(envs_do_not_create_tables) & set(environ):
             existing_tables = self.dynamodb_client.list_tables()["TableNames"]
             self.create_therapies_table(existing_tables)
             self.create_meta_data_table(existing_tables)
 
         self.therapies = self.dynamodb.Table(therapy_concepts_table)
         self.metadata = self.dynamodb.Table(therapy_metadata_table)
         self.batch = self.therapies.batch_writer()
```

### Comparing `thera-py-0.4.0/therapy/etl/base.py` & `thera-py-0.4.dev0/therapy/etl/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 
 from pydantic import ValidationError
 import requests
 import bioversions
 from disease.query import QueryHandler as DiseaseNormalizer
 
 from therapy import APP_ROOT, ITEM_TYPES, DownloadException
-from therapy.schemas import Drug, SourceName
+from therapy.schemas import Drug
 from therapy.database import Database
-from therapy.etl.rules import Rules
 
 
 logger = logging.getLogger("therapy")
 logger.setLevel(logging.DEBUG)
 
 DEFAULT_DATA_PATH: Path = APP_ROOT / "data"
 
@@ -34,25 +33,25 @@
     Default methods are declared to provide basic functions for core source
     data-gathering phases (extraction, transformation, loading), as well
     as some common subtasks (getting most recent version, downloading data
     from an FTP server). Classes should expand or reimplement these methods as
     needed.
     """
 
-    def __init__(self, database: Database, data_path: Path = DEFAULT_DATA_PATH) -> None:
+    def __init__(self, database: Database,
+                 data_path: Path = DEFAULT_DATA_PATH) -> None:
         """Extract from sources.
 
         :param Database database: application database object
         :param Path data_path: path to app data directory
         """
-        self._name = self.__class__.__name__
+        name = self.__class__.__name__.lower()
         self.database = database
-        self._src_dir: Path = Path(data_path / self._name.lower())
+        self._src_dir: Path = Path(data_path / name)
         self._added_ids: List[str] = []
-        self._rules = Rules(SourceName(self._name))
 
     def perform_etl(self, use_existing: bool = False) -> List[str]:
         """Public-facing method to begin ETL procedures on given data.
         Returned concept IDs can be passed to Merge method for computing
         merged concepts.
 
         :param bool use_existing: if True, don't try to retrieve latest source data
@@ -84,31 +83,26 @@
         """Provide simple callback function to extract the largest file within a given
         zipfile and save it within the appropriate data directory.
         :param Path dl_path: path to temp data file
         :param Path outfile_path: path to save file within
         """
         with zipfile.ZipFile(dl_path, "r") as zip_ref:
             if len(zip_ref.filelist) > 1:
-                files = sorted(
-                    zip_ref.filelist, key=lambda z: z.file_size, reverse=True
-                )
+                files = sorted(zip_ref.filelist, key=lambda z: z.file_size,
+                               reverse=True)
                 target = files[0]
             else:
                 target = zip_ref.filelist[0]
             target.filename = outfile_path.name
             zip_ref.extract(target, path=outfile_path.parent)
         os.remove(dl_path)
 
     @staticmethod
-    def _http_download(
-        url: str,
-        outfile_path: Path,
-        headers: Optional[Dict] = None,
-        handler: Optional[Callable[[Path, Path], None]] = None,
-    ) -> None:
+    def _http_download(url: str, outfile_path: Path, headers: Optional[Dict] = None,
+                       handler: Optional[Callable[[Path, Path], None]] = None) -> None:
         """Perform HTTP download of remote data file.
         :param str url: URL to retrieve file from
         :param Path outfile_path: path to where file should be saved. Must be an actual
             Path instance rather than merely a pathlike string.
         :param Optional[Dict] headers: Any needed HTTP headers to include in request
         :param Optional[Callable[[Path, Path], None]] handler: provide if downloaded
             file requires additional action, e.g. it's a zip file.
@@ -145,17 +139,16 @@
                 ftp.cwd(host_dir)
                 with open(self._src_dir / host_fn, "wb") as fp:
                     ftp.retrbinary(f"RETR {host_fn}", fp.write)
         except ftplib.all_errors as e:
             logger.error(f"FTP download failed: {e}")
             raise Exception(e)
 
-    def _parse_version(
-        self, file_path: Path, pattern: Optional[re.Pattern] = None
-    ) -> str:
+    def _parse_version(self, file_path: Path, pattern: Optional[re.Pattern] = None
+                       ) -> str:
         """Get version number from provided file path.
 
         :param Path file_path: path to located source data file
         :param Optional[re.Pattern] pattern: regex pattern to use
         :return: source data version
         :raises: FileNotFoundError if version parsing fails
         """
@@ -163,20 +156,14 @@
             pattern = re.compile(type(self).__name__.lower() + r"_(.+)\..+")
         matches = re.match(pattern, file_path.name)
         if matches is None:
             raise FileNotFoundError
         else:
             return matches.groups()[0]
 
-    def _get_existing_files(self) -> List[Path]:
-        """Get existing source files from data directory.
-        :return: sorted list of file objects
-        """
-        return list(sorted(self._src_dir.glob(f"{self._name.lower()}_*.*")))
-
     def _extract_data(self, use_existing: bool = False) -> None:
         """Get source file from data directory.
 
         This method should ensure the source data directory exists, acquire source data,
         set the source version value, and assign the source file location to
         `self._src_file`. Child classes needing additional functionality (like setting
         up a DB cursor, or managing multiple source files) will need to reimplement
@@ -185,15 +172,15 @@
         and if the local file is out-of-date, the newest version will be acquired.
 
         :param bool use_existing: if True, don't try to fetch latest source data
         """
         self._src_dir.mkdir(exist_ok=True, parents=True)
         src_name = type(self).__name__.lower()
         if use_existing:
-            files = self._get_existing_files()
+            files = list(sorted(self._src_dir.glob(f"{src_name}_*.*")))
             if len(files) < 1:
                 raise FileNotFoundError(f"No source data found for {src_name}")
             self._src_file: Path = files[-1]
             try:
                 self._version = self._parse_version(self._src_file)
             except FileNotFoundError:
                 raise FileNotFoundError(
@@ -229,15 +216,14 @@
         Additionally, this method takes responsibility for:
             * validating record structure correctness
             * removing duplicates from list-like fields
             * removing empty fields
 
         :param Dict therapy: valid therapy object.
         """
-        therapy = self._rules.apply_rules_to_therapy(therapy)
         try:
             Drug(**therapy)
         except ValidationError as e:
             logger.error(f"Attempted to load invalid therapy: {therapy}")
             raise e
 
         concept_id = therapy["concept_id"]
@@ -248,15 +234,16 @@
                 if value is None or value == []:
                     del therapy[attr_type]
                     continue
 
                 if attr_type == "label":
                     value = value.strip()
                     therapy["label"] = value
-                    self.database.add_ref_record(value.lower(), concept_id, item_type)
+                    self.database.add_ref_record(value.lower(),
+                                                 concept_id, item_type)
                     continue
 
                 value_set = {v.strip() for v in value}
 
                 # clean up listlike symbol fields
                 if attr_type == "aliases" and "trade_names" in therapy:
                     value = list(value_set - set(therapy["trade_names"]))
@@ -278,27 +265,23 @@
                 for item in {item.lower() for item in value}:
                     self.database.add_ref_record(item, concept_id, item_type)
                 therapy[attr_type] = value
 
         # compress has_indication
         indications = therapy.get("has_indication")
         if indications:
-            therapy["has_indication"] = list(
-                {
-                    json.dumps(
-                        [
-                            ind["disease_id"],
-                            ind["disease_label"],
-                            ind.get("normalized_disease_id"),
-                            ind.get("supplemental_info"),
-                        ]
-                    )
-                    for ind in indications
-                }
-            )
+            therapy["has_indication"] = list({
+                json.dumps([
+                    ind["disease_id"],
+                    ind["disease_label"],
+                    ind.get("normalized_disease_id"),
+                    ind.get("supplemental_info")
+                ])
+                for ind in indications
+            })
         elif "has_indication" in therapy:
             del therapy["has_indication"]
 
         # handle detail fields
         approval_attrs = ("approval_ratings", "approval_year")
         for field in approval_attrs:
             if approval_attrs in therapy and therapy[field] is None:
@@ -307,15 +290,16 @@
         self.database.add_record(therapy)
         self._added_ids.append(concept_id)
 
 
 class DiseaseIndicationBase(Base):
     """Base class for sources that require disease normalization capabilities."""
 
-    def __init__(self, database: Database, data_path: Path = DEFAULT_DATA_PATH):
+    def __init__(self, database: Database,
+                 data_path: Path = DEFAULT_DATA_PATH):
         """Initialize source ETL instance.
 
         :param therapy.database.Database database: application database
         :param Path data_path: path to normalizer data directory
         """
         super().__init__(database, data_path)
         self.disease_normalizer = DiseaseNormalizer(self.database.endpoint_url)
@@ -328,15 +312,7 @@
         """
         response = self.disease_normalizer.normalize(query)
         if response.match_type > 0:
             return response.disease_descriptor.disease
         else:
             logger.warning(f"Failed to normalize disease term: {query}")
             return None
-
-
-class SourceFormatException(Exception):
-    """Raise when source data formatting is incompatible with the source transformation
-    methods: for example, if columns in a CSV file have changed.
-    """
-
-    pass
```

### Comparing `thera-py-0.4.0/therapy/etl/chembl.py` & `thera-py-0.4.dev0/therapy/etl/chembl.py`

 * *Files identical despite different names*

### Comparing `thera-py-0.4.0/therapy/etl/chemidplus.py` & `thera-py-0.4.dev0/therapy/etl/chemidplus.py`

 * *Files identical despite different names*

### Comparing `thera-py-0.4.0/therapy/etl/drugbank.py` & `thera-py-0.4.dev0/therapy/etl/drugbank.py`

 * *Files identical despite different names*

### Comparing `thera-py-0.4.0/therapy/etl/drugsatfda.py` & `thera-py-0.4.dev0/therapy/etl/drugsatfda.py`

 * *Files identical despite different names*

### Comparing `thera-py-0.4.0/therapy/etl/guidetopharmacology.py` & `thera-py-0.4.dev0/therapy/etl/guidetopharmacology.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 """Module for Guide to PHARMACOLOGY ETL methods."""
-from typing import Optional, Dict, Any, List, Union
+from typing import Optional, Dict, Any, List, Union, Tuple
 import csv
 import html
 from pathlib import Path
 import re
 
 import requests
 
 from therapy import logger
 from therapy.schemas import SourceMeta, SourceName, NamespacePrefix, ApprovalRating
-from therapy.etl.base import Base, SourceFormatException
-
-
-TAG_PATTERN = re.compile("</?[a-zA-Z]+>")
-PMID_PATTERN = re.compile(r"\[PMID:[ ]?\d+\]")
+from therapy.etl.base import Base
 
 
 class GuideToPHARMACOLOGY(Base):
     """Class for Guide to PHARMACOLOGY ETL methods."""
 
     def _download_data(self) -> None:
         """Download the latest version of Guide to PHARMACOLOGY."""
@@ -57,14 +53,15 @@
         self._src_dir.mkdir(exist_ok=True, parents=True)
         prefix = SourceName.GUIDETOPHARMACOLOGY.value.lower()
         if use_existing:
             ligands_files = list(sorted(self._src_dir.glob(f"{prefix}_ligands_*.tsv")))
             if len(ligands_files) < 1:
                 raise FileNotFoundError("No GtoPdb ligands files found")
 
+            mapping_file: Optional[Tuple] = None
             for ligands_file in ligands_files[::-1]:
                 try:
                     version = self._parse_version(
                         ligands_file,
                         re.compile(prefix + r"_ligands_(.+)\.tsv")
                     )
                 except FileNotFoundError:
@@ -72,19 +69,19 @@
                         "Unable to parse GtoPdb version value from ligands file "
                         f"located at {ligands_file.absolute().as_uri()} -- check "
                         "filename against schema defined in README: "
                         "https://github.com/cancervariants/therapy-normalization#update-sources"  # noqa: E501
                     )
                 check_mapping_file = self._src_dir / f"{prefix}_ligand_id_mapping_{version}.tsv"  # noqa: E501
                 if check_mapping_file.exists():
-                    self._version = version
+                    self.version = version
                     self._ligands_file = ligands_file
                     self._mapping_file = check_mapping_file
                     break
-            if self._mapping_file is None:
+            if mapping_file is None:
                 raise FileNotFoundError(
                     "Unable to find complete GtoPdb data set with matching version "
                     "values. Check filenames against schema defined in README: "
                     "https://github.com/cancervariants/therapy-normalization#update-sources"  # noqa: E501
                 )
         else:
             self._version = self.get_latest_version()
@@ -99,51 +96,28 @@
         """Transform Guide To PHARMACOLOGY data."""
         data: Dict[str, Any] = dict()
         self._transform_ligands(data)
         self._transform_ligand_id_mappings(data)
         for param in data.values():
             self._load_therapy(param)
 
-    @staticmethod
-    def _process_name(name: str) -> str:
-        """Remove tags from GtoP name object.
-        :param name: raw drug referent
-        :return: cleaned name (may be unchanged)
-        """
-        name = re.sub(TAG_PATTERN, "", name)
-        return name
-
     def _transform_ligands(self, data: Dict) -> None:
         """Transform ligands data file and add this data to `data`.
 
         :param dict data: Transformed data
         """
         with open(self._ligands_file, "r") as f:
             rows = csv.reader(f, delimiter="\t")
-
-            # check that file structure is the same
             next(rows)
-            if next(rows) != [
-                "Ligand ID", "Name", "Species", "Type", "Approved", "Withdrawn",
-                "Labelled", "Radioactive", "PubChem SID", "PubChem CID", "UniProt ID",
-                "Ensembl ID", "Ligand Subunit IDs", "Ligand Subunit Name",
-                "Ligand Subunit UniProt IDs", "Ligand Subunit Ensembl IDs",
-                "IUPAC name", "INN", "Synonyms", "SMILES", "InChIKey", "InChI",
-                "GtoImmuPdb", "GtoMPdb", "Antibacterial"
-            ]:
-                raise SourceFormatException(
-                    "GtoP ligands file contains missing or unrecognized columns. See "
-                    "FAQ in README for suggested resolution."
-                )
 
             for row in rows:
                 params: Dict[str, Union[List[str], str]] = {
                     "concept_id":
                         f"{NamespacePrefix.GUIDETOPHARMACOLOGY.value}:{row[0]}",
-                    "label": self._process_name(row[1]),
+                    "label": row[1],
                     "src_name": SourceName.GUIDETOPHARMACOLOGY.value
                 }
 
                 approval_rating = self._set_approval_rating(row[4], row[5])
                 if approval_rating:
                     params["approval_ratings"] = [approval_rating]
 
@@ -151,98 +125,70 @@
                 aliases = list()
                 if row[8]:
                     associated_with.append(f"{NamespacePrefix.PUBCHEMSUBSTANCE.value}:{row[8]}")  # noqa: E501
                 if row[9]:
                     associated_with.append(f"{NamespacePrefix.PUBCHEMCOMPOUND.value}:{row[9]}")  # noqa: E501
                 if row[10]:
                     associated_with.append(f"{NamespacePrefix.UNIPROT.value}:{row[10]}")
-                if row[16]:
-                    aliases.append(self._process_name(row[16]))  # IUPAC
-                if row[17]:
+                if row[11]:
+                    # IUPAC
+                    aliases.append(row[11])
+                if row[12]:
                     # International Non-proprietary Name assigned by the WHO
-                    aliases.append(self._process_name(row[17]))
-                if row[18]:
+                    aliases.append(row[12])
+                if row[13]:
                     # synonyms
-                    synonyms = row[18].split("|")
+                    synonyms = row[13].split("|")
                     for s in synonyms:
                         if "&" in s and ";" in s:
                             name_code = s[s.index("&"):s.index(";") + 1]
                             if name_code.lower() in ["&reg;", "&trade;"]:
                                 # Remove trademark symbols to allow for search
                                 s = s.replace(name_code, "")
                             s = html.unescape(s)
-                        aliases.append(self._process_name(s))
-                if row[20]:
-                    associated_with.append(f"{NamespacePrefix.INCHIKEY.value}:{row[20]}")  # noqa: E501
+                        aliases.append(s)
+                if row[15]:
+                    associated_with.append(f"{NamespacePrefix.INCHIKEY.value}:{row[15]}")  # noqa: E501
 
                 if associated_with:
                     params["associated_with"] = associated_with
                 if aliases:
                     params["aliases"] = aliases
 
                 data[params["concept_id"]] = params
 
-    @staticmethod
-    def _get_xrefs(ref: str, namespace: str) -> List[str]:
-        """Construct xrefs from raw string.
-        :param ref: raw ref value (may need to be separated)
-        :param namspace: namespace prefix to use
-        :return: List (usually with just one member) of xref IDs
-        """
-        xrefs = []
-        for split_ref in ref.split("|"):
-            xref = f"{namespace}:{split_ref}"
-            xrefs.append(xref)
-        return xrefs
-
     def _transform_ligand_id_mappings(self, data: Dict) -> None:
         """Transform ligand_id_mappings and add this data to `data`
         All ligands found in this file should already be in data
 
         :param dict data: Transformed data
         """
         with open(self._mapping_file.absolute(), "r") as f:
             rows = csv.reader(f, delimiter="\t")
-            next(rows)
-            if next(rows) != [
-                "Ligand id", "Name", "Species", "Type", "PubChem SID", "PubChem CID",
-                "ChEMBl ID", "Chebi ID", "UniProt id", "Ensembl ID", "IUPAC name",
-                "INN", "CAS", "DrugBank ID", "Drug Central ID"
-            ]:
-                raise SourceFormatException(
-                    "GtoP ligand mapping file contains missing or unrecognized "
-                    "columns. See FAQ in README for suggested resolution."
-                )
-
             for row in rows:
                 concept_id = f"{NamespacePrefix.GUIDETOPHARMACOLOGY.value}:{row[0]}"
 
                 if concept_id not in data:
                     logger.debug(f"{concept_id} not in ligands")
                     continue
                 params = data[concept_id]
                 xrefs = list()
                 associated_with = params.get("associated_with", [])
                 if row[6]:
-                    xrefs += self._get_xrefs(row[6], NamespacePrefix.CHEMBL.value)
+                    xrefs.append(f"{NamespacePrefix.CHEMBL.value}:{row[6]}")
                 if row[7]:
-                    # CHEBI IDs are already namespaced
+                    # CHEBI
                     associated_with.append(row[7])
-                if row[8]:
-                    associated_with += self._get_xrefs(
-                        row[8], NamespacePrefix.UNIPROT.value
-                    )
+                if row[11]:
+                    xrefs.append(f"{NamespacePrefix.CASREGISTRY.value}:{row[11]}")
                 if row[12]:
-                    xrefs += self._get_xrefs(row[12], NamespacePrefix.CASREGISTRY.value)
+                    xrefs.append(f"{NamespacePrefix.DRUGBANK.value}:{row[12]}")
                 if row[13]:
-                    xrefs += self._get_xrefs(row[13], NamespacePrefix.DRUGBANK.value)
-                if row[14]:
-                    associated_with += self._get_xrefs(
-                        row[14], NamespacePrefix.DRUGCENTRAL.value
-                    )
+                    associated_with.append(f"{NamespacePrefix.DRUGCENTRAL.value}:{row[13]}")  # noqa: E501
+
                 if xrefs:
                     params["xrefs"] = xrefs
                 if associated_with:
                     params["associated_with"] = associated_with
 
     def _set_approval_rating(self, approved: str,
                              withdrawn: str) -> Optional[str]:
```

### Comparing `thera-py-0.4.0/therapy/etl/hemonc.py` & `thera-py-0.4.dev0/therapy/etl/hemonc.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                         "https://github.com/cancervariants/therapy-normalization#update-sources"  # noqa: E501
                     )
                 other_files = (
                     self._src_dir / f"hemonc_rels_{version}.csv",
                     self._src_dir / f"hemonc_synonyms_{version}.csv"
                 )
                 if other_files[0].exists() and other_files[1].exists():
-                    self._version = version
+                    self.version = version
                     src_files = (
                         concepts_file,
                         other_files[0],
                         other_files[1]
                     )
                     break
             if src_files is None:
```

### Comparing `thera-py-0.4.0/therapy/etl/merge.py` & `thera-py-0.4.dev0/therapy/etl/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,23 @@
 
     def create_merged_concepts(self, record_ids: Set[str]) -> None:
         """Create concept groups, generate merged concept records, and update database.
 
         :param Set[str] record_ids: concept identifiers from which groups should be
             generated.
         """
-        self._create_record_id_sets(record_ids)
+        logger.info("Generating record ID sets...")
+        start = timer()
+        for record_id in record_ids:
+            new_group = self._create_record_id_set(record_id)
+            if new_group:
+                for concept_id in new_group:
+                    self._groups[concept_id] = new_group
+        end = timer()
+        logger.debug(f"Built record ID sets in {end - start} seconds")
 
         # don't create separate records for single-member groups
         self._groups = {k: v for k, v in self._groups.items() if len(v) > 1}
 
         logger.info("Creating merged records and updating database...")
         uploaded_ids = set()
         start = timer()
@@ -74,15 +82,16 @@
         """Rx Norm provides brand references back to original therapy concepts.  This
         routine checks whether an ID from a concept group requires an additional
         dereference to obtain the original RxNorm record.
 
         :param str record_id: RxNorm concept ID to check
         :return: concept ID for RxNorm record if successful, None otherwise
         """
-        brand_lookup = self.database.get_records_by_type(record_id, "rx_brand")
+        brand_lookup = self.database.get_records_by_type(record_id,
+                                                         "rx_brand")
         n = len(brand_lookup)
         if n == 1:
             lookup_id = brand_lookup[0]["concept_id"]
             db_record = self.database.get_record_by_id(lookup_id,
                                                        False)
             if db_record:
                 return db_record["concept_id"]
@@ -140,17 +149,16 @@
                     drugsatfda_ref = self._get_drugsatfda_from_unii(ref)
                     if drugsatfda_ref:
                         drugsatfda_refs.add(drugsatfda_ref)
             self._unii_to_drugsatfda[unii] = drugsatfda_refs
             xrefs |= drugsatfda_refs
         return xrefs
 
-    def _create_record_id_set(
-        self, record_id: str, observed_id_set: Optional[Set] = None
-    ) -> Set[str]:
+    def _create_record_id_set(self, record_id: str,
+                              observed_id_set: Set = None) -> Set[str]:
         """Create concept ID group for an individual record ID.
 
         :param str record_id: concept ID for record to build group from
         :return: set of related identifiers pertaining to a common concept.
         """
         if observed_id_set is None:
             observed_id_set = set()
@@ -179,29 +187,14 @@
         if not local_id_set:
             return observed_id_set | {db_record["concept_id"]}
         merged_id_set = {record_id} | observed_id_set
         for local_record_id in local_id_set - observed_id_set:
             merged_id_set |= self._create_record_id_set(local_record_id, merged_id_set)
         return merged_id_set
 
-    def _create_record_id_sets(self, record_ids: Set[str]) -> None:
-        """Update self._groups with normalized concept groups.
-        :param Set[str] record_ids: concept identifiers from which groups should be
-            generated.
-        """
-        logger.info("Generating record ID sets...")
-        start = timer()
-        for record_id in record_ids:
-            new_group = self._create_record_id_set(record_id)
-            if new_group:
-                for concept_id in new_group:
-                    self._groups[concept_id] = new_group
-        end = timer()
-        logger.debug(f"Built record ID sets in {end - start} seconds")
-
     def _generate_merged_record(self, record_id_set: Set[str]) -> Dict:
         """Generate merged record from provided concept ID group.
         Where attributes are 'set-like', they should be combined, and where
         they are 'scalar-like', assign from the highest-priority source where
         that attribute is not None.
 
         Uses the SourcePriority schema to define source priority.
```

### Comparing `thera-py-0.4.0/therapy/etl/ncit.py` & `thera-py-0.4.dev0/therapy/etl/ncit.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,17 @@
                                        f"{node.P207.first()}")
             if node.P210:
                 xrefs.append(f"{NamespacePrefix.CASREGISTRY.value}:"
                              f"{node.P210.first()}")
             if node.P319:
                 associated_with.append(f"{NamespacePrefix.UNII.value}:"
                                        f"{node.P319.first()}")
+            if node.P320:
+                associated_with.append(f"{NamespacePrefix.ISO.value}:"
+                                       f"{node.P320.first()}")
             if node.P368:
                 iri = node.P368.first()
                 if ":" in iri:
                     iri = iri.split(":")[1]
                 associated_with.append(f"{NamespacePrefix.CHEBI.value}:{iri}")
             params: RecordParams = {  # type: ignore
                 "concept_id": concept_id,
```

### Comparing `thera-py-0.4.0/therapy/etl/rxnorm.py` & `thera-py-0.4.dev0/therapy/etl/rxnorm.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 from os import environ, remove
 from typing import List, Dict
 from pathlib import Path
 
 import yaml
 import bioversions
 from boto3.dynamodb.table import BatchWriter
+import requests
 
 from therapy import DownloadException, XREF_SOURCES, ASSOC_WITH_SOURCES, ITEM_TYPES
-from therapy.schemas import SourceName, NamespacePrefix, SourceMeta, ApprovalRating, \
-    RecordParams
+from therapy.schemas import SourceName, NamespacePrefix, SourceMeta, Drug, \
+    ApprovalRating, RecordParams
 from therapy.etl.base import Base
 
 logger = logging.getLogger("therapy")
 logger.setLevel(logging.DEBUG)
 
 # Designated Alias, Designated Syn, Tall Man Syn, Machine permutation
 # Generic Drug Name, Designated Preferred Name, Preferred Entry Term,
@@ -85,25 +86,30 @@
             logger.error("Could not find RXNORM_API_KEY in environment variables.")
             raise DownloadException("RXNORM_API_KEY not found.")
 
         url = bioversions.resolve("rxnorm").homepage
         if not url:
             raise DownloadException("Could not resolve RxNorm homepage")
 
-        self._http_download(
-            f"https://uts-ws.nlm.nih.gov/download?url={url}&apiKey={api_key}",
-            self._src_dir,
-            handler=self._zip_handler
-        )
-
-    def _get_existing_files(self) -> List[Path]:
-        """Get existing source RRF files from data directory.
-        :return: sorted list of file objects
-        """
-        return list(sorted(self._src_dir.glob("rxnorm_*.RRF")))
+        tgt_data = {"apikey": api_key}
+        headers = {"Content-Type": "application/x-www-form-urlencoded"}
+        api_url = "https://utslogin.nlm.nih.gov/cas/v1/api-key"
+        tgt_r = requests.post(api_url,
+                              data=tgt_data, headers=headers)
+        tgt_matches = re.findall(r'https://.+(TGT.+)" m', tgt_r.text)
+        if not tgt_matches:
+            raise DownloadException("Unable to retrieve TGT")
+        tgt_value = tgt_matches[0]
+
+        st_data = {"service": url}
+        st_url = f"https://utslogin.nlm.nih.gov/cas/v1/tickets/{tgt_value}"
+        st_r = requests.post(st_url, data=st_data, headers=headers)
+
+        self._http_download(f"{url}?ticket={st_r.text}", self._src_dir,
+                            handler=self._zip_handler)
 
     def _extract_data(self, use_existing: bool = False) -> None:
         """Get source files from RxNorm data directory.
         This class expects a file named `rxnorm_<version>.RRF` and a file named
         `rxnorm_drug_forms_<version>.yaml`. This method will download and
         generate them if they are unavailable.
 
@@ -165,14 +171,15 @@
 
                         params = {"concept_id": value["concept_id"]}
 
                         for field in list(ITEM_TYPES.keys()) + ["approval_ratings"]:
                             field_value = value.get(field)
                             if field_value:
                                 params[field] = field_value
+                        assert Drug(**params)
                         self._load_therapy(params)
 
     def _get_brands(self, row: List, ingredient_brands: Dict) -> None:
         """Add ingredient and brand to ingredient_brands.
 
         :param List row: A row in the RxNorm data file.
         :param Dict ingredient_brands: Store brands for each ingredient
@@ -181,17 +188,18 @@
         term = row[14]
         ingredients_brand = \
             re.sub(r"(\d*)(\d*\.)?\d+ (MG|UNT|ML)?(/(ML|HR|MG))?",
                    "", term)
         brand = term.split("[")[-1].split("]")[0]
         ingredients = ingredients_brand.replace(f"[{brand}]", "")
         if "/" in ingredients:
-            ingredients_list = ingredients.split("/")
-            for ingredient in ingredients_list:
-                self._add_term(ingredient_brands, brand, ingredient.strip())
+            ingredients = ingredients.split("/")
+            for ingredient in ingredients:
+                self._add_term(ingredient_brands, brand,
+                               ingredient.strip())
         else:
             self._add_term(ingredient_brands, brand,
                            ingredients.strip())
 
     def _get_trade_names(self, value: Dict, precise_ingredient: Dict,
                          ingredient_brands: Dict, sbdfs: Dict) -> None:
         """Get trade names for a given ingredient.
@@ -299,29 +307,28 @@
     def _add_xref_assoc(self, params: Dict, row: List) -> None:
         """Add xref or associated_with to therapy.
 
         :param Dict params: A transformed therapy record.
         :param List row: A row in the RxNorm data file.
         """
         ref = row[11]
-        lui = row[13]
-        if ref and lui != "NOCODE":
+        if ref:
             if ref == "MTHSPL":
                 xref_assoc = "UNII"
             else:
                 xref_assoc = row[11].upper()
 
             if xref_assoc in XREF_SOURCES:
                 source_id =\
-                    f"{NamespacePrefix[xref_assoc].value}:{lui}"
+                    f"{NamespacePrefix[xref_assoc].value}:{row[13]}"
                 if source_id != params["concept_id"]:
                     # Sometimes concept_id is included in the source field
                     self._add_term(params, source_id, "xrefs")
             elif xref_assoc in ASSOC_WITH_SOURCES:
-                source_id = f"{NamespacePrefix[xref_assoc].value}:{lui}"
+                source_id = f"{NamespacePrefix[xref_assoc].value}:{row[13]}"
                 self._add_term(params, source_id, "associated_with")
             else:
                 logger.info(f"{xref_assoc} not in NameSpacePrefix.")
 
     def _load_meta(self) -> None:
         """Add RxNorm metadata."""
         meta = SourceMeta(
```

### Comparing `thera-py-0.4.0/therapy/etl/wikidata.py` & `thera-py-0.4.dev0/therapy/etl/wikidata.py`

 * *Files identical despite different names*

### Comparing `thera-py-0.4.0/therapy/main.py` & `thera-py-0.4.dev0/therapy/main.py`

 * *Files identical despite different names*

### Comparing `thera-py-0.4.0/therapy/query.py` & `thera-py-0.4.dev0/therapy/query.py`

 * *Files identical despite different names*

### Comparing `thera-py-0.4.0/therapy/schemas.py` & `thera-py-0.4.dev0/therapy/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module contains data models for representing VICC therapy records."""
 from typing import List, Optional, Dict, Union, Any, Type, Set
 from enum import Enum, IntEnum
 from datetime import datetime
 
 from ga4gh.vrsatile.pydantic.core_models import CURIE
-from ga4gh.vrsatile.pydantic.vrsatile_models import TherapeuticDescriptor
+from ga4gh.vrsatile.pydantic.vrsatile_models import DiseaseDescriptor, \
+    TherapeuticDescriptor
 from pydantic import BaseModel, StrictBool
 
 from therapy.version import __version__
 
 # Working structure for object in preparation for upload to DB
 RecordParams = Dict[str, Union[List, Set, str, Dict[str, Any]]]
 
@@ -224,41 +225,52 @@
     GUIDETOPHARMACOLOGY = "GuideToPHARMACOLOGY"
 
 
 class NamespacePrefix(Enum):
     """Define string constraints for namespace prefixes on concept IDs."""
 
     ATC = "atc"  # Anatomical Therapeutic Chemical Classification System
+    BINDINGDB = "bindingdb"
     CHEBI = "CHEBI"
     CHEMBL = "chembl"
     CHEMIDPLUS = "chemidplus"
     CASREGISTRY = CHEMIDPLUS
+    CHEMSPIDER = "chemspider"
     CVX = "cvx"  # Vaccines Administered
     DRUGBANK = "drugbank"
     DRUGCENTRAL = "drugcentral"
     DRUGSATFDA_ANDA = "drugsatfda.anda"
     DRUGSATFDA_NDA = "drugsatfda.nda"
     HEMONC = "hemonc"
     INCHIKEY = "inchikey"
+    ISO = "iso"
+    IUPHAR = "iuphar"
     IUPHAR_LIGAND = "iuphar.ligand"
     GUIDETOPHARMACOLOGY = IUPHAR_LIGAND
+    KEGGCOMPOUND = "kegg.compound"
+    KEGGDRUG = "kegg.drug"
     MMSL = "mmsl"  # Multum MediSource Lexicon
     MSH = "mesh"  # Medical Subject Headings
+    MTHCMSFRF = "mthcmsfrf"  # CMS Formulary Reference File
     NCIT = "ncit"
     NDC = "ndc"  # National Drug Code
+    PDB = "pdb"
+    PHARMGKB = "pharmgkb.drug"
     PUBCHEMCOMPOUND = "pubchem.compound"
     PUBCHEMSUBSTANCE = "pubchem.substance"
     RXNORM = "rxcui"
     SPL = "spl"  # Structured Product Labeling
+    THERAPEUTICTARGETSDB = "ttd"
     UMLS = "umls"
     UNII = "unii"
     UNIPROT = "uniprot"
     USP = "usp"  # USP Compendial Nomenclature
     VANDF = "vandf"  # Veterans Health Administration National Drug File
     WIKIDATA = "wikidata"
+    ZINC = "zinc"
 
 
 class DataLicenseAttributes(BaseModel):
     """Define constraints for data license attributes."""
 
     non_commercial: StrictBool
     share_alike: StrictBool
@@ -388,14 +400,24 @@
                         "share_alike": True,
                         "attribution": True
                     }
                 },
             }
 
 
+class ApprovalRatingValue(BaseModel):
+    """VOD Extension class for regulatory approval rating/indication
+    value attributes.
+    """
+
+    approval_ratings: Optional[List[ApprovalRating]]
+    approval_year: Optional[List[str]]
+    has_indication: Optional[List[DiseaseDescriptor]]
+
+
 class ServiceMeta(BaseModel):
     """Metadata regarding the therapy-normalization service."""
 
     name = "thera-py"
     version = __version__
     response_datetime: datetime
     url = "https://github.com/cancervariants/therapy-normalization"
```

