# Comparing `tmp/retrotype-0.0.3.tar.gz` & `tmp/retrotype-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retrotype-0.0.3.tar", last modified: Sat Dec 31 02:47:49 2022, max compression
+gzip compressed data, was "retrotype-1.0.0.tar", last modified: Sun May  7 20:17:42 2023, max compression
```

## Comparing `retrotype-0.0.3.tar` & `retrotype-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2022-12-31 02:47:49.597082 retrotype-0.0.3/
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     1072 2022-11-11 18:54:20.000000 retrotype-0.0.3/LICENSE
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     6140 2022-12-31 02:47:49.597082 retrotype-0.0.3/PKG-INFO
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     4223 2022-12-09 04:10:35.000000 retrotype-0.0.3/README.md
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     1310 2022-12-31 02:45:10.000000 retrotype-0.0.3/pyproject.toml
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       38 2022-12-31 02:47:49.597082 retrotype-0.0.3/setup.cfg
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       74 2022-12-09 04:10:35.000000 retrotype-0.0.3/setup.py
-drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2022-12-31 02:47:49.593082 retrotype-0.0.3/src/
-drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2022-12-31 02:47:49.593082 retrotype-0.0.3/src/retrotype/
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)        0 2022-12-09 04:10:35.000000 retrotype-0.0.3/src/retrotype/__init__.py
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     7054 2022-12-09 04:10:35.000000 retrotype-0.0.3/src/retrotype/char_maps.py
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     7392 2022-12-31 02:45:10.000000 retrotype-0.0.3/src/retrotype/retrotype_cli.py
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)    18023 2022-12-31 02:45:10.000000 retrotype-0.0.3/src/retrotype/retrotype_lib.py
-drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2022-12-31 02:47:49.597082 retrotype-0.0.3/src/retrotype.egg-info/
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     6140 2022-12-31 02:47:49.000000 retrotype-0.0.3/src/retrotype.egg-info/PKG-INFO
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)      380 2022-12-31 02:47:49.000000 retrotype-0.0.3/src/retrotype.egg-info/SOURCES.txt
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)        1 2022-12-31 02:47:49.000000 retrotype-0.0.3/src/retrotype.egg-info/dependency_links.txt
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       78 2022-12-31 02:47:49.000000 retrotype-0.0.3/src/retrotype.egg-info/entry_points.txt
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       60 2022-12-31 02:47:49.000000 retrotype-0.0.3/src/retrotype.egg-info/requires.txt
--rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       10 2022-12-31 02:47:49.000000 retrotype-0.0.3/src/retrotype.egg-info/top_level.txt
+drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2023-05-07 20:17:42.552525 retrotype-1.0.0/
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     1072 2022-11-11 18:54:20.000000 retrotype-1.0.0/LICENSE
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     6140 2023-05-07 20:17:42.552525 retrotype-1.0.0/PKG-INFO
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     4223 2022-12-09 04:10:35.000000 retrotype-1.0.0/README.md
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     1310 2023-05-07 20:01:25.000000 retrotype-1.0.0/pyproject.toml
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       38 2023-05-07 20:17:42.552525 retrotype-1.0.0/setup.cfg
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       74 2022-12-09 04:10:35.000000 retrotype-1.0.0/setup.py
+drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2023-05-07 20:17:42.548525 retrotype-1.0.0/src/
+drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2023-05-07 20:17:42.548525 retrotype-1.0.0/src/retrotype/
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)        0 2022-12-09 04:10:35.000000 retrotype-1.0.0/src/retrotype/__init__.py
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     7054 2022-12-09 04:10:35.000000 retrotype-1.0.0/src/retrotype/char_maps.py
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     7977 2023-04-29 20:13:09.000000 retrotype-1.0.0/src/retrotype/retrotype_cli.py
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)    17445 2023-04-29 20:13:09.000000 retrotype-1.0.0/src/retrotype/retrotype_lib.py
+drwxrwxr-x   0 mbuhidar  (1000) mbuhidar  (1000)        0 2023-05-07 20:17:42.552525 retrotype-1.0.0/src/retrotype.egg-info/
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)     6140 2023-05-07 20:17:42.000000 retrotype-1.0.0/src/retrotype.egg-info/PKG-INFO
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)      380 2023-05-07 20:17:42.000000 retrotype-1.0.0/src/retrotype.egg-info/SOURCES.txt
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)        1 2023-05-07 20:17:42.000000 retrotype-1.0.0/src/retrotype.egg-info/dependency_links.txt
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       78 2023-05-07 20:17:42.000000 retrotype-1.0.0/src/retrotype.egg-info/entry_points.txt
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       60 2023-05-07 20:17:42.000000 retrotype-1.0.0/src/retrotype.egg-info/requires.txt
+-rw-rw-r--   0 mbuhidar  (1000) mbuhidar  (1000)       10 2023-05-07 20:17:42.000000 retrotype-1.0.0/src/retrotype.egg-info/top_level.txt
```

### Comparing `retrotype-0.0.3/LICENSE` & `retrotype-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retrotype-0.0.3/PKG-INFO` & `retrotype-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retrotype
-Version: 0.0.3
+Version: 1.0.0
 Summary: Debuging and conversion tool for 1980s magazine type-in programs
 Author-email: Michael Buhidar <mbuhidar@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Michael Buhidar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `retrotype-0.0.3/README.md` & `retrotype-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `retrotype-0.0.3/pyproject.toml` & `retrotype-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "retrotype"
