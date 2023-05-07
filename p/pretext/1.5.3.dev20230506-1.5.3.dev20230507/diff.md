# Comparing `tmp/pretext-1.5.3.dev20230506.tar.gz` & `tmp/pretext-1.5.3.dev20230507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.5.3.dev20230506.tar", max compression
+gzip compressed data, was "pretext-1.5.3.dev20230507.tar", max compression
```

## Comparing `pretext-1.5.3.dev20230506.tar` & `pretext-1.5.3.dev20230507.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35148 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/LICENSE
--rw-r--r--   0        0        0     9664 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/README.md
--rw-r--r--   0        0        0     1440 2023-05-06 06:17:26.843531 pretext-1.5.3.dev20230506/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/__main__.py
--rw-r--r--   0        0        0     7344 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/build.py
--rw-r--r--   0        0        0    22954 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/core/__init__.py
--rw-r--r--   0        0        0   173946 2023-05-06 06:17:31.727570 pretext-1.5.3.dev20230506/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/core/resources.py
--rw-r--r--   0        0        0  1052517 2023-05-06 06:17:31.727570 pretext-1.5.3.dev20230506/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/generate.py
--rw-r--r--   0        0        0    24172 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/project.py
--rw-r--r--   0        0        0      516 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160171 2023-05-06 06:17:31.771571 pretext-1.5.3.dev20230506/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7677 2023-05-06 06:17:31.791571 pretext-1.5.3.dev20230506/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173370 2023-05-06 06:17:31.787571 pretext-1.5.3.dev20230506/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     1236 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4718 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0      630 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/postCreateCommand.sh
--rw-r--r--   0        0        0     1710 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8453 2023-05-06 06:17:31.795571 pretext-1.5.3.dev20230506/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18300 2023-05-06 06:16:46.551190 pretext-1.5.3.dev20230506/pretext/utils.py
--rw-r--r--   0        0        0     1119 2023-05-06 06:17:26.843531 pretext-1.5.3.dev20230506/pyproject.toml
--rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.3.dev20230506/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/LICENSE
+-rw-r--r--   0        0        0     9664 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/README.md
+-rw-r--r--   0        0        0     1440 2023-05-07 06:17:58.022873 pretext-1.5.3.dev20230507/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/pretext/__main__.py
+-rw-r--r--   0        0        0     7344 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/pretext/build.py
+-rw-r--r--   0        0        0    22954 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/pretext/core/__init__.py
+-rw-r--r--   0        0        0   173946 2023-05-07 06:18:03.066977 pretext-1.5.3.dev20230507/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/pretext/core/resources.py
+-rw-r--r--   0        0        0  1052638 2023-05-07 06:18:03.066977 pretext-1.5.3.dev20230507/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/pretext/generate.py
+-rw-r--r--   0        0        0    24172 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-05-07 06:18:03.134978 pretext-1.5.3.dev20230507/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-07 06:18:03.134978 pretext-1.5.3.dev20230507/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160171 2023-05-07 06:18:03.110978 pretext-1.5.3.dev20230507/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7677 2023-05-07 06:18:03.126978 pretext-1.5.3.dev20230507/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173370 2023-05-07 06:18:03.122978 pretext-1.5.3.dev20230507/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     1236 2023-05-07 06:18:03.134978 pretext-1.5.3.dev20230507/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4718 2023-05-07 06:18:03.130978 pretext-1.5.3.dev20230507/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0      630 2023-05-07 06:18:03.134978 pretext-1.5.3.dev20230507/pretext/templates/resources/postCreateCommand.sh
+-rw-r--r--   0        0        0     1710 2023-05-07 06:18:03.134978 pretext-1.5.3.dev20230507/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-05-07 06:18:03.134978 pretext-1.5.3.dev20230507/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8453 2023-05-07 06:18:03.134978 pretext-1.5.3.dev20230507/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18300 2023-05-07 06:17:14.137923 pretext-1.5.3.dev20230507/pretext/utils.py
+-rw-r--r--   0        0        0     1119 2023-05-07 06:17:58.022873 pretext-1.5.3.dev20230507/pyproject.toml
+-rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.3.dev20230507/PKG-INFO
```

### Comparing `pretext-1.5.3.dev20230506/LICENSE` & `pretext-1.5.3.dev20230507/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/README.md` & `pretext-1.5.3.dev20230507/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/__init__.py` & `pretext-1.5.3.dev20230507/pretext/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
 
