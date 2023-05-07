# Comparing `tmp/cramjam-2.7.0rc2.tar.gz` & `tmp/cramjam-2.7.0rc3.tar.gz`

## Comparing `cramjam-2.7.0rc2.tar` & `cramjam-2.7.0rc3.tar`

### file list

```diff
@@ -1,49 +1,53 @@
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 cramjam-2.7.0rc2/Cargo.toml
--rw-r--r--   0      501       20      112 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/.cargo/config
--rw-r--r--   0      501       20     7819 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/.github/workflows/CI.yml
--rw-r--r--   0      501       20     1854 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/.gitignore
--rw-r--r--   0      501       20     1070 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/LICENSE
--rw-r--r--   0      501       20      971 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/Makefile
--rw-r--r--   0      501       20     3075 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/README.md
--rw-r--r--   0      501       20      121 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/benchmark-requirements.txt
--rw-r--r--   0      501       20    75826 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/benchmarks/README.md
--rw-r--r--   0      501       20     1167 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/benchmarks/data/COPYING
--rw-r--r--   0      501       20    14168 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/Mark.Twain-Tom.Sawyer.txt
--rw-r--r--   0      501       20   152089 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/alice29.txt
--rw-r--r--   0      501       20   125179 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/asyoulik.txt
--rw-r--r--   0      501       20   123093 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/fireworks.jpeg
--rw-r--r--   0      501       20   118588 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/geo.protodata
--rw-r--r--   0      501       20   102400 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/html
--rw-r--r--   0      501       20   409600 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/html_x_4
--rw-r--r--   0      501       20   184320 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/kppkn.gtb
--rw-r--r--   0      501       20   426754 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/lcet10.txt
--rw-r--r--   0      501       20   102400 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/paper-100k.pdf
--rw-r--r--   0      501       20   481861 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/plrabn12.txt
--rw-r--r--   0      501       20   702087 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/urls.10K
--rw-r--r--   0      501       20     7670 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/test_bench.py
--rw-r--r--   0      501       20       66 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/dev-requirements.txt
--rw-r--r--   0      501       20      422 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/pyproject.toml
--rw-r--r--   0      501       20       15 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/rustfmt.toml
--rw-r--r--   0      501       20     4381 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/brotli.rs
--rw-r--r--   0      501       20     4239 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/bzip2.rs
--rw-r--r--   0      501       20     4323 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/deflate.rs
--rw-r--r--   0      501       20      577 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/exceptions.rs
--rw-r--r--   0      501       20     4875 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/gzip.rs
--rw-r--r--   0      501       20    18803 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/io.rs
--rw-r--r--   0      501       20    17757 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/lib.rs
--rw-r--r--   0      501       20    10417 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/lz4.rs
--rw-r--r--   0      501       20     6754 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/snappy.rs
--rw-r--r--   0      501       20     4179 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/zstd.rs
--rw-r--r--   0      501       20        0 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/tests/__init__.py
--rw-r--r--   0      501       20      857 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt
--rw-r--r--   0      501       20      375 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.br
--rw-r--r--   0      501       20      495 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.bz2
--rw-r--r--   0      501       20      472 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.gz
--rw-r--r--   0      501       20      665 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.lz4
--rw-r--r--   0      501       20      660 2023-04-29 05:00:15.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.snappy
--rw-r--r--   0      501       20      465 2023-04-29 05:00:15.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.zst
--rw-r--r--   0      501       20     1140 2023-04-29 05:00:15.000000 cramjam-2.7.0rc2/tests/test_integration.py
--rw-r--r--   0      501       20     1481 2023-04-29 05:00:15.000000 cramjam-2.7.0rc2/tests/test_rust_io.py
--rw-r--r--   0      501       20    10785 2023-04-29 05:00:15.000000 cramjam-2.7.0rc2/tests/test_variants.py
--rw-r--r--   0      501       20    12043 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/Cargo.lock
--rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 cramjam-2.7.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      332 1970-01-01 00:00:00.000000 cramjam-2.7.0rc3/local_dependencies/libcramjam/Cargo.toml
+-rw-r--r--   0      501       20      119 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/local_dependencies/libcramjam/README.md
+-rw-r--r--   0      501       20      960 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/local_dependencies/libcramjam/src/brotli.rs
+-rw-r--r--   0      501       20      846 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/local_dependencies/libcramjam/src/bzip2.rs
+-rw-r--r--   0      501       20      878 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/local_dependencies/libcramjam/src/deflate.rs
+-rw-r--r--   0      501       20     1442 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/local_dependencies/libcramjam/src/gzip.rs
+-rw-r--r--   0      501       20     3637 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/local_dependencies/libcramjam/src/lib.rs
+-rw-r--r--   0      501       20     1230 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/local_dependencies/libcramjam/src/lz4.rs
+-rw-r--r--   0      501       20     1690 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/local_dependencies/libcramjam/src/snappy.rs
+-rw-r--r--   0      501       20      837 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/local_dependencies/libcramjam/src/zstd.rs
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 cramjam-2.7.0rc3/Cargo.toml
+-rw-r--r--   0      501       20      971 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/Makefile
+-rw-r--r--   0      501       20     3152 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/README.md
+-rw-r--r--   0      501       20      121 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmark-requirements.txt
+-rw-r--r--   0      501       20    75826 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/README.md
+-rw-r--r--   0      501       20     1167 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/COPYING
+-rw-r--r--   0      501       20    14168 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/Mark.Twain-Tom.Sawyer.txt
+-rw-r--r--   0      501       20   152089 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/alice29.txt
+-rw-r--r--   0      501       20   125179 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/asyoulik.txt
+-rw-r--r--   0      501       20   123093 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/fireworks.jpeg
+-rw-r--r--   0      501       20   118588 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/geo.protodata
+-rw-r--r--   0      501       20   102400 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/html
+-rw-r--r--   0      501       20   409600 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/html_x_4
+-rw-r--r--   0      501       20   184320 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/kppkn.gtb
+-rw-r--r--   0      501       20   426754 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/lcet10.txt
+-rw-r--r--   0      501       20   102400 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/paper-100k.pdf
+-rw-r--r--   0      501       20   481861 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/plrabn12.txt
+-rw-r--r--   0      501       20   702087 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/data/urls.10K
+-rw-r--r--   0      501       20     7670 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/benchmarks/test_bench.py
+-rw-r--r--   0      501       20      575 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/pyproject.toml
+-rw-r--r--   0      501       20     3612 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/src/brotli.rs
+-rw-r--r--   0      501       20     3484 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/src/bzip2.rs
+-rw-r--r--   0      501       20     3541 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/src/deflate.rs
+-rw-r--r--   0      501       20      577 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/src/exceptions.rs
+-rw-r--r--   0      501       20     3477 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/src/gzip.rs
+-rw-r--r--   0      501       20    20445 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/src/io.rs
+-rw-r--r--   0      501       20    14277 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/src/lib.rs
+-rw-r--r--   0      501       20     9192 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/src/lz4.rs
+-rw-r--r--   0      501       20     6151 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/src/snappy.rs
+-rw-r--r--   0      501       20     3441 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/src/zstd.rs
+-rw-r--r--   0      501       20        0 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/tests/__init__.py
+-rw-r--r--   0      501       20      857 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/tests/data/integration/plaintext.txt
+-rw-r--r--   0      501       20      375 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/tests/data/integration/plaintext.txt.br
+-rw-r--r--   0      501       20      495 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/tests/data/integration/plaintext.txt.bz2
+-rw-r--r--   0      501       20      472 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/tests/data/integration/plaintext.txt.gz
+-rw-r--r--   0      501       20      665 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/tests/data/integration/plaintext.txt.lz4
+-rw-r--r--   0      501       20      660 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/tests/data/integration/plaintext.txt.snappy
+-rw-r--r--   0      501       20      465 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/tests/data/integration/plaintext.txt.zst
+-rw-r--r--   0      501       20     1140 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/tests/test_integration.py
+-rw-r--r--   0      501       20     1481 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/tests/test_rust_io.py
+-rw-r--r--   0      501       20    11545 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/tests/test_variants.py
+-rw-r--r--   0      501       20    19416 2023-05-07 09:50:40.000000 cramjam-2.7.0rc3/Cargo.lock
+-rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 cramjam-2.7.0rc3/PKG-INFO
```

