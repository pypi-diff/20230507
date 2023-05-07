# Comparing `tmp/satsim-0.15.0.tar.gz` & `tmp/satsim-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsim-0.15.0.tar", last modified: Thu May  4 05:43:55 2023, max compression
+gzip compressed data, was "satsim-0.15.1.tar", last modified: Sun May  7 18:08:12 2023, max compression
```

## Comparing `satsim-0.15.0.tar` & `satsim-0.15.1.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.635508 satsim-0.15.0/
--rw-r--r--   0 root         (0) root         (0)      170 2022-07-22 19:32:02.000000 satsim-0.15.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     3255 2023-02-17 19:27:57.000000 satsim-0.15.0/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)     6957 2023-05-04 05:31:05.000000 satsim-0.15.0/HISTORY.md
--rw-r--r--   0 root         (0) root         (0)      291 2022-07-22 19:32:02.000000 satsim-0.15.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8582 2023-05-04 05:43:55.635508 satsim-0.15.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1049 2023-05-04 05:31:05.000000 satsim-0.15.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.615508 satsim-0.15.0/docs/
--rw-r--r--   0 root         (0) root         (0)      608 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.615508 satsim-0.15.0/docs/_build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.615508 satsim-0.15.0/docs/_build/html/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.615508 satsim-0.15.0/docs/_build/html/_static/
--rw-r--r--   0 root         (0) root         (0)    14813 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.615508 satsim-0.15.0/docs/_build/html/_static/css/
--rw-r--r--   0 root         (0) root         (0)     3229 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.615508 satsim-0.15.0/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 root         (0) root         (0)   165742 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   444379 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   165548 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    98024 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    77160 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 root         (0) root         (0)   135235 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 root         (0) root         (0)     4472 2023-05-04 05:40:35.000000 satsim-0.15.0/docs/_build/html/_static/doctools.js
--rw-r--r--   0 root         (0) root         (0)      421 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 root         (0) root         (0)      286 2023-05-04 05:40:35.000000 satsim-0.15.0/docs/_build/html/_static/file.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/docs/_build/html/_static/js/
--rw-r--r--   0 root         (0) root         (0)      934 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 root         (0) root         (0)     4370 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 root         (0) root         (0)     2734 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 root         (0) root         (0)     5023 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 root         (0) root         (0)     4758 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/_static/language_data.js
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-04 05:40:35.000000 satsim-0.15.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-04 05:40:35.000000 satsim-0.15.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 root         (0) root         (0)     4846 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/_static/pygments.css
--rw-r--r--   0 root         (0) root         (0)    18215 2023-05-04 05:40:35.000000 satsim-0.15.0/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 root         (0) root         (0)     4712 2023-05-04 05:40:35.000000 satsim-0.15.0/docs/_build/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/docs/_build/html/api/
--rw-r--r--   0 root         (0) root         (0)    10121 2023-05-04 05:43:52.000000 satsim-0.15.0/docs/_build/html/api/satsim.dataset.html
--rw-r--r--   0 root         (0) root         (0)    10056 2023-05-04 05:43:52.000000 satsim-0.15.0/docs/_build/html/api/satsim.generator.html
--rw-r--r--   0 root         (0) root         (0)    59162 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.generator.obs.html
--rw-r--r--   0 root         (0) root         (0)   106508 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.geometry.html
--rw-r--r--   0 root         (0) root         (0)   159759 2023-05-04 05:43:52.000000 satsim-0.15.0/docs/_build/html/api/satsim.html
--rw-r--r--   0 root         (0) root         (0)    91699 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.image.html
--rw-r--r--   0 root         (0) root         (0)    37488 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.io.html
--rw-r--r--   0 root         (0) root         (0)    33473 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.math.html
--rw-r--r--   0 root         (0) root         (0)    14551 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.pipeline.html
--rw-r--r--   0 root         (0) root         (0)    19353 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.time.html
--rw-r--r--   0 root         (0) root         (0)    24867 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.util.html
--rw-r--r--   0 root         (0) root         (0)   404446 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/api/satsim.vecmath.html
--rw-r--r--   0 root         (0) root         (0)   122688 2023-05-04 05:43:52.000000 satsim-0.15.0/docs/_build/html/api.html
--rw-r--r--   0 root         (0) root         (0)     5491 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/authors.html
--rw-r--r--   0 root         (0) root         (0)    13939 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/contributing.html
--rw-r--r--   0 root         (0) root         (0)    95509 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/genindex.html
--rw-r--r--   0 root         (0) root         (0)    18083 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/history.html
--rw-r--r--   0 root         (0) root         (0)     9534 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/index.html
--rw-r--r--   0 root         (0) root         (0)     7750 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/installation.html
--rw-r--r--   0 root         (0) root         (0)    17277 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/py-modindex.html
--rw-r--r--   0 root         (0) root         (0)     4196 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/search.html
--rw-r--r--   0 root         (0) root         (0)   122825 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/searchindex.js
--rw-r--r--   0 root         (0) root         (0)    37538 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/usage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/docs/api/
--rw-r--r--   0 root         (0) root         (0)      310 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.dataset.rst
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.generator.obs.rst
--rw-r--r--   0 root         (0) root         (0)      218 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.generator.rst
--rw-r--r--   0 root         (0) root         (0)     1872 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.geometry.rst
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.image.rst
--rw-r--r--   0 root         (0) root         (0)      673 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.io.rst
--rw-r--r--   0 root         (0) root         (0)     1138 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.math.rst
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.pipeline.rst
--rw-r--r--   0 root         (0) root         (0)      730 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.rst
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.time.rst
--rw-r--r--   0 root         (0) root         (0)      572 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.util.rst
--rw-r--r--   0 root         (0) root         (0)     1276 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.vecmath.rst
--rw-r--r--   0 root         (0) root         (0)      136 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/api.rst
--rw-r--r--   0 root         (0) root         (0)       28 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/authors.rst
--rw-r--r--   0 root         (0) root         (0)     4906 2023-05-04 05:31:05.000000 satsim-0.15.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)       33 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)       27 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/history.rst
--rw-r--r--   0 root         (0) root         (0)      265 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1475 2023-02-17 19:27:57.000000 satsim-0.15.0/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      768 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)    11419 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/
--rw-r--r--   0 root         (0) root         (0)      264 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4131 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/cli.py
--rw-r--r--   0 root         (0) root         (0)    20530 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3455 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/dataset/augment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/generator/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/generator/obs/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/obs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12937 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/obs/breakup.py
--rw-r--r--   0 root         (0) root         (0)     2330 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/obs/cso.py
--rw-r--r--   0 root         (0) root         (0)     6239 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/obs/geometry.py
--rw-r--r--   0 root         (0) root         (0)     1248 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/obs/io.py
--rw-r--r--   0 root         (0) root         (0)     3703 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/obs/rpo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/geometry/
--rw-r--r--   0 root         (0) root         (0)       66 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/geometry/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20912 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/geometry/astrometric.py
--rw-r--r--   0 root         (0) root         (0)     2251 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/geometry/csvsc.py
--rw-r--r--   0 root         (0) root         (0)     5268 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/geometry/draw.py
--rw-r--r--   0 root         (0) root         (0)     3404 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/geometry/ephemeris.py
--rw-r--r--   0 root         (0) root         (0)     1672 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/geometry/random.py
--rw-r--r--   0 root         (0) root         (0)     1150 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/geometry/sgp4.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/geometry/sprite.py
--rw-r--r--   0 root         (0) root         (0)    11346 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/geometry/sstr7.py
--rw-r--r--   0 root         (0) root         (0)     4340 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/geometry/transform.py
--rw-r--r--   0 root         (0) root         (0)     4619 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/geometry/twobody.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-02-17 00:02:42.000000 satsim-0.15.0/satsim/geometry/wcs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/image/
--rw-r--r--   0 root         (0) root         (0)       58 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/image/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9793 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/image/augment.py
--rw-r--r--   0 root         (0) root         (0)    16625 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/image/fpa.py
--rw-r--r--   0 root         (0) root         (0)     5359 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/image/model.py
--rw-r--r--   0 root         (0) root         (0)     2895 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/image/noise.py
--rw-r--r--   0 root         (0) root         (0)     6166 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/image/psf.py
--rw-r--r--   0 root         (0) root         (0)    10401 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/image/render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/io/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14550 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/io/czml.py
--rw-r--r--   0 root         (0) root         (0)     4319 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/io/fits.py
--rw-r--r--   0 root         (0) root         (0)     2445 2023-03-15 01:56:05.000000 satsim-0.15.0/satsim/io/image.py
--rw-r--r--   0 root         (0) root         (0)     8031 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/io/satnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/math/
--rw-r--r--   0 root         (0) root         (0)       81 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/math/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-04-05 08:00:38.000000 satsim-0.15.0/satsim/math/angle.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/math/const.py
--rw-r--r--   0 root         (0) root         (0)      951 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/math/conv.py
--rw-r--r--   0 root         (0) root         (0)     5551 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/math/fft.py
--rw-r--r--   0 root         (0) root         (0)     2726 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/math/interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2948 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/math/random.py
--rw-r--r--   0 root         (0) root         (0)      590 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/math/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/pipeline/
--rw-r--r--   0 root         (0) root         (0)     1087 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42871 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/satsim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/time/
--rw-r--r--   0 root         (0) root         (0)     4259 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/time/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/util/
--rw-r--r--   0 root         (0) root         (0)      130 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2761 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/util/system.py
--rw-r--r--   0 root         (0) root         (0)     3271 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/util/thread.py
--rw-r--r--   0 root         (0) root         (0)     2044 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/util/timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/vecmath/
--rw-r--r--   0 root         (0) root         (0)    17668 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Cartesian2.py
--rw-r--r--   0 root         (0) root         (0)    20896 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Cartesian3.py
--rw-r--r--   0 root         (0) root         (0)    18429 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Cartesian4.py
--rw-r--r--   0 root         (0) root         (0)    21727 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Matrix2.py
--rw-r--r--   0 root         (0) root         (0)    42567 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Matrix3.py
--rw-r--r--   0 root         (0) root         (0)    73877 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Matrix4.py
--rw-r--r--   0 root         (0) root         (0)    25251 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Quaternion.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8582 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3994 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      539 2023-05-04 05:43:55.635508 satsim-0.15.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1796 2023-05-04 05:31:05.000000 satsim-0.15.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/tests/
--rw-r--r--   0 root         (0) root         (0)       64 2023-02-20 21:03:12.000000 satsim-0.15.0/tests/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.613806 satsim-0.15.1/
+-rw-r--r--   0 root         (0) root         (0)      170 2022-07-22 19:32:02.000000 satsim-0.15.1/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     3255 2023-02-17 19:27:57.000000 satsim-0.15.1/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)     7121 2023-05-06 01:51:21.000000 satsim-0.15.1/HISTORY.md
+-rw-r--r--   0 root         (0) root         (0)      291 2022-07-22 19:32:02.000000 satsim-0.15.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8746 2023-05-07 18:08:12.613806 satsim-0.15.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-05-04 05:31:05.000000 satsim-0.15.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      608 2022-07-22 19:32:02.000000 satsim-0.15.1/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.593806 satsim-0.15.1/docs/_build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/docs/_build/html/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/docs/_build/html/_static/
+-rw-r--r--   0 root         (0) root         (0)    14813 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/docs/_build/html/_static/css/
+-rw-r--r--   0 root         (0) root         (0)     3229 2023-05-07 18:04:01.000000 satsim-0.15.1/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 root         (0) root         (0)   165742 2023-05-07 18:04:01.000000 satsim-0.15.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   444379 2023-05-07 18:04:01.000000 satsim-0.15.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   165548 2023-05-07 18:04:01.000000 satsim-0.15.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    98024 2023-05-07 18:04:01.000000 satsim-0.15.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    77160 2023-05-07 18:04:01.000000 satsim-0.15.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 root         (0) root         (0)   135235 2023-05-07 18:04:01.000000 satsim-0.15.1/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 root         (0) root         (0)     4472 2023-05-07 18:04:00.000000 satsim-0.15.1/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 root         (0) root         (0)      421 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 root         (0) root         (0)      286 2023-05-07 18:04:00.000000 satsim-0.15.1/docs/_build/html/_static/file.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/docs/_build/html/_static/js/
+-rw-r--r--   0 root         (0) root         (0)      934 2023-05-07 18:04:01.000000 satsim-0.15.1/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 root         (0) root         (0)     4370 2023-05-07 18:04:01.000000 satsim-0.15.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-05-07 18:04:01.000000 satsim-0.15.1/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 root         (0) root         (0)     5023 2023-05-07 18:04:01.000000 satsim-0.15.1/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-07 18:04:00.000000 satsim-0.15.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-07 18:04:00.000000 satsim-0.15.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 root         (0) root         (0)     4846 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 root         (0) root         (0)    18215 2023-05-07 18:04:00.000000 satsim-0.15.1/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-05-07 18:04:00.000000 satsim-0.15.1/docs/_build/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/docs/_build/html/api/
+-rw-r--r--   0 root         (0) root         (0)    10121 2023-05-07 18:08:10.000000 satsim-0.15.1/docs/_build/html/api/satsim.dataset.html
+-rw-r--r--   0 root         (0) root         (0)    10056 2023-05-07 18:08:10.000000 satsim-0.15.1/docs/_build/html/api/satsim.generator.html
+-rw-r--r--   0 root         (0) root         (0)    59162 2023-05-07 18:08:10.000000 satsim-0.15.1/docs/_build/html/api/satsim.generator.obs.html
+-rw-r--r--   0 root         (0) root         (0)   106508 2023-05-07 18:08:10.000000 satsim-0.15.1/docs/_build/html/api/satsim.geometry.html
+-rw-r--r--   0 root         (0) root         (0)   159759 2023-05-07 18:08:09.000000 satsim-0.15.1/docs/_build/html/api/satsim.html
+-rw-r--r--   0 root         (0) root         (0)    91699 2023-05-07 18:08:10.000000 satsim-0.15.1/docs/_build/html/api/satsim.image.html
+-rw-r--r--   0 root         (0) root         (0)    37490 2023-05-07 18:08:10.000000 satsim-0.15.1/docs/_build/html/api/satsim.io.html
+-rw-r--r--   0 root         (0) root         (0)    33473 2023-05-07 18:08:10.000000 satsim-0.15.1/docs/_build/html/api/satsim.math.html
+-rw-r--r--   0 root         (0) root         (0)    14551 2023-05-07 18:08:10.000000 satsim-0.15.1/docs/_build/html/api/satsim.pipeline.html
+-rw-r--r--   0 root         (0) root         (0)    19353 2023-05-07 18:08:10.000000 satsim-0.15.1/docs/_build/html/api/satsim.time.html
+-rw-r--r--   0 root         (0) root         (0)    24867 2023-05-07 18:08:10.000000 satsim-0.15.1/docs/_build/html/api/satsim.util.html
+-rw-r--r--   0 root         (0) root         (0)   404446 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/api/satsim.vecmath.html
+-rw-r--r--   0 root         (0) root         (0)   122688 2023-05-07 18:08:09.000000 satsim-0.15.1/docs/_build/html/api.html
+-rw-r--r--   0 root         (0) root         (0)     5491 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/authors.html
+-rw-r--r--   0 root         (0) root         (0)    13939 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/contributing.html
+-rw-r--r--   0 root         (0) root         (0)    95509 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/genindex.html
+-rw-r--r--   0 root         (0) root         (0)    18474 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/history.html
+-rw-r--r--   0 root         (0) root         (0)     9628 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/index.html
+-rw-r--r--   0 root         (0) root         (0)     7750 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/installation.html
+-rw-r--r--   0 root         (0) root         (0)    17277 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/py-modindex.html
+-rw-r--r--   0 root         (0) root         (0)     4196 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/search.html
+-rw-r--r--   0 root         (0) root         (0)   122864 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/searchindex.js
+-rw-r--r--   0 root         (0) root         (0)    37538 2023-05-07 18:08:11.000000 satsim-0.15.1/docs/_build/html/usage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/docs/api/
+-rw-r--r--   0 root         (0) root         (0)      310 2023-05-07 18:08:00.000000 satsim-0.15.1/docs/api/satsim.dataset.rst
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-07 18:08:00.000000 satsim-0.15.1/docs/api/satsim.generator.obs.rst
+-rw-r--r--   0 root         (0) root         (0)      218 2023-05-07 18:08:00.000000 satsim-0.15.1/docs/api/satsim.generator.rst
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-05-07 18:08:00.000000 satsim-0.15.1/docs/api/satsim.geometry.rst
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-07 18:08:00.000000 satsim-0.15.1/docs/api/satsim.image.rst
+-rw-r--r--   0 root         (0) root         (0)      673 2023-05-07 18:08:00.000000 satsim-0.15.1/docs/api/satsim.io.rst
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-05-07 18:08:00.000000 satsim-0.15.1/docs/api/satsim.math.rst
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-07 18:08:00.000000 satsim-0.15.1/docs/api/satsim.pipeline.rst
+-rw-r--r--   0 root         (0) root         (0)      730 2023-05-07 18:08:00.000000 satsim-0.15.1/docs/api/satsim.rst
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-07 18:08:00.000000 satsim-0.15.1/docs/api/satsim.time.rst
+-rw-r--r--   0 root         (0) root         (0)      572 2023-05-07 18:08:00.000000 satsim-0.15.1/docs/api/satsim.util.rst
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-05-07 18:08:00.000000 satsim-0.15.1/docs/api/satsim.vecmath.rst
+-rw-r--r--   0 root         (0) root         (0)      136 2022-07-22 19:32:02.000000 satsim-0.15.1/docs/api.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2022-07-22 19:32:02.000000 satsim-0.15.1/docs/authors.rst
+-rw-r--r--   0 root         (0) root         (0)     4906 2023-05-06 01:12:33.000000 satsim-0.15.1/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)       33 2022-07-22 19:32:02.000000 satsim-0.15.1/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)       27 2022-07-22 19:32:02.000000 satsim-0.15.1/docs/history.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2022-07-22 19:32:02.000000 satsim-0.15.1/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-02-17 19:27:57.000000 satsim-0.15.1/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      768 2022-07-22 19:32:02.000000 satsim-0.15.1/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)    11419 2022-07-22 19:32:02.000000 satsim-0.15.1/docs/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/satsim/
+-rw-r--r--   0 root         (0) root         (0)      264 2023-05-06 01:12:35.000000 satsim-0.15.1/satsim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/cli.py
+-rw-r--r--   0 root         (0) root         (0)    20530 2023-02-17 19:27:57.000000 satsim-0.15.1/satsim/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/satsim/dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3455 2023-05-04 05:31:05.000000 satsim-0.15.1/satsim/dataset/augment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/satsim/generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/generator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/satsim/generator/obs/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/generator/obs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/generator/obs/breakup.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/generator/obs/cso.py
+-rw-r--r--   0 root         (0) root         (0)     6239 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/generator/obs/geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/generator/obs/io.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/generator/obs/rpo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.613806 satsim-0.15.1/satsim/geometry/
+-rw-r--r--   0 root         (0) root         (0)       66 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/geometry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20912 2023-04-13 09:36:02.000000 satsim-0.15.1/satsim/geometry/astrometric.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-02-17 19:27:57.000000 satsim-0.15.1/satsim/geometry/csvsc.py
+-rw-r--r--   0 root         (0) root         (0)     5268 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/geometry/draw.py
+-rw-r--r--   0 root         (0) root         (0)     3404 2023-02-17 19:27:57.000000 satsim-0.15.1/satsim/geometry/ephemeris.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/geometry/random.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/geometry/sgp4.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-02-17 19:27:57.000000 satsim-0.15.1/satsim/geometry/sprite.py
+-rw-r--r--   0 root         (0) root         (0)    11346 2023-02-17 19:27:57.000000 satsim-0.15.1/satsim/geometry/sstr7.py
+-rw-r--r--   0 root         (0) root         (0)     4340 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/geometry/transform.py
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-02-17 19:27:57.000000 satsim-0.15.1/satsim/geometry/twobody.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-02-17 00:02:42.000000 satsim-0.15.1/satsim/geometry/wcs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.613806 satsim-0.15.1/satsim/image/
+-rw-r--r--   0 root         (0) root         (0)       58 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/image/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9793 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/image/augment.py
+-rw-r--r--   0 root         (0) root         (0)    16625 2023-05-04 05:31:05.000000 satsim-0.15.1/satsim/image/fpa.py
+-rw-r--r--   0 root         (0) root         (0)     5359 2023-02-17 19:27:57.000000 satsim-0.15.1/satsim/image/model.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-05-04 05:31:05.000000 satsim-0.15.1/satsim/image/noise.py
+-rw-r--r--   0 root         (0) root         (0)     6166 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/image/psf.py
+-rw-r--r--   0 root         (0) root         (0)    10401 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/image/render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.613806 satsim-0.15.1/satsim/io/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14550 2023-05-04 05:31:05.000000 satsim-0.15.1/satsim/io/czml.py
+-rw-r--r--   0 root         (0) root         (0)     4319 2023-05-04 05:31:05.000000 satsim-0.15.1/satsim/io/fits.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2023-03-15 01:56:05.000000 satsim-0.15.1/satsim/io/image.py
+-rw-r--r--   0 root         (0) root         (0)     8079 2023-05-06 01:13:41.000000 satsim-0.15.1/satsim/io/satnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.613806 satsim-0.15.1/satsim/math/
+-rw-r--r--   0 root         (0) root         (0)       81 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/math/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-04-05 08:00:38.000000 satsim-0.15.1/satsim/math/angle.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-04-13 09:36:02.000000 satsim-0.15.1/satsim/math/const.py
+-rw-r--r--   0 root         (0) root         (0)      951 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/math/conv.py
+-rw-r--r--   0 root         (0) root         (0)     5551 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/math/fft.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2023-02-17 19:27:57.000000 satsim-0.15.1/satsim/math/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2948 2023-02-17 19:27:57.000000 satsim-0.15.1/satsim/math/random.py
+-rw-r--r--   0 root         (0) root         (0)      590 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/math/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.613806 satsim-0.15.1/satsim/pipeline/
+-rw-r--r--   0 root         (0) root         (0)     1087 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/pipeline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42871 2023-05-04 05:31:05.000000 satsim-0.15.1/satsim/satsim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.613806 satsim-0.15.1/satsim/time/
+-rw-r--r--   0 root         (0) root         (0)     4259 2023-04-13 09:36:02.000000 satsim-0.15.1/satsim/time/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.613806 satsim-0.15.1/satsim/util/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2761 2023-05-04 05:31:05.000000 satsim-0.15.1/satsim/util/system.py
+-rw-r--r--   0 root         (0) root         (0)     3271 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/util/thread.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2022-07-22 19:32:02.000000 satsim-0.15.1/satsim/util/timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.613806 satsim-0.15.1/satsim/vecmath/
+-rw-r--r--   0 root         (0) root         (0)    17668 2023-04-13 09:36:02.000000 satsim-0.15.1/satsim/vecmath/Cartesian2.py
+-rw-r--r--   0 root         (0) root         (0)    20896 2023-04-13 09:36:02.000000 satsim-0.15.1/satsim/vecmath/Cartesian3.py
+-rw-r--r--   0 root         (0) root         (0)    18429 2023-04-13 09:36:02.000000 satsim-0.15.1/satsim/vecmath/Cartesian4.py
+-rw-r--r--   0 root         (0) root         (0)    21727 2023-04-13 09:36:02.000000 satsim-0.15.1/satsim/vecmath/Matrix2.py
+-rw-r--r--   0 root         (0) root         (0)    42567 2023-04-13 09:36:02.000000 satsim-0.15.1/satsim/vecmath/Matrix3.py
+-rw-r--r--   0 root         (0) root         (0)    73877 2023-04-13 09:36:02.000000 satsim-0.15.1/satsim/vecmath/Matrix4.py
+-rw-r--r--   0 root         (0) root         (0)    25251 2023-04-13 09:36:02.000000 satsim-0.15.1/satsim/vecmath/Quaternion.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-04-13 09:36:02.000000 satsim-0.15.1/satsim/vecmath/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.603806 satsim-0.15.1/satsim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8746 2023-05-07 18:08:12.000000 satsim-0.15.1/satsim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3994 2023-05-07 18:08:12.000000 satsim-0.15.1/satsim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 18:08:12.000000 satsim-0.15.1/satsim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-07 18:08:12.000000 satsim-0.15.1/satsim.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 18:08:12.000000 satsim-0.15.1/satsim.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      370 2023-05-07 18:08:12.000000 satsim-0.15.1/satsim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-07 18:08:12.000000 satsim-0.15.1/satsim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2023-05-07 18:08:12.613806 satsim-0.15.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-05-06 01:12:12.000000 satsim-0.15.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 18:08:12.613806 satsim-0.15.1/tests/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-02-20 21:03:12.000000 satsim-0.15.1/tests/README.md
```

### Comparing `satsim-0.15.0/CONTRIBUTING.rst` & `satsim-0.15.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/HISTORY.md` & `satsim-0.15.1/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 History
 =======
 
