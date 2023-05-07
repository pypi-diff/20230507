# Comparing `tmp/pyemaps-1.0.3.tar.gz` & `tmp/pyemaps-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\sharon\dev_space\pyemaps_root\pyemaps\dist\tmptb505fne\pyemaps-1.0.3.tar", last modified: Sun Apr 23 21:58:38 2023, max compression
+gzip compressed data, was "C:\Users\sharon\dev_space\pyemaps_root\pyemaps\dist\.tmp-lzse0gda\pyemaps-1.0.4.tar", last modified: Sun May  7 17:11:58 2023, max compression
```

## Comparing `pyemaps-1.0.3.tar` & `pyemaps-1.0.4.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 21:58:38.000000 pyemaps-1.0.3/
--rw-rw-rw-   0        0        0    47330 2023-04-03 21:05:15.000000 pyemaps-1.0.3/COPYING
-drwxrwxrwx   0        0        0        0 2023-04-23 21:58:38.000000 pyemaps-1.0.3/CifFile/
-drwxrwxrwx   0        0        0        0 2023-04-23 21:58:38.000000 pyemaps-1.0.3/CifFile/src/
--rw-rw-rw-   0        0        0   152727 2022-08-25 21:11:57.000000 pyemaps-1.0.3/CifFile/src/CifFile_module.py
--rw-rw-rw-   0        0        0   117625 2022-08-25 21:11:57.000000 pyemaps-1.0.3/CifFile/src/StarFile.py
--rw-rw-rw-   0        0        0     2905 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/TypeContentsParser.py
--rw-rw-rw-   0        0        0    14238 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/YappsStarParser_1_0.py
--rw-rw-rw-   0        0        0    14246 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/YappsStarParser_1_1.py
--rw-rw-rw-   0        0        0    21486 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/YappsStarParser_2_0.py
--rw-rw-rw-   0        0        0    22321 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/YappsStarParser_STAR2.py
--rw-rw-rw-   0        0        0      447 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:58:38.000000 pyemaps-1.0.3/CifFile/src/drel/
--rw-rw-rw-   0        0        0       13 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/drel/__init__.py
--rw-rw-rw-   0        0        0    16879 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/drel/drel_ast_yacc.py
--rw-rw-rw-   0        0        0     4645 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/drel/drel_lex.py
--rw-rw-rw-   0        0        0     4383 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/drel/drel_runtime.py
--rw-rw-rw-   0        0        0    81599 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/drel/parsetab.py
--rw-rw-rw-   0        0        0    29728 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/drel/py_from_ast.py
--rw-rw-rw-   0        0        0    82535 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/parsetab.py
--rw-rw-rw-   0        0        0    14038 2022-08-25 21:11:58.000000 pyemaps-1.0.3/CifFile/src/yapps3_compiled_rt.py
--rw-rw-rw-   0        0        0      273 2023-04-04 15:49:10.000000 pyemaps-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      942 2023-04-23 21:58:38.000000 pyemaps-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-03 21:05:15.000000 pyemaps-1.0.3/README.md
--rw-rw-rw-   0        0        0     3052 2022-08-22 20:53:01.000000 pyemaps-1.0.3/__config__.py
--rw-rw-rw-   0        0        0     5814 2023-04-03 21:05:15.000000 pyemaps-1.0.3/__init__.py
--rw-rw-rw-   0        0        0     4634 2023-04-23 21:55:13.000000 pyemaps-1.0.3/__main__.py
--rw-rw-rw-   0        0        0       21 2023-04-23 21:58:20.000000 pyemaps-1.0.3/__version__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:58:38.000000 pyemaps-1.0.3/cdata/
--rw-rw-rw-   0        0        0      143 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Aluminium.xtl
--rw-rw-rw-   0        0        0      273 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/AluminiumOxide.xtl
--rw-rw-rw-   0        0        0      147 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Aluminium_FCC.xtl
--rw-rw-rw-   0        0        0      364 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/BariumTitanate_180k.xtl
--rw-rw-rw-   0        0        0      450 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/BariumTitanate_270k.xtl
--rw-rw-rw-   0        0        0      452 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/BariumTitanate_Tetra.xtl
--rw-rw-rw-   0        0        0     2221 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/BiMnO3.xtl
--rw-rw-rw-   0        0        0      528 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Boron_Tetra.xtl
--rw-rw-rw-   0        0        0      278 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/CadmiumSelenide_Hex.xtl
--rw-rw-rw-   0        0        0      197 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/CadmiumSulfide_Cubic.xtl
--rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/CadmiumSulfide_Hex.xtl
--rw-rw-rw-   0        0        0      146 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Chromium_BCC.xtl
--rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/CoSb3_Skutterudite.xtl
--rw-rw-rw-   0        0        0      269 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/CopperOxide.xtl
--rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Copper_FCC.xtl
--rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Cu2O_Cuprite.xtl
--rw-rw-rw-   0        0        0      131 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Diamond.xtl
--rw-rw-rw-   0        0        0      626 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/ErbiumPyrogermanate.xtl
--rw-rw-rw-   0        0        0      198 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/FePd_Tetra.xtl
--rw-rw-rw-   0        0        0      672 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/FeS2_Pyrite.xtl
--rw-rw-rw-   0        0        0      205 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/GalliumAntimonide.xtl
--rw-rw-rw-   0        0        0      201 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/GalliumArsenide.xtl
--rw-rw-rw-   0        0        0      240 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/GalliumNitride.xtl
--rw-rw-rw-   0        0        0      132 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Germanium.xtl
--rw-rw-rw-   0        0        0      142 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Gold_FCC.xtl
--rw-rw-rw-   0        0        0      202 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/IndiumArsenide.xtl
--rw-rw-rw-   0        0        0      271 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/LaMnO3.xtl
--rw-rw-rw-   0        0        0      594 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/LeadZirconateTitanate.xtl
--rw-rw-rw-   0        0        0      965 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Li2MnO3.xtl
--rw-rw-rw-   0        0        0      239 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/NaFeO2.xtl
--rw-rw-rw-   0        0        0      165 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Nb3Sn.xtl
--rw-rw-rw-   0        0        0     3751 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Pentacene.xtl
--rw-rw-rw-   0        0        0      797 2022-07-21 19:25:58.000000 pyemaps-1.0.3/cdata/SiAlONa.xtl
--rw-rw-rw-   0        0        0      113 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Silicon.xtl
--rw-rw-rw-   0        0        0      362 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/StrontiumTitanate.xtl
--rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/TelluriumDioxide.xtl
--rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/TinDioxide_RT.xtl
--rw-rw-rw-   0        0        0      280 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/TitaniumDioxide_Anatase.xtl
--rw-rw-rw-   0        0        0      281 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/TitaniumDioxide_Rutile.xtl
--rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/TungstenDiselenide.xtl
--rw-rw-rw-   0        0        0      366 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/VanadiumDioxide_RT.xtl
--rw-rw-rw-   0        0        0      160 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/ZincOxide.xtl
--rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/Zinc_HCP.xtl
--rw-rw-rw-   0        0        0      203 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/ZirconiumNitride.xtl
--rw-rw-rw-   0        0        0      353 2022-07-14 01:36:02.000000 pyemaps-1.0.3/cdata/limno2.xtl
--rw-rw-rw-   0        0        0    41586 2023-04-03 21:05:15.000000 pyemaps-1.0.3/crystals.py
--rw-rw-rw-   0        0        0     2582 2023-04-23 21:55:13.000000 pyemaps-1.0.3/ddiffs.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:58:38.000000 pyemaps-1.0.3/diffract/
--rw-rw-rw-   0        0        0     1417 2023-04-03 21:05:15.000000 pyemaps-1.0.3/diffract/__init__.py
--rw-rw-rw-   0        0        0    25106 2023-04-23 21:55:13.000000 pyemaps-1.0.3/diffract/bloch_dec.py
--rw-rw-rw-   0        0        0     6927 2023-04-23 21:55:13.000000 pyemaps-1.0.3/diffract/csf_dec.py
--rw-rw-rw-   0        0        0    15552 2023-04-23 21:55:13.000000 pyemaps-1.0.3/diffract/dif_dec.py
--rw-rw-rw-   0        0        0     5069 2023-04-03 21:05:15.000000 pyemaps-1.0.3/diffract/dpgen_dec.py
--rw-rw-rw-   0        0        0     7159 2023-04-23 21:55:13.000000 pyemaps-1.0.3/diffract/mxtal_dec.py
--rw-rw-rw-   0        0        0     3327 2023-04-23 21:55:13.000000 pyemaps-1.0.3/diffract/powder_dec.py
--rw-rw-rw-   0        0        0     2350 2023-04-03 21:05:15.000000 pyemaps-1.0.3/diffract/stereo_dec.py
--rw-rw-rw-   0        0        0    19525 2023-04-23 21:55:13.000000 pyemaps-1.0.3/display.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:58:38.000000 pyemaps-1.0.3/ediom/
--rw-rw-rw-   0        0        0     7322 2023-04-03 21:10:13.000000 pyemaps-1.0.3/ediom/ediom.py
--rw-rw-rw-   0        0        0    35898 2023-04-23 21:58:00.000000 pyemaps-1.0.3/ediom/ediom_dec.py
--rw-rw-rw-   0        0        0    27128 2023-04-23 21:55:13.000000 pyemaps-1.0.3/emcontrols.py
--rw-rw-rw-   0        0        0     7175 2023-04-03 21:05:15.000000 pyemaps-1.0.3/errors.py
--rw-rw-rw-   0        0        0    33216 2023-04-23 21:55:13.000000 pyemaps-1.0.3/fileutils.py
--rw-rw-rw-   0        0        0    30922 2023-04-23 21:55:13.000000 pyemaps-1.0.3/kdiffs.py
--rw-rw-rw-   0        0        0     1020 2022-07-14 01:36:02.000000 pyemaps-1.0.3/license.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 21:58:38.000000 pyemaps-1.0.3/pyemaps.egg-info/
--rw-rw-rw-   0        0        0      942 2023-04-23 21:58:37.000000 pyemaps-1.0.3/pyemaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5640 2023-04-23 21:58:38.000000 pyemaps-1.0.3/pyemaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 21:58:37.000000 pyemaps-1.0.3/pyemaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-23 21:58:38.000000 pyemaps-1.0.3/pyemaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 21:58:38.000000 pyemaps-1.0.3/pyemaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      119 2022-08-18 02:23:09.000000 pyemaps-1.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-23 21:58:38.000000 pyemaps-1.0.3/samples/
--rw-rw-rw-   0        0        0   160008 2023-04-03 21:05:15.000000 pyemaps-1.0.3/samples/al.img
--rw-rw-rw-   0        0        0   852144 2023-04-18 14:23:21.000000 pyemaps-1.0.3/samples/al_db.bin
--rw-rw-rw-   0        0        0     2703 2023-04-23 21:55:13.000000 pyemaps-1.0.3/samples/al_ediom.py
--rw-rw-rw-   0        0        0     2137 2023-04-03 21:05:15.000000 pyemaps-1.0.3/samples/powder.py
--rw-rw-rw-   0        0        0     3625 2023-04-03 21:05:15.000000 pyemaps-1.0.3/samples/si_bloch.py
--rw-rw-rw-   0        0        0     1676 2023-04-18 01:01:39.000000 pyemaps-1.0.3/samples/si_constructor.py
--rw-rw-rw-   0        0        0     1862 2023-04-23 21:55:13.000000 pyemaps-1.0.3/samples/si_csf.py
--rw-rw-rw-   0        0        0     3953 2023-04-18 21:27:47.000000 pyemaps-1.0.3/samples/si_dif.py
--rw-rw-rw-   0        0        0      795 2023-04-23 21:55:13.000000 pyemaps-1.0.3/samples/si_dpgen.py
--rw-rw-rw-   0        0        0     2691 2023-04-03 21:05:15.000000 pyemaps-1.0.3/samples/si_pyemaps.py
--rw-rw-rw-   0        0        0     1707 2023-04-03 21:05:15.000000 pyemaps-1.0.3/samples/si_rawblochimgs.py
--rw-rw-rw-   0        0        0     3672 2023-04-23 21:55:13.000000 pyemaps-1.0.3/samples/si_scm.py
--rw-rw-rw-   0        0        0     3280 2023-04-23 21:55:13.000000 pyemaps-1.0.3/samples/si_stereo.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:58:38.000000 pyemaps-1.0.3/scattering/
--rw-rw-rw-   0        0        0      892 2023-04-03 21:05:15.000000 pyemaps-1.0.3/scattering/__init__.py
--rw-rw-rw-   0        0        0      184 2023-04-03 21:05:15.000000 pyemaps-1.0.3/scattering/sct_dec.py
--rw-rw-rw-   0        0        0      734 2023-04-23 21:58:38.000000 pyemaps-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0    20552 2023-04-23 21:55:13.000000 pyemaps-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:58:38.000000 pyemaps-1.0.3/spg/
--rw-rw-rw-   0        0        0      849 2023-04-03 21:05:15.000000 pyemaps-1.0.3/spg/__init__.py
--rw-rw-rw-   0        0        0      793 2023-04-03 21:05:15.000000 pyemaps-1.0.3/spg/spg_dec.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/
+-rw-rw-rw-   0        0        0    47330 2023-04-03 21:05:15.000000 pyemaps-1.0.4/COPYING
+drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/CifFile/
+drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/CifFile/src/
+-rw-rw-rw-   0        0        0   152727 2022-08-25 21:11:57.000000 pyemaps-1.0.4/CifFile/src/CifFile_module.py
+-rw-rw-rw-   0        0        0   117625 2022-08-25 21:11:57.000000 pyemaps-1.0.4/CifFile/src/StarFile.py
+-rw-rw-rw-   0        0        0     2905 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/TypeContentsParser.py
+-rw-rw-rw-   0        0        0    14238 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/YappsStarParser_1_0.py
+-rw-rw-rw-   0        0        0    14246 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/YappsStarParser_1_1.py
+-rw-rw-rw-   0        0        0    21486 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/YappsStarParser_2_0.py
+-rw-rw-rw-   0        0        0    22321 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/YappsStarParser_STAR2.py
+-rw-rw-rw-   0        0        0      447 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/
+-rw-rw-rw-   0        0        0       13 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/__init__.py
+-rw-rw-rw-   0        0        0    16879 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/drel_ast_yacc.py
+-rw-rw-rw-   0        0        0     4645 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/drel_lex.py
+-rw-rw-rw-   0        0        0     4383 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/drel_runtime.py
+-rw-rw-rw-   0        0        0    81599 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/parsetab.py
+-rw-rw-rw-   0        0        0    29728 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/drel/py_from_ast.py
+-rw-rw-rw-   0        0        0    82535 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/parsetab.py
+-rw-rw-rw-   0        0        0    14038 2022-08-25 21:11:58.000000 pyemaps-1.0.4/CifFile/src/yapps3_compiled_rt.py
+-rw-rw-rw-   0        0        0      273 2023-04-04 15:49:10.000000 pyemaps-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      885 2023-05-07 17:11:58.000000 pyemaps-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-03 21:05:15.000000 pyemaps-1.0.4/README.md
+-rw-rw-rw-   0        0        0     3052 2022-08-22 20:53:01.000000 pyemaps-1.0.4/__config__.py
+-rw-rw-rw-   0        0        0     5814 2023-04-03 21:05:15.000000 pyemaps-1.0.4/__init__.py
+-rw-rw-rw-   0        0        0     4634 2023-04-23 21:55:13.000000 pyemaps-1.0.4/__main__.py
+-rw-rw-rw-   0        0        0       21 2023-05-07 17:11:53.000000 pyemaps-1.0.4/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/cdata/
+-rw-rw-rw-   0        0        0      143 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Aluminium.xtl
+-rw-rw-rw-   0        0        0      273 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/AluminiumOxide.xtl
+-rw-rw-rw-   0        0        0      147 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Aluminium_FCC.xtl
+-rw-rw-rw-   0        0        0      364 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/BariumTitanate_180k.xtl
+-rw-rw-rw-   0        0        0      450 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/BariumTitanate_270k.xtl
+-rw-rw-rw-   0        0        0      452 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/BariumTitanate_Tetra.xtl
+-rw-rw-rw-   0        0        0     2221 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/BiMnO3.xtl
+-rw-rw-rw-   0        0        0      528 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Boron_Tetra.xtl
+-rw-rw-rw-   0        0        0      278 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/CadmiumSelenide_Hex.xtl
+-rw-rw-rw-   0        0        0      197 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/CadmiumSulfide_Cubic.xtl
+-rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/CadmiumSulfide_Hex.xtl
+-rw-rw-rw-   0        0        0      146 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Chromium_BCC.xtl
+-rw-rw-rw-   0        0        0      276 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/CoSb3_Skutterudite.xtl
+-rw-rw-rw-   0        0        0      269 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/CopperOxide.xtl
+-rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Copper_FCC.xtl
+-rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Cu2O_Cuprite.xtl
+-rw-rw-rw-   0        0        0      131 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Diamond.xtl
+-rw-rw-rw-   0        0        0      626 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/ErbiumPyrogermanate.xtl
+-rw-rw-rw-   0        0        0      198 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/FePd_Tetra.xtl
+-rw-rw-rw-   0        0        0      672 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/FeS2_Pyrite.xtl
+-rw-rw-rw-   0        0        0      205 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/GalliumAntimonide.xtl
+-rw-rw-rw-   0        0        0      201 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/GalliumArsenide.xtl
+-rw-rw-rw-   0        0        0      240 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/GalliumNitride.xtl
+-rw-rw-rw-   0        0        0      132 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Germanium.xtl
+-rw-rw-rw-   0        0        0      142 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Gold_FCC.xtl
+-rw-rw-rw-   0        0        0      202 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/IndiumArsenide.xtl
+-rw-rw-rw-   0        0        0      271 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/LaMnO3.xtl
+-rw-rw-rw-   0        0        0      594 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/LeadZirconateTitanate.xtl
+-rw-rw-rw-   0        0        0      965 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Li2MnO3.xtl
+-rw-rw-rw-   0        0        0      239 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/NaFeO2.xtl
+-rw-rw-rw-   0        0        0      165 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Nb3Sn.xtl
+-rw-rw-rw-   0        0        0     3751 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Pentacene.xtl
+-rw-rw-rw-   0        0        0      797 2022-07-21 19:25:58.000000 pyemaps-1.0.4/cdata/SiAlONa.xtl
+-rw-rw-rw-   0        0        0      113 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Silicon.xtl
+-rw-rw-rw-   0        0        0      362 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/StrontiumTitanate.xtl
+-rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/TelluriumDioxide.xtl
+-rw-rw-rw-   0        0        0      272 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/TinDioxide_RT.xtl
+-rw-rw-rw-   0        0        0      280 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/TitaniumDioxide_Anatase.xtl
+-rw-rw-rw-   0        0        0      281 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/TitaniumDioxide_Rutile.xtl
+-rw-rw-rw-   0        0        0      277 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/TungstenDiselenide.xtl
+-rw-rw-rw-   0        0        0      366 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/VanadiumDioxide_RT.xtl
+-rw-rw-rw-   0        0        0      160 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/ZincOxide.xtl
+-rw-rw-rw-   0        0        0      144 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/Zinc_HCP.xtl
+-rw-rw-rw-   0        0        0      203 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/ZirconiumNitride.xtl
+-rw-rw-rw-   0        0        0      353 2022-07-14 01:36:02.000000 pyemaps-1.0.4/cdata/limno2.xtl
+-rw-rw-rw-   0        0        0    41588 2023-05-05 15:21:45.000000 pyemaps-1.0.4/crystals.py
+-rw-rw-rw-   0        0        0     2582 2023-04-23 21:55:13.000000 pyemaps-1.0.4/ddiffs.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/diffract/
+-rw-rw-rw-   0        0        0     1417 2023-04-03 21:05:15.000000 pyemaps-1.0.4/diffract/__init__.py
+-rw-rw-rw-   0        0        0    26094 2023-05-07 15:47:33.000000 pyemaps-1.0.4/diffract/bloch_dec.py
+-rw-rw-rw-   0        0        0     6927 2023-04-23 21:55:13.000000 pyemaps-1.0.4/diffract/csf_dec.py
+-rw-rw-rw-   0        0        0    15552 2023-04-23 21:55:13.000000 pyemaps-1.0.4/diffract/dif_dec.py
+-rw-rw-rw-   0        0        0     5069 2023-04-03 21:05:15.000000 pyemaps-1.0.4/diffract/dpgen_dec.py
+-rw-rw-rw-   0        0        0     7159 2023-04-23 21:55:13.000000 pyemaps-1.0.4/diffract/mxtal_dec.py
+-rw-rw-rw-   0        0        0     3327 2023-04-23 21:55:13.000000 pyemaps-1.0.4/diffract/powder_dec.py
+-rw-rw-rw-   0        0        0     2350 2023-04-03 21:05:15.000000 pyemaps-1.0.4/diffract/stereo_dec.py
+-rw-rw-rw-   0        0        0    19525 2023-05-05 16:35:51.000000 pyemaps-1.0.4/display.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/ediom/
+-rw-rw-rw-   0        0        0     7322 2023-04-03 21:10:13.000000 pyemaps-1.0.4/ediom/ediom.py
+-rw-rw-rw-   0        0        0    35898 2023-04-23 21:58:00.000000 pyemaps-1.0.4/ediom/ediom_dec.py
+-rw-rw-rw-   0        0        0    27128 2023-04-23 21:55:13.000000 pyemaps-1.0.4/emcontrols.py
+-rw-rw-rw-   0        0        0     7175 2023-04-03 21:05:15.000000 pyemaps-1.0.4/errors.py
+-rw-rw-rw-   0        0        0    33216 2023-04-23 21:55:13.000000 pyemaps-1.0.4/fileutils.py
+-rw-rw-rw-   0        0        0    30922 2023-04-23 21:55:13.000000 pyemaps-1.0.4/kdiffs.py
+-rw-rw-rw-   0        0        0     1020 2022-07-14 01:36:02.000000 pyemaps-1.0.4/license.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/pyemaps.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-05-07 17:11:58.000000 pyemaps-1.0.4/pyemaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5768 2023-05-07 17:11:58.000000 pyemaps-1.0.4/pyemaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 17:11:58.000000 pyemaps-1.0.4/pyemaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-05-07 17:11:58.000000 pyemaps-1.0.4/pyemaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-07 17:11:58.000000 pyemaps-1.0.4/pyemaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2022-08-18 02:23:09.000000 pyemaps-1.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/samples/
+-rw-rw-rw-   0        0        0   160008 2023-04-03 21:05:15.000000 pyemaps-1.0.4/samples/al.img
+-rw-rw-rw-   0        0        0   852144 2023-04-18 14:23:21.000000 pyemaps-1.0.4/samples/al_db.bin
+-rw-rw-rw-   0        0        0     2703 2023-04-23 21:55:13.000000 pyemaps-1.0.4/samples/al_ediom.py
+-rw-rw-rw-   0        0        0     2137 2023-04-03 21:05:15.000000 pyemaps-1.0.4/samples/powder.py
+-rw-rw-rw-   0        0        0     3625 2023-04-03 21:05:15.000000 pyemaps-1.0.4/samples/si_bloch.py
+-rw-rw-rw-   0        0        0     1676 2023-04-18 01:01:39.000000 pyemaps-1.0.4/samples/si_constructor.py
+-rw-rw-rw-   0        0        0     1862 2023-04-23 21:55:13.000000 pyemaps-1.0.4/samples/si_csf.py
+-rw-rw-rw-   0        0        0     3953 2023-04-18 21:27:47.000000 pyemaps-1.0.4/samples/si_dif.py
+-rw-rw-rw-   0        0        0      795 2023-04-23 21:55:13.000000 pyemaps-1.0.4/samples/si_dpgen.py
+-rw-rw-rw-   0        0        0     2691 2023-04-03 21:05:15.000000 pyemaps-1.0.4/samples/si_pyemaps.py
+-rw-rw-rw-   0        0        0     1707 2023-04-03 21:05:15.000000 pyemaps-1.0.4/samples/si_rawblochimgs.py
+-rw-rw-rw-   0        0        0     3766 2023-05-03 20:38:32.000000 pyemaps-1.0.4/samples/si_scm.py
+-rw-rw-rw-   0        0        0     3280 2023-04-23 21:55:13.000000 pyemaps-1.0.4/samples/si_stereo.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/scattering/
+-rw-rw-rw-   0        0        0      892 2023-04-03 21:05:15.000000 pyemaps-1.0.4/scattering/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-04-03 21:05:15.000000 pyemaps-1.0.4/scattering/sct_dec.py
+-rw-rw-rw-   0        0        0      734 2023-05-07 17:11:58.000000 pyemaps-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0    21517 2023-05-06 22:11:10.000000 pyemaps-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:11:58.000000 pyemaps-1.0.4/spg/
+-rw-rw-rw-   0        0        0      849 2023-04-03 21:05:15.000000 pyemaps-1.0.4/spg/__init__.py
+-rw-rw-rw-   0        0        0      793 2023-04-03 21:05:15.000000 pyemaps-1.0.4/spg/spg_dec.py
```

### Comparing `pyemaps-1.0.3/COPYING` & `pyemaps-1.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/CifFile_module.py` & `pyemaps-1.0.4/CifFile/src/CifFile_module.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/StarFile.py` & `pyemaps-1.0.4/CifFile/src/StarFile.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/TypeContentsParser.py` & `pyemaps-1.0.4/CifFile/src/TypeContentsParser.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/YappsStarParser_1_0.py` & `pyemaps-1.0.4/CifFile/src/YappsStarParser_1_0.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/YappsStarParser_1_1.py` & `pyemaps-1.0.4/CifFile/src/YappsStarParser_1_1.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/YappsStarParser_2_0.py` & `pyemaps-1.0.4/CifFile/src/YappsStarParser_2_0.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/YappsStarParser_STAR2.py` & `pyemaps-1.0.4/CifFile/src/YappsStarParser_STAR2.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/drel/drel_ast_yacc.py` & `pyemaps-1.0.4/CifFile/src/drel/drel_ast_yacc.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/drel/drel_lex.py` & `pyemaps-1.0.4/CifFile/src/drel/drel_lex.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/drel/drel_runtime.py` & `pyemaps-1.0.4/CifFile/src/drel/drel_runtime.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/drel/parsetab.py` & `pyemaps-1.0.4/CifFile/src/drel/parsetab.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/drel/py_from_ast.py` & `pyemaps-1.0.4/CifFile/src/drel/py_from_ast.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/parsetab.py` & `pyemaps-1.0.4/CifFile/src/parsetab.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/CifFile/src/yapps3_compiled_rt.py` & `pyemaps-1.0.4/CifFile/src/yapps3_compiled_rt.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/PKG-INFO` & `pyemaps-1.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: pyemaps
-Version: 1.0.3
-Summary: UNKNOWN
+Version: 1.0.4
 Home-page: https://www.emlabsolutions.com
 Author: EMLab Solutions, Inc.
 Author-email: support@emlabsoftware.com
