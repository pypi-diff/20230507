# Comparing `tmp/plotfish2-0.1.1.tar.gz` & `tmp/plotfish2-0.1.2.tar.gz`

## Comparing `plotfish2-0.1.1.tar` & `plotfish2-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 plotfish2-0.1.1/Cargo.toml
--rw-r--r--   0      501       20     2809 2023-04-16 04:25:51.000000 plotfish2-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0      501       20      759 2023-04-16 04:25:51.000000 plotfish2-0.1.1/.gitignore
--rw-r--r--   0      501       20      238 2023-04-27 03:04:56.000000 plotfish2-0.1.1/example.py
--rw-r--r--   0      501       20      966 2023-04-27 02:57:29.000000 plotfish2-0.1.1/index.js
--rw-r--r--   0      501       20     1160 2023-04-16 04:25:51.000000 plotfish2-0.1.1/package-lock.json
--rw-r--r--   0      501       20      522 2023-04-16 04:25:51.000000 plotfish2-0.1.1/package.json
--rw-r--r--   0      501       20      413 2023-04-29 21:01:15.000000 plotfish2-0.1.1/pyproject.toml
--rw-r--r--   0      501       20      777 2023-04-29 20:56:32.000000 plotfish2-0.1.1/python/plotfish/__init__.py
--rw-r--r--   0      501       20        0 2023-04-16 04:25:51.000000 plotfish2-0.1.1/python/plotfish/plotfish.pyi
--rw-r--r--   0      501       20        0 2023-04-16 04:25:51.000000 plotfish2-0.1.1/python/plotfish/py.typed
--rw-r--r--   0      501       20     6718 2023-04-20 02:37:31.000000 plotfish2-0.1.1/src/lib.rs
--rw-r--r--   0      501       20    34903 2023-04-16 04:20:34.000000 plotfish2-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      258 1970-01-01 00:00:00.000000 plotfish2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 plotfish2-0.1.2/Cargo.toml
+-rw-r--r--   0      501       20     2809 2023-04-16 04:25:51.000000 plotfish2-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      759 2023-04-16 04:25:51.000000 plotfish2-0.1.2/.gitignore
+-rw-r--r--   0      501       20      238 2023-05-03 02:29:55.000000 plotfish2-0.1.2/example.py
+-rw-r--r--   0      501       20      966 2023-05-03 02:29:55.000000 plotfish2-0.1.2/index.js
+-rw-r--r--   0      501       20     1160 2023-04-16 04:25:51.000000 plotfish2-0.1.2/package-lock.json
+-rw-r--r--   0      501       20      522 2023-04-16 04:25:51.000000 plotfish2-0.1.2/package.json
+-rw-r--r--   0      501       20      413 2023-05-07 02:33:38.000000 plotfish2-0.1.2/pyproject.toml
+-rw-r--r--   0      501       20      777 2023-05-03 02:29:55.000000 plotfish2-0.1.2/python/plotfish/__init__.py
+-rw-r--r--   0      501       20        0 2023-04-16 04:25:51.000000 plotfish2-0.1.2/python/plotfish/plotfish.pyi
+-rw-r--r--   0      501       20        0 2023-04-16 04:25:51.000000 plotfish2-0.1.2/python/plotfish/py.typed
+-rw-r--r--   0      501       20     6845 2023-05-07 00:04:12.000000 plotfish2-0.1.2/src/lib.rs
+-rw-r--r--   0      501       20    34903 2023-04-16 04:20:34.000000 plotfish2-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      258 1970-01-01 00:00:00.000000 plotfish2-0.1.2/PKG-INFO
```

### Comparing `plotfish2-0.1.1/Cargo.toml` & `plotfish2-0.1.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.1/.github/workflows/CI.yml` & `plotfish2-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.1/.gitignore` & `plotfish2-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.1/index.js` & `plotfish2-0.1.2/index.js`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.1/package-lock.json` & `plotfish2-0.1.2/package-lock.json`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.1/package.json` & `plotfish2-0.1.2/package.json`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.1/python/plotfish/__init__.py` & `plotfish2-0.1.2/python/plotfish/__init__.py`

 * *Files identical despite different names*

### Comparing `plotfish2-0.1.1/src/lib.rs` & `plotfish2-0.1.2/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -27,32 +27,34 @@
     Counter { change: f64 },
     ProgressBar { value: f64, total: f64 },
 }
 
 #[derive(Serialize, Clone)]
 struct Datapoint {
     #[serde(flatten)]
-    plot_type: PlotType,
-    plot_name: String,
+    #[serde(rename(serialize = "metricType"))]
+    metric_type: PlotType,
+    #[serde(rename(serialize = "metricName"))]
+    metric_name: String,
     timestamp: u128,
 }
 
 struct FishingRod {
     riverbed_url: String,
     runtime: Runtime,
     http_client: reqwest::Client,
     api_key: String,
     datapoints_buffer: Arc<Mutex<Vec<Datapoint>>>,
 }
 
-fn get_nanoseconds_since_epoch() -> u128 {
+fn get_milliseconds_since_epoch() -> u128 {
     SystemTime::now()
         .duration_since(UNIX_EPOCH)
         .unwrap()
-        .as_nanos()
+        .as_millis()
 }
 
 impl Finalize for FishingRod {}
 
 impl FishingRod {
     pub fn new(riverbed_url: String, api_key: String) -> Self {
         let runtime = Builder::new_multi_thread()
@@ -102,17 +104,17 @@
             }
         });
     }
 
     async fn record_datapoint(&self, plot_name: String, plot_type: PlotType) {
         let mut datapoints_buffer = self.datapoints_buffer.lock().await;
         datapoints_buffer.push(Datapoint {
-            plot_type,
-            plot_name,
-            timestamp: get_nanoseconds_since_epoch(),
+            metric_type: plot_type,
+            metric_name: plot_name,
+            timestamp: get_milliseconds_since_epoch(),
         });
     }
 
     pub fn record_datapoint_blocking(&self, plot_name: String, plot_type: PlotType) {
         self.runtime
             .block_on(self.record_datapoint(plot_name, plot_type));
     }
```

### Comparing `plotfish2-0.1.1/Cargo.lock` & `plotfish2-0.1.2/Cargo.lock`

 * *Files identical despite different names*

