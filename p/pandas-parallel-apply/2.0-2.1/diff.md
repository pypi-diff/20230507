# Comparing `tmp/pandas-parallel-apply-2.0.tar.gz` & `tmp/pandas-parallel-apply-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-parallel-apply-2.0.tar", last modified: Fri Oct  7 07:27:19 2022, max compression
+gzip compressed data, was "pandas-parallel-apply-2.1.tar", last modified: Sun May  7 19:22:17 2023, max compression
```

## Comparing `pandas-parallel-apply-2.0.tar` & `pandas-parallel-apply-2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-10-07 07:27:19.054398 pandas-parallel-apply-2.0/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      483 2022-10-07 06:43:13.000000 pandas-parallel-apply-2.0/LICENSE
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2618 2022-10-07 07:27:19.054398 pandas-parallel-apply-2.0/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2308 2022-10-07 07:21:07.000000 pandas-parallel-apply-2.0/README.md
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-10-07 07:27:19.054398 pandas-parallel-apply-2.0/pandas_parallel_apply/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      157 2022-10-07 07:04:34.000000 pandas-parallel-apply-2.0/pandas_parallel_apply/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1711 2022-10-07 07:15:33.000000 pandas-parallel-apply-2.0/pandas_parallel_apply/data_frame_parallel.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3739 2022-10-07 07:16:19.000000 pandas-parallel-apply-2.0/pandas_parallel_apply/groupby_parallel.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2713 2022-10-07 07:10:34.000000 pandas-parallel-apply-2.0/pandas_parallel_apply/logger.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      933 2022-10-07 07:15:40.000000 pandas-parallel-apply-2.0/pandas_parallel_apply/series_parallel.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1503 2022-10-07 07:17:07.000000 pandas-parallel-apply-2.0/pandas_parallel_apply/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-10-07 07:27:19.054398 pandas-parallel-apply-2.0/pandas_parallel_apply.egg-info/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2618 2022-10-07 07:27:18.000000 pandas-parallel-apply-2.0/pandas_parallel_apply.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      553 2022-10-07 07:27:18.000000 pandas-parallel-apply-2.0/pandas_parallel_apply.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2022-10-07 07:27:18.000000 pandas-parallel-apply-2.0/pandas_parallel_apply.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       25 2022-10-07 07:27:18.000000 pandas-parallel-apply-2.0/pandas_parallel_apply.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       22 2022-10-07 07:27:18.000000 pandas-parallel-apply-2.0/pandas_parallel_apply.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2022-10-07 07:27:19.054398 pandas-parallel-apply-2.0/setup.cfg
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1842 2022-10-07 07:26:32.000000 pandas-parallel-apply-2.0/setup.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-10-07 07:27:19.054398 pandas-parallel-apply-2.0/test/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      554 2022-10-07 07:22:03.000000 pandas-parallel-apply-2.0/test/test_apply_df.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      480 2022-10-07 07:21:28.000000 pandas-parallel-apply-2.0/test/test_apply_df_col.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1964 2022-10-07 07:24:37.000000 pandas-parallel-apply-2.0/test/test_apply_df_groupby.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-05-07 19:22:17.121851 pandas-parallel-apply-2.1/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      483 2023-05-04 05:18:15.000000 pandas-parallel-apply-2.1/LICENSE
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3978 2023-05-07 19:22:17.121851 pandas-parallel-apply-2.1/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3700 2023-05-07 19:20:31.000000 pandas-parallel-apply-2.1/README.md
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-05-07 19:22:17.121851 pandas-parallel-apply-2.1/pandas_parallel_apply/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      157 2023-05-04 05:18:15.000000 pandas-parallel-apply-2.1/pandas_parallel_apply/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1788 2023-05-04 06:57:52.000000 pandas-parallel-apply-2.1/pandas_parallel_apply/data_frame_parallel.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3711 2023-05-04 06:57:52.000000 pandas-parallel-apply-2.1/pandas_parallel_apply/groupby_parallel.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3230 2023-05-04 06:57:31.000000 pandas-parallel-apply-2.1/pandas_parallel_apply/logger.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      974 2023-05-04 06:57:52.000000 pandas-parallel-apply-2.1/pandas_parallel_apply/series_parallel.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2139 2023-05-04 06:57:52.000000 pandas-parallel-apply-2.1/pandas_parallel_apply/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-05-07 19:22:17.121851 pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3978 2023-05-07 19:22:17.000000 pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      572 2023-05-07 19:22:17.000000 pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2023-05-07 19:22:17.000000 pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       71 2023-05-07 19:22:17.000000 pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       22 2023-05-07 19:22:17.000000 pandas-parallel-apply-2.1/pandas_parallel_apply.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2023-05-07 19:22:17.121851 pandas-parallel-apply-2.1/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1830 2023-05-07 19:21:47.000000 pandas-parallel-apply-2.1/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-05-07 19:22:17.121851 pandas-parallel-apply-2.1/test/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      562 2023-05-04 06:58:51.000000 pandas-parallel-apply-2.1/test/test_apply_df.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      502 2023-05-04 06:57:31.000000 pandas-parallel-apply-2.1/test/test_apply_df_col.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2041 2023-05-04 06:57:31.000000 pandas-parallel-apply-2.1/test/test_apply_df_groupby.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      553 2023-05-04 06:57:31.000000 pandas-parallel-apply-2.1/test/test_utils.py
```

### Comparing `pandas-parallel-apply-2.0/PKG-INFO` & `pandas-parallel-apply-2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,164 +1,232 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7061 6e64  : 2.1.Name: pand
-00000020: 6173 2d70 6172 616c 6c65 6c2d 6170 706c  as-parallel-appl
-00000030: 790a 5665 7273 696f 6e3a 2032 2e30 0a53  y.Version: 2.0.S
-00000040: 756d 6d61 7279 3a20 5772 6170 7065 7220  ummary: Wrapper 
-00000050: 666f 7220 6466 2061 6e64 2064 665b 636f  for df and df[co
-00000060: 6c5d 2e61 7070 6c79 2070 6172 616c 6c65  l].apply paralle
-00000070: 6c69 7a65 640a 486f 6d65 2d70 6167 653a  lized.Home-page:
-00000080: 2068 7474 7073 3a2f 2f67 6974 6c61 622e   https://gitlab.
-00000090: 636f 6d2f 6d69 6861 6963 7269 7374 6961  com/mihaicristia
-000000a0: 6e70 6972 7675 2f70 616e 6461 732d 7061  npirvu/pandas-pa
-000000b0: 7261 6c6c 656c 2d61 7070 6c79 0a4c 6963  rallel-apply.Lic
-000000c0: 656e 7365 3a20 5754 4650 4c0a 506c 6174  ense: WTFPL.Plat
-000000d0: 666f 726d 3a20 554e 4b4e 4f57 4e0a 5265  form: UNKNOWN.Re
-000000e0: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
-000000f0: 3d33 2e38 0a44 6573 6372 6970 7469 6f6e  =3.8.Description
-00000100: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
-00000110: 6578 742f 6d61 726b 646f 776e 0a4c 6963  ext/markdown.Lic
-00000120: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
-00000130: 5345 0a0a 2320 7061 6e64 6173 2d70 6172  SE..# pandas-par
-00000140: 616c 6c65 6c2d 6170 706c 790a 0a50 6172  allel-apply..Par
-00000150: 616c 6c65 6c20 7772 6170 7065 7273 2066  allel wrappers f
-00000160: 6f72 2060 6466 2e61 7070 6c79 2866 6e29  or `df.apply(fn)
-00000170: 602c 2060 6466 5b63 6f6c 5d2e 6170 706c  `, `df[col].appl
-00000180: 7928 666e 2960 2c20 6073 6572 6965 732e  y(fn)`, `series.
-00000190: 6170 706c 7928 666e 2960 2061 6e64 2060  apply(fn)` and `
-000001a0: 6466 2e67 726f 7570 6279 285b 636f 6c73  df.groupby([cols
-000001b0: 5d29 2e61 7070 6c79 2866 6e29 6020 7769  ]).apply(fn)` wi
-000001c0: 7468 2074 7164 6d20 696e 636c 7564 6564  th tqdm included
-000001d0: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-000001e0: 6e0a 0a60 7069 7020 696e 7374 616c 6c20  n..`pip install 
-000001f0: 7061 6e64 6173 2d70 6172 616c 6c65 6c2d  pandas-parallel-
-00000200: 6170 706c 7960 0a0a 2323 2045 7861 6d70  apply`..## Examp
-00000210: 6c65 730a 5365 6520 6065 7861 6d70 6c65  les.See `example
-00000220: 732f 6020 666f 7220 7573 6167 6520 6f6e  s/` for usage on
-00000230: 2073 6f6d 6520 6475 6d6d 7920 6461 7461   some dummy data
-00000240: 6672 616d 6520 616e 6420 7365 7269 6573  frame and series
-00000250: 2e0a 0a23 2320 5573 6167 650a 0a23 2323  ...## Usage..###
-00000260: 2041 7070 6c79 206f 6e20 6561 6368 2072   Apply on each r
-00000270: 6f77 206f 6620 6120 6461 7461 6672 616d  ow of a datafram
-00000280: 650a 0a60 6466 2e61 7070 6c79 2866 6e29  e..`df.apply(fn)
-00000290: 6020 2d3e 2060 4461 7461 4672 616d 6550  ` -> `DataFrameP
-000002a0: 6172 616c 6c65 6c28 6466 2c20 6e5f 636f  arallel(df, n_co
-000002b0: 7265 733a 2069 6e74 203d 204e 6f6e 652c  res: int = None,
-000002c0: 2070 6261 723a 2062 6f6f 6c20 3d20 5472   pbar: bool = Tr
-000002d0: 7565 292e 6170 706c 7928 666e 2960 0a0a  ue).apply(fn)`..
-000002e0: 2323 2320 4170 706c 7920 6f6e 2061 2063  ### Apply on a c
-000002f0: 6f6c 756d 6e20 6f66 2061 2064 6174 6166  olumn of a dataf
-00000300: 7261 6d65 2061 6e64 2072 6574 7572 6e20  rame and return 
-00000310: 7468 6520 5365 7269 6573 0a60 6466 5b63  the Series.`df[c
-00000320: 6f6c 5d2e 6170 706c 7928 666e 2c20 6178  ol].apply(fn, ax
-00000330: 6973 3d31 2960 202d 3e20 6044 6174 6146  is=1)` -> `DataF
-00000340: 7261 6d65 5061 7261 6c6c 656c 2864 662c  rameParallel(df,
-00000350: 206e 5f63 6f72 6573 3a20 696e 7420 3d20   n_cores: int = 
-00000360: 4e6f 6e65 2c20 7062 6172 3a20 626f 6f6c  None, pbar: bool
-00000370: 203d 2054 7275 6529 5b63 6f6c 5d2e 6170   = True)[col].ap
-00000380: 706c 7928 666e 2c20 6178 6973 3d31 2960  ply(fn, axis=1)`
-00000390: 0a0a 2323 2320 4170 706c 7920 6f6e 2061  ..### Apply on a
-000003a0: 2073 6572 6965 730a 6073 6572 6965 732e   series.`series.
-000003b0: 6170 706c 7928 666e 2960 202d 3e20 6053  apply(fn)` -> `S
-000003c0: 6572 6965 7350 6172 616c 6c65 6c28 7365  eriesParallel(se
-000003d0: 7269 6573 2c20 6e5f 636f 7265 733a 2069  ries, n_cores: i
-000003e0: 6e74 203d 204e 6f6e 652c 2070 6261 723a  nt = None, pbar:
-000003f0: 2062 6f6f 6c20 3d20 5472 7565 292e 6170   bool = True).ap
-00000400: 706c 7928 666e 2960 0a0a 2323 2320 4772  ply(fn)`..### Gr
-00000410: 6f75 7042 7920 6170 706c 790a 6064 662e  oupBy apply.`df.
-00000420: 6772 6f75 7062 7928 5b63 6f6c 735d 292e  groupby([cols]).
-00000430: 6170 706c 7928 666e 2960 202d 3e20 6044  apply(fn)` -> `D
-00000440: 6174 6146 7261 6d65 5061 7261 6c6c 656c  ataFrameParallel
-00000450: 2864 662c 206e 5f63 6f72 6573 3a20 696e  (df, n_cores: in
-00000460: 7420 3d20 4e6f 6e65 2c20 7062 6172 3a20  t = None, pbar: 
-00000470: 626f 6f6c 203d 2054 7275 6529 2e67 726f  bool = True).gro
-00000480: 7570 6279 285b 636f 6c73 5d29 2e61 7070  upby([cols]).app
-00000490: 6c79 2866 6e29 600a 0a23 2320 4469 7363  ly(fn)`..## Disc
-000004a0: 6c61 696d 6572 730a 0a2d 2054 6869 7320  laimers..- This 
-000004b0: 6973 2061 6e20 6578 7065 7269 6d65 6e74  is an experiment
-000004c0: 616c 2072 6570 6f73 6974 6f72 792e 2049  al repository. I
-000004d0: 7420 6d61 7920 6c65 6164 2074 6f20 756e  t may lead to un
-000004e0: 6578 7065 6374 6564 2062 6568 6176 696f  expected behavio
-000004f0: 7572 2e0a 0a2d 204e 6f74 2061 6c6c 2074  ur...- Not all t
-00000500: 6865 206d 6572 6769 6e67 2073 656d 616e  he merging seman
-00000510: 7469 6373 206f 6620 7061 6e64 6173 2061  tics of pandas a
-00000520: 7265 2073 7570 706f 7274 6564 2e20 5061  re supported. Pa
-00000530: 6e64 6173 2068 6173 2077 6569 7264 2061  ndas has weird a
-00000540: 6e64 2063 6f6d 706c 6578 206d 6574 686f  nd complex metho
-00000550: 6473 206f 6620 636f 6e76 6572 7469 6e67  ds of converting
-00000560: 2061 6e20 6170 706c 7920 7265 7475 726e   an apply return
-00000570: 2e20 466f 7220 6578 616d 706c 652c 2061  . For example, a
-00000580: 2073 6572 6965 7320 6170 706c 7920 6675   series apply fu
-00000590: 6e63 7469 6f6e 206d 6179 2072 6574 7572  nction may retur
-000005a0: 6e20 6120 6461 7461 6672 616d 652c 2061  n a dataframe, a
-000005b0: 2073 6572 6965 732c 2061 2064 6963 742c   series, a dict,
-000005c0: 2061 206c 6973 7420 6574 632e 2041 6c6c   a list etc. All
-000005d0: 206f 6620 7468 6573 6520 6172 6520 636f   of these are co
-000005e0: 6e76 6572 7465 6420 696e 2073 6f6d 6520  nverted in some 
-000005f0: 7370 6563 6966 6963 2077 6179 2e20 536f  specific way. So
-00000600: 6d65 2063 6173 6573 206d 6179 206e 6f74  me cases may not
-00000610: 2062 6520 7375 7070 6f72 7465 640a 0a2d   be supported..-
-00000620: 2047 726f 7570 6279 2061 7070 6c79 2066   Groupby apply f
-00000630: 756e 6374 696f 6e73 2061 7265 202a 2a6d  unctions are **m
-00000640: 7563 682a 2a20 736c 6f77 6572 2074 6861  uch** slower tha
-00000650: 6e20 7468 6569 7220 7365 7269 616c 2076  n their serial v
-00000660: 6172 6961 6e74 2063 7572 7265 6e74 6c79  ariant currently
-00000670: 2e20 5374 696c 6c20 6578 7065 7269 6d65  . Still experime
-00000680: 6e74 696e 6720 7769 7468 2068 6f77 2074  nting with how t
-00000690: 6f20 6d61 6b65 2069 7420 6661 7374 6572  o make it faster
-000006a0: 2e20 4974 206c 6f6f 6b73 2063 6f72 7265  . It looks corre
-000006b0: 6374 2c20 6a75 7374 2031 302d 3130 3078  ct, just 10-100x
-000006c0: 2073 6c6f 7765 7220 666f 7220 736f 6d65   slower for some
-000006d0: 2073 6d61 6c6c 2065 7861 6d70 6c65 732e   small examples.
-000006e0: 204d 6179 2062 6520 6265 7474 6572 2061   May be better a
-000006f0: 7320 6461 7461 6672 616d 6520 6765 7420  s dataframe get 
-00000700: 6269 6767 6572 2e0a 0a2d 2055 7369 6e67  bigger...- Using
-00000710: 2060 6e5f 636f 7265 733d 3060 2077 696c   `n_cores=0` wil
-00000720: 6c20 6361 6c6c 2074 6865 2075 6e64 6572  l call the under
-00000730: 6c79 696e 6720 7061 6e64 6173 2063 6f64  lying pandas cod
-00000740: 6520 6469 7265 6374 6c79 2c20 736f 2074  e directly, so t
-00000750: 6865 2069 6e74 6572 6661 6365 2069 7320  he interface is 
-00000760: 6a75 7374 2061 2077 7261 7070 6572 2e20  just a wrapper. 
-00000770: 5573 696e 6e67 2060 6e5f 636f 7265 733d  Usinng `n_cores=
-00000780: 3160 2077 696c 6c20 6372 6561 7465 2061  1` will create a
-00000790: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
-000007a0: 2070 6f6f 6c20 6f66 206a 7573 7420 3120   pool of just 1 
-000007b0: 636f 7265 2c20 736f 2074 6865 2063 6f64  core, so the cod
-000007c0: 6520 6973 2070 6172 616c 6c65 6c20 2874  e is parallel (t
-000007d0: 6875 7320 6e6f 7420 7275 6e6e 696e 6720  hus not running 
-000007e0: 6f6e 2074 6865 206d 6169 6e20 7072 6f63  on the main proc
-000007f0: 6573 7329 2c20 6275 7420 6d61 7920 6e6f  ess), but may no
-00000800: 7420 7969 656c 6420 6d75 6368 2073 7065  t yield much spe
-00000810: 6564 2069 6d70 726f 7665 6d65 6e74 2c20  ed improvement, 
-00000820: 6578 6365 7074 2066 6f72 206e 6f74 2062  except for not b
-00000830: 6c6f 636b 696e 6720 7468 6520 6d61 696e  locking the main
-00000840: 2070 726f 6365 7373 2e20 4d61 7920 6265   process. May be
-00000850: 2075 7365 6675 6c20 696e 2073 6f6d 6520   useful in some 
-00000860: 4755 4920 6170 7073 0a0a 2d20 5765 2072  GUI apps..- We r
-00000870: 6563 6f6d 6d65 6e64 206f 6e6c 7920 6f62  ecommend only ob
-00000880: 6a65 6374 206f 7269 656e 7465 6420 6170  ject oriented ap
-00000890: 7072 6f61 6368 2e20 596f 7520 6361 6e20  proach. You can 
-000008a0: 7573 6520 7468 6520 696e 7465 726e 616c  use the internal
-000008b0: 2060 6170 706c 795f 6f6e 5f64 665f 7061   `apply_on_df_pa
-000008c0: 7261 6c6c 656c 602c 2060 6170 706c 795f  rallel`, `apply_
-000008d0: 6f6e 5f64 665f 636f 6c5f 7061 7261 6c6c  on_df_col_parall
-000008e0: 656c 602c 2060 6170 706c 795f 6f6e 5f73  el`, `apply_on_s
-000008f0: 6572 6965 735f 7061 7261 6c6c 656c 602c  eries_parallel`,
-00000900: 2060 6170 706c 795f 6f6e 5f67 726f 7570   `apply_on_group
-00000910: 6279 5f70 6172 616c 6c65 6c60 2c20 6275  by_parallel`, bu
-00000920: 7420 6974 2075 7375 616c 6c79 2061 6464  t it usually add
-00000930: 7320 756e 6e65 6365 7373 6172 7920 636f  s unnecessary co
-00000940: 6d70 6c65 7869 7479 2074 6f20 7468 6520  mplexity to the 
-00000950: 636f 6465 2e0a 0a2d 2059 6f75 2063 616e  code...- You can
-00000960: 2069 676e 6f72 6520 7468 6520 606e 5f63   ignore the `n_c
-00000970: 6f72 6573 6020 6172 6775 6d65 6e74 2074  ores` argument t
-00000980: 6f20 616c 6c20 7468 6520 636f 6e73 7472  o all the constr
-00000990: 7563 746f 7273 2e20 4966 206e 6f74 2073  uctors. If not s
-000009a0: 6574 2c20 6974 2077 696c 6c20 6465 6661  et, it will defa
-000009b0: 756c 7420 746f 2074 6865 2065 6e76 6972  ult to the envir
-000009c0: 6f6e 6d65 6e74 2076 6172 6961 626c 6520  onment variable 
-000009d0: 6050 414e 4441 535f 5041 5241 4c4c 454c  `PANDAS_PARALLEL
-000009e0: 5f41 5050 4c59 5f4e 5f43 4f52 4553 602e  _APPLY_N_CORES`.
-000009f0: 2049 6620 7468 6973 2069 7320 616c 736f   If this is also
-00000a00: 206e 6f74 2073 6574 2c20 6974 2064 6566   not set, it def
-00000a10: 6175 6c74 7320 746f 2030 2028 7365 7269  aults to 0 (seri
-00000a20: 616c 2061 7070 6c79 292e 0a0a 5468 6174  al apply)...That
-00000a30: 2773 2061 6c6c 2e0a 0a0a                 's all....
+00000000: 2320 7061 6e64 6173 2d70 6172 616c 6c65  # pandas-paralle
+00000010: 6c2d 6170 706c 790a 0a3c 6469 7620 616c  l-apply..<div al
+00000020: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000030: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000040: 2f67 6974 6c61 622e 636f 6d2f 6d65 6568  /gitlab.com/meeh
+00000050: 6169 2f70 616e 6461 732d 7061 7261 6c6c  ai/pandas-parall
+00000060: 656c 2d61 7070 6c79 2f2d 2f62 6c6f 622f  el-apply/-/blob/
+00000070: 6d61 696e 2f4c 4943 454e 5345 223e 0a20  main/LICENSE">. 
+00000080: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000090: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000000a0: 2e69 6f2f 6769 746c 6162 2f6c 6963 656e  .io/gitlab/licen
+000000b0: 7365 2f6d 6565 6861 692f 7061 6e64 6173  se/meehai/pandas
+000000c0: 2d70 6172 616c 6c65 6c2d 6170 706c 7922  -parallel-apply"
+000000d0: 2061 6c74 3d22 4c69 6365 6e73 6522 2f3e   alt="License"/>
+000000e0: 0a20 203c 2f61 3e0a 2020 3c61 2068 7265  .  </a>.  <a hre
+000000f0: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
+00000100: 6f72 672f 7072 6f6a 6563 742f 7061 6e64  org/project/pand
+00000110: 6173 2d70 6172 616c 6c65 6c2d 6170 706c  as-parallel-appl
+00000120: 792f 223e 0a20 2020 203c 696d 6720 7372  y/">.    <img sr
+00000130: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000140: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+00000150: 2f70 616e 6461 732d 7061 7261 6c6c 656c  /pandas-parallel
+00000160: 2d61 7070 6c79 2220 616c 743d 2250 7950  -apply" alt="PyP
+00000170: 6920 4c61 7465 7374 2052 656c 6561 7365  i Latest Release
+00000180: 222f 3e0a 2020 3c2f 613e 0a3c 2f64 6976  "/>.  </a>.</div
+00000190: 3e0a 0a50 6172 616c 6c65 6c20 7772 6170  >..Parallel wrap
+000001a0: 7065 7273 2066 6f72 2060 6466 2e61 7070  pers for `df.app
+000001b0: 6c79 2866 6e29 602c 2060 6466 5b63 6f6c  ly(fn)`, `df[col
+000001c0: 5d2e 6170 706c 7928 666e 2960 2c20 6073  ].apply(fn)`, `s
+000001d0: 6572 6965 732e 6170 706c 7928 666e 2960  eries.apply(fn)`
+000001e0: 2c20 616e 6420 6064 662e 6772 6f75 7062  , and `df.groupb
+000001f0: 7928 5b63 6f6c 735d 292e 6170 706c 7928  y([cols]).apply(
+00000200: 666e 2960 2c20 7769 7468 2074 7164 6d20  fn)`, with tqdm 
+00000210: 7072 6f67 7265 7373 2062 6172 7320 696e  progress bars in
+00000220: 636c 7564 6564 2e0a 0a23 2320 496e 7374  cluded...## Inst
+00000230: 616c 6c61 7469 6f6e 0a0a 6070 6970 2069  allation..`pip i
+00000240: 6e73 7461 6c6c 2070 616e 6461 732d 7061  nstall pandas-pa
+00000250: 7261 6c6c 656c 2d61 7070 6c79 600a 0a49  rallel-apply`..I
+00000260: 6d70 6f72 7420 7769 7468 3a0a 6060 6070  mport with:.```p
+00000270: 7974 686f 6e0a 6672 6f6d 2070 616e 6461  ython.from panda
+00000280: 735f 7061 7261 6c6c 656c 5f61 7070 6c79  s_parallel_apply
+00000290: 2069 6d70 6f72 7420 4461 7461 4672 616d   import DataFram
+000002a0: 6550 6172 616c 6c65 6c2c 2053 6572 6965  eParallel, Serie
+000002b0: 7350 6172 616c 6c65 6c0a 6060 600a 0a23  sParallel.```..#
+000002c0: 2320 4578 616d 706c 6573 0a53 6565 2060  # Examples.See `
+000002d0: 6578 616d 706c 6573 2f60 2066 6f72 2075  examples/` for u
+000002e0: 7361 6765 206f 6e20 736f 6d65 2064 756d  sage on some dum
+000002f0: 6d79 2064 6174 6166 7261 6d65 7320 616e  my dataframes an
+00000300: 6420 7365 7269 6573 2e0a 0a23 2320 5573  d series...## Us
+00000310: 6167 650a 0a60 6060 7079 7468 6f6e 0a23  age..```python.#
+00000320: 2041 7070 6c79 206f 6e20 6561 6368 2072   Apply on each r
+00000330: 6f77 206f 6620 6120 6461 7461 6672 616d  ow of a datafram
+00000340: 650a 6466 2e61 7070 6c79 2866 6e29 0a23  e.df.apply(fn).#
+00000350: 202d 3e0a 4461 7461 4672 616d 6550 6172   ->.DataFramePar
+00000360: 616c 6c65 6c28 6466 2c20 6e5f 636f 7265  allel(df, n_core
+00000370: 733a 2069 6e74 203d 204e 6f6e 652c 2070  s: int = None, p
+00000380: 6261 723a 2062 6f6f 6c20 3d20 5472 7565  bar: bool = True
+00000390: 292e 6170 706c 7928 666e 290a 0a23 2041  ).apply(fn)..# A
+000003a0: 7070 6c79 206f 6e20 6120 636f 6c75 6d6e  pply on a column
+000003b0: 206f 6620 6120 6461 7461 6672 616d 6520   of a dataframe 
+000003c0: 2872 6574 7572 6e73 2061 2053 6572 6965  (returns a Serie
+000003d0: 7329 0a64 665b 636f 6c5d 2e61 7070 6c79  s).df[col].apply
+000003e0: 2866 6e2c 2061 7869 733d 3129 0a23 202d  (fn, axis=1).# -
+000003f0: 3e0a 4461 7461 4672 616d 6550 6172 616c  >.DataFrameParal
+00000400: 6c65 6c28 6466 2c20 6e5f 636f 7265 733a  lel(df, n_cores:
+00000410: 2069 6e74 203d 204e 6f6e 652c 2070 6261   int = None, pba
+00000420: 723a 2062 6f6f 6c20 3d20 5472 7565 295b  r: bool = True)[
+00000430: 636f 6c5d 2e61 7070 6c79 2866 6e2c 2061  col].apply(fn, a
+00000440: 7869 733d 3129 0a0a 2320 4170 706c 7920  xis=1)..# Apply 
+00000450: 6f6e 2061 2073 6572 6965 730a 7365 7269  on a series.seri
+00000460: 6573 2e61 7070 6c79 2866 6e29 0a23 202d  es.apply(fn).# -
+00000470: 3e20 0a53 6572 6965 7350 6172 616c 6c65  > .SeriesParalle
+00000480: 6c28 7365 7269 6573 2c20 6e5f 636f 7265  l(series, n_core
+00000490: 733a 2069 6e74 203d 204e 6f6e 652c 2070  s: int = None, p
+000004a0: 6261 723a 2062 6f6f 6c20 3d20 5472 7565  bar: bool = True
+000004b0: 292e 6170 706c 7928 666e 290a 0a23 2047  ).apply(fn)..# G
+000004c0: 726f 7570 4279 2061 7070 6c79 0a64 662e  roupBy apply.df.
+000004d0: 6772 6f75 7062 7928 5b63 6f6c 735d 292e  groupby([cols]).
+000004e0: 6170 706c 7928 666e 290a 2320 2d3e 0a44  apply(fn).# ->.D
+000004f0: 6174 6146 7261 6d65 5061 7261 6c6c 656c  ataFrameParallel
+00000500: 2864 662c 206e 5f63 6f72 6573 3a20 696e  (df, n_cores: in
+00000510: 7420 3d20 4e6f 6e65 2c20 7062 6172 3a20  t = None, pbar: 
+00000520: 626f 6f6c 203d 2054 7275 6529 2e67 726f  bool = True).gro
+00000530: 7570 6279 285b 636f 6c73 5d29 2e61 7070  upby([cols]).app
+00000540: 6c79 2866 6e29 0a60 6060 0a0a 2323 2048  ly(fn).```..## H
+00000550: 6f77 2069 7420 776f 726b 730a 0a49 7420  ow it works..It 
+00000560: 7461 6b65 7320 7468 6520 6c65 6e67 7468  takes the length
+00000570: 206f 6620 796f 7572 2064 6174 6166 7261   of your datafra
+00000580: 6d65 2028 6f72 2073 6572 6965 732c 206f  me (or series, o
+00000590: 7220 6772 6f75 7065 7229 203d 204e 2061  r grouper) = N a
+000005a0: 6e64 2074 6865 2060 6e5f 636f 7265 7360  nd the `n_cores`
+000005b0: 2070 726f 7669 6465 6420 746f 2074 6865   provided to the
+000005c0: 2063 6f6e 7374 7275 6374 6f72 7320 284b   constructors (K
+000005d0: 292e 0a49 7420 7468 656e 2073 706c 6974  )..It then split
+000005e0: 7320 7468 6520 6461 7461 6672 616d 6520  s the dataframe 
+000005f0: 696e 204b 2063 6875 6e6b 7320 6f66 204e  in K chunks of N
+00000600: 2f4b 2073 697a 6520 616e 6420 7370 6177  /K size and spaw
+00000610: 6e73 204b 206e 6577 2070 726f 6365 7373  ns K new process
+00000620: 6573 2c20 6561 6368 2070 726f 6365 7373  es, each process
+00000630: 696e 6720 7468 6520 6465 7369 7265 6420  ing the desired 
+00000640: 6368 756e 6b73 2e0a 0a4f 6e6c 7920 726f  chunks...Only ro
+00000650: 772d 7769 7365 2028 7065 7266 6563 7420  w-wise (perfect 
+00000660: 7061 7261 6c6c 656c 6162 6c65 2920 6f70  parallelable) op
+00000670: 6572 6174 696f 6e73 2061 7265 2073 7570  erations are sup
+00000680: 706f 7274 6564 2c20 736f 2060 6466 2e61  ported, so `df.a
+00000690: 7070 6c79 2866 6e2c 2061 7869 733d 3129  pply(fn, axis=1)
+000006a0: 6020 6973 206f 6b61 792c 2062 7574 0a60  ` is okay, but.`
+000006b0: 6466 2e61 7070 6c79 2866 6e2c 2061 7869  df.apply(fn, axi
+000006c0: 733d 3029 6020 6973 206e 6f74 2062 6563  s=0)` is not bec
+000006d0: 6175 7365 2069 7420 6d61 7920 7265 7175  ause it may requ
+000006e0: 6972 6520 726f 7773 2074 6861 7420 6172  ire rows that ar
+000006f0: 6520 6f6e 206f 7468 6572 2077 6f72 6b65  e on other worke
+00000700: 7273 2e0a 0a49 7420 6973 2061 7373 756d  rs...It is assum
+00000710: 6564 2074 6861 7420 6561 6368 2072 6f77  ed that each row
+00000720: 2069 7320 7072 6f63 6573 7365 6420 696e   is processed in
+00000730: 2073 696d 696c 6172 2074 696d 652c 2073   similar time, s
+00000740: 6f20 7468 6520 4e2f 4b20 6368 756e 6b73  o the N/K chunks
+00000750: 2077 696c 6c20 6669 6e69 7368 6520 6d6f   will finishe mo
+00000760: 7265 206f 7220 6c65 7373 2061 7420 7468  re or less at th
+00000770: 6520 7361 6d65 2074 696d 652e 0a0a 2323  e same time...##
+00000780: 2320 4675 7475 7265 2049 6d70 726f 7665  # Future Improve
+00000790: 6d65 6e74 0a0a 4e6f 7420 7375 7070 6f72  ment..Not suppor
+000007a0: 7465 6420 6275 7420 6d61 7920 6265 2069  ted but may be i
+000007b0: 6e74 6572 6573 7469 6e67 3a20 6465 6669  nteresting: defi
+000007c0: 6e65 2061 6c73 6f20 6120 6e75 6d62 6572  ne also a number
+000007d0: 206f 6620 6368 756e 6b73 2028 433e 4b29   of chunks (C>K)
+000007e0: 2c20 736f 2074 6865 2064 6620 6973 2061  , so the df is a
+000007f0: 6374 7561 6c6c 7920 7370 6c69 7420 696e  ctually split in
+00000800: 204e 2f43 2063 6875 6e6b 732c 0a61 6e64   N/C chunks,.and
+00000810: 2074 6865 7365 7320 6172 6520 7061 7373   theses are pass
+00000820: 6564 2075 7369 6e67 2061 2072 6f75 6e64  ed using a round
+00000830: 2d72 6f62 696e 2061 7070 726f 6163 6820  -robin approach 
+00000840: 746f 2074 6865 204b 2070 726f 6365 7373  to the K process
+00000850: 6573 2e20 5269 6768 7420 6e6f 772c 2043  es. Right now, C
+00000860: 3d4b 2c20 736f 2077 6865 6e65 7665 7220  =K, so whenever 
+00000870: 6f6e 6520 7072 6f63 6573 7320 6669 6e69  one process fini
+00000880: 7368 6573 2c0a 6974 2077 696c 6c20 6e6f  shes,.it will no
+00000890: 7420 6265 2061 7373 6967 6e65 6420 616e  t be assigned an
+000008a0: 7920 6d6f 7265 2077 6f72 6b2e 0a0a 2323  y more work...##
+000008b0: 206e 5f63 6f72 6573 2073 656d 616e 7469   n_cores semanti
+000008c0: 6373 0a2d 2060 6e5f 636f 7265 7320 3c20  cs.- `n_cores < 
+000008d0: 2d31 6020 2d3e 2074 6872 6f77 7320 616e  -1` -> throws an
+000008e0: 2065 7272 6f72 0a2d 2060 6e5f 636f 7265   error.- `n_core
+000008f0: 7320 3d3d 202d 3160 202d 3e20 7573 6573  s == -1` -> uses
+00000900: 2060 6370 755f 636f 756e 7428 2960 202d   `cpu_count()` -
+00000910: 2031 2063 6f72 6573 0a2d 2060 6e5f 636f   1 cores.- `n_co
+00000920: 7265 7320 3d3d 2030 6020 2d3e 2075 7365  res == 0` -> use
+00000930: 7320 7365 7269 616c 2f73 7461 6e64 6172  s serial/standar
+00000940: 6420 7061 6e64 6173 2066 756e 6374 696f  d pandas functio
+00000950: 6e73 0a2d 2060 6e5f 636f 7265 7320 3d3d  ns.- `n_cores ==
+00000960: 2031 6020 2d3e 2073 7061 776e 7320 6120   1` -> spawns a 
+00000970: 7369 6e67 6c65 2070 726f 6365 7373 2061  single process a
+00000980: 6c6f 6e67 7369 6465 2074 6865 206d 6169  longside the mai
+00000990: 6e20 6f6e 650a 2d20 606e 5f63 6f72 6573  n one.- `n_cores
+000009a0: 203e 2031 6020 2d3e 2073 7061 6e77 7320   > 1` -> spanws 
+000009b0: 4e20 7072 6f63 6573 7365 7320 616e 6420  N processes and 
+000009c0: 6368 756e 6b73 2074 6865 2064 660a 2d20  chunks the df.- 
+000009d0: 606e 5f63 6f72 6573 203e 2063 7075 5f63  `n_cores > cpu_c
+000009e0: 7075 6e74 2829 6020 2d3e 2074 6872 6f77  punt()` -> throw
+000009f0: 7320 616e 2077 6172 6e69 6e67 0a2d 2060  s an warning.- `
+00000a00: 6e5f 636f 7265 7320 3e20 6c65 6e28 6466  n_cores > len(df
+00000a10: 2960 202d 3e20 6c69 6d69 7473 2074 6f20  )` -> limits to 
+00000a20: 606c 656e 2864 6629 600a 0a4f 6e20 4350  `len(df)`..On CP
+00000a30: 552d 626f 756e 6420 7461 736b 7320 2863  U-bound tasks (c
+00000a40: 616c 6375 6c61 7469 6f6e 7329 2c20 606e  alculations), `n
+00000a50: 5f63 6f72 6573 203d 202d 3160 2069 7320  _cores = -1` is 
+00000a60: 6c69 6b65 6c79 2074 6f20 6265 2066 6173  likely to be fas
+00000a70: 7465 7374 2e20 4f6e 206e 6574 776f 726b  test. On network
+00000a80: 2d62 6f75 6e64 206f 7065 7261 7469 6f6e  -bound operation
+00000a90: 7320 2865 2e67 2e2c 2077 6865 7265 2074  s (e.g., where t
+00000aa0: 6872 6561 6473 206d 6179 2069 6e76 6f6b  hreads may invok
+00000ab0: 6520 6e65 7477 6f72 6b20 6361 6c6c 7329  e network calls)
+00000ac0: 2c0a 7573 696e 6720 6120 7665 7279 2068  ,.using a very h
+00000ad0: 6967 6820 606e 5f63 6f72 6573 6020 7661  igh `n_cores` va
+00000ae0: 6c75 6520 6d61 7920 6265 2062 656e 6566  lue may be benef
+00000af0: 6963 6961 6c2e 0a0a 2323 2044 6973 636c  icial...## Discl
+00000b00: 6169 6d65 7273 0a0a 2d20 5468 6973 2069  aimers..- This i
+00000b10: 7320 616e 2065 7870 6572 696d 656e 7461  s an experimenta
+00000b20: 6c20 7265 706f 7369 746f 7279 2e20 4974  l repository. It
+00000b30: 206d 6179 206c 6561 6420 746f 2075 6e65   may lead to une
+00000b40: 7870 6563 7465 6420 6265 6861 7669 6f75  xpected behaviou
+00000b50: 722e 0a0a 2d20 4e6f 7420 616c 6c20 7468  r...- Not all th
+00000b60: 6520 6d65 7267 696e 6720 7365 6d61 6e74  e merging semant
+00000b70: 6963 7320 6f66 2070 616e 6461 7320 6172  ics of pandas ar
+00000b80: 6520 7375 7070 6f72 7465 642e 2050 616e  e supported. Pan
+00000b90: 6461 7320 6861 7320 7765 6972 6420 616e  das has weird an
+00000ba0: 6420 636f 6d70 6c65 7820 6d65 7468 6f64  d complex method
+00000bb0: 7320 6f66 2063 6f6e 7665 7274 696e 6720  s of converting 
+00000bc0: 616e 2061 7070 6c79 2072 6574 7572 6e2e  an apply return.
+00000bd0: 2046 6f72 2065 7861 6d70 6c65 2c20 6120   For example, a 
+00000be0: 7365 7269 6573 2061 7070 6c79 2066 756e  series apply fun
+00000bf0: 6374 696f 6e20 6d61 7920 7265 7475 726e  ction may return
+00000c00: 2061 2064 6174 6166 7261 6d65 2c20 6120   a dataframe, a 
+00000c10: 7365 7269 6573 2c20 6120 6469 6374 2c20  series, a dict, 
+00000c20: 6120 6c69 7374 2c20 6574 632e 2041 6c6c  a list, etc. All
+00000c30: 206f 6620 7468 6573 6520 6172 6520 636f   of these are co
+00000c40: 6e76 6572 7465 6420 696e 2073 6f6d 6520  nverted in some 
+00000c50: 7370 6563 6966 6963 2077 6179 2e20 536f  specific way. So
+00000c60: 6d65 2063 6173 6573 206d 6179 206e 6f74  me cases may not
+00000c70: 2062 6520 7375 7070 6f72 7465 642e 0a0a   be supported...
+00000c80: 2d20 4772 6f75 7062 7920 6170 706c 7920  - Groupby apply 
+00000c90: 6675 6e63 7469 6f6e 7320 6172 6520 2a2a  functions are **
+00000ca0: 6d75 6368 2a2a 2073 6c6f 7765 7220 7468  much** slower th
+00000cb0: 616e 2074 6865 6972 2073 6572 6961 6c20  an their serial 
+00000cc0: 7661 7269 616e 7420 6375 7272 656e 746c  variant currentl
+00000cd0: 792e 2053 7469 6c6c 2065 7870 6572 696d  y. Still experim
+00000ce0: 656e 7469 6e67 2077 6974 6820 686f 7720  enting with how 
+00000cf0: 746f 206d 616b 6520 6974 2066 6173 7465  to make it faste
+00000d00: 722e 2049 7420 6c6f 6f6b 7320 636f 7272  r. It looks corr
+00000d10: 6563 742c 206a 7573 7420 3130 2d31 3030  ect, just 10-100
+00000d20: 7820 736c 6f77 6572 2066 6f72 2073 6f6d  x slower for som
+00000d30: 6520 736d 616c 6c20 6578 616d 706c 6573  e small examples
+00000d40: 2e20 4d61 7920 6265 2062 6574 7465 7220  . May be better 
+00000d50: 6173 2064 6174 6166 7261 6d65 2067 6574  as dataframe get
+00000d60: 2062 6967 6765 722e 0a0a 2d20 5573 696e   bigger...- Usin
+00000d70: 6720 606e 5f63 6f72 6573 203d 2031 6020  g `n_cores = 1` 
+00000d80: 7769 6c6c 2063 7265 6174 6520 6120 6d75  will create a mu
+00000d90: 6c74 6970 726f 6365 7373 696e 6720 706f  ltiprocessing po
+00000da0: 6f6c 206f 6620 6a75 7374 2031 2063 6f72  ol of just 1 cor
+00000db0: 652c 2073 6f20 7468 6520 636f 6465 2069  e, so the code i
+00000dc0: 7320 7061 7261 6c6c 656c 2028 7468 7573  s parallel (thus
+00000dd0: 206e 6f74 2072 756e 6e69 6e67 206f 6e20   not running on 
+00000de0: 7468 6520 6d61 696e 2070 726f 6365 7373  the main process
+00000df0: 292c 2062 7574 206d 6179 206e 6f74 2079  ), but may not y
+00000e00: 6965 6c64 206d 7563 6820 7370 6565 6420  ield much speed 
+00000e10: 696d 7072 6f76 656d 656e 742c 2065 7863  improvement, exc
+00000e20: 6570 7420 666f 7220 6e6f 7420 626c 6f63  ept for not bloc
+00000e30: 6b69 6e67 2074 6865 206d 6169 6e20 7072  king the main pr
+00000e40: 6f63 6573 732e 204d 6179 2062 6520 7573  ocess. May be us
+00000e50: 6566 756c 2069 6e20 736f 6d65 2047 5549  eful in some GUI
+00000e60: 2061 7070 732e 0a0a 5468 6174 2773 2061   apps...That's a
+00000e70: 6c6c 2e0a                                ll..
```