+0.15.1
+---------------------
+
+* Remove clipping of negative values in ground truth files by default.
+* Fix missing dependencies for ground truth file generation.
+
+
 0.15.0
 ---------------------
 
 * Add support to save ground truth image data to the Annotations directory. Set sim option `save_ground_truth` to `true`.
 * Add support for running on CPU with no GPU acceleration.
 * Add CZML options for sensor visualization and object billboard image.
```

### Comparing `satsim-0.15.0/PKG-INFO` & `satsim-0.15.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsim
-Version: 0.15.0
+Version: 0.15.1
 Summary: Satellite observation and scene simulator.
 Home-page: https://github.com/ssc-ai/satsim
 Author: Alex Cabello
 Author-email: alexander.cabello@algoritics.com
 License: UNKNOWN
 Keywords: satsim
 Platform: UNKNOWN
@@ -37,14 +37,21 @@
 --------
 
 * [History](HISTORY.md)
 
 History
 =======
 
+0.15.1
+---------------------
+
+* Remove clipping of negative values in ground truth files by default.
+* Fix missing dependencies for ground truth file generation.
+
+
 0.15.0
 ---------------------
 
 * Add support to save ground truth image data to the Annotations directory. Set sim option `save_ground_truth` to `true`.
 * Add support for running on CPU with no GPU acceleration.
 * Add CZML options for sensor visualization and object billboard image.