-CORE_COMMIT = 'd658fc893c209a8f31052b661a52fae381f7ff20'
+CORE_COMMIT = '7db4ce5c1b6b52969c4cbc53f52445b5322eb2f8'
 
 
 def activate():
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.5.3.dev20230506/pretext/build.py` & `pretext-1.5.3.dev20230507/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/cli.py` & `pretext-1.5.3.dev20230507/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/codechat.py` & `pretext-1.5.3.dev20230507/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/config/xml_overlay.py` & `pretext-1.5.3.dev20230507/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/core/pretext.py` & `pretext-1.5.3.dev20230507/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/core/resources.py` & `pretext-1.5.3.dev20230507/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/core/resources.zip` & `pretext-1.5.3.dev20230507/pretext/core/resources.zip`

 * *Files 20% similar despite different names*

#### zipinfo {}

```diff
@@ -1,150 +1,150 @@
-Zip file size: 1052517 bytes, number of entries: 148
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 xsl/utilities/
--rw-r--r--  2.0 unx    11766 b- defN 23-May-06 06:17 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx   261852 b- defN 23-May-06 06:17 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-May-06 06:17 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-May-06 06:17 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-May-06 06:17 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-May-06 06:17 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-May-06 06:17 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-May-06 06:17 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-May-06 06:17 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-May-06 06:17 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-May-06 06:17 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    69315 b- defN 23-May-06 06:17 xsl/pretext-braille.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-May-06 06:17 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx   544147 b- defN 23-May-06 06:17 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx    65459 b- defN 23-May-06 06:17 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-May-06 06:17 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-May-06 06:17 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-May-06 06:17 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-May-06 06:17 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-May-06 06:17 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-May-06 06:17 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx   139661 b- defN 23-May-06 06:17 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-May-06 06:17 xsl/README.md
--rw-r--r--  2.0 unx     2740 b- defN 23-May-06 06:17 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx   604338 b- defN 23-May-06 06:17 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-May-06 06:17 xsl/entities.ent
--rw-r--r--  2.0 unx     2846 b- defN 23-May-06 06:17 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-May-06 06:17 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-May-06 06:17 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-May-06 06:17 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx   541182 b- defN 23-May-06 06:17 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-May-06 06:17 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-May-06 06:17 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    39922 b- defN 23-May-06 06:17 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-May-06 06:17 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   103788 b- defN 23-May-06 06:17 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-May-06 06:17 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx   111553 b- defN 23-May-06 06:17 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-May-06 06:17 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-May-06 06:17 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1810 b- defN 23-May-06 06:17 xsl/utilities/README.md
--rw-r--r--  2.0 unx      513 b- defN 23-May-06 06:17 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-May-06 06:17 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-May-06 06:17 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-May-06 06:17 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx    17285 b- defN 23-May-06 06:17 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-May-06 06:17 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-May-06 06:17 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-May-06 06:17 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    15736 b- defN 23-May-06 06:17 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-May-06 06:17 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-May-06 06:17 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-May-06 06:17 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-May-06 06:17 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-May-06 06:17 xsl/localizations/README.md
--rw-r--r--  2.0 unx     2227 b- defN 23-May-06 06:17 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-May-06 06:17 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-May-06 06:17 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-May-06 06:17 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    15938 b- defN 23-May-06 06:17 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-May-06 06:17 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-May-06 06:17 xsl/localizations/pt-PT.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 xsl/support/play-button/
--rw-r--r--  2.0 unx     5800 b- defN 23-May-06 06:17 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-May-06 06:17 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     5065 b- defN 23-May-06 06:17 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-May-06 06:17 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-May-06 06:17 xsl/support/README.md
--rw-r--r--  2.0 unx      486 b- defN 23-May-06 06:17 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5241 b- defN 23-May-06 06:17 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      722 b- defN 23-May-06 06:17 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-May-06 06:17 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-May-06 06:17 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx     3024 b- defN 23-May-06 06:17 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-May-06 06:17 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-May-06 06:17 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-May-06 06:17 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-May-06 06:17 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx   133917 b- defN 23-May-06 06:17 schema/pretext.xml
--rw-r--r--  2.0 unx   124561 b- defN 23-May-06 06:17 schema/pretext.xsd
--rw-r--r--  2.0 unx    18421 b- defN 23-May-06 06:17 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx      326 b- defN 23-May-06 06:17 schema/xml.xsd
--rw-r--r--  2.0 unx    57960 b- defN 23-May-06 06:17 schema/pretext.rnc
--rw-r--r--  2.0 unx     1180 b- defN 23-May-06 06:17 schema/README.md
--rw-r--r--  2.0 unx     3135 b- defN 23-May-06 06:17 schema/build.sh
--rw-r--r--  2.0 unx    34210 b- defN 23-May-06 06:17 schema/pretext-dev.rng
--rw-r--r--  2.0 unx    25290 b- defN 23-May-06 06:17 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    17587 b- defN 23-May-06 06:17 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx   101402 b- defN 23-May-06 06:17 schema/pretext.rng
--rw-r--r--  2.0 unx     2446 b- defN 23-May-06 06:17 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx      691 b- defN 23-May-06 06:17 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx    71198 b- defN 23-May-06 06:17 css/pretext_add_on.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-06 06:17 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     1280 b- defN 23-May-06 06:17 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2438 b- defN 23-May-06 06:17 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx    12567 b- defN 23-May-06 06:17 css/style_oscarlevin.css
--rw-r--r--  2.0 unx    14069 b- defN 23-May-06 06:17 css/setcolors.css
--rw-r--r--  2.0 unx     1865 b- defN 23-May-06 06:17 css/README.md
--rw-r--r--  2.0 unx     4021 b- defN 23-May-06 06:17 css/update_css
--rw-r--r--  2.0 unx     4308 b- defN 23-May-06 06:17 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx   146685 b- defN 23-May-06 06:17 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-May-06 06:17 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-06 06:17 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     7761 b- defN 23-May-06 06:17 css/style_default.css
--rw-r--r--  2.0 unx     1362 b- defN 23-May-06 06:17 css/epub.css
--rw-r--r--  2.0 unx     2608 b- defN 23-May-06 06:17 css/colors_default.css
--rw-r--r--  2.0 unx     3473 b- defN 23-May-06 06:17 css/style_soundwriting.css
--rw-r--r--  2.0 unx   435680 b- defN 23-May-06 06:17 css/mathbook-3.css
--rw-r--r--  2.0 unx     1338 b- defN 23-May-06 06:17 css/colors_red_blue.css
--rw-r--r--  2.0 unx     2441 b- defN 23-May-06 06:17 css/kindle.css
--rw-r--r--  2.0 unx    63664 b- defN 23-May-06 06:17 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     1276 b- defN 23-May-06 06:17 css/colors_maroon_grey.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 script/braille/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-May-06 06:17 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-May-06 06:17 script/mbx
--rw-r--r--  2.0 unx     2573 b- defN 23-May-06 06:17 script/braille/pretext-symbol.dis
--rw-r--r--  2.0 unx     8913 b- defN 23-May-06 06:17 script/braille/pretext.sem
--rw-r--r--  2.0 unx      735 b- defN 23-May-06 06:17 script/braille/README.md
--rw-r--r--  2.0 unx     6616 b- defN 23-May-06 06:17 script/braille/pretext-liblouis.cfg
--rw-r--r--  2.0 unx     1011 b- defN 23-May-06 06:17 script/braille/pretext-liblouis-emboss.cfg
--rw-r--r--  2.0 unx      490 b- defN 23-May-06 06:17 script/braille/pretext-liblouis-electronic.cfg
--rw-r--r--  2.0 unx      481 b- defN 23-May-06 06:17 script/mjsre/README.md
--rw-r--r--  2.0 unx       92 b- defN 23-May-06 06:17 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-May-06 06:17 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx      116 b- defN 23-May-06 06:17 script/mjsre/package.json
--rw-r--r--  2.0 unx     2566 b- defN 23-May-06 06:17 pretext/pretext.cfg
--rw-r--r--  2.0 unx     1367 b- defN 23-May-06 06:17 pretext/README.md
--rw-r--r--  2.0 unx   173946 b- defN 23-May-06 06:17 pretext/pretext.py
--rw-r--r--  2.0 unx    35057 b- defN 23-May-06 06:17 pretext/braille_format.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-06 06:17 pretext/__init__.py
--rw-r--r--  2.0 unx     1955 b- defN 23-May-06 06:17 pretext/module-test.py
--rw-r--r--  2.0 unx    31361 b- defN 23-May-06 06:17 pretext/pretext
-148 files, 4879036 bytes uncompressed, 1034093 bytes compressed:  78.8%
+Zip file size: 1052638 bytes, number of entries: 148
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 xsl/utilities/
+-rw-r--r--  2.0 unx    11766 b- defN 23-May-07 06:18 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx   261852 b- defN 23-May-07 06:18 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-May-07 06:18 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-May-07 06:18 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-May-07 06:18 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-May-07 06:18 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-May-07 06:18 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-May-07 06:18 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-May-07 06:18 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-May-07 06:18 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-May-07 06:18 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    69315 b- defN 23-May-07 06:18 xsl/pretext-braille.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-May-07 06:18 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx   544213 b- defN 23-May-07 06:18 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    65459 b- defN 23-May-07 06:18 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-May-07 06:18 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-May-07 06:18 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-May-07 06:18 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-May-07 06:18 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-May-07 06:18 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-May-07 06:18 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-May-07 06:18 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-May-07 06:18 xsl/README.md
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-07 06:18 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx   604691 b- defN 23-May-07 06:18 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-May-07 06:18 xsl/entities.ent
+-rw-r--r--  2.0 unx     2846 b- defN 23-May-07 06:18 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-May-07 06:18 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-May-07 06:18 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-May-07 06:18 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx   541182 b- defN 23-May-07 06:18 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-May-07 06:18 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-May-07 06:18 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    39922 b- defN 23-May-07 06:18 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-May-07 06:18 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx   103788 b- defN 23-May-07 06:18 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-May-07 06:18 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx   111553 b- defN 23-May-07 06:18 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-May-07 06:18 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-May-07 06:18 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1810 b- defN 23-May-07 06:18 xsl/utilities/README.md
+-rw-r--r--  2.0 unx      513 b- defN 23-May-07 06:18 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 23-May-07 06:18 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-May-07 06:18 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-May-07 06:18 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx    17285 b- defN 23-May-07 06:18 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-May-07 06:18 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-May-07 06:18 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-May-07 06:18 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    15736 b- defN 23-May-07 06:18 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-May-07 06:18 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-May-07 06:18 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-May-07 06:18 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-May-07 06:18 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-May-07 06:18 xsl/localizations/README.md
+-rw-r--r--  2.0 unx     2227 b- defN 23-May-07 06:18 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-May-07 06:18 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-May-07 06:18 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-May-07 06:18 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    15938 b- defN 23-May-07 06:18 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-May-07 06:18 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-May-07 06:18 xsl/localizations/pt-PT.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 xsl/support/play-button/
+-rw-r--r--  2.0 unx     5800 b- defN 23-May-07 06:18 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-May-07 06:18 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     5065 b- defN 23-May-07 06:18 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-May-07 06:18 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-May-07 06:18 xsl/support/README.md
+-rw-r--r--  2.0 unx      486 b- defN 23-May-07 06:18 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5241 b- defN 23-May-07 06:18 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      722 b- defN 23-May-07 06:18 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-May-07 06:18 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-May-07 06:18 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx     3024 b- defN 23-May-07 06:18 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-May-07 06:18 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-May-07 06:18 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-May-07 06:18 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-May-07 06:18 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx   133930 b- defN 23-May-07 06:18 schema/pretext.xml
+-rw-r--r--  2.0 unx   124610 b- defN 23-May-07 06:18 schema/pretext.xsd
+-rw-r--r--  2.0 unx    18421 b- defN 23-May-07 06:18 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx      326 b- defN 23-May-07 06:18 schema/xml.xsd
+-rw-r--r--  2.0 unx    57973 b- defN 23-May-07 06:18 schema/pretext.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-May-07 06:18 schema/README.md
+-rw-r--r--  2.0 unx     3135 b- defN 23-May-07 06:18 schema/build.sh
+-rw-r--r--  2.0 unx    34210 b- defN 23-May-07 06:18 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx    25290 b- defN 23-May-07 06:18 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    17587 b- defN 23-May-07 06:18 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx   101444 b- defN 23-May-07 06:18 schema/pretext.rng
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-07 06:18 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx      691 b- defN 23-May-07 06:18 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-May-07 06:18 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-07 06:18 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-07 06:18 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-07 06:18 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-07 06:18 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-May-07 06:18 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-May-07 06:18 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-07 06:18 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-May-07 06:18 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-May-07 06:18 css/setcolors.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-May-07 06:18 css/README.md
+-rw-r--r--  2.0 unx     4021 b- defN 23-May-07 06:18 css/update_css
+-rw-r--r--  2.0 unx     4308 b- defN 23-May-07 06:18 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-07 06:18 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-May-07 06:18 css/mathbook-content.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-May-07 06:18 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-07 06:18 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-07 06:18 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-May-07 06:18 css/style_default.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-May-07 06:18 css/epub.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-May-07 06:18 css/colors_default.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-May-07 06:18 css/style_soundwriting.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-May-07 06:18 css/mathbook-3.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-May-07 06:18 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-May-07 06:18 css/kindle.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-May-07 06:18 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-May-07 06:18 css/colors_maroon_grey.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 script/braille/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-May-07 06:18 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-May-07 06:18 script/mbx
+-rw-r--r--  2.0 unx     2573 b- defN 23-May-07 06:18 script/braille/pretext-symbol.dis
+-rw-r--r--  2.0 unx     8913 b- defN 23-May-07 06:18 script/braille/pretext.sem
+-rw-r--r--  2.0 unx      735 b- defN 23-May-07 06:18 script/braille/README.md
+-rw-r--r--  2.0 unx     6616 b- defN 23-May-07 06:18 script/braille/pretext-liblouis.cfg
+-rw-r--r--  2.0 unx     1011 b- defN 23-May-07 06:18 script/braille/pretext-liblouis-emboss.cfg
+-rw-r--r--  2.0 unx      490 b- defN 23-May-07 06:18 script/braille/pretext-liblouis-electronic.cfg
+-rw-r--r--  2.0 unx      481 b- defN 23-May-07 06:18 script/mjsre/README.md
+-rw-r--r--  2.0 unx       92 b- defN 23-May-07 06:18 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-May-07 06:18 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx      116 b- defN 23-May-07 06:18 script/mjsre/package.json
+-rw-r--r--  2.0 unx     2566 b- defN 23-May-07 06:18 pretext/pretext.cfg
+-rw-r--r--  2.0 unx     1367 b- defN 23-May-07 06:18 pretext/README.md
+-rw-r--r--  2.0 unx   173946 b- defN 23-May-07 06:18 pretext/pretext.py
+-rw-r--r--  2.0 unx    35057 b- defN 23-May-07 06:18 pretext/braille_format.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-07 06:18 pretext/__init__.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-May-07 06:18 pretext/module-test.py
+-rw-r--r--  2.0 unx    31361 b- defN 23-May-07 06:18 pretext/pretext
+148 files, 4879397 bytes uncompressed, 1034214 bytes compressed:  78.8%
```

#### xsl/pretext-common.xsl

##### xsl/pretext-common.xsl

```diff
@@ -132,15 +132,16 @@
   <!-- ######### -->
   <!-- Variables -->
   <!-- ######### -->
   <!-- The single quote character cannot be directly     -->
   <!-- used in a string in XSLT functions, not even as   -->
   <!-- &apos;. But if it is stored as a variable, then   -->
   <!-- XSLT 1.0 will be OK with using $apos.             -->