### Comparing `pandas-parallel-apply-2.0/pandas_parallel_apply/data_frame_parallel.py` & `pandas-parallel-apply-2.1/pandas_parallel_apply/data_frame_parallel.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,44 +6,44 @@
     parallel => DataFrameParallel(df, n_cores)[col_name].apply(f)
 
 Apply on row
 Usage:
     standard => df.apply(f, axis=1)
     parallel => DataFrameParallel(df, n_cores).apply(f, axis=1)
 """
+from functools import partial
+from typing import Callable
 import pandas as pd
 
 from .series_parallel import SeriesParallel
 from .groupby_parallel import GroupByParallel
-from typing import Callable
-from .utils import parallelize_dataframe, get_default_n_cores
-from functools import partial
+from .utils import parallelize_dataframe
 
 
-def apply_on_df(df: pd.DataFrame, f: Callable, pbar: bool = True) -> pd.Series:
+def _apply_on_df(df: pd.DataFrame, f: Callable, pbar: bool = True) -> pd.Series:
     """Apply a function on each row (all possible columns), returning a series"""
     if pbar:
         return df.progress_apply(f, axis=1)
-    else:
-        return df.apply(f, axis=1)
+    return df.apply(f, axis=1)
 
 class DataFrameParallel:
-    def __init__(self, df: pd.DataFrame, n_cores: int = None, pbar: bool = True):
-        if n_cores is None:
-            n_cores = get_default_n_cores()
-
+    """DataFrameParallel implementation"""
+    def __init__(self, df: pd.DataFrame, n_cores: int, pbar: bool = True):
         self.df = df
         self.n_cores = n_cores
         self.pbar = pbar
 
+    # pylint: disable=unused-argument
     def apply(self, func, axis, raw: bool = False, result_type = None, args=(), **kwargs):
+        """Wrapper on top of regular df.apply(fn)"""
         assert axis == 1, "Only axis=1 is supported in parallel df apply"
-        return parallelize_dataframe(self.df, partial(apply_on_df, f=func, pbar=self.pbar), self.n_cores)
+        return parallelize_dataframe(self.df, partial(_apply_on_df, f=func, pbar=self.pbar), self.n_cores)
 
     def groupby(self, *args, **kwargs):
+        """Wrapper on top of regular df.groupby(col)"""
         return GroupByParallel(self.df.groupby(*args, **kwargs), self.n_cores, self.pbar)
 
     def __getitem__(self, x):
         return SeriesParallel(self.df[x], self.n_cores, self.pbar)
 
     def __str__(self) -> str:
         f_str = f"[Parallel DataFrame - {self.n_cores} crores]\n" + self.df.__str__()
```

### Comparing `pandas-parallel-apply-2.0/pandas_parallel_apply/groupby_parallel.py` & `pandas-parallel-apply-2.1/pandas_parallel_apply/groupby_parallel.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,20 @@
     parallel => DataFrameParallel(df, n_cores).groupby([cols]).apply(f)
              => GroupByPrallel(df.groupby[cols], n_cores).apply(f)
 """
 from typing import Callable, List, Union
 from functools import partial
 from pandas.core.groupby.generic import DataFrameGroupBy
 from pandas.core.indexes.multi import MultiIndex
