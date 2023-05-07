# Comparing `tmp/plotfish2-0.1.3.tar.gz` & `tmp/plotfish2-0.1.4.tar.gz`

## Comparing `plotfish2-0.1.3.tar` & `plotfish2-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 plotfish2-0.1.3/Cargo.toml
--rw-r--r--   0      501       20     2809 2023-04-16 04:25:51.000000 plotfish2-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0      501       20      759 2023-04-16 04:25:51.000000 plotfish2-0.1.3/.gitignore
--rw-r--r--   0      501       20      238 2023-05-03 02:29:55.000000 plotfish2-0.1.3/example.py
--rw-r--r--   0      501       20      966 2023-05-03 02:29:55.000000 plotfish2-0.1.3/index.js
--rw-r--r--   0      501       20     1160 2023-04-16 04:25:51.000000 plotfish2-0.1.3/package-lock.json
--rw-r--r--   0      501       20      522 2023-04-16 04:25:51.000000 plotfish2-0.1.3/package.json
--rw-r--r--   0      501       20      413 2023-05-07 02:36:19.000000 plotfish2-0.1.3/pyproject.toml
--rw-r--r--   0      501       20      777 2023-05-03 02:29:55.000000 plotfish2-0.1.3/python/plotfish/__init__.py
--rw-r--r--   0      501       20        0 2023-04-16 04:25:51.000000 plotfish2-0.1.3/python/plotfish/plotfish.pyi
--rw-r--r--   0      501       20        0 2023-04-16 04:25:51.000000 plotfish2-0.1.3/python/plotfish/py.typed
--rw-r--r--   0      501       20     6845 2023-05-07 02:35:29.000000 plotfish2-0.1.3/src/lib.rs
--rw-r--r--   0      501       20    34903 2023-04-16 04:20:34.000000 plotfish2-0.1.3/Cargo.lock
--rw-r--r--   0        0        0      258 1970-01-01 00:00:00.000000 plotfish2-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 plotfish2-0.1.4/Cargo.toml
+-rw-r--r--   0      501       20     2809 2023-04-16 04:25:51.000000 plotfish2-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      759 2023-04-16 04:25:51.000000 plotfish2-0.1.4/.gitignore
+-rw-r--r--   0      501       20      238 2023-05-03 02:29:55.000000 plotfish2-0.1.4/example.py
+-rw-r--r--   0      501       20      966 2023-05-03 02:29:55.000000 plotfish2-0.1.4/index.js
+-rw-r--r--   0      501       20     1160 2023-04-16 04:25:51.000000 plotfish2-0.1.4/package-lock.json
+-rw-r--r--   0      501       20      522 2023-04-16 04:25:51.000000 plotfish2-0.1.4/package.json
+-rw-r--r--   0      501       20      413 2023-05-07 02:45:01.000000 plotfish2-0.1.4/pyproject.toml
+-rw-r--r--   0      501       20      777 2023-05-03 02:29:55.000000 plotfish2-0.1.4/python/plotfish/__init__.py
+-rw-r--r--   0      501       20        0 2023-04-16 04:25:51.000000 plotfish2-0.1.4/python/plotfish/plotfish.pyi
+-rw-r--r--   0      501       20        0 2023-04-16 04:25:51.000000 plotfish2-0.1.4/python/plotfish/py.typed
+-rw-r--r--   0      501       20     6846 2023-05-07 02:44:08.000000 plotfish2-0.1.4/src/lib.rs
+-rw-r--r--   0      501       20    34903 2023-04-16 04:20:34.000000 plotfish2-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0      258 1970-01-01 00:00:00.000000 plotfish2-0.1.4/PKG-INFO
```

### Comparing `plotfish2-0.1.3/Cargo.toml` & `plotfish2-0.1.4/Cargo.toml`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.3/.github/workflows/CI.yml` & `plotfish2-0.1.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.3/.gitignore` & `plotfish2-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.3/index.js` & `plotfish2-0.1.4/index.js`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.3/package-lock.json` & `plotfish2-0.1.4/package-lock.json`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.3/package.json` & `plotfish2-0.1.4/package.json`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.3/python/plotfish/__init__.py` & `plotfish2-0.1.4/python/plotfish/__init__.py`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.3/src/lib.rs` & `plotfish2-0.1.4/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     time::{sleep_until, Instant},
 };
 
 // TODO: Error handling
 
 /// A Python module implemented in Rust.
 #[derive(Serialize, Clone)]
-#[serde(rename_all = "snake_case", tag = "plot_type")]
+#[serde(rename_all = "snake_case", tag = "metricType")]
 pub enum PlotType {
     Line { value: f64 },
     Counter { change: f64 },
     ProgressBar { value: f64, total: f64 },
 }
 
 #[derive(Serialize, Clone)]
```

### Comparing `plotfish2-0.1.3/Cargo.lock` & `plotfish2-0.1.4/Cargo.lock`

 * *Files identical despite different names*