-License: UNKNOWN
 Keywords: Transmission,Electron,Diffraction,Simulation,Crystallography,Python
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: license.txt
 License-File: COPYING
 
 Check our full [pyemaps documentation](https://emlab-solutions.github.io/pyemaps) for latest updates.
-
```

### Comparing `pyemaps-1.0.3/__config__.py` & `pyemaps-1.0.4/__config__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/__init__.py` & `pyemaps-1.0.4/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/__main__.py` & `pyemaps-1.0.4/__main__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/cdata/BiMnO3.xtl` & `pyemaps-1.0.4/cdata/BiMnO3.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/cdata/Boron_Tetra.xtl` & `pyemaps-1.0.4/cdata/Boron_Tetra.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/cdata/ErbiumPyrogermanate.xtl` & `pyemaps-1.0.4/cdata/ErbiumPyrogermanate.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/cdata/FeS2_Pyrite.xtl` & `pyemaps-1.0.4/cdata/FeS2_Pyrite.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/cdata/LeadZirconateTitanate.xtl` & `pyemaps-1.0.4/cdata/LeadZirconateTitanate.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/cdata/Li2MnO3.xtl` & `pyemaps-1.0.4/cdata/Li2MnO3.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/cdata/Pentacene.xtl` & `pyemaps-1.0.4/cdata/Pentacene.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/cdata/SiAlONa.xtl` & `pyemaps-1.0.4/cdata/SiAlONa.xtl`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/crystals.py` & `pyemaps-1.0.4/crystals.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 and calculations.
 
 """
 
 from enum import Enum
 import os
 import json
-from tkinter import N
+# from tkinter import N
     
 import numpy as np
 from numpy import asfortranarray as farray
 
 from .errors import *
 from .fileutils import *
```

### Comparing `pyemaps-1.0.3/ddiffs.py` & `pyemaps-1.0.4/ddiffs.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/diffract/__init__.py` & `pyemaps-1.0.4/diffract/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/diffract/bloch_dec.py` & `pyemaps-1.0.4/diffract/bloch_dec.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,68 +379,69 @@
             sn2 = '{0: < #06d}'. format(int(net2))
             st1 = '{0: < #016.10f}'. format(float(t1))
             st2 = '{0: < #016.10f}'. format(float(t2))
             st3 = '{0: < #016.7g}'. format(float(t3))
 
             print(f"{sn1}{sn2}{st1}{st2}{st3}")   
 
-    def getBeams(self, bPrint=False):
-        '''
-        Prints selected beams for current dynamic diffraction simulation 
-        session marked by 
-        `beginBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.beginBloch>`_
-        and `endBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.endBloch>`_.
+    # def getBeams(self, bPrint=False):
+    #     '''
+    #     Prints selected beams for current dynamic diffraction simulation 
+    #     session marked by 
+    #     `beginBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.beginBloch>`_
+    #     and `endBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.endBloch>`_.
         
-        This information is available right after beginBloch call.
+    #     This information is available right after beginBloch call.
 
-        :param bPrint: whether to print selected beams info on standard output
-        :type bPrint: bool, optional, default `False`
+    #     :param bPrint: whether to print selected beams info on standard output
+    #     :type bPrint: bool, optional, default `False`
 
-        :return: The number of selected beams and the selected beams list in Miller indexes.
-        :rtype: a python tuple.
+    #     :return: The number of selected beams and the selected beams list in Miller indexes.
+    #     :rtype: a python tuple.
 
-        '''    
-        nmidx = bloch.get_nbeams()
-        if nmidx <= 0:
-            raise BlochError("failed to retrieve diffracted beams info")
+    #     '''    
+    #     nmidx = bloch.get_nbeams()
+    #     if nmidx <= 0:
+    #         raise BlochError("failed to retrieve diffracted beams info")
 
-        ev = farray(np.zeros((3, nmidx), dtype=int))
-        ev, ret = bloch.getbeams(ev)
+    #     ev = farray(np.zeros((3, nmidx), dtype=int))
+    #     ev, ret = bloch.getbeams(ev)
 
-        if ret != 0:
-            raise BlochError("failed to retrieve incidental beams info")
+    #     if ret != 0:
+    #         raise BlochError("failed to retrieve incidental beams info")
 
-        evv = np.transpose(ev) 
+    #     evv = np.transpose(ev) 
         
-        if bPrint:
-            shkl = "h   K   l"
-            print(f"{shkl:^12}")
+    #     if bPrint:
+    #         shkl = "h   K   l"
+    #         print(f"{shkl:^12}")
 
-            for e in evv:
-                h,k,l = e
-                sh = '{0: < #04d}'. format(int(h))
-                sk = '{0: < #04d}'. format(int(k))
-                sl = '{0: < #04d}'. format(int(l))
+    #         for e in evv:
+    #             h,k,l = e
+    #             sh = '{0: < #04d}'. format(int(h))
+    #             sk = '{0: < #04d}'. format(int(k))
+    #             sl = '{0: < #04d}'. format(int(l))
 
-                print(f"{sh}{sk}{sl}") 
+    #             print(f"{sh}{sk}{sl}") 
 
-        return nmidx, evv  
+    #     return nmidx, evv  
      
 # ----------------deprecated and folded into getSCMatrix call----------------
     # def getEigen(self, ib_coords=(0,0)):
     #     '''
     #     Returns eigen values for given sampling point.
     #     It must be called during a dynamic diffraction simulation session
     #     marked by
     #     `beginBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.beginBloch>`_ and 
     #     `endBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.endBloch>`_.   
     #     :param ib_coords: Sampling point coordinates tuple
     #     :type ib_coords: tuple, optional, default (0,0)
     #     :return: a list of complex eigen values at sampling point location
     #     :rtype: numpy.ndarray
+
     #     Example of the eigen vales:
     #     .. code-block:: console
     #         Eigen values at: (0, 0):
     #         [ 0.04684002-0.00218389j -0.2064669 -0.00147516j -0.30446348+0.00055009j
     #         -0.27657617+0.00023512j -0.2765751 +0.00023515j  0.00539041-0.00382443j
     #         -0.535879  -0.00023585j -0.5612881 +0.00045343j -0.55369247+0.00026236j
     #         -0.55368818+0.00026249j -0.19093572+0.00066419j -0.1550311 +0.00045471j
@@ -470,38 +471,53 @@
                     rvec = (0.0,0.0,0.0)
                     ):
         '''
         
         Obtains scattering matrix at a given sampling point. To get a list of sampling 
         points used in this dynamic simulation session, call 
         `printIBDetails <pyemaps.crystals.html#pyemaps.crystals.Crystal.printIBDetails>`_
-        after `beginBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.beginBloch>`_
+        after `beginBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.beginBloch>`_.
+        In addition to the scattering matrix, it also generates associated eigen values
+        and diffracted beams.
         
         This call must be made during a dynamic simulation session marked by
         `beginBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.beginBloch>`_ and   
-        `endBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.endBloch>`_
+        `endBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.endBloch>`_.
 
-        :param ib_coords: Sampling point coordinates tuple
+        :param ib_coords: Sampling point coordinates tuple.
         :type ib_coords: tuple, optional, defaults to (0, 0)
 
-        :param thickness: Sample thickness
+        :param thickness: Sample thickness.
         :type thickness: int, optional, defaults to 200
 
-        :param rvec: R vector shifting atom coordinates in crystal, each value between 0.0 and 1.0
+        :param rvec: R vector shifting atom coordinates in crystal, each value between 0.0 and 1.0.
         :type rvec: tuple of 3 floats, optional, defaults to (0.0,0.0,0.0)
 
-        :return: 2D scattering matrix size and the complex scattering matrix and its associated eigen values.
+        :return: scattering matrix size; scattering matrix; eigen values; diffracted beams.
         :rtype: a tuple. 
 
         Default values for sample_thickness:
         
         ::
 
             DEF_THICKNESS[0] = 200
 
+        Example of the eigen vales:
+
+        .. code-block:: console
+
+            Eigen values at: (0, 0):
+            [ 0.04684002-0.00218389j -0.2064669 -0.00147516j -0.30446348+0.00055009j
+            -0.27657617+0.00023512j -0.2765751 +0.00023515j  0.00539041-0.00382443j
+            -0.535879  -0.00023585j -0.5612881 +0.00045343j -0.55369247+0.00026236j
+            -0.55368818+0.00026249j -0.19093572+0.00066419j -0.1550311 +0.00045471j
+            -0.15503166+0.00045471j -0.58842399-0.00202841j -0.67850191+0.00042728j
+            -0.72713566+0.00060655j -0.70972681+0.00052279j -0.72092338+0.0005903j
+            -0.72093237+0.00059052j -0.64608335-0.0001983j  -0.64607544-0.00019853j]
+
         '''
 
         #  validate the input values
         if ib_coords is None or len(ib_coords) != 2 or not all(isinstance(v, int) for v in ib_coords):  
             raise BlochError("Invalid incident beam coordinates input, must be tuple of two integers2")   
 
         if sample_thickness is None or not isinstance(sample_thickness, int):
