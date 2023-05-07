# Comparing `tmp/fsai_grpc_api-0.0.98.tar.gz` & `tmp/fsai_grpc_api-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsai_grpc_api-0.0.98.tar", max compression
+gzip compressed data, was "fsai_grpc_api-0.0.99.tar", max compression
```

## Comparing `fsai_grpc_api-0.0.98.tar` & `fsai_grpc_api-0.0.99.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       70 2022-12-27 18:38:23.108725 fsai_grpc_api-0.0.98/README.md
--rw-r--r--   0        0        0    13487 2022-12-27 18:38:23.108725 fsai_grpc_api-0.0.98/fsai_grpc_api/ManifestStorageHelper.py
--rw-r--r--   0        0        0        0 2022-12-27 18:38:23.108725 fsai_grpc_api-0.0.98/fsai_grpc_api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-27 18:38:23.108725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/__init__.py
--rw-r--r--   0        0        0    26123 2022-12-27 18:38:23.108725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/area_of_interest_api_pb2.py
--rw-r--r--   0        0        0    10904 2022-12-27 18:38:23.108725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/area_of_interest_api_pb2_grpc.py
--rw-r--r--   0        0        0     4965 2022-12-27 18:38:23.108725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/category_api_pb2.py
--rw-r--r--   0        0        0     2770 2022-12-27 18:38:23.108725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/category_api_pb2_grpc.py
--rw-r--r--   0        0        0     8651 2022-12-27 18:38:23.108725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/detection_api_pb2.py
--rw-r--r--   0        0        0     2798 2022-12-27 18:38:23.108725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/detection_api_pb2_grpc.py
--rw-r--r--   0        0        0    32040 2022-12-27 18:38:23.108725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/detection_instance_api_pb2.py
--rw-r--r--   0        0        0    11321 2022-12-27 18:38:23.108725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/detection_instance_api_pb2_grpc.py
--rw-r--r--   0        0        0     5861 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/feature_api_pb2.py
--rw-r--r--   0        0        0     2742 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/feature_api_pb2_grpc.py
--rw-r--r--   0        0        0    16564 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/image_api_pb2.py
--rw-r--r--   0        0        0     6267 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/image_api_pb2_grpc.py
--rw-r--r--   0        0        0    12465 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/mission_api_pb2.py
--rw-r--r--   0        0        0     4479 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/mission_api_pb2_grpc.py
--rw-r--r--   0        0        0   122342 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/protoc_gen_validate/validate_pb2.py
--rw-r--r--   0        0        0      159 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/protoc_gen_validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0    18944 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/query_api_pb2.py
--rw-r--r--   0        0        0     4726 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/query_api_pb2_grpc.py
--rw-r--r--   0        0        0     4856 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/source_api_pb2.py
--rw-r--r--   0        0        0     2714 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/source_api_pb2_grpc.py
--rw-r--r--   0        0        0     6995 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/utils_pb2.py
--rw-r--r--   0        0        0      159 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/utils_pb2_grpc.py
--rw-r--r--   0        0        0     7198 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/workflow_api_pb2.py
--rw-r--r--   0        0        0     4518 2022-12-27 18:38:23.112725 fsai_grpc_api-0.0.98/fsai_grpc_api/protos/workflow_api_pb2_grpc.py
--rw-r--r--   0        0        0     1145 2022-12-27 18:38:23.684722 fsai_grpc_api-0.0.98/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 fsai_grpc_api-0.0.98/setup.py
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 fsai_grpc_api-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0       70 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/README.md
+-rw-r--r--   0        0        0    13487 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/ManifestStorageHelper.py
+-rw-r--r--   0        0        0        0 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/__init__.py
+-rw-r--r--   0        0        0    26123 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/area_of_interest_api_pb2.py
+-rw-r--r--   0        0        0    10904 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/area_of_interest_api_pb2_grpc.py
+-rw-r--r--   0        0        0     4965 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/category_api_pb2.py
+-rw-r--r--   0        0        0     2770 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/category_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8651 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/detection_api_pb2.py
+-rw-r--r--   0        0        0     2798 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/detection_api_pb2_grpc.py
+-rw-r--r--   0        0        0    32040 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/detection_instance_api_pb2.py
+-rw-r--r--   0        0        0    11321 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/detection_instance_api_pb2_grpc.py
+-rw-r--r--   0        0        0     5861 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/feature_api_pb2.py
+-rw-r--r--   0        0        0     2742 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/feature_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16564 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/image_api_pb2.py
+-rw-r--r--   0        0        0     6267 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/image_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16346 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/mission_api_pb2.py
+-rw-r--r--   0        0        0     6248 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/mission_api_pb2_grpc.py
+-rw-r--r--   0        0        0   122342 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/protoc_gen_validate/validate_pb2.py
+-rw-r--r--   0        0        0      159 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/protoc_gen_validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0    18944 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/query_api_pb2.py
+-rw-r--r--   0        0        0     4726 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/query_api_pb2_grpc.py
+-rw-r--r--   0        0        0     4856 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/source_api_pb2.py
+-rw-r--r--   0        0        0     2714 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/source_api_pb2_grpc.py
+-rw-r--r--   0        0        0     6995 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/utils_pb2.py
+-rw-r--r--   0        0        0      159 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/utils_pb2_grpc.py
+-rw-r--r--   0        0        0     7198 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/workflow_api_pb2.py
+-rw-r--r--   0        0        0     4518 2022-12-29 02:06:52.360810 fsai_grpc_api-0.0.99/fsai_grpc_api/protos/workflow_api_pb2_grpc.py
+-rw-r--r--   0        0        0     1145 2022-12-29 02:06:52.920800 fsai_grpc_api-0.0.99/pyproject.toml
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 fsai_grpc_api-0.0.99/setup.py
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 fsai_grpc_api-0.0.99/PKG-INFO
```

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/ManifestStorageHelper.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/ManifestStorageHelper.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/area_of_interest_api_pb2.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/area_of_interest_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/area_of_interest_api_pb2_grpc.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/area_of_interest_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/category_api_pb2.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/category_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/category_api_pb2_grpc.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/category_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/detection_api_pb2.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/detection_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/detection_api_pb2_grpc.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/detection_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/detection_instance_api_pb2.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/detection_instance_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/detection_instance_api_pb2_grpc.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/detection_instance_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/feature_api_pb2.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/feature_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/feature_api_pb2_grpc.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/feature_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/image_api_pb2.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/image_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/image_api_pb2_grpc.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/image_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/mission_api_pb2.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/mission_api_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='fsai_grpc_api/protos/mission_api.proto',
   package='',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n&fsai_grpc_api/protos/mission_api.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a fsai_grpc_api/protos/utils.proto\"\x98\x01\n\x07Mission\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"1\n\x14\x43reateMissionRequest\x12\x19\n\x07mission\x18\x01 \x01(\x0b\x32\x08.Mission\"T\n\x15\x43reateMissionResponse\x12 \n\x0b\x63hange_type\x18\x01 \x01(\x0e\x32\x0b.ChangeType\x12\x19\n\x07mission\x18\x02 \x01(\x0b\x32\x08.Mission\"0\n\x13ListMissionsRequest\x12\x19\n\x07mission\x18\x01 \x01(\x0b\x32\x08.Mission\"T\n\x14ListMissionsResponse\x12 \n\x0b\x63hange_type\x18\x01 \x01(\x0e\x32\x0b.ChangeType\x12\x1a\n\x08missions\x18\x02 \x03(\x0b\x32\x08.Mission2\x89\x01\n\nMissionApi\x12>\n\rCreateMission\x12\x15.CreateMissionRequest\x1a\x16.CreateMissionResponse\x12;\n\x0cListMissions\x12\x14.ListMissionsRequest\x1a\x15.ListMissionsResponseb\x06proto3'
+  serialized_pb=b'\n&fsai_grpc_api/protos/mission_api.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a fsai_grpc_api/protos/utils.proto\"\x98\x01\n\x07Mission\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"1\n\x14\x43reateMissionRequest\x12\x19\n\x07mission\x18\x01 \x01(\x0b\x32\x08.Mission\"T\n\x15\x43reateMissionResponse\x12 \n\x0b\x63hange_type\x18\x01 \x01(\x0e\x32\x0b.ChangeType\x12\x19\n\x07mission\x18\x02 \x01(\x0b\x32\x08.Mission\"0\n\x13ListMissionsRequest\x12\x19\n\x07mission\x18\x01 \x01(\x0b\x32\x08.Mission\"T\n\x14ListMissionsResponse\x12 \n\x0b\x63hange_type\x18\x01 \x01(\x0e\x32\x0b.ChangeType\x12\x1a\n\x08missions\x18\x02 \x03(\x0b\x32\x08.Mission\"2\n\x15GetMissionByIdRequest\x12\x19\n\x07mission\x18\x01 \x01(\x0b\x32\x08.Mission\"U\n\x16GetMissionByIdResponse\x12 \n\x0b\x63hange_type\x18\x01 \x01(\x0e\x32\x0b.ChangeType\x12\x19\n\x07mission\x18\x02 \x01(\x0b\x32\x08.Mission2\xcc\x01\n\nMissionApi\x12>\n\rCreateMission\x12\x15.CreateMissionRequest\x1a\x16.CreateMissionResponse\x12;\n\x0cListMissions\x12\x14.ListMissionsRequest\x1a\x15.ListMissionsResponse\x12\x41\n\x0eGetMissionById\x12\x16.GetMissionByIdRequest\x1a\x17.GetMissionByIdResponseb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,fsai__grpc__api_dot_protos_dot_utils__pb2.DESCRIPTOR,])
 
 
 
 
 _MISSION = _descriptor.Descriptor(
@@ -225,27 +225,103 @@
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=451,
   serialized_end=535,
 )
 
+
+_GETMISSIONBYIDREQUEST = _descriptor.Descriptor(
+  name='GetMissionByIdRequest',
+  full_name='GetMissionByIdRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='mission', full_name='GetMissionByIdRequest.mission', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=537,
+  serialized_end=587,
+)
+
+
+_GETMISSIONBYIDRESPONSE = _descriptor.Descriptor(
+  name='GetMissionByIdResponse',
+  full_name='GetMissionByIdResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='change_type', full_name='GetMissionByIdResponse.change_type', index=0,
+      number=1, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='mission', full_name='GetMissionByIdResponse.mission', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=589,
+  serialized_end=674,
+)
+
 _MISSION.fields_by_name['created_at'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _MISSION.fields_by_name['updated_at'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _CREATEMISSIONREQUEST.fields_by_name['mission'].message_type = _MISSION
 _CREATEMISSIONRESPONSE.fields_by_name['change_type'].enum_type = fsai__grpc__api_dot_protos_dot_utils__pb2._CHANGETYPE
 _CREATEMISSIONRESPONSE.fields_by_name['mission'].message_type = _MISSION
 _LISTMISSIONSREQUEST.fields_by_name['mission'].message_type = _MISSION
 _LISTMISSIONSRESPONSE.fields_by_name['change_type'].enum_type = fsai__grpc__api_dot_protos_dot_utils__pb2._CHANGETYPE
 _LISTMISSIONSRESPONSE.fields_by_name['missions'].message_type = _MISSION
+_GETMISSIONBYIDREQUEST.fields_by_name['mission'].message_type = _MISSION
+_GETMISSIONBYIDRESPONSE.fields_by_name['change_type'].enum_type = fsai__grpc__api_dot_protos_dot_utils__pb2._CHANGETYPE
+_GETMISSIONBYIDRESPONSE.fields_by_name['mission'].message_type = _MISSION
 DESCRIPTOR.message_types_by_name['Mission'] = _MISSION
 DESCRIPTOR.message_types_by_name['CreateMissionRequest'] = _CREATEMISSIONREQUEST
 DESCRIPTOR.message_types_by_name['CreateMissionResponse'] = _CREATEMISSIONRESPONSE
 DESCRIPTOR.message_types_by_name['ListMissionsRequest'] = _LISTMISSIONSREQUEST
 DESCRIPTOR.message_types_by_name['ListMissionsResponse'] = _LISTMISSIONSRESPONSE
+DESCRIPTOR.message_types_by_name['GetMissionByIdRequest'] = _GETMISSIONBYIDREQUEST
+DESCRIPTOR.message_types_by_name['GetMissionByIdResponse'] = _GETMISSIONBYIDRESPONSE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Mission = _reflection.GeneratedProtocolMessageType('Mission', (_message.Message,), {
   'DESCRIPTOR' : _MISSION,
   '__module__' : 'fsai_grpc_api.protos.mission_api_pb2'
   # @@protoc_insertion_point(class_scope:Mission)
   })
@@ -275,25 +351,39 @@
 ListMissionsResponse = _reflection.GeneratedProtocolMessageType('ListMissionsResponse', (_message.Message,), {
   'DESCRIPTOR' : _LISTMISSIONSRESPONSE,
   '__module__' : 'fsai_grpc_api.protos.mission_api_pb2'
   # @@protoc_insertion_point(class_scope:ListMissionsResponse)
   })
 _sym_db.RegisterMessage(ListMissionsResponse)
 
+GetMissionByIdRequest = _reflection.GeneratedProtocolMessageType('GetMissionByIdRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETMISSIONBYIDREQUEST,
+  '__module__' : 'fsai_grpc_api.protos.mission_api_pb2'
+  # @@protoc_insertion_point(class_scope:GetMissionByIdRequest)
+  })
+_sym_db.RegisterMessage(GetMissionByIdRequest)
+
+GetMissionByIdResponse = _reflection.GeneratedProtocolMessageType('GetMissionByIdResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETMISSIONBYIDRESPONSE,
+  '__module__' : 'fsai_grpc_api.protos.mission_api_pb2'
+  # @@protoc_insertion_point(class_scope:GetMissionByIdResponse)
+  })
+_sym_db.RegisterMessage(GetMissionByIdResponse)
+
 
 
 _MISSIONAPI = _descriptor.ServiceDescriptor(
   name='MissionApi',
   full_name='MissionApi',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=538,
-  serialized_end=675,
+  serialized_start=677,
+  serialized_end=881,
   methods=[
   _descriptor.MethodDescriptor(
     name='CreateMission',
     full_name='MissionApi.CreateMission',
     index=0,
     containing_service=None,
     input_type=_CREATEMISSIONREQUEST,
@@ -307,13 +397,23 @@
     index=1,
     containing_service=None,
     input_type=_LISTMISSIONSREQUEST,
     output_type=_LISTMISSIONSRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
+  _descriptor.MethodDescriptor(
+    name='GetMissionById',
+    full_name='MissionApi.GetMissionById',
+    index=2,
+    containing_service=None,
+    input_type=_GETMISSIONBYIDREQUEST,
+    output_type=_GETMISSIONBYIDRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_MISSIONAPI)
 
 DESCRIPTOR.services_by_name['MissionApi'] = _MISSIONAPI
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/mission_api_pb2_grpc.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/mission_api_pb2_grpc.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,19 @@
                 response_deserializer=fsai__grpc__api_dot_protos_dot_mission__api__pb2.CreateMissionResponse.FromString,
                 )
         self.ListMissions = channel.unary_unary(
                 '/MissionApi/ListMissions',
                 request_serializer=fsai__grpc__api_dot_protos_dot_mission__api__pb2.ListMissionsRequest.SerializeToString,
                 response_deserializer=fsai__grpc__api_dot_protos_dot_mission__api__pb2.ListMissionsResponse.FromString,
                 )
+        self.GetMissionById = channel.unary_unary(
+                '/MissionApi/GetMissionById',
+                request_serializer=fsai__grpc__api_dot_protos_dot_mission__api__pb2.GetMissionByIdRequest.SerializeToString,
+                response_deserializer=fsai__grpc__api_dot_protos_dot_mission__api__pb2.GetMissionByIdResponse.FromString,
+                )
 
 
 class MissionApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def CreateMission(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -37,27 +42,38 @@
 
     def ListMissions(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetMissionById(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_MissionApiServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CreateMission': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateMission,
                     request_deserializer=fsai__grpc__api_dot_protos_dot_mission__api__pb2.CreateMissionRequest.FromString,
                     response_serializer=fsai__grpc__api_dot_protos_dot_mission__api__pb2.CreateMissionResponse.SerializeToString,
             ),
             'ListMissions': grpc.unary_unary_rpc_method_handler(
                     servicer.ListMissions,
                     request_deserializer=fsai__grpc__api_dot_protos_dot_mission__api__pb2.ListMissionsRequest.FromString,
                     response_serializer=fsai__grpc__api_dot_protos_dot_mission__api__pb2.ListMissionsResponse.SerializeToString,
             ),
+            'GetMissionById': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetMissionById,
+                    request_deserializer=fsai__grpc__api_dot_protos_dot_mission__api__pb2.GetMissionByIdRequest.FromString,
+                    response_serializer=fsai__grpc__api_dot_protos_dot_mission__api__pb2.GetMissionByIdResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'MissionApi', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -93,7 +109,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/MissionApi/ListMissions',
             fsai__grpc__api_dot_protos_dot_mission__api__pb2.ListMissionsRequest.SerializeToString,
             fsai__grpc__api_dot_protos_dot_mission__api__pb2.ListMissionsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetMissionById(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/MissionApi/GetMissionById',
+            fsai__grpc__api_dot_protos_dot_mission__api__pb2.GetMissionByIdRequest.SerializeToString,
+            fsai__grpc__api_dot_protos_dot_mission__api__pb2.GetMissionByIdResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/protoc_gen_validate/validate_pb2.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/protoc_gen_validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/query_api_pb2.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/query_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/query_api_pb2_grpc.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/query_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/source_api_pb2.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/source_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/source_api_pb2_grpc.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/source_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/utils_pb2.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/workflow_api_pb2.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/workflow_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/fsai_grpc_api/protos/workflow_api_pb2_grpc.py` & `fsai_grpc_api-0.0.99/fsai_grpc_api/protos/workflow_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fsai_grpc_api-0.0.98/pyproject.toml` & `fsai_grpc_api-0.0.99/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fsai-grpc-api"
-version = "v0.0.98"
+version = "v0.0.99"
 description = "Auto-generate library for use with GRPC API."
 authors = ["Michael Mohamed <michael@foundationstack.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fsai-dev/fsai-cli-tools"
 repository = "https://github.com/fsai-dev/fsai-cli-tools"
```

### Comparing `fsai_grpc_api-0.0.98/setup.py` & `fsai_grpc_api-0.0.99/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'marshmallow>=3.17.1,<4.0.0',
  'protobuf>=4.21.11,<5.0.0',
  'pydash>=5.1.0,<6.0.0',
  'python-dateutil>=2.8.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'fsai-grpc-api',
-    'version': '0.0.98',
+    'version': '0.0.99',
     'description': 'Auto-generate library for use with GRPC API.',
     'long_description': '# Development\n\nTo re-generate the proto library, run `make proto-gen`\n',
     'author': 'Michael Mohamed',
     'author_email': 'michael@foundationstack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fsai-dev/fsai-cli-tools',
```

### Comparing `fsai_grpc_api-0.0.98/PKG-INFO` & `fsai_grpc_api-0.0.99/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsai-grpc-api
-Version: 0.0.98
+Version: 0.0.99
 Summary: Auto-generate library for use with GRPC API.
 Home-page: https://github.com/fsai-dev/fsai-cli-tools
 License: MIT
 Author: Michael Mohamed
 Author-email: michael@foundationstack.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

