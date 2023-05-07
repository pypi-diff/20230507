# Comparing `tmp/pep440_rs-0.3.6.tar.gz` & `tmp/pep440_rs-0.3.7.tar.gz`

## Comparing `pep440_rs-0.3.6.tar` & `pep440_rs-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 pep440_rs-0.3.6/Cargo.toml
--rw-r--r--   0      501       20      901 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/Changelog.md
--rw-r--r--   0      501       20    10173 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/License-Apache
--rw-r--r--   0      501       20     1293 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/License-BSD
--rw-r--r--   0      501       20     2981 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/Readme.md
--rw-r--r--   0      501       20      274 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/pyproject.toml
--rw-r--r--   0      501       20     2105 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/python/Readme.md
--rw-r--r--   0      501       20     4043 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/src/lib.rs
--rw-r--r--   0      501       20    39057 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/src/version.rs
--rw-r--r--   0      501       20    42526 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/src/version_specifier.rs
--rw-r--r--   0      501       20    10917 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/Cargo.lock
--rw-r--r--   0      501       20     1084 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/python/pep440_rs/__init__.pyi
--rw-r--r--   0      501       20      534 2023-04-24 11:02:04.000000 pep440_rs-0.3.6/python/pep440_rs/__init__.py
--rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 pep440_rs-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 pep440_rs-0.3.7/Cargo.toml
+-rw-r--r--   0      501       20      901 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/Changelog.md
+-rw-r--r--   0      501       20    10173 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/License-Apache
+-rw-r--r--   0      501       20     1293 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/License-BSD
+-rw-r--r--   0      501       20     2981 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/Readme.md
+-rw-r--r--   0      501       20      312 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/pyproject.toml
+-rw-r--r--   0      501       20     2105 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/python/Readme.md
+-rw-r--r--   0      501       20     4043 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/src/lib.rs
+-rw-r--r--   0      501       20    39609 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/src/version.rs
+-rw-r--r--   0      501       20    42546 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/src/version_specifier.rs
+-rw-r--r--   0      501       20    10916 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/Cargo.lock
+-rw-r--r--   0      501       20     1131 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/python/pep440_rs/__init__.pyi
+-rw-r--r--   0      501       20      534 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/python/pep440_rs/__init__.py
+-rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 pep440_rs-0.3.7/PKG-INFO
```

### Comparing `pep440_rs-0.3.6/Changelog.md` & `pep440_rs-0.3.7/Changelog.md`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.6/License-Apache` & `pep440_rs-0.3.7/License-Apache`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.6/License-BSD` & `pep440_rs-0.3.7/License-BSD`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.6/Readme.md` & `pep440_rs-0.3.7/Readme.md`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.6/python/Readme.md` & `pep440_rs-0.3.7/python/Readme.md`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.6/src/lib.rs` & `pep440_rs-0.3.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.6/src/version.rs` & `pep440_rs-0.3.7/src/version.rs`

 * *Files 2% similar despite different names*

```diff
@@ -340,14 +340,30 @@
     }
     /// The [developmental release](https://peps.python.org/pep-0440/#developmental-releases),
     /// if any
     #[getter]
     pub fn dev(&self) -> Option<usize> {
         self.0.dev
     }
+    /// The first item of release or 0 if unavailable.
+    #[getter]
+    #[allow(clippy::get_first)]
+    pub fn major(&self) -> usize {
+        self.release().get(0).cloned().unwrap_or_default()
+    }
+    /// The second item of release or 0 if unavailable.
+    #[getter]
+    pub fn minor(&self) -> usize {
+        self.release().get(1).cloned().unwrap_or_default()
+    }
+    /// The third item of release or 0 if unavailable.
+    #[getter]
+    pub fn micro(&self) -> usize {
+        self.release().get(2).cloned().unwrap_or_default()
+    }
 
     /// Parses a PEP 440 version string
     #[cfg(feature = "pyo3")]
     #[new]
     pub fn parse(version: String) -> PyResult<Self> {
         Ok(Self(
             Version::from_str(&version).map_err(PyValueError::new_err)?,
@@ -369,15 +385,15 @@
     pub fn __str__(&self) -> String {
         self.0.to_string()
     }
 
     /// Returns the normalized representation
     #[cfg(feature = "pyo3")]
     pub fn __repr__(&self) -> String {
-        format!(r#""{}""#, self.0)
+        format!(r#"<Version("{}")>"#, self.0)
     }
 
     /// Returns the normalized representation
     #[cfg(feature = "pyo3")]
     pub fn __hash__(&self) -> u64 {
         let mut hasher = DefaultHasher::new();
         self.0.hash(&mut hasher);
@@ -761,14 +777,15 @@
             .name("release")
             // Should be forbidden by the regex
             .ok_or_else(|| "No release in version".to_string())?
             .as_str()
             .split('.')
             .map(|segment| segment.parse::<usize>().map_err(|err| err.to_string()))
             .collect::<Result<Vec<usize>, String>>()?;
+
         let star = captures.name("trailing_dot_star").is_some();
         if star {
             if pre.is_some() {
                 return Err(
                     "You can't have both a trailing `.*` and a prerelease version".to_string(),
                 );
             }
```

