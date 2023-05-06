# Comparing `tmp/forust-0.2.3.tar.gz` & `tmp/forust-0.2.4.tar.gz`

## Comparing `forust-0.2.3.tar` & `forust-0.2.4.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 forust-0.2.3/local_dependencies/forust-ml/Cargo.toml
--rw-r--r--   0     1001      123     5608 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      262 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/.gitignore
--rw-r--r--   0     1001      123      320 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/.pre-commit-config.yaml
--rw-r--r--   0     1001      123    11341 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/LICENSE
--rw-r--r--   0     1001      123    11318 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/README.md
--rw-r--r--   0     1001      123     4100 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/benches/forust_benchmarks.rs
--rw-r--r--   0     1001      123   456826 2023-05-01 02:09:09.000000 forust-0.2.3/local_dependencies/forust-ml/dist/forust-0.2.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
--rw-r--r--   0     1001      123   749549 2023-05-01 02:08:24.000000 forust-0.2.3/local_dependencies/forust-ml/dist/forust-0.2.3.tar.gz
--rw-r--r--   0     1001      123    16121 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/resources/pdp_plot_age.png
--rw-r--r--   0     1001      123    10758 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
--rw-r--r--   0     1001      123    57018 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/resources/titanic.csv
--rw-r--r--   0     1001      123   655700 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/resources/tree-image-crop.png
--rw-r--r--   0     1001      123     2556 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/rs-example.md
--rwxr-xr-x   0     1001      123     1137 2023-05-01 02:09:18.000000 forust-0.2.3/local_dependencies/forust-ml/run-maturin-action.sh
--rw-r--r--   0     1001      123     1179 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/scripts/make_resources.py
--rw-r--r--   0     1001      123       53 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/scripts/run-python-tests.ps1
--rw-r--r--   0     1001      123       53 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/scripts/run-python-tests.sh
--rw-r--r--   0     1001      123     5610 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/binning.rs
--rw-r--r--   0     1001      123      248 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/constraints.rs
--rw-r--r--   0     1001      123     8384 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/data.rs
--rw-r--r--   0     1001      123      585 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/errors.rs
--rw-r--r--   0     1001      123    23141 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/gradientbooster.rs
--rw-r--r--   0     1001      123     9052 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/histogram.rs
--rw-r--r--   0     1001      123      318 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/lib.rs
--rw-r--r--   0     1001      123     5958 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/node.rs
--rw-r--r--   0     1001      123     4125 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/objective.rs
--rw-r--r--   0     1001      123     3542 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/partial_dependence.rs
--rw-r--r--   0     1001      123    27131 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/splitter.rs
--rw-r--r--   0     1001      123    17335 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/tree.rs
--rw-r--r--   0     1001      123    28906 2023-05-01 02:04:47.000000 forust-0.2.3/local_dependencies/forust-ml/src/utils.rs
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.3/Cargo.toml
--rw-r--r--   0     1001      123      685 2023-05-01 02:04:47.000000 forust-0.2.3/.gitignore
--rw-r--r--   0     1001      123    11318 2023-05-01 02:05:18.000000 forust-0.2.3/README.md
--rw-r--r--   0     1001      123    17331 2023-05-01 02:04:47.000000 forust-0.2.3/forust/__init__.py
--rw-r--r--   0     1001      123      785 2023-05-01 02:04:47.000000 forust-0.2.3/pyproject.toml
--rw-r--r--   0     1001      123     7353 2023-05-01 02:04:47.000000 forust-0.2.3/scratch.py
--rw-r--r--   0     1001      123     9225 2023-05-01 02:04:47.000000 forust-0.2.3/src/lib.rs
--rw-r--r--   0     1001      123    11077 2023-05-01 02:04:47.000000 forust-0.2.3/tests/test_booster.py
--rw-r--r--   0     1001      123    11341 2023-05-01 02:05:18.000000 forust-0.2.3/LICENSE
--rw-r--r--   0     1001      123    11318 2023-05-01 02:05:18.000000 forust-0.2.3/README.md
--rw-r--r--   0        0        0    12102 1970-01-01 00:00:00.000000 forust-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 forust-0.2.4/local_dependencies/forust-ml/Cargo.toml
+-rw-r--r--   0      501       20     5608 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      262 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/.gitignore
+-rw-r--r--   0      501       20      320 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/.pre-commit-config.yaml
+-rw-r--r--   0      501       20    11341 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/LICENSE
+-rw-r--r--   0      501       20    11917 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/README.md
+-rw-r--r--   0      501       20     4100 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/benches/forust_benchmarks.rs
+-rw-r--r--   0      501       20   416799 2023-05-06 22:15:57.000000 forust-0.2.4/local_dependencies/forust-ml/dist/forust-0.2.4-cp310-cp310-macosx_10_7_x86_64.whl
+-rw-r--r--   0      501       20   751559 2023-05-06 22:14:53.000000 forust-0.2.4/local_dependencies/forust-ml/dist/forust-0.2.4.tar.gz
+-rw-r--r--   0      501       20    16121 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/resources/pdp_plot_age.png
+-rw-r--r--   0      501       20    10758 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
+-rw-r--r--   0      501       20    57018 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/resources/titanic.csv
+-rw-r--r--   0      501       20   655700 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/resources/tree-image-crop.png
+-rw-r--r--   0      501       20     2556 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/rs-example.md
+-rw-r--r--   0      501       20     1179 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/scripts/make_resources.py
+-rw-r--r--   0      501       20       53 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/scripts/run-python-tests.ps1
+-rw-r--r--   0      501       20       53 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/scripts/run-python-tests.sh
+-rw-r--r--   0      501       20     5610 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/binning.rs
+-rw-r--r--   0      501       20      248 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/constraints.rs
+-rw-r--r--   0      501       20     8384 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/data.rs
+-rw-r--r--   0      501       20      585 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/errors.rs
+-rw-r--r--   0      501       20    24537 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/gradientbooster.rs
+-rw-r--r--   0      501       20     9357 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/histogram.rs
+-rw-r--r--   0      501       20      318 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/lib.rs
+-rw-r--r--   0      501       20     6060 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/node.rs
+-rw-r--r--   0      501       20     4125 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/objective.rs
+-rw-r--r--   0      501       20     4054 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/partial_dependence.rs
+-rw-r--r--   0      501       20    34423 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/splitter.rs
+-rw-r--r--   0      501       20    17831 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/tree.rs
+-rw-r--r--   0      501       20    29472 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/utils.rs
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.4/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-05-06 22:11:27.000000 forust-0.2.4/.gitignore
+-rw-r--r--   0      501       20    11917 2023-05-06 22:12:03.000000 forust-0.2.4/README.md
+-rw-r--r--   0      501       20    18185 2023-05-06 22:11:27.000000 forust-0.2.4/forust/__init__.py
+-rw-r--r--   0      501       20      785 2023-05-06 22:11:27.000000 forust-0.2.4/pyproject.toml
+-rw-r--r--   0      501       20     7353 2023-05-06 22:11:27.000000 forust-0.2.4/scratch.py
+-rw-r--r--   0      501       20     9433 2023-05-06 22:11:27.000000 forust-0.2.4/src/lib.rs
+-rw-r--r--   0      501       20    12380 2023-05-06 22:11:27.000000 forust-0.2.4/tests/test_booster.py
+-rw-r--r--   0      501       20    11341 2023-05-06 22:12:03.000000 forust-0.2.4/LICENSE
+-rw-r--r--   0      501       20    11917 2023-05-06 22:12:03.000000 forust-0.2.4/README.md
+-rw-r--r--   0        0        0    12701 1970-01-01 00:00:00.000000 forust-0.2.4/PKG-INFO
```

### Comparing `forust-0.2.3/local_dependencies/forust-ml/Cargo.toml` & `forust-0.2.4/local_dependencies/forust-ml/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "forust-ml"
-version = "0.2.3"
+version = "0.2.4"
 edition = "2021"
 authors = ["James Inlow <james.d.inlow@gmail.com>"]
 homepage = "https://github.com/jinlow/forust"
 description = "A lightweight gradient boosting implementation in Rust."
 license-file = "LICENSE"
 readme = "README.md"
 repository = "https://github.com/jinlow/forust"
```

### Comparing `forust-0.2.3/local_dependencies/forust-ml/.github/workflows/CI.yml` & `forust-0.2.4/local_dependencies/forust-ml/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/local_dependencies/forust-ml/LICENSE` & `forust-0.2.4/local_dependencies/forust-ml/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/local_dependencies/forust-ml/README.md` & `forust-0.2.4/local_dependencies/forust-ml/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.3"
+forust-ml = "0.2.4"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -56,21 +56,22 @@
  - `base_score` ***(float, optional)***: The initial prediction value of the model. Defaults to 0.5.
  - `nbins` ***(int, optional)***: Number of bins to calculate to partition the data. Setting this to
     a smaller number, will result in faster training time, while potentially sacrificing
     accuracy. If there are more bins, than unique values in a column, all unique values
     will be used. Defaults to 256.
  - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
     with this model? Defaults to `True`.
- - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. Defaults to `True`.
+ - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. If `create_missing_branch` is set to `True` having this parameter be set to `True` will result in the missing branch further split, if this parameter is `False` then in that case the missing branch will always be a terminal node. Defaults to `True`.
  - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
  - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
       training a tree. Defaults to 1.0, meaning all data is used for training.
  - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
       algorithm. Defaults to 0.
  - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
