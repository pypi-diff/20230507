# Comparing `tmp/faucetconfrpc-0.8.tar.gz` & `tmp/faucetconfrpc-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/faucetconfrpc-0.8.tar", last modified: Fri Jul 10 04:04:24 2020, max compression
+gzip compressed data, was "dist/faucetconfrpc-0.9.tar", last modified: Thu Jul 16 10:42:45 2020, max compression
```

## Comparing `faucetconfrpc-0.8.tar` & `faucetconfrpc-0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-10 04:04:24.000000 faucetconfrpc-0.8/
--rw-r--r--   0 runner    (1001) docker     (116)      113 2020-07-10 04:03:59.000000 faucetconfrpc-0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-10 04:04:24.000000 faucetconfrpc-0.8/faucetconfrpc/
--rw-r--r--   0 runner    (1001) docker     (116)    27716 2020-07-10 04:03:59.000000 faucetconfrpc-0.8/faucetconfrpc/faucetconfrpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (116)    14400 2020-07-10 04:03:59.000000 faucetconfrpc-0.8/faucetconfrpc/faucetconfrpc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (116)     3543 2020-07-10 04:03:59.000000 faucetconfrpc-0.8/faucetconfrpc/faucetconfrpc_client_lib.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1614 2020-07-10 04:03:59.000000 faucetconfrpc-0.8/faucetconfrpc/faucetconfrpc_client.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    13981 2020-07-10 04:03:59.000000 faucetconfrpc-0.8/faucetconfrpc/faucetconfrpc_server.py
--rw-r--r--   0 runner    (1001) docker     (116)     4066 2020-07-10 04:03:59.000000 faucetconfrpc-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)        4 2020-07-10 04:03:59.000000 faucetconfrpc-0.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-10 04:04:24.000000 faucetconfrpc-0.8/faucetconfrpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      450 2020-07-10 04:04:24.000000 faucetconfrpc-0.8/faucetconfrpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-10 04:04:23.000000 faucetconfrpc-0.8/faucetconfrpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       51 2020-07-10 04:04:23.000000 faucetconfrpc-0.8/faucetconfrpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2020-07-10 04:04:23.000000 faucetconfrpc-0.8/faucetconfrpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      271 2020-07-10 04:04:23.000000 faucetconfrpc-0.8/faucetconfrpc.egg-info/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (116)      522 2020-07-10 04:03:59.000000 faucetconfrpc-0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)      271 2020-07-10 04:04:24.000000 faucetconfrpc-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    11365 2020-07-10 04:03:59.000000 faucetconfrpc-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      102 2020-07-10 04:04:24.000000 faucetconfrpc-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       57 2020-07-10 04:03:59.000000 faucetconfrpc-0.8/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-16 10:42:45.000000 faucetconfrpc-0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)      113 2020-07-16 10:42:20.000000 faucetconfrpc-0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-16 10:42:45.000000 faucetconfrpc-0.9/faucetconfrpc/
+-rw-r--r--   0 runner    (1001) docker     (116)    28192 2020-07-16 10:42:20.000000 faucetconfrpc-0.9/faucetconfrpc/faucetconfrpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14400 2020-07-16 10:42:20.000000 faucetconfrpc-0.9/faucetconfrpc/faucetconfrpc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3647 2020-07-16 10:42:20.000000 faucetconfrpc-0.9/faucetconfrpc/faucetconfrpc_client_lib.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     1614 2020-07-16 10:42:20.000000 faucetconfrpc-0.9/faucetconfrpc/faucetconfrpc_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    14338 2020-07-16 10:42:20.000000 faucetconfrpc-0.9/faucetconfrpc/faucetconfrpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4066 2020-07-16 10:42:20.000000 faucetconfrpc-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)        4 2020-07-16 10:42:20.000000 faucetconfrpc-0.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-16 10:42:45.000000 faucetconfrpc-0.9/faucetconfrpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      450 2020-07-16 10:42:45.000000 faucetconfrpc-0.9/faucetconfrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-16 10:42:44.000000 faucetconfrpc-0.9/faucetconfrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       51 2020-07-16 10:42:44.000000 faucetconfrpc-0.9/faucetconfrpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2020-07-16 10:42:44.000000 faucetconfrpc-0.9/faucetconfrpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      271 2020-07-16 10:42:44.000000 faucetconfrpc-0.9/faucetconfrpc.egg-info/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (116)      522 2020-07-16 10:42:20.000000 faucetconfrpc-0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)      271 2020-07-16 10:42:45.000000 faucetconfrpc-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    11365 2020-07-16 10:42:20.000000 faucetconfrpc-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      102 2020-07-16 10:42:45.000000 faucetconfrpc-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)       57 2020-07-16 10:42:20.000000 faucetconfrpc-0.9/MANIFEST.in
```

### Comparing `faucetconfrpc-0.8/faucetconfrpc/faucetconfrpc_pb2.py` & `faucetconfrpc-0.9/faucetconfrpc/faucetconfrpc_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='faucetconfrpc/faucetconfrpc.proto',
   package='faucetconfserver',
   syntax='proto3',
   serialized_options=b'Z\022.;faucetconfserver',