```

### Comparing `satsim-0.15.0/README.md` & `satsim-0.15.1/README.md`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/Makefile` & `satsim-0.15.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/basic.css` & `satsim-0.15.1/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/css/badge_only.css` & `satsim-0.15.1/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `satsim-0.15.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `satsim-0.15.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `satsim-0.15.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `satsim-0.15.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `satsim-0.15.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/css/theme.css` & `satsim-0.15.1/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/doctools.js` & `satsim-0.15.1/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/js/badge_only.js` & `satsim-0.15.1/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `satsim-0.15.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/js/html5shiv.min.js` & `satsim-0.15.1/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/js/theme.js` & `satsim-0.15.1/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/language_data.js` & `satsim-0.15.1/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/pygments.css` & `satsim-0.15.1/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/searchtools.js` & `satsim-0.15.1/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/_static/sphinx_highlight.js` & `satsim-0.15.1/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/_build/html/api/satsim.dataset.html` & `satsim-0.15.1/docs/_build/html/api/satsim.dataset.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.dataset package &mdash; SatSim 0.15.0 documentation</title>
+  <title>satsim.dataset package &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.15.0/docs/_build/html/api/satsim.generator.html` & `satsim-0.15.1/docs/_build/html/api/satsim.generator.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.generator package &mdash; SatSim 0.15.0 documentation</title>
+  <title>satsim.generator package &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.15.0/docs/_build/html/api/satsim.generator.obs.html` & `satsim-0.15.1/docs/_build/html/api/satsim.generator.obs.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.generator.obs package &mdash; SatSim 0.15.0 documentation</title>
+  <title>satsim.generator.obs package &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.15.0/docs/_build/html/api/satsim.geometry.html` & `satsim-0.15.1/docs/_build/html/api/satsim.geometry.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.geometry package &mdash; SatSim 0.15.0 documentation</title>
+  <title>satsim.geometry package &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.15.0/docs/_build/html/api/satsim.html` & `satsim-0.15.1/docs/_build/html/api/satsim.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim package &mdash; SatSim 0.15.0 documentation</title>
+  <title>satsim package &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.15.0/docs/_build/html/api/satsim.image.html` & `satsim-0.15.1/docs/_build/html/api/satsim.image.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.image package &mdash; SatSim 0.15.0 documentation</title>
+  <title>satsim.image package &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.15.0/docs/_build/html/api/satsim.io.html` & `satsim-0.15.1/docs/_build/html/api/satsim.io.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.io package &mdash; SatSim 0.15.0 documentation</title>
+  <title>satsim.io package &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -188,15 +188,15 @@
 </dd></dl>
 
 </section>
 <section id="module-satsim.io.fits">
 <span id="satsim-io-fits-module"></span><h2>satsim.io.fits module<a class="headerlink" href="#module-satsim.io.fits" title="Permalink to this heading"></a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="satsim.io.fits.save">
-<span class="sig-prename descclassname"><span class="pre">satsim.io.fits.</span></span><span class="sig-name descname"><span class="pre">save</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">filename</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fpa</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exposure_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dt_start</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">5,</span> <span class="pre">4,</span> <span class="pre">5,</span> <span class="pre">43,</span> <span class="pre">45,</span> <span class="pre">661952)</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">header</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">{}</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">overwrite</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'uint16'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.fits.save" title="Permalink to this definition"></a></dt>
+<span class="sig-prename descclassname"><span class="pre">satsim.io.fits.</span></span><span class="sig-name descname"><span class="pre">save</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">filename</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fpa</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exposure_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dt_start</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">5,</span> <span class="pre">7,</span> <span class="pre">18,</span> <span class="pre">8,</span> <span class="pre">3,</span> <span class="pre">128576)</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">header</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">{}</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">overwrite</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'uint16'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.fits.save" title="Permalink to this definition"></a></dt>
 <dd><p>Save a SatNet compatible FITS file.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>filename</strong> – <cite>string</cite>, the FITS filename.</p></li>
 <li><p><strong>fpa</strong> – <cite>np.array</cite>, input image as a 2D numpy array.</p></li>
 <li><p><strong>exposure_time</strong> – <cite>float</cite>, exposure time for header.</p></li>
@@ -302,15 +302,15 @@
 <dd class="field-even"><p>A <cite>dict</cite>, the data object for <cite>set_frame_annotation</cite></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="satsim.io.satnet.write_frame">
-<span class="sig-prename descclassname"><span class="pre">satsim.io.satnet.</span></span><span class="sig-name descname"><span class="pre">write_frame</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">dir_name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sat_name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fpa_digital</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">meta_data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">frame_num</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exposure_time</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time_stamp</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ssp</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">show_obs_boxes</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">save_pickle</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'uint16'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">save_jpeg</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ground_truth</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ground_truth_min</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.satnet.write_frame" title="Permalink to this definition"></a></dt>
+<span class="sig-prename descclassname"><span class="pre">satsim.io.satnet.</span></span><span class="sig-name descname"><span class="pre">write_frame</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">dir_name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sat_name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fpa_digital</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">meta_data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">frame_num</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exposure_time</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time_stamp</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ssp</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">show_obs_boxes</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">save_pickle</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'uint16'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">save_jpeg</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ground_truth</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ground_truth_min</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.satnet.write_frame" title="Permalink to this definition"></a></dt>
 <dd><p>Write image and annotation files compatible with SatNet. In addition,
 writes annotated images and SatSim configuration file for reference.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>dir_name</strong> – <cite>string</cite>, directory to save files to</p></li>
 <li><p><strong>sat_name</strong> – <cite>string</cite>, satellite name</p></li>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -109,15 +109,15 @@
                 * obs_cache âlist, list of SatSim Skyfield objects.
                 * filename âstr, if not None, save czml output. default=None
         Returns:
             Adict, the CZML output
 
 ***** satsim.io.fits moduleï *****
   satsim.io.fits.save(filename, fpa, exposure_time=0,
-  dt_start=datetime.datetime(2023, 5, 4, 5, 43, 45, 661952), header={},
+  dt_start=datetime.datetime(2023, 5, 7, 18, 8, 3, 128576), header={},
   overwrite=False, dtype='uint16', astrometrics=None)ï
       Save a SatNet compatible FITS file.
         Parameters:
                 * filename âstring, the FITS filename.
                 * fpa ânp.array, input image as a 2D numpy array.
                 * exposure_time âfloat, exposure time for header.
                 * dt_start âdatetime, datetime of start of exposure.
@@ -185,15 +185,15 @@
                 * filter_ob âboolean, bounds min and max and remove out of
                   bounds
         Returns:
             Adict, the data object forset_frame_annotation
   satsim.io.satnet.write_frame(dir_name, sat_name, fpa_digital, meta_data,
   frame_num, exposure_time, time_stamp, ssp, show_obs_boxes=True,
   astrometrics=None, save_pickle=False, dtype='uint16', save_jpeg=True,
-  ground_truth=None, ground_truth_min=0)ï
+  ground_truth=None, ground_truth_min=None)ï
       Write image and annotation files compatible with SatNet. In addition,
       writes annotated images and SatSim configuration file for reference.
         Parameters:
                 * dir_name âstring, directory to save files to
                 * sat_name âstring, satellite name
                 * fpa_digital âarray, image as a numpy array
                 * meta_data âdict, annotation data generated
```