+ - `create_missing_branch` ***(bool, optional)***: An experimental parameter, that if `True`, will create a separate branch for missing, creating a ternary tree, the missing node will be given the same weight value as the parent node. If this parameter is `False`, missing will be sent down either the left or right branch, creating a binary tree. Defaults to `False`.
 
 ### Training and Predicting
 
 Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
 In the case of this example, the predictions are the log odds of a given record being 1.
 
 ```python
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.3" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.4" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -45,15 +45,18 @@
 time, while potentially sacrificing accuracy. If there are more bins, than
 unique values in a column, all unique values will be used. Defaults to 256. -
 `parallel` ***(bool, optional)***: Should multiple cores be used when training
 and predicting with this model? Defaults to `True`. - `allow_missing_splits`
 ***(bool, optional)***: Allow for splits to be made such that all missing
 values go down one branch, and all non-missing values go down the other, if
 this results in the greatest reduction of loss. If this is false, splits will
-only be made on non missing values. Defaults to `True`. -
+only be made on non missing values. If `create_missing_branch` is set to `True`
+having this parameter be set to `True` will result in the missing branch
+further split, if this parameter is `False` then in that case the missing
+branch will always be a terminal node. Defaults to `True`. -
 `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are
 used to enforce a specific relationship between the training features and the
 target variable. A dictionary should be provided where the keys are the feature
 index value if the model will be fit on a numpy array, or a feature name if it
 will be fit on a pandas Dataframe. The values of the dictionary should be an
 integer value of -1, 1, or 0 to specify the relationship that should be
 estimated between the respective feature and the target variable. Use a value
@@ -62,51 +65,55 @@
 will not have any constraint applied. If `None` is passed no constraints will
 be enforced on any variable. Defaults to `None`. - `subsample` ***(float,
 optional)***: Percent of records to randomly sample at each iteration when
 training a tree. Defaults to 1.0, meaning all data is used for training. -
 `seed` ***(integer, optional)***: Integer value used to seed any randomness
 used in the algorithm. Defaults to 0. - `missing` ***(float, optional)***:
 Value to consider missing, when training and predicting with the booster.
-Defaults to `np.nan`. ### Training and Predicting Once, the booster has been
-initialized, it can be fit on a provided dataset, and performance field. After
-fitting, the model can be used to predict on a dataset. In the case of this
-example, the predictions are the log odds of a given record being 1. ```python
-# Small example dataset from seaborn import load_dataset df = load_dataset
-("titanic") X = df.select_dtypes("number").drop(columns=["survived"]) y = df
-["survived"] # Initialize a booster with defaults. from forust import
-GradientBooster model = GradientBooster(objective_type="LogLoss") model.fit(X,
-y) # Predict on data model.predict(X.head()) # array([-1.94919663, 2.25863229,
-0.32963671, 2.48732194, -3.00371813]) # predict contributions
-model.predict_contributions(X.head()) # array([[-0.63014213, 0.33880048, -
-0.16520798, -0.07798772, -0.85083578, # -1.07720813], # [ 1.05406709,
-0.08825999, 0.21662544, -0.12083538, 0.35209258, # -1.07720813], ``` The `fit`
-method accepts the following arguments. - `X` ***(FrameLike)***: Either a
-pandas DataFrame, or a 2 dimensional numpy array, with numeric data. - `y` ***
-(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If
-"LogLoss" was the objective type specified, then this should only contain 1 or
-0 values, where 1 is the positive class being predicted. If "SquaredLoss" is
-the objective type, then any continuous variable can be provided. -
-`sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use
-when training the model. If None is passed, a weight of 1 will be used for
-every record. Defaults to None. The predict method accepts the following
-arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2
-dimensional numpy array, with numeric data. - `parallel` ***(Optional[bool],
-optional)***: Optionally specify if the predict function should run in parallel
-on multiple threads. If `None` is passed, the `parallel` attribute of the
-booster will be used. Defaults to `None`. The `predict_contributions` method
-will predict with the fitted booster on new data, returning the feature
-contribution matrix. The last column is the bias term. - `X` ***(FrameLike)***:
+Defaults to `np.nan`. - `create_missing_branch` ***(bool, optional)***: An
+experimental parameter, that if `True`, will create a separate branch for
+missing, creating a ternary tree, the missing node will be given the same
+weight value as the parent node. If this parameter is `False`, missing will be
+sent down either the left or right branch, creating a binary tree. Defaults to
+`False`. ### Training and Predicting Once, the booster has been initialized, it
+can be fit on a provided dataset, and performance field. After fitting, the
+model can be used to predict on a dataset. In the case of this example, the
+predictions are the log odds of a given record being 1. ```python # Small
+example dataset from seaborn import load_dataset df = load_dataset("titanic") X
+= df.select_dtypes("number").drop(columns=["survived"]) y = df["survived"] #
+Initialize a booster with defaults. from forust import GradientBooster model =
+GradientBooster(objective_type="LogLoss") model.fit(X, y) # Predict on data
+model.predict(X.head()) # array([-1.94919663, 2.25863229, 0.32963671,
+2.48732194, -3.00371813]) # predict contributions model.predict_contributions
+(X.head()) # array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -
+0.85083578, # -1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -
+0.12083538, 0.35209258, # -1.07720813], ``` The `fit` method accepts the
+following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2
+dimensional numpy array, with numeric data. - `y` ***(ArrayLike)***: Either a
+pandas Series, or a 1 dimensional numpy array. If "LogLoss" was the objective
+type specified, then this should only contain 1 or 0 values, where 1 is the
+positive class being predicted. If "SquaredLoss" is the objective type, then
+any continuous variable can be provided. - `sample_weight` ***(Optional
+[ArrayLike], optional)***: Instance weights to use when training the model. If
+None is passed, a weight of 1 will be used for every record. Defaults to None.
+The predict method accepts the following arguments. - `X` ***(FrameLike)***:
 Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
 `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
 function should run in parallel on multiple threads. If `None` is passed, the
-`parallel` attribute of the booster will be used. Defaults to `None`. ###
-Inspecting the Model Once the booster has been fit, each individual tree
-structure can be retrieved in text form, using the `text_dump` method. This
-method returns a list, the same length as the number of trees in the model.
-```python model.text_dump()[0] # 0:[0 < 3]
+`parallel` attribute of the booster will be used. Defaults to `None`. The
+`predict_contributions` method will predict with the fitted booster on new
+data, returning the feature contribution matrix. The last column is the bias
+term. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional
+numpy array, with numeric data. - `parallel` ***(Optional[bool], optional)***:
+Optionally specify if the predict function should run in parallel on multiple
+threads. If `None` is passed, the `parallel` attribute of the booster will be
+used. Defaults to `None`. ### Inspecting the Model Once the booster has been
+fit, each individual tree structure can be retrieved in text form, using the
+`text_dump` method. This method returns a list, the same length as the number
+of trees in the model. ```python model.text_dump()[0] # 0:[0 < 3]
 yes=1,no=2,missing=2,gain=91.50833,cover=209.388307 # 1:[4 < 13.7917]
 yes=3,no=4,missing=4,gain=28.185467,cover=94.00148 # 3:[1 < 18]
 yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348 # 7:[1 < 17]
 yes=15,no=16,missing=16,gain=0.691266,cover=0.705011 # 15:leaf=-
 0.15120,cover=0.23500 # 16:leaf=0.154097,cover=0.470007 ``` The `json_dump`
 method performs the same action, but returns the model as a json representation
 rather than a text string. To see an estimate for how a given feature is used
```

### Comparing `forust-0.2.3/local_dependencies/forust-ml/benches/forust_benchmarks.rs` & `forust-0.2.4/local_dependencies/forust-ml/benches/forust_benchmarks.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/local_dependencies/forust-ml/resources/pdp_plot_age.png` & `forust-0.2.4/local_dependencies/forust-ml/resources/pdp_plot_age.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png` & `forust-0.2.4/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/local_dependencies/forust-ml/resources/titanic.csv` & `forust-0.2.4/local_dependencies/forust-ml/resources/titanic.csv`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/local_dependencies/forust-ml/resources/tree-image-crop.png` & `forust-0.2.4/local_dependencies/forust-ml/resources/tree-image-crop.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/local_dependencies/forust-ml/rs-example.md` & `forust-0.2.4/local_dependencies/forust-ml/rs-example.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## A Complete Rust Example
 
 To run this example, add the following code to your `Cargo.toml` file.
 ```toml
 [dependencies]
-forust-ml = "0.2.3"
+forust-ml = "0.2.4"
 polars = "0.24"
 reqwest = { version = "0.11", features = ["blocking"] }
 ```
 
 The following is a runable example using `polars` for data processing. The actual data manipulation can be performed with any tool, the only vital part, is the data be in column major format.
 ```rust
 use forust_ml::{GradientBooster, Matrix};
```

### Comparing `forust-0.2.3/local_dependencies/forust-ml/scripts/make_resources.py` & `forust-0.2.4/local_dependencies/forust-ml/scripts/make_resources.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/local_dependencies/forust-ml/src/binning.rs` & `forust-0.2.4/local_dependencies/forust-ml/src/binning.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/local_dependencies/forust-ml/src/data.rs` & `forust-0.2.4/local_dependencies/forust-ml/src/data.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/local_dependencies/forust-ml/src/errors.rs` & `forust-0.2.4/local_dependencies/forust-ml/src/errors.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/local_dependencies/forust-ml/src/gradientbooster.rs` & `forust-0.2.4/local_dependencies/forust-ml/src/gradientbooster.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use crate::binning::bin_matrix;
 use crate::constraints::ConstraintMap;
 use crate::data::Matrix;
 use crate::errors::ForustError;
 use crate::objective::{gradient_hessian_callables, ObjectiveType};
-use crate::splitter::MissingImputerSplitter;
+use crate::splitter::{MissingBranchSplitter, MissingImputerSplitter, Splitter};
 use crate::tree::Tree;
 use rand::rngs::StdRng;
 use rand::SeedableRng;
 use rayon::prelude::*;
 use serde::{Deserialize, Deserializer, Serialize};
 use std::collections::HashMap;
 use std::fs;
