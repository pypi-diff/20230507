# Comparing `tmp/ansys-mapdl-reader-0.52.8.tar.gz` & `tmp/ansys-mapdl-reader-0.52.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-mapdl-reader-0.52.8.tar", last modified: Thu Jan 26 19:46:32 2023, max compression
+gzip compressed data, was "ansys-mapdl-reader-0.52.9.tar", last modified: Thu Feb  9 08:14:23 2023, max compression
```

## Comparing `ansys-mapdl-reader-0.52.8.tar` & `ansys-mapdl-reader-0.52.9.tar`

### file list

```diff
@@ -1,59 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-01-26 19:46:32.349269 ansys-mapdl-reader-0.52.8/
--rw-rw-rw-   0        0        0     1110 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/LICENSE
--rw-rw-rw-   0        0        0       39 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/MANIFEST.in
--rw-rw-rw-   0        0        0    12265 2023-01-26 19:46:32.349269 ansys-mapdl-reader-0.52.8/PKG-INFO
--rw-rw-rw-   0        0        0    11343 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-01-26 19:46:32.302392 ansys-mapdl-reader-0.52.8/ansys/
-drwxrwxrwx   0        0        0        0 2023-01-26 19:46:32.302392 ansys-mapdl-reader-0.52.8/ansys/mapdl/
-drwxrwxrwx   0        0        0        0 2023-01-26 19:46:32.333644 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/
--rw-rw-rw-   0        0        0     1040 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/__init__.py
--rw-rw-rw-   0        0        0     2130 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/_mp_keys.py
--rw-rw-rw-   0        0        0    11811 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/_rst_keys.py
--rw-rw-rw-   0        0        0      299 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/_version.py
--rw-rw-rw-   0        0        0    27958 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/archive.py
--rw-rw-rw-   0        0        0     2134 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cell_quality.py
--rw-rw-rw-   0        0        0    16675 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/common.py
--rw-rw-rw-   0        0        0    69919 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cyclic_reader.py
-drwxrwxrwx   0        0        0        0 2023-01-26 19:46:32.333644 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/
--rw-rw-rw-   0        0        0     5116 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/_archive.pyx
--rw-rw-rw-   0        0        0    63926 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/_binary_reader.pyx
--rw-rw-rw-   0        0        0   153187 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/_cellqual.pyx
--rw-rw-rw-   0        0        0    21686 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/_reader.pyx
--rw-rw-rw-   0        0        0     9615 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/_relaxmidside.pyx
--rw-rw-rw-   0        0        0    13105 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/archive.c
--rw-rw-rw-   0        0        0      548 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/archive.h
--rw-rw-rw-   0        0        0    18886 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/binary_reader.cpp
--rw-rw-rw-   0        0        0      472 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/binary_reader.h
--rw-rw-rw-   0        0        0      154 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/parsefull.h
--rw-rw-rw-   0        0        0    11294 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/reader.c
--rw-rw-rw-   0        0        0      320 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/reader.h
--rw-rw-rw-   0        0        0    16932 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/vtk_support.c
--rw-rw-rw-   0        0        0      158 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/vtk_support.h
--rw-rw-rw-   0        0        0    15235 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/dis_result.py
--rw-rw-rw-   0        0        0    16705 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/elements.py
--rw-rw-rw-   0        0        0    31430 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/emat.py
--rw-rw-rw-   0        0        0      459 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/errors.py
-drwxrwxrwx   0        0        0        0 2023-01-26 19:46:32.349269 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/
--rw-rw-rw-   0        0        0    45192 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/HexBeam.cdb
--rw-rw-rw-   0        0        0   569028 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/TetBeam.cdb
--rw-rw-rw-   0        0        0       51 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/__init__.py
--rw-rw-rw-   0        0        0     3566 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/downloads.py
--rw-rw-rw-   0        0        0     7125 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/examples.py
--rw-rw-rw-   0        0        0   851968 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/file.full
--rw-rw-rw-   0        0        0   917504 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/file.rst
--rw-rw-rw-   0        0        0    80838 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/sector.cdb
--rw-rw-rw-   0        0        0    14379 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/full.py
--rw-rw-rw-   0        0        0    26873 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/mesh.py
--rw-rw-rw-   0        0        0     7891 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/misc.py
--rw-rw-rw-   0        0        0     7134 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/plotting.py
--rw-rw-rw-   0        0        0   186966 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/rst.py
--rw-rw-rw-   0        0        0    10764 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/rst_avail.py
-drwxrwxrwx   0        0        0        0 2023-01-26 19:46:32.349269 ansys-mapdl-reader-0.52.8/ansys_mapdl_reader.egg-info/
--rw-rw-rw-   0        0        0    12265 2023-01-26 19:46:32.000000 ansys-mapdl-reader-0.52.8/ansys_mapdl_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2036 2023-01-26 19:46:32.000000 ansys-mapdl-reader-0.52.8/ansys_mapdl_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-26 19:46:32.000000 ansys-mapdl-reader-0.52.8/ansys_mapdl_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-01-26 19:46:32.000000 ansys-mapdl-reader-0.52.8/ansys_mapdl_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-01-26 19:46:32.000000 ansys-mapdl-reader-0.52.8/ansys_mapdl_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1001 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-26 19:46:32.349269 ansys-mapdl-reader-0.52.8/setup.cfg
--rw-rw-rw-   0        0        0     3648 2023-01-26 19:45:37.000000 ansys-mapdl-reader-0.52.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-09 08:14:23.325569 ansys-mapdl-reader-0.52.9/
+-rw-rw-rw-   0        0        0     1110 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    12265 2023-02-09 08:14:23.325569 ansys-mapdl-reader-0.52.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11343 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-02-09 08:14:23.278651 ansys-mapdl-reader-0.52.9/ansys/
+drwxrwxrwx   0        0        0        0 2023-02-09 08:14:23.278651 ansys-mapdl-reader-0.52.9/ansys/mapdl/
+drwxrwxrwx   0        0        0        0 2023-02-09 08:14:23.309899 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/
+-rw-rw-rw-   0        0        0     1040 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/__init__.py
+-rw-rw-rw-   0        0        0     2130 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/_mp_keys.py
+-rw-rw-rw-   0        0        0    11811 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/_rst_keys.py
+-rw-rw-rw-   0        0        0      299 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/_version.py
+-rw-rw-rw-   0        0        0    27956 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/archive.py
+-rw-rw-rw-   0        0        0     2134 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cell_quality.py
+-rw-rw-rw-   0        0        0    16671 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/common.py
+-rw-rw-rw-   0        0        0    69919 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cyclic_reader.py
+drwxrwxrwx   0        0        0        0 2023-02-09 08:14:23.309899 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/
+-rw-rw-rw-   0        0        0     5116 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/_archive.pyx
+-rw-rw-rw-   0        0        0    63926 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/_binary_reader.pyx
+-rw-rw-rw-   0        0        0   153187 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/_cellqual.pyx
+-rw-rw-rw-   0        0        0    21686 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/_reader.pyx
+-rw-rw-rw-   0        0        0     9615 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/_relaxmidside.pyx
+-rw-rw-rw-   0        0        0    13105 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/archive.c
+-rw-rw-rw-   0        0        0      548 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/archive.h
+-rw-rw-rw-   0        0        0    18886 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/binary_reader.cpp
+-rw-rw-rw-   0        0        0      472 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/binary_reader.h
+-rw-rw-rw-   0        0        0      154 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/parsefull.h
+-rw-rw-rw-   0        0        0    11294 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/reader.c
+-rw-rw-rw-   0        0        0      320 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/reader.h
+-rw-rw-rw-   0        0        0    16932 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/vtk_support.c
+-rw-rw-rw-   0        0        0      158 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/vtk_support.h
+-rw-rw-rw-   0        0        0    15235 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/dis_result.py
+-rw-rw-rw-   0        0        0    16705 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/elements.py
+-rw-rw-rw-   0        0        0    31430 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/emat.py
+-rw-rw-rw-   0        0        0      459 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/errors.py
+drwxrwxrwx   0        0        0        0 2023-02-09 08:14:23.309899 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/
+-rw-rw-rw-   0        0        0    45192 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/HexBeam.cdb
+-rw-rw-rw-   0        0        0   569028 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/TetBeam.cdb
+-rw-rw-rw-   0        0        0       51 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/__init__.py
+-rw-rw-rw-   0        0        0     3566 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/downloads.py
+-rw-rw-rw-   0        0        0     7125 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/examples.py
+-rw-rw-rw-   0        0        0   851968 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/file.full
+-rw-rw-rw-   0        0        0   917504 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/file.rst
+-rw-rw-rw-   0        0        0    80838 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/sector.cdb
+-rw-rw-rw-   0        0        0    14377 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/full.py
+-rw-rw-rw-   0        0        0    26871 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/mesh.py
+-rw-rw-rw-   0        0        0     7891 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/misc.py
+-rw-rw-rw-   0        0        0     7134 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/plotting.py
+-rw-rw-rw-   0        0        0   186397 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/rst.py
+-rw-rw-rw-   0        0        0    10764 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/rst_avail.py
+drwxrwxrwx   0        0        0        0 2023-02-09 08:14:23.309899 ansys-mapdl-reader-0.52.9/ansys_mapdl_reader.egg-info/
+-rw-rw-rw-   0        0        0    12265 2023-02-09 08:14:23.000000 ansys-mapdl-reader-0.52.9/ansys_mapdl_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2220 2023-02-09 08:14:23.000000 ansys-mapdl-reader-0.52.9/ansys_mapdl_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-09 08:14:23.000000 ansys-mapdl-reader-0.52.9/ansys_mapdl_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-02-09 08:14:23.000000 ansys-mapdl-reader-0.52.9/ansys_mapdl_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-02-09 08:14:23.000000 ansys-mapdl-reader-0.52.9/ansys_mapdl_reader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1001 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-02-09 08:14:23.325569 ansys-mapdl-reader-0.52.9/setup.cfg
+-rw-rw-rw-   0        0        0     3648 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-09 08:14:23.325569 ansys-mapdl-reader-0.52.9/tests/
+-rw-rw-rw-   0        0        0      487 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/tests/test_beam44.py
+-rw-rw-rw-   0        0        0    15079 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/tests/test_binary_reader.py
+-rw-rw-rw-   0        0        0     1941 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/tests/test_binary_reader_cython.py
+-rw-rw-rw-   0        0        0    15857 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/tests/test_cyclic.py
+-rw-rw-rw-   0        0        0     9241 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/tests/test_dist_rst.py
+-rw-rw-rw-   0        0        0     1676 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/tests/test_emat.py
+-rw-rw-rw-   0        0        0     2884 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/tests/test_full.py
+-rw-rw-rw-   0        0        0    20949 2023-02-09 08:13:08.000000 ansys-mapdl-reader-0.52.9/tests/test_rst.py
```

### Comparing `ansys-mapdl-reader-0.52.8/LICENSE` & `ansys-mapdl-reader-0.52.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/PKG-INFO` & `ansys-mapdl-reader-0.52.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-mapdl-reader
-Version: 0.52.8
+Version: 0.52.9
 Summary: Pythonic interface to files generated by MAPDL
 Home-page: https://github.com/pyansys/pymapdl-reader
 License: MIT
 Keywords: vtk MAPDL ANSYS cdb full rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