-  <!-- Use like "contat('L',$apos,'Hospital')"           -->
+  <!-- Use like "concat('L',$apos,'Hospital')"           -->
+  <!-- Unicode Character 'APOSTROPHE' (U+0027)           -->
   <xsl:variable name="apos">'</xsl:variable>
   <!-- Here we perform manipulations of math elements and subsequent  -->
   <!-- text nodes that lead with punctuation.  Basically, punctuation -->
   <!-- can migrate from the start of the text node and into the math, -->
   <!-- wrapped in a \text{}.  We generally do this to display math as -->
   <!-- a service to authors.  MathJax needs help for inline math.     -->
   <!-- Braille and audio do not do so well with this manipulation.    -->
```

#### xsl/extract-pg.xsl

##### xsl/extract-pg.xsl

```diff
@@ -794,16 +794,16 @@
       <!-- targeted feedback messages for specific wrong answers -->
       <xsl:if test="contains(.//pg-code,'AnswerHints')">
         <xsl:call-template name="macro-padding">
           <xsl:with-param name="string" select="'answerHints.pl'"/>
           <xsl:with-param name="b-human-readable" select="$b-human-readable"/>
         </xsl:call-template>
       </xsl:if>
-      <!-- checkboxes multiple choice answers or the very useful NchooseK function-->
-      <xsl:if test=".//var[@form='checkboxes'] or contains(.//pg-code,'NchooseK')">
+      <!-- the very useful NchooseK function-->
+      <xsl:if test="contains(.//pg-code,'NchooseK')">
         <xsl:call-template name="macro-padding">
           <xsl:with-param name="string" select="'PGchoicemacros.pl'"/>
           <xsl:with-param name="b-human-readable" select="$b-human-readable"/>
         </xsl:call-template>
       </xsl:if>
       <!-- essay answers -->
       <xsl:if test=".//var[@form='essay'] or contains(.//pg-code,'explanation_box')">