@@ -54,14 +54,15 @@
     pub parallel: bool,
     pub allow_missing_splits: bool,
     pub monotone_constraints: Option<ConstraintMap>,
     pub subsample: f32,
     pub seed: u64,
     #[serde(deserialize_with = "parse_missing")]
     pub missing: f64,
+    pub create_missing_branch: bool,
     pub trees: Vec<Tree>,
     metadata: HashMap<String, String>,
 }
 
 fn parse_missing<'de, D>(d: D) -> Result<f64, D::Error>
 where
     D: Deserializer<'de>,
@@ -84,14 +85,15 @@
             256,
             true,
             true,
             None,
             1.,
             0,
             f64::NAN,
+            false,
         )
     }
 }
 
 impl GradientBooster {
     /// Gradient Booster object
     ///
@@ -113,19 +115,24 @@
     /// * `min_leaf_weight` - Minimum sum of the hessian values of the loss function
     ///   required to be in a node.
     /// * `base_score` - The initial prediction value of the model.
     /// * `nbins` - Number of bins to calculate to partition the data. Setting this to
     ///   a smaller number, will result in faster training time, while potentially sacrificing
     ///   accuracy. If there are more bins, than unique values in a column, all unique values
     ///   will be used.
+    /// * `parallel` - Should the algorithm be run in parallel?
+    /// * `allow_missing_splits` - Should the algorithm allow splits that completed seperate out missing
+    /// and non-missing values, in the case where `create_missing_branch` is false. When `create_missing_branch`
+    /// is true, setting this to true will result in the missin branch being further split.
     /// * `monotone_constraints` - Constraints that are used to enforce a specific relationship
     ///   between the training features and the target variable.
     /// * `subsample` - Percent of records to randomly sample at each iteration when training a tree.
     /// * `seed` - Integer value used to seed any randomness used in the algorithm.
     /// * `missing` - Value to consider missing.
+    /// * `create_missing_branch` - Should missing be split out it's own separate branch?
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         objective_type: ObjectiveType,
         iterations: usize,
         learning_rate: f32,
         max_depth: usize,
         max_leaves: usize,
@@ -136,14 +143,15 @@
         nbins: u16,
         parallel: bool,
         allow_missing_splits: bool,
         monotone_constraints: Option<ConstraintMap>,
         subsample: f32,
         seed: u64,
         missing: f64,
+        create_missing_branch: bool,
     ) -> Self {
         GradientBooster {
             objective_type,
             iterations,
             learning_rate,
             max_depth,
             max_leaves,
@@ -154,14 +162,15 @@
             nbins,
             parallel,
             allow_missing_splits,
             monotone_constraints,
             subsample,
             seed,
             missing,
+            create_missing_branch,
             trees: Vec::new(),
             metadata: HashMap::new(),
         }
     }
 
     /// Fit the gradient booster on a provided dataset.
     ///
@@ -171,28 +180,52 @@
     /// training the model. If None is passed, a weight of 1 will be used for every record.
     pub fn fit(
         &mut self,
         data: &Matrix<f64>,
         y: &[f64],
         sample_weight: &[f64],
     ) -> Result<(), ForustError> {
-        let mut rng = StdRng::seed_from_u64(self.seed);
         let constraints_map = self
             .monotone_constraints
             .as_ref()
             .unwrap_or(&ConstraintMap::new())
             .to_owned();
-        let splitter = MissingImputerSplitter {
-            l2: self.l2,
-            gamma: self.gamma,
-            min_leaf_weight: self.min_leaf_weight,
-            learning_rate: self.learning_rate,
-            allow_missing_splits: self.allow_missing_splits,
-            constraints_map,
+        if self.create_missing_branch {
+            let splitter = MissingBranchSplitter {
+                l2: self.l2,
+                gamma: self.gamma,
+                min_leaf_weight: self.min_leaf_weight,
+                learning_rate: self.learning_rate,
+                allow_missing_splits: self.allow_missing_splits,
+                constraints_map,
+            };
+            self.fit_trees(y, sample_weight, data, &splitter)?;
+        } else {
+            let splitter = MissingImputerSplitter {
+                l2: self.l2,
+                gamma: self.gamma,
+                min_leaf_weight: self.min_leaf_weight,
+                learning_rate: self.learning_rate,
+                allow_missing_splits: self.allow_missing_splits,
+                constraints_map,
+            };
+            self.fit_trees(y, sample_weight, data, &splitter)?;
         };
+
+        Ok(())
+    }
+
+    fn fit_trees<T: Splitter>(
+        &mut self,
+        y: &[f64],
+        sample_weight: &[f64],
+        data: &Matrix<f64>,
+        splitter: &T,
+    ) -> Result<(), ForustError> {
+        let mut rng = StdRng::seed_from_u64(self.seed);
         let mut yhat = vec![self.base_score; y.len()];
         let (calc_grad, calc_hess) = gradient_hessian_callables(&self.objective_type);
         let mut grad = calc_grad(y, &yhat, sample_weight);
         let mut hess = calc_hess(y, &yhat, sample_weight);
 
         // Generate binned data
         // TODO
@@ -204,15 +237,15 @@
         for _ in 0..self.iterations {
             let mut tree = Tree::new();
             tree.fit(
                 &bdata,
                 &binned_data.cuts,
                 &grad,
                 &hess,
-                &splitter,
+                splitter,
                 self.max_leaves,
                 self.max_depth,
                 self.parallel,
                 self.subsample,
                 &mut rng,
             );
             let preds = tree.predict(data, self.parallel, &self.missing);
```

### Comparing `forust-0.2.3/local_dependencies/forust-ml/src/histogram.rs` & `forust-0.2.4/local_dependencies/forust-ml/src/histogram.rs`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,23 @@
                 v.hessian_sum += f64::from(*h);
             }
         });
     histogram.iter().map(|b| b.as_f32_bin()).collect()
 }
 
 impl HistogramMatrix {
+    /// Create an empty histogram matrix.
+    pub fn empty() -> Self {
+        HistogramMatrix(JaggedMatrix {
+            data: Vec::new(),
+            ends: Vec::new(),
+            cols: 0,
+            n_records: 0,
+        })
+    }
     pub fn new(
         data: &Matrix<u16>,
         cuts: &JaggedMatrix<f64>,
         grad: &[f32],
         hess: &[f32],
         index: &[usize],
         parallel: bool,
@@ -119,24 +128,25 @@
         let col_index: Vec<usize> = (0..data.cols).collect();
         // Sort gradients and hessians to reduce cache hits.
         // This made a really sizeable difference on larger datasets
         // Bringing training time down from nearly 6 minutes, to 2 minutes.
         // Sort gradients and hessians to reduce cache hits.
         // This made a really sizeable difference on larger datasets
         // Bringing training time down from nearly 6 minutes, to 2 minutes.
-        let sorted_grad = if !sort {
-            grad.to_vec()
+        let (sorted_grad, sorted_hess) = if !sort {
+            (grad.to_vec(), hess.to_vec())
         } else {
-            index.iter().map(|i| grad[*i]).collect::<Vec<f32>>()
-        };
-
-        let sorted_hess = if !sort {
-            hess.to_vec()
-        } else {
-            index.iter().map(|i| hess[*i]).collect::<Vec<f32>>()
+            let mut n_grad = Vec::new();
+            let mut n_hess = Vec::new();
+            for i in index {
+                let i_ = *i;
+                n_grad.push(grad[i_]);
+                n_hess.push(hess[i_]);
+            }
+            (n_grad, n_hess)
         };
 
         let histograms = if parallel {
             col_index
                 .par_iter()
                 .flat_map(|col| {
                     create_feature_histogram(
```

### Comparing `forust-0.2.3/local_dependencies/forust-ml/src/node.rs` & `forust-0.2.4/local_dependencies/forust-ml/src/node.rs`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     pub left_child: usize,
     pub right_child: usize,
     pub start_idx: usize,
     pub stop_idx: usize,
     pub lower_bound: f32,
     pub upper_bound: f32,
     pub is_leaf: bool,
+    pub is_missing_leaf: bool,
 }
 
 #[derive(Deserialize, Serialize)]
 pub struct Node {
     pub num: usize,
     pub weight_value: f32,
     pub hessian_sum: f32,
@@ -61,22 +62,18 @@
         } else if v < &self.split_value {
             self.left_child
         } else {
             //  if v >= &self.split_value
             self.right_child
         }
     }
-}
 
-#[derive(Deserialize, Serialize)]
-pub struct LeafNode {
-    pub num: usize,
-    pub weight_value: f32,
-    pub hessian_sum: f32,
-    pub depth: usize,
+    pub fn has_missing_branch(&self) -> bool {
+        (self.missing_node != self.right_child) && (self.missing_node != self.left_child)
+    }
 }
 
 impl SplittableNode {
     pub fn from_node_info(
         num: usize,
         histograms: HistogramMatrix,
         depth: usize,
@@ -99,14 +96,15 @@
             left_child: 0,
             right_child: 0,
             start_idx,
             stop_idx,
             lower_bound: node_info.bounds.0,
             upper_bound: node_info.bounds.1,
             is_leaf: true,
+            is_missing_leaf: false,
         }
     }
 
     /// Create a default splitable node,
     /// we default to the node being a leaf.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
@@ -137,34 +135,37 @@
             left_child: 0,
             right_child: 0,
             start_idx,
             stop_idx,
             lower_bound,
             upper_bound,
             is_leaf: true,