### Comparing `satsim-0.15.0/docs/_build/html/api/satsim.math.html` & `satsim-0.15.1/docs/_build/html/api/satsim.math.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.math package &mdash; SatSim 0.15.0 documentation</title>
+  <title>satsim.math package &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.15.0/docs/_build/html/api/satsim.pipeline.html` & `satsim-0.15.1/docs/_build/html/api/satsim.pipeline.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.pipeline package &mdash; SatSim 0.15.0 documentation</title>
+  <title>satsim.pipeline package &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.15.0/docs/_build/html/api/satsim.time.html` & `satsim-0.15.1/docs/_build/html/api/satsim.time.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.time package &mdash; SatSim 0.15.0 documentation</title>
+  <title>satsim.time package &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.15.0/docs/_build/html/api/satsim.util.html` & `satsim-0.15.1/docs/_build/html/api/satsim.util.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.util package &mdash; SatSim 0.15.0 documentation</title>
+  <title>satsim.util package &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.15.0/docs/_build/html/api/satsim.vecmath.html` & `satsim-0.15.1/docs/_build/html/api/satsim.vecmath.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.vecmath package &mdash; SatSim 0.15.0 documentation</title>
+  <title>satsim.vecmath package &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.15.0/docs/_build/html/api.html` & `satsim-0.15.1/docs/_build/html/api.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>API Documentation &mdash; SatSim 0.15.0 documentation</title>
+  <title>API Documentation &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.15.0/docs/_build/html/authors.html` & `satsim-0.15.1/docs/_build/html/authors.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Credits &mdash; SatSim 0.15.0 documentation</title>
+  <title>Credits &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
```

### Comparing `satsim-0.15.0/docs/_build/html/contributing.html` & `satsim-0.15.1/docs/_build/html/contributing.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Contributing &mdash; SatSim 0.15.0 documentation</title>
+  <title>Contributing &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
           o Getting_Started_for_Developers
           o Merge_Request_Guidelines
