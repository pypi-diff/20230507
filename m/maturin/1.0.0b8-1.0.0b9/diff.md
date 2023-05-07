# Comparing `tmp/maturin-1.0.0b8.tar.gz` & `tmp/maturin-1.0.0b9.tar.gz`

## Comparing `maturin-1.0.0b8.tar` & `maturin-1.0.0b9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 maturin-1.0.0b8/Cargo.toml
--rw-r--r--   0     1001      123     1692 2023-05-04 14:56:10.000000 maturin-1.0.0b8/.cirrus.yml
--rw-r--r--   0     1001      123       94 2023-05-04 14:56:10.000000 maturin-1.0.0b8/.codespellrc
--rw-r--r--   0     1001      123      252 2023-05-04 14:56:10.000000 maturin-1.0.0b8/.config/nextest.toml
--rw-r--r--   0     1001      123      180 2023-05-04 14:56:10.000000 maturin-1.0.0b8/.dockerignore
--rw-r--r--   0     1001      123      184 2023-05-04 14:56:10.000000 maturin-1.0.0b8/.gitignore
--rw-r--r--   0     1001      123    65671 2023-05-04 14:56:10.000000 maturin-1.0.0b8/Cargo.lock
--rw-r--r--   0     1001      123    55621 2023-05-04 14:56:10.000000 maturin-1.0.0b8/Changelog.md
--rw-r--r--   0     1001      123     3228 2023-05-04 14:56:10.000000 maturin-1.0.0b8/Code-of-Conduct.md
--rw-r--r--   0     1001      123     2386 2023-05-04 14:56:10.000000 maturin-1.0.0b8/Dockerfile
--rw-r--r--   0     1001      123      245 2023-05-04 14:56:10.000000 maturin-1.0.0b8/MANIFEST.in
--rw-r--r--   0     1001      123    16573 2023-05-04 14:56:10.000000 maturin-1.0.0b8/README.md
--rw-r--r--   0     1001      123       16 2023-05-04 14:56:10.000000 maturin-1.0.0b8/clippy.toml
--rw-r--r--   0     1001      123     9664 2023-05-04 14:56:10.000000 maturin-1.0.0b8/deny.toml
--rw-r--r--   0     1001      123    10847 2023-05-04 14:56:10.000000 maturin-1.0.0b8/license-apache
--rw-r--r--   0     1001      123     1051 2023-05-04 14:56:10.000000 maturin-1.0.0b8/license-mit
--rw-r--r--   0     1001      123     6236 2023-05-04 14:56:10.000000 maturin-1.0.0b8/maturin/__init__.py
--rw-r--r--   0     1001      123      956 2023-05-04 14:56:10.000000 maturin-1.0.0b8/maturin/__main__.py
--rw-r--r--   0     1001      123     5162 2023-05-04 14:56:10.000000 maturin-1.0.0b8/maturin/import_hook.py
--rw-r--r--   0     1001      123      200 2023-05-04 14:56:10.000000 maturin-1.0.0b8/netlify.toml
--rw-r--r--   0     1001      123     2170 2023-05-04 14:56:10.000000 maturin-1.0.0b8/noxfile.py
--rw-r--r--   0     1001      123     1290 2023-05-04 14:56:10.000000 maturin-1.0.0b8/pyproject.toml
--rw-r--r--   0     1001      123     2868 2023-05-04 14:56:10.000000 maturin-1.0.0b8/setup.py
--rw-r--r--   0     1001      123    19534 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/audit.rs
--rw-r--r--   0     1001      123    53261 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/manylinux-policy.json
--rw-r--r--   0     1001      123      242 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/mod.rs
--rw-r--r--   0     1001      123     1862 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/musllinux-policy.json
--rw-r--r--   0     1001      123     1389 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/musllinux.rs
--rw-r--r--   0     1001      123     3777 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/patchelf.rs
--rw-r--r--   0     1001      123     4602 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/platform_tag.rs
--rw-r--r--   0     1001      123     5393 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/policy.rs
--rw-r--r--   0     1001      123     1169 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/auditwheel/repair.rs
--rw-r--r--   0     1001      123    47514 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/build_context.rs
--rw-r--r--   0     1001      123    57254 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/build_options.rs
--rw-r--r--   0     1001      123     5407 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/cargo_toml.rs
--rw-r--r--   0     1001      123    33723 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/ci.rs
--rw-r--r--   0     1001      123    23999 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/compile.rs
--rw-r--r--   0     1001      123     8342 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/cross_compile.rs
--rw-r--r--   0     1001      123     6119 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/develop.rs
--rw-r--r--   0     1001      123     2233 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/lib.rs
--rw-r--r--   0     1001      123    17816 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/main.rs
--rw-r--r--   0     1001      123    32462 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/metadata.rs
--rw-r--r--   0     1001      123    44938 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/module_writer.rs
--rw-r--r--   0     1001      123     8203 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/new_project.rs
--rw-r--r--   0     1001      123    16142 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/project_layout.rs
--rw-r--r--   0     1001      123    17317 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/pyproject_toml.rs
--rw-r--r--   0     1001      123    11820 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/config.rs
--rw-r--r--   0     1001      123     1595 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/get_interpreter_metadata.py
--rw-r--r--   0     1001      123    34577 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/mod.rs
--rw-r--r--   0     1001      123      443 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-emscripten.json
--rw-r--r--   0     1001      123     3861 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-freebsd.json
--rw-r--r--   0     1001      123    14124 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-linux.json
--rw-r--r--   0     1001      123     3812 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-macos.json
--rw-r--r--   0     1001      123      738 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-netbsd.json
--rw-r--r--   0     1001      123     2353 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-openbsd.json
--rw-r--r--   0     1001      123     3341 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/python_interpreter/sysconfig-windows.json
--rw-r--r--   0     1001      123    34671 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/source_distribution.rs
--rw-r--r--   0     1001      123    18478 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/target.rs
--rw-r--r--   0     1001      123      686 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/.gitignore.j2
--rw-r--r--   0     1001      123      518 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/Cargo.toml.j2
--rw-r--r--   0     1001      123      149 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/__init__.py.j2
--rw-r--r--   0     1001      123      123 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/build.rs.j2
--rw-r--r--   0     1001      123       47 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/example.udl.j2
--rw-r--r--   0     1001      123      722 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/lib.rs.j2
--rw-r--r--   0     1001      123       45 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/main.rs.j2
--rw-r--r--   0     1001      123      859 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/templates/pyproject.toml.j2
--rw-r--r--   0     1001      123    22846 2023-05-04 14:56:10.000000 maturin-1.0.0b8/src/upload.rs
--rwxr-xr-x   0     1001      123      974 2023-05-04 14:56:10.000000 maturin-1.0.0b8/test-dockerfile.sh
--rw-r--r--   0        0        0    17754 1970-01-01 00:00:00.000000 maturin-1.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 maturin-1.0.0b9/Cargo.toml
+-rw-r--r--   0     1001      123     1692 2023-05-06 13:28:59.000000 maturin-1.0.0b9/.cirrus.yml
+-rw-r--r--   0     1001      123       94 2023-05-06 13:28:59.000000 maturin-1.0.0b9/.codespellrc
+-rw-r--r--   0     1001      123      252 2023-05-06 13:28:59.000000 maturin-1.0.0b9/.config/nextest.toml
+-rw-r--r--   0     1001      123      180 2023-05-06 13:28:59.000000 maturin-1.0.0b9/.dockerignore
+-rw-r--r--   0     1001      123      184 2023-05-06 13:28:59.000000 maturin-1.0.0b9/.gitignore
+-rw-r--r--   0     1001      123    65671 2023-05-06 13:28:59.000000 maturin-1.0.0b9/Cargo.lock
+-rw-r--r--   0     1001      123    55621 2023-05-06 13:28:59.000000 maturin-1.0.0b9/Changelog.md
+-rw-r--r--   0     1001      123     3228 2023-05-06 13:28:59.000000 maturin-1.0.0b9/Code-of-Conduct.md
+-rw-r--r--   0     1001      123     2386 2023-05-06 13:28:59.000000 maturin-1.0.0b9/Dockerfile
+-rw-r--r--   0     1001      123      245 2023-05-06 13:28:59.000000 maturin-1.0.0b9/MANIFEST.in
+-rw-r--r--   0     1001      123    16573 2023-05-06 13:28:59.000000 maturin-1.0.0b9/README.md
+-rw-r--r--   0     1001      123       16 2023-05-06 13:28:59.000000 maturin-1.0.0b9/clippy.toml
+-rw-r--r--   0     1001      123     9664 2023-05-06 13:28:59.000000 maturin-1.0.0b9/deny.toml
+-rw-r--r--   0     1001      123    10847 2023-05-06 13:28:59.000000 maturin-1.0.0b9/license-apache
+-rw-r--r--   0     1001      123     1051 2023-05-06 13:28:59.000000 maturin-1.0.0b9/license-mit
+-rw-r--r--   0     1001      123     6236 2023-05-06 13:28:59.000000 maturin-1.0.0b9/maturin/__init__.py
+-rw-r--r--   0     1001      123      956 2023-05-06 13:28:59.000000 maturin-1.0.0b9/maturin/__main__.py
+-rw-r--r--   0     1001      123     5162 2023-05-06 13:28:59.000000 maturin-1.0.0b9/maturin/import_hook.py
+-rw-r--r--   0     1001      123      200 2023-05-06 13:28:59.000000 maturin-1.0.0b9/netlify.toml
+-rw-r--r--   0     1001      123     2170 2023-05-06 13:28:59.000000 maturin-1.0.0b9/noxfile.py
+-rw-r--r--   0     1001      123     1290 2023-05-06 13:28:59.000000 maturin-1.0.0b9/pyproject.toml
+-rw-r--r--   0     1001      123     2868 2023-05-06 13:28:59.000000 maturin-1.0.0b9/setup.py
+-rw-r--r--   0     1001      123    19534 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/audit.rs
+-rw-r--r--   0     1001      123    53261 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/manylinux-policy.json
+-rw-r--r--   0     1001      123      242 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/mod.rs
+-rw-r--r--   0     1001      123     1862 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/musllinux-policy.json
+-rw-r--r--   0     1001      123     1389 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/musllinux.rs
+-rw-r--r--   0     1001      123     3777 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/patchelf.rs
+-rw-r--r--   0     1001      123     4602 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/platform_tag.rs
+-rw-r--r--   0     1001      123     5393 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/policy.rs
+-rw-r--r--   0     1001      123     1169 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/repair.rs
+-rw-r--r--   0     1001      123    47514 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/build_context.rs
+-rw-r--r--   0     1001      123    57281 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/build_options.rs
+-rw-r--r--   0     1001      123     5407 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/cargo_toml.rs
+-rw-r--r--   0     1001      123    33723 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/ci.rs
+-rw-r--r--   0     1001      123    24202 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/compile.rs
+-rw-r--r--   0     1001      123     8342 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/cross_compile.rs
+-rw-r--r--   0     1001      123     6119 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/develop.rs
+-rw-r--r--   0     1001      123     2233 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/lib.rs
+-rw-r--r--   0     1001      123    17816 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/main.rs
+-rw-r--r--   0     1001      123    32462 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/metadata.rs
+-rw-r--r--   0     1001      123    44938 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/module_writer.rs
+-rw-r--r--   0     1001      123     8203 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/new_project.rs
+-rw-r--r--   0     1001      123    16142 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/project_layout.rs
+-rw-r--r--   0     1001      123    17317 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/pyproject_toml.rs
+-rw-r--r--   0     1001      123    11820 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/config.rs
+-rw-r--r--   0     1001      123     1595 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/get_interpreter_metadata.py
+-rw-r--r--   0     1001      123    34577 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/mod.rs
+-rw-r--r--   0     1001      123      443 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-emscripten.json
+-rw-r--r--   0     1001      123     3861 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-freebsd.json
+-rw-r--r--   0     1001      123    14124 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-linux.json
+-rw-r--r--   0     1001      123     3812 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-macos.json
+-rw-r--r--   0     1001      123      738 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-netbsd.json
+-rw-r--r--   0     1001      123     2353 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-openbsd.json
+-rw-r--r--   0     1001      123     3341 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-windows.json
+-rw-r--r--   0     1001      123    34671 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/source_distribution.rs
+-rw-r--r--   0     1001      123    18478 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/target.rs
+-rw-r--r--   0     1001      123      686 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/.gitignore.j2
+-rw-r--r--   0     1001      123      518 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/Cargo.toml.j2
+-rw-r--r--   0     1001      123      149 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/__init__.py.j2
+-rw-r--r--   0     1001      123      123 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/build.rs.j2
+-rw-r--r--   0     1001      123       47 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/example.udl.j2
+-rw-r--r--   0     1001      123      722 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/lib.rs.j2
+-rw-r--r--   0     1001      123       45 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/main.rs.j2
+-rw-r--r--   0     1001      123      859 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/pyproject.toml.j2
+-rw-r--r--   0     1001      123    22846 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/upload.rs
+-rwxr-xr-x   0     1001      123      974 2023-05-06 13:28:59.000000 maturin-1.0.0b9/test-dockerfile.sh
+-rw-r--r--   0        0        0    17754 1970-01-01 00:00:00.000000 maturin-1.0.0b9/PKG-INFO
```

### Comparing `maturin-1.0.0b8/Cargo.toml` & `maturin-1.0.0b9/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 authors = ["konstin <konstin@mailbox.org>", "messense <messense@icloud.com>"]
 name = "maturin"