-from multiprocessing import cpu_count
 from tqdm import tqdm
 import pandas as pd
 from pathos.multiprocessing import ProcessingPool as Pool
 import numpy as np
-from .utils import get_default_n_cores
 from .logger import logger
+from .utils import get_n_cores
 
 
 def _groupby_serial_func(data: List, func: Callable, pbar: bool = True) -> List:
     _range = tqdm(data) if pbar else data
     return [func(x) for x in _range]
 
 def _get_multi_index_key(concat_res, key_data):
@@ -30,15 +29,15 @@
         multi_key = n_keys * [key_data[i]]
         counter_key = concat_res[i].index
         new_key = tuple(zip(multi_key, counter_key))
         new_key_data.extend(new_key)
     key_data = MultiIndex.from_tuples(new_key_data)
     return key_data
 
-def chunk_df(df_grouped: DataFrameGroupBy, n_cores: int) -> List[List]:
+def _chunk_df(df_grouped: DataFrameGroupBy, n_cores: int) -> List[List]:
     chunk_size = len(df_grouped) // n_cores + (len(df_grouped) % n_cores != 0)
     key_data = []
     chunked_data = []
     current_chunk = []
     for item in iter(df_grouped):
         key_data.append(item[0])
         current_chunk.append(item[1])
@@ -46,22 +45,22 @@
             chunked_data.append(current_chunk)
             current_chunk = []
     if 0 < len(current_chunk) < chunk_size:
         chunked_data.append(current_chunk)
     assert n_cores == len(chunked_data)
     return key_data, chunked_data
 