```

### Comparing `satsim-0.15.0/docs/_build/html/genindex.html` & `satsim-0.15.1/docs/_build/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; SatSim 0.15.0 documentation</title>
+  <title>Index &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -26,15 +26,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
```

### Comparing `satsim-0.15.0/docs/_build/html/history.html` & `satsim-0.15.1/docs/_build/html/history.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>History &mdash; SatSim 0.15.0 documentation</title>
+  <title>History &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -46,38 +46,39 @@
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
 <li class="toctree-l1"><a class="reference internal" href="contributing.html">Contributing</a></li>
 <li class="toctree-l1"><a class="reference internal" href="api.html">API Documentation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="authors.html">Credits</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">History</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#id1">0.15.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id2">0.14.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id3">0.13.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id4">0.13.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id5">0.12.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id6">0.11.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id7">0.10.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id8">0.9.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id9">0.9.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id10">0.8.3</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id11">0.8.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id12">0.8.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id13">0.8.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id14">0.7.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id15">0.7.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id16">0.7.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id17">0.6.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id18">0.6.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id19">0.5.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id20">0.4.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id21">0.3.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id22">0.2.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id23">0.1.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id24">0.1.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id1">0.15.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id2">0.15.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id3">0.14.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id4">0.13.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id5">0.13.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id6">0.12.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id7">0.11.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id8">0.10.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id9">0.9.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id10">0.9.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id11">0.8.3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id12">0.8.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id13">0.8.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id14">0.8.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id15">0.7.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id16">0.7.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id17">0.7.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id18">0.6.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id19">0.6.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id20">0.5.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id21">0.4.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id22">0.3.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id23">0.2.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id24">0.1.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id25">0.1.0</a></li>
 </ul>
 </li>
 </ul>
 
         </div>
       </div>
     </nav>
@@ -101,228 +102,235 @@
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="history">
 <h1>History<a class="headerlink" href="#history" title="Permalink to this heading"></a></h1>
 <section id="id1">
-<h2>0.15.0<a class="headerlink" href="#id1" title="Permalink to this heading"></a></h2>
+<h2>0.15.1<a class="headerlink" href="#id1" title="Permalink to this heading"></a></h2>
+<ul class="simple">
+<li><p>Remove clipping of negative values in ground truth files by default.</p></li>
+<li><p>Fix missing dependencies for ground truth file generation.</p></li>
+</ul>
+</section>
+<section id="id2">
+<h2>0.15.0<a class="headerlink" href="#id2" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support to save ground truth image data to the Annotations directory. Set sim option <cite>save_ground_truth</cite> to <cite>true</cite>.</p></li>
 <li><p>Add support for running on CPU with no GPU acceleration.</p></li>
 <li><p>Add CZML options for sensor visualization and object billboard image.</p></li>
 </ul>
 </section>
-<section id="id2">
-<h2>0.14.0<a class="headerlink" href="#id2" title="Permalink to this heading"></a></h2>
+<section id="id3">
+<h2>0.14.0<a class="headerlink" href="#id3" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add vector math library.</p></li>
 <li><p>Add CZML output for sensor visualization.</p></li>
 <li><p>Fix objects not updating properly when image renderer is off.</p></li>
 </ul>
 </section>
-<section id="id3">
-<h2>0.13.1<a class="headerlink" href="#id3" title="Permalink to this heading"></a></h2>
+<section id="id4">
+<h2>0.13.1<a class="headerlink" href="#id4" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add argument to set folder name in <cite>gen_multi</cite>.</p></li>
 <li><p>Add environment variable, <cite>SATSIM_SKYFIELD_LOAD_DIR</cite>, to specify location of Skyfield ephemeris files.</p></li>
 <li><p>Fix incorrect CZML output when image renderer is off.</p></li>
 </ul>
 </section>
-<section id="id4">
-<h2>0.13.0<a class="headerlink" href="#id4" title="Permalink to this heading"></a></h2>
+<section id="id5">
+<h2>0.13.0<a class="headerlink" href="#id5" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add ephemeris objects that are propagated with the Lagrange interpolator.</p></li>
 <li><p>Add Cesium CZML output. Set sim option <cite>save_czml</cite> to <cite>false</cite> to disable.</p></li>
 <li><p>Add CSV text file star catalog loader. This feature is useful for small catalogs such as Hipparcos and simulating wide FOV sensors.</p></li>
 <li><p>Add multiplier and clipping for radial cosine.</p></li>
 <li><p>Add option to skip image rendering. Set sim option <cite>mode</cite> to <cite>none</cite> to bypass image rendering.</p></li>
 <li><p>Update interfaces for newest version of Skyfield, Poliastro, POPPY, and AstroPy.</p></li>
 <li><p>Fix star renderer issue removing stars in field of view for non-square arrays.</p></li>
 </ul>
 </section>
-<section id="id5">
-<h2>0.12.0<a class="headerlink" href="#id5" title="Permalink to this heading"></a></h2>
+<section id="id6">
+<h2>0.12.0<a class="headerlink" href="#id6" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add augmentation of SatNet <cite>tf.data.Dataset</cite>. This feature allows injecting synthetic targets into real data during training.</p></li>
 <li><p>Add FFT convolution to <cite>add_patch</cite> sprite render and <cite>scatter_shift</cite> image augmenter for speed improvement.</p></li>
 <li><p>Add cache last PSF FFT to <cite>fftconv2p</cite> for speed improvement for static PSFs.</p></li>
 <li><p>Add two-body state vector as a trackable target.</p></li>
 <li><p>Add moon and sun model and misc methods to calculate phase angle and target brightness.</p></li>
 </ul>
 </section>
-<section id="id6">
-<h2>0.11.0<a class="headerlink" href="#id6" title="Permalink to this heading"></a></h2>
+<section id="id7">
+<h2>0.11.0<a class="headerlink" href="#id7" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support to render star motion with FFT. Set sim option <cite>star_render_mode</cite> to <cite>fft</cite>.</p></li>
 <li><p>Add option to sample photon noise multiple times. Set sim option <cite>num_shot_noise_samples</cite> to integer number.</p></li>
 <li><p>Add support to render a satellite as a sprite. Set <cite>model</cite> option in obs.</p></li>
 <li><p>Add support to load and augment sprite model with <cite>$pipeline</cite> operator.</p></li>
 <li><p>Add cropped POPPY PSF generation.</p></li>
 <li><p>Fix GreatCircle propagator tracking offset.</p></li>
 <li><p>Fix runtime exception when site and track_mode are not defined.</p></li>
 <li><p>Add TensorFlow 2.6 and update TensorFlow 2.2 and 2.4 Docker build file.</p></li>
 </ul>
 </section>
-<section id="id7">
-<h2>0.10.0<a class="headerlink" href="#id7" title="Permalink to this heading"></a></h2>
+<section id="id8">
+<h2>0.10.0<a class="headerlink" href="#id8" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support for piecewise rendering. Set sim option <cite>render_size</cite> to enable. For example, [256, 256].</p></li>
 <li><p>Add <cite>fixed</cite> tracking mode with mount azimuth and elevation.</p></li>
 <li><p>Add great circle propagator for targets.</p></li>
 <li><p>Add in-memory image generation. See generator function <cite>image_generator</cite>.</p></li>
 <li><p>Fix missing stars when FOV crosses zero degree RA.</p></li>
 <li><p>Add curved targets using bezier curve raster. Enabled by default. Set sim option <cite>num_target_samples</cite> to 2 to enable linear raster.</p></li>
 <li><p>Add LRU cache to star catalog reader.</p></li>
 <li><p>Add option to turn off SNR calculation. Set sim option <cite>calculate_snr</cite> to false will render targets and stars together.</p></li>
 <li><p>Handle unstable SGP4 TLEs.</p></li>
 <li><p>Add TensorFlow 2.4 Docker build file.</p></li>
 <li><p>Add debug output for pristine images of targets and stars.</p></li>
 </ul>
 </section>
-<section id="id8">
-<h2>0.9.1<a class="headerlink" href="#id8" title="Permalink to this heading"></a></h2>
+<section id="id9">
+<h2>0.9.1<a class="headerlink" href="#id9" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Calculate POPPY input wavefront resolution to avoid PSF aliasing.</p></li>
 <li><p>Add support for additional FITS image data types (<cite>int16</cite>, <cite>uint16</cite>, <cite>int32</cite>, <cite>uint32</cite>, <cite>float32</cite>).</p></li>
 <li><p>Add batch processing to <cite>transform_and_add_counts</cite> to support batch processing of stars.</p></li>
 <li><p>Add <cite>auto</cite> option to calculate temporal oversample factor based on star velocities.</p></li>
 <li><p>Add option to turn off serializing config data to pickle file (<cite>save_pickle</cite>).</p></li>
 <li><p>Add option to turn off png movie output (<cite>save_movie</cite>).</p></li>
 <li><p>Add <cite>crop_and_resize</cite> and <cite>flip</cite> image augmentation.</p></li>
 <li><p>Set pixels with values beyond the pixel data type’s capacity to the maximum value for that data type.</p></li>
 <li><p>Add <cite>lognormal</cite> function to generate a distribution with a true target mean.</p></li>
 <li><p>Fix issue with sidereal track.</p></li>
 <li><p>Fix issue with fragment velocity not being randomly sampled.</p></li>
 </ul>
 </section>
