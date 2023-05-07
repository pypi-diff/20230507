# Comparing `tmp/chafa.py-1.1.1.tar.gz` & `tmp/chafa.py-1.1.2.tar.gz`

## Comparing `chafa.py-1.1.1.tar` & `chafa.py-1.1.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 chafa_py-1.1.1/TODO.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/Makefile
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/conf.py
--rw-r--r--   0        0        0   182328 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/crunchyfy.png
--rw-r--r--   0        0        0   123186 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/crunchyfy.svg
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/index.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/make.bat
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/requirements.txt
--rw-r--r--   0        0        0    71540 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/_chafa_img/snake.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/_scripts/img_to_html.py
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/_static/custom.css
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/_static/table.js
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/Canvas.rst
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/CanvasConfig.rst
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/Functions.rst
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/Loader.rst
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/SymbolMap.rst
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/TermDb.rst
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/TermInfo.rst
--rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/api/enums.rst
--rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/examples.rst
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/installation.rst
--rw-r--r--   0        0        0    80589 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/snake.jpg
--rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial.rst
--rw-r--r--   0        0        0    71699 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/afsnake.png
--rw-r--r--   0        0        0    71067 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/alpha_snake.png
--rw-r--r--   0        0        0   485607 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/grid_snake.png
--rw-r--r--   0        0        0   163677 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/kitty_ok.png
--rw-r--r--   0        0        0    52962 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/kitty_pixels.png
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/selector_snake.png
--rw-r--r--   0        0        0    72741 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/sixels.png
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/snake_color.png
--rw-r--r--   0        0        0    10719 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/snake_edit_char.png
--rw-r--r--   0        0        0     9496 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/snake_right_aspect.png
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/snake_with_a.png
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 chafa_py-1.1.1/docs/usage/tutorial_img/snake_wrong_aspect.png
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_PIL.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_aspect.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_detect.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_html.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_pyvips.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_raw_color.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/example_simple.py
--rw-r--r--   0        0        0    80589 2020-02-02 00:00:00.000000 chafa_py-1.1.1/examples/snake.jpg
--rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 chafa_py-1.1.1/img/logo.svg
--rw-r--r--   0        0        0    12392 2020-02-02 00:00:00.000000 chafa_py-1.1.1/img/readme_snake.jpg
--rw-r--r--   0        0        0    12392 2020-02-02 00:00:00.000000 chafa_py-1.1.1/img/readme_snake.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/linux/LINUX_SOS_GO_HERE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/macos/MACOS_DYLIBS_GO_HERE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/windows/WINDOWS_DLLS_GO_HERE
--rw-r--r--   0        0        0   289788 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/windows/libchafa-0.dll
--rw-r--r--   0        0        0  1383156 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/windows/libglib-2.0-0.dll
--rw-r--r--   0        0        0  1114369 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/windows/libiconv-2.dll
--rw-r--r--   0        0        0   136724 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/windows/libintl-8.dll
--rw-r--r--   0        0        0   393081 2020-02-02 00:00:00.000000 chafa_py-1.1.1/libs/windows/libpcre2-8-0.dll
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 chafa_py-1.1.1/src/chafa/__init__.py
--rw-r--r--   0        0        0    83257 2020-02-02 00:00:00.000000 chafa_py-1.1.1/src/chafa/chafa.py
--rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 chafa_py-1.1.1/src/chafa/loader.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 chafa_py-1.1.1/tests/0_PIL_test.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 chafa_py-1.1.1/tests/1_aspect_test.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 chafa_py-1.1.1/tests/2_raw_test.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 chafa_py-1.1.1/tests/3_capabilities_test.py
--rw-r--r--   0        0        0    80589 2020-02-02 00:00:00.000000 chafa_py-1.1.1/tests/snake.jpg
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 chafa_py-1.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 chafa_py-1.1.1/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 chafa_py-1.1.1/COPYING.LESSER
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 chafa_py-1.1.1/README.md
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 chafa_py-1.1.1/hatch_build.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 chafa_py-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 chafa_py-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 chafa.py-1.1.2/TODO.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/Makefile
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/conf.py
+-rw-r--r--   0        0        0   182328 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/crunchyfy.png
+-rw-r--r--   0        0        0   123186 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/crunchyfy.svg
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/make.bat
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/requirements.txt
+-rw-r--r--   0        0        0    71540 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/_chafa_img/snake.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/_scripts/img_to_html.py
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/_static/custom.css
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/_static/table.js
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/api/Canvas.rst
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/api/CanvasConfig.rst
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/api/Functions.rst
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/api/Loader.rst
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/api/SymbolMap.rst
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/api/TermDb.rst
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/api/TermInfo.rst
+-rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/api/enums.rst
+-rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/examples.rst
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/installation.rst
+-rw-r--r--   0        0        0    80589 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/snake.jpg
+-rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial.rst
+-rw-r--r--   0        0        0    71699 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial_img/afsnake.png
+-rw-r--r--   0        0        0    71067 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial_img/alpha_snake.png
+-rw-r--r--   0        0        0   485607 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial_img/grid_snake.png
+-rw-r--r--   0        0        0   163677 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial_img/kitty_ok.png
+-rw-r--r--   0        0        0    52962 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial_img/kitty_pixels.png
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial_img/selector_snake.png
+-rw-r--r--   0        0        0    72741 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial_img/sixels.png
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial_img/snake_color.png
+-rw-r--r--   0        0        0    10719 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial_img/snake_edit_char.png
+-rw-r--r--   0        0        0     9496 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial_img/snake_right_aspect.png
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial_img/snake_with_a.png
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 chafa.py-1.1.2/docs/usage/tutorial_img/snake_wrong_aspect.png
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 chafa.py-1.1.2/examples/example_PIL.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 chafa.py-1.1.2/examples/example_aspect.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 chafa.py-1.1.2/examples/example_detect.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chafa.py-1.1.2/examples/example_html.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 chafa.py-1.1.2/examples/example_pyvips.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 chafa.py-1.1.2/examples/example_raw_color.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 chafa.py-1.1.2/examples/example_simple.py
+-rw-r--r--   0        0        0    80589 2020-02-02 00:00:00.000000 chafa.py-1.1.2/examples/snake.jpg
+-rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 chafa.py-1.1.2/img/logo.svg
+-rw-r--r--   0        0        0    12392 2020-02-02 00:00:00.000000 chafa.py-1.1.2/img/readme_snake.jpg
+-rw-r--r--   0        0        0    12392 2020-02-02 00:00:00.000000 chafa.py-1.1.2/img/readme_snake.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chafa.py-1.1.2/libs/linux/LINUX_SOS_GO_HERE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chafa.py-1.1.2/libs/macos/MACOS_DYLIBS_GO_HERE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chafa.py-1.1.2/libs/windows/WINDOWS_DLLS_GO_HERE
+-rw-r--r--   0        0        0   289788 2020-02-02 00:00:00.000000 chafa.py-1.1.2/libs/windows/libchafa-0.dll
+-rw-r--r--   0        0        0  1383156 2020-02-02 00:00:00.000000 chafa.py-1.1.2/libs/windows/libglib-2.0-0.dll
+-rw-r--r--   0        0        0  1114369 2020-02-02 00:00:00.000000 chafa.py-1.1.2/libs/windows/libiconv-2.dll
+-rw-r--r--   0        0        0   136724 2020-02-02 00:00:00.000000 chafa.py-1.1.2/libs/windows/libintl-8.dll
+-rw-r--r--   0        0        0   393081 2020-02-02 00:00:00.000000 chafa.py-1.1.2/libs/windows/libpcre2-8-0.dll
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 chafa.py-1.1.2/src/chafa/__init__.py
+-rw-r--r--   0        0        0    83350 2020-02-02 00:00:00.000000 chafa.py-1.1.2/src/chafa/chafa.py
+-rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 chafa.py-1.1.2/src/chafa/loader.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 chafa.py-1.1.2/tests/0_PIL_test.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 chafa.py-1.1.2/tests/1_aspect_test.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 chafa.py-1.1.2/tests/2_raw_test.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 chafa.py-1.1.2/tests/3_capabilities_test.py
+-rw-r--r--   0        0        0    80589 2020-02-02 00:00:00.000000 chafa.py-1.1.2/tests/snake.jpg
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 chafa.py-1.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 chafa.py-1.1.2/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 chafa.py-1.1.2/COPYING.LESSER
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 chafa.py-1.1.2/README.md
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 chafa.py-1.1.2/hatch_build.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 chafa.py-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 chafa.py-1.1.2/PKG-INFO
```

### Comparing `chafa_py-1.1.1/TODO.md` & `chafa.py-1.1.2/TODO.md`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/Makefile` & `chafa.py-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/conf.py` & `chafa.py-1.1.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import sys
 sys.path.append('../src/chafa')
 
 project = 'chafa.py'
 copyright = '2022, Erica Ferrua Edwardsdóttir'
 author = 'Erica Ferrua Edwardsdóttir'
-release = '1.1.1'
+release = '1.1.2'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinxemoji.sphinxemoji',
     'sphinx.ext.intersphinx',
@@ -65,8 +65,8 @@
     '**': [
         'about.html',
         'navigation.html',
         'relations.html',
         'searchbox.html',
         'donate.html',
     ]
-}
+}
```

