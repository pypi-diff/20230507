# Comparing `tmp/pymp4-1.3.2.tar.gz` & `tmp/pymp4-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymp4-1.3.2.tar", last modified: Tue Mar 28 07:51:23 2023, max compression
+gzip compressed data, was "pymp4-1.4.0.tar", max compression
```

## Comparing `pymp4-1.3.2.tar` & `pymp4-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:51:23.552116 pymp4-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-03-28 07:51:11.000000 pymp4-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-28 07:51:23.552116 pymp4-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-28 07:51:11.000000 pymp4-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-28 07:51:23.552116 pymp4-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-28 07:51:11.000000 pymp4-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:51:23.548116 pymp4-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:51:23.552116 pymp4-1.3.2/src/pymp4/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 07:51:11.000000 pymp4-1.3.2/src/pymp4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-28 07:51:11.000000 pymp4-1.3.2/src/pymp4/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-28 07:51:11.000000 pymp4-1.3.2/src/pymp4/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27114 2023-03-28 07:51:11.000000 pymp4-1.3.2/src/pymp4/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:51:23.552116 pymp4-1.3.2/src/pymp4/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-28 07:51:11.000000 pymp4-1.3.2/src/pymp4/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-03-28 07:51:11.000000 pymp4-1.3.2/src/pymp4/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:51:23.552116 pymp4-1.3.2/src/pymp4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-28 07:51:23.000000 pymp4-1.3.2/src/pymp4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-28 07:51:23.000000 pymp4-1.3.2/src/pymp4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 07:51:23.000000 pymp4-1.3.2/src/pymp4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-28 07:51:23.000000 pymp4-1.3.2/src/pymp4.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-28 07:51:23.000000 pymp4-1.3.2/src/pymp4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 07:51:23.000000 pymp4-1.3.2/src/pymp4.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:51:23.552116 pymp4-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-03-28 07:51:11.000000 pymp4-1.3.2/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-28 07:51:11.000000 pymp4-1.3.2/tests/test_dashboxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-03-28 07:51:11.000000 pymp4-1.3.2/tests/test_util.py
+-rw-r--r--   0        0        0    11339 2023-05-07 15:01:12.333352 pymp4-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1839 2023-05-07 15:01:12.333352 pymp4-1.4.0/README.md
+-rw-r--r--   0        0        0     1212 2023-05-07 15:01:12.333352 pymp4-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-07 15:01:12.333352 pymp4-1.4.0/src/pymp4/__init__.py
+-rw-r--r--   0        0        0      664 2023-05-07 15:01:12.333352 pymp4-1.4.0/src/pymp4/cli.py
+-rw-r--r--   0        0        0      651 2023-05-07 15:01:12.333352 pymp4-1.4.0/src/pymp4/exceptions.py
+-rw-r--r--   0        0        0    28245 2023-05-07 15:01:12.333352 pymp4-1.4.0/src/pymp4/parser.py
+-rw-r--r--   0        0        0       74 2023-05-07 15:01:12.333352 pymp4-1.4.0/src/pymp4/tools/__init__.py
+-rw-r--r--   0        0        0     2250 2023-05-07 15:01:12.333352 pymp4-1.4.0/src/pymp4/util.py
+-rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 pymp4-1.4.0/PKG-INFO
```

### Comparing `pymp4-1.3.2/LICENSE` & `pymp4-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymp4-1.3.2/src/pymp4/cli.py` & `pymp4-1.4.0/src/pymp4/cli.py`

 * *Files identical despite different names*

### Comparing `pymp4-1.3.2/src/pymp4/exceptions.py` & `pymp4-1.4.0/src/pymp4/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymp4-1.3.2/src/pymp4/parser.py` & `pymp4-1.4.0/src/pymp4/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,15 +407,16 @@
     Padding(6, pattern=b"\x00"),
     "data_reference_index" / Default(Int16ub, 1),
     Embedded(Switch(this.format, {
         b"ec-3": MP4ASampleEntryBox,
         b"mp4a": MP4ASampleEntryBox,
         b"enca": MP4ASampleEntryBox,
         b"avc1": AVC1SampleEntryBox,
-        b"encv": AVC1SampleEntryBox
+        b"encv": AVC1SampleEntryBox,
+        b"wvtt": Struct("children" / LazyBound(lambda ctx: GreedyRange(Box)))
     }, Struct("data" / GreedyBytes)))
 ))
 
 BitRateBox = Struct(
     "type" / Const(b"btrt"),
     "bufferSizeDB" / Int32ub,
     "maxBitrate" / Int32ub,
@@ -690,26 +691,34 @@
                            PrefixedArray(Int32ub, UUIDBytes(Bytes(16)))),
                         None),
     "init_data" / Prefixed(Int32ub, GreedyBytes)
 )
 
 TrackEncryptionBox = Struct(
     "type" / If(this._.type != b"uuid", Const(b"tenc")),
-    "version" / Default(Int8ub, 0),
+    "version" / Default(OneOf(Int8ub, (0, 1)), 0),
     "flags" / Default(Int24ub, 0),
-    "_reserved0" / Const(Int8ub, 0),
-    "_reserved1" / Const(Int8ub, 0),
-    "is_encrypted" / Int8ub,
-    "iv_size" / Int8ub,
+    "_reserved" / Const(Int8ub, 0),
+    "default_byte_blocks" / Default(IfThenElse(
+        this.version > 0,
+        BitStruct(
+            # count of encrypted blocks in the protection pattern, where each block is 16-bytes
+            "crypt" / Nibble,
+            # count of unencrypted blocks in the protection pattern
+            "skip" / Nibble
+        ),
+        Const(Int8ub, 0)
+    ), 0),
+    "is_encrypted" / OneOf(Int8ub, (0, 1)),
+    "iv_size" / OneOf(Int8ub, (0, 8, 16)),
     "key_ID" / UUIDBytes(Bytes(16)),
-    "constant_iv" / Default(If(this.is_encrypted and this.iv_size == 0,
-                               PrefixedArray(Int8ub, Byte),
-                               ),
-                            None)
-
+    "constant_iv" / Default(If(
+        this.is_encrypted and this.iv_size == 0,
+        PrefixedArray(Int8ub, Byte)
+    ), None)
 )
 
 SampleEncryptionBox = Struct(
     "type" / If(this._.type != b"uuid", Const(b"senc")),
     "version" / Const(Int8ub, 0),
     "flags" / BitStruct(
         Padding(22),
@@ -754,14 +763,41 @@
     "data" / Switch(this.extended_type, {
         UUID("A2394F52-5A9B-4F14-A244-6C427C648DF4"): SampleEncryptionBox,
         UUID("D08A4F18-10F3-4A82-B6C8-32D8ABA183D3"): ProtectionSystemHeaderBox,
         UUID("8974DBCE-7BE7-4C51-84F9-7148F9882554"): TrackEncryptionBox
     }, GreedyBytes)
 )
 
+# WebVTT boxes
+
+CueIDBox = Struct(
+    "type" / Const(b"iden"),
+    "cue_id" / GreedyString("utf8")
+)
+
+CueSettingsBox = Struct(
+    "type" / Const(b"sttg"),
+    "settings" / GreedyString("utf8")
+)
+
+CuePayloadBox = Struct(
+    "type" / Const(b"payl"),
+    "cue_text" / GreedyString("utf8")
+)
+
+WebVTTConfigurationBox = Struct(
+    "type" / Const(b"vttC"),
+    "config" / GreedyString("utf8")
+)
+
+WebVTTSourceLabelBox = Struct(
+    "type" / Const(b"vlab"),
+    "label" / GreedyString("utf8")
+)
+
 ContainerBoxLazy = LazyBound(lambda ctx: ContainerBox)
 
 
 class TellMinusSizeOf(Subconstruct):
     def __init__(self, subcon):
         super(TellMinusSizeOf, self).__init__(subcon)
         self.flagbuildnone = True
@@ -828,15 +864,23 @@
         b"schm": SchemeTypeBox,
         b"schi": ContainerBoxLazy,
         # piff
         b"uuid": UUIDBox,
         # HDS boxes
         b'abst': HDSSegmentBox,
         b'asrt': HDSSegmentRunBox,
-        b'afrt': HDSFragmentRunBox
+        b'afrt': HDSFragmentRunBox,
+        # WebVTT
+        b"vttC": WebVTTConfigurationBox,
+        b"vlab": WebVTTSourceLabelBox,
+        b"vttc": ContainerBoxLazy,
+        b"vttx": ContainerBoxLazy,
+        b"iden": CueIDBox,
+        b"sttg": CueSettingsBox,
+        b"payl": CuePayloadBox
     }, default=RawBox)),
     "end" / Tell
 ))
 
 ContainerBox = Struct(
     "type" / String(4, padchar=b" ", paddir="right"),
     "children" / GreedyRange(Box)
```

### Comparing `pymp4-1.3.2/src/pymp4/util.py` & `pymp4-1.4.0/src/pymp4/util.py`

 * *Files identical despite different names*