+            is_missing_leaf: false,
         }
     }
 
     pub fn update_children(
         &mut self,
+        missing_child: usize,
         left_child: usize,
         right_child: usize,
         split_info: &SplitInfo,
     ) {
         self.left_child = left_child;
         self.right_child = right_child;
         self.split_feature = split_info.split_feature;
-        self.split_gain = split_info.left_node.gain + split_info.right_node.gain - self.gain_value;
-        self.split_value = split_info.split_value;
-        self.missing_node = match split_info.missing_node {
-            MissingInfo::Left => left_child,
-            MissingInfo::Right => right_child,
-            MissingInfo::Branch(_) => todo!(),
-            MissingInfo::EmptyBranch => todo!(),
+        let missing_split_gain = match &split_info.missing_node {
+            MissingInfo::Branch(ni) => ni.gain,
+            _ => 0.,
         };
+        self.split_gain =
+            split_info.left_node.gain + split_info.right_node.gain + missing_split_gain
+                - self.gain_value;
+        self.split_value = split_info.split_value;
+        self.missing_node = missing_child;
         self.is_leaf = false;
     }
     pub fn as_node(&self) -> Node {
         Node {
             num: self.num,
             weight_value: self.weight_value,
             hessian_sum: self.hessian_sum,
```

### Comparing `forust-0.2.3/local_dependencies/forust-ml/src/objective.rs` & `forust-0.2.4/local_dependencies/forust-ml/src/objective.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/local_dependencies/forust-ml/src/partial_dependence.rs` & `forust-0.2.4/local_dependencies/forust-ml/src/partial_dependence.rs`

 * *Files 26% similar despite different names*

```diff
@@ -31,30 +31,47 @@
         } else {
             n.right_child
         };
         tree_partial_dependence(tree, child, feature, value, proportion, missing)
     } else {
         let left_cover = get_node_cover(tree, n.left_child);
         let right_cover = get_node_cover(tree, n.right_child);
-        let total_cover = left_cover + right_cover;
+        let missing_cover = if n.has_missing_branch() {
+            get_node_cover(tree, n.missing_node)
+        } else {
+            0.0
+        };
+        let total_cover = left_cover + right_cover + missing_cover;
+        let missing_pd = if n.has_missing_branch() {
+            tree_partial_dependence(
+                tree,
+                n.missing_node,
+                feature,
+                value,
+                proportion * (missing_cover / total_cover),
+                missing,
+            )
+        } else {
+            0.
+        };
         tree_partial_dependence(
             tree,
             n.left_child,
             feature,
             value,
             proportion * (left_cover / total_cover),
             missing,
         ) + tree_partial_dependence(
             tree,
             n.right_child,
             feature,
             value,
             proportion * (right_cover / total_cover),
             missing,
-        )
+        ) + missing_pd
     }
 }
 
 #[cfg(test)]
 mod tests {
     use rand::rngs::StdRng;
     use rand::SeedableRng;
```

### Comparing `forust-0.2.3/local_dependencies/forust-ml/src/splitter.rs` & `forust-0.2.4/local_dependencies/forust-ml/src/splitter.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 use crate::constraints::{Constraint, ConstraintMap};
 use crate::data::{JaggedMatrix, Matrix};
 use crate::histogram::HistogramMatrix;
 use crate::node::SplittableNode;
-use crate::utils::{constrained_weight, cull_gain, gain_given_weight, pivot_on_split, weight};
+use crate::utils::{
+    constrained_weight, cull_gain, gain_given_weight, pivot_on_split,
+    pivot_on_split_exclude_missing, weight,
+};
 
 #[derive(Debug)]
 pub struct SplitInfo {
     pub split_gain: f32,
     pub split_feature: usize,
     pub split_value: f64,
     pub split_bin: u16,
@@ -24,24 +27,27 @@
     pub bounds: (f32, f32),
 }
 
 #[derive(Debug)]
 pub enum MissingInfo {
     Left,
     Right,
-    EmptyBranch,
+    Leaf(NodeInfo),
     Branch(NodeInfo),
 }
 
 pub trait Splitter {
     fn get_constraint(&self, feature: &usize) -> Option<&Constraint>;
     // fn get_allow_missing_splits(&self) -> bool;
     fn get_gamma(&self) -> f32;
     fn get_l2(&self) -> f32;
 
+    /// Find the best possible split, considering all feature histograms.
+    /// If we wanted to add Column sampling, this is probably where
+    /// we would need to do it, otherwise, it would be at the tree level.
     fn best_split(&self, node: &SplittableNode) -> Option<SplitInfo> {
         let mut best_split_info = None;
         let mut best_gain = 0.0;
         let HistogramMatrix(histograms) = &node.histograms;
         for i in 0..histograms.cols {
             let split_info = self.best_feature_split(node, i);
             match split_info {
@@ -110,16 +116,25 @@
                     cuml_grad += bin.gradient_sum;
                     cuml_hess += bin.hessian_sum;
                     continue;
                 }
                 Some(v) => v,
             };
 
-            let split_gain =
-                (left_node_info.gain + right_node_info.gain - node.gain_value) - self.get_gamma();
+            // TODO!
+            // Should we be doing this?
+            // or should missing gain not factor in at
+            // all to the split gain?
+            let missing_gain = match &missing_info {
+                MissingInfo::Branch(v) | MissingInfo::Leaf(v) => v.gain,
+                _ => 0.0,
+            };
+            let split_gain = (left_node_info.gain + right_node_info.gain + missing_gain
+                - node.gain_value)
+                - self.get_gamma();
 
             // Check monotonicity holds
             let split_gain = cull_gain(
                 split_gain,
                 left_node_info.weight,
                 right_node_info.weight,
                 constraint,
@@ -162,33 +177,33 @@
             // Update for new value
             cuml_grad += bin.gradient_sum;
             cuml_hess += bin.hessian_sum;
         }
         split_info
     }
 
-    /// Handle the split info, creating the children nodes, for the provided nodes
-    /// push them onto the growable stack.
-    /// Return a tuple, where the first value is the number of nodes pushed onto the
-    /// growable stack, and the second value is the number of potential leaves
-    /// that have been added.
+    /// Handle the split info, creating the children nodes, this function
+    /// will return a vector of new splitable nodes, that can be added to the
+    /// growable stack, and further split, or converted to leaf nodes.
     #[allow(clippy::too_many_arguments)]
     fn handle_split_info(
         &self,
         split_info: SplitInfo,
         n_nodes: &usize,
         node: &mut SplittableNode,
         index: &mut [usize],
         data: &Matrix<u16>,
         cuts: &JaggedMatrix<f64>,
         grad: &[f32],
         hess: &[f32],
         parallel: bool,
     ) -> Vec<SplittableNode>;
 
+    /// Split the node, if we cant find a best split, we will need to
+    /// return an empty vector, this node is a leaf.
     #[allow(clippy::too_many_arguments)]
     fn split_node(
         &self,
         n_nodes: &usize,
         node: &mut SplittableNode,
         index: &mut [usize],
         data: &Matrix<u16>,
@@ -282,30 +297,46 @@
 
         // Check the min_hessian constraint first
         if (right_hessian < self.min_leaf_weight) || (left_hessian < self.min_leaf_weight) {
             // Update for new value
             return None;
         }
 
+        // We have not considered missing at all up until this point, we could if we wanted
+        // to give more predictive power probably to missing.
         // If we don't want to allow the missing branch to be split further,
         // we will default to creating an empty branch.
-        let missing_info = // Check Missing direction
-        if ((missing_gradient != 0.0) || (missing_hessian != 0.0)) || !self.allow_missing_splits {
-            MissingInfo::EmptyBranch
-        } else {
-            let missing_weight = weight(&self.get_l2(), missing_gradient, missing_hessian);
-            let missing_gain = gain_given_weight(&self.get_l2(), missing_gradient, missing_hessian, missing_weight);
+
+        // Set weight to the parent weight...
+        let missing_weight = weight(
+            &self.get_l2(),
+            missing_gradient + left_gradient + right_gradient,
+            missing_hessian + left_hessian + right_hessian,
+        ); // weight(&self.get_l2(), missing_gradient, missing_hessian);
+        let missing_gain = gain_given_weight(
+            &self.get_l2(),
+            missing_gradient,
+            missing_hessian,
+            missing_weight,
+        );
+        let missing_info = NodeInfo {
+            grad: missing_gradient,
+            gain: missing_gain,
+            cover: missing_hessian,
+            weight: missing_weight * self.learning_rate,
+            bounds: (f32::NEG_INFINITY, f32::INFINITY),
+        };
+        let missing_node = // Check Missing direction
+        if ((missing_gradient != 0.0) || (missing_hessian != 0.0)) && self.allow_missing_splits {
             MissingInfo::Branch(
-                NodeInfo {
-                    grad: missing_gradient,
-                    gain: missing_gain,
-                    cover: missing_hessian,
-                    weight: missing_weight * self.learning_rate,
-                    bounds: (f32::NEG_INFINITY, f32::INFINITY),
-                }
+                missing_info
+            )
+        } else {
+            MissingInfo::Leaf(
+                missing_info
             )
         };
 
         if (right_hessian < self.min_leaf_weight) || (left_hessian < self.min_leaf_weight) {
             // Update for new value
             return None;
         }
@@ -320,32 +351,209 @@
             NodeInfo {
                 grad: right_gradient,
                 gain: right_gain,
                 cover: right_hessian,
                 weight: right_weight * self.learning_rate,
                 bounds: (f32::NEG_INFINITY, f32::INFINITY),
             },
-            missing_info,
+            missing_node,
         ))
     }
 
-    #[allow(unused)]
     fn handle_split_info(
         &self,
         split_info: SplitInfo,
         n_nodes: &usize,
         node: &mut SplittableNode,
         index: &mut [usize],
         data: &Matrix<u16>,
         cuts: &JaggedMatrix<f64>,
         grad: &[f32],
         hess: &[f32],
         parallel: bool,
     ) -> Vec<SplittableNode> {
-        todo!()
+        let missing_child = *n_nodes;
+        let left_child = missing_child + 1;
+        let right_child = missing_child + 2;
+        node.update_children(missing_child, left_child, right_child, &split_info);
+
+        let (missing_is_leaf, missing_info) = match split_info.missing_node {
+            MissingInfo::Branch(i) => (false, i),
+            MissingInfo::Leaf(i) => (true, i),
+            _ => unreachable!(),
+        };
+
+        // We need to move all of the index's above and below our
+        // split value.
+        // pivot the sub array that this node has on our split value
+        // Missing all falls to the bottom.
+        let (mut missing_split_idx, mut split_idx) = pivot_on_split_exclude_missing(
+            &mut index[node.start_idx..node.stop_idx],
+            data.get_col(split_info.split_feature),
+            split_info.split_bin,
+        );
+        // Calculate histograms
+        let total_recs = node.stop_idx - node.start_idx;
+        let n_right = total_recs - split_idx;
+        let n_left = total_recs - n_right - missing_split_idx;
+        let n_missing = total_recs - (n_right + n_left);
+        let max_ = match vec![n_missing, n_left, n_right]
+            .iter()
+            .enumerate()
+            .max_by(|(_, i), (_, j)| i.cmp(j))
+        {
+            Some((i, _)) => i,
+            // if we can't compare them, it doesn't
+            // really matter, build the histogram on
+            // any of them.
+            None => 0,
+        };
+
+        // Now that we have calculated the number of records
+        // add the start index, to make the split_index
+        // relative to the entire index array
+        split_idx += node.start_idx;
+        missing_split_idx += node.start_idx;
+
+        // Build the histograms for the smaller node.
+        let left_histograms: HistogramMatrix;
+        let right_histograms: HistogramMatrix;
+        let missing_histograms: HistogramMatrix;
+        if n_missing == 0 {
+            if max_ == 1 {
+                missing_histograms = HistogramMatrix::empty();
+                right_histograms = HistogramMatrix::new(
+                    data,
+                    cuts,
+                    grad,
+                    hess,
+                    &index[split_idx..node.stop_idx],
+                    parallel,
+                    true,
+                );
+                left_histograms =
+                    HistogramMatrix::from_parent_child(&node.histograms, &right_histograms);
+            } else {
+                missing_histograms = HistogramMatrix::empty();
+                left_histograms = HistogramMatrix::new(
+                    data,
+                    cuts,
+                    grad,
+                    hess,
+                    &index[missing_split_idx..split_idx],
+                    parallel,
+                    true,
+                );
+                right_histograms =
+                    HistogramMatrix::from_parent_child(&node.histograms, &left_histograms);
+            }
+        } else if max_ == 0 {
+            // Max is missing, calculate the other two
+            // levels histograms.
+            left_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[missing_split_idx..split_idx],
+                parallel,
+                true,
+            );
+            right_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[split_idx..node.stop_idx],
+                parallel,
+                true,
+            );
+            missing_histograms = HistogramMatrix::from_parent_two_children(
+                &node.histograms,
+                &left_histograms,
+                &right_histograms,
+            )
+        } else if max_ == 1 {
+            missing_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[node.start_idx..missing_split_idx],
+                parallel,
+                true,
+            );
+            right_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[split_idx..node.stop_idx],
+                parallel,
+                true,
+            );
+            left_histograms = HistogramMatrix::from_parent_two_children(
+                &node.histograms,
+                &missing_histograms,
+                &right_histograms,
+            )
+        } else {
+            // right is the largest
+
+            missing_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[node.start_idx..missing_split_idx],
+                parallel,
+                true,
+            );
+            left_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[missing_split_idx..split_idx],
+                parallel,
+                true,
+            );
+            right_histograms = HistogramMatrix::from_parent_two_children(
+                &node.histograms,
+                &missing_histograms,
+                &left_histograms,
+            )
+        }
+
+        let mut missing_node = SplittableNode::from_node_info(
+            missing_child,
+            missing_histograms,
+            node.depth + 1,
+            node.start_idx,
+            missing_split_idx,
+            missing_info,
+        );
+        missing_node.is_missing_leaf = missing_is_leaf;
+        let left_node = SplittableNode::from_node_info(
+            left_child,
+            left_histograms,
+            node.depth + 1,
+            missing_split_idx,
+            split_idx,
+            split_info.left_node,
+        );
+        let right_node = SplittableNode::from_node_info(
+            right_child,
+            right_histograms,
+            node.depth + 1,
+            split_idx,
+            node.stop_idx,
+            split_info.right_node,
+        );
+        vec![missing_node, left_node, right_node]
     }
 }
 
 /// Missing imputer splitter
 /// Splitter that imputes missing values, by sending
 /// them down either the right or left branch, depending
 /// on which results in a higher increase in gain.