### Comparing `chafa_py-1.1.1/docs/crunchyfy.png` & `chafa.py-1.1.2/docs/crunchyfy.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/crunchyfy.svg` & `chafa.py-1.1.2/docs/crunchyfy.svg`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/index.rst` & `chafa.py-1.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/make.bat` & `chafa.py-1.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/_chafa_img/snake.html` & `chafa.py-1.1.2/docs/_chafa_img/snake.html`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/_scripts/img_to_html.py` & `chafa.py-1.1.2/docs/_scripts/img_to_html.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/_static/custom.css` & `chafa.py-1.1.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/_static/table.js` & `chafa.py-1.1.2/docs/_static/table.js`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/api/Canvas.rst` & `chafa.py-1.1.2/docs/api/Canvas.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/api/CanvasConfig.rst` & `chafa.py-1.1.2/docs/api/CanvasConfig.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/api/Functions.rst` & `chafa.py-1.1.2/docs/api/Functions.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/api/Loader.rst` & `chafa.py-1.1.2/docs/api/Loader.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/api/SymbolMap.rst` & `chafa.py-1.1.2/docs/api/SymbolMap.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/api/TermDb.rst` & `chafa.py-1.1.2/docs/api/TermDb.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/api/TermInfo.rst` & `chafa.py-1.1.2/docs/api/TermInfo.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/api/enums.rst` & `chafa.py-1.1.2/docs/api/enums.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/examples.rst` & `chafa.py-1.1.2/docs/usage/examples.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/installation.rst` & `chafa.py-1.1.2/docs/usage/installation.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/snake.jpg` & `chafa.py-1.1.2/docs/usage/snake.jpg`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial.rst` & `chafa.py-1.1.2/docs/usage/tutorial.rst`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial_img/afsnake.png` & `chafa.py-1.1.2/docs/usage/tutorial_img/afsnake.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial_img/alpha_snake.png` & `chafa.py-1.1.2/docs/usage/tutorial_img/alpha_snake.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial_img/grid_snake.png` & `chafa.py-1.1.2/docs/usage/tutorial_img/grid_snake.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial_img/kitty_ok.png` & `chafa.py-1.1.2/docs/usage/tutorial_img/kitty_ok.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial_img/kitty_pixels.png` & `chafa.py-1.1.2/docs/usage/tutorial_img/kitty_pixels.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial_img/selector_snake.png` & `chafa.py-1.1.2/docs/usage/tutorial_img/selector_snake.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial_img/sixels.png` & `chafa.py-1.1.2/docs/usage/tutorial_img/sixels.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial_img/snake_color.png` & `chafa.py-1.1.2/docs/usage/tutorial_img/snake_color.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial_img/snake_edit_char.png` & `chafa.py-1.1.2/docs/usage/tutorial_img/snake_edit_char.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial_img/snake_right_aspect.png` & `chafa.py-1.1.2/docs/usage/tutorial_img/snake_right_aspect.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial_img/snake_with_a.png` & `chafa.py-1.1.2/docs/usage/tutorial_img/snake_with_a.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/docs/usage/tutorial_img/snake_wrong_aspect.png` & `chafa.py-1.1.2/docs/usage/tutorial_img/snake_wrong_aspect.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/examples/example_PIL.py` & `chafa.py-1.1.2/examples/example_PIL.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/examples/example_aspect.py` & `chafa.py-1.1.2/examples/example_aspect.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/examples/example_detect.py` & `chafa.py-1.1.2/examples/example_detect.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/examples/example_html.py` & `chafa.py-1.1.2/examples/example_html.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/examples/example_pyvips.py` & `chafa.py-1.1.2/examples/example_pyvips.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/examples/example_raw_color.py` & `chafa.py-1.1.2/examples/example_raw_color.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/examples/example_simple.py` & `chafa.py-1.1.2/examples/example_simple.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/examples/snake.jpg` & `chafa.py-1.1.2/examples/snake.jpg`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/img/logo.svg` & `chafa.py-1.1.2/img/logo.svg`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/img/readme_snake.jpg` & `chafa.py-1.1.2/img/readme_snake.jpg`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/img/readme_snake.png` & `chafa.py-1.1.2/img/readme_snake.png`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/libs/windows/libchafa-0.dll` & `chafa.py-1.1.2/libs/windows/libchafa-0.dll`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/libs/windows/libglib-2.0-0.dll` & `chafa.py-1.1.2/libs/windows/libglib-2.0-0.dll`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/libs/windows/libiconv-2.dll` & `chafa.py-1.1.2/libs/windows/libiconv-2.dll`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/libs/windows/libintl-8.dll` & `chafa.py-1.1.2/libs/windows/libintl-8.dll`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/libs/windows/libpcre2-8-0.dll` & `chafa.py-1.1.2/libs/windows/libpcre2-8-0.dll`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/src/chafa/__init__.py` & `chafa.py-1.1.2/src/chafa/__init__.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/src/chafa/chafa.py` & `chafa.py-1.1.2/src/chafa/chafa.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,19 @@
 
 # Figure out which libraries we need to import
 if platform.system() == "Linux":
     import termios
     _lib_glib = "libglib-2.0.so"
     _lib      = _root_dir / "libs" / "libchafa.so"
 