```

### Comparing `ansys-mapdl-reader-0.52.8/README.rst` & `ansys-mapdl-reader-0.52.9/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/__init__.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/_mp_keys.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/_mp_keys.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/_rst_keys.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/_rst_keys.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/archive.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,15 +638,14 @@
         typenum,
         nodenum,
         mode="a",
     )
 
     if include_components:
         with open(filename, "a") as fid:
-
             # write node components
             for node_key in grid.point_data:
                 arr = grid.point_data[node_key]
                 if arr.dtype in [np.uint8, np.bool_]:
                     items = nodenum[arr.view(np.bool_)]
                     write_cmblock(fid, items, node_key, "NODE")
```

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cell_quality.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cell_quality.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/common.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,18 +305,16 @@
     longint = struct.pack(">I", inth) + struct.pack(">I", intl)
     return struct.unpack(">q", longint)[0]
 
 
 def read_standard_header(filename):
     """Reads standard header"""
     with open(filename, "rb") as f:
-
         endian = "<"
         if np.fromfile(f, dtype="<i", count=1) != 100:
-
             # Check if big enos
             f.seek(0)
             if np.fromfile(f, dtype=">i", count=1) == 100:
                 endian = ">"
 
             # Otherwise, it's probably not a result file
             else:
```

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cyclic_reader.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cyclic_reader.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/_archive.pyx` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/_archive.pyx`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/_binary_reader.pyx` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/_binary_reader.pyx`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/_cellqual.pyx` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/_cellqual.pyx`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/_reader.pyx` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/_reader.pyx`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/_relaxmidside.pyx` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/_relaxmidside.pyx`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/archive.c` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/archive.c`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/archive.h` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/archive.h`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/binary_reader.cpp` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/binary_reader.cpp`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/reader.c` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/reader.c`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/cython/vtk_support.c` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/cython/vtk_support.c`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/dis_result.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/dis_result.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/elements.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/elements.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/emat.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/emat.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/HexBeam.cdb` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/HexBeam.cdb`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/TetBeam.cdb` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/TetBeam.cdb`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/downloads.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/examples.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/examples.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/file.full` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/file.full`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/file.rst` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/file.rst`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/examples/sector.cdb` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/examples/sector.cdb`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/full.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/full.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,14 @@
         if mdata is not None:
             self._mrow = mrow
             self._mcol = mcol
             self._mdata = mdata
 
         # output as a sparse matrix
         if as_sparse:
-
             if kdata is not None:
                 k = coo_matrix((self.neqn,) * 2)
                 k.data = kdata  # data has to be set first
                 k.row = krow
                 k.col = kcol
 
                 # convert to csc matrix (generally faster for sparse solvers)
```

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/mesh.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
 
         # ANSYS element type to VTK map
         type_ref = np.empty(2 << 16, np.int32)  # 131072
         type_ref[self._ekey[:, 0]] = etype_map[self._ekey[:, 1]]
 
         if allowable_types is None or 200 in allowable_types:
             for etype_ind, etype in self._ekey:
-
                 # MESH200
                 if etype == 200 and etype_ind in self.key_option:
                     # keyoption 1 contains various cell types
                     # map them to the corresponding type (see elements.py)
                     mapped = MESH200_MAP[self.key_option[etype_ind][0][1]]
                     type_ref[etype_ind] = mapped
```

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/misc.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/misc.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/plotting.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/plotting.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/rst.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/rst.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import time
 from typing import Union
 import warnings
 
 import numpy as np
 import pyvista as pv
 from pyvista import _vtk as vtk
+from pyvista.themes import DefaultTheme
 from tqdm import tqdm
 
 from ansys.mapdl.reader import _binary_reader, _reader, elements
 from ansys.mapdl.reader._binary_reader import (
     AnsysFile,
     cells_with_all_nodes,
     cells_with_any_nodes,
@@ -56,15 +57,15 @@
     base = int(num // 8)
     shift = int(num % 8)
     return (data & (1 << shift)) >> shift
 
 
 EMAIL_ME = """Please raise an issue at:
 https://github.com/pyansys/pymapdl-reader/issues
-Or email the developer at alexander.kaszynski@ansys.com
+Or email the PyAnsys support team at pyansys.support@ansys.com
 """
 np.seterr(divide="ignore", invalid="ignore")
 
 
 # Pointer information from ansys interface manual
 # =============================================================================
 # Individual element index table
@@ -3016,36 +3017,36 @@
         plotter = pv.Plotter(off_screen=off_screen, notebook=notebook)
 
         # set axes
         if kwargs.pop("show_axes", True):
             plotter.add_axes()
 
         # set background
-        plotter.background_color = kwargs.pop("background", None)
+        theme = DefaultTheme()
+        theme.background = kwargs.pop("background", None)
 
         # remove extra keyword args
         kwargs.pop("node_components", None)
         kwargs.pop("sel_type_all", None)
 
         if overlay_wireframe:
             plotter.add_mesh(self.grid, style="wireframe", color="w", opacity=0.5)
 
         copied_mesh = mesh.copy()
         plotter.add_mesh(copied_mesh, scalars=scalars, rng=rng, cmap=cmap, **kwargs)
 
         # set scalar bar text colors
         if text_color:
-            text_color = pv.parse_color(text_color)
-            plotter.scalar_bar.GetLabelTextProperty().SetColor(text_color)
-            plotter.scalar_bar.GetAnnotationTextProperty().SetColor(text_color)
-            plotter.scalar_bar.GetTitleTextProperty().SetColor(text_color)
+            theme = DefaultTheme()
+            theme.color = text_color
+            pv.global_theme.load_theme(theme)
 
         # NAN/missing data are white
         # plotter.renderers[0].SetUseDepthPeeling(1)  # <-- for transparency issues
-        plotter.mapper.GetLookupTable().SetNanColor(1, 1, 1, 1)
+        theme.nan_color = [1, 1, 1, 1]
 
         if cpos:
             plotter.camera_position = cpos
 
         if movie_filename:
             movie_filename = str(movie_filename)
             if movie_filename.strip()[-3:] == "gif":
@@ -3099,15 +3100,14 @@
                     vtk.vtkCommand.ExitEvent,
                     lambda render, event: exit_callback(plotter, render, event),
                 )
 
             first_loop = True
             cached_normals = [None for _ in range(n_frames)]
             while self._animating:
-
                 for j, angle in enumerate(np.linspace(0, np.pi * 2, n_frames + 1)[:-1]):
                     mag_adj = np.sin(angle)
                     if scalars is not None:
                         copied_mesh.active_scalars[:] = scalars * mag_adj
                     copied_mesh.points[:] = orig_pts + disp * mag_adj
 
                     # normals have to be updated on the fly
@@ -3117,20 +3117,16 @@
                                 cell_normals=False, inplace=True
                             )
                             cached_normals[j] = copied_mesh.point_data["Normals"]
                         else:
                             copied_mesh.point_data["Normals"][:] = cached_normals[j]
 
                     if add_text:
-                        # 2 maps to vtk.vtkCornerAnnotation.UpperLeft
-                        plotter.textActor.SetText(
-                            2,
-                            "%s\nPhase %.1f Degrees"
-                            % (result_text, (angle * 180 / np.pi)),
-                        )
+                        phase = angle * 180 / np.pi
+                        plotter.add_text(f"{result_text} \nPhase {phase} Degrees")
 
                     # at max supported framerate
                     plotter.update(1, force_redraw=True)
                     if not self._animating:
                         break
 
                     if movie_filename and first_loop:
@@ -3260,37 +3256,36 @@
         plotter = pv.Plotter(off_screen=off_screen, notebook=notebook)
 
         # set axes
         if kwargs.pop("show_axes", True):
             plotter.add_axes()
 
         # set background
-        plotter.background_color = kwargs.pop("background", None)
+        theme = DefaultTheme()
+        theme.background = kwargs.pop("background", None)
 
         # remove extra keyword args
         kwargs.pop("node_components", None)
         kwargs.pop("sel_type_all", None)
 
         # if overlay_wireframe:
         #     plotter.add_mesh(self.grid, style='wireframe', color='w',
         #                      opacity=0.5)
 
         copied_mesh = mesh.copy()
         plotter.add_mesh(copied_mesh, scalars=scalars[0], rng=rng, cmap=cmap, **kwargs)
 
         # set scalar bar text colors
         if text_color:
-            text_color = pv.parse_color(text_color)
-            plotter.scalar_bar.GetLabelTextProperty().SetColor(text_color)
-            plotter.scalar_bar.GetAnnotationTextProperty().SetColor(text_color)
-            plotter.scalar_bar.GetTitleTextProperty().SetColor(text_color)
+            theme.color = text_color
+            pv.global_theme.load_theme(theme)
 
         # NAN/missing data are white
         # plotter.renderers[0].SetUseDepthPeeling(1)  # <-- for transparency issues
-        plotter.mapper.GetLookupTable().SetNanColor(1, 1, 1, 1)
+        theme.nan_color = [1, 1, 1, 1]
 
         if cpos:
             plotter.camera_position = cpos
 
         if movie_filename:
             movie_filename = str(movie_filename)
             if movie_filename.strip()[-3:] == "gif":
@@ -3331,16 +3326,15 @@
         first_loop = True
         while self._animating:
             for i, data in enumerate(scalars):
                 tstart_render = time.time()
                 copied_mesh.active_scalars[:] = data
 
                 if text is not None:
-                    # 2 maps to vtk.vtkCornerAnnotation.UpperLeft
-                    plotter.textActor.SetText(2, text[i])
+                    plotter.add_text(text[i])
 
                 # at max supported framerate
                 plotter.update(1, force_redraw=True)
                 if not self._animating:
                     break
 
                 if movie_filename and first_loop:
```

### Comparing `ansys-mapdl-reader-0.52.8/ansys/mapdl/reader/rst_avail.py` & `ansys-mapdl-reader-0.52.9/ansys/mapdl/reader/rst_avail.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/ansys_mapdl_reader.egg-info/PKG-INFO` & `ansys-mapdl-reader-0.52.9/ansys_mapdl_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-mapdl-reader
-Version: 0.52.8
+Version: 0.52.9
 Summary: Pythonic interface to files generated by MAPDL
 Home-page: https://github.com/pyansys/pymapdl-reader
 License: MIT
 Keywords: vtk MAPDL ANSYS cdb full rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
```

### Comparing `ansys-mapdl-reader-0.52.8/ansys_mapdl_reader.egg-info/SOURCES.txt` & `ansys-mapdl-reader-0.52.9/ansys_mapdl_reader.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -52,8 +52,16 @@
 ansys/mapdl/reader/examples/file.full
 ansys/mapdl/reader/examples/file.rst
 ansys/mapdl/reader/examples/sector.cdb
 ansys_mapdl_reader.egg-info/PKG-INFO
 ansys_mapdl_reader.egg-info/SOURCES.txt
 ansys_mapdl_reader.egg-info/dependency_links.txt
 ansys_mapdl_reader.egg-info/requires.txt
-ansys_mapdl_reader.egg-info/top_level.txt
+ansys_mapdl_reader.egg-info/top_level.txt
+tests/test_beam44.py
+tests/test_binary_reader.py
+tests/test_binary_reader_cython.py
+tests/test_cyclic.py
+tests/test_dist_rst.py
+tests/test_emat.py
+tests/test_full.py
+tests/test_rst.py
```

### Comparing `ansys-mapdl-reader-0.52.8/pyproject.toml` & `ansys-mapdl-reader-0.52.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-reader-0.52.8/setup.py` & `ansys-mapdl-reader-0.52.9/setup.py`

 * *Files identical despite different names*