@@ -922,14 +922,19 @@
         <xsl:with-param name="b-human-readable" select="$b-human-readable"/>
       </xsl:apply-templates>
       <!-- popup menu multiple choice answers -->
       <xsl:apply-templates select="." mode="parser">
         <xsl:with-param name="parser" select="'PopUp'"/>
         <xsl:with-param name="b-human-readable" select="$b-human-readable"/>
       </xsl:apply-templates>
+      <!-- checkboxes multiple choice answers -->
+      <xsl:apply-templates select="." mode="parser">
+        <xsl:with-param name="parser" select="'CheckboxList'"/>
+        <xsl:with-param name="b-human-readable" select="$b-human-readable"/>
+      </xsl:apply-templates>
       <!-- allow "'" as part of answers, as an effective derivative operator -->
       <!-- note unusual usage precludes using parser modal template here -->
       <xsl:if test="contains(.//pg-code,'parser::Prime')">
         <xsl:call-template name="macro-padding">
           <xsl:with-param name="string" select="'parserPrime.pl'"/>
           <xsl:with-param name="b-human-readable" select="$b-human-readable"/>
         </xsl:call-template>
@@ -1286,17 +1291,14 @@
   <!-- ############## -->
   <!-- PERL Variables -->
   <!-- ############## -->
   <!-- PGML markup for Perl variable in LaTeX expression -->
   <xsl:template match="var">
     <xsl:text>[</xsl:text>
     <xsl:value-of select="@name"/>
-    <xsl:if test="@form='checkboxes'">
-      <xsl:text>-&gt;correct_ans()</xsl:text>
-    </xsl:if>
     <xsl:text>]</xsl:text>
     <!-- if the variable is a string of PGML syntax to be processed -->
     <xsl:if test="@data='pgml'">
       <xsl:text>**</xsl:text>
     </xsl:if>
   </xsl:template>
   <xsl:template match="latex-image/var" mode="latex-image">
