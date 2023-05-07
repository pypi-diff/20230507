# Comparing `tmp/minify_html-0.9.1-cp39-none-win_amd64.whl.zip` & `tmp/minify_html-0.9.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,9 @@
-Zip file size: 545535 bytes, number of entries: 5
--rw-r--r--  4.6 unx    17189 b- defN 22-Jun-21 16:42 minify_html-0.9.1.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 22-Jun-21 16:42 minify_html-0.9.1.dist-info/WHEEL
--rw-r--r--  4.6 unx      127 b- defN 22-Jun-21 16:42 minify_html/__init__.py
--rwxr-xr-x  4.6 unx  1974272 b- defN 22-Jun-21 16:42 minify_html/minify_html.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      400 b- defN 22-Jun-21 16:42 minify_html-0.9.1.dist-info/RECORD
-5 files, 1992084 bytes uncompressed, 544797 bytes compressed:  72.7%
+Zip file size: 546351 bytes, number of entries: 7
+-rw-r--r--  4.6 unx    17314 b- defN 22-Jun-22 04:10 minify_html-0.9.2.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 22-Jun-22 04:10 minify_html-0.9.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx      127 b- defN 22-Jun-22 04:10 minify_html/__init__.py
+-rw-r--r--  4.6 unx      474 b- defN 22-Jun-22 04:10 minify_html/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 22-Jun-22 04:10 minify_html/py.typed
+-rwxr-xr-x  4.6 unx  1974784 b- defN 22-Jun-22 04:10 minify_html/minify_html.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      554 b- defN 22-Jun-22 04:10 minify_html-0.9.2.dist-info/RECORD
+7 files, 1993349 bytes uncompressed, 545373 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -1,16 +1,22 @@
-Filename: minify_html-0.9.1.dist-info/METADATA
+Filename: minify_html-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: minify_html-0.9.1.dist-info/WHEEL
+Filename: minify_html-0.9.2.dist-info/WHEEL
 Comment: 
 
 Filename: minify_html/__init__.py
 Comment: 
 
+Filename: minify_html/__init__.pyi
+Comment: 
+
+Filename: minify_html/py.typed
+Comment: 
+
 Filename: minify_html/minify_html.cp39-win_amd64.pyd
 Comment: 
 
-Filename: minify_html-0.9.1.dist-info/RECORD
+Filename: minify_html-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `minify_html-0.9.1.dist-info/METADATA` & `minify_html-0.9.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minify_html
-Version: 0.9.1
+Version: 0.9.2
 Summary: Extremely fast and smart HTML + JS + CSS minifier
 Home-Page: https://github.com/wilsonzlin/minify-html
 Author: Wilson Lin <code@wilsonl.in>
 Author-email: Wilson Lin <code@wilsonl.in>
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/wilsonzlin/minify-html.git
@@ -30,70 +30,76 @@
 
 View the [changelog](./CHANGELOG.md) to see the latest updates.
 
 ## Performance
 
 Comparison with [html-minifier](https://github.com/kangax/html-minifier) and [minimize](https://github.com/Swaagie/minimize), run on the top web pages. [See the breakdown here.](./bench)
 
-<img width="400" alt="Chart showing speed of HTML minifiers" src="https://wilsonl.in/minify-html/bench/0.9.1/core/average-speeds.png"><img width="400" alt="Chart showing compression of HTML minifiers" src="https://wilsonl.in/minify-html/bench/0.9.1/core/average-sizes.png">
+<img width="400" alt="Chart showing speed of HTML minifiers" src="https://wilsonl.in/minify-html/bench/0.9.2/core/average-speeds.png"><img width="400" alt="Chart showing compression of HTML minifiers" src="https://wilsonl.in/minify-html/bench/0.9.2/core/average-sizes.png">
 
 The [onepass](https://github.com/wilsonzlin/minify-html/tree/master/rust/onepass) variant is even more optimised for speed. See its [README](https://github.com/wilsonzlin/minify-html/tree/master/rust/onepass) for more details.
 
 ## Compatibility and usage
 
 <details>
 <summary><img width="24" src="https://wilsonl.in/minify-html/icon/cli.png"> <strong>CLI</strong></summary>
 
 Precompiled binaries are available for Linux, macOS, and Windows.
 
 ### Get
 
-[Linux x64](https://wilsonl.in/minify-html/bin/0.9.1-linux-x86_64) |
-[Linux ARM64](https://wilsonl.in/minify-html/bin/0.9.1-linux-arm64) |
-[macOS x64](https://wilsonl.in/minify-html/bin/0.9.1-macos-x86_64) |
-[macOS ARM64](https://wilsonl.in/minify-html/bin/0.9.1-macos-arm64) |
-[Windows x64](https://wilsonl.in/minify-html/bin/0.9.1-windows-x86_64.exe)
+[Linux x64](https://wilsonl.in/minify-html/bin/0.9.2-linux-x86_64) |
+[Linux ARM64](https://wilsonl.in/minify-html/bin/0.9.2-linux-arm64) |
+[macOS x64](https://wilsonl.in/minify-html/bin/0.9.2-macos-x86_64) |
+[macOS ARM64](https://wilsonl.in/minify-html/bin/0.9.2-macos-arm64) |
+[Windows x64](https://wilsonl.in/minify-html/bin/0.9.2-windows-x86_64.exe)
 
 ### Use
 
 Use the `--help` argument for more details.
 
 ```bash
 minify-html --output /path/to/output.min.html --keep-closing-tags --minify-css /path/to/src.html
 ```
 
+To quickly parallel process a batch of files in place:
+
+```bash
+minify-html --keep-closing-tags --minify-css /path/to/**/*.html
+```
+
 </details>
 
 <details>
 <summary><img width="24" src="https://wilsonl.in/minify-html/icon/rust.png"> <strong>Rust</strong></summary>
 
 ### Get
 
 ```toml
 [dependencies]
-minify-html = { version = "0.9.1" }
+minify-html = "0.9.2"
 ```
 
 ### Use
 
 Check out the [docs](https://docs.rs/minify-html) for API and usage examples.
 
 </details>
 
 <details>
 <summary><img width="24" src="https://wilsonl.in/minify-html/icon/deno.png"> <strong>Deno</strong></summary>
 
-- Package: https://wilsonl.in/minify-html/deno/0.9.1/index.js
+- Package: https://wilsonl.in/minify-html/deno/0.9.2/index.js
 - Binding: [WASM](https://webassembly.org/)
 - Platforms: All
 
 ### Use
 
 ```ts
-import init, {minify} from "https://wilsonl.in/minify-html/deno/0.9.1/index.js";
+import init, {minify} from "https://wilsonl.in/minify-html/deno/0.9.2/index.js";
 
 const encoder = new TextEncoder();
 const decoder = new TextDecoder();
 
 await init();
 
 const minified = decoder.decode(minify(encoder.encode("<p>  Hello, world!  </p>"), { keep_spaces_between_attributes: true, keep_comments: true }));
@@ -150,15 +156,15 @@
 
 Add as a Maven dependency:
 
 ```xml
 <dependency>
   <groupId>in.wilsonl.minifyhtml</groupId>
   <artifactId>minify-html</artifactId>
-  <version>0.9.1</version>
+  <version>0.9.2</version>
 </dependency>
 ```
 
 ### Use
 
 ```java
 import in.wilsonl.minifyhtml.Configuration;
```