-<section id="id9">
-<h2>0.9.0<a class="headerlink" href="#id9" title="Permalink to this heading"></a></h2>
+<section id="id10">
+<h2>0.9.0<a class="headerlink" href="#id10" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add Physical Optics Propagation in Python (POPPY) PSF generation.</p></li>
 <li><p>Add PSF augmentation with <cite>$pipeline</cite> replacement key.</p></li>
 <li><p>Add <cite>$function</cite> and <cite>$compound</cite> replacement key.</p></li>
 <li><p>Add ability to generate stray light from a <cite>$function</cite> replacement key.</p></li>
 <li><p>Add built-in 2D polynomial image generator for stray light, <cite>polygrid2d</cite>.</p></li>
 <li><p>Add built-in cosine fourth image generator for irradiance falloff, <cite>radial_cos2d</cite>.</p></li>
 <li><p>Add built-in sine wave image generator for fix pattern noise, <cite>sin2d</cite>.</p></li>
 <li><p>Add built-in image generator from AstroPy model, <cite>astropy_model2d</cite>.</p></li>
 <li><p>Add built-in image augmentation, <cite>scatter_shift</cite> and <cite>scatter_shift_polar</cite>.</p></li>
 <li><p>Add <cite>$cache</cite> replacement key (caching works for PSF and <cite>$function</cite>).</p></li>
 </ul>
 </section>
-<section id="id10">
-<h2>0.8.3<a class="headerlink" href="#id10" title="Permalink to this heading"></a></h2>
+<section id="id11">
+<h2>0.8.3<a class="headerlink" href="#id11" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Fix new Skyfield incompatibility.</p></li>
 </ul>
 </section>
-<section id="id11">
-<h2>0.8.2<a class="headerlink" href="#id11" title="Permalink to this heading"></a></h2>
+<section id="id12">
+<h2>0.8.2<a class="headerlink" href="#id12" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Prefix replacement keys with <cite>$</cite> in SatSim configuration file.</p></li>
 <li><p>Add option to scale collision fragments by cosine of the exit angle.</p></li>
 </ul>
 </section>
-<section id="id12">
-<h2>0.8.1<a class="headerlink" href="#id12" title="Permalink to this heading"></a></h2>
+<section id="id13">
+<h2>0.8.1<a class="headerlink" href="#id13" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add astrometric metadata into FITS header</p></li>
 <li><p>Refactor WCS library</p></li>
 <li><p>Add option to flip images about x or y axis</p></li>
 <li><p>Add option to refresh stars for each frame</p></li>
 <li><p>Add RPO from TLE generator</p></li>
 </ul>
 </section>
-<section id="id13">
-<h2>0.8.0<a class="headerlink" href="#id13" title="Permalink to this heading"></a></h2>
+<section id="id14">
+<h2>0.8.0<a class="headerlink" href="#id14" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add two body propagator</p></li>
 <li><p>Add object <cite>create</cite>, <cite>delete</cite>, and <cite>update</cite> events</p></li>
 <li><p>Add collision generator</p></li>
 <li><p>Add breakup generator</p></li>
 <li><p>Add <cite>ref</cite> keyword to configuration</p></li>
 <li><p>Add <cite>key</cite> keyword to <cite>import</cite> configuration</p></li>
 <li><p>Refactor astrometric library</p></li>
 </ul>
 </section>
-<section id="id14">
-<h2>0.7.2<a class="headerlink" href="#id14" title="Permalink to this heading"></a></h2>
+<section id="id15">
+<h2>0.7.2<a class="headerlink" href="#id15" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add option to specify star and obs velocity in polar coordinates</p></li>
 </ul>
 </section>
-<section id="id15">
-<h2>0.7.1<a class="headerlink" href="#id15" title="Permalink to this heading"></a></h2>
+<section id="id16">
+<h2>0.7.1<a class="headerlink" href="#id16" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add option to turn off shot noise: <cite>sim.enable_shot_noise: true</cite></p></li>
 <li><p>Add option to turn off annotation boxes in image: <cite>sim.show_obs_boxes: true</cite></p></li>
 <li><p>Add option to specify velocity in arcseconds: <cite>sim.velocity_units: arcsec</cite></p></li>
 <li><p>Fix PNG output threading issue</p></li>
 </ul>
 </section>
-<section id="id16">
-<h2>0.7.0<a class="headerlink" href="#id16" title="Permalink to this heading"></a></h2>
+<section id="id17">
+<h2>0.7.0<a class="headerlink" href="#id17" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add function pipelines to support variable target brightness</p></li>
 </ul>
 </section>
-<section id="id17">
-<h2>0.6.1<a class="headerlink" href="#id17" title="Permalink to this heading"></a></h2>
+<section id="id18">
+<h2>0.6.1<a class="headerlink" href="#id18" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Fix built-in generators not included in distribution</p></li>
 <li><p>Add dockerfile</p></li>
 </ul>
 </section>
-<section id="id18">
-<h2>0.6.0<a class="headerlink" href="#id18" title="Permalink to this heading"></a></h2>
+<section id="id19">
+<h2>0.6.0<a class="headerlink" href="#id19" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add configuration import.</p></li>
 <li><p>Add configuration generator functions.</p></li>
 <li><p>Add built-in generator for breakups.</p></li>
 <li><p>Add built-in generator for CSOs.</p></li>
 <li><p>Add built-in generator for loading TLE files.</p></li>
 </ul>
 </section>
-<section id="id19">
-<h2>0.5.0<a class="headerlink" href="#id19" title="Permalink to this heading"></a></h2>
+<section id="id20">
+<h2>0.5.0<a class="headerlink" href="#id20" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Runtime optimization.</p></li>
 <li><p>Add parallel processing and multi-gpu utilization.</p></li>
 <li><p>Add option to limit gpu memory usage.</p></li>
 </ul>
 </section>
-<section id="id20">
-<h2>0.4.0<a class="headerlink" href="#id20" title="Permalink to this heading"></a></h2>
+<section id="id21">
+<h2>0.4.0<a class="headerlink" href="#id21" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add signal to noise calculation for target pixels.</p></li>
 </ul>
 </section>
-<section id="id21">
-<h2>0.3.0<a class="headerlink" href="#id21" title="Permalink to this heading"></a></h2>
+<section id="id22">
+<h2>0.3.0<a class="headerlink" href="#id22" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support for two line element set SGP4 satellite propagator.</p></li>
 <li><p>Add support for rate and sidereal track from topocentric site.</p></li>
 </ul>
 </section>
-<section id="id22">
-<h2>0.2.0<a class="headerlink" href="#id22" title="Permalink to this heading"></a></h2>
+<section id="id23">
+<h2>0.2.0<a class="headerlink" href="#id23" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support for SSTR7 star catalog.</p></li>
 </ul>
 </section>
-<section id="id23">
-<h2>0.1.1<a class="headerlink" href="#id23" title="Permalink to this heading"></a></h2>
+<section id="id24">
+<h2>0.1.1<a class="headerlink" href="#id24" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add target position to annotation file.</p></li>
 <li><p>Updates to run GitLab CI.</p></li>
 </ul>
 </section>
-<section id="id24">
-<h2>0.1.0<a class="headerlink" href="#id24" title="Permalink to this heading"></a></h2>
+<section id="id25">
+<h2>0.1.0<a class="headerlink" href="#id25" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>First release.</p></li>
 </ul>
 </section>
 </section>
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
     * History
+          o 0.15.1
           o 0.15.0
           o 0.14.0
           o 0.13.1
           o 0.13.0
           o 0.12.0
           o 0.11.0
           o 0.10.0
@@ -39,14 +40,18 @@
           o 0.1.1
           o 0.1.0
    SatSim
     * History
     * View_page_source
 ===============================================================================
 ****** Historyï ******
+***** 0.15.1ï *****
+    * Remove clipping of negative values in ground truth files by default.
+    * Fix missing dependencies for ground truth file generation.
+
 ***** 0.15.0ï *****
     * Add support to save ground truth image data to the Annotations directory.
       Set sim optionsave_ground_truthtotrue.
     * Add support for running on CPU with no GPU acceleration.
     * Add CZML options for sensor visualization and object billboard image.
 
 ***** 0.14.0ï *****
```

### Comparing `satsim-0.15.0/docs/_build/html/index.html` & `satsim-0.15.1/docs/_build/html/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Documentation for SatSim &mdash; SatSim 0.15.0 documentation</title>
+  <title>Documentation for SatSim &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -106,38 +106,39 @@
 </li>
 <li class="toctree-l1"><a class="reference internal" href="authors.html">Credits</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="authors.html#development-lead">Development Lead</a></li>
 <li class="toctree-l2"><a class="reference internal" href="authors.html#contributors">Contributors</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="history.html">History</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id1">0.15.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id2">0.14.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id3">0.13.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id4">0.13.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id5">0.12.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id6">0.11.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id7">0.10.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id8">0.9.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id9">0.9.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id10">0.8.3</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id11">0.8.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id12">0.8.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id13">0.8.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id14">0.7.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id15">0.7.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id16">0.7.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id17">0.6.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id18">0.6.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id19">0.5.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id20">0.4.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id21">0.3.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id22">0.2.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id23">0.1.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id24">0.1.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id1">0.15.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id2">0.15.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id3">0.14.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id4">0.13.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id5">0.13.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id6">0.12.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id7">0.11.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id8">0.10.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id9">0.9.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id10">0.9.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id11">0.8.3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id12">0.8.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id13">0.8.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id14">0.8.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id15">0.7.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id16">0.7.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id17">0.7.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id18">0.6.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id19">0.6.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id20">0.5.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id21">0.4.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id22">0.3.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id23">0.2.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id24">0.1.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id25">0.1.0</a></li>
 </ul>
 </li>
 </ul>
 </div>
 </section>
 <section id="indices-and-tables">
 <h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading"></a></h1>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