-def apply_on_groupby_parallel(df_grouped: DataFrameGroupBy, func: Callable, n_cores: int, pbar: bool = True,
+def _apply_on_groupby_parallel(df_grouped: DataFrameGroupBy, func: Callable, n_cores: int, pbar: bool = True,
                               keep_original_indexes: bool = False) -> Union[pd.DataFrame, pd.Series]:
+    n_cores = get_n_cores(n_cores, df_grouped)
     if n_cores == 0:
         logger.info("n_cores is set to 0, returning serial apply.")
         return df_grouped.apply(func)
 
-    n_cores = min(cpu_count(), len(df_grouped), n_cores)
-    key_data, chunked_data = chunk_df(df_grouped, n_cores)
+    key_data, chunked_data = _chunk_df(df_grouped, n_cores)
 
     # Run the multi-process job
     pool = Pool(n_cores)
     pool_res = pool.map(partial(_groupby_serial_func, func=func, pbar=pbar), chunked_data)
 
     # Concatenate the result to preserve the original result of a regular groupby pandas code.
     concat_res = []
@@ -83,18 +82,18 @@
     # Fix the index
     res.index = key_data
     res.index.name = df_grouped.keys
     return res
 
 
 class GroupByParallel:
-    def __init__(self, df_grouped: DataFrameGroupBy, n_cores: int = None, pbar: bool = True,
+    """GroupByParallel implementation"""
+    def __init__(self, df_grouped: DataFrameGroupBy, n_cores: int, pbar: bool = True,
                  keep_original_indexes: bool = False):
-        if n_cores is None:
-            n_cores = get_default_n_cores()
         self.df_grouped = df_grouped
         self.n_cores = n_cores
         self.pbar = pbar
         self.keep_original_indexes = keep_original_indexes
-    
+
     def apply(self, func: Callable):
-        return apply_on_groupby_parallel(self.df_grouped, func, self.n_cores, self.pbar, self.keep_original_indexes)
+        """Wrapper on top of regular df.groupby(col).apply(fn)"""
+        return _apply_on_groupby_parallel(self.df_grouped, func, self.n_cores, self.pbar, self.keep_original_indexes)
```

### Comparing `pandas-parallel-apply-2.0/pandas_parallel_apply/logger.py` & `pandas-parallel-apply-2.1/pandas_parallel_apply/logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,100 @@
-"""Python logger settings."""
+"""
+Python logger settings.
+Uses Env variables to control the log level:
+
+YOUR_KEY_LOGLEVEL=4 python blabla.py
+and logger.debug4("message")
+
+"""
+# pylint: disable=protected-access
 
 import os
+import sys
 import logging
+from colorama import Fore, Back, Style
+
+KEY = "PANDAS_PARALLEL_APPLY"
+ENV_KEY = f"{KEY}_LOGLEVEL"
+# defaults to -1 (no logger!).
+env_var = int(os.environ[ENV_KEY]) if ENV_KEY in os.environ else -1
 
-# define custom logging levels
+# we need numbers below 5 (last logging module used number)
 logging.DEBUG2 = 3
-logging.addLevelName(logging.DEBUG2, "DEBUG-VERBOSE")
-logging.__all__ += ["DEBUG2"]
+logging.DEBUG3 = 2
+logging.DEBUG4 = 1
+try:
+    loglevel = {
+        -1: logging.NOTSET,
+        0: logging.INFO,
+        1: logging.DEBUG,
+        2: logging.DEBUG2,
+        3: logging.DEBUG3,
+        4: logging.DEBUG4,
+    }[env_var]
+except KeyError:
+    sys.stderr.write(f"You tried to use {KEY}_LOGLEVEL={env_var}. You need to set it between -1 and 4\n")
+    sys.exit(1)
+# add the custom ones in the logger
+logging.addLevelName(logging.DEBUG2, "DGB2")
+logging.addLevelName(logging.DEBUG3, "DGB3")
+logging.addLevelName(logging.DEBUG4, "DGB4")
 
 
 class CustomFormatter(logging.Formatter):
     """Custom formatting for logger."""
 
-    yellow = "\x1b[33;20m"
-    green = "\x1b[32;20m"
-    cyan = "\x1b[36;20m"
-    red = "\x1b[31;20m"
-    bold_red = "\x1b[31;1m"
-    reset = "\x1b[0m"
-
+    reset = Style.RESET_ALL
     pre = "[%(asctime)s-%(name)s-%(levelname)s]"
     post = "(%(filename)s:%(funcName)s:%(lineno)d)"
 
-    # Example [TIME:LEVEL:NAME] Message [FILE:FUNC:LINE]
+    # Example [TIME:LEVEL:NAME] Message [FILE:FUNC:LINE]. We can update some other format here easily
     FORMATS = {
-        logging.DEBUG: f"{cyan}{pre}{reset} %(message)s {yellow}{post}{reset}",
-        logging.DEBUG2: f"{cyan}{pre}{reset} %(message)s {yellow}{post}{reset}",
-        logging.INFO: f"{green}{pre}{reset} %(message)s {yellow}{post}{reset}",
-        logging.WARNING: f"{yellow}{pre}{reset} %(message)s {yellow}{post}{reset}",
-        logging.ERROR: f"{red}{pre}{reset} %(message)s {yellow}{post}{reset}",
-        logging.CRITICAL: f"{bold_red}{pre}{reset} %(message)s {yellow}{post}{reset}",
+        logging.DEBUG: f"{Fore.CYAN}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.DEBUG2: f"{Fore.CYAN}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.DEBUG3: f"{Fore.MAGENTA}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.DEBUG4: f"{Back.RED}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.INFO: f"{Fore.GREEN}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.WARNING: f"{Fore.YELLOW}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.ERROR: f"{Fore.RED}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
+        logging.CRITICAL: f"{Back.RED}{pre}{reset} %(message)s {Fore.YELLOW}{post}{reset}",
     }
 
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno)
         formatter = logging.Formatter(log_fmt)
+        formatter.formatTime = self.formatTime
         return formatter.format(record)
 
+    # here we define the time format.
+    def formatTime(self, record, datefmt=None):
+        return super().formatTime(record, "%Y%m%d %H:%M:%S")
+
+
+# instantiate logger and set log level
+
+
+def _debug2(self, message, *args, **kws):
+    if self.isEnabledFor(logging.DEBUG2):
+        self._log(logging.DEBUG2, message, args, **kws)
+
+
+def _debug3(self, message, *args, **kws):
+    if self.isEnabledFor(logging.DEBUG3):
+        self._log(logging.DEBUG3, message, args, **kws)
+
+
+def _debug4(self, message, *args, **kws):
+    if self.isEnabledFor(logging.DEBUG4):
+        self._log(logging.DEBUG4, message, args, **kws)
 
-class CustomLogger:
-    """
-    Custom logger.
-    Attributes:
-        name (str): Logger's name.
-    Usage:
-        Set the ``<NAME>_LOGLEVEL`` environment variable to control the logging level for the whole project.
-        If not set, the default logging level is ``DEBUG`` (0 = no logging, 1 = info, 2 = debug, 3 = debug verbose).
-    """
-
-    log_levels = {0: logging.NOTSET, 1: logging.INFO, 2: logging.DEBUG, 3: logging.DEBUG2}
-
-    def __init__(self, name: str = "PANDAS_PARALLEL_APPLY"):
-
-        # initialize logger and set logging level
-        self.logger = logging.getLogger(name)
-        env_var = int(os.environ[f"{name}_LOGLEVEL"]) if f"{name}_LOGLEVEL" in os.environ else 2
-        self.logger.setLevel(self.log_levels[env_var])
-        self.logger.debug2 = lambda msg: self.logger.log(logging.DEBUG2, msg)
-
-        # add custom formatter to logger
-        handler = logging.StreamHandler()
-        handler.setFormatter(CustomFormatter())
-        self.logger.addHandler(handler)
-
-    def get_logger(self):
-        """Get logger."""
-        return self.logger
-
-    def set_level(self, level: int):
-        """
-        Change logging level: 0 = no logging, 1 = info, 2 = debug, 3 = debug verbose.
-        """
-        if 0 <= level <= 3:
-            self.logger.setLevel(self.log_levels[level])
-        else:
-            raise ValueError("Unknown logging level.")
 
+logger = logging.getLogger(KEY)
+logger.setLevel(loglevel)
+logging.Logger.debug2 = _debug2
+logging.Logger.debug3 = _debug3
+logging.Logger.debug4 = _debug4
 
-# global project logger
-logger = CustomLogger().get_logger()
+# add custom formatter to logger
+handler = logging.StreamHandler()
+handler.setFormatter(CustomFormatter())
+logger.addHandler(handler)
```

### Comparing `pandas-parallel-apply-2.0/pandas_parallel_apply/series_parallel.py` & `pandas-parallel-apply-2.1/pandas_parallel_apply/series_parallel.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 Apply on series
 Usage:
     standard => series.apply(f)
     parallel => SeriesParallel(series, n_cores).apply(f)
              => SeriesParallel(df[col], n_cores).apply(f)
 """
 from typing import Callable
-import pandas as pd
 from functools import partial
+import pandas as pd
 
-from .utils import parallelize_dataframe, get_default_n_cores
+from .utils import parallelize_dataframe
 
 
-def apply_on_series(series: pd.Series, f: Callable, pbar: bool = True) -> pd.Series:
+def _apply_on_series(series: pd.Series, f: Callable, pbar: bool = True) -> pd.Series:
+    """Returns progress_apply or simple apply based on pbar"""
     if pbar:
         return series.progress_apply(f)
-    else:
-        return series.apply(f)
+    return series.apply(f)
 
 
 class SeriesParallel:
-    def __init__(self, series: pd.Series, n_cores: int = None, pbar: bool = True):
-        if n_cores is None:
-            n_cores = get_default_n_cores()
+    """SeriesParallel implementation"""
+    def __init__(self, series: pd.Series, n_cores: int, pbar: bool = True):
         self.series = series
         self.n_cores = n_cores
         self.pbar = pbar
-    
+
     def apply(self, func: Callable) -> pd.Series:
-        return parallelize_dataframe(self.series, partial(apply_on_series, f=func, pbar=self.pbar), self.n_cores)
+        """Wrapper on top of regular ser.apply(fn)"""
+        return parallelize_dataframe(self.series, partial(_apply_on_series, f=func, pbar=self.pbar), self.n_cores)
```

### Comparing `pandas-parallel-apply-2.0/setup.py` & `pandas-parallel-apply-2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,17 @@
                 print("Dependency to a git repository should have the format:")
                 print("git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name")
         else:
             required.append(line)
     return required, dependency_links
 
 name = "pandas-parallel-apply"
-version = "2.0"
+version = "2.1"
 description = "Wrapper for df and df[col].apply parallelized"
-url = "https://gitlab.com/mihaicristianpirvu/pandas-parallel-apply"
+url = "https://gitlab.com/meehai/pandas-parallel-apply"
 
 loc = path.abspath(path.dirname(__file__))
 with open(f"{loc}/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 try:
     with open(f"{loc}/requirements.txt") as f:
```

### Comparing `pandas-parallel-apply-2.0/test/test_apply_df.py` & `pandas-parallel-apply-2.1/test/test_apply_df.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 df = pd.DataFrame(data, columns=["A", "B", 1])
 
 def f(x):
     return [x["A"] + 99, x["B"], x[1]]
 
 def test_apply_df_1():
     asdf = df.apply(f, axis=1)
-    dfp = DataFrameParallel(df, 4, pbar=False)
+    dfp = DataFrameParallel(df, n_cores=4, pbar=False)
     asdf2 = dfp.apply(f, axis=1)
     assert np.allclose(np.concatenate(asdf), np.concatenate(asdf2))
```

### Comparing `pandas-parallel-apply-2.0/test/test_apply_df_groupby.py` & `pandas-parallel-apply-2.1/test/test_apply_df_groupby.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,45 +13,45 @@
 N = 10000000
 data_random = {"A": np.random.randint(0, 10, size=(N, )), "B": np.arange(N),
     "C": [chr(ord("A") + np.random.randint(0, 26)) for _ in range(N)] }
 
 def test_one_col_return_series():
     df = pd.DataFrame(data_random)
     Y = df.groupby("A").apply(len)
-    K = GroupByParallel(df.groupby("A"), pbar=False).apply(len)
-    P = DataFrameParallel(df, pbar=False).groupby("A").apply(len)
+    K = GroupByParallel(df.groupby("A"), n_cores=4, pbar=False).apply(len)
+    P = DataFrameParallel(df, n_cores=4, pbar=False).groupby("A").apply(len)
 
     assert np.allclose(Y.values, K.values)
     assert np.allclose(Y.values, P.values)
 
 def test_one_col_return_df():
     df = pd.DataFrame(data_random)
     f = lambda df: df.iloc[0]
     Y = df.groupby("A").apply(f)
-    K = GroupByParallel(df.groupby("A"), pbar=False).apply(f)
-    P = DataFrameParallel(df, pbar=False).groupby("A").apply(f)
+    K = GroupByParallel(df.groupby("A"), n_cores=4, pbar=False).apply(f)
+    P = DataFrameParallel(df, n_cores=4, pbar=False).groupby("A").apply(f)
     assert (Y != K).sum().sum() == 0
     assert (Y != P).sum().sum() == 0
 
 def run_one_col_return_tricky_df_no_index(df):
     def f(df):
         np.random.seed(42)
         N = np.random.randint(1, len(df) + 1)
         return df.iloc[0 : N]
 
     df = pd.DataFrame(data_random)
     Y = df.groupby("A").apply(f)
-    K = GroupByParallel(df.groupby("A"), pbar=False, keep_original_indexes=False).apply(f)
-    P = DataFrameParallel(df, pbar=False).groupby("A").apply(f)
+    K = GroupByParallel(df.groupby("A"), n_cores=4, pbar=False, keep_original_indexes=False).apply(f)
+    P = DataFrameParallel(df, n_cores=4, pbar=False).groupby("A").apply(f)
     assert (Y.values != K.values).sum() == 0
     assert (Y.values != P.values).sum() == 0
 
 def run_one_col_return_tricky_df_plus_index(df):
     def f(df):
         np.random.seed(42)
         N = np.random.randint(1, len(df) + 1)
         return df.iloc[0 : N]
 
     df = pd.DataFrame(data_random)
     Y = df.groupby("A").apply(f)
-    K = GroupByParallel(df.groupby("A"), pbar=False, keep_original_indexes=True).apply(f)
+    K = GroupByParallel(df.groupby("A"), n_cores=4, pbar=False, keep_original_indexes=True).apply(f)
     assert (Y != K).sum().sum() == 0
```