### Comparing `pep440_rs-0.3.6/src/version_specifier.rs` & `pep440_rs-0.3.7/src/version_specifier.rs`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
     /// Returns the normalized representation
     pub fn __str__(&self) -> String {
         self.to_string()
     }
 
     /// Returns the normalized representation
     pub fn __repr__(&self) -> String {
-        format!(r#""{}""#, self)
+        format!(r#"<VersionSpecifier("{}")>"#, self)
     }
 
     fn __richcmp__(&self, other: &Self, op: CompareOp) -> PyResult<bool> {
         if matches!(op, CompareOp::Eq) {
             Ok(self == other)
         } else {
             Err(PyNotImplementedError::new_err(
```

### Comparing `pep440_rs-0.3.6/Cargo.lock` & `pep440_rs-0.3.7/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.143"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "edc207893e85c5d6be840e969b496b53d94cec8be2d501b214f50daa97fa8024"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -105,15 +105,15 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "pep440_rs"
-version = "0.3.6"
+version = "0.3.7"
 dependencies = [
  "indoc 2.0.1",
  "lazy_static",
  "pyo3",
  "regex",
  "serde",
  "tracing",
@@ -234,26 +234,26 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.160"
+version = "1.0.162"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
+checksum = "71b2f6e1ab5c2b98c05f0f35b236b22e8df7ead6ffbf51d7808da7f8817e7ab6"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.160"
+version = "1.0.162"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
+checksum = "a2a0814352fd64b58489904a44ea8d90cb1a91dcb6b4f5ebabc32c8318e93cb6"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
@@ -282,17 +282,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tracing"
 version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
@@ -300,21 +300,21 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
```

### Comparing `pep440_rs-0.3.6/python/pep440_rs/__init__.pyi` & `pep440_rs-0.3.7/python/pep440_rs/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # Generated by `stubgen -p pep440_rs`
 from typing import Any, ClassVar
 
+
 class Version:
     dev: Any
     epoch: Any
     post: Any
     pre: Any
     release: Any
+    major: Any
+    minor: Any
+    micro: Any
 
     @classmethod
     def __init__(cls, *args, **kwargs) -> None: ...
     def any_prerelease(self, *args, **kwargs) -> Any: ...
     def parse_star(self, *args, **kwargs) -> Any: ...
     def __eq__(self, other) -> Any: ...
     def __ge__(self, other) -> Any: ...
     def __gt__(self, other) -> Any: ...
     def __hash__(self) -> Any: ...
     def __le__(self, other) -> Any: ...
     def __lt__(self, other) -> Any: ...
     def __ne__(self, other) -> Any: ...
 
+
 class VersionSpecifier:
     __hash__: ClassVar[None] = ...
 
     @classmethod
     def __init__(cls, *args, **kwargs) -> None: ...
     def contains(self, *args, **kwargs) -> Any: ...
     def __contains__(self, other) -> Any: ...
```

### Comparing `pep440_rs-0.3.6/python/pep440_rs/__init__.py` & `pep440_rs-0.3.7/python/pep440_rs/__init__.py`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.6/PKG-INFO` & `pep440_rs-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pep440_rs
-Version: 0.3.6
+Version: 0.3.7
 Summary: A library for python version numbers and specifiers, implementing PEP 440
 License: Apache-2.0 OR BSD-2-Clause
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/konstin/pep440-rs
 
 # PEP440 in rust
```