@@ -542,22 +750,21 @@
         index: &mut [usize],
         data: &Matrix<u16>,
         cuts: &JaggedMatrix<f64>,
         grad: &[f32],
         hess: &[f32],
         parallel: bool,
     ) -> Vec<SplittableNode> {
-        let left_idx = *n_nodes;
-        let right_idx = left_idx + 1;
+        let left_child = *n_nodes;
+        let right_child = left_child + 1;
 
         let missing_right = match split_info.missing_node {
             MissingInfo::Left => false,
             MissingInfo::Right => true,
-            MissingInfo::Branch(_) => todo!(),
-            MissingInfo::EmptyBranch => todo!(),
+            _ => unreachable!(),
         };
 
         // We need to move all of the index's above and below our
         // split value.
         // pivot the sub array that this node has on our split value
         // Here we assign missing to a specific direction.
         // This will need to be refactored once we add a
@@ -566,15 +773,15 @@
             &mut index[node.start_idx..node.stop_idx],
             data.get_col(split_info.split_feature),
             split_info.split_bin,
             missing_right,
         );
         // Calculate histograms
         let total_recs = node.stop_idx - node.start_idx;
-        let n_right = total_recs - split_idx - 1;
+        let n_right = total_recs - split_idx;
         let n_left = total_recs - n_right;
 
         // Now that we have calculated the number of records
         // add the start index, to make the split_index
         // relative to the entire index array
         split_idx += node.start_idx;
 
@@ -602,27 +809,31 @@
                 &index[split_idx..node.stop_idx],
                 parallel,
                 true,
             );
             left_histograms =
                 HistogramMatrix::from_parent_child(&node.histograms, &right_histograms);
         }
-
-        node.update_children(left_idx, right_idx, &split_info);
+        let missing_child = if missing_right {
+            right_child
+        } else {
+            left_child
+        };
+        node.update_children(missing_child, left_child, right_child, &split_info);
 
         let left_node = SplittableNode::from_node_info(
-            left_idx,
+            left_child,
             left_histograms,
             node.depth + 1,
             node.start_idx,
             split_idx,
             split_info.left_node,
         );
         let right_node = SplittableNode::from_node_info(
-            right_idx,
+            right_child,
             right_histograms,
             node.depth + 1,
             split_idx,
             node.stop_idx,
             split_info.right_node,
         );
         vec![left_node, right_node]
@@ -791,11 +1002,11 @@
             0,
             grad.len(),
             f32::NEG_INFINITY,
             f32::INFINITY,
         );
         let s = splitter.best_split(&mut n).unwrap();
         println!("{:?}", s);
-        n.update_children(1, 2, &s);
+        n.update_children(2, 1, 2, &s);
         assert_eq!(0, s.split_feature);
     }
 }
```

### Comparing `forust-0.2.3/local_dependencies/forust-ml/src/tree.rs` & `forust-0.2.4/local_dependencies/forust-ml/src/tree.rs`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,17 @@
                 n_leaves += 1;
             } else {
                 self.nodes[n_idx].make_parent_node(node);
                 n_leaves += n_new_nodes;
                 n_nodes += n_new_nodes;
                 for n in new_nodes {
                     self.nodes.push(n.as_node());
-                    growable.push_front(n)
+                    if !n.is_missing_leaf {
+                        growable.push_front(n)
+                    }
                 }
             }
         }
     }
     pub fn predict_contributions_row(
         &self,
         row: &[f64],
@@ -270,19 +272,25 @@
     }
     fn distribute_node_leaf_weights(&self, i: usize, weights: &mut [f64]) -> f64 {
         let node = &self.nodes[i];
         let mut w = node.weight_value as f64;
         if !node.is_leaf {
             let left_node = &self.nodes[node.left_child];
             let right_node = &self.nodes[node.right_child];
-            w = ((left_node.hessian_sum as f64
-                * self.distribute_node_leaf_weights(node.left_child, weights))
-                + (right_node.hessian_sum as f64
-                    * self.distribute_node_leaf_weights(node.right_child, weights)))
-                / (node.hessian_sum as f64);
+            w = left_node.hessian_sum as f64
+                * self.distribute_node_leaf_weights(node.left_child, weights);
+            w += right_node.hessian_sum as f64
+                * self.distribute_node_leaf_weights(node.right_child, weights);
+            // If this a tree with a missing branch.
+            if node.has_missing_branch() {
+                let missing_node = &self.nodes[node.missing_node];
+                w += missing_node.hessian_sum as f64
+                    * self.distribute_node_leaf_weights(node.missing_node, weights);
+            }
+            w /= node.hessian_sum as f64;
         }
         weights[i] = w;
         w
     }
     pub fn distribute_leaf_weights(&self) -> Vec<f64> {
         let mut weights = vec![0.; self.nodes.len()];
         self.distribute_node_leaf_weights(0, &mut weights);
@@ -302,14 +310,17 @@
             let node = &self.nodes[idx];
             if node.is_leaf {
                 r += format!("{}{}\n", "      ".repeat(node.depth).as_str(), node).as_str();
             } else {
                 r += format!("{}{}\n", "      ".repeat(node.depth).as_str(), node).as_str();
                 print_buffer.push(node.right_child);
                 print_buffer.push(node.left_child);
+                if node.has_missing_branch() {
+                    print_buffer.push(node.missing_node);
+                }
             }
         }
         write!(f, "{}", r)
     }
 }
 
 #[cfg(test)]
```