-  serialized_pb=b'\n!faucetconfrpc/faucetconfrpc.proto\x12\x10\x66\x61ucetconfserver\"/\n\x14GetConfigFileRequest\x12\x17\n\x0f\x63onfig_filename\x18\x01 \x01(\t\")\n\x12GetConfigFileReply\x12\x13\n\x0b\x63onfig_yaml\x18\x01 \x01(\t\"S\n\x14SetConfigFileRequest\x12\x17\n\x0f\x63onfig_filename\x18\x01 \x01(\t\x12\x13\n\x0b\x63onfig_yaml\x18\x02 \x01(\t\x12\r\n\x05merge\x18\x03 \x01(\x08\"\x14\n\x12SetConfigFileReply\"M\n\x18\x44\x65lConfigFromFileRequest\x12\x17\n\x0f\x63onfig_filename\x18\x01 \x01(\t\x12\x18\n\x10\x63onfig_yaml_keys\x18\x02 \x01(\t\"\x18\n\x16\x44\x65lConfigFromFileReply\"P\n\x14\x41\x64\x64PortMirrorRequest\x12\x0f\n\x07\x64p_name\x18\x01 \x01(\t\x12\x0f\n\x07port_no\x18\x02 \x01(\x05\x12\x16\n\x0emirror_port_no\x18\x03 \x01(\x05\"\x14\n\x12\x41\x64\x64PortMirrorReply\"S\n\x17RemovePortMirrorRequest\x12\x0f\n\x07\x64p_name\x18\x01 \x01(\t\x12\x0f\n\x07port_no\x18\x02 \x01(\x05\x12\x16\n\x0emirror_port_no\x18\x03 \x01(\x05\"\x17\n\x15RemovePortMirrorReply\"C\n\x11SetPortAclRequest\x12\x0f\n\x07\x64p_name\x18\x01 \x01(\t\x12\x0f\n\x07port_no\x18\x02 \x01(\x05\x12\x0c\n\x04\x61\x63ls\x18\x03 \x01(\t\"\x11\n\x0fSetPortAclReply\"B\n\x11\x41\x64\x64PortAclRequest\x12\x0f\n\x07\x64p_name\x18\x01 \x01(\t\x12\x0f\n\x07port_no\x18\x02 \x01(\x05\x12\x0b\n\x03\x61\x63l\x18\x03 \x01(\t\"\x11\n\x0f\x41\x64\x64PortAclReply\"E\n\x14RemovePortAclRequest\x12\x0f\n\x07\x64p_name\x18\x01 \x01(\t\x12\x0f\n\x07port_no\x18\x02 \x01(\x05\x12\x0b\n\x03\x61\x63l\x18\x03 \x01(\t\"\x14\n\x12RemovePortAclReply2\x9d\x06\n\x10\x46\x61ucetConfServer\x12_\n\rGetConfigFile\x12&.faucetconfserver.GetConfigFileRequest\x1a$.faucetconfserver.GetConfigFileReply\"\x00\x12_\n\rSetConfigFile\x12&.faucetconfserver.SetConfigFileRequest\x1a$.faucetconfserver.SetConfigFileReply\"\x00\x12k\n\x11\x44\x65lConfigFromFile\x12*.faucetconfserver.DelConfigFromFileRequest\x1a(.faucetconfserver.DelConfigFromFileReply\"\x00\x12_\n\rAddPortMirror\x12&.faucetconfserver.AddPortMirrorRequest\x1a$.faucetconfserver.AddPortMirrorReply\"\x00\x12h\n\x10RemovePortMirror\x12).faucetconfserver.RemovePortMirrorRequest\x1a\'.faucetconfserver.RemovePortMirrorReply\"\x00\x12V\n\nAddPortAcl\x12#.faucetconfserver.AddPortAclRequest\x1a!.faucetconfserver.AddPortAclReply\"\x00\x12_\n\rRemovePortAcl\x12&.faucetconfserver.RemovePortAclRequest\x1a$.faucetconfserver.RemovePortAclReply\"\x00\x12V\n\nSetPortAcl\x12#.faucetconfserver.SetPortAclRequest\x1a!.faucetconfserver.SetPortAclReply\"\x00\x42\x14Z\x12.;faucetconfserverb\x06proto3'
+  serialized_pb=b'\n!faucetconfrpc/faucetconfrpc.proto\x12\x10\x66\x61ucetconfserver\"/\n\x14GetConfigFileRequest\x12\x17\n\x0f\x63onfig_filename\x18\x01 \x01(\t\")\n\x12GetConfigFileReply\x12\x13\n\x0b\x63onfig_yaml\x18\x01 \x01(\t\"q\n\x14SetConfigFileRequest\x12\x17\n\x0f\x63onfig_filename\x18\x01 \x01(\t\x12\x13\n\x0b\x63onfig_yaml\x18\x02 \x01(\t\x12\r\n\x05merge\x18\x03 \x01(\x08\x12\x1c\n\x14\x64\x65l_config_yaml_keys\x18\x04 \x01(\t\"\x14\n\x12SetConfigFileReply\"M\n\x18\x44\x65lConfigFromFileRequest\x12\x17\n\x0f\x63onfig_filename\x18\x01 \x01(\t\x12\x18\n\x10\x63onfig_yaml_keys\x18\x02 \x01(\t\"\x18\n\x16\x44\x65lConfigFromFileReply\"P\n\x14\x41\x64\x64PortMirrorRequest\x12\x0f\n\x07\x64p_name\x18\x01 \x01(\t\x12\x0f\n\x07port_no\x18\x02 \x01(\x05\x12\x16\n\x0emirror_port_no\x18\x03 \x01(\x05\"\x14\n\x12\x41\x64\x64PortMirrorReply\"S\n\x17RemovePortMirrorRequest\x12\x0f\n\x07\x64p_name\x18\x01 \x01(\t\x12\x0f\n\x07port_no\x18\x02 \x01(\x05\x12\x16\n\x0emirror_port_no\x18\x03 \x01(\x05\"\x17\n\x15RemovePortMirrorReply\"C\n\x11SetPortAclRequest\x12\x0f\n\x07\x64p_name\x18\x01 \x01(\t\x12\x0f\n\x07port_no\x18\x02 \x01(\x05\x12\x0c\n\x04\x61\x63ls\x18\x03 \x01(\t\"\x11\n\x0fSetPortAclReply\"B\n\x11\x41\x64\x64PortAclRequest\x12\x0f\n\x07\x64p_name\x18\x01 \x01(\t\x12\x0f\n\x07port_no\x18\x02 \x01(\x05\x12\x0b\n\x03\x61\x63l\x18\x03 \x01(\t\"\x11\n\x0f\x41\x64\x64PortAclReply\"E\n\x14RemovePortAclRequest\x12\x0f\n\x07\x64p_name\x18\x01 \x01(\t\x12\x0f\n\x07port_no\x18\x02 \x01(\x05\x12\x0b\n\x03\x61\x63l\x18\x03 \x01(\t\"\x14\n\x12RemovePortAclReply2\x9d\x06\n\x10\x46\x61ucetConfServer\x12_\n\rGetConfigFile\x12&.faucetconfserver.GetConfigFileRequest\x1a$.faucetconfserver.GetConfigFileReply\"\x00\x12_\n\rSetConfigFile\x12&.faucetconfserver.SetConfigFileRequest\x1a$.faucetconfserver.SetConfigFileReply\"\x00\x12k\n\x11\x44\x65lConfigFromFile\x12*.faucetconfserver.DelConfigFromFileRequest\x1a(.faucetconfserver.DelConfigFromFileReply\"\x00\x12_\n\rAddPortMirror\x12&.faucetconfserver.AddPortMirrorRequest\x1a$.faucetconfserver.AddPortMirrorReply\"\x00\x12h\n\x10RemovePortMirror\x12).faucetconfserver.RemovePortMirrorRequest\x1a\'.faucetconfserver.RemovePortMirrorReply\"\x00\x12V\n\nAddPortAcl\x12#.faucetconfserver.AddPortAclRequest\x1a!.faucetconfserver.AddPortAclReply\"\x00\x12_\n\rRemovePortAcl\x12&.faucetconfserver.RemovePortAclRequest\x1a$.faucetconfserver.RemovePortAclReply\"\x00\x12V\n\nSetPortAcl\x12#.faucetconfserver.SetPortAclRequest\x1a!.faucetconfserver.SetPortAclReply\"\x00\x42\x14Z\x12.;faucetconfserverb\x06proto3'
 )
 
 
 
 
 _GETCONFIGFILEREQUEST = _descriptor.Descriptor(
   name='GetConfigFileRequest',
@@ -110,28 +110,35 @@
     _descriptor.FieldDescriptor(
       name='merge', full_name='faucetconfserver.SetConfigFileRequest.merge', index=2,
       number=3, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='del_config_yaml_keys', full_name='faucetconfserver.SetConfigFileRequest.del_config_yaml_keys', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=147,
-  serialized_end=230,
+  serialized_end=260,
 )
 
 
 _SETCONFIGFILEREPLY = _descriptor.Descriptor(
   name='SetConfigFileReply',
   full_name='faucetconfserver.SetConfigFileReply',
   filename=None,
@@ -146,16 +153,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=232,
-  serialized_end=252,
+  serialized_start=262,
+  serialized_end=282,
 )
 
 
 _DELCONFIGFROMFILEREQUEST = _descriptor.Descriptor(
   name='DelConfigFromFileRequest',
   full_name='faucetconfserver.DelConfigFromFileRequest',
   filename=None,
@@ -184,16 +191,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=254,
-  serialized_end=331,
+  serialized_start=284,
+  serialized_end=361,
 )
 
 
 _DELCONFIGFROMFILEREPLY = _descriptor.Descriptor(
   name='DelConfigFromFileReply',
   full_name='faucetconfserver.DelConfigFromFileReply',
   filename=None,
@@ -208,16 +215,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=333,
-  serialized_end=357,
+  serialized_start=363,
+  serialized_end=387,
 )
 
 
 _ADDPORTMIRRORREQUEST = _descriptor.Descriptor(
   name='AddPortMirrorRequest',
   full_name='faucetconfserver.AddPortMirrorRequest',
   filename=None,
@@ -253,16 +260,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=359,
-  serialized_end=439,
+  serialized_start=389,
+  serialized_end=469,
 )
 
 
 _ADDPORTMIRRORREPLY = _descriptor.Descriptor(
   name='AddPortMirrorReply',
   full_name='faucetconfserver.AddPortMirrorReply',
   filename=None,
@@ -277,16 +284,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=441,
-  serialized_end=461,
+  serialized_start=471,
+  serialized_end=491,
 )
 
 
 _REMOVEPORTMIRRORREQUEST = _descriptor.Descriptor(
   name='RemovePortMirrorRequest',
   full_name='faucetconfserver.RemovePortMirrorRequest',
   filename=None,
@@ -322,16 +329,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=463,
-  serialized_end=546,
+  serialized_start=493,
+  serialized_end=576,
 )
 
 
 _REMOVEPORTMIRRORREPLY = _descriptor.Descriptor(
   name='RemovePortMirrorReply',
   full_name='faucetconfserver.RemovePortMirrorReply',
   filename=None,
@@ -346,16 +353,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=548,
-  serialized_end=571,
+  serialized_start=578,
+  serialized_end=601,
 )
 
 
 _SETPORTACLREQUEST = _descriptor.Descriptor(
   name='SetPortAclRequest',
   full_name='faucetconfserver.SetPortAclRequest',
   filename=None,
@@ -391,16 +398,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=573,
-  serialized_end=640,
+  serialized_start=603,
+  serialized_end=670,
 )
 
 
 _SETPORTACLREPLY = _descriptor.Descriptor(
   name='SetPortAclReply',
   full_name='faucetconfserver.SetPortAclReply',
   filename=None,
@@ -415,16 +422,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=642,
-  serialized_end=659,
+  serialized_start=672,
+  serialized_end=689,
 )
 
 
 _ADDPORTACLREQUEST = _descriptor.Descriptor(
   name='AddPortAclRequest',
   full_name='faucetconfserver.AddPortAclRequest',
   filename=None,
@@ -460,16 +467,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=661,
-  serialized_end=727,
+  serialized_start=691,
+  serialized_end=757,
 )
 
 
 _ADDPORTACLREPLY = _descriptor.Descriptor(
   name='AddPortAclReply',
   full_name='faucetconfserver.AddPortAclReply',
   filename=None,
@@ -484,16 +491,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=729,
-  serialized_end=746,
+  serialized_start=759,
+  serialized_end=776,
 )
 
 
 _REMOVEPORTACLREQUEST = _descriptor.Descriptor(
   name='RemovePortAclRequest',
   full_name='faucetconfserver.RemovePortAclRequest',
   filename=None,
@@ -529,16 +536,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=748,
-  serialized_end=817,
+  serialized_start=778,
+  serialized_end=847,
 )
 
 
 _REMOVEPORTACLREPLY = _descriptor.Descriptor(
   name='RemovePortAclReply',
   full_name='faucetconfserver.RemovePortAclReply',
   filename=None,
@@ -553,16 +560,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=819,
-  serialized_end=839,
+  serialized_start=849,
+  serialized_end=869,
 )
 
 DESCRIPTOR.message_types_by_name['GetConfigFileRequest'] = _GETCONFIGFILEREQUEST
 DESCRIPTOR.message_types_by_name['GetConfigFileReply'] = _GETCONFIGFILEREPLY
 DESCRIPTOR.message_types_by_name['SetConfigFileRequest'] = _SETCONFIGFILEREQUEST
 DESCRIPTOR.message_types_by_name['SetConfigFileReply'] = _SETCONFIGFILEREPLY
 DESCRIPTOR.message_types_by_name['DelConfigFromFileRequest'] = _DELCONFIGFROMFILEREQUEST
@@ -696,16 +703,16 @@
 
 _FAUCETCONFSERVER = _descriptor.ServiceDescriptor(
   name='FaucetConfServer',
   full_name='faucetconfserver.FaucetConfServer',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
-  serialized_start=842,
-  serialized_end=1639,
+  serialized_start=872,
+  serialized_end=1669,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetConfigFile',
     full_name='faucetconfserver.FaucetConfServer.GetConfigFile',
     index=0,
     containing_service=None,
     input_type=_GETCONFIGFILEREQUEST,
```

### Comparing `faucetconfrpc-0.8/faucetconfrpc/faucetconfrpc_pb2_grpc.py` & `faucetconfrpc-0.9/faucetconfrpc/faucetconfrpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `faucetconfrpc-0.8/faucetconfrpc/faucetconfrpc_client_lib.py` & `faucetconfrpc-0.9/faucetconfrpc/faucetconfrpc_client_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,22 +33,24 @@
         """Get a YAML config file."""
         response = self._call(self.stub.GetConfigFile, faucetconfrpc_pb2.GetConfigFileRequest(
             config_filename=config_filename))
         if response is not None:
             return yaml.safe_load(response.config_yaml)
         return None
 
-    def set_config_file(self, config_yaml, config_filename=None, merge=True):
+    def set_config_file(self, config_yaml, config_filename=None, merge=True,
+                        del_config_yaml_keys=''):
         """Set a YAML config file."""
         if isinstance(config_yaml, dict):
             config_yaml = yaml.dump(config_yaml)
         return self._call(self.stub.SetConfigFile, faucetconfrpc_pb2.SetConfigFileRequest(
             config_filename=config_filename,
             config_yaml=config_yaml,
-            merge=merge))
+            merge=merge,
+            del_config_yaml_keys=del_config_yaml_keys))
 
     def del_config_from_file(self, config_yaml_keys, config_filename=None):
         """Delete a key from YAML config file."""
         if isinstance(config_yaml_keys, list):
             config_yaml_keys = yaml.dump(config_yaml_keys)
         return self._call(self.stub.DelConfigFromFile, faucetconfrpc_pb2.DelConfigFromFileRequest(
             config_filename=config_filename,
```

### Comparing `faucetconfrpc-0.8/faucetconfrpc/faucetconfrpc_client.py` & `faucetconfrpc-0.9/faucetconfrpc/faucetconfrpc_client.py`

 * *Files identical despite different names*

### Comparing `faucetconfrpc-0.8/faucetconfrpc/faucetconfrpc_server.py` & `faucetconfrpc-0.9/faucetconfrpc/faucetconfrpc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,40 +106,48 @@
         new_file = tempfile.NamedTemporaryFile(
             mode='wt', dir=config_dir, delete=False)
         new_file_name = new_file.name
         new_file.write(yaml.dump(config_yaml))
         new_file.close()
         os.rename(new_file_name, os.path.join(config_dir, config_filename))
 
-    def _set_config_file(self, config_filename, config_yaml, merge):
+    def _set_config_file(self, config_filename, config_yaml, merge, del_yaml_keys=None):
         try:
             config_filename = self._validate_filename(config_filename)
             new_config_yaml = yaml.safe_load(config_yaml)
             if merge:
                 curr_config_yaml = self._get_config_file(config_filename)
+                if del_yaml_keys:
+                    curr_config_yaml = self._del_keys_from_yaml(
+                        del_yaml_keys, curr_config_yaml)
                 new_config_yaml = self._yaml_merge(curr_config_yaml, new_config_yaml)
             self._validate_config_tree(config_filename, new_config_yaml)
             self._replace_config_file(config_filename, new_config_yaml)
         except (FileNotFoundError, PermissionError, _ServerError) as err:
             raise _ServerError(err)
 
+    @staticmethod
+    def _del_keys_from_yaml(config_yaml_keys, new_config_yaml):
+        config_yaml_keys = yaml.safe_load(config_yaml_keys)
+        if not isinstance(config_yaml_keys, list):
+            raise _ServerError('config_yaml_keys %s not a list' % config_yaml_keys)
+        penultimate_key = new_config_yaml
+        last_key = config_yaml_keys[-1]
+        for key in config_yaml_keys[:-1]:
+            penultimate_key = penultimate_key[key]
+        if isinstance(penultimate_key, dict):
+            del penultimate_key[last_key]
+        else:
+            penultimate_key.remove(last_key)
+        return new_config_yaml
+
     def _del_config_from_file(self, config_filename, config_yaml_keys):
         try:
-            config_yaml_keys = yaml.safe_load(config_yaml_keys)
-            if not isinstance(config_yaml_keys, list):
-                raise _ServerError('config_yaml_keys %s not a list' % config_yaml_keys)
-            new_config_yaml = self._get_config_file(config_filename)
-            penultimate_key = new_config_yaml
-            last_key = config_yaml_keys[-1]
-            for key in config_yaml_keys[:-1]:
-                penultimate_key = penultimate_key[key]
-            if isinstance(penultimate_key, dict):
-                del penultimate_key[last_key]
-            else:
-                penultimate_key.remove(last_key)
+            new_config_yaml = self._del_keys_from_yaml(
+                config_yaml_keys, self._get_config_file(config_filename))
             self._validate_config_tree(config_filename, new_config_yaml)
             self._replace_config_file(config_filename, new_config_yaml)
         except (KeyError, ValueError, _ServerError) as err:
             raise _ServerError(err)
 
     @staticmethod
     def _log_error(context, request, err):
@@ -165,15 +173,16 @@
         """Overwrite/update config file contents with provided YAML."""
         with self.lock:
             try:
                 config_filename = request.config_filename
                 if not config_filename:
                     config_filename = self._filename_for_yaml(request.config_yaml)
                 self._set_config_file(
-                    config_filename, request.config_yaml, request.merge)
+                    config_filename, request.config_yaml, request.merge,
+                    request.del_config_yaml_keys)
             except _ServerError as err:
                 self._log_error(context, request, err)
         return faucetconfrpc_pb2.SetConfigFileReply()
 
     def _get_mirror(self, request):
         dps = self._validate_faucet_config(self.config_dir)
         dp = dps[request.dp_name]  # pylint: disable=invalid-name
```

### Comparing `faucetconfrpc-0.8/README.md` & `faucetconfrpc-0.9/README.md`

 * *Files identical despite different names*

### Comparing `faucetconfrpc-0.8/setup.py` & `faucetconfrpc-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `faucetconfrpc-0.8/LICENSE` & `faucetconfrpc-0.9/LICENSE`

 * *Files identical despite different names*