@@ -1325,19 +1327,27 @@
           <xsl:value-of select="@width"/>
         </xsl:when>
         <xsl:otherwise>
           <xsl:text>5</xsl:text>
         </xsl:otherwise>
       </xsl:choose>
     </xsl:variable>
-    <!-- when an answer blank is the first thing on a line, indent -->
-    <!-- this is a styling preference that can't be customized     -->
-    <xsl:if test="(count(preceding-sibling::*)+count(preceding-sibling::text()))=0 and parent::p/parent::statement">
-      <xsl:text/>
-    </xsl:if>
+    <!-- Answer inputs all on their own p get indented         -->
+    <!-- This is a styling preference that can't be customized -->
+    <xsl:choose>
+      <!-- We don't indent for radio buttons or checkboxes input -->
+      <!-- which ought to be in their own p in the first place   -->
+      <xsl:when test="@form = 'buttons' or @form = 'checkboxes'"/>
+      <!-- We don't indent for answer input that is within certain structures -->
+      <xsl:when test="ancestor::li or ancestor::tabular"/>
+      <!-- We don't indent when the input field is inline with a p -->
+      <xsl:when test="count(parent::p/*) + string-length(normalize-space(parent::p/text())) = 0">
+        <xsl:text/>
+      </xsl:when>
+    </xsl:choose>
     <xsl:text>[_]</xsl:text>
     <!-- multiplier for MathObjects like Matrix, Vector, ColumnVector -->
     <xsl:if test="@form='array'">
       <xsl:text>*</xsl:text>
     </xsl:if>
     <xsl:text>{</xsl:text>
     <xsl:choose>
@@ -1349,29 +1359,14 @@
       </xsl:otherwise>
     </xsl:choose>
     <xsl:text>}</xsl:text>
     <xsl:text>{</xsl:text>
     <xsl:value-of select="$width"/>
     <xsl:text>}</xsl:text>
   </xsl:template>