-version = "0.0.3"
+version = "1.0.0"
 description = "Debuging and conversion tool for 1980s magazine type-in programs"
 readme = "README.md"
 authors = [{ name = "Michael Buhidar", email = "mbuhidar@gmail.com" }]
 maintainers = []
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `retrotype-0.0.3/src/retrotype/char_maps.py` & `retrotype-1.0.0/src/retrotype/char_maps.py`

 * *Files identical despite different names*

### Comparing `retrotype-0.0.3/src/retrotype/retrotype_cli.py` & `retrotype-1.0.0/src/retrotype/retrotype_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,30 @@
 from retrotype.retrotype_lib import (
     Checksums,
     OutputFiles,
     TextListing,
     TokenizedLine,
 )
 
+SOURCE_CHOICES = ["ahoy1", "ahoy2", "ahoy3"]
+
+
+def check_source(source: str) -> str:
+    """Custom type for source argument for custom verbiage when argument
+    error is encountered.
+    """
+    if source in SOURCE_CHOICES:
+        return source
+    source_string = "'" + "', '".join(SOURCE_CHOICES) + "'"
+    raise argparse.ArgumentTypeError(
+        f"invalid choice: '{source}'\n"
+        "Magazine format not yet supported - "
+        f"choose from {source_string}."
+    )
+
 
 def parse_args(argv):
     """Parses command line inputs and generate command line interface and
     documentation.
     """
     parser = argparse.ArgumentParser(
         description="A tokenizer for Commodore BASIC typein programs. Supports"
@@ -71,16 +87,16 @@
         "- 0x1201 - VIC20 +16\n"
         "- 0x1201 - VIC20 +24K\n",
     )
 
     parser.add_argument(
         "-s",
         "--source",
-        choices=["ahoy1", "ahoy2", "ahoy3"],
-        type=str,
+        choices=SOURCE_CHOICES,
+        type=check_source,  # custom type instead of str
         nargs=1,
         required=False,
         metavar="source_format",
         default=["ahoy2"],
         help="Specifies the magazine source for conversion and checksum:\n"
         "ahoy1 - Ahoy magazine (Apr-May 1984)\n"
         "ahoy2 - Ahoy magazine (Jun 1984-Apr 1987) (default)\n"
@@ -125,15 +141,15 @@
     # call function to parse command line input arguments
     args = parse_args(argv)
 
     # call function to read input file lines
     tl = TextListing(args.file_in)
     try:
         raw_listing = tl.read_listing()
-    except IOError:
+    except FileNotFoundError:
         print("File read failed - please check source file name and path.")
         sys.exit(1)
 
     # check each line to insure each starts with a line number
     # and that the line numbers are sequential.
     if sequence_message := tl.check_line_num_seq(raw_listing):
         print(sequence_message)
@@ -144,16 +160,16 @@
         print(brace_message)
         sys.exit(1)
 
     # Create lines list converting to common special character codes in braces
     if args.source[0][:4] == "ahoy":
         lines_list = tl.ahoy_lines_list(raw_listing)
     else:
-        print("Magazine format not yet supported.")
-        sys.exit(1)
+        # reserved for selecting future magazine formats
+        sys.exit(1)  # pragma: no cover
 
     addr = int(args.loadaddr[0], 16)
 
     out_list = []
     ahoy_checksums = []
 
     for line in lines_list:
@@ -174,16 +190,16 @@
         if args.source[0] == "ahoy1":
             ahoy_checksums.append((line_num, cs.ahoy1_checksum()))
         elif args.source[0] == "ahoy2":
             ahoy_checksums.append((line_num, cs.ahoy2_checksum()))
         elif args.source[0] == "ahoy3":
             ahoy_checksums.append((line_num, cs.ahoy3_checksum()))
         else:
-            print("Magazine format not yet supported.")
-            sys.exit(1)
+            # reserved for selecting future magazine formats
+            sys.exit(1)  # pragma: no cover
 
         addr = addr + len(byte_list) + 4
 
         token_ln.extend(
             (
                 addr.to_bytes(2, "little"),
                 line_num.to_bytes(2, "little"),
@@ -208,13 +224,13 @@
 
     # Write text file containing line numbers, checksums, and line count
     ofiles.write_checksums(f"{file_stem}.chk")
 
     # Print line checksums to terminal, formatted based on screen width
     print("Line Checksums:\n")
     if not width:
-        width = get_terminal_size()[0]
+        width = get_terminal_size()[0]  # pragma: no cover
     print_checksums(ahoy_checksums, width)
 
 
 if __name__ == "__main__":
     sys.exit(command_line_runner())  # pragma: no cover
```

### Comparing `retrotype-0.0.3/src/retrotype/retrotype_lib.py` & `retrotype-1.0.0/src/retrotype/retrotype_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -312,41 +312,44 @@
     codes printed in the magazine for checking each line for typed in accuracy.
     """
 
     def __init__(self, line_num: int, byte_list: List[int]) -> None:
         self.line_num = line_num
         self.byte_list = byte_list
 
+    def xor_to_checksum(self, xor_value: int) -> str:
+        # get high nibble of xor_value
+        high_nib = (xor_value & 0xF0) >> 4
+        high_char_val = high_nib + 65  # 0x41
+        # get low nibble of xor_value
+        low_nib = xor_value & 0x0F
+        low_char_val = low_nib + 65  # 0x41
+        # return value of checksum
+        return chr(high_char_val) + chr(low_char_val)
+
     def ahoy1_checksum(self) -> str:
         """
         Method to create Ahoy checksums from passed in byte list to match the
         codes printed in the magazine for checking each line for typed
         accuracy. Covers Ahoy Bug Repellent version for Mar-Apr 1984 issues.
         """
 
         next_value = 0
 
         for char_val in self.byte_list:
-            # Detect spaces that are outside of quotes and ignore them, else
-            # execute primary checksum generation algorithm
+            # Detect spaces and ignore them
             if char_val == 32:
                 continue
-            next_value = char_val + next_value
-            next_value = next_value << 1
+            next_value += char_val
+            # left shift 1 bit and limit next_value to fit in one byte
+            next_value = (next_value << 1) & 255
 
         xor_value = next_value
 
-        # get high nibble of xor_value
-        high_nib = (xor_value & 0xF0) >> 4
-        high_char_val = high_nib + 65  # 0x41
-        # get low nibble of xor_value
-        low_nib = xor_value & 0x0F
-        low_char_val = low_nib + 65  # 0x41
-        # return value of checksum
-        return chr(high_char_val) + chr(low_char_val)
+        return self.xor_to_checksum(xor_value)
 
     def ahoy2_checksum(self) -> str:
         """
         Method to create Ahoy checksums from passed in byte list to match the
         codes printed in the magazine for checking each line for typed in
         accuracy. Covers Ahoy Bug Repellent version for May 1984-Apr 1987
         issues.
@@ -378,22 +381,15 @@
             xor_value = next_value ^ char_position
 
             # limit next value to fit in one byte
             next_value = next_value & 255
 
             char_position = char_position + 1
 
-        # get high nibble of xor_value
-        high_nib = (xor_value & 0xF0) >> 4
-        high_char_val = high_nib + 65  # 0x41
-        # get low nibble of xor_value
-        low_nib = xor_value & 0x0F
-        low_char_val = low_nib + 65  # 0x41
-        # return value of checksum
-        return chr(high_char_val) + chr(low_char_val)
+        return self.xor_to_checksum(xor_value)
 
     def ahoy3_checksum(self) -> str:
         """
         Method to create Ahoy checksums from passed in line number and
         byte list to match the codes printed in the magazine for checking each
         line for typed in accuracy. Covers the last Ahoy Bug Repellent
         version introduced in May 1987.
@@ -404,17 +400,14 @@
         in_quotes = False
 
         line_low = self.line_num % 256
         line_hi = int(self.line_num / 256)
 
         byte_line = [line_low] + [line_hi] + self.byte_list
 
-        # byte_list.insert(0, line_hi)
-        # byte_list.insert(0, line_low)
-
         for char_val in byte_line:
 
             # Detect quote symbol in line and toggle in-quotes flag
             if char_val == 34:
                 in_quotes = not in_quotes
 
             # Detect spaces that are outside of quotes and ignore them, else
@@ -427,22 +420,15 @@
             xor_value = next_value ^ char_position
 
             # limit next value to fit in one byte
             next_value = next_value & 255
 
             char_position = char_position + 1
 
-        # get high nibble of xor_value
-        high_nib = (xor_value & 0xF0) >> 4
-        high_char_val = high_nib + 65  # 0x41
-        # get low nibble of xor_value
-        low_nib = xor_value & 0x0F
-        low_char_val = low_nib + 65  # 0x41
-        # return value of checksum
-        return chr(high_char_val) + chr(low_char_val)
+        return self.xor_to_checksum(xor_value)
 
 
 class OutputFiles:
     """
     Support for writing binary files readable on Commodore computers or
     emulators and writing checksum files for comparison to codes printed in
     the magazines.
```

### Comparing `retrotype-0.0.3/src/retrotype.egg-info/PKG-INFO` & `retrotype-1.0.0/src/retrotype.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retrotype
-Version: 0.0.3
+Version: 1.0.0
 Summary: Debuging and conversion tool for 1980s magazine type-in programs
 Author-email: Michael Buhidar <mbuhidar@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Michael Buhidar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