### Comparing `forust-0.2.3/local_dependencies/forust-ml/src/utils.rs` & `forust-0.2.4/local_dependencies/forust-ml/src/utils.rs`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,17 @@
 
 /// Provided a list of index values, pivot those values
 /// around a specific split value so all of the values less
 /// than the split value are on one side, and then all of the
 /// values greater than or equal to the split value are above.
 /// Missing values, will be pushed to the bottom, a value of
 /// zero is missing in this case.
+/// Returns a tuple, the first is the first non-missing value
+/// index, the second is the first value that is greater than
+/// our provided split value.
 ///
 /// WARNING!!! Currently, this function fails, if all the values are
 /// missing...
 ///
 /// * `index` - The index values to sort.
 /// * `feature` - The feature vector to use to sort the index by.
 /// * `split_value` - the split value to use to pivot on.
@@ -343,15 +346,15 @@
                 Ordering::Greater => break,
             }
         }
         if low < high {
             index.swap(high, low);
         }
     }
-    (low, missing)
+    (missing, low)
 }
 
 /// Function to compare a value to our split value.
 /// Our split value will _never_ be missing (0), thus we
 /// don't have to worry about that.
 #[inline]
 pub fn missing_compare(split_value: &u16, cmp_value: u16, missing_right: bool) -> Ordering {
@@ -648,27 +651,27 @@
         fn pivot_missing_assert(
             split_value: u16,
             idx: &[usize],
             f: &[u16],
             split_i: &(usize, usize),
         ) {
             // Check they are lower than..
-            for i in 0..split_i.0 {
+            for i in 0..split_i.1 {
                 assert!(f[idx[i]] < split_value);
             }
             // Check missing got moved
-            for i in 0..split_i.1 {
+            for i in 0..split_i.0 {
                 assert!(f[idx[i]] == 0);
             }
             // Check none are less than...
-            for i in split_i.0..(idx.len()) {
+            for i in split_i.1..(idx.len()) {
                 assert!(!(f[idx[i]] < split_value));
             }
             // Check none other are missing...
-            for i in split_i.1..(idx.len()) {
+            for i in split_i.0..(idx.len()) {
                 assert!(f[idx[i]] != 0);
             }
         }
         // TODO: Add more tests for this...
         // Using minimum value...
         let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
         let f = vec![15, 10, 10, 0, 3, 0, 0, 9, 3, 5, 2, 6, 13, 19, 14];
@@ -705,14 +708,22 @@
         let mut idx = vec![0, 1, 2, 3, 4, 5];
         let f = vec![1, 0, 1, 3, 0, 4];
         let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 2);
         // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
         // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
         pivot_missing_assert(2, &idx, &f, &split_i);
 
+        // Ensure it works on all missing...
+        // let mut idx = vec![0, 1, 2, 3, 4, 5];
+        // let f: Vec<u16> = vec![3; idx.len()];
+        // let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 2);
+        // // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
+        // // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
+        // pivot_missing_assert(2, &idx, &f, &split_i);
+
         // Check if none missing...
         // TODO: Add more tests for this...
         let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
         let f = vec![15, 10, 10, 2, 3, 5, 7, 9, 3, 5, 2, 6, 13, 19, 14];
         let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
         //let split_i = pivot_on_split(&mut idx, &f, 10, false);
         // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
```

### Comparing `forust-0.2.3/.gitignore` & `forust-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/README.md` & `forust-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.3"
+forust-ml = "0.2.4"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -56,21 +56,22 @@
  - `base_score` ***(float, optional)***: The initial prediction value of the model. Defaults to 0.5.
  - `nbins` ***(int, optional)***: Number of bins to calculate to partition the data. Setting this to
     a smaller number, will result in faster training time, while potentially sacrificing
     accuracy. If there are more bins, than unique values in a column, all unique values
     will be used. Defaults to 256.
  - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
     with this model? Defaults to `True`.
- - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. Defaults to `True`.
+ - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. If `create_missing_branch` is set to `True` having this parameter be set to `True` will result in the missing branch further split, if this parameter is `False` then in that case the missing branch will always be a terminal node. Defaults to `True`.
  - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
  - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
       training a tree. Defaults to 1.0, meaning all data is used for training.
  - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
       algorithm. Defaults to 0.
  - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
+ - `create_missing_branch` ***(bool, optional)***: An experimental parameter, that if `True`, will create a separate branch for missing, creating a ternary tree, the missing node will be given the same weight value as the parent node. If this parameter is `False`, missing will be sent down either the left or right branch, creating a binary tree. Defaults to `False`.
 
 ### Training and Predicting
 
 Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
 In the case of this example, the predictions are the log odds of a given record being 1.
 
 ```python
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.3" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.4" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -45,15 +45,18 @@
 time, while potentially sacrificing accuracy. If there are more bins, than
 unique values in a column, all unique values will be used. Defaults to 256. -
 `parallel` ***(bool, optional)***: Should multiple cores be used when training
 and predicting with this model? Defaults to `True`. - `allow_missing_splits`
 ***(bool, optional)***: Allow for splits to be made such that all missing
 values go down one branch, and all non-missing values go down the other, if
 this results in the greatest reduction of loss. If this is false, splits will
-only be made on non missing values. Defaults to `True`. -
+only be made on non missing values. If `create_missing_branch` is set to `True`
+having this parameter be set to `True` will result in the missing branch
+further split, if this parameter is `False` then in that case the missing
+branch will always be a terminal node. Defaults to `True`. -
 `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are
 used to enforce a specific relationship between the training features and the
 target variable. A dictionary should be provided where the keys are the feature
 index value if the model will be fit on a numpy array, or a feature name if it
 will be fit on a pandas Dataframe. The values of the dictionary should be an
 integer value of -1, 1, or 0 to specify the relationship that should be
 estimated between the respective feature and the target variable. Use a value
@@ -62,51 +65,55 @@
 will not have any constraint applied. If `None` is passed no constraints will
 be enforced on any variable. Defaults to `None`. - `subsample` ***(float,
 optional)***: Percent of records to randomly sample at each iteration when
 training a tree. Defaults to 1.0, meaning all data is used for training. -
 `seed` ***(integer, optional)***: Integer value used to seed any randomness
 used in the algorithm. Defaults to 0. - `missing` ***(float, optional)***:
 Value to consider missing, when training and predicting with the booster.
-Defaults to `np.nan`. ### Training and Predicting Once, the booster has been
-initialized, it can be fit on a provided dataset, and performance field. After
-fitting, the model can be used to predict on a dataset. In the case of this
-example, the predictions are the log odds of a given record being 1. ```python
-# Small example dataset from seaborn import load_dataset df = load_dataset
-("titanic") X = df.select_dtypes("number").drop(columns=["survived"]) y = df
-["survived"] # Initialize a booster with defaults. from forust import
-GradientBooster model = GradientBooster(objective_type="LogLoss") model.fit(X,
-y) # Predict on data model.predict(X.head()) # array([-1.94919663, 2.25863229,
-0.32963671, 2.48732194, -3.00371813]) # predict contributions
-model.predict_contributions(X.head()) # array([[-0.63014213, 0.33880048, -
-0.16520798, -0.07798772, -0.85083578, # -1.07720813], # [ 1.05406709,
-0.08825999, 0.21662544, -0.12083538, 0.35209258, # -1.07720813], ``` The `fit`
-method accepts the following arguments. - `X` ***(FrameLike)***: Either a
-pandas DataFrame, or a 2 dimensional numpy array, with numeric data. - `y` ***
-(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If
-"LogLoss" was the objective type specified, then this should only contain 1 or
-0 values, where 1 is the positive class being predicted. If "SquaredLoss" is
-the objective type, then any continuous variable can be provided. -
-`sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use
-when training the model. If None is passed, a weight of 1 will be used for
-every record. Defaults to None. The predict method accepts the following
-arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2
-dimensional numpy array, with numeric data. - `parallel` ***(Optional[bool],
-optional)***: Optionally specify if the predict function should run in parallel
-on multiple threads. If `None` is passed, the `parallel` attribute of the
-booster will be used. Defaults to `None`. The `predict_contributions` method
-will predict with the fitted booster on new data, returning the feature
-contribution matrix. The last column is the bias term. - `X` ***(FrameLike)***:
+Defaults to `np.nan`. - `create_missing_branch` ***(bool, optional)***: An
+experimental parameter, that if `True`, will create a separate branch for
+missing, creating a ternary tree, the missing node will be given the same
+weight value as the parent node. If this parameter is `False`, missing will be
+sent down either the left or right branch, creating a binary tree. Defaults to
+`False`. ### Training and Predicting Once, the booster has been initialized, it
+can be fit on a provided dataset, and performance field. After fitting, the
+model can be used to predict on a dataset. In the case of this example, the
+predictions are the log odds of a given record being 1. ```python # Small
+example dataset from seaborn import load_dataset df = load_dataset("titanic") X
+= df.select_dtypes("number").drop(columns=["survived"]) y = df["survived"] #
+Initialize a booster with defaults. from forust import GradientBooster model =
+GradientBooster(objective_type="LogLoss") model.fit(X, y) # Predict on data
+model.predict(X.head()) # array([-1.94919663, 2.25863229, 0.32963671,
+2.48732194, -3.00371813]) # predict contributions model.predict_contributions
+(X.head()) # array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -
+0.85083578, # -1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -
+0.12083538, 0.35209258, # -1.07720813], ``` The `fit` method accepts the
+following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2
+dimensional numpy array, with numeric data. - `y` ***(ArrayLike)***: Either a
+pandas Series, or a 1 dimensional numpy array. If "LogLoss" was the objective
+type specified, then this should only contain 1 or 0 values, where 1 is the
+positive class being predicted. If "SquaredLoss" is the objective type, then
+any continuous variable can be provided. - `sample_weight` ***(Optional
+[ArrayLike], optional)***: Instance weights to use when training the model. If
+None is passed, a weight of 1 will be used for every record. Defaults to None.
+The predict method accepts the following arguments. - `X` ***(FrameLike)***:
 Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
 `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
 function should run in parallel on multiple threads. If `None` is passed, the
-`parallel` attribute of the booster will be used. Defaults to `None`. ###
-Inspecting the Model Once the booster has been fit, each individual tree
-structure can be retrieved in text form, using the `text_dump` method. This
-method returns a list, the same length as the number of trees in the model.
-```python model.text_dump()[0] # 0:[0 < 3]
+`parallel` attribute of the booster will be used. Defaults to `None`. The
+`predict_contributions` method will predict with the fitted booster on new
+data, returning the feature contribution matrix. The last column is the bias
+term. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional
+numpy array, with numeric data. - `parallel` ***(Optional[bool], optional)***:
+Optionally specify if the predict function should run in parallel on multiple
+threads. If `None` is passed, the `parallel` attribute of the booster will be
+used. Defaults to `None`. ### Inspecting the Model Once the booster has been
+fit, each individual tree structure can be retrieved in text form, using the
+`text_dump` method. This method returns a list, the same length as the number
+of trees in the model. ```python model.text_dump()[0] # 0:[0 < 3]
 yes=1,no=2,missing=2,gain=91.50833,cover=209.388307 # 1:[4 < 13.7917]
 yes=3,no=4,missing=4,gain=28.185467,cover=94.00148 # 3:[1 < 18]
 yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348 # 7:[1 < 17]
 yes=15,no=16,missing=16,gain=0.691266,cover=0.705011 # 15:leaf=-
 0.15120,cover=0.23500 # 16:leaf=0.154097,cover=0.470007 ``` The `json_dump`
 method performs the same action, but returns the model as a json representation
 rather than a text string. To see an estimate for how a given feature is used
```

### Comparing `forust-0.2.3/forust/__init__.py` & `forust-0.2.4/forust/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         nbins: int = 256,
         parallel: bool = True,
         allow_missing_splits: bool = True,
         monotone_constraints: Union[dict[Any, int], None] = None,
         subsample: float = 1.0,
         seed: int = 0,
         missing: float = np.nan,
+        create_missing_branch: bool = False,
     ):
         """Gradient Booster Class, used to generate gradient boosted decision tree ensembles.
 
         Args:
             objective_type (str, optional): The name of objective function used to optimize.
                 Valid options include "LogLoss" to use logistic loss as the objective function
                 (binary classification), or "SquaredLoss" to use Squared Error as the objective
@@ -126,15 +127,18 @@
                 accuracy. If there are more bins, than unique values in a column, all unique values
                 will be used. Defaults to 256.
             parallel (bool, optional): Should multiple cores be used when training and predicting
                 with this model? Defaults to `True`.
             allow_missing_splits (bool, optional): Allow for splits to be made such that all missing values go
                 down one branch, and all non-missing values go down the other, if this results
                 in the greatest reduction of loss. If this is false, splits will only be made on non
-                missing values. Defaults to `True`.
+                missing values. If `create_missing_branch` is set to `True` having this parameter be
+                set to `True` will result in the missing branch further split, if this parameter
+                is `False` then in that case the missing branch will always be a terminal node.
+                Defaults to `True`.
             monotone_constraints (dict[Any, int], optional): Constraints that are used to enforce a
                 specific relationship between the training features and the target variable. A dictionary
                 should be provided where the keys are the feature index value if the model will be fit on
                 a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of
                 the dictionary should be an integer value of -1, 1, or 0 to specify the relationship
                 that should be estimated between the respective feature and the target variable.
                 Use a value of -1 to enforce a negative relationship, 1 a positive relationship,
@@ -143,14 +147,18 @@
                 will be enforced on any variable.  Defaults to `None`.
             subsample (float, optional): Percent of records to randomly sample at each iteration when
                 training a tree. Defaults to 1.0, meaning all data is used to training.
             seed (integer, optional): Integer value used to seed any randomness used in the
                 algorithm. Defaults to 0.
             missing (float, optional): Value to consider missing, when training and predicting
                 with the booster. Defaults to `np.nan`.
+            create_missing_branch (bool, optional): An experimental parameter, that if `True`, will
+                create a separate branch for missing, creating a ternary tree, the missing node will be given the same
+                weight value as the parent node. If this parameter is `False`, missing will be sent
+                down either the left or right branch, creating a binary tree. Defaults to `False`.
 
         Raises:
             TypeError: Raised if an invalid dtype is passed.
         """
         booster = CrateGradientBooster(
             objective_type=objective_type,
             iterations=iterations,
@@ -164,14 +172,15 @@
             nbins=nbins,
             parallel=parallel,
             allow_missing_splits=allow_missing_splits,
             monotone_constraints={},
             subsample=subsample,
             seed=seed,
             missing=missing,
+            create_missing_branch=create_missing_branch,
         )
         monotone_constraints_ = (
             {} if monotone_constraints is None else monotone_constraints
         )
         self.booster = cast(BoosterType, booster)
         self.objective_type = objective_type
         self.iterations = iterations
@@ -180,19 +189,20 @@
         self.max_leaves = max_leaves
         self.l2 = l2
         self.gamma = gamma
         self.min_leaf_weight = min_leaf_weight
         self.base_score = base_score
         self.nbins = nbins
         self.parallel = parallel
-        self.allow_missing_splits = (allow_missing_splits,)
+        self.allow_missing_splits = allow_missing_splits
         self.monotone_constraints = monotone_constraints_
         self.subsample = subsample
         self.seed = seed
         self.missing = missing
+        self.create_missing_branch = create_missing_branch
 
     def fit(
         self,
         X: FrameLike,
         y: ArrayLike,
         sample_weight: Union[ArrayLike, None] = None,
     ):
```

### Comparing `forust-0.2.3/pyproject.toml` & `forust-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/scratch.py` & `forust-0.2.4/scratch.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/src/lib.rs` & `forust-0.2.4/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         nbins: u16,
         parallel: bool,
         allow_missing_splits: bool,
         monotone_constraints: HashMap<usize, i8>,
         subsample: f32,
         seed: u64,
         missing: f64,
+        create_missing_branch: bool,
     ) -> PyResult<Self> {
         let constraints = int_map_to_constraint_map(monotone_constraints)?;
         let objective_ = match objective_type {
             "LogLoss" => Ok(ObjectiveType::LogLoss),
             "SquaredLoss" => Ok(ObjectiveType::SquaredLoss),
             _ => Err(PyValueError::new_err(format!("Not a valid objective type passed, expected one of 'LogLoss', 'SquaredLoss', but '{}' was provided.", objective_type))),
         }?;
@@ -72,14 +73,15 @@
             nbins,
             parallel,
             allow_missing_splits,
             Some(constraints),
             subsample,
             seed,
             missing,
+            create_missing_branch,
         );
         Ok(GradientBooster { booster })
     }
 
     #[setter]
     fn set_monotone_constraints(&mut self, value: HashMap<usize, i8>) -> PyResult<()> {
         let map = int_map_to_constraint_map(value)?;
@@ -232,14 +234,18 @@
                 "allow_missing_splits",
                 self.booster.allow_missing_splits.to_object(py),
             ),
             ("monotone_constraints", constraints.to_object(py)),
             ("subsample", self.booster.subsample.to_object(py)),
             ("seed", self.booster.seed.to_object(py)),
             ("missing", self.booster.missing.to_object(py)),