+    try:
+        ctypes.CDLL(_lib_glib)
+    except OSError:
+        _lib_glib = find_glib()
+
     if not _lib.exists():
         _lib = find_chafa()
 
 elif platform.system() == "Windows":
     os.add_dll_directory(os.path.dirname(__file__))
 
     _lib_glib = _root_dir / "libs" / "libglib-2.0-0.dll"
```

### Comparing `chafa_py-1.1.1/src/chafa/loader.py` & `chafa.py-1.1.2/src/chafa/loader.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/tests/0_PIL_test.py` & `chafa.py-1.1.2/tests/0_PIL_test.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/tests/1_aspect_test.py` & `chafa.py-1.1.2/tests/1_aspect_test.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/tests/2_raw_test.py` & `chafa.py-1.1.2/tests/2_raw_test.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/tests/snake.jpg` & `chafa.py-1.1.2/tests/snake.jpg`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/.gitignore` & `chafa.py-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/COPYING` & `chafa.py-1.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/COPYING.LESSER` & `chafa.py-1.1.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/README.md` & `chafa.py-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/hatch_build.py` & `chafa.py-1.1.2/hatch_build.py`

 * *Files identical despite different names*

### Comparing `chafa_py-1.1.1/pyproject.toml` & `chafa.py-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name    = "chafa.py"
-version = "1.1.1"
+version = "1.1.2"
 license = "LGPL-3.0"
 
 authors = [
     { name="Erica Ferrua Edwardsdóttir", email="e@mage.black" }
 ]
 
 description = "Python bindings for Chafa. Visualize images with text in python. "
```

### Comparing `chafa_py-1.1.1/PKG-INFO` & `chafa.py-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chafa.py
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python bindings for Chafa. Visualize images with text in python. 
 Project-URL: Homepage, https://chafapy.mage.black
 Project-URL: Source, https://github.com/guardkenzie/chafa.py
 Project-URL: Bug Tracker, https://github.com/guardkenzie/chafa.py/issues
 Author-email: Erica Ferrua Edwardsdóttir <e@mage.black>
 License-Expression: LGPL-3.0
 License-File: COPYING
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chafa.py Version: 1.1.1 Summary: Python bindings
+Metadata-Version: 2.1 Name: chafa.py Version: 1.1.2 Summary: Python bindings
 for Chafa. Visualize images with text in python. Project-URL: Homepage, https:/
 /chafapy.mage.black Project-URL: Source, https://github.com/guardkenzie/
 chafa.py Project-URL: Bug Tracker, https://github.com/guardkenzie/chafa.py/
 issues Author-email: Erica Ferrua EdwardsdÃ³ttir
 mage.black> License-Expression: LGPL-3.0 License-File: COPYING License-File:
 COPYING.LESSER Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: MacOS Classifier: Operating
```