### Comparing `cramjam-2.7.0rc2/Makefile` & `cramjam-2.7.0rc3/Makefile`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/README.md` & `cramjam-2.7.0rc3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-# pyrus-cramjam
+# cramjam-python
 
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![CI](https://github.com/milesgranger/pyrus-cramjam/workflows/CI/badge.svg?branch=master)](https://github.com/milesgranger/pyrus-cramjam/actions?query=branch=master)
 [![PyPI](https://img.shields.io/pypi/v/cramjam.svg)](https://pypi.org/project/cramjam)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/cramjam/badges/version.svg)](https://anaconda.org/conda-forge/cramjam)
 [![Downloads](https://pepy.tech/badge/cramjam/month)](https://pepy.tech/project/cramjam)
 
 [API Documentation](https://docs.rs/cramjam)
 
 ### Install
 ```commandline
 pip install --upgrade cramjam  # Requires no Python or system dependencies!
 ```
 
+### CLI
+
+A CLI interface is available as [`cramjam-cli`](./../cramjam-cli)
+
 ---
 
 Extremely thin Python bindings to de/compression algorithms in Rust.
 Allows for using algorithms such as Snappy, without any system dependencies.
 
 This is handy when being used in environments like AWS Lambda, where installing
 packages like `python-snappy` becomes difficult because of system level dependencies.
```

### Comparing `cramjam-2.7.0rc2/benchmarks/README.md` & `cramjam-2.7.0rc3/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/COPYING` & `cramjam-2.7.0rc3/benchmarks/data/COPYING`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/Mark.Twain-Tom.Sawyer.txt` & `cramjam-2.7.0rc3/benchmarks/data/Mark.Twain-Tom.Sawyer.txt`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/alice29.txt` & `cramjam-2.7.0rc3/benchmarks/data/alice29.txt`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/asyoulik.txt` & `cramjam-2.7.0rc3/benchmarks/data/asyoulik.txt`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/fireworks.jpeg` & `cramjam-2.7.0rc3/benchmarks/data/fireworks.jpeg`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/geo.protodata` & `cramjam-2.7.0rc3/benchmarks/data/geo.protodata`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/html` & `cramjam-2.7.0rc3/benchmarks/data/html`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/html_x_4` & `cramjam-2.7.0rc3/benchmarks/data/html_x_4`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/kppkn.gtb` & `cramjam-2.7.0rc3/benchmarks/data/kppkn.gtb`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/lcet10.txt` & `cramjam-2.7.0rc3/benchmarks/data/lcet10.txt`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/paper-100k.pdf` & `cramjam-2.7.0rc3/benchmarks/data/paper-100k.pdf`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/plrabn12.txt` & `cramjam-2.7.0rc3/benchmarks/data/plrabn12.txt`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/data/urls.10K` & `cramjam-2.7.0rc3/benchmarks/data/urls.10K`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/benchmarks/test_bench.py` & `cramjam-2.7.0rc3/benchmarks/test_bench.py`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/src/brotli.rs` & `cramjam-2.7.0rc3/src/gzip.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,87 @@
-//! brotli de/compression interface
+//! gzip de/compression interface
 use crate::exceptions::{CompressionError, DecompressionError};
-use crate::io::RustyBuffer;
-use crate::{AsBytes, BytesType};
+use crate::io::{AsBytes, RustyBuffer};
+use crate::BytesType;
 use pyo3::prelude::*;
 use pyo3::wrap_pyfunction;
 use pyo3::PyResult;
-use std::io::{Cursor, Write};
+use std::io::Cursor;
 
-const DEFAULT_COMPRESSION_LEVEL: u32 = 11;
-const BUF_SIZE: usize = 1 << 17; // Taken from brotli kCompressFragementTwoPassBlockSize
-const LGWIN: u32 = 22;
+const DEFAULT_COMPRESSION_LEVEL: u32 = 6;
 
 pub(crate) fn init_py_module(m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(compress, m)?)?;
     m.add_function(wrap_pyfunction!(decompress, m)?)?;
     m.add_function(wrap_pyfunction!(compress_into, m)?)?;
     m.add_function(wrap_pyfunction!(decompress_into, m)?)?;
     m.add_class::<Compressor>()?;
     m.add_class::<Decompressor>()?;
     Ok(())
 }
 
-/// Brotli decompression.
+/// Gzip decompression.
 ///
 /// Python Example
 /// --------------
 /// ```python
-/// >>> cramjam.brotli.decompress(compressed_bytes, output_len=Optional[int])
+/// >>> cramjam.gzip.decompress(compressed_bytes, output_len=Optional[int])
 /// ```
 #[pyfunction]
 pub fn decompress(py: Python, data: BytesType, output_len: Option<usize>) -> PyResult<RustyBuffer> {
-    crate::generic!(py, internal::decompress[data], output_len = output_len).map_err(DecompressionError::from_err)
+    crate::generic!(py, libcramjam::gzip::decompress[data], output_len = output_len)
+        .map_err(DecompressionError::from_err)
 }
 
-/// Brotli compression.
+/// Gzip compression.
 ///
 /// Python Example
 /// --------------
 /// ```python
-/// >>> cramjam.brotli.compress(b'some bytes here', level=9, output_len=Option[int])  # level defaults to 11
+/// >>> cramjam.gzip.compress(b'some bytes here', level=2, output_len=Optional[int])  # Level defaults to 6
 /// ```
 #[pyfunction]
 pub fn compress(py: Python, data: BytesType, level: Option<u32>, output_len: Option<usize>) -> PyResult<RustyBuffer> {
-    crate::generic!(py, internal::compress[data], output_len = output_len, level = level)
-        .map_err(CompressionError::from_err)
+    crate::generic!(
+        py,
+        libcramjam::gzip::compress[data],
+        output_len = output_len,
+        level = level
+    )
+    .map_err(CompressionError::from_err)
 }
 
 /// Compress directly into an output buffer
 #[pyfunction]
 pub fn compress_into(py: Python, input: BytesType, mut output: BytesType, level: Option<u32>) -> PyResult<usize> {
-    crate::generic!(py, internal::compress[input, output], level=level).map_err(CompressionError::from_err)
+    crate::generic!(py, libcramjam::gzip::compress[input, output], level = level).map_err(CompressionError::from_err)
 }
 
 /// Decompress directly into an output buffer
 #[pyfunction]
 pub fn decompress_into(py: Python, input: BytesType, mut output: BytesType) -> PyResult<usize> {
-    crate::generic!(py, internal::decompress[input, output]).map_err(DecompressionError::from_err)
+    crate::generic!(py, libcramjam::gzip::decompress[input, output]).map_err(DecompressionError::from_err)
 }
 
-/// Brotli Compressor object for streaming compression
+/// GZIP Compressor object for streaming compression
 #[pyclass]
 pub struct Compressor {
-    inner: Option<brotli::CompressorWriter<Cursor<Vec<u8>>>>,
+    inner: Option<libcramjam::gzip::flate2::write::GzEncoder<Cursor<Vec<u8>>>>,
 }
 
 #[pymethods]
 impl Compressor {
     /// Initialize a new `Compressor` instance.
     #[new]
     pub fn __init__(level: Option<u32>) -> PyResult<Self> {
-        let level = level.unwrap_or_else(|| DEFAULT_COMPRESSION_LEVEL);
-        let inner = brotli::CompressorWriter::new(Cursor::new(vec![]), BUF_SIZE, level, LGWIN);
+        let level = level.unwrap_or(DEFAULT_COMPRESSION_LEVEL);
+        let inner = libcramjam::gzip::flate2::write::GzEncoder::new(
+            Cursor::new(vec![]),
+            libcramjam::gzip::flate2::Compression::new(level),
+        );
         Ok(Self { inner: Some(inner) })
     }
 
     /// Compress input into the current compressor's stream.
     pub fn compress(&mut self, input: &[u8]) -> PyResult<usize> {
         crate::io::stream_compress(&mut self.inner, input)
     }
@@ -83,38 +90,12 @@
     pub fn flush(&mut self) -> PyResult<RustyBuffer> {
         crate::io::stream_flush(&mut self.inner, |e| e.get_mut())
     }
 
     /// Consume the current compressor state and return the compressed stream
     /// **NB** The compressor will not be usable after this method is called.
     pub fn finish(&mut self) -> PyResult<RustyBuffer> {
-        crate::io::stream_finish(&mut self.inner, |mut inner| {
-            inner.flush().map(|_| inner.into_inner().into_inner())
-        })
+        crate::io::stream_finish(&mut self.inner, |inner| inner.finish().map(|c| c.into_inner()))
     }
 }
 
-crate::make_decompressor!();
-
-pub(crate) mod internal {
-
-    use crate::brotli::{BUF_SIZE, DEFAULT_COMPRESSION_LEVEL, LGWIN};
-    use std::io::prelude::*;
-    use std::io::Error;
-
-    /// Decompress via Brotli
-    #[inline(always)]
-    pub fn decompress<W: Write + ?Sized, R: Read>(input: R, output: &mut W) -> Result<usize, Error> {
-        let mut decoder = brotli::Decompressor::new(input, BUF_SIZE);
-        let n_bytes = std::io::copy(&mut decoder, output)?;
-        Ok(n_bytes as usize)
-    }
-
-    /// Compress via Brotli
-    #[inline(always)]
-    pub fn compress<W: Write + ?Sized, R: Read>(input: R, output: &mut W, level: Option<u32>) -> Result<usize, Error> {
-        let level = level.unwrap_or_else(|| DEFAULT_COMPRESSION_LEVEL);
-        let mut encoder = brotli::CompressorReader::new(input, BUF_SIZE, level, LGWIN);
-        let n_bytes = std::io::copy(&mut encoder, output)?;
-        Ok(n_bytes as usize)
-    }
-}
+crate::make_decompressor!(gzip);
```

### Comparing `cramjam-2.7.0rc2/src/bzip2.rs` & `cramjam-2.7.0rc3/src/bzip2.rs`

 * *Files 26% similar despite different names*

```diff
@@ -24,56 +24,62 @@
 /// Python Example
 /// --------------
 /// ```python
 /// >>> cramjam.bzip2.decompress(compressed_bytes, output_len=Optional[int])
 /// ```
 #[pyfunction]
 pub fn decompress(py: Python, data: BytesType, output_len: Option<usize>) -> PyResult<RustyBuffer> {
-    crate::generic!(py, internal::decompress[data], output_len = output_len).map_err(DecompressionError::from_err)
+    crate::generic!(py, libcramjam::bzip2::decompress[data], output_len = output_len)
+        .map_err(DecompressionError::from_err)
 }
 
 /// bzip2 compression.
 ///
 /// Python Example
 /// --------------
 /// ```python
 /// >>> cramjam.bzip2.compress(b'some bytes here', level=6, output_len=Option[int])  # level defaults to 6
 /// ```
 #[pyfunction]
 pub fn compress(py: Python, data: BytesType, level: Option<u32>, output_len: Option<usize>) -> PyResult<RustyBuffer> {
-    crate::generic!(py, internal::compress[data], output_len = output_len, level = level)
-        .map_err(CompressionError::from_err)
+    crate::generic!(
+        py,
+        libcramjam::bzip2::compress[data],
+        output_len = output_len,
+        level = level
+    )
+    .map_err(CompressionError::from_err)
 }
 
 /// Compress directly into an output buffer
 #[pyfunction]
 pub fn compress_into(py: Python, input: BytesType, mut output: BytesType, level: Option<u32>) -> PyResult<usize> {
-    crate::generic!(py, internal::compress[input, output], level = level).map_err(CompressionError::from_err)
+    crate::generic!(py, libcramjam::bzip2::compress[input, output], level = level).map_err(CompressionError::from_err)
 }
 
 /// Decompress directly into an output buffer
 #[pyfunction]
 pub fn decompress_into(py: Python, input: BytesType, mut output: BytesType) -> PyResult<usize> {
-    crate::generic!(py, internal::decompress[input, output]).map_err(DecompressionError::from_err)
+    crate::generic!(py, libcramjam::bzip2::decompress[input, output]).map_err(DecompressionError::from_err)
 }
 
 /// bzip2 Compressor object for streaming compression
 #[pyclass]
 pub struct Compressor {
-    inner: Option<bzip2::write::BzEncoder<Cursor<Vec<u8>>>>,
+    inner: Option<libcramjam::bzip2::bzip2::write::BzEncoder<Cursor<Vec<u8>>>>,
 }
 
 #[pymethods]
 impl Compressor {
     /// Initialize a new `Compressor` instance.
     #[new]
     pub fn __init__(level: Option<u32>) -> PyResult<Self> {
         let level = level.unwrap_or_else(|| DEFAULT_COMPRESSION_LEVEL);
-        let comp = bzip2::Compression::new(level);
-        let inner = bzip2::write::BzEncoder::new(Cursor::new(vec![]), comp);
+        let comp = libcramjam::bzip2::bzip2::Compression::new(level);
+        let inner = libcramjam::bzip2::bzip2::write::BzEncoder::new(Cursor::new(vec![]), comp);
         Ok(Self { inner: Some(inner) })
     }
 
     /// Compress input into the current compressor's stream.
     pub fn compress(&mut self, input: &[u8]) -> PyResult<usize> {
         crate::io::stream_compress(&mut self.inner, input)
     }
@@ -86,33 +92,8 @@
     /// Consume the current compressor state and return the compressed stream
     /// **NB** The compressor will not be usable after this method is called.
     pub fn finish(&mut self) -> PyResult<RustyBuffer> {
         crate::io::stream_finish(&mut self.inner, |inner| inner.finish().map(|c| c.into_inner()))
     }
 }
 
-crate::make_decompressor!();
-
-pub(crate) mod internal {
-
-    use super::DEFAULT_COMPRESSION_LEVEL;
-    use bzip2::read::{BzEncoder, MultiBzDecoder};
-    use std::io::prelude::*;
-    use std::io::Error;
-
-    /// Decompress via bzip2
-    #[inline(always)]
-    pub fn decompress<W: Write + ?Sized, R: Read>(input: R, output: &mut W) -> Result<usize, Error> {
-        let mut decoder = MultiBzDecoder::new(input);
-        let n_bytes = std::io::copy(&mut decoder, output)?;
-        Ok(n_bytes as usize)
-    }
-
-    /// Compress via bzip2
-    #[inline(always)]
-    pub fn compress<W: Write + ?Sized, R: Read>(input: R, output: &mut W, level: Option<u32>) -> Result<usize, Error> {
-        let level = level.unwrap_or_else(|| DEFAULT_COMPRESSION_LEVEL);
-        let mut encoder = BzEncoder::new(input, bzip2::Compression::new(level));
-        let n_bytes = std::io::copy(&mut encoder, output)?;
-        Ok(n_bytes as usize)
-    }
-}
+crate::make_decompressor!(bzip2);
```

### Comparing `cramjam-2.7.0rc2/src/exceptions.rs` & `cramjam-2.7.0rc3/src/exceptions.rs`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/src/io.rs` & `cramjam-2.7.0rc3/src/io.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 //! Module holds native Rust objects exposed to Python, or objects
 //! which wrap native Python objects to provide additional functionality
 //! or tighter integration with de/compression algorithms.
 //!
 use std::convert::TryFrom;
 use std::fs::{File, OpenOptions};
 use std::io::{copy, Cursor, Read, Seek, SeekFrom, Write};
+use std::mem;
 use std::os::raw::c_int;
 
 use crate::exceptions::CompressionError;
 use crate::BytesType;
-use pyo3::buffer::{Element, PyBuffer};
-use pyo3::exceptions::PyBufferError;
+use pyo3::exceptions::{self, PyBufferError};
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
 use pyo3::{ffi, AsPyPointer};
 use std::path::PathBuf;
 
 pub(crate) trait AsBytes {
     fn as_bytes(&self) -> &[u8];
@@ -165,81 +165,129 @@
     fn __len__(&self) -> PyResult<usize> {
         self.len()
     }
 }
 
 /// Internal wrapper to PyBuffer, not exposed thru API
 /// used only for impl of Read/Write
-pub struct PythonBuffer<T: Element> {
-    pub(crate) inner: PyBuffer<T>,
+// Inspired from pyo3 PyBuffer<T>, but here we don't want or care about T
+pub struct PythonBuffer {
+    pub(crate) inner: std::pin::Pin<Box<ffi::Py_buffer>>,
     pub(crate) pos: usize,
 }
-impl<T: Element> PythonBuffer<T> {
+// PyBuffer is thread-safe: the shape of the buffer is immutable while a Py_buffer exists.
+// Accessing the buffer contents is protected using the GIL.
+unsafe impl Send for PythonBuffer {}
+unsafe impl Sync for PythonBuffer {}
+
+impl PythonBuffer {
     /// Reset the read/write position of cursor
     pub fn reset_position(&mut self) {
         self.pos = 0;
     }
     /// Explicitly set the position of the cursor
     pub fn set_position(&mut self, pos: usize) {
         self.pos = pos;
     }
     /// Get the current position of the cursor
     pub fn position(&self) -> usize {
         self.pos
     }
     /// Is the Python buffer readonly
     pub fn readonly(&self) -> bool {
-        self.inner.readonly()
+        self.inner.readonly != 0
     }
     /// Get the underlying buffer as a slice of bytes
     pub fn as_slice(&self) -> &[u8] {
-        unsafe { std::slice::from_raw_parts(self.inner.buf_ptr() as *const u8, self.inner.len_bytes()) }
+        unsafe { std::slice::from_raw_parts(self.buf_ptr() as *const u8, self.len_bytes()) }
     }
     /// Get the underlying buffer as a mutable slice of bytes
     pub fn as_slice_mut(&mut self) -> PyResult<&mut [u8]> {
         // TODO: For v3 release, add self.readonly check; bytes is readonly but
         // v1 and v2 releases have not treated it as such.
-        Ok(unsafe { std::slice::from_raw_parts_mut(self.inner.buf_ptr() as *mut u8, self.inner.len_bytes()) })
+        Ok(unsafe { std::slice::from_raw_parts_mut(self.buf_ptr() as *mut u8, self.len_bytes()) })
+    }
+    /// If underlying buffer is c_contiguous
+    pub fn is_c_contiguous(&self) -> bool {
+        unsafe { ffi::PyBuffer_IsContiguous(&*self.inner as *const ffi::Py_buffer, b'C' as std::os::raw::c_char) != 0 }
+    }
+    /// Dimensions for buffer
+    pub fn dimensions(&self) -> usize {
+        self.inner.ndim as usize
+    }
+    /// raw pointer to buffer
+    pub fn buf_ptr(&self) -> *mut std::os::raw::c_void {
+        self.inner.buf
+    }
+    /// length of buffer in bytes
+    pub fn len_bytes(&self) -> usize {
+        self.inner.len as usize
+    }
+    /// the buffer item size
+    pub fn item_size(&self) -> usize {
+        self.inner.itemsize as usize
+    }
+    /// number of items in buffer
+    pub fn item_count(&self) -> usize {
+        (self.inner.len as usize) / (self.inner.itemsize as usize)
     }
 }
 
-impl<'py, T: Element> FromPyObject<'py> for PythonBuffer<T> {
+impl Drop for PythonBuffer {
+    fn drop(&mut self) {
+        Python::with_gil(|_| unsafe { ffi::PyBuffer_Release(&mut *self.inner) })
+    }
+}
+
+impl<'py> FromPyObject<'py> for PythonBuffer {
     fn extract(obj: &'py PyAny) -> PyResult<Self> {
-        let buf = PyBuffer::get(obj)?;
-        PythonBuffer::try_from(buf)
+        Self::try_from(obj)
     }
 }
 
-impl<T: Element> TryFrom<PyBuffer<T>> for PythonBuffer<T> {
+impl<'py> TryFrom<&'py PyAny> for PythonBuffer {
     type Error = PyErr;
-    fn try_from(buf: PyBuffer<T>) -> Result<Self, Self::Error> {
-        if !buf.is_c_contiguous() {
+    fn try_from(obj: &'py PyAny) -> Result<Self, Self::Error> {
+        let mut buf = Box::new(mem::MaybeUninit::uninit());
+        let rc = unsafe { ffi::PyObject_GetBuffer(obj.as_ptr(), buf.as_mut_ptr(), ffi::PyBUF_CONTIG_RO) };
+        if rc != 0 {
+            return Err(exceptions::PyBufferError::new_err(
+                "Failed to get buffer, is it C contiguous, and shape is not null?",
+            ));
+        }
+        let buf = Box::new(unsafe { mem::MaybeUninit::<ffi::Py_buffer>::assume_init(*buf) });
+        let buf = Self {
+            inner: std::pin::Pin::from(buf),
+            pos: 0,
+        };
+        // sanity checks
+        if buf.inner.shape.is_null() {
+            Err(exceptions::PyBufferError::new_err("shape is null"))
+        } else if !buf.is_c_contiguous() {
             Err(PyBufferError::new_err("Buffer is not C contiguous"))
-        } else if buf.dimensions() != 1 {
-            Err(PyBufferError::new_err("Buffer is not 1 dimensional"))
         } else {
-            Ok(Self { inner: buf, pos: 0 })
+            Ok(buf)
         }
     }
 }
 
-impl<T: Element> Read for PythonBuffer<T> {
+impl Read for PythonBuffer {
     fn read(&mut self, buf: &mut [u8]) -> std::io::Result<usize> {
         let slice = self.as_slice();
         if self.pos < slice.len() {
             let nbytes = (&slice[self.pos..]).read(buf)?;
             self.pos += nbytes;
             Ok(nbytes)
         } else {
             Ok(0)
         }
     }
 }
 
-impl<T: Element> Write for PythonBuffer<T> {
+impl Write for PythonBuffer {
     fn write(&mut self, buf: &[u8]) -> std::io::Result<usize> {
         let pos = self.position();
         let slice = self
             .as_slice_mut()
             .map_err(|e| std::io::Error::new(std::io::ErrorKind::Other, e.to_string()))?;
         let len = slice.len();
 
@@ -459,17 +507,17 @@
     }
 }
 impl Seek for RustyFile {
     fn seek(&mut self, pos: SeekFrom) -> std::io::Result<u64> {
         self.inner.seek(pos)
     }
 }
-impl<T: Element> Seek for PythonBuffer<T> {
+impl Seek for PythonBuffer {
     fn seek(&mut self, pos: SeekFrom) -> std::io::Result<u64> {
-        let len = self.inner.len_bytes();
+        let len = self.len_bytes();
         let current = self.position();
         match pos {
             SeekFrom::Start(n) => self.set_position(n as usize),
             SeekFrom::End(n) => self.set_position((len as i64 - n) as usize),
             SeekFrom::Current(n) => self.set_position((current as i64 + n) as usize),
         }
         Ok(self.position() as _)
```

### Comparing `cramjam-2.7.0rc2/src/lz4.rs` & `cramjam-2.7.0rc3/src/lz4.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 //! lz4 de/compression interface
 use crate::exceptions::{CompressionError, DecompressionError};
 use crate::io::{AsBytes, RustyBuffer};
 use crate::BytesType;
-use lz4::{block, block::CompressionMode};
+use libcramjam::lz4::lz4::{block, block::CompressionMode};
 use pyo3::prelude::*;
 use pyo3::wrap_pyfunction;
 use pyo3::PyResult;
 use std::io::Cursor;
 
 const DEFAULT_COMPRESSION_LEVEL: u32 = 4;
 
@@ -34,41 +34,46 @@
 /// --------------
 /// ```python
 /// >>> # Note, output_len is currently ignored; underlying algorithm does not support reading to slice at this time
 /// >>> cramjam.lz4.decompress(compressed_bytes, output_len=Optional[int])
 /// ```
 #[pyfunction]
 pub fn decompress(py: Python, data: BytesType, output_len: Option<usize>) -> PyResult<RustyBuffer> {
-    crate::generic!(py, internal::decompress[data], output_len = output_len).map_err(DecompressionError::from_err)
+    crate::generic!(py, libcramjam::lz4::decompress[data], output_len = output_len).map_err(DecompressionError::from_err)
 }
 
 /// lZ4 compression.
 ///
 /// Python Example
 /// --------------
 /// ```python
 /// >>> # Note, output_len is currently ignored; underlying algorithm does not support reading to slice at this time
 /// >>> cramjam.lz4.compress(b'some bytes here', output_len=Optional[int])
 /// ```
 #[pyfunction]
 pub fn compress(py: Python, data: BytesType, level: Option<u32>, output_len: Option<usize>) -> PyResult<RustyBuffer> {
-    crate::generic!(py, internal::compress[data], output_len = output_len, level = level)
-        .map_err(CompressionError::from_err)
+    crate::generic!(
+        py,
+        libcramjam::lz4::compress[data],
+        output_len = output_len,
+        level = level
+    )
+    .map_err(CompressionError::from_err)
 }
 
 /// Compress directly into an output buffer
 #[pyfunction]
 pub fn compress_into(py: Python, input: BytesType, mut output: BytesType, level: Option<u32>) -> PyResult<usize> {
-    crate::generic!(py, internal::compress[input, output], level = level).map_err(CompressionError::from_err)
+    crate::generic!(py, libcramjam::lz4::compress[input, output], level = level).map_err(CompressionError::from_err)
 }
 
 /// Decompress directly into an output buffer
 #[pyfunction]
 pub fn decompress_into(py: Python, input: BytesType, mut output: BytesType) -> PyResult<usize> {
-    crate::generic!(py, internal::decompress[input, output]).map_err(DecompressionError::from_err)
+    crate::generic!(py, libcramjam::lz4::decompress[input, output]).map_err(DecompressionError::from_err)
 }
 
 /// LZ4 _block_ decompression.
 ///
 /// `output_len` is optional, it's the upper bound length of decompressed data; if it's not provided,
 /// then it's assumed `store_size=True` was used during compression and length will then be taken
 /// from the header.
@@ -215,23 +220,23 @@
 pub fn compress_block_bound(src: BytesType) -> PyResult<usize> {
     block::compress_bound(src.len()).map_err(|e| pyo3::exceptions::PyValueError::new_err(e.to_string()))
 }
 
 /// lz4 Compressor object for streaming compression
 #[pyclass]
 pub struct Compressor {
-    inner: Option<lz4::Encoder<Cursor<Vec<u8>>>>,
+    inner: Option<libcramjam::lz4::lz4::Encoder<Cursor<Vec<u8>>>>,
 }
 
 #[pymethods]
 impl Compressor {
     /// Initialize a new `Compressor` instance.
     #[new]
     pub fn __init__(level: Option<u32>) -> PyResult<Self> {
-        let inner = lz4::EncoderBuilder::new()
+        let inner = libcramjam::lz4::lz4::EncoderBuilder::new()
             .auto_flush(true)
             .level(level.unwrap_or_else(|| DEFAULT_COMPRESSION_LEVEL))
             .build(Cursor::new(vec![]))?;
         Ok(Self { inner: Some(inner) })
     }
 
     /// Compress input into the current compressor's stream.
@@ -255,46 +260,8 @@
         crate::io::stream_finish(&mut self.inner, |inner| {
             let (cursor, result) = inner.finish();
             result.map(|_| cursor.into_inner())
         })
     }
 }
 
-crate::make_decompressor!();
-
-pub(crate) mod internal {
-    use crate::lz4::DEFAULT_COMPRESSION_LEVEL;
-    use lz4::{Decoder, EncoderBuilder};
-    use std::io::{BufReader, Error, Read, Seek, SeekFrom, Write};
-
-    /// Decompress lz4 data
-    #[inline(always)]
-    pub fn decompress<W: Write + ?Sized, R: Read>(input: R, output: &mut W) -> Result<usize, Error> {
-        let mut decoder = Decoder::new(input)?;
-        let n_bytes = std::io::copy(&mut decoder, output)?;
-        decoder.finish().1?;
-        Ok(n_bytes as usize)
-    }
-
-    /// Compress lz4 data
-    #[inline(always)]
-    pub fn compress<W: Write + ?Sized + Seek, R: Read>(
-        input: R,
-        output: &mut W,
-        level: Option<u32>,
-    ) -> Result<usize, Error> {
-        let start_pos = output.seek(SeekFrom::Current(0))?;
-        let mut encoder = EncoderBuilder::new()
-            .auto_flush(true)
-            .level(level.unwrap_or_else(|| DEFAULT_COMPRESSION_LEVEL))
-            .build(output)?;
-
-        // this returns, bytes read from uncompressed, input; we want bytes written
-        // but lz4 only implements Read for Encoder
-        let mut buf = BufReader::new(input);
-        std::io::copy(&mut buf, &mut encoder)?;
-        let (w, r) = encoder.finish();
-        r?;
-        let ending_pos = w.seek(SeekFrom::Current(0))?;
-        Ok((ending_pos - start_pos) as usize)
-    }
-}
+crate::make_decompressor!(lz4);
```

### Comparing `cramjam-2.7.0rc2/src/snappy.rs` & `cramjam-2.7.0rc3/src/snappy.rs`

 * *Files 16% similar despite different names*

```diff
@@ -29,43 +29,44 @@
 /// --------------
 /// ```python
 /// >>> # bytes or bytearray; bytearray is faster
 /// >>> cramjam.snappy.decompress(compressed_bytes, output_len=Optional[None])
 /// ```
 #[pyfunction]
 pub fn decompress(py: Python, data: BytesType, output_len: Option<usize>) -> PyResult<RustyBuffer> {
-    crate::generic!(py, internal::decompress[data], output_len = output_len).map_err(DecompressionError::from_err)
+    crate::generic!(py, libcramjam::snappy::decompress[data], output_len = output_len)
+        .map_err(DecompressionError::from_err)
 }
 
 /// Snappy compression.
 ///
 /// Python Example
 /// --------------
 /// ```python
 /// >>> _ = cramjam.snappy.compress(b'some bytes here')
 /// >>> _ = cramjam.snappy.compress(bytearray(b'this avoids double allocation in rust side, and thus faster!'))  # <- use bytearray where possible
 /// ```
 #[pyfunction]
 pub fn compress(py: Python, data: BytesType, output_len: Option<usize>) -> PyResult<RustyBuffer> {
-    crate::generic!(py, internal::compress[data], output_len = output_len).map_err(CompressionError::from_err)
+    crate::generic!(py, libcramjam::snappy::compress[data], output_len = output_len).map_err(CompressionError::from_err)
 }
 
 /// Snappy decompression, raw
 /// This does not use the snappy 'framed' encoding of compressed bytes.
 ///
 /// Python Example
 /// --------------
 /// ```python
 /// >>> cramjam.snappy.decompress_raw(compressed_raw_bytes)
 /// ```
 #[pyfunction]
 #[allow(unused_variables)]
 pub fn decompress_raw(py: Python, data: BytesType, output_len: Option<usize>) -> PyResult<RustyBuffer> {
     let bytes = data.as_bytes();
-    py.allow_threads(|| snap::raw::Decoder::new().decompress_vec(bytes))
+    py.allow_threads(|| libcramjam::snappy::raw::decompress_vec(bytes))
         .map_err(DecompressionError::from_err)
         .map(From::from)
 }
 
 /// Snappy compression raw.
 /// This does not use the snappy 'framed' encoding of compressed bytes.
 ///
@@ -74,75 +75,75 @@
 /// ```python
 /// >>> cramjam.snappy.compress_raw(b'some bytes here')
 /// ```
 #[pyfunction]
 #[allow(unused_variables)]
 pub fn compress_raw(py: Python, data: BytesType, output_len: Option<usize>) -> PyResult<RustyBuffer> {
     let bytes = data.as_bytes();
-    py.allow_threads(|| snap::raw::Encoder::new().compress_vec(bytes))
+    py.allow_threads(|| libcramjam::snappy::raw::compress_vec(bytes))
         .map_err(CompressionError::from_err)
         .map(From::from)
 }
 
 /// Compress directly into an output buffer
 #[pyfunction]
 pub fn compress_into(py: Python, input: BytesType, mut output: BytesType) -> PyResult<usize> {
-    crate::generic!(py, internal::compress[input, output]).map_err(CompressionError::from_err)
+    crate::generic!(py, libcramjam::snappy::compress[input, output]).map_err(CompressionError::from_err)
 }
 
 /// Decompress directly into an output buffer
 #[pyfunction]
 pub fn decompress_into(py: Python, input: BytesType, mut output: BytesType) -> PyResult<usize> {
-    crate::generic!(py, internal::decompress[input, output]).map_err(DecompressionError::from_err)
+    crate::generic!(py, libcramjam::snappy::decompress[input, output]).map_err(DecompressionError::from_err)
 }
 
 /// Compress raw format directly into an output buffer
 #[pyfunction]
 pub fn compress_raw_into(py: Python, input: BytesType, mut output: BytesType) -> PyResult<usize> {
     let bytes_in = input.as_bytes();
     let bytes_out = output.as_bytes_mut();
-    py.allow_threads(|| snap::raw::Encoder::new().compress(bytes_in, bytes_out))
+    py.allow_threads(|| libcramjam::snappy::raw::compress(bytes_in, bytes_out))
         .map_err(CompressionError::from_err)
 }
 
 /// Decompress raw format directly into an output buffer
 #[pyfunction]
 pub fn decompress_raw_into(py: Python, input: BytesType, mut output: BytesType) -> PyResult<usize> {
     let bytes_in = input.as_bytes();
     let bytes_out = output.as_bytes_mut();
-    py.allow_threads(|| snap::raw::Decoder::new().decompress(bytes_in, bytes_out))
+    py.allow_threads(|| libcramjam::snappy::raw::decompress(bytes_in, bytes_out))
         .map_err(DecompressionError::from_err)
 }
 
 /// Get the expected max compressed length for snappy raw compression; this is the size
 /// of buffer that should be passed to `compress_raw_into`
 #[pyfunction]
 pub fn compress_raw_max_len(data: BytesType) -> usize {
-    snap::raw::max_compress_len(data.len())
+    libcramjam::snappy::snap::raw::max_compress_len(data.len())
 }
 
 /// Get the decompressed length for the given data. This is the size of buffer
 /// that should be passed to `decompress_raw_into`
 #[pyfunction]
 pub fn decompress_raw_len(data: BytesType) -> PyResult<usize> {
-    snap::raw::decompress_len(data.as_bytes()).map_err(DecompressionError::from_err)
+    libcramjam::snappy::snap::raw::decompress_len(data.as_bytes()).map_err(DecompressionError::from_err)
 }
 
 /// Snappy Compressor object for streaming compression
 #[pyclass]
 pub struct Compressor {
-    inner: Option<snap::write::FrameEncoder<Cursor<Vec<u8>>>>,
+    inner: Option<libcramjam::snappy::snap::write::FrameEncoder<Cursor<Vec<u8>>>>,
 }
 
 #[pymethods]
 impl Compressor {
     /// Initialize a new `Compressor` instance.
     #[new]
     pub fn __init__() -> PyResult<Self> {
-        let inner = snap::write::FrameEncoder::new(Cursor::new(vec![]));
+        let inner = libcramjam::snappy::snap::write::FrameEncoder::new(Cursor::new(vec![]));
         Ok(Self { inner: Some(inner) })
     }
 
     /// Compress input into the current compressor's stream.
     pub fn compress(&mut self, input: &[u8]) -> PyResult<usize> {
         crate::io::stream_compress(&mut self.inner, input)
     }
@@ -155,29 +156,8 @@
     /// Consume the current compressor state and return the compressed stream
     /// **NB** The compressor will not be usable after this method is called.
     pub fn finish(&mut self) -> PyResult<RustyBuffer> {
         crate::io::stream_finish(&mut self.inner, |inner| inner.into_inner().map(|c| c.into_inner()))
     }
 }
 
-crate::make_decompressor!();
-
-pub(crate) mod internal {
-    use snap::read::{FrameDecoder, FrameEncoder};
-    use std::io::{Error, Read, Write};
-
-    /// Decompress snappy data framed
-    #[inline(always)]
-    pub fn decompress<W: Write + ?Sized, R: Read>(input: R, output: &mut W) -> Result<usize, Error> {
-        let mut decoder = FrameDecoder::new(input);
-        let n_bytes = std::io::copy(&mut decoder, output)?;
-        Ok(n_bytes as usize)
-    }
-
-    /// Decompress snappy data framed
-    #[inline(always)]
-    pub fn compress<W: Write + ?Sized, R: Read>(data: R, output: &mut W) -> Result<usize, Error> {
-        let mut encoder = FrameEncoder::new(data);
-        let n_bytes = std::io::copy(&mut encoder, output)?;
-        Ok(n_bytes as usize)
-    }
-}
+crate::make_decompressor!(snappy);
```

### Comparing `cramjam-2.7.0rc2/src/zstd.rs` & `cramjam-2.7.0rc3/src/brotli.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,86 @@
-//! zstd de/compression interface
+//! brotli de/compression interface
 use crate::exceptions::{CompressionError, DecompressionError};
 use crate::io::RustyBuffer;
 use crate::{AsBytes, BytesType};
 use pyo3::prelude::*;
 use pyo3::wrap_pyfunction;
 use pyo3::PyResult;
-use std::io::Cursor;
+use std::io::{Cursor, Write};
 
-const DEFAULT_COMPRESSION_LEVEL: i32 = 0;
+const DEFAULT_COMPRESSION_LEVEL: u32 = 11;
+const BUF_SIZE: usize = 1 << 17; // Taken from brotli kCompressFragementTwoPassBlockSize
+const LGWIN: u32 = 22;
 
 pub(crate) fn init_py_module(m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(compress, m)?)?;
     m.add_function(wrap_pyfunction!(decompress, m)?)?;
     m.add_function(wrap_pyfunction!(compress_into, m)?)?;
     m.add_function(wrap_pyfunction!(decompress_into, m)?)?;
     m.add_class::<Compressor>()?;
     m.add_class::<Decompressor>()?;
     Ok(())
 }
 
-/// ZSTD decompression.
+/// Brotli decompression.
 ///
 /// Python Example
 /// --------------
 /// ```python
-/// >>> cramjam.zstd.decompress(compressed_bytes, output_len=Optional[int])
+/// >>> cramjam.brotli.decompress(compressed_bytes, output_len=Optional[int])
 /// ```
 #[pyfunction]
 pub fn decompress(py: Python, data: BytesType, output_len: Option<usize>) -> PyResult<RustyBuffer> {
-    crate::generic!(py, internal::decompress[data], output_len = output_len).map_err(DecompressionError::from_err)
+    crate::generic!(py, libcramjam::brotli::decompress[data], output_len = output_len)
+        .map_err(DecompressionError::from_err)
 }
 
-/// ZSTD compression.
+/// Brotli compression.
 ///
 /// Python Example
 /// --------------
 /// ```python
-/// >>> cramjam.zstd.compress(b'some bytes here', level=0, output_len=Optional[int])  # level defaults to 11
+/// >>> cramjam.brotli.compress(b'some bytes here', level=9, output_len=Option[int])  # level defaults to 11
 /// ```
 #[pyfunction]
-pub fn compress(py: Python, data: BytesType, level: Option<i32>, output_len: Option<usize>) -> PyResult<RustyBuffer> {
-    crate::generic!(py, internal::compress[data], output_len = output_len, level = level)
-        .map_err(CompressionError::from_err)
+pub fn compress(py: Python, data: BytesType, level: Option<u32>, output_len: Option<usize>) -> PyResult<RustyBuffer> {
+    crate::generic!(
+        py,
+        libcramjam::brotli::compress[data],
+        output_len = output_len,
+        level = level
+    )
+    .map_err(CompressionError::from_err)
 }
 
 /// Compress directly into an output buffer
 #[pyfunction]
-pub fn compress_into(py: Python, input: BytesType, mut output: BytesType, level: Option<i32>) -> PyResult<usize> {
-    crate::generic!(py, internal::compress[input, output], level = level).map_err(CompressionError::from_err)
+pub fn compress_into(py: Python, input: BytesType, mut output: BytesType, level: Option<u32>) -> PyResult<usize> {
+    crate::generic!(py, libcramjam::brotli::compress[input, output], level=level).map_err(CompressionError::from_err)
 }
 
 /// Decompress directly into an output buffer
 #[pyfunction]
-pub fn decompress_into<'a>(py: Python<'a>, input: BytesType<'a>, mut output: BytesType<'a>) -> PyResult<usize> {
-    crate::generic!(py, internal::decompress[input, output]).map_err(DecompressionError::from_err)
+pub fn decompress_into(py: Python, input: BytesType, mut output: BytesType) -> PyResult<usize> {
+    crate::generic!(py, libcramjam::brotli::decompress[input, output]).map_err(DecompressionError::from_err)
 }
 
-/// ZSTD Compressor object for streaming compression
+/// Brotli Compressor object for streaming compression
 #[pyclass]
 pub struct Compressor {
-    inner: Option<zstd::stream::write::Encoder<'static, Cursor<Vec<u8>>>>,
+    inner: Option<libcramjam::brotli::brotli::CompressorWriter<Cursor<Vec<u8>>>>,
 }
 
 #[pymethods]
 impl Compressor {
     /// Initialize a new `Compressor` instance.
     #[new]
-    pub fn __init__(level: Option<i32>) -> PyResult<Self> {
-        let inner = zstd::stream::write::Encoder::new(Cursor::new(vec![]), level.unwrap_or(DEFAULT_COMPRESSION_LEVEL))?;
+    pub fn __init__(level: Option<u32>) -> PyResult<Self> {
+        let level = level.unwrap_or_else(|| DEFAULT_COMPRESSION_LEVEL);
+        let inner = libcramjam::brotli::brotli::CompressorWriter::new(Cursor::new(vec![]), BUF_SIZE, level, LGWIN);
         Ok(Self { inner: Some(inner) })
     }
 
     /// Compress input into the current compressor's stream.
     pub fn compress(&mut self, input: &[u8]) -> PyResult<usize> {
         crate::io::stream_compress(&mut self.inner, input)
     }
@@ -80,35 +89,14 @@
     pub fn flush(&mut self) -> PyResult<RustyBuffer> {
         crate::io::stream_flush(&mut self.inner, |e| e.get_mut())
     }
 
     /// Consume the current compressor state and return the compressed stream
     /// **NB** The compressor will not be usable after this method is called.
     pub fn finish(&mut self) -> PyResult<RustyBuffer> {
-        crate::io::stream_finish(&mut self.inner, |inner| inner.finish().map(|v| v.into_inner()))
+        crate::io::stream_finish(&mut self.inner, |mut inner| {
+            inner.flush().map(|_| inner.into_inner().into_inner())
+        })
     }
 }
 
-crate::make_decompressor!();
-
-pub(crate) mod internal {
-
-    use crate::zstd::DEFAULT_COMPRESSION_LEVEL;
-    use std::io::{Error, Read, Write};
-
-    /// Decompress gzip data
-    #[inline(always)]
-    pub fn decompress<W: Write + ?Sized, R: Read>(input: R, output: &mut W) -> Result<usize, Error> {
-        let mut decoder = zstd::stream::read::Decoder::new(input)?;
-        let n_bytes = std::io::copy(&mut decoder, output)?;
-        Ok(n_bytes as usize)
-    }
-
-    /// Compress gzip data
-    #[inline(always)]
-    pub fn compress<W: Write + ?Sized, R: Read>(input: R, output: &mut W, level: Option<i32>) -> Result<usize, Error> {
-        let level = level.unwrap_or_else(|| DEFAULT_COMPRESSION_LEVEL); // 0 will use zstd's default, currently 3
-        let mut encoder = zstd::stream::read::Encoder::new(input, level)?;
-        let n_bytes = std::io::copy(&mut encoder, output)?;
-        Ok(n_bytes as usize)
-    }
-}
+crate::make_decompressor!(brotli);
```

### Comparing `cramjam-2.7.0rc2/tests/data/integration/plaintext.txt` & `cramjam-2.7.0rc3/tests/data/integration/plaintext.txt`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.lz4` & `cramjam-2.7.0rc3/tests/data/integration/plaintext.txt.lz4`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.snappy` & `cramjam-2.7.0rc3/tests/data/integration/plaintext.txt.snappy`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/tests/test_integration.py` & `cramjam-2.7.0rc3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/tests/test_rust_io.py` & `cramjam-2.7.0rc3/tests/test_rust_io.py`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc2/tests/test_variants.py` & `cramjam-2.7.0rc3/tests/test_variants.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 import gzip
 import pytest
 import numpy as np
 import cramjam
 import hashlib
 from datetime import timedelta
 from hypothesis import strategies as st, given, settings
+from hypothesis.extra import numpy as st_np
 
 VARIANTS = ("snappy", "brotli", "bzip2", "lz4", "gzip", "deflate", "zstd")
 
 # Some OS can be slow or have higher variability in their runtimes on CI
-settings.register_profile("local", deadline=timedelta(milliseconds=1000))
-settings.register_profile("CI", deadline=None)
+settings.register_profile(
+    "local", deadline=timedelta(milliseconds=1000), max_examples=100
+)
+settings.register_profile("CI", deadline=None, max_examples=25)
 if os.getenv("CI"):
     settings.load_profile("CI")
 else:
     settings.load_profile("local")
 
 
 def same_same(a, b):
@@ -24,14 +27,31 @@
 
 def test_has_version():
     from cramjam import __version__
 
     assert isinstance(__version__, str)
 
 
+@pytest.mark.parametrize("variant_str", VARIANTS)
+@given(arr=st_np.arrays(st_np.scalar_dtypes(), shape=st.integers(0, int(1e5))))
+def test_variants_different_dtypes(variant_str, arr):
+    variant = getattr(cramjam, variant_str)
+    compressed = variant.compress(arr)
+    decompressed = variant.decompress(compressed)
+    assert same_same(bytes(decompressed), arr.tobytes())
+
+    # And compress n dims > 1
+    if arr.shape[0] % 2 == 0:
+        arr = arr.reshape((2, -1))
+        compressed = variant.compress(arr)
+        decompressed = variant.decompress(compressed)
+        assert same_same(bytes(decompressed), arr.tobytes())
+        
+
+
 @pytest.mark.parametrize("is_bytearray", (True, False))
 @pytest.mark.parametrize("variant_str", VARIANTS)
 @given(uncompressed=st.binary(min_size=1))
 def test_variants_simple(variant_str, is_bytearray, uncompressed: bytes):
 
     variant = getattr(cramjam, variant_str)
 
@@ -40,15 +60,15 @@
 
     compressed = variant.compress(uncompressed)
     assert compressed.read() != uncompressed
     compressed.seek(0)
     assert isinstance(compressed, cramjam.Buffer)
 
     decompressed = variant.decompress(compressed, output_len=len(uncompressed))
-    assert decompressed.read() == uncompressed
+    assert same_same(decompressed.read(), uncompressed)
     assert isinstance(decompressed, cramjam.Buffer)
 
 
 @pytest.mark.parametrize("variant_str", VARIANTS)
 def test_variants_raise_exception(variant_str):
     variant = getattr(cramjam, variant_str)
     with pytest.raises(cramjam.DecompressionError):
@@ -258,15 +278,15 @@
     assert bytes(lz4.compress_block(data, store_size=False)) == expected
 
     # Round trip the current collection of compression kwargs
     out = lz4.decompress_block(
         lz4.compress_block(data, **compress_kwargs),
         output_len=len(data) if not compress_kwargs["store_size"] else None,
     )
-    assert bytes(out) == data
+    assert same_same(bytes(out), data)
 
 
 @given(first=st.binary(), second=st.binary())
 def test_gzip_multiple_streams(first: bytes, second: bytes):
 
     out1 = gzip.compress(first)
     out2 = gzip.compress(second)
@@ -276,15 +296,15 @@
     out = bytes(cramjam.gzip.decompress(out1 + out2))
     assert out == first + second
 
     # works with data compressed by cramjam
     o1 = bytes(cramjam.gzip.compress(first))
     o2 = bytes(cramjam.gzip.compress(second))
     out = bytes(cramjam.gzip.decompress(o1 + o2))
-    assert out == first + second
+    assert same_same(out, first + second)
 
 
 @pytest.mark.parametrize(
     "mod",
     (
         cramjam.brotli,
         cramjam.bzip2,
@@ -303,15 +323,15 @@
     out = bytes(compressor.flush())
 
     compressor.compress(second)
     out += bytes(compressor.flush())
 
     out += bytes(compressor.finish())
     decompressed = mod.decompress(out)
-    assert bytes(decompressed) == first + second
+    assert same_same(bytes(decompressed), first + second)
 
     # just empty bytes after the first .finish()
     # same behavior as brotli.Compressor()
     assert bytes(compressor.finish()) == b""
 
     # compress will raise an error as the stream is completed
     with pytest.raises(cramjam.CompressionError):
```

### Comparing `cramjam-2.7.0rc2/Cargo.lock` & `cramjam-2.7.0rc3/Cargo.lock`

 * *Files 24% similar despite different names*

```diff
@@ -20,14 +20,63 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
 dependencies = [
  "alloc-no-stdlib",
 ]
 
 [[package]]
+name = "anstream"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6342bd4f5a1205d7f41e94a41a901f5647c938cdfa96036338e8533c9d6c2450"
+dependencies = [
+ "anstyle",
+ "anstyle-parse",
+ "anstyle-query",
+ "anstyle-wincon",
+ "colorchoice",
+ "is-terminal",
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
+
+[[package]]
+name = "anstyle-parse"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e765fd216e48e067936442276d1d57399e37bce53c264d6fefbe298080cb57ee"
+dependencies = [
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle-query"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+dependencies = [
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "anstyle-wincon"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
+dependencies = [
+ "anstyle",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "bitflags"
@@ -53,14 +102,20 @@
 checksum = "4b6561fd3f895a11e8f72af2cb7d22e08366bebc2b6b57f7744c4bda27034744"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
+name = "bytesize"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "38fcc2979eff34a4b84e1cf9a1e3da42a7d44b3b690a40cdcb23e3d556cfb2e5"
+
+[[package]]
 name = "bzip2"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bdb116a6ef3f6c3698828873ad02c3014b3c85cadb88496095628e3ef1e347f8"
 dependencies = [
  "bzip2-sys",
  "libc",
@@ -89,19 +144,69 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "clap"
+version = "4.2.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8a1f23fa97e1d1641371b51f35535cb26959b8e27ab50d167a8b996b5bada819"
+dependencies = [
+ "clap_builder",
+ "clap_derive",
+ "once_cell",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.2.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0fdc5d93c358224b4d6867ef1356d740de2303e9892edc06c5340daeccd96bab"
+dependencies = [
+ "anstream",
+ "anstyle",
+ "bitflags",
+ "clap_lex",
+ "strsim",
+]
+
+[[package]]
+name = "clap_derive"
+version = "4.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f9644cd56d6b87dbe899ef8b053e331c0637664e9e21a33dfcdc36093f5c5c4"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.15",
+]
+
+[[package]]
+name = "clap_lex"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
+
+[[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
 name = "cramjam"
 version = "2.7.0-rc2"
 dependencies = [
  "brotli",
+ "bytesize",
  "bzip2",
+ "clap",
  "flate2",
  "lz4",
  "pyo3",
  "snap",
  "zstd",
 ]
 
@@ -111,43 +216,105 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "errno"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "errno-dragonfly"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "flate2"
 version = "1.0.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
+name = "hermit-abi"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "io-lifetimes"
+version = "1.0.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
+dependencies = [
+ "hermit-abi",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "is-terminal"
+version = "0.4.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+dependencies = [
+ "hermit-abi",
+ "io-lifetimes",
+ "rustix",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "jobserver"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+
+[[package]]
+name = "linux-raw-sys"
+version = "0.3.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b64f40e5e03e0d54f03845c8197d0291253cdbedfb1cb46b13c2c117554a9f4c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -215,28 +382,28 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "pkg-config"
 version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.53"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba466839c78239c09faf015484e5cc04860f88242cff4d03eb038f04b4699b73"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.1"
@@ -279,26 +446,26 @@
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
@@ -312,14 +479,28 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "rustix"
+version = "0.37.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bc809f704c03a812ac71f22456c857be34185cac691a4316f27ab0f633bb9009"
+dependencies = [
+ "bitflags",
+ "errno",
+ "io-lifetimes",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
@@ -330,25 +511,42 @@
 [[package]]
 name = "snap"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5e9f0ab6ef7eb7353d9119c170a436d1bf248eea575ac42d19d12f4e34130831"
 
 [[package]]
+name = "strsim"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
 name = "unicode-ident"
@@ -359,80 +557,152 @@
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "utf8parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
+
+[[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
 name = "zstd"
 version = "0.11.2+zstd.1.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "20cc960326ece64f010d2d2107537f26dc589a6573a316bd5b1dba685fa5fde4"
 dependencies = [
  "zstd-safe",
 ]
```

### Comparing `cramjam-2.7.0rc2/PKG-INFO` & `cramjam-2.7.0rc3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 Metadata-Version: 2.1
 Name: cramjam
-Version: 2.7.0rc2
-License-File: LICENSE
+Version: 2.7.0rc3
+Requires-Dist: black ==22.3.0 ; extra == 'dev'
+Requires-Dist: numpy ; extra == 'dev'
+Requires-Dist: pytest >=5.30 ; extra == 'dev'
+Requires-Dist: pytest-xdist ; extra == 'dev'
+Requires-Dist: hypothesis ; extra == 'dev'
+Provides-Extra: dev
 Summary: Thin Python bindings to de/compression algorithms in Rust
 Keywords: compression,decompression,snappy,zstd,bz2,gzip,lz4,brotli,deflate
 Author: Miles Granger <miles59923@gmail.com>
 Author-email: Miles Granger <miles59923@gmail.com>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/milesgranger/pyrus-cramjam
 Project-URL: documentation, https://docs.rs/cramjam/latest/cramjam
 Project-URL: repository, https://github.com/milesgranger/pyrus-cramjam
 
-# pyrus-cramjam
+# cramjam-python
 
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![CI](https://github.com/milesgranger/pyrus-cramjam/workflows/CI/badge.svg?branch=master)](https://github.com/milesgranger/pyrus-cramjam/actions?query=branch=master)
 [![PyPI](https://img.shields.io/pypi/v/cramjam.svg)](https://pypi.org/project/cramjam)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/cramjam/badges/version.svg)](https://anaconda.org/conda-forge/cramjam)
 [![Downloads](https://pepy.tech/badge/cramjam/month)](https://pepy.tech/project/cramjam)
 
 [API Documentation](https://docs.rs/cramjam)
 
 ### Install
 ```commandline
 pip install --upgrade cramjam  # Requires no Python or system dependencies!
 ```
 
+### CLI
+
+A CLI interface is available as [`cramjam-cli`](./../cramjam-cli)
+
 ---
 
 Extremely thin Python bindings to de/compression algorithms in Rust.
 Allows for using algorithms such as Snappy, without any system dependencies.
 
 This is handy when being used in environments like AWS Lambda, where installing
 packages like `python-snappy` becomes difficult because of system level dependencies.
```