+            (
+                "create_missing_branch",
+                self.booster.create_missing_branch.to_object(py),
+            ),
         ];
         let dict = key_vals.into_py_dict(py);
         Ok(dict.to_object(py))
     }
 }
 
 #[pyfunction]
```

### Comparing `forust-0.2.3/tests/test_booster.py` & `forust-0.2.4/tests/test_booster.py`

 * *Files 11% similar despite different names*

```diff
@@ -411,14 +411,57 @@
 
     xmod_contribs = xmod.get_booster().predict(
         xgb.DMatrix(X), approx_contribs=True, pred_contribs=True
     )
     assert np.allclose(fmod_contribs, xmod_contribs, atol=0.000001)
 
 
+def test_missing_branch_with_contributions(X_y):
+    X, y = X_y
+    X = X
+    fmod_miss_leaf = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        base_score=0.5,
+        allow_missing_splits=False,
+        create_missing_branch=True,
+    )
+    fmod_miss_leaf.fit(X, y)
+    fmod_miss_leaf_preds = fmod_miss_leaf.predict(X)
+    fmod_miss_leaf_conts = fmod_miss_leaf.predict_contributions(X)
+    assert np.allclose(fmod_miss_leaf_conts.sum(1), fmod_miss_leaf_preds)
+
+    fmod_miss_branch = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        base_score=0.5,
+        allow_missing_splits=True,
+        create_missing_branch=True,
+    )
+    fmod_miss_branch.fit(X, y)
+    fmod_miss_branch_preds = fmod_miss_branch.predict(X)
+    fmod_miss_branch_conts = fmod_miss_branch.predict_contributions(X)
+    assert np.allclose(fmod_miss_branch_conts.sum(1), fmod_miss_branch_preds)
+    assert not np.allclose(fmod_miss_branch_preds, fmod_miss_leaf_preds)
+
+
 def test_booster_metadata(X_y, tmp_path):
     f64_model_path = tmp_path / "modelf64_sl.json"
     X, y = X_y
     X = X
     fmod = GradientBooster(
         iterations=100,
         learning_rate=0.3,
```

### Comparing `forust-0.2.3/LICENSE` & `forust-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.3/PKG-INFO` & `forust-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forust
-Version: 0.2.3
+Version: 0.2.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.3
 Requires-Dist: maturin; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
@@ -43,15 +43,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.3"
+forust-ml = "0.2.4"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -77,21 +77,22 @@
  - `base_score` ***(float, optional)***: The initial prediction value of the model. Defaults to 0.5.
  - `nbins` ***(int, optional)***: Number of bins to calculate to partition the data. Setting this to
     a smaller number, will result in faster training time, while potentially sacrificing
     accuracy. If there are more bins, than unique values in a column, all unique values
     will be used. Defaults to 256.
  - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
     with this model? Defaults to `True`.
- - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. Defaults to `True`.
+ - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. If `create_missing_branch` is set to `True` having this parameter be set to `True` will result in the missing branch further split, if this parameter is `False` then in that case the missing branch will always be a terminal node. Defaults to `True`.
  - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
  - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
       training a tree. Defaults to 1.0, meaning all data is used for training.
  - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
       algorithm. Defaults to 0.
  - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
+ - `create_missing_branch` ***(bool, optional)***: An experimental parameter, that if `True`, will create a separate branch for missing, creating a ternary tree, the missing node will be given the same weight value as the parent node. If this parameter is `False`, missing will be sent down either the left or right branch, creating a binary tree. Defaults to `False`.
 
 ### Training and Predicting
 
 Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
 In the case of this example, the predictions are the log odds of a given record being 1.
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: forust Version: 0.2.3 Classifier: Programming
+Metadata-Version: 2.1 Name: forust Version: 0.2.4 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy>=1.21 Requires-Dist: pandas>=1.3 Requires-Dist: maturin;
 extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist: seaborn;
 extra == 'dev' Requires-Dist: xgboost==1.6.1; extra == 'dev' Requires-Dist:
 scikit-learn; extra == 'dev' Provides-Extra: dev License-File: LICENSE Summary:
 A lightweight gradient boosting implementation in Rust. Keywords:
@@ -24,15 +24,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.3" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.4" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -56,15 +56,18 @@
 time, while potentially sacrificing accuracy. If there are more bins, than
 unique values in a column, all unique values will be used. Defaults to 256. -
 `parallel` ***(bool, optional)***: Should multiple cores be used when training
 and predicting with this model? Defaults to `True`. - `allow_missing_splits`
 ***(bool, optional)***: Allow for splits to be made such that all missing
 values go down one branch, and all non-missing values go down the other, if
 this results in the greatest reduction of loss. If this is false, splits will
-only be made on non missing values. Defaults to `True`. -
+only be made on non missing values. If `create_missing_branch` is set to `True`
+having this parameter be set to `True` will result in the missing branch
+further split, if this parameter is `False` then in that case the missing
+branch will always be a terminal node. Defaults to `True`. -
 `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are
 used to enforce a specific relationship between the training features and the
 target variable. A dictionary should be provided where the keys are the feature
 index value if the model will be fit on a numpy array, or a feature name if it
 will be fit on a pandas Dataframe. The values of the dictionary should be an
 integer value of -1, 1, or 0 to specify the relationship that should be
 estimated between the respective feature and the target variable. Use a value
@@ -73,51 +76,55 @@
 will not have any constraint applied. If `None` is passed no constraints will
 be enforced on any variable. Defaults to `None`. - `subsample` ***(float,
 optional)***: Percent of records to randomly sample at each iteration when
 training a tree. Defaults to 1.0, meaning all data is used for training. -
 `seed` ***(integer, optional)***: Integer value used to seed any randomness
 used in the algorithm. Defaults to 0. - `missing` ***(float, optional)***:
 Value to consider missing, when training and predicting with the booster.
-Defaults to `np.nan`. ### Training and Predicting Once, the booster has been
-initialized, it can be fit on a provided dataset, and performance field. After
-fitting, the model can be used to predict on a dataset. In the case of this
-example, the predictions are the log odds of a given record being 1. ```python
-# Small example dataset from seaborn import load_dataset df = load_dataset
-("titanic") X = df.select_dtypes("number").drop(columns=["survived"]) y = df
-["survived"] # Initialize a booster with defaults. from forust import
-GradientBooster model = GradientBooster(objective_type="LogLoss") model.fit(X,
-y) # Predict on data model.predict(X.head()) # array([-1.94919663, 2.25863229,
-0.32963671, 2.48732194, -3.00371813]) # predict contributions
-model.predict_contributions(X.head()) # array([[-0.63014213, 0.33880048, -
-0.16520798, -0.07798772, -0.85083578, # -1.07720813], # [ 1.05406709,
-0.08825999, 0.21662544, -0.12083538, 0.35209258, # -1.07720813], ``` The `fit`
-method accepts the following arguments. - `X` ***(FrameLike)***: Either a
-pandas DataFrame, or a 2 dimensional numpy array, with numeric data. - `y` ***
-(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If
-"LogLoss" was the objective type specified, then this should only contain 1 or
-0 values, where 1 is the positive class being predicted. If "SquaredLoss" is
-the objective type, then any continuous variable can be provided. -
-`sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use
-when training the model. If None is passed, a weight of 1 will be used for
-every record. Defaults to None. The predict method accepts the following
-arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2
-dimensional numpy array, with numeric data. - `parallel` ***(Optional[bool],
-optional)***: Optionally specify if the predict function should run in parallel
-on multiple threads. If `None` is passed, the `parallel` attribute of the
-booster will be used. Defaults to `None`. The `predict_contributions` method
-will predict with the fitted booster on new data, returning the feature
-contribution matrix. The last column is the bias term. - `X` ***(FrameLike)***:
+Defaults to `np.nan`. - `create_missing_branch` ***(bool, optional)***: An
+experimental parameter, that if `True`, will create a separate branch for
+missing, creating a ternary tree, the missing node will be given the same
+weight value as the parent node. If this parameter is `False`, missing will be
+sent down either the left or right branch, creating a binary tree. Defaults to
+`False`. ### Training and Predicting Once, the booster has been initialized, it
+can be fit on a provided dataset, and performance field. After fitting, the
+model can be used to predict on a dataset. In the case of this example, the
+predictions are the log odds of a given record being 1. ```python # Small
+example dataset from seaborn import load_dataset df = load_dataset("titanic") X
+= df.select_dtypes("number").drop(columns=["survived"]) y = df["survived"] #
+Initialize a booster with defaults. from forust import GradientBooster model =
+GradientBooster(objective_type="LogLoss") model.fit(X, y) # Predict on data
+model.predict(X.head()) # array([-1.94919663, 2.25863229, 0.32963671,
+2.48732194, -3.00371813]) # predict contributions model.predict_contributions
+(X.head()) # array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -
+0.85083578, # -1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -
+0.12083538, 0.35209258, # -1.07720813], ``` The `fit` method accepts the
+following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2
+dimensional numpy array, with numeric data. - `y` ***(ArrayLike)***: Either a
+pandas Series, or a 1 dimensional numpy array. If "LogLoss" was the objective
+type specified, then this should only contain 1 or 0 values, where 1 is the
+positive class being predicted. If "SquaredLoss" is the objective type, then
+any continuous variable can be provided. - `sample_weight` ***(Optional
+[ArrayLike], optional)***: Instance weights to use when training the model. If
+None is passed, a weight of 1 will be used for every record. Defaults to None.
+The predict method accepts the following arguments. - `X` ***(FrameLike)***:
 Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
 `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
 function should run in parallel on multiple threads. If `None` is passed, the
-`parallel` attribute of the booster will be used. Defaults to `None`. ###
-Inspecting the Model Once the booster has been fit, each individual tree
-structure can be retrieved in text form, using the `text_dump` method. This
-method returns a list, the same length as the number of trees in the model.
-```python model.text_dump()[0] # 0:[0 < 3]
+`parallel` attribute of the booster will be used. Defaults to `None`. The
+`predict_contributions` method will predict with the fitted booster on new
+data, returning the feature contribution matrix. The last column is the bias
+term. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional
+numpy array, with numeric data. - `parallel` ***(Optional[bool], optional)***:
+Optionally specify if the predict function should run in parallel on multiple
+threads. If `None` is passed, the `parallel` attribute of the booster will be
+used. Defaults to `None`. ### Inspecting the Model Once the booster has been
+fit, each individual tree structure can be retrieved in text form, using the
+`text_dump` method. This method returns a list, the same length as the number
+of trees in the model. ```python model.text_dump()[0] # 0:[0 < 3]
 yes=1,no=2,missing=2,gain=91.50833,cover=209.388307 # 1:[4 < 13.7917]
 yes=3,no=4,missing=4,gain=28.185467,cover=94.00148 # 3:[1 < 18]
 yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348 # 7:[1 < 17]
 yes=15,no=16,missing=16,gain=0.691266,cover=0.705011 # 15:leaf=-
 0.15120,cover=0.23500 # 16:leaf=0.154097,cover=0.470007 ``` The `json_dump`
 method performs the same action, but returns the model as a json representation
 rather than a text string. To see an estimate for how a given feature is used
```