-  <!-- Checkbox answers -->
-  <!-- TODO: not really supported yet. The checkbox handling in WeBWorK is  -->
-  <!-- technically broken. The issue is only surfacing when trying to do a  -->
-  <!-- checkbox problem from an iframe. Any attempt to check multiple boxes -->
-  <!-- and submit leads to only one box being seen as checked by WeBWorK.   -->
-  <xsl:template match="var[@form='checkboxes']" mode="field">
-    <xsl:text>[@</xsl:text>
-    <xsl:value-of select="@name"/>
-    <xsl:text>-&gt;print_a() @]*</xsl:text>
-    <xsl:text>END_PGML</xsl:text>
-    <xsl:text>ANS(checkbox_cmp(</xsl:text>
-    <xsl:value-of select="@name"/>
-    <xsl:text>-&gt;correct_ans()));</xsl:text>
-    <xsl:text>BEGIN_PGML</xsl:text>
-  </xsl:template>
   <!-- Essay answers -->
   <!-- Example: [@ ANS(essay_cmp); essay_box(6,76) @]*   -->
   <!-- Requires:  PGessaymacros.pl, automatically loaded -->
   <!-- http://webwork.maa.org/moodle/mod/forum/discuss.php?d=3370 -->
   <xsl:template match="var[@form='essay']" mode="field">
     <xsl:param name="b-human-readable"/>
     <xsl:text>[@ANS(essay_cmp());</xsl:text>
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -5603,17 +5603,24 @@
     <xsl:text/>
   </xsl:template>
   <!-- Once upon a time, we broke up markup meant for MathJax that occured   -->
   <!-- outside of what we know is a mathematical context ("accidental        -->
   <!-- mathematics").   We did this by breaking up strings with a zero-width -->
   <!-- space (U+200B), but a better device is wrapping a delimiter in a span -->
   <!-- (see this technique in the "text-processing" template in the Jupyter  -->
-  <!-- conversion.  However, MathJax 3 lets us target/ignore spcific         -->
+  <!-- conversion).  However, MathJax 3 lets us target/ignore specific       -->
   <!-- locations for its translation.  So the "text-processing" template     -->
-  <!-- that was once here is now gone.                                       -->
+  <!-- that was once here is now gone.  But now it is back, to upgrade a     -->
+  <!-- keyboard "plain" apostrophe to a Unicode "curly" apostrophe.          -->
+  <xsl:template name="text-processing">
+    <xsl:param name="text"/>
+    <!-- 'RIGHT SINGLE QUOTATION MARK' (U+2019) -->
+    <xsl:variable name="apostophe-fixed" select="str:replace($text, $apos, '’')"/>
+    <xsl:value-of select="$apostophe-fixed"/>
+  </xsl:template>
   <!-- We cruise knowled content for necessity of hidden knowls -->
   <xsl:template match="*" mode="is-hidden">
     <xsl:text>false</xsl:text>
   </xsl:template>
   <!-- ############################# -->
   <!-- End: Block Production, Knowls -->
   <!-- ############################# -->
```

#### schema/pretext.xml

##### schema/pretext.xml

```diff
@@ -2690,15 +2690,15 @@
                     attribute category {
                                         &quot;angle&quot; | &quot;decimal&quot; | &quot;exponent&quot;
                                       | &quot;formula&quot; | &quot;fraction&quot; | &quot;inequality&quot;
                                       | &quot;integer&quot; | &quot;interval&quot; | &quot;logarithm&quot;
                                       | &quot;limit&quot; | &quot;number&quot; | &quot;point&quot;
                                       | &quot;syntax&quot; | &quot;quantity&quot; | &quot;vector&quot;
                                       }?,
-                    attribute form {&quot;popup&quot;|&quot;buttons&quot;|&quot;none&quot;}?) |
+                    attribute form {&quot;popup&quot;|&quot;buttons&quot;|&quot;checkboxes&quot;|&quot;none&quot;}?) |
                     (attribute form {&quot;essay&quot;},
                     attribute width {text}?)
                 }
             WWInstruction =
                 element instruction {TextShort}
             HintWW =
                 element hint {
```

#### schema/pretext.xsd

##### schema/pretext.xsd

```diff
@@ -2425,14 +2425,15 @@
     </xs:annotation>
     <xs:complexType>
       <xs:attribute name="form">
         <xs:simpleType>
           <xs:restriction base="xs:token">
             <xs:enumeration value="popup"/>
             <xs:enumeration value="buttons"/>
+            <xs:enumeration value="checkboxes"/>
             <xs:enumeration value="none"/>
             <xs:enumeration value="essay"/>
           </xs:restriction>
         </xs:simpleType>
       </xs:attribute>
       <xs:attribute name="name"/>
       <xs:attribute name="evaluator"/>
```

#### schema/pretext.rnc

```diff
@@ -1069,15 +1069,15 @@
                     attribute category {
                                         "angle" | "decimal" | "exponent"
                                       | "formula" | "fraction" | "inequality"
                                       | "integer" | "interval" | "logarithm"
                                       | "limit" | "number" | "point"
                                       | "syntax" | "quantity" | "vector"
                                       }?,
-                    attribute form {"popup"|"buttons"|"none"}?) |
+                    attribute form {"popup"|"buttons"|"checkboxes"|"none"}?) |
                     (attribute form {"essay"},
                     attribute width {text}?)
                 }
             WWInstruction =
                 element instruction {TextShort}
             HintWW =
                 element hint {
```

#### schema/pretext.rng

##### schema/pretext.rng

```diff
@@ -2746,14 +2746,15 @@
             </attribute>
           </optional>
           <optional>
             <attribute name="form">
               <choice>
                 <value>popup</value>
                 <value>buttons</value>
+                <value>checkboxes</value>
                 <value>none</value>
               </choice>
             </attribute>
           </optional>
         </group>
         <group>
           <attribute name="form">
```

### Comparing `pretext-1.5.3.dev20230506/pretext/generate.py` & `pretext-1.5.3.dev20230507/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/project.py` & `pretext-1.5.3.dev20230507/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/templates/__init__.py` & `pretext-1.5.3.dev20230507/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/templates/resources/.gitignore` & `pretext-1.5.3.dev20230507/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/templates/resources/article.zip` & `pretext-1.5.3.dev20230507/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 160171 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-06 06:17 codechat_config.yaml
--rw-r--r--  2.0 unx       86 b- defN 23-May-06 06:16 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-06 06:17 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-06 06:17 .gitignore
--rw-r--r--  2.0 unx      242 b- defN 23-May-06 06:16 publication/publication.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-May-06 06:16 assets/frog.jpg
--rw-r--r--  2.0 unx      630 b- defN 23-May-06 06:17 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-06 06:17 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      449 b- defN 23-May-06 06:16 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-May-06 06:16 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-May-06 06:16 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-07 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx       86 b- defN 23-May-07 06:17 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-07 06:18 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-07 06:18 .gitignore
+-rw-r--r--  2.0 unx      242 b- defN 23-May-07 06:17 publication/publication.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-07 06:17 assets/frog.jpg
+-rw-r--r--  2.0 unx      630 b- defN 23-May-07 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-07 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      449 b- defN 23-May-07 06:17 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-May-07 06:17 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-May-07 06:17 source/main.ptx
 15 files, 164515 bytes uncompressed, 158505 bytes compressed:  3.7%
```

### Comparing `pretext-1.5.3.dev20230506/pretext/templates/resources/book.zip` & `pretext-1.5.3.dev20230507/pretext/templates/resources/book.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 7677 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-06 06:17 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-May-06 06:16 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-06 06:17 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-06 06:17 .gitignore
--rw-r--r--  2.0 unx     6114 b- defN 23-May-06 06:16 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-06 06:17 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-06 06:17 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     1767 b- defN 23-May-06 06:16 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-07 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-May-07 06:17 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-07 06:18 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-07 06:18 .gitignore
+-rw-r--r--  2.0 unx     6114 b- defN 23-May-07 06:17 publication/publication.ptx
+-rw-r--r--  2.0 unx      630 b- defN 23-May-07 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-07 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     1767 b- defN 23-May-07 06:17 source/main.ptx
 11 files, 15483 bytes uncompressed, 6439 bytes compressed:  58.4%
```

### Comparing `pretext-1.5.3.dev20230506/pretext/templates/resources/demo.zip` & `pretext-1.5.3.dev20230507/pretext/templates/resources/demo.zip`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,37 +1,37 @@
 Zip file size: 173370 bytes, number of entries: 35
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-06 06:17 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-May-06 06:16 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-06 06:17 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-06 06:17 .gitignore
--rw-r--r--  2.0 unx     6092 b- defN 23-May-06 06:16 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-May-06 06:16 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-May-06 06:16 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx      630 b- defN 23-May-06 06:17 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-06 06:17 .devcontainer/devcontainer.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 source/images/
--rw-r--r--  2.0 unx      339 b- defN 23-May-06 06:16 source/ch-features.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-May-06 06:16 source/ch-generate.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-May-06 06:16 source/frontmatter.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-May-06 06:16 source/sec-features.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-May-06 06:16 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-May-06 06:16 source/ch-empty.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-May-06 06:16 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-May-06 06:16 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-May-06 06:16 source/docinfo.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-May-06 06:16 source/ex-first.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-May-06 06:16 source/backmatter.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-May-06 06:16 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-May-06 06:16 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-May-06 06:16 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-May-06 06:16 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-May-06 06:16 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-May-06 06:16 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 23-May-06 06:16 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-May-06 06:16 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx       10 b- defN 23-May-06 06:16 source/images/sageplot2d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-07 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-May-07 06:17 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-07 06:18 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-07 06:18 .gitignore
+-rw-r--r--  2.0 unx     6092 b- defN 23-May-07 06:17 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-07 06:17 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-May-07 06:17 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx      630 b- defN 23-May-07 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-07 06:18 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 source/images/
+-rw-r--r--  2.0 unx      339 b- defN 23-May-07 06:17 source/ch-features.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-May-07 06:17 source/ch-generate.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-May-07 06:17 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-May-07 06:17 source/sec-features.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-May-07 06:17 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-May-07 06:17 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-May-07 06:17 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-May-07 06:17 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-May-07 06:17 source/docinfo.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-May-07 06:17 source/ex-first.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-May-07 06:17 source/backmatter.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-May-07 06:17 source/main.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-May-07 06:17 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-May-07 06:17 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-May-07 06:17 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-May-07 06:17 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-May-07 06:17 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 23-May-07 06:17 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-May-07 06:17 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx       10 b- defN 23-May-07 06:17 source/images/sageplot2d.sage
 35 files, 189778 bytes uncompressed, 169270 bytes compressed:  10.8%
```

### Comparing `pretext-1.5.3.dev20230506/pretext/templates/resources/devcontainer.json` & `pretext-1.5.3.dev20230507/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/templates/resources/hello.zip` & `pretext-1.5.3.dev20230507/pretext/templates/resources/hello.zip`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 4718 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-06 06:17 codechat_config.yaml
--rw-r--r--  2.0 unx       69 b- defN 23-May-06 06:16 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-May-06 06:16 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-06 06:17 .gitignore
--rw-r--r--  2.0 unx      242 b- defN 23-May-06 06:16 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-06 06:17 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-06 06:17 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      156 b- defN 23-May-06 06:16 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-07 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx       69 b- defN 23-May-07 06:17 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-May-07 06:17 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-07 06:18 .gitignore
+-rw-r--r--  2.0 unx      242 b- defN 23-May-07 06:17 publication/publication.ptx
+-rw-r--r--  2.0 unx      630 b- defN 23-May-07 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-07 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      156 b- defN 23-May-07 06:17 source/main.ptx
 11 files, 7494 bytes uncompressed, 3480 bytes compressed:  53.6%
```

### Comparing `pretext-1.5.3.dev20230506/pretext/templates/resources/postCreateCommand.sh` & `pretext-1.5.3.dev20230507/pretext/templates/resources/postCreateCommand.sh`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/templates/resources/project.ptx` & `pretext-1.5.3.dev20230507/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pretext/templates/resources/slideshow.zip` & `pretext-1.5.3.dev20230507/pretext/templates/resources/slideshow.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 8453 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:17 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-06 06:16 xsl/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-06 06:17 codechat_config.yaml
--rw-r--r--  2.0 unx      784 b- defN 23-May-06 06:16 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-06 06:17 .gitignore
--rw-r--r--  2.0 unx      190 b- defN 23-May-06 06:16 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-May-06 06:16 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-06 06:17 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-06 06:17 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx    11200 b- defN 23-May-06 06:16 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-07 06:17 xsl/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-07 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx      784 b- defN 23-May-07 06:17 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-07 06:18 .gitignore
+-rw-r--r--  2.0 unx      190 b- defN 23-May-07 06:17 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-May-07 06:17 publication/publication.ptx
+-rw-r--r--  2.0 unx      630 b- defN 23-May-07 06:18 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-07 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx    11200 b- defN 23-May-07 06:17 source/main.ptx
 12 files, 20081 bytes uncompressed, 7121 bytes compressed:  64.5%
```

### Comparing `pretext-1.5.3.dev20230506/pretext/utils.py` & `pretext-1.5.3.dev20230507/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230506/pyproject.toml` & `pretext-1.5.3.dev20230507/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.5.3.dev20230506"
+version = "1.5.3.dev20230507"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.5.3.dev20230506/PKG-INFO` & `pretext-1.5.3.dev20230507/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.5.3.dev20230506
+Version: 1.5.3.dev20230507
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