@@ -35,14 +35,15 @@
           o Other_Ways_of_Contributing
     * API_Documentation
           o satsim_package
     * Credits
           o Development_Lead
           o Contributors
     * History
+          o 0.15.1
           o 0.15.0
           o 0.14.0
           o 0.13.1
           o 0.13.0
           o 0.12.0
           o 0.11.0
           o 0.10.0
```

### Comparing `satsim-0.15.0/docs/_build/html/installation.html` & `satsim-0.15.1/docs/_build/html/installation.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Installation &mdash; SatSim 0.15.0 documentation</title>
+  <title>Installation &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
           o Stable_Release
           o From_Sources
     * Usage
     * Contributing
```

### Comparing `satsim-0.15.0/docs/_build/html/py-modindex.html` & `satsim-0.15.1/docs/_build/html/py-modindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; SatSim 0.15.0 documentation</title>
+  <title>Python Module Index &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
```

### Comparing `satsim-0.15.0/docs/_build/html/search.html` & `satsim-0.15.1/docs/_build/html/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; SatSim 0.15.0 documentation</title>
+  <title>Search &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
```

### Comparing `satsim-0.15.0/docs/_build/html/searchindex.js` & `satsim-0.15.1/docs/_build/html/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -462,20 +462,20 @@
         "x": [1, 4, 5, 6, 8, 9, 12, 15],
         "between": [1, 4, 5, 6, 8, 10, 12, 18],
         "If": [1, 6, 7, 8, 11, 12, 14, 17, 18],
         "choic": 1,
         "chosen": 1,
         "1": [1, 4, 5, 6, 8, 9, 11, 12, 16, 18],
         "2": [1, 2, 4, 5, 6, 7, 8, 11, 12, 16, 18],
-        "4": [1, 6, 7, 8, 12, 16, 18],
-        "8": [1, 4, 6, 12, 16, 18],
+        "4": [1, 6, 8, 12, 16, 18],
+        "8": [1, 4, 6, 7, 12, 16, 18],
         "length": [1, 4, 5, 6, 7, 8, 12, 18],
         "randint": [1, 4, 18],
         "e": [1, 5, 6, 7, 8],
-        "7": [1, 4, 12, 16, 18],
+        "7": [1, 4, 7, 12, 16, 18],
         "number": [1, 2, 4, 5, 6, 7, 8, 10, 12, 15, 18],
         "disk": 1,
         "subsequ": 1,
         "call": [1, 8, 11, 12, 18],
         "output_dir": [1, 18],
         "write": [1, 7],
         "arrai": [1, 4, 5, 6, 7, 8, 10, 11, 12, 15, 18],
@@ -707,15 +707,15 @@
         "95": 4,
         "02": 4,
         "t": [4, 5, 6, 9, 10, 12, 17, 18],
         "eman": [4, 18],
         "point": [4, 5, 6, 7, 8, 12, 18],
         "elaps": [4, 5, 11],
         "epoch": [4, 5, 6],
-        "3": [4, 5, 6, 8, 12, 14, 16, 18],
+        "3": [4, 5, 6, 7, 8, 12, 14, 16, 18],
         "direct": [4, 5, 6, 12, 18],
         "30": [4, 5, 8, 18],
         "about": [4, 5, 6, 12, 14, 15],
         "mean": [4, 6, 8, 15],
         "express": [4, 12],
         "min": [4, 5, 7, 8, 12],
         "max": [4, 5, 6, 7, 8, 12],
@@ -1294,17 +1294,16 @@
         "document": 7,
         "obs_cach": 7,
         "scenario": 7,
         "exposure_tim": 7,
         "dt_start": 7,
         "datetim": 7,
         "2023": 7,
-        "43": 7,
-        "45": 7,
-        "661952": 7,
+        "18": [7, 18],
+        "128576": 7,
         "header": [7, 15],
         "overwrit": 7,
         "np": 7,
         "exposur": [7, 18],
         "placehold": [7, 18],
         "implement": [7, 10, 12, 14],
         "exist": [7, 12],
@@ -1558,15 +1557,15 @@
         "third": 12,
         "exponenti": 12,
         "accur": 12,
         "10e": 12,
         "s0": 12,
         "s1": 12,
         "pitch": 12,
-        "neg": 12,
+        "neg": [12, 15],
         "logarithm": 12,
         "alex": 13,
         "cabello": 13,
         "alexand": 13,
         "algorit": 13,
         "com": [13, 14, 17],
         "yet": 13,
@@ -1658,14 +1657,16 @@
         "propos": 14,
         "explain": 14,
         "keep": 14,
         "scope": 14,
         "narrow": 14,
         "easier": 14,
         "truth": 15,
+        "miss": 15,
+        "depend": 15,
         "save_ground_truth": 15,
         "billboard": 15,
         "librari": 15,
         "properli": 15,
         "satsim_skyfield_load_dir": 15,
         "incorrect": 15,
         "csv": 15,
@@ -1684,15 +1685,14 @@
         "misc": [15, 18],
         "phase": 15,
         "track_mod": 15,
         "piecewis": 15,
         "render_s": 15,
         "256": [15, 18],
         "mount": 15,
-        "miss": 15,
         "raster": 15,
         "num_target_sampl": 15,
         "lru": 15,
         "reader": 15,
         "turn": 15,
         "calculate_snr": 15,
         "handl": 15,
@@ -1789,15 +1789,14 @@
         "100000": 18,
         "1500": 18,
         "ensquar": 18,
         "gap": 18,
         "num_fram": 18,
         "galact": 18,
         "19": 18,
-        "18": 18,
         "019444": 18,
         "0055556": 18,
         "016667": 18,
         "036111": 18,
         "038889": 18,
         "097222": 18,
         "66944": 18,
@@ -2611,17 +2610,17 @@
         "bug": 14,
         "write": 14,
         "submit": 14,
         "feedback": 14,
         "histori": 15,
         "0": 15,
         "15": 15,
+        "1": 15,
         "14": 15,
         "13": 15,
-        "1": 15,
         "12": 15,
         "11": 15,
         "10": 15,
         "9": 15,
         "8": 15,
         "3": 15,
         "2": 15,
@@ -2889,86 +2888,89 @@
         ],
         "Submit Feedback": [
             [14, "submit-feedback"]
         ],
         "History": [
             [15, "history"]
         ],