-version = "1.0.0-beta.8"
+version = "1.0.0-beta.9"
 description = "Build and publish crates with pyo3, rust-cpython and cffi bindings as well as rust binaries as python packages"
 exclude = ["test-crates/**/*", "sysconfig/*", "test-data/*", "ci/*", "tests/*", "guide/*", ".github/*"]
 homepage = "https://github.com/pyo3/maturin"
 readme = "README.md"
 repository = "https://github.com/pyo3/maturin"
 license = "MIT OR Apache-2.0"
 keywords = ["python", "cffi", "packaging", "pypi", "pyo3"]
```

### Comparing `maturin-1.0.0b8/.cirrus.yml` & `maturin-1.0.0b9/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/Cargo.lock` & `maturin-1.0.0b9/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.70"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
@@ -75,17 +75,17 @@
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
@@ -1012,15 +1012,15 @@
 checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
 dependencies = [
  "regex-automata",
 ]
 
 [[package]]
 name = "maturin"
-version = "1.0.0-beta.8"
+version = "1.0.0-beta.9"
 dependencies = [
  "anyhow",
  "base64 0.13.1",
  "bytesize",
  "cargo-config2",
  "cargo-options",
  "cargo-xwin",
@@ -1352,17 +1352,17 @@
 name = "path-slash"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e91099d4268b0e11973f036e885d652fb0b21fedcf69738c627f94db6a44f42"
 
 [[package]]
 name = "pep440_rs"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aac177a025c60a4dd25d638bf33e746d1ead5f7123f6650f35b4394c7ce1a104"
+checksum = "3d6f6ead185985925c7e2b5ddb57ed5ef9d95835bf3994a5ce74403653898ab6"
 dependencies = [
  "lazy_static",
  "regex",
  "serde",
  "tracing",
  "unicode-width",
 ]
@@ -1518,17 +1518,17 @@
 checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "quoted_printable"
-version = "0.4.7"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a24039f627d8285853cc90dcddf8c1ebfaa91f834566948872b225b9a28ed1b6"
+checksum = "5a3866219251662ec3b26fc217e3e05bf9c4f84325234dfb96bf0bf840889e49"
 
 [[package]]
 name = "rand"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
 dependencies = [
@@ -2060,34 +2060,34 @@
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.20"
+version = "0.3.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
+checksum = "8f3403384eaacbca9923fa06940178ac13e4edb725486d70e8e15881d0c836cc"
 dependencies = [
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
@@ -2199,17 +2199,17 @@
 dependencies = [
  "serde",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-subscriber"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6176eae26dd70d0c919749377897b54a9276bd7061339665dd68777926b5a70"
+checksum = "30a651bc37f915e81f087d86e62a18eec5f79550c7faff886f7090b4ea757c77"
 dependencies = [
  "matchers",
  "nu-ansi-term",
  "once_cell",
  "regex",
  "serde",
  "serde_json",
@@ -2587,17 +2587,17 @@
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "winnow"
-version = "0.4.1"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
+checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "xattr"
 version = "0.2.3"
```

### Comparing `maturin-1.0.0b8/Changelog.md` & `maturin-1.0.0b9/Changelog.md`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/Code-of-Conduct.md` & `maturin-1.0.0b9/Code-of-Conduct.md`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/Dockerfile` & `maturin-1.0.0b9/Dockerfile`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/README.md` & `maturin-1.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/deny.toml` & `maturin-1.0.0b9/deny.toml`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/license-apache` & `maturin-1.0.0b9/license-apache`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/license-mit` & `maturin-1.0.0b9/license-mit`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/maturin/__init__.py` & `maturin-1.0.0b9/maturin/__init__.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/maturin/__main__.py` & `maturin-1.0.0b9/maturin/__main__.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/maturin/import_hook.py` & `maturin-1.0.0b9/maturin/import_hook.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/noxfile.py` & `maturin-1.0.0b9/noxfile.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/pyproject.toml` & `maturin-1.0.0b9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/setup.py` & `maturin-1.0.0b9/setup.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/auditwheel/audit.rs` & `maturin-1.0.0b9/src/auditwheel/audit.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/auditwheel/manylinux-policy.json` & `maturin-1.0.0b9/src/auditwheel/manylinux-policy.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/auditwheel/musllinux-policy.json` & `maturin-1.0.0b9/src/auditwheel/musllinux-policy.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/auditwheel/musllinux.rs` & `maturin-1.0.0b9/src/auditwheel/musllinux.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/auditwheel/patchelf.rs` & `maturin-1.0.0b9/src/auditwheel/patchelf.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/auditwheel/platform_tag.rs` & `maturin-1.0.0b9/src/auditwheel/platform_tag.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/auditwheel/policy.rs` & `maturin-1.0.0b9/src/auditwheel/policy.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/auditwheel/repair.rs` & `maturin-1.0.0b9/src/auditwheel/repair.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/build_context.rs` & `maturin-1.0.0b9/src/build_context.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/build_options.rs` & `maturin-1.0.0b9/src/build_options.rs`

 * *Files 0% similar despite different names*

```diff
@@ -991,14 +991,15 @@
         BridgeModel::Bin(find_bindings(&deps, &packages))
     } else {
         bail!("Couldn't detect the binding type; Please specify them with --bindings/-b")
     };
 
     if !(bridge.is_bindings("pyo3") || bridge.is_bindings("pyo3-ffi")) {
         eprintln!("🔗 Found {bridge} bindings");
+        return Ok(bridge);
     }
 
     for &lib in PYO3_BINDING_CRATES.iter() {
         if !bridge.is_bin() && bridge.is_bindings(lib) {
             let pyo3_node = deps[lib];
             if !pyo3_node.features.contains(&"extension-module".to_string()) {
                 let version = cargo_metadata[&pyo3_node.id].version.to_string();
```

### Comparing `maturin-1.0.0b8/src/cargo_toml.rs` & `maturin-1.0.0b9/src/cargo_toml.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/ci.rs` & `maturin-1.0.0b9/src/ci.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/compile.rs` & `maturin-1.0.0b9/src/compile.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 use crate::target::RUST_1_64_0;
 #[cfg(feature = "zig")]
 use crate::PlatformTag;
 use crate::{BuildContext, PythonInterpreter, Target};
 use anyhow::{anyhow, bail, Context, Result};
 use fat_macho::FatWriter;
 use fs_err::{self as fs, File};
+use normpath::PathExt;
 use std::collections::HashMap;
 use std::env;
 use std::io::{BufReader, Read};
 use std::path::{Path, PathBuf};
 use std::process::Stdio;
 use std::str;
 use tracing::{debug, trace};
@@ -149,15 +150,15 @@
     context: &BuildContext,
     python_interpreter: Option<&PythonInterpreter>,
     compile_target: &CompileTarget,
 ) -> Result<HashMap<String, BuildArtifact>> {
     let target = &context.target;
 
     let mut cargo_rustc: cargo_options::Rustc = context.cargo_options.clone().into();
-    cargo_rustc.message_format = vec!["json".to_string()];
+    cargo_rustc.message_format = vec!["json-render-diagnostics".to_string()];
 
     // --release and --profile are conflicting options
     if context.release && cargo_rustc.profile.is_none() {
         cargo_rustc.release = true;
     }
 
     // Add `--crate-type cdylib` if available
@@ -365,17 +366,20 @@
 
     // Setup `PYO3_CONFIG_FILE` if we are cross compiling for pyo3 bindings
     if let Some(interpreter) = python_interpreter {
         // Target python interpreter isn't runnable when cross compiling
         if interpreter.runnable {
             if bridge_model.is_bindings("pyo3")
                 || bridge_model.is_bindings("pyo3-ffi")
-                || (matches!(bridge_model, BridgeModel::BindingsAbi3(_, _))
-                    && interpreter.interpreter_kind.is_pypy())
+                || matches!(bridge_model, BridgeModel::BindingsAbi3(_, _))
             {
+                debug!(
+                    "Setting PYO3_PYTHON to {}",
+                    interpreter.executable.display()
+                );
                 build_command
                     .env("PYO3_PYTHON", &interpreter.executable)
                     .env(
                         "PYO3_ENVIRONMENT_SIGNATURE",
                         interpreter.environment_signature(),
                     );
             }
@@ -397,15 +401,16 @@
             fs::create_dir_all(&maturin_target_dir)?;
             fs::write(&config_file, pyo3_config).with_context(|| {
                 format!(
                     "Failed to create pyo3 config file at '{}'",
                     config_file.display()
                 )
             })?;
-            build_command.env("PYO3_CONFIG_FILE", config_file);
+            let abs_config_file = config_file.normalize()?.into_path_buf();
+            build_command.env("PYO3_CONFIG_FILE", abs_config_file);
         }
     }
 
     if let Some(lib_dir) = env::var_os("MATURIN_PYTHON_SYSCONFIGDATA_DIR") {
         build_command.env("PYO3_CROSS_LIB_DIR", lib_dir);
     }
```

### Comparing `maturin-1.0.0b8/src/cross_compile.rs` & `maturin-1.0.0b9/src/cross_compile.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/develop.rs` & `maturin-1.0.0b9/src/develop.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/lib.rs` & `maturin-1.0.0b9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/main.rs` & `maturin-1.0.0b9/src/main.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/metadata.rs` & `maturin-1.0.0b9/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/module_writer.rs` & `maturin-1.0.0b9/src/module_writer.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/new_project.rs` & `maturin-1.0.0b9/src/new_project.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/project_layout.rs` & `maturin-1.0.0b9/src/project_layout.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/pyproject_toml.rs` & `maturin-1.0.0b9/src/pyproject_toml.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/python_interpreter/config.rs` & `maturin-1.0.0b9/src/python_interpreter/config.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/python_interpreter/get_interpreter_metadata.py` & `maturin-1.0.0b9/src/python_interpreter/get_interpreter_metadata.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/python_interpreter/mod.rs` & `maturin-1.0.0b9/src/python_interpreter/mod.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/python_interpreter/sysconfig-freebsd.json` & `maturin-1.0.0b9/src/python_interpreter/sysconfig-freebsd.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/python_interpreter/sysconfig-linux.json` & `maturin-1.0.0b9/src/python_interpreter/sysconfig-linux.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/python_interpreter/sysconfig-macos.json` & `maturin-1.0.0b9/src/python_interpreter/sysconfig-macos.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/python_interpreter/sysconfig-netbsd.json` & `maturin-1.0.0b9/src/python_interpreter/sysconfig-netbsd.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/python_interpreter/sysconfig-openbsd.json` & `maturin-1.0.0b9/src/python_interpreter/sysconfig-openbsd.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/python_interpreter/sysconfig-windows.json` & `maturin-1.0.0b9/src/python_interpreter/sysconfig-windows.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/source_distribution.rs` & `maturin-1.0.0b9/src/source_distribution.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/target.rs` & `maturin-1.0.0b9/src/target.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/templates/.gitignore.j2` & `maturin-1.0.0b9/src/templates/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/templates/Cargo.toml.j2` & `maturin-1.0.0b9/src/templates/Cargo.toml.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/templates/lib.rs.j2` & `maturin-1.0.0b9/src/templates/lib.rs.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/templates/pyproject.toml.j2` & `maturin-1.0.0b9/src/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/src/upload.rs` & `maturin-1.0.0b9/src/upload.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/test-dockerfile.sh` & `maturin-1.0.0b9/test-dockerfile.sh`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b8/PKG-INFO` & `maturin-1.0.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maturin
-Version: 1.0.0b8
+Version: 1.0.0b9
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: tomli >=1.1.0 ; python_version < '3.11'
 Requires-Dist: ziglang ~=0.10.0 ; extra == 'zig'
 Requires-Dist: patchelf ; extra == 'patchelf'
```