@@ -514,19 +530,20 @@
         scmdim, RET = bloch.compute_scm([ib_coords[0], ib_coords[1]])
         
         if RET != 0 or scmdim <= 0:
             raise BlochError("Error finding corresponding scattering matrix")
 
         scm = farray(np.zeros((scmdim, scmdim)), dtype=np.complex64)
         ev = farray(np.zeros(scmdim), dtype=np.complex64)
-        scm, ev, ret = bloch.getscm(sample_thickness, rvec, scm, ev)
+        bms = farray(np.zeros((3, scmdim), dtype=int))
+        scm, ev, bms, ret = bloch.getscm(sample_thickness, rvec, scm, ev, bms)
         if ret != 0:
             raise BlochError('Error retieving scattering matrix, input matrix dimension too small, use printIBDetails to find extact dimentsion')
 
-        return scmdim, scm, ev
+        return scmdim, scm, ev, np.transpose(bms)
 
     def endBloch(self):
        """
        Clean up Bloch module. This function follows 
         `beginBloch <pyemaps.crystals.html#pyemaps.crystals.Crystal.beginBloch>`_
        to mark the end of a dynamic simulation session.
 
@@ -645,15 +662,15 @@
                 
 
     target.beginBloch = beginBloch
     target._getBlochFN = _getBlochFN
 
     # ---These calls must be between beginBloch and endBloch calls
     target.printIBDetails = printIBDetails
-    target.getBeams = getBeams
+    # target.getBeams = getBeams     <-------deprecate
     target.getSCMatrix = getSCMatrix
     target.getBlochImages = getBlochImages
     # ---These calls must be between beginBloch and endBloch calls
 
     target.endBloch = endBloch
 
     target.generateBloch = generateBloch
```

### Comparing `pyemaps-1.0.3/diffract/csf_dec.py` & `pyemaps-1.0.4/diffract/csf_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/diffract/dif_dec.py` & `pyemaps-1.0.4/diffract/dif_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/diffract/dpgen_dec.py` & `pyemaps-1.0.4/diffract/dpgen_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/diffract/mxtal_dec.py` & `pyemaps-1.0.4/diffract/mxtal_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/diffract/powder_dec.py` & `pyemaps-1.0.4/diffract/powder_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/diffract/stereo_dec.py` & `pyemaps-1.0.4/diffract/stereo_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/display.py` & `pyemaps-1.0.4/display.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/ediom/ediom.py` & `pyemaps-1.0.4/ediom/ediom.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/ediom/ediom_dec.py` & `pyemaps-1.0.4/ediom/ediom_dec.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/emcontrols.py` & `pyemaps-1.0.4/emcontrols.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/errors.py` & `pyemaps-1.0.4/errors.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/fileutils.py` & `pyemaps-1.0.4/fileutils.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/kdiffs.py` & `pyemaps-1.0.4/kdiffs.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/license.txt` & `pyemaps-1.0.4/license.txt`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/pyemaps.egg-info/PKG-INFO` & `pyemaps-1.0.4/pyemaps.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: pyemaps
-Version: 1.0.3
-Summary: UNKNOWN
+Version: 1.0.4
 Home-page: https://www.emlabsolutions.com
 Author: EMLab Solutions, Inc.
 Author-email: support@emlabsoftware.com
-License: UNKNOWN
 Keywords: Transmission,Electron,Diffraction,Simulation,Crystallography,Python
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: license.txt
 License-File: COPYING
 
 Check our full [pyemaps documentation](https://emlab-solutions.github.io/pyemaps) for latest updates.
-
```

### Comparing `pyemaps-1.0.3/pyemaps.egg-info/SOURCES.txt` & `pyemaps-1.0.4/pyemaps.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/ediom/refine.cpp
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/ediom/simplxc.cpp
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/ediom/symmetry.cpp
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/asf.f90
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/atom.f
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/bloch.f90
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/bloch_mem.f90
+C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/cbloch.f90
+C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/cdpgen.f90
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/crystal_mem.f90
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/csf.f90
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/csf_types.f90
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/diff_memalloc.f90
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/diff_types.f90
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/diffract.f90
 C:/Users/sharon/dev_space/pyemaps_root/pyemaps/emaps/dp_gen.f90
```

### Comparing `pyemaps-1.0.3/samples/al.img` & `pyemaps-1.0.4/samples/al.img`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/samples/al_db.bin` & `pyemaps-1.0.4/samples/al_db.bin`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/samples/al_ediom.py` & `pyemaps-1.0.4/samples/al_ediom.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/samples/powder.py` & `pyemaps-1.0.4/samples/powder.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/samples/si_bloch.py` & `pyemaps-1.0.4/samples/si_bloch.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/samples/si_constructor.py` & `pyemaps-1.0.4/samples/si_constructor.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/samples/si_csf.py` & `pyemaps-1.0.4/samples/si_csf.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/samples/si_dif.py` & `pyemaps-1.0.4/samples/si_dif.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/samples/si_dpgen.py` & `pyemaps-1.0.4/samples/si_dpgen.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/samples/si_pyemaps.py` & `pyemaps-1.0.4/samples/si_pyemaps.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/samples/si_rawblochimgs.py` & `pyemaps-1.0.4/samples/si_rawblochimgs.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/samples/si_stereo.py` & `pyemaps-1.0.4/samples/si_stereo.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/scattering/__init__.py` & `pyemaps-1.0.4/scattering/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/setup.cfg` & `pyemaps-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/setup.py` & `pyemaps-1.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,46 +25,65 @@
 mod_name = "emaps"
 
 MKLROOT = os.getenv('MKLROOT')
 IFORTROOT = os.getenv('IFORTROOT')
 
 dpgen_cobj = 'write_dpbin.o'
 
-# removing 4R8 option - returning to 4 bytes real
-# compile_args=['-Qm64',
-#               '-WB',
-#               '-heap-arrays',
-#             #   '-Qopenmp',
-#             #   '-Qopenmp-simd',
-#               '-GS', 
-#               '-4R8',
-#               '-fpp',
-#               '-warn:nointerfaces',
-#               '-O2', #this option does not work with -fast
-#               '-libs:static',
-#               '-MT',
-#               '-assume:buffered_io',
-#               '-traceback',
-#             #   '-align:array32byte',
-#             #   '-Qparallel',
-#             #   '-Qopt-report:2',
-#               '-c']
-
+compile_args_debug=['-Qm64',
+                    '-Od',
+              '-WB',
+              '-heap-arrays:1024',
+              '-Qopenmp',
+              '-Qmkl',
+            #   '-Qopenmp-simd',
+            #   '-GS:partial', 
+              '-fpp',
+              '-warn:all',
+            #   '-O2', #this option does not work with -fast
+            #   '-libs:static',
+            #   '-MT',
+            #   '-assume:buffered_io',
+            #   '-traceback',
+            #   '-check:all',
+            #   '-align:array32byte',
+            #   '-Qparallel',
+            #   '-Qopt-report:2',
+              '-c']
+# --------------- production options--------------
 compile_args=['-Qm64',
               '-WB',
-              '-heap-arrays',
-              '-GS', 
+              '-heap-arrays:1024',
+              '-Qopenmp',
+              '-Qmkl',
+              '-GS:partial', 
               '-fpp',
-              '-warn:nointerfaces',
+              '-warn:all',
               '-O2', #this option does not work with -fast
               '-libs:static',
               '-MT',
               '-assume:buffered_io',
-            #   '-traceback',
               '-c']
+
+# --------debugging options-----------
+# compile_args=['-Qm64',
+#               '-WB',
+#               '-heap-arrays:1024',
+#               '-check:all',
+#               'Qfp-stack-check',
+#               '-Qopenmp',
+#               '-GS:partial', 
+#               '-fpp',
+#               '-warn:nointerfaces',
+#             #   '-O2', #this option does not work with -fast
+#             #   '-libs:static',
+#               '-MT',
+#               '-assume:buffered_io',
+#               '-traceback',
+#               '-c']
               
 compile_args_lin= ['-m64',
                    '-WB', 
                    '-qopenmp', 
                    '-qmkl', 
                    '-heap-arrays', 
 	               '-r8', 
@@ -110,23 +129,25 @@
             'readutils.f',
             'sfsub.f90', 
             'spgroup.f90', 
             'lafit.f90'
             ]
 
 bloch_files = ['zg.f90',
+               'cbloch.f90',
                'bloch_mem.f90',
                'bloch.f90'
               ]
 stereo_files = ['stereo.f90']
 
 mxtal_files = ['mxtal_mem.f90',
                'mxtal.f90']
 
-dpgen_files =['dp_types.f90',
+dpgen_files =['cdpgen.f90',
+              'dp_types.f90',
 			  'dp_gen.f90'
              ]
 
 csf_files =['csf_types.f90',
 			  'csf.f90'
             ]
 
@@ -175,19 +196,22 @@
     for sf in ediomSRCFiles:
         src_list.append(os.path.join(ediom_dir, sf))
     print(f'Ediom source file list: {src_list}')
     # exit()
     return src_list   
    
 def get_ediom_includes():
-    
+    #  for ccompiler cl arguement too long issue
+    # see https://github.com/pypa/setuptools/pull/3775/commits/dd03b731045d5bb0b47648554f9a1a7429ef306a
+    # temporary fix
     import numpy as np
     from sysconfig import get_paths
     
     includeDirs=[np.get_include()]
+    # python's include
     includeDirs.append(get_paths()['include'])
     includeDirs.append(get_ediom_srcdir())
 
     return includeDirs
 
 def get_ediom_libs():
     from sysconfig import get_paths
@@ -361,27 +385,28 @@
     return out
 
 def get_library_dirs():
     
     import platform
 
     lib_folder = ''
+    mkl_folder = 'intel64'
 
     osname = platform.platform().lower()
     print(f'OS name found: {osname}')
     if  'windows' in osname:
         lib_folder = 'intel64_win'
     elif 'linux' in osname:
         lib_folder = 'intel64'
     else:
         raise Exception('Unsupported OS')
 
     libdir = []
     libdir.append(os.path.join(IFORTROOT, 'compiler', 'lib', lib_folder)) #intel openmp libdir
-    libdir.append(os.path.join(MKLROOT, 'lib', lib_folder))
+    libdir.append(os.path.join(MKLROOT, 'lib', mkl_folder))
     
     return libdir
 
 def get_include_dirs():
     # pass
     incl = []
     incl.append(get_emaps_srcdir())
@@ -401,15 +426,15 @@
 
     libs.insert(0, lapack_lib)
     return libs
 
 def get_compiler_args():
     import sys
     if sys.platform == 'win32': 
-        return compile_args
+        return compile_args if pyemaps_debug == 0 else compile_args_debug
     elif sys.platform == 'linux':
         return compile_args_lin
     else:
         raise Exception('The OS is not supported')
 
 def get_install_requires():
     import sys
@@ -424,16 +449,14 @@
         install_reqs += ['intel-fortran-rt == 2022.1.0',
                          'mkl == 2022.1.0']
         return install_reqs
     else:
         raise Exception('The OS is not supported')
     
 def get_emaps_macros():
-    # print(f'setup.py: build_type: {build_type}')
-    # exit()
     
     if build_type != 'uiuc' and build_type != 'full' and build_type != 'free':
         raise ValueError("Error: build type not specified")
 
     def_list = [('NPY_NO_DEPRECATED_API','NPY_1_7_API_VERSION')]
     
     undef_list = []
@@ -455,22 +478,28 @@
 
     if pyemaps_debug != 0:
         # print(f'Build is debug build: {pyemaps_debug}')
         def_list.append(('__BDEBUG__', 1))
     else:
         # print(f'Build is not a debug build: {pyemaps_debug}')
         undef_list.append('__BDEBUG__')
+        undef_list.append('__INIT0__')
     
     # print(f'defundef list: {def_list}, {undef_list}')
     # exit()
     return [def_list, undef_list]
     
 # ------------------- must set this before build -------------------
-pyemaps_build_defs, pyemaps_build_undefs= get_emaps_macros()
 
+# from distutils import ccompiler
+# cc = ccompiler.new_compiler()
+# cc.set_include_dirs([])
+
+
+pyemaps_build_defs, pyemaps_build_undefs= get_emaps_macros()
 pyemaps_dif = Extension("pyemaps.diffract.emaps",
         sources                = get_diffract_sources(),
         extra_f90_compile_args     = get_compiler_args(),
         define_macros          = pyemaps_build_defs,
         undef_macros           = pyemaps_build_undefs,
         extra_link_args        =["-static", ],
         libraries              = get_libraries(),
@@ -509,15 +538,14 @@
             sources                 =get_ediom_sources(),
             extra_objects           =[],
             include_dirs            =get_ediom_includes(),
             library_dirs            =get_ediom_libs(),
             libraries               =[],
             define_macros           = pyemaps_build_defs,
             undef_macros            = pyemaps_build_undefs,
-            extra_compile_args      =[],
             extra_link_args         =[],
             swig_opts               =['-python']
 )
 
 def get_version(f):
     version = {}
     with open(f + ".py") as fp:
```

### Comparing `pyemaps-1.0.3/spg/__init__.py` & `pyemaps-1.0.4/spg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemaps-1.0.3/spg/spg_dec.py` & `pyemaps-1.0.4/spg/spg_dec.py`

 * *Files identical despite different names*