-        "0.15.0": [
+        "0.15.1": [
             [15, "id1"]
         ],
-        "0.14.0": [
+        "0.15.0": [
             [15, "id2"]
         ],
-        "0.13.1": [
+        "0.14.0": [
             [15, "id3"]
         ],
-        "0.13.0": [
+        "0.13.1": [
             [15, "id4"]
         ],
-        "0.12.0": [
+        "0.13.0": [
             [15, "id5"]
         ],
-        "0.11.0": [
+        "0.12.0": [
             [15, "id6"]
         ],
-        "0.10.0": [
+        "0.11.0": [
             [15, "id7"]
         ],
-        "0.9.1": [
+        "0.10.0": [
             [15, "id8"]
         ],
-        "0.9.0": [
+        "0.9.1": [
             [15, "id9"]
         ],
-        "0.8.3": [
+        "0.9.0": [
             [15, "id10"]
         ],
-        "0.8.2": [
+        "0.8.3": [
             [15, "id11"]
         ],
-        "0.8.1": [
+        "0.8.2": [
             [15, "id12"]
         ],
-        "0.8.0": [
+        "0.8.1": [
             [15, "id13"]
         ],
-        "0.7.2": [
+        "0.8.0": [
             [15, "id14"]
         ],
-        "0.7.1": [
+        "0.7.2": [
             [15, "id15"]
         ],
-        "0.7.0": [
+        "0.7.1": [
             [15, "id16"]
         ],
-        "0.6.1": [
+        "0.7.0": [
             [15, "id17"]
         ],
-        "0.6.0": [
+        "0.6.1": [
             [15, "id18"]
         ],
-        "0.5.0": [
+        "0.6.0": [
             [15, "id19"]
         ],
-        "0.4.0": [
+        "0.5.0": [
             [15, "id20"]
         ],
-        "0.3.0": [
+        "0.4.0": [
             [15, "id21"]
         ],
-        "0.2.0": [
+        "0.3.0": [
             [15, "id22"]
         ],
-        "0.1.1": [
+        "0.2.0": [
             [15, "id23"]
         ],
-        "0.1.0": [
+        "0.1.1": [
             [15, "id24"]
         ],
+        "0.1.0": [
+            [15, "id25"]
+        ],
         "Documentation for SatSim": [
             [16, "documentation-for-satsim"]
         ],
         "Contents:": [
             [16, null]
         ],
         "Indices and tables": [
```

### Comparing `satsim-0.15.0/docs/_build/html/usage.html` & `satsim-0.15.1/docs/_build/html/usage.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Usage &mdash; SatSim 0.15.0 documentation</title>
+  <title>Usage &mdash; SatSim 0.15.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.15.0
+                0.15.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.15.0
+0.15.1
 [q                   ]
 Contents:
     * Installation
     * Usage
           o Python_Module
           o Command_Line_Interface
           o Parameters_and_Configuration
```

### Comparing `satsim-0.15.0/docs/api/satsim.generator.obs.rst` & `satsim-0.15.1/docs/api/satsim.generator.obs.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/api/satsim.geometry.rst` & `satsim-0.15.1/docs/api/satsim.geometry.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/api/satsim.image.rst` & `satsim-0.15.1/docs/api/satsim.image.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/api/satsim.io.rst` & `satsim-0.15.1/docs/api/satsim.io.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/api/satsim.math.rst` & `satsim-0.15.1/docs/api/satsim.math.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/api/satsim.rst` & `satsim-0.15.1/docs/api/satsim.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/api/satsim.util.rst` & `satsim-0.15.1/docs/api/satsim.util.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/api/satsim.vecmath.rst` & `satsim-0.15.1/docs/api/satsim.vecmath.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/conf.py` & `satsim-0.15.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,17 +54,17 @@
 author = u"Alex Cabello"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = '0.15.0'
+version = '0.15.1'
 # The full version, including alpha/beta/rc tags.
-release = '0.15.0'
+release = '0.15.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `satsim-0.15.0/docs/installation.rst` & `satsim-0.15.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/make.bat` & `satsim-0.15.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/docs/usage.rst` & `satsim-0.15.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/cli.py` & `satsim-0.15.1/satsim/cli.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/config.py` & `satsim-0.15.1/satsim/config.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/dataset/augment.py` & `satsim-0.15.1/satsim/dataset/augment.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/generator/obs/breakup.py` & `satsim-0.15.1/satsim/generator/obs/breakup.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/generator/obs/cso.py` & `satsim-0.15.1/satsim/generator/obs/cso.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/generator/obs/geometry.py` & `satsim-0.15.1/satsim/generator/obs/geometry.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/generator/obs/io.py` & `satsim-0.15.1/satsim/generator/obs/io.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/generator/obs/rpo.py` & `satsim-0.15.1/satsim/generator/obs/rpo.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/geometry/astrometric.py` & `satsim-0.15.1/satsim/geometry/astrometric.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/geometry/csvsc.py` & `satsim-0.15.1/satsim/geometry/csvsc.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/geometry/draw.py` & `satsim-0.15.1/satsim/geometry/draw.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/geometry/ephemeris.py` & `satsim-0.15.1/satsim/geometry/ephemeris.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/geometry/random.py` & `satsim-0.15.1/satsim/geometry/random.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/geometry/sgp4.py` & `satsim-0.15.1/satsim/geometry/sgp4.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/geometry/sprite.py` & `satsim-0.15.1/satsim/geometry/sprite.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/geometry/sstr7.py` & `satsim-0.15.1/satsim/geometry/sstr7.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/geometry/transform.py` & `satsim-0.15.1/satsim/geometry/transform.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/geometry/twobody.py` & `satsim-0.15.1/satsim/geometry/twobody.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/geometry/wcs.py` & `satsim-0.15.1/satsim/geometry/wcs.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/image/augment.py` & `satsim-0.15.1/satsim/image/augment.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/image/fpa.py` & `satsim-0.15.1/satsim/image/fpa.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/image/model.py` & `satsim-0.15.1/satsim/image/model.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/image/noise.py` & `satsim-0.15.1/satsim/image/noise.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/image/psf.py` & `satsim-0.15.1/satsim/image/psf.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/image/render.py` & `satsim-0.15.1/satsim/image/render.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/io/czml.py` & `satsim-0.15.1/satsim/io/czml.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/io/fits.py` & `satsim-0.15.1/satsim/io/fits.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/io/image.py` & `satsim-0.15.1/satsim/io/image.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/io/satnet.py` & `satsim-0.15.1/satsim/io/satnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             'pixels': opix,
             'snr': osnr,
         }))
 
     return data
 
 
-def write_frame(dir_name, sat_name, fpa_digital, meta_data, frame_num, exposure_time, time_stamp, ssp, show_obs_boxes=True, astrometrics=None, save_pickle=False, dtype='uint16', save_jpeg=True, ground_truth=None, ground_truth_min=0):
+def write_frame(dir_name, sat_name, fpa_digital, meta_data, frame_num, exposure_time, time_stamp, ssp, show_obs_boxes=True, astrometrics=None, save_pickle=False, dtype='uint16', save_jpeg=True, ground_truth=None, ground_truth_min=None):
     """Write image and annotation files compatible with SatNet. In addition,
     writes annotated images and SatSim configuration file for reference.
 
     Args:
         dir_name: `string`, directory to save files to
         sat_name: `string`, satellite name
         fpa_digital: `array`, image as a numpy array
@@ -214,11 +214,12 @@
         # broadcast scalars
         def f(x):
             return x if x.shape == fpa_digital.shape else np.resize(x, fpa_digital.shape)
 
         ground_truth = np.stack(list(map(f, ground_truth.values())))
 
         # clip values
-        ground_truth[ground_truth < ground_truth_min] = 0
+        if ground_truth_min is not None:
+            ground_truth[ground_truth < ground_truth_min] = 0
 
         tifffile.imwrite(os.path.join(annotation_dir, '{}.tiff'.format(file_name)), np.stack(ground_truth), dtype='float32', bigtiff=True, compression='lzw',
                          metadata={'ImageDescription': keys})
```

### Comparing `satsim-0.15.0/satsim/math/angle.py` & `satsim-0.15.1/satsim/math/angle.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/math/const.py` & `satsim-0.15.1/satsim/math/const.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/math/conv.py` & `satsim-0.15.1/satsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/math/fft.py` & `satsim-0.15.1/satsim/math/fft.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/math/interpolate.py` & `satsim-0.15.1/satsim/math/interpolate.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/math/random.py` & `satsim-0.15.1/satsim/math/random.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/math/stats.py` & `satsim-0.15.1/satsim/math/stats.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/pipeline/__init__.py` & `satsim-0.15.1/satsim/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/satsim.py` & `satsim-0.15.1/satsim/satsim.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/time/__init__.py` & `satsim-0.15.1/satsim/time/__init__.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/util/system.py` & `satsim-0.15.1/satsim/util/system.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/util/thread.py` & `satsim-0.15.1/satsim/util/thread.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/util/timer.py` & `satsim-0.15.1/satsim/util/timer.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/vecmath/Cartesian2.py` & `satsim-0.15.1/satsim/vecmath/Cartesian2.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/vecmath/Cartesian3.py` & `satsim-0.15.1/satsim/vecmath/Cartesian3.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/vecmath/Cartesian4.py` & `satsim-0.15.1/satsim/vecmath/Cartesian4.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/vecmath/Matrix2.py` & `satsim-0.15.1/satsim/vecmath/Matrix2.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/vecmath/Matrix3.py` & `satsim-0.15.1/satsim/vecmath/Matrix3.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/vecmath/Matrix4.py` & `satsim-0.15.1/satsim/vecmath/Matrix4.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim/vecmath/Quaternion.py` & `satsim-0.15.1/satsim/vecmath/Quaternion.py`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/satsim.egg-info/PKG-INFO` & `satsim-0.15.1/satsim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsim
-Version: 0.15.0
+Version: 0.15.1
 Summary: Satellite observation and scene simulator.
 Home-page: https://github.com/ssc-ai/satsim
 Author: Alex Cabello
 Author-email: alexander.cabello@algoritics.com
 License: UNKNOWN
 Keywords: satsim
 Platform: UNKNOWN
@@ -37,14 +37,21 @@
 --------
 
 * [History](HISTORY.md)
 
 History
 =======
 
+0.15.1
+---------------------
+
+* Remove clipping of negative values in ground truth files by default.
+* Fix missing dependencies for ground truth file generation.
+
+
 0.15.0
 ---------------------
 
 * Add support to save ground truth image data to the Annotations directory. Set sim option `save_ground_truth` to `true`.
 * Add support for running on CPU with no GPU acceleration.
 * Add CZML options for sensor visualization and object billboard image.
```

### Comparing `satsim-0.15.0/satsim.egg-info/SOURCES.txt` & `satsim-0.15.1/satsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satsim-0.15.0/setup.cfg` & `satsim-0.15.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.15.0
+current_version = 0.15.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `satsim-0.15.0/setup.py` & `satsim-0.15.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     'diskcache==5.0.3',
     'pydash~=4.9.0',
     'asdf==2.14.3',
     'pygc==1.3.0',
     'numba~=0.56.0',
     'pooch~=1.6.0',
     'czmlpy~=0.9.0',
+    'tifffile==2023.4.12',
+    'imagecodecs==2023.3.16',
 ]
 
 setup_requirements = ['pytest-runner', ]
 
 test_requirements = ['pytest', ]
 
 setup(
@@ -63,10 +65,10 @@
     keywords='satsim',
     name='satsim',
     packages=find_packages(include=['satsim', 'satsim.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ssc-ai/satsim',
-    version='0.15.0',
+    version='0.15.1',
     zip_safe=False,
 )
```

