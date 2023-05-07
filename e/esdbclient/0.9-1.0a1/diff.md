# Comparing `tmp/esdbclient-0.9.tar.gz` & `tmp/esdbclient-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esdbclient-0.9.tar", max compression
+gzip compressed data, was "esdbclient-1.0a1.tar", max compression
```

## Comparing `esdbclient-0.9.tar` & `esdbclient-1.0a1.tar`

### file list

```diff
@@ -1,26 +1,33 @@
--rw-r--r--   0        0        0     1520 2022-06-23 14:19:18.317032 esdbclient-0.9/LICENSE
--rw-r--r--   0        0        0    48510 2023-02-12 01:08:46.249759 esdbclient-0.9/README.md
--rw-r--r--   0        0        0      434 2023-02-12 00:54:11.519980 esdbclient-0.9/esdbclient/__init__.py
--rw-r--r--   0        0        0     7519 2023-02-12 01:03:15.566450 esdbclient-0.9/esdbclient/client.py
--rw-r--r--   0        0        0    18582 2023-02-12 00:54:11.835919 esdbclient-0.9/esdbclient/esdbapi.py
--rw-r--r--   0        0        0      800 2023-02-12 00:54:11.521056 esdbclient-0.9/esdbclient/events.py
--rw-r--r--   0        0        0      710 2022-06-23 14:19:18.318601 esdbclient-0.9/esdbclient/exceptions.py
--rw-r--r--   0        0        0     1790 2023-01-23 18:02:35.248448 esdbclient-0.9/esdbclient/protos/Grpc/code_pb2.py
--rw-r--r--   0        0        0    13555 2023-01-23 18:02:35.249448 esdbclient-0.9/esdbclient/protos/Grpc/code_pb2.pyi
--rw-r--r--   0        0        0      158 2022-11-06 16:49:34.017453 esdbclient-0.9/esdbclient/protos/Grpc/code_pb2_grpc.py
--rw-r--r--   0        0        0    43977 2023-01-31 13:52:51.273428 esdbclient-0.9/esdbclient/protos/Grpc/persistent_pb2.py
--rw-r--r--   0        0        0    73085 2023-01-31 13:52:51.274163 esdbclient-0.9/esdbclient/protos/Grpc/persistent_pb2.pyi
--rw-r--r--   0        0        0    15771 2023-01-31 13:52:51.274680 esdbclient-0.9/esdbclient/protos/Grpc/persistent_pb2_grpc.py
--rw-r--r--   0        0        0     3782 2023-01-23 18:02:35.250362 esdbclient-0.9/esdbclient/protos/Grpc/shared_pb2.py
--rw-r--r--   0        0        0     9874 2023-01-23 18:02:35.251226 esdbclient-0.9/esdbclient/protos/Grpc/shared_pb2.pyi
--rw-r--r--   0        0        0      158 2022-11-06 16:49:34.030872 esdbclient-0.9/esdbclient/protos/Grpc/shared_pb2_grpc.py
--rw-r--r--   0        0        0     1686 2023-01-23 18:02:35.252048 esdbclient-0.9/esdbclient/protos/Grpc/status_pb2.py
--rw-r--r--   0        0        0     2838 2023-01-23 18:02:35.252880 esdbclient-0.9/esdbclient/protos/Grpc/status_pb2.pyi
--rw-r--r--   0        0        0      158 2022-11-06 16:49:34.040459 esdbclient-0.9/esdbclient/protos/Grpc/status_pb2_grpc.py
--rw-r--r--   0        0        0    19933 2023-01-23 18:02:35.254530 esdbclient-0.9/esdbclient/protos/Grpc/streams_pb2.py
--rw-r--r--   0        0        0    71744 2023-01-23 18:02:35.257256 esdbclient-0.9/esdbclient/protos/Grpc/streams_pb2.pyi
--rw-r--r--   0        0        0     9787 2022-11-06 16:49:34.163884 esdbclient-0.9/esdbclient/protos/Grpc/streams_pb2_grpc.py
--rw-r--r--   0        0        0        0 2022-06-23 14:19:18.321130 esdbclient-0.9/esdbclient/py.typed
--rw-r--r--   0        0        0     2536 2023-02-12 01:12:22.638342 esdbclient-0.9/pyproject.toml
--rw-r--r--   0        0        0    50700 1970-01-01 00:00:00.000000 esdbclient-0.9/setup.py
--rw-r--r--   0        0        0    49802 1970-01-01 00:00:00.000000 esdbclient-0.9/PKG-INFO
+-rw-r--r--   0        0        0     1520 2022-06-23 14:19:18.317032 esdbclient-1.0a1/LICENSE
+-rw-r--r--   0        0        0    86403 2023-05-07 12:49:55.444028 esdbclient-1.0a1/README.md
+-rw-r--r--   0        0        0      434 2023-02-13 14:52:23.129600 esdbclient-1.0a1/esdbclient/__init__.py
+-rw-r--r--   0        0        0    30306 2023-05-06 01:57:28.748219 esdbclient-1.0a1/esdbclient/client.py
+-rw-r--r--   0        0        0    10774 2023-05-06 01:57:28.437362 esdbclient-1.0a1/esdbclient/connection.py
+-rw-r--r--   0        0        0    52086 2023-05-06 01:57:28.437903 esdbclient-1.0a1/esdbclient/esdbapi.py
+-rw-r--r--   0        0        0      800 2023-02-12 00:54:11.521056 esdbclient-1.0a1/esdbclient/events.py
+-rw-r--r--   0        0        0     2722 2023-05-06 00:00:09.029052 esdbclient-1.0a1/esdbclient/exceptions.py
+-rw-r--r--   0        0        0    13259 2023-05-04 18:02:58.100189 esdbclient-1.0a1/esdbclient/protos/Grpc/cluster_pb2.py
+-rw-r--r--   0        0        0    37436 2023-05-04 18:02:58.100620 esdbclient-1.0a1/esdbclient/protos/Grpc/cluster_pb2.pyi
+-rw-r--r--   0        0        0    19336 2023-05-04 18:02:58.101022 esdbclient-1.0a1/esdbclient/protos/Grpc/cluster_pb2_grpc.py
+-rw-r--r--   0        0        0     1790 2023-05-04 12:45:59.572583 esdbclient-1.0a1/esdbclient/protos/Grpc/code_pb2.py
+-rw-r--r--   0        0        0    13555 2023-05-04 12:45:57.273734 esdbclient-1.0a1/esdbclient/protos/Grpc/code_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-04 12:45:57.195931 esdbclient-1.0a1/esdbclient/protos/Grpc/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2817 2023-05-04 18:02:58.101379 esdbclient-1.0a1/esdbclient/protos/Grpc/gossip_pb2.py
+-rw-r--r--   0        0        0     5524 2023-05-04 18:02:58.101647 esdbclient-1.0a1/esdbclient/protos/Grpc/gossip_pb2.pyi
+-rw-r--r--   0        0        0     2752 2023-05-04 18:02:58.101900 esdbclient-1.0a1/esdbclient/protos/Grpc/gossip_pb2_grpc.py
+-rw-r--r--   0        0        0    22467 2023-05-04 12:45:59.544177 esdbclient-1.0a1/esdbclient/protos/Grpc/persistent_pb2.py
+-rw-r--r--   0        0        0    73220 2023-05-04 12:45:58.367039 esdbclient-1.0a1/esdbclient/protos/Grpc/persistent_pb2.pyi
+-rw-r--r--   0        0        0    15771 2023-05-04 12:45:59.569446 esdbclient-1.0a1/esdbclient/protos/Grpc/persistent_pb2_grpc.py
+-rw-r--r--   0        0        0     3782 2023-05-04 12:45:59.547001 esdbclient-1.0a1/esdbclient/protos/Grpc/shared_pb2.py
+-rw-r--r--   0        0        0     9874 2023-05-04 12:45:57.428467 esdbclient-1.0a1/esdbclient/protos/Grpc/shared_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-04 12:45:57.202606 esdbclient-1.0a1/esdbclient/protos/Grpc/shared_pb2_grpc.py
+-rw-r--r--   0        0        0     1686 2023-05-04 12:45:59.523110 esdbclient-1.0a1/esdbclient/protos/Grpc/status_pb2.py
+-rw-r--r--   0        0        0     2838 2023-05-04 12:45:57.271099 esdbclient-1.0a1/esdbclient/protos/Grpc/status_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-04 12:45:57.242089 esdbclient-1.0a1/esdbclient/protos/Grpc/status_pb2_grpc.py
+-rw-r--r--   0        0        0    19933 2023-05-04 12:45:59.582961 esdbclient-1.0a1/esdbclient/protos/Grpc/streams_pb2.py
+-rw-r--r--   0        0        0    71744 2023-05-04 12:45:58.391686 esdbclient-1.0a1/esdbclient/protos/Grpc/streams_pb2.pyi
+-rw-r--r--   0        0        0     9787 2023-05-04 12:45:57.418995 esdbclient-1.0a1/esdbclient/protos/Grpc/streams_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2022-06-23 14:19:18.321130 esdbclient-1.0a1/esdbclient/py.typed
+-rw-r--r--   0        0        0     2614 2023-05-07 12:55:12.001437 esdbclient-1.0a1/pyproject.toml
+-rw-r--r--   0        0        0    89564 1970-01-01 00:00:00.000000 esdbclient-1.0a1/setup.py
+-rw-r--r--   0        0        0    87733 1970-01-01 00:00:00.000000 esdbclient-1.0a1/PKG-INFO
```

### Comparing `esdbclient-0.9/LICENSE` & `esdbclient-1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `esdbclient-0.9/esdbclient/events.py` & `esdbclient-1.0a1/esdbclient/events.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.9/esdbclient/protos/Grpc/code_pb2.py` & `esdbclient-1.0a1/esdbclient/protos/Grpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.9/esdbclient/protos/Grpc/code_pb2.pyi` & `esdbclient-1.0a1/esdbclient/protos/Grpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-0.9/esdbclient/protos/Grpc/persistent_pb2.pyi` & `esdbclient-1.0a1/esdbclient/protos/Grpc/persistent_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
+import collections.abc
 import esdbclient.protos.Grpc.shared_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
+import sys
 import typing
-import typing_extensions
+
+if sys.version_info >= (3, 10):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class ReadReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
     class Options(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+        @typing_extensions.final
         class UUIDOption(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
             STRUCTURED_FIELD_NUMBER: builtins.int
             STRING_FIELD_NUMBER: builtins.int
             @property
             def structured(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
             @property
             def string(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
             def __init__(
                 self,
                 *,
-                structured: typing.Optional[
-                    esdbclient.protos.Grpc.shared_pb2.Empty
-                ] = ...,
-                string: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
+                structured: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
+                string: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
             ) -> None: ...
             def HasField(
                 self,
                 field_name: typing_extensions.Literal[
                     "content",
                     b"content",
                     "string",
@@ -55,41 +63,40 @@
                     b"string",
                     "structured",
                     b"structured",
                 ],
             ) -> None: ...
             def WhichOneof(
                 self, oneof_group: typing_extensions.Literal["content", b"content"]
-            ) -> typing.Optional[typing_extensions.Literal["structured", "string"]]: ...
+            ) -> typing_extensions.Literal["structured", "string"] | None: ...
 
         STREAM_IDENTIFIER_FIELD_NUMBER: builtins.int
         ALL_FIELD_NUMBER: builtins.int
         GROUP_NAME_FIELD_NUMBER: builtins.int
         BUFFER_SIZE_FIELD_NUMBER: builtins.int
         UUID_OPTION_FIELD_NUMBER: builtins.int
         @property
         def stream_identifier(
             self,
         ) -> esdbclient.protos.Grpc.shared_pb2.StreamIdentifier: ...
         @property
         def all(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
-        group_name: typing.Text
+        group_name: builtins.str
         buffer_size: builtins.int
         @property
         def uuid_option(self) -> global___ReadReq.Options.UUIDOption: ...
         def __init__(
             self,
             *,
-            stream_identifier: typing.Optional[
-                esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
-            ] = ...,
-            all: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
-            group_name: typing.Text = ...,
+            stream_identifier: esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
+            | None = ...,
+            all: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
+            group_name: builtins.str = ...,
             buffer_size: builtins.int = ...,
-            uuid_option: typing.Optional[global___ReadReq.Options.UUIDOption] = ...,
+            uuid_option: global___ReadReq.Options.UUIDOption | None = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "all",
                 b"all",
                 "stream_identifier",
@@ -116,61 +123,62 @@
                 "uuid_option",
                 b"uuid_option",
             ],
         ) -> None: ...
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal["stream_option", b"stream_option"],
-        ) -> typing.Optional[typing_extensions.Literal["stream_identifier", "all"]]: ...
+        ) -> typing_extensions.Literal["stream_identifier", "all"] | None: ...
 
+    @typing_extensions.final
     class Ack(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         ID_FIELD_NUMBER: builtins.int
         IDS_FIELD_NUMBER: builtins.int
         id: builtins.bytes
         @property
         def ids(
             self,
         ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
             esdbclient.protos.Grpc.shared_pb2.UUID
         ]: ...
         def __init__(
             self,
             *,
             id: builtins.bytes = ...,
-            ids: typing.Optional[
-                typing.Iterable[esdbclient.protos.Grpc.shared_pb2.UUID]
-            ] = ...,
+            ids: collections.abc.Iterable[esdbclient.protos.Grpc.shared_pb2.UUID]
+            | None = ...,
         ) -> None: ...
         def ClearField(
             self, field_name: typing_extensions.Literal["id", b"id", "ids", b"ids"]
         ) -> None: ...
 
+    @typing_extensions.final
     class Nack(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         class _Action:
             ValueType = typing.NewType("ValueType", builtins.int)
             V: typing_extensions.TypeAlias = ValueType
 
         class _ActionEnumTypeWrapper(
             google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[
                 ReadReq.Nack._Action.ValueType
             ],
             builtins.type,
-        ):
+        ):  # noqa: F821
             DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
             Unknown: ReadReq.Nack._Action.ValueType  # 0
             Park: ReadReq.Nack._Action.ValueType  # 1
             Retry: ReadReq.Nack._Action.ValueType  # 2
             Skip: ReadReq.Nack._Action.ValueType  # 3
             Stop: ReadReq.Nack._Action.ValueType  # 4
 
-        class Action(_Action, metaclass=_ActionEnumTypeWrapper):
-            pass
+        class Action(_Action, metaclass=_ActionEnumTypeWrapper): ...
         Unknown: ReadReq.Nack.Action.ValueType  # 0
         Park: ReadReq.Nack.Action.ValueType  # 1
         Retry: ReadReq.Nack.Action.ValueType  # 2
         Skip: ReadReq.Nack.Action.ValueType  # 3
         Stop: ReadReq.Nack.Action.ValueType  # 4
 
         ID_FIELD_NUMBER: builtins.int
@@ -181,24 +189,23 @@
         @property
         def ids(
             self,
         ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
             esdbclient.protos.Grpc.shared_pb2.UUID
         ]: ...
         action: global___ReadReq.Nack.Action.ValueType
-        reason: typing.Text
+        reason: builtins.str
         def __init__(
             self,
             *,
             id: builtins.bytes = ...,
-            ids: typing.Optional[
-                typing.Iterable[esdbclient.protos.Grpc.shared_pb2.UUID]
-            ] = ...,
+            ids: collections.abc.Iterable[esdbclient.protos.Grpc.shared_pb2.UUID]
+            | None = ...,
             action: global___ReadReq.Nack.Action.ValueType = ...,
-            reason: typing.Text = ...,
+            reason: builtins.str = ...,
         ) -> None: ...
         def ClearField(
             self,
             field_name: typing_extensions.Literal[
                 "action", b"action", "id", b"id", "ids", b"ids", "reason", b"reason"
             ],
         ) -> None: ...
@@ -211,17 +218,17 @@
     @property
     def ack(self) -> global___ReadReq.Ack: ...
     @property
     def nack(self) -> global___ReadReq.Nack: ...
     def __init__(
         self,
         *,
-        options: typing.Optional[global___ReadReq.Options] = ...,
-        ack: typing.Optional[global___ReadReq.Ack] = ...,
-        nack: typing.Optional[global___ReadReq.Nack] = ...,
+        options: global___ReadReq.Options | None = ...,
+        ack: global___ReadReq.Ack | None = ...,
+        nack: global___ReadReq.Nack | None = ...,
     ) -> None: ...
     def HasField(
         self,
         field_name: typing_extensions.Literal[
             "ack", b"ack", "content", b"content", "nack", b"nack", "options", b"options"
         ],
     ) -> builtins.bool: ...
@@ -229,38 +236,43 @@
         self,
         field_name: typing_extensions.Literal[
             "ack", b"ack", "content", b"content", "nack", b"nack", "options", b"options"
         ],
     ) -> None: ...
     def WhichOneof(
         self, oneof_group: typing_extensions.Literal["content", b"content"]
-    ) -> typing.Optional[typing_extensions.Literal["options", "ack", "nack"]]: ...
+    ) -> typing_extensions.Literal["options", "ack", "nack"] | None: ...
 
 global___ReadReq = ReadReq
 
+@typing_extensions.final
 class ReadResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
     class ReadEvent(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+        @typing_extensions.final
         class RecordedEvent(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+            @typing_extensions.final
             class MetadataEntry(google.protobuf.message.Message):
                 DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
                 KEY_FIELD_NUMBER: builtins.int
                 VALUE_FIELD_NUMBER: builtins.int
-                key: typing.Text
-                value: typing.Text
+                key: builtins.str
+                value: builtins.str
                 def __init__(
                     self,
                     *,
-                    key: typing.Text = ...,
-                    value: typing.Text = ...,
+                    key: builtins.str = ...,
+                    value: builtins.str = ...,
                 ) -> None: ...
                 def ClearField(
                     self,
                     field_name: typing_extensions.Literal[
                         "key", b"key", "value", b"value"
                     ],
                 ) -> None: ...
@@ -282,31 +294,29 @@
             stream_revision: builtins.int
             prepare_position: builtins.int
             commit_position: builtins.int
             @property
             def metadata(
                 self,
             ) -> google.protobuf.internal.containers.ScalarMap[
-                typing.Text, typing.Text
+                builtins.str, builtins.str
             ]: ...
             custom_metadata: builtins.bytes
             data: builtins.bytes
             def __init__(
                 self,
                 *,
-                id: typing.Optional[esdbclient.protos.Grpc.shared_pb2.UUID] = ...,
-                stream_identifier: typing.Optional[
-                    esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
-                ] = ...,
+                id: esdbclient.protos.Grpc.shared_pb2.UUID | None = ...,
+                stream_identifier: esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
+                | None = ...,
                 stream_revision: builtins.int = ...,
                 prepare_position: builtins.int = ...,
                 commit_position: builtins.int = ...,
-                metadata: typing.Optional[
-                    typing.Mapping[typing.Text, typing.Text]
-                ] = ...,
+                metadata: collections.abc.Mapping[builtins.str, builtins.str]
+                | None = ...,
                 custom_metadata: builtins.bytes = ...,
                 data: builtins.bytes = ...,
             ) -> None: ...
             def HasField(
                 self,
                 field_name: typing_extensions.Literal[
                     "id", b"id", "stream_identifier", b"stream_identifier"
@@ -349,22 +359,20 @@
         def no_position(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         retry_count: builtins.int
         @property
         def no_retry_count(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         def __init__(
             self,
             *,
-            event: typing.Optional[global___ReadResp.ReadEvent.RecordedEvent] = ...,
-            link: typing.Optional[global___ReadResp.ReadEvent.RecordedEvent] = ...,
+            event: global___ReadResp.ReadEvent.RecordedEvent | None = ...,
+            link: global___ReadResp.ReadEvent.RecordedEvent | None = ...,
             commit_position: builtins.int = ...,
-            no_position: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
+            no_position: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
             retry_count: builtins.int = ...,
-            no_retry_count: typing.Optional[
-                esdbclient.protos.Grpc.shared_pb2.Empty
-            ] = ...,
+            no_retry_count: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "commit_position",
                 b"commit_position",
                 "count",
@@ -403,32 +411,30 @@
                 "retry_count",
                 b"retry_count",
             ],
         ) -> None: ...
         @typing.overload
         def WhichOneof(
             self, oneof_group: typing_extensions.Literal["count", b"count"]
-        ) -> typing.Optional[
-            typing_extensions.Literal["retry_count", "no_retry_count"]
-        ]: ...
+        ) -> typing_extensions.Literal["retry_count", "no_retry_count"] | None: ...
         @typing.overload
         def WhichOneof(
             self, oneof_group: typing_extensions.Literal["position", b"position"]
-        ) -> typing.Optional[
-            typing_extensions.Literal["commit_position", "no_position"]
-        ]: ...
+        ) -> typing_extensions.Literal["commit_position", "no_position"] | None: ...
 
+    @typing_extensions.final
     class SubscriptionConfirmation(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         SUBSCRIPTION_ID_FIELD_NUMBER: builtins.int
-        subscription_id: typing.Text
+        subscription_id: builtins.str
         def __init__(
             self,
             *,
-            subscription_id: typing.Text = ...,
+            subscription_id: builtins.str = ...,
         ) -> None: ...
         def ClearField(
             self,
             field_name: typing_extensions.Literal[
                 "subscription_id", b"subscription_id"
             ],
         ) -> None: ...
@@ -440,18 +446,17 @@
     @property
     def subscription_confirmation(
         self,
     ) -> global___ReadResp.SubscriptionConfirmation: ...
     def __init__(
         self,
         *,
-        event: typing.Optional[global___ReadResp.ReadEvent] = ...,
-        subscription_confirmation: typing.Optional[
-            global___ReadResp.SubscriptionConfirmation
-        ] = ...,
+        event: global___ReadResp.ReadEvent | None = ...,
+        subscription_confirmation: global___ReadResp.SubscriptionConfirmation
+        | None = ...,
     ) -> None: ...
     def HasField(
         self,
         field_name: typing_extensions.Literal[
             "content",
             b"content",
             "event",
@@ -469,74 +474,73 @@
             b"event",
             "subscription_confirmation",
             b"subscription_confirmation",
         ],
     ) -> None: ...
     def WhichOneof(
         self, oneof_group: typing_extensions.Literal["content", b"content"]
-    ) -> typing.Optional[
-        typing_extensions.Literal["event", "subscription_confirmation"]
-    ]: ...
+    ) -> typing_extensions.Literal["event", "subscription_confirmation"] | None: ...
 
 global___ReadResp = ReadResp
 
+@typing_extensions.final
 class CreateReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _ConsumerStrategy:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
     class _ConsumerStrategyEnumTypeWrapper(
         google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[
             CreateReq._ConsumerStrategy.ValueType
         ],
         builtins.type,
-    ):
+    ):  # noqa: F821
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         DispatchToSingle: CreateReq._ConsumerStrategy.ValueType  # 0
         RoundRobin: CreateReq._ConsumerStrategy.ValueType  # 1
         Pinned: CreateReq._ConsumerStrategy.ValueType  # 2
 
     class ConsumerStrategy(
         _ConsumerStrategy, metaclass=_ConsumerStrategyEnumTypeWrapper
-    ):
-        pass
+    ): ...
     DispatchToSingle: CreateReq.ConsumerStrategy.ValueType  # 0
     RoundRobin: CreateReq.ConsumerStrategy.ValueType  # 1
     Pinned: CreateReq.ConsumerStrategy.ValueType  # 2
 
+    @typing_extensions.final
     class Options(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         STREAM_FIELD_NUMBER: builtins.int
         ALL_FIELD_NUMBER: builtins.int
         STREAM_IDENTIFIER_FIELD_NUMBER: builtins.int
         GROUP_NAME_FIELD_NUMBER: builtins.int
         SETTINGS_FIELD_NUMBER: builtins.int
         @property
         def stream(self) -> global___CreateReq.StreamOptions: ...
         @property
         def all(self) -> global___CreateReq.AllOptions: ...
         @property
         def stream_identifier(
             self,
         ) -> esdbclient.protos.Grpc.shared_pb2.StreamIdentifier: ...
-        group_name: typing.Text
+        group_name: builtins.str
         @property
         def settings(self) -> global___CreateReq.Settings: ...
         def __init__(
             self,
             *,
-            stream: typing.Optional[global___CreateReq.StreamOptions] = ...,
-            all: typing.Optional[global___CreateReq.AllOptions] = ...,
-            stream_identifier: typing.Optional[
-                esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
-            ] = ...,
-            group_name: typing.Text = ...,
-            settings: typing.Optional[global___CreateReq.Settings] = ...,
+            stream: global___CreateReq.StreamOptions | None = ...,
+            all: global___CreateReq.AllOptions | None = ...,
+            stream_identifier: esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
+            | None = ...,
+            group_name: builtins.str = ...,
+            settings: global___CreateReq.Settings | None = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "all",
                 b"all",
                 "settings",
@@ -565,18 +569,20 @@
                 "stream_option",
                 b"stream_option",
             ],
         ) -> None: ...
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal["stream_option", b"stream_option"],
-        ) -> typing.Optional[typing_extensions.Literal["stream", "all"]]: ...
+        ) -> typing_extensions.Literal["stream", "all"] | None: ...
 
+    @typing_extensions.final
     class StreamOptions(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         STREAM_IDENTIFIER_FIELD_NUMBER: builtins.int
         REVISION_FIELD_NUMBER: builtins.int
         START_FIELD_NUMBER: builtins.int
         END_FIELD_NUMBER: builtins.int
         @property
         def stream_identifier(
             self,
@@ -585,20 +591,19 @@
         @property
         def start(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         @property
         def end(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         def __init__(
             self,
             *,
-            stream_identifier: typing.Optional[
-                esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
-            ] = ...,
+            stream_identifier: esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
+            | None = ...,
             revision: builtins.int = ...,
-            start: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
-            end: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
+            start: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
+            end: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "end",
                 b"end",
                 "revision",
@@ -627,38 +632,42 @@
             ],
         ) -> None: ...
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal[
                 "revision_option", b"revision_option"
             ],
-        ) -> typing.Optional[typing_extensions.Literal["revision", "start", "end"]]: ...
+        ) -> typing_extensions.Literal["revision", "start", "end"] | None: ...
 
+    @typing_extensions.final
     class AllOptions(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+        @typing_extensions.final
         class FilterOptions(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+            @typing_extensions.final
             class Expression(google.protobuf.message.Message):
                 DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
                 REGEX_FIELD_NUMBER: builtins.int
                 PREFIX_FIELD_NUMBER: builtins.int
-                regex: typing.Text
+                regex: builtins.str
                 @property
                 def prefix(
                     self,
                 ) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[
-                    typing.Text
+                    builtins.str
                 ]: ...
                 def __init__(
                     self,
                     *,
-                    regex: typing.Text = ...,
-                    prefix: typing.Optional[typing.Iterable[typing.Text]] = ...,
+                    regex: builtins.str = ...,
+                    prefix: collections.abc.Iterable[builtins.str] | None = ...,
                 ) -> None: ...
                 def ClearField(
                     self,
                     field_name: typing_extensions.Literal[
                         "prefix", b"prefix", "regex", b"regex"
                     ],
                 ) -> None: ...
@@ -679,22 +688,20 @@
             max: builtins.int
             @property
             def count(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
             checkpointIntervalMultiplier: builtins.int
             def __init__(
                 self,
                 *,
-                stream_identifier: typing.Optional[
-                    global___CreateReq.AllOptions.FilterOptions.Expression
-                ] = ...,
-                event_type: typing.Optional[
-                    global___CreateReq.AllOptions.FilterOptions.Expression
-                ] = ...,
+                stream_identifier: global___CreateReq.AllOptions.FilterOptions.Expression
+                | None = ...,
+                event_type: global___CreateReq.AllOptions.FilterOptions.Expression
+                | None = ...,
                 max: builtins.int = ...,
-                count: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
+                count: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
                 checkpointIntervalMultiplier: builtins.int = ...,
             ) -> None: ...
             def HasField(
                 self,
                 field_name: typing_extensions.Literal[
                     "count",
                     b"count",
@@ -728,21 +735,21 @@
                     "window",
                     b"window",
                 ],
             ) -> None: ...
             @typing.overload
             def WhichOneof(
                 self, oneof_group: typing_extensions.Literal["filter", b"filter"]
-            ) -> typing.Optional[
-                typing_extensions.Literal["stream_identifier", "event_type"]
-            ]: ...
+            ) -> (
+                typing_extensions.Literal["stream_identifier", "event_type"] | None
+            ): ...
             @typing.overload
             def WhichOneof(
                 self, oneof_group: typing_extensions.Literal["window", b"window"]
-            ) -> typing.Optional[typing_extensions.Literal["max", "count"]]: ...
+            ) -> typing_extensions.Literal["max", "count"] | None: ...
 
         POSITION_FIELD_NUMBER: builtins.int
         START_FIELD_NUMBER: builtins.int
         END_FIELD_NUMBER: builtins.int
         FILTER_FIELD_NUMBER: builtins.int
         NO_FILTER_FIELD_NUMBER: builtins.int
         @property
@@ -754,19 +761,19 @@
         @property
         def filter(self) -> global___CreateReq.AllOptions.FilterOptions: ...
         @property
         def no_filter(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         def __init__(
             self,
             *,
-            position: typing.Optional[global___CreateReq.Position] = ...,
-            start: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
-            end: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
-            filter: typing.Optional[global___CreateReq.AllOptions.FilterOptions] = ...,
-            no_filter: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
+            position: global___CreateReq.Position | None = ...,
+            start: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
+            end: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
+            filter: global___CreateReq.AllOptions.FilterOptions | None = ...,
+            no_filter: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "all_option",
                 b"all_option",
                 "end",
@@ -801,23 +808,25 @@
                 "start",
                 b"start",
             ],
         ) -> None: ...
         @typing.overload
         def WhichOneof(
             self, oneof_group: typing_extensions.Literal["all_option", b"all_option"]
-        ) -> typing.Optional[typing_extensions.Literal["position", "start", "end"]]: ...
+        ) -> typing_extensions.Literal["position", "start", "end"] | None: ...
         @typing.overload
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal["filter_option", b"filter_option"],
-        ) -> typing.Optional[typing_extensions.Literal["filter", "no_filter"]]: ...
+        ) -> typing_extensions.Literal["filter", "no_filter"] | None: ...
 
+    @typing_extensions.final
     class Position(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         COMMIT_POSITION_FIELD_NUMBER: builtins.int
         PREPARE_POSITION_FIELD_NUMBER: builtins.int
         commit_position: builtins.int
         prepare_position: builtins.int
         def __init__(
             self,
             *,
@@ -830,16 +839,18 @@
                 "commit_position",
                 b"commit_position",
                 "prepare_position",
                 b"prepare_position",
             ],
         ) -> None: ...
 
+    @typing_extensions.final
     class Settings(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         RESOLVE_LINKS_FIELD_NUMBER: builtins.int
         REVISION_FIELD_NUMBER: builtins.int
         EXTRA_STATISTICS_FIELD_NUMBER: builtins.int
         MAX_RETRY_COUNT_FIELD_NUMBER: builtins.int
         MIN_CHECKPOINT_COUNT_FIELD_NUMBER: builtins.int
         MAX_CHECKPOINT_COUNT_FIELD_NUMBER: builtins.int
         MAX_SUBSCRIBER_COUNT_FIELD_NUMBER: builtins.int
@@ -863,15 +874,15 @@
         read_batch_size: builtins.int
         history_buffer_size: builtins.int
         named_consumer_strategy: global___CreateReq.ConsumerStrategy.ValueType
         message_timeout_ticks: builtins.int
         message_timeout_ms: builtins.int
         checkpoint_after_ticks: builtins.int
         checkpoint_after_ms: builtins.int
-        consumer_strategy: typing.Text
+        consumer_strategy: builtins.str
         def __init__(
             self,
             *,
             resolve_links: builtins.bool = ...,
             revision: builtins.int = ...,
             extra_statistics: builtins.bool = ...,
             max_retry_count: builtins.int = ...,
@@ -882,15 +893,15 @@
             read_batch_size: builtins.int = ...,
             history_buffer_size: builtins.int = ...,
             named_consumer_strategy: global___CreateReq.ConsumerStrategy.ValueType = ...,
             message_timeout_ticks: builtins.int = ...,
             message_timeout_ms: builtins.int = ...,
             checkpoint_after_ticks: builtins.int = ...,
             checkpoint_after_ms: builtins.int = ...,
-            consumer_strategy: typing.Text = ...,
+            consumer_strategy: builtins.str = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "checkpoint_after",
                 b"checkpoint_after",
                 "checkpoint_after_ms",
@@ -948,106 +959,111 @@
         ) -> None: ...
         @typing.overload
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal[
                 "checkpoint_after", b"checkpoint_after"
             ],
-        ) -> typing.Optional[
+        ) -> (
             typing_extensions.Literal["checkpoint_after_ticks", "checkpoint_after_ms"]
-        ]: ...
+            | None
+        ): ...
         @typing.overload
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal[
                 "message_timeout", b"message_timeout"
             ],
-        ) -> typing.Optional[
+        ) -> (
             typing_extensions.Literal["message_timeout_ticks", "message_timeout_ms"]
-        ]: ...
+            | None
+        ): ...
 
     OPTIONS_FIELD_NUMBER: builtins.int
     @property
     def options(self) -> global___CreateReq.Options: ...
     def __init__(
         self,
         *,
-        options: typing.Optional[global___CreateReq.Options] = ...,
+        options: global___CreateReq.Options | None = ...,
     ) -> None: ...
     def HasField(
         self, field_name: typing_extensions.Literal["options", b"options"]
     ) -> builtins.bool: ...
     def ClearField(
         self, field_name: typing_extensions.Literal["options", b"options"]
     ) -> None: ...
 
 global___CreateReq = CreateReq
 
+@typing_extensions.final
 class CreateResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     def __init__(
         self,
     ) -> None: ...
 
 global___CreateResp = CreateResp
 
+@typing_extensions.final
 class UpdateReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _ConsumerStrategy:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
     class _ConsumerStrategyEnumTypeWrapper(
         google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[
             UpdateReq._ConsumerStrategy.ValueType
         ],
         builtins.type,
-    ):
+    ):  # noqa: F821
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         DispatchToSingle: UpdateReq._ConsumerStrategy.ValueType  # 0
         RoundRobin: UpdateReq._ConsumerStrategy.ValueType  # 1
         Pinned: UpdateReq._ConsumerStrategy.ValueType  # 2
 
     class ConsumerStrategy(
         _ConsumerStrategy, metaclass=_ConsumerStrategyEnumTypeWrapper
-    ):
-        pass
+    ): ...
     DispatchToSingle: UpdateReq.ConsumerStrategy.ValueType  # 0
     RoundRobin: UpdateReq.ConsumerStrategy.ValueType  # 1
     Pinned: UpdateReq.ConsumerStrategy.ValueType  # 2
 
+    @typing_extensions.final
     class Options(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         STREAM_FIELD_NUMBER: builtins.int
         ALL_FIELD_NUMBER: builtins.int
         STREAM_IDENTIFIER_FIELD_NUMBER: builtins.int
         GROUP_NAME_FIELD_NUMBER: builtins.int
         SETTINGS_FIELD_NUMBER: builtins.int
         @property
         def stream(self) -> global___UpdateReq.StreamOptions: ...
         @property
         def all(self) -> global___UpdateReq.AllOptions: ...
         @property
         def stream_identifier(
             self,
         ) -> esdbclient.protos.Grpc.shared_pb2.StreamIdentifier: ...
-        group_name: typing.Text
+        group_name: builtins.str
         @property
         def settings(self) -> global___UpdateReq.Settings: ...
         def __init__(
             self,
             *,
-            stream: typing.Optional[global___UpdateReq.StreamOptions] = ...,
-            all: typing.Optional[global___UpdateReq.AllOptions] = ...,
-            stream_identifier: typing.Optional[
-                esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
-            ] = ...,
-            group_name: typing.Text = ...,
-            settings: typing.Optional[global___UpdateReq.Settings] = ...,
+            stream: global___UpdateReq.StreamOptions | None = ...,
+            all: global___UpdateReq.AllOptions | None = ...,
+            stream_identifier: esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
+            | None = ...,
+            group_name: builtins.str = ...,
+            settings: global___UpdateReq.Settings | None = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "all",
                 b"all",
                 "settings",
@@ -1076,18 +1092,20 @@
                 "stream_option",
                 b"stream_option",
             ],
         ) -> None: ...
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal["stream_option", b"stream_option"],
-        ) -> typing.Optional[typing_extensions.Literal["stream", "all"]]: ...
+        ) -> typing_extensions.Literal["stream", "all"] | None: ...
 
+    @typing_extensions.final
     class StreamOptions(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         STREAM_IDENTIFIER_FIELD_NUMBER: builtins.int
         REVISION_FIELD_NUMBER: builtins.int
         START_FIELD_NUMBER: builtins.int
         END_FIELD_NUMBER: builtins.int
         @property
         def stream_identifier(
             self,
@@ -1096,20 +1114,19 @@
         @property
         def start(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         @property
         def end(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         def __init__(
             self,
             *,
-            stream_identifier: typing.Optional[
-                esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
-            ] = ...,
+            stream_identifier: esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
+            | None = ...,
             revision: builtins.int = ...,
-            start: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
-            end: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
+            start: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
+            end: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "end",
                 b"end",
                 "revision",
@@ -1138,33 +1155,35 @@
             ],
         ) -> None: ...
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal[
                 "revision_option", b"revision_option"
             ],
-        ) -> typing.Optional[typing_extensions.Literal["revision", "start", "end"]]: ...
+        ) -> typing_extensions.Literal["revision", "start", "end"] | None: ...
 
+    @typing_extensions.final
     class AllOptions(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         POSITION_FIELD_NUMBER: builtins.int
         START_FIELD_NUMBER: builtins.int
         END_FIELD_NUMBER: builtins.int
         @property
         def position(self) -> global___UpdateReq.Position: ...
         @property
         def start(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         @property
         def end(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         def __init__(
             self,
             *,
-            position: typing.Optional[global___UpdateReq.Position] = ...,
-            start: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
-            end: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
+            position: global___UpdateReq.Position | None = ...,
+            start: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
+            end: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "all_option",
                 b"all_option",
                 "end",
@@ -1186,18 +1205,20 @@
                 b"position",
                 "start",
                 b"start",
             ],
         ) -> None: ...
         def WhichOneof(
             self, oneof_group: typing_extensions.Literal["all_option", b"all_option"]
-        ) -> typing.Optional[typing_extensions.Literal["position", "start", "end"]]: ...
+        ) -> typing_extensions.Literal["position", "start", "end"] | None: ...
 
+    @typing_extensions.final
     class Position(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         COMMIT_POSITION_FIELD_NUMBER: builtins.int
         PREPARE_POSITION_FIELD_NUMBER: builtins.int
         commit_position: builtins.int
         prepare_position: builtins.int
         def __init__(
             self,
             *,
@@ -1210,16 +1231,18 @@
                 "commit_position",
                 b"commit_position",
                 "prepare_position",
                 b"prepare_position",
             ],
         ) -> None: ...
 
+    @typing_extensions.final
     class Settings(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         RESOLVE_LINKS_FIELD_NUMBER: builtins.int
         REVISION_FIELD_NUMBER: builtins.int
         EXTRA_STATISTICS_FIELD_NUMBER: builtins.int
         MAX_RETRY_COUNT_FIELD_NUMBER: builtins.int
         MIN_CHECKPOINT_COUNT_FIELD_NUMBER: builtins.int
         MAX_CHECKPOINT_COUNT_FIELD_NUMBER: builtins.int
         MAX_SUBSCRIBER_COUNT_FIELD_NUMBER: builtins.int
@@ -1323,75 +1346,81 @@
         ) -> None: ...
         @typing.overload
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal[
                 "checkpoint_after", b"checkpoint_after"
             ],
-        ) -> typing.Optional[
+        ) -> (
             typing_extensions.Literal["checkpoint_after_ticks", "checkpoint_after_ms"]
-        ]: ...
+            | None
+        ): ...
         @typing.overload
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal[
                 "message_timeout", b"message_timeout"
             ],
-        ) -> typing.Optional[
+        ) -> (
             typing_extensions.Literal["message_timeout_ticks", "message_timeout_ms"]
-        ]: ...
+            | None
+        ): ...
 
     OPTIONS_FIELD_NUMBER: builtins.int
     @property
     def options(self) -> global___UpdateReq.Options: ...
     def __init__(
         self,
         *,
-        options: typing.Optional[global___UpdateReq.Options] = ...,
+        options: global___UpdateReq.Options | None = ...,
     ) -> None: ...
     def HasField(
         self, field_name: typing_extensions.Literal["options", b"options"]
     ) -> builtins.bool: ...
     def ClearField(
         self, field_name: typing_extensions.Literal["options", b"options"]
     ) -> None: ...
 
 global___UpdateReq = UpdateReq
 
+@typing_extensions.final
 class UpdateResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     def __init__(
         self,
     ) -> None: ...
 
 global___UpdateResp = UpdateResp
 
+@typing_extensions.final
 class DeleteReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
     class Options(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         STREAM_IDENTIFIER_FIELD_NUMBER: builtins.int
         ALL_FIELD_NUMBER: builtins.int
         GROUP_NAME_FIELD_NUMBER: builtins.int
         @property
         def stream_identifier(
             self,
         ) -> esdbclient.protos.Grpc.shared_pb2.StreamIdentifier: ...
         @property
         def all(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
-        group_name: typing.Text
+        group_name: builtins.str
         def __init__(
             self,
             *,
-            stream_identifier: typing.Optional[
-                esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
-            ] = ...,
-            all: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
-            group_name: typing.Text = ...,
+            stream_identifier: esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
+            | None = ...,
+            all: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
+            group_name: builtins.str = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "all",
                 b"all",
                 "stream_identifier",
@@ -1412,64 +1441,68 @@
                 "stream_option",
                 b"stream_option",
             ],
         ) -> None: ...
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal["stream_option", b"stream_option"],
-        ) -> typing.Optional[typing_extensions.Literal["stream_identifier", "all"]]: ...
+        ) -> typing_extensions.Literal["stream_identifier", "all"] | None: ...
 
     OPTIONS_FIELD_NUMBER: builtins.int
     @property
     def options(self) -> global___DeleteReq.Options: ...
     def __init__(
         self,
         *,
-        options: typing.Optional[global___DeleteReq.Options] = ...,
+        options: global___DeleteReq.Options | None = ...,
     ) -> None: ...
     def HasField(
         self, field_name: typing_extensions.Literal["options", b"options"]
     ) -> builtins.bool: ...
     def ClearField(
         self, field_name: typing_extensions.Literal["options", b"options"]
     ) -> None: ...
 
 global___DeleteReq = DeleteReq
 
+@typing_extensions.final
 class DeleteResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     def __init__(
         self,
     ) -> None: ...
 
 global___DeleteResp = DeleteResp
 
+@typing_extensions.final
 class GetInfoReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
     class Options(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         STREAM_IDENTIFIER_FIELD_NUMBER: builtins.int
         ALL_FIELD_NUMBER: builtins.int
         GROUP_NAME_FIELD_NUMBER: builtins.int
         @property
         def stream_identifier(
             self,
         ) -> esdbclient.protos.Grpc.shared_pb2.StreamIdentifier: ...
         @property
         def all(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
-        group_name: typing.Text
+        group_name: builtins.str
         def __init__(
             self,
             *,
-            stream_identifier: typing.Optional[
-                esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
-            ] = ...,
-            all: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
-            group_name: typing.Text = ...,
+            stream_identifier: esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
+            | None = ...,
+            all: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
+            group_name: builtins.str = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "all",
                 b"all",
                 "stream_identifier",
@@ -1490,42 +1523,44 @@
                 "stream_option",
                 b"stream_option",
             ],
         ) -> None: ...
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal["stream_option", b"stream_option"],
-        ) -> typing.Optional[typing_extensions.Literal["stream_identifier", "all"]]: ...
+        ) -> typing_extensions.Literal["stream_identifier", "all"] | None: ...
 
     OPTIONS_FIELD_NUMBER: builtins.int
     @property
     def options(self) -> global___GetInfoReq.Options: ...
     def __init__(
         self,
         *,
-        options: typing.Optional[global___GetInfoReq.Options] = ...,
+        options: global___GetInfoReq.Options | None = ...,
     ) -> None: ...
     def HasField(
         self, field_name: typing_extensions.Literal["options", b"options"]
     ) -> builtins.bool: ...
     def ClearField(
         self, field_name: typing_extensions.Literal["options", b"options"]
     ) -> None: ...
 
 global___GetInfoReq = GetInfoReq
 
+@typing_extensions.final
 class GetInfoResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     SUBSCRIPTION_INFO_FIELD_NUMBER: builtins.int
     @property
     def subscription_info(self) -> global___SubscriptionInfo: ...
     def __init__(
         self,
         *,
-        subscription_info: typing.Optional[global___SubscriptionInfo] = ...,
+        subscription_info: global___SubscriptionInfo | None = ...,
     ) -> None: ...
     def HasField(
         self,
         field_name: typing_extensions.Literal[
             "subscription_info", b"subscription_info"
         ],
     ) -> builtins.bool: ...
@@ -1534,54 +1569,58 @@
         field_name: typing_extensions.Literal[
             "subscription_info", b"subscription_info"
         ],
     ) -> None: ...
 
 global___GetInfoResp = GetInfoResp
 
+@typing_extensions.final
 class SubscriptionInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
     class ConnectionInfo(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         FROM_FIELD_NUMBER: builtins.int
         USERNAME_FIELD_NUMBER: builtins.int
         AVERAGE_ITEMS_PER_SECOND_FIELD_NUMBER: builtins.int
         TOTAL_ITEMS_FIELD_NUMBER: builtins.int
         COUNT_SINCE_LAST_MEASUREMENT_FIELD_NUMBER: builtins.int
         OBSERVED_MEASUREMENTS_FIELD_NUMBER: builtins.int
         AVAILABLE_SLOTS_FIELD_NUMBER: builtins.int
         IN_FLIGHT_MESSAGES_FIELD_NUMBER: builtins.int
         CONNECTION_NAME_FIELD_NUMBER: builtins.int
-        username: typing.Text
+        username: builtins.str
         average_items_per_second: builtins.int
         total_items: builtins.int
         count_since_last_measurement: builtins.int
         @property
         def observed_measurements(
             self,
         ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
             global___SubscriptionInfo.Measurement
         ]: ...
         available_slots: builtins.int
         in_flight_messages: builtins.int
-        connection_name: typing.Text
+        connection_name: builtins.str
         def __init__(
             self,
             *,
-            username: typing.Text = ...,
+            username: builtins.str = ...,
             average_items_per_second: builtins.int = ...,
             total_items: builtins.int = ...,
             count_since_last_measurement: builtins.int = ...,
-            observed_measurements: typing.Optional[
-                typing.Iterable[global___SubscriptionInfo.Measurement]
-            ] = ...,
+            observed_measurements: collections.abc.Iterable[
+                global___SubscriptionInfo.Measurement
+            ]
+            | None = ...,
             available_slots: builtins.int = ...,
             in_flight_messages: builtins.int = ...,
-            connection_name: typing.Text = ...,
+            connection_name: builtins.str = ...,
         ) -> None: ...
         def ClearField(
             self,
             field_name: typing_extensions.Literal[
                 "available_slots",
                 b"available_slots",
                 "average_items_per_second",
@@ -1599,24 +1638,26 @@
                 "total_items",
                 b"total_items",
                 "username",
                 b"username",
             ],
         ) -> None: ...
 
+    @typing_extensions.final
     class Measurement(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: typing.Text
+        key: builtins.str
         value: builtins.int
         def __init__(
             self,
             *,
-            key: typing.Text = ...,
+            key: builtins.str = ...,
             value: builtins.int = ...,
         ) -> None: ...
         def ClearField(
             self,
             field_name: typing_extensions.Literal["key", b"key", "value", b"value"],
         ) -> None: ...
 
@@ -1644,78 +1685,77 @@
     LIVE_BUFFER_COUNT_FIELD_NUMBER: builtins.int
     RETRY_BUFFER_COUNT_FIELD_NUMBER: builtins.int
     TOTAL_IN_FLIGHT_MESSAGES_FIELD_NUMBER: builtins.int
     OUTSTANDING_MESSAGES_COUNT_FIELD_NUMBER: builtins.int
     NAMED_CONSUMER_STRATEGY_FIELD_NUMBER: builtins.int
     MAX_SUBSCRIBER_COUNT_FIELD_NUMBER: builtins.int
     PARKED_MESSAGE_COUNT_FIELD_NUMBER: builtins.int
-    event_source: typing.Text
-    group_name: typing.Text
-    status: typing.Text
+    event_source: builtins.str
+    group_name: builtins.str
+    status: builtins.str
     @property
     def connections(
         self,
     ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
         global___SubscriptionInfo.ConnectionInfo
     ]: ...
     average_per_second: builtins.int
     total_items: builtins.int
     count_since_last_measurement: builtins.int
-    last_checkpointed_event_position: typing.Text
-    last_known_event_position: typing.Text
+    last_checkpointed_event_position: builtins.str
+    last_known_event_position: builtins.str
     resolve_link_tos: builtins.bool
-    start_from: typing.Text
+    start_from: builtins.str
     message_timeout_milliseconds: builtins.int
     extra_statistics: builtins.bool
     max_retry_count: builtins.int
     live_buffer_size: builtins.int
     buffer_size: builtins.int
     read_batch_size: builtins.int
     check_point_after_milliseconds: builtins.int
     min_check_point_count: builtins.int
     max_check_point_count: builtins.int
     read_buffer_count: builtins.int
     live_buffer_count: builtins.int
     retry_buffer_count: builtins.int
     total_in_flight_messages: builtins.int
     outstanding_messages_count: builtins.int
-    named_consumer_strategy: typing.Text
+    named_consumer_strategy: builtins.str
     max_subscriber_count: builtins.int
     parked_message_count: builtins.int
     def __init__(
         self,
         *,
-        event_source: typing.Text = ...,
-        group_name: typing.Text = ...,
-        status: typing.Text = ...,
-        connections: typing.Optional[
-            typing.Iterable[global___SubscriptionInfo.ConnectionInfo]
-        ] = ...,
+        event_source: builtins.str = ...,
+        group_name: builtins.str = ...,
+        status: builtins.str = ...,
+        connections: collections.abc.Iterable[global___SubscriptionInfo.ConnectionInfo]
+        | None = ...,
         average_per_second: builtins.int = ...,
         total_items: builtins.int = ...,
         count_since_last_measurement: builtins.int = ...,
-        last_checkpointed_event_position: typing.Text = ...,
-        last_known_event_position: typing.Text = ...,
+        last_checkpointed_event_position: builtins.str = ...,
+        last_known_event_position: builtins.str = ...,
         resolve_link_tos: builtins.bool = ...,
-        start_from: typing.Text = ...,
+        start_from: builtins.str = ...,
         message_timeout_milliseconds: builtins.int = ...,
         extra_statistics: builtins.bool = ...,
         max_retry_count: builtins.int = ...,
         live_buffer_size: builtins.int = ...,
         buffer_size: builtins.int = ...,
         read_batch_size: builtins.int = ...,
         check_point_after_milliseconds: builtins.int = ...,
         min_check_point_count: builtins.int = ...,
         max_check_point_count: builtins.int = ...,
         read_buffer_count: builtins.int = ...,
         live_buffer_count: builtins.int = ...,
         retry_buffer_count: builtins.int = ...,
         total_in_flight_messages: builtins.int = ...,
         outstanding_messages_count: builtins.int = ...,
-        named_consumer_strategy: typing.Text = ...,
+        named_consumer_strategy: builtins.str = ...,
         max_subscriber_count: builtins.int = ...,
         parked_message_count: builtins.int = ...,
     ) -> None: ...
     def ClearField(
         self,
         field_name: typing_extensions.Literal[
             "average_per_second",
@@ -1775,44 +1815,46 @@
             "total_items",
             b"total_items",
         ],
     ) -> None: ...
 
 global___SubscriptionInfo = SubscriptionInfo
 
+@typing_extensions.final
 class ReplayParkedReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
     class Options(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         GROUP_NAME_FIELD_NUMBER: builtins.int
         STREAM_IDENTIFIER_FIELD_NUMBER: builtins.int
         ALL_FIELD_NUMBER: builtins.int
         STOP_AT_FIELD_NUMBER: builtins.int
         NO_LIMIT_FIELD_NUMBER: builtins.int
-        group_name: typing.Text
+        group_name: builtins.str
         @property
         def stream_identifier(
             self,
         ) -> esdbclient.protos.Grpc.shared_pb2.StreamIdentifier: ...
         @property
         def all(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         stop_at: builtins.int
         @property
         def no_limit(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         def __init__(
             self,
             *,
-            group_name: typing.Text = ...,
-            stream_identifier: typing.Optional[
-                esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
-            ] = ...,
-            all: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
+            group_name: builtins.str = ...,
+            stream_identifier: esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
+            | None = ...,
+            all: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
             stop_at: builtins.int = ...,
-            no_limit: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
+            no_limit: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "all",
                 b"all",
                 "no_limit",
@@ -1846,64 +1888,68 @@
                 b"stream_option",
             ],
         ) -> None: ...
         @typing.overload
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal["stop_at_option", b"stop_at_option"],
-        ) -> typing.Optional[typing_extensions.Literal["stop_at", "no_limit"]]: ...
+        ) -> typing_extensions.Literal["stop_at", "no_limit"] | None: ...
         @typing.overload
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal["stream_option", b"stream_option"],
-        ) -> typing.Optional[typing_extensions.Literal["stream_identifier", "all"]]: ...
+        ) -> typing_extensions.Literal["stream_identifier", "all"] | None: ...
 
     OPTIONS_FIELD_NUMBER: builtins.int
     @property
     def options(self) -> global___ReplayParkedReq.Options: ...
     def __init__(
         self,
         *,
-        options: typing.Optional[global___ReplayParkedReq.Options] = ...,
+        options: global___ReplayParkedReq.Options | None = ...,
     ) -> None: ...
     def HasField(
         self, field_name: typing_extensions.Literal["options", b"options"]
     ) -> builtins.bool: ...
     def ClearField(
         self, field_name: typing_extensions.Literal["options", b"options"]
     ) -> None: ...
 
 global___ReplayParkedReq = ReplayParkedReq
 
+@typing_extensions.final
 class ReplayParkedResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     def __init__(
         self,
     ) -> None: ...
 
 global___ReplayParkedResp = ReplayParkedResp
 
+@typing_extensions.final
 class ListReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
     class Options(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         LIST_ALL_SUBSCRIPTIONS_FIELD_NUMBER: builtins.int
         LIST_FOR_STREAM_FIELD_NUMBER: builtins.int
         @property
         def list_all_subscriptions(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         @property
         def list_for_stream(self) -> global___ListReq.StreamOption: ...
         def __init__(
             self,
             *,
-            list_all_subscriptions: typing.Optional[
-                esdbclient.protos.Grpc.shared_pb2.Empty
-            ] = ...,
-            list_for_stream: typing.Optional[global___ListReq.StreamOption] = ...,
+            list_all_subscriptions: esdbclient.protos.Grpc.shared_pb2.Empty
+            | None = ...,
+            list_for_stream: global___ListReq.StreamOption | None = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "list_all_subscriptions",
                 b"list_all_subscriptions",
                 "list_for_stream",
@@ -1921,33 +1967,34 @@
                 b"list_for_stream",
                 "list_option",
                 b"list_option",
             ],
         ) -> None: ...
         def WhichOneof(
             self, oneof_group: typing_extensions.Literal["list_option", b"list_option"]
-        ) -> typing.Optional[
+        ) -> (
             typing_extensions.Literal["list_all_subscriptions", "list_for_stream"]
-        ]: ...
+            | None
+        ): ...
 
+    @typing_extensions.final
     class StreamOption(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         STREAM_FIELD_NUMBER: builtins.int
         ALL_FIELD_NUMBER: builtins.int
         @property
         def stream(self) -> esdbclient.protos.Grpc.shared_pb2.StreamIdentifier: ...
         @property
         def all(self) -> esdbclient.protos.Grpc.shared_pb2.Empty: ...
         def __init__(
             self,
             *,
-            stream: typing.Optional[
-                esdbclient.protos.Grpc.shared_pb2.StreamIdentifier
-            ] = ...,
-            all: typing.Optional[esdbclient.protos.Grpc.shared_pb2.Empty] = ...,
+            stream: esdbclient.protos.Grpc.shared_pb2.StreamIdentifier | None = ...,
+            all: esdbclient.protos.Grpc.shared_pb2.Empty | None = ...,
         ) -> None: ...
         def HasField(
             self,
             field_name: typing_extensions.Literal[
                 "all", b"all", "stream", b"stream", "stream_option", b"stream_option"
             ],
         ) -> builtins.bool: ...
@@ -1956,47 +2003,47 @@
             field_name: typing_extensions.Literal[
                 "all", b"all", "stream", b"stream", "stream_option", b"stream_option"
             ],
         ) -> None: ...
         def WhichOneof(
             self,
             oneof_group: typing_extensions.Literal["stream_option", b"stream_option"],
-        ) -> typing.Optional[typing_extensions.Literal["stream", "all"]]: ...
+        ) -> typing_extensions.Literal["stream", "all"] | None: ...
 
     OPTIONS_FIELD_NUMBER: builtins.int
     @property
     def options(self) -> global___ListReq.Options: ...
     def __init__(
         self,
         *,
-        options: typing.Optional[global___ListReq.Options] = ...,
+        options: global___ListReq.Options | None = ...,
     ) -> None: ...
     def HasField(
         self, field_name: typing_extensions.Literal["options", b"options"]
     ) -> builtins.bool: ...
     def ClearField(
         self, field_name: typing_extensions.Literal["options", b"options"]
     ) -> None: ...
 
 global___ListReq = ListReq
 
+@typing_extensions.final
 class ListResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     SUBSCRIPTIONS_FIELD_NUMBER: builtins.int
     @property
     def subscriptions(
         self,
     ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
         global___SubscriptionInfo
     ]: ...
     def __init__(
         self,
         *,
-        subscriptions: typing.Optional[
-            typing.Iterable[global___SubscriptionInfo]
-        ] = ...,
+        subscriptions: collections.abc.Iterable[global___SubscriptionInfo] | None = ...,
     ) -> None: ...
     def ClearField(
         self, field_name: typing_extensions.Literal["subscriptions", b"subscriptions"]
     ) -> None: ...
 
 global___ListResp = ListResp
```

### Comparing `esdbclient-0.9/esdbclient/protos/Grpc/persistent_pb2_grpc.py` & `esdbclient-1.0a1/esdbclient/protos/Grpc/persistent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.9/esdbclient/protos/Grpc/shared_pb2.py` & `esdbclient-1.0a1/esdbclient/protos/Grpc/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.9/esdbclient/protos/Grpc/shared_pb2.pyi` & `esdbclient-1.0a1/esdbclient/protos/Grpc/shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-0.9/esdbclient/protos/Grpc/status_pb2.py` & `esdbclient-1.0a1/esdbclient/protos/Grpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.9/esdbclient/protos/Grpc/status_pb2.pyi` & `esdbclient-1.0a1/esdbclient/protos/Grpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-0.9/esdbclient/protos/Grpc/streams_pb2.py` & `esdbclient-1.0a1/esdbclient/protos/Grpc/streams_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.9/esdbclient/protos/Grpc/streams_pb2.pyi` & `esdbclient-1.0a1/esdbclient/protos/Grpc/streams_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-0.9/esdbclient/protos/Grpc/streams_pb2_grpc.py` & `esdbclient-1.0a1/esdbclient/protos/Grpc/streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.9/pyproject.toml` & `esdbclient-1.0a1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esdbclient"
-version = "0.9"
+version = "1.0a1"
 description = "Python gRPC Client for EventStoreDB"
 authors = [
     "John Bywater <john.bywater@appropriatesoftware.net>",
 ]
 license = "BSD 3-Clause"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -20,17 +20,20 @@
 readme = "README.md"
 homepage = "https://github.com/pyeventsourcing/esdbclient"
 repository = "https://github.com/pyeventsourcing/esdbclient"
 include = ["esdbclient/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
-grpcio = ">=1.51.0,<1.52.0"  # 1.52.0 hangs on fork
-protobuf = "^4.21.0"
+grpcio = ">=1.51.0,!=1.52.*"  # 1.52.0 hangs on fork
+protobuf = ">=3.11.0"
+#protobuf = "^4.21.0"
+#protobuf = ">=3.11.0,<3.21.0"
 typing_extensions = "*"
+dnspython = "^2.3.0"
 
 [tool.poetry.dev-dependencies]
 black = { version = "*", allow-prereleases = true }
 flake8 = "*"
 flake8-broken-line = "*"
 flake8-bugbear = "*"
 flake8-coding = "*"
```

### Comparing `esdbclient-0.9/PKG-INFO` & `esdbclient-1.0a1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,3113 +1,5484 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6573 6462  : 2.1.Name: esdb
 00000020: 636c 6965 6e74 0a56 6572 7369 6f6e 3a20  client.Version: 
-00000030: 302e 390a 5375 6d6d 6172 793a 2050 7974  0.9.Summary: Pyt
-00000040: 686f 6e20 6752 5043 2043 6c69 656e 7420  hon gRPC Client 
-00000050: 666f 7220 4576 656e 7453 746f 7265 4442  for EventStoreDB
-00000060: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
-00000070: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00000080: 7965 7665 6e74 736f 7572 6369 6e67 2f65  yeventsourcing/e
-00000090: 7364 6263 6c69 656e 740a 4c69 6365 6e73  sdbclient.Licens
-000000a0: 653a 2042 5344 2033 2d43 6c61 7573 650a  e: BSD 3-Clause.
-000000b0: 4175 7468 6f72 3a20 4a6f 686e 2042 7977  Author: John Byw
-000000c0: 6174 6572 0a41 7574 686f 722d 656d 6169  ater.Author-emai
-000000d0: 6c3a 206a 6f68 6e2e 6279 7761 7465 7240  l: john.bywater@
-000000e0: 6170 7072 6f70 7269 6174 6573 6f66 7477  appropriatesoftw
-000000f0: 6172 652e 6e65 740a 5265 7175 6972 6573  are.net.Requires
-00000100: 2d50 7974 686f 6e3a 203e 3d33 2e37 2c3c  -Python: >=3.7,<
-00000110: 342e 300a 436c 6173 7369 6669 6572 3a20  4.0.Classifier: 
-00000120: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-00000130: 7573 203a 3a20 3320 2d20 416c 7068 610a  us :: 3 - Alpha.
-00000140: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
-00000150: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000160: 7665 6420 3a3a 2042 5344 204c 6963 656e  ved :: BSD Licen
-00000170: 7365 0a43 6c61 7373 6966 6965 723a 204c  se.Classifier: L
-00000180: 6963 656e 7365 203a 3a20 4f74 6865 722f  icense :: Other/
-00000190: 5072 6f70 7269 6574 6172 7920 4c69 6365  Proprietary Lice
-000001a0: 6e73 650a 436c 6173 7369 6669 6572 3a20  nse.Classifier: 
-000001b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001c0: 7561 6765 203a 3a20 5079 7468 6f6e 0a43  uage :: Python.C
-000001d0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000001e0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0a43  :: Python :: 3.C
-00000200: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000210: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000220: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
-00000230: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000240: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000250: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000260: 2e38 0a43 6c61 7373 6966 6965 723a 2050  .8.Classifier: P
-00000270: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000280: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000290: 2033 2e39 0a43 6c61 7373 6966 6965 723a   3.9.Classifier:
-000002a0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000002b0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002c0: 3a3a 2033 2e31 300a 436c 6173 7369 6669  :: 3.10.Classifi
-000002d0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-000002e0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002f0: 6f6e 203a 3a20 332e 3131 0a43 6c61 7373  on :: 3.11.Class
-00000300: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000310: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000320: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
-00000330: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000340: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000350: 7974 686f 6e20 3a3a 2033 2e31 300a 436c  ython :: 3.10.Cl
-00000360: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000370: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000380: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
-00000390: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000003a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000003b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000003c0: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
-000003d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000003e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000003f0: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
-00000400: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000410: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000420: 3a3a 2033 2e39 0a52 6571 7569 7265 732d  :: 3.9.Requires-
-00000430: 4469 7374 3a20 6772 7063 696f 2028 3e3d  Dist: grpcio (>=
-00000440: 312e 3531 2e30 2c3c 312e 3532 2e30 290a  1.51.0,<1.52.0).
-00000450: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000460: 726f 746f 6275 6620 283e 3d34 2e32 312e  rotobuf (>=4.21.
-00000470: 302c 3c35 2e30 2e30 290a 5265 7175 6972  0,<5.0.0).Requir
-00000480: 6573 2d44 6973 743a 2074 7970 696e 675f  es-Dist: typing_
-00000490: 6578 7465 6e73 696f 6e73 0a50 726f 6a65  extensions.Proje
-000004a0: 6374 2d55 524c 3a20 5265 706f 7369 746f  ct-URL: Reposito
-000004b0: 7279 2c20 6874 7470 733a 2f2f 6769 7468  ry, https://gith
-000004c0: 7562 2e63 6f6d 2f70 7965 7665 6e74 736f  ub.com/pyeventso
-000004d0: 7572 6369 6e67 2f65 7364 6263 6c69 656e  urcing/esdbclien
-000004e0: 740a 4465 7363 7269 7074 696f 6e2d 436f  t.Description-Co
-000004f0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00000500: 2f6d 6172 6b64 6f77 6e0a 0a23 2050 7974  /markdown..# Pyt
-00000510: 686f 6e20 6752 5043 2043 6c69 656e 7420  hon gRPC Client 
-00000520: 666f 7220 4576 656e 7453 746f 7265 4442  for EventStoreDB
-00000530: 0a0a 5468 6973 2070 6163 6b61 6765 2070  ..This package p
-00000540: 726f 7669 6465 7320 6120 5079 7468 6f6e  rovides a Python
-00000550: 2067 5250 4320 636c 6965 6e74 2066 6f72   gRPC client for
-00000560: 0a5b 4576 656e 7453 746f 7265 4442 5d28  .[EventStoreDB](
-00000570: 6874 7470 733a 2f2f 7777 772e 6576 656e  https://www.even
-00000580: 7473 746f 7265 2e63 6f6d 2f29 2e0a 0a54  tstore.com/)...T
-00000590: 6869 7320 636c 6965 6e74 2068 6173 2062  his client has b
-000005a0: 6565 6e20 6465 7665 6c6f 7065 6420 616e  een developed an
-000005b0: 6420 7465 7374 6564 2074 6f20 776f 726b  d tested to work
-000005c0: 2077 6974 6820 4576 656e 7453 746f 7265   with EventStore
-000005d0: 4442 204c 5453 0a76 6572 7369 6f6e 7320  DB LTS.versions 
-000005e0: 3231 2e31 3020 616e 6420 3231 2e31 302c  21.10 and 21.10,
-000005f0: 2077 6974 686f 7574 2061 6e64 2077 6974   without and wit
-00000600: 686f 7574 2053 534c 2f54 4c53 2065 6e61  hout SSL/TLS ena
-00000610: 626c 6564 206f 6e20 626f 7468 0a74 6865  bled on both.the
-00000620: 7365 2076 6572 7369 6f6e 732c 2061 6e64  se versions, and
-00000630: 2077 6974 6820 5079 7468 6f6e 2076 6572   with Python ver
-00000640: 7369 6f6e 7320 332e 372c 2033 2e38 2c20  sions 3.7, 3.8, 
-00000650: 332e 392c 2033 2e31 302c 2061 6e64 2033  3.9, 3.10, and 3
-00000660: 2e31 310a 6163 726f 7373 2061 6c6c 206f  .11.across all o
-00000670: 6620 7468 6520 6162 6f76 652e 2054 6865  f the above. The
-00000680: 2074 6573 7420 636f 7665 7261 6765 2069   test coverage i
-00000690: 7320 3130 3025 2069 6e63 6c75 6469 6e67  s 100% including
-000006a0: 2062 7261 6e63 6820 636f 7665 7261 6765   branch coverage
-000006b0: 2e0a 0a41 6c6c 2074 6865 2063 6f64 6520  ...All the code 
-000006c0: 696e 2074 6869 7320 7061 636b 6167 6520  in this package 
-000006d0: 6861 7320 7479 7069 6e67 2061 6e6e 6f74  has typing annot
-000006e0: 6174 696f 6e73 2e20 5468 6520 7374 6174  ations. The stat
-000006f0: 6963 2074 7970 696e 670a 616e 6e6f 7461  ic typing.annota
-00000700: 7469 6f6e 7320 6368 6563 6b65 6420 7265  tions checked re
-00000710: 6c61 7469 7665 6c79 2073 7472 6963 746c  latively strictl
-00000720: 7920 7769 7468 206d 7970 792e 0a0a 4e6f  y with mypy...No
-00000730: 7420 616c 6c20 7468 6520 6665 6174 7572  t all the featur
-00000740: 6573 206f 6620 7468 6520 4576 656e 7453  es of the EventS
-00000750: 746f 7265 4442 2041 5049 2061 7265 2070  toreDB API are p
-00000760: 7265 7365 6e74 6564 0a62 7920 7468 6973  resented.by this
-00000770: 2063 6c69 656e 7420 696e 2069 7473 2063   client in its c
-00000780: 7572 7265 6e74 2066 6f72 6d2c 2068 6f77  urrent form, how
-00000790: 6576 6572 206d 616e 7920 6f66 2074 6865  ever many of the
-000007a0: 206d 6f73 740a 7573 6566 756c 2061 7370   most.useful asp
-000007b0: 6563 7473 2061 7265 2070 7265 7365 6e74  ects are present
-000007c0: 6564 2069 6e20 616e 2065 6173 792d 746f  ed in an easy-to
-000007d0: 2d75 7365 2069 6e74 6572 6661 6365 2028  -use interface (
-000007e0: 7365 6520 6265 6c6f 7729 2e0a 466f 7220  see below)..For 
-000007f0: 616e 2065 7861 6d70 6c65 206f 6620 7573  an example of us
-00000800: 6167 652c 2073 6565 2074 6865 205b 6576  age, see the [ev
-00000810: 656e 7473 6f75 7263 696e 672d 6576 656e  entsourcing-even
-00000820: 7473 746f 7265 6462 5d28 0a68 7474 7073  tstoredb](.https
-00000830: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
-00000840: 6576 656e 7473 6f75 7263 696e 672f 6576  eventsourcing/ev
-00000850: 656e 7473 6f75 7263 696e 672d 6576 656e  entsourcing-even
-00000860: 7473 746f 7265 6462 2920 7061 636b 6167  tstoredb) packag
-00000870: 652e 0a0a 2323 2054 6162 6c65 206f 6620  e...## Table of 
-00000880: 636f 6e74 656e 7473 0a0a 3c21 2d2d 2054  contents..<!-- T
-00000890: 4f43 202d 2d3e 0a2a 205b 496e 7374 616c  OC -->.* [Instal
-000008a0: 6c61 7469 6f6e 5d28 2369 6e73 7461 6c6c  lation](#install
-000008b0: 6174 696f 6e29 0a2a 205b 5365 7276 6572  ation).* [Server
-000008c0: 5d28 2373 6572 7665 7229 0a20 202a 205b  ](#server).  * [
-000008d0: 5374 6172 7420 4576 656e 7453 746f 7265  Start EventStore
-000008e0: 4442 5d28 2373 7461 7274 2d65 7665 6e74  DB](#start-event
-000008f0: 7374 6f72 6564 6229 0a20 202a 205b 5374  storedb).  * [St
-00000900: 6f70 2045 7665 6e74 5374 6f72 6544 425d  op EventStoreDB]
-00000910: 2823 7374 6f70 2d65 7665 6e74 7374 6f72  (#stop-eventstor
-00000920: 6564 6229 0a2a 205b 436c 6965 6e74 5d28  edb).* [Client](
-00000930: 2363 6c69 656e 7429 0a2a 205b 5374 7265  #client).* [Stre
-00000940: 616d 735d 2823 7374 7265 616d 7329 0a20  ams](#streams). 
-00000950: 202a 205b 4170 7065 6e64 2065 7665 6e74   * [Append event
-00000960: 735d 2823 6170 7065 6e64 2d65 7665 6e74  s](#append-event
-00000970: 7329 0a20 202a 205b 4765 7420 6375 7272  s).  * [Get curr
-00000980: 656e 7420 7374 7265 616d 2070 6f73 6974  ent stream posit
-00000990: 696f 6e5d 2823 6765 742d 6375 7272 656e  ion](#get-curren
-000009a0: 742d 7374 7265 616d 2d70 6f73 6974 696f  t-stream-positio
-000009b0: 6e29 0a20 202a 205b 5265 6164 2073 7472  n).  * [Read str
-000009c0: 6561 6d20 6576 656e 7473 5d28 2372 6561  eam events](#rea
-000009d0: 642d 7374 7265 616d 2d65 7665 6e74 7329  d-stream-events)
-000009e0: 0a20 202a 205b 4964 656d 706f 7465 6e74  .  * [Idempotent
-000009f0: 2077 7269 7465 735d 2823 6964 656d 706f   writes](#idempo
-00000a00: 7465 6e74 2d77 7269 7465 7329 0a20 202a  tent-writes).  *
-00000a10: 205b 5265 6164 2061 6c6c 2072 6563 6f72   [Read all recor
-00000a20: 6465 6420 6576 656e 7473 5d28 2372 6561  ded events](#rea
-00000a30: 642d 616c 6c2d 7265 636f 7264 6564 2d65  d-all-recorded-e
-00000a40: 7665 6e74 7329 0a20 202a 205b 4765 7420  vents).  * [Get 
-00000a50: 6375 7272 656e 7420 636f 6d6d 6974 2070  current commit p
-00000a60: 6f73 6974 696f 6e5d 2823 6765 742d 6375  osition](#get-cu
-00000a70: 7272 656e 742d 636f 6d6d 6974 2d70 6f73  rrent-commit-pos
-00000a80: 6974 696f 6e29 0a2a 205b 5375 6273 6372  ition).* [Subscr
-00000a90: 6970 7469 6f6e 735d 2823 7375 6273 6372  iptions](#subscr
-00000aa0: 6970 7469 6f6e 7329 0a20 202a 205b 4361  iptions).  * [Ca
-00000ab0: 7463 682d 7570 2073 7562 7363 7269 7074  tch-up subscript
-00000ac0: 696f 6e73 5d28 2363 6174 6368 2d75 702d  ions](#catch-up-
-00000ad0: 7375 6273 6372 6970 7469 6f6e 7329 0a20  subscriptions). 
-00000ae0: 202a 205b 5065 7273 6973 7465 6e74 2073   * [Persistent s
-00000af0: 7562 7363 7269 7074 696f 6e73 5d28 2370  ubscriptions](#p
-00000b00: 6572 7369 7374 656e 742d 7375 6273 6372  ersistent-subscr
-00000b10: 6970 7469 6f6e 7329 0a2a 205b 4e6f 7465  iptions).* [Note
-00000b20: 735d 2823 6e6f 7465 7329 0a20 202a 205b  s](#notes).  * [
-00000b30: 5265 6775 6c61 7220 6578 7072 6573 7369  Regular expressi
-00000b40: 6f6e 2066 696c 7465 7273 5d28 2372 6567  on filters](#reg
-00000b50: 756c 6172 2d65 7870 7265 7373 696f 6e2d  ular-expression-
-00000b60: 6669 6c74 6572 7329 0a20 202a 205b 5468  filters).  * [Th
-00000b70: 6520 4e65 7745 7665 6e74 2063 6c61 7373  e NewEvent class
-00000b80: 5d28 2374 6865 2d6e 6577 6576 656e 742d  ](#the-newevent-
-00000b90: 636c 6173 7329 0a20 202a 205b 5468 6520  class).  * [The 
-00000ba0: 5265 636f 7264 6564 4576 656e 7420 636c  RecordedEvent cl
-00000bb0: 6173 735d 2823 7468 652d 7265 636f 7264  ass](#the-record
-00000bc0: 6564 6576 656e 742d 636c 6173 7329 0a2a  edevent-class).*
-00000bd0: 205b 436f 6e74 7269 6275 746f 7273 5d28   [Contributors](
-00000be0: 2363 6f6e 7472 6962 7574 6f72 7329 0a20  #contributors). 
-00000bf0: 202a 205b 496e 7374 616c 6c20 506f 6574   * [Install Poet
-00000c00: 7279 5d28 2369 6e73 7461 6c6c 2d70 6f65  ry](#install-poe
-00000c10: 7472 7929 0a20 202a 205b 5365 7475 7020  try).  * [Setup 
-00000c20: 666f 7220 5079 4368 6172 6d20 7573 6572  for PyCharm user
-00000c30: 735d 2823 7365 7475 702d 666f 722d 7079  s](#setup-for-py
-00000c40: 6368 6172 6d2d 7573 6572 7329 0a20 202a  charm-users).  *
-00000c50: 205b 5365 7475 7020 6672 6f6d 2063 6f6d   [Setup from com
-00000c60: 6d61 6e64 206c 696e 655d 2823 7365 7475  mand line](#setu
-00000c70: 702d 6672 6f6d 2d63 6f6d 6d61 6e64 2d6c  p-from-command-l
-00000c80: 696e 6529 0a20 202a 205b 5072 6f6a 6563  ine).  * [Projec
-00000c90: 7420 4d61 6b65 6669 6c65 2063 6f6d 6d61  t Makefile comma
-00000ca0: 6e64 735d 2823 7072 6f6a 6563 742d 6d61  nds](#project-ma
-00000cb0: 6b65 6669 6c65 2d63 6f6d 6d61 6e64 7329  kefile-commands)
-00000cc0: 0a3c 212d 2d20 544f 4320 2d2d 3e0a 0a23  .<!-- TOC -->..#
-00000cd0: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
-00000ce0: 5573 6520 7069 7020 746f 2069 6e73 7461  Use pip to insta
-00000cf0: 6c6c 2074 6869 7320 7061 636b 6167 6520  ll this package 
-00000d00: 6672 6f6d 0a5b 7468 6520 5079 7468 6f6e  from.[the Python
-00000d10: 2050 6163 6b61 6765 2049 6e64 6578 5d28   Package Index](
-00000d20: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000d30: 2f70 726f 6a65 6374 2f65 7364 6263 6c69  /project/esdbcli
-00000d40: 656e 742f 292e 0a0a 2020 2020 2420 7069  ent/)...    $ pi
-00000d50: 7020 696e 7374 616c 6c20 6573 6462 636c  p install esdbcl
-00000d60: 6965 6e74 0a0a 4974 2069 7320 7265 636f  ient..It is reco
-00000d70: 6d6d 656e 6465 6420 746f 2069 6e73 7461  mmended to insta
-00000d80: 6c6c 2050 7974 686f 6e20 7061 636b 6167  ll Python packag
-00000d90: 6573 2069 6e74 6f20 6120 5079 7468 6f6e  es into a Python
-00000da0: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
-00000db0: 6d65 6e74 2e0a 0a0a 2323 2053 6572 7665  ment....## Serve
-00000dc0: 720a 0a23 2323 2053 7461 7274 2045 7665  r..### Start Eve
-00000dd0: 6e74 5374 6f72 6544 420a 0a55 7365 2044  ntStoreDB..Use D
-00000de0: 6f63 6b65 7220 746f 2072 756e 2045 7665  ocker to run Eve
-00000df0: 6e74 5374 6f72 6544 4220 7573 696e 6720  ntStoreDB using 
-00000e00: 7468 6520 6f66 6669 6369 616c 2044 6f63  the official Doc
-00000e10: 6b65 7220 636f 6e74 6169 6e65 7220 696d  ker container im
-00000e20: 6167 6520 6f6e 2044 6f63 6b65 7248 7562  age on DockerHub
-00000e30: 2e0a 0a46 6f72 2064 6576 656c 6f70 6d65  ...For developme
-00000e40: 6e74 2c20 796f 7520 6361 6e20 7374 6172  nt, you can star
-00000e50: 7420 6120 2273 6563 7572 6522 2073 6572  t a "secure" ser
-00000e60: 7665 7220 6c6f 6361 6c6c 7920 6f6e 2070  ver locally on p
-00000e70: 6f72 7420 3231 3133 2075 7369 6e67 2074  ort 2113 using t
-00000e80: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00000e90: 6d61 6e64 2e0a 0a20 2020 2024 2064 6f63  mand...    $ doc
-00000ea0: 6b65 7220 7275 6e20 2d64 202d 2d6e 616d  ker run -d --nam
-00000eb0: 6520 6d79 2d65 7665 6e74 7374 6f72 6564  e my-eventstored
-00000ec0: 6220 2d69 7420 2d70 2032 3131 333a 3231  b -it -p 2113:21
-00000ed0: 3133 202d 2d65 6e76 2022 484f 4d45 3d2f  13 --env "HOME=/
-00000ee0: 746d 7022 2065 7665 6e74 7374 6f72 652f  tmp" eventstore/
-00000ef0: 6576 656e 7473 746f 7265 3a32 322e 3130  eventstore:22.10
-00000f00: 2e30 2d62 7573 7465 722d 736c 696d 202d  .0-buster-slim -
-00000f10: 2d64 6576 0a0a 416c 7465 726e 6174 6976  -dev..Alternativ
-00000f20: 656c 792c 2079 6f75 2063 616e 2073 7461  ely, you can sta
-00000f30: 7274 2061 6e20 2269 6e73 6563 7572 6522  rt an "insecure"
-00000f40: 2073 6572 7665 7220 6c6f 6361 6c6c 7920   server locally 
-00000f50: 6f6e 2070 6f72 7420 3231 3133 2075 7369  on port 2113 usi
-00000f60: 6e67 2074 6865 2066 6f6c 6c6f 7769 6e67  ng the following
-00000f70: 2063 6f6d 6d61 6e64 2e0a 0a20 2020 2024   command...    $
-00000f80: 2064 6f63 6b65 7220 7275 6e20 2d64 202d   docker run -d -
-00000f90: 2d6e 616d 6520 6d79 2d65 7665 6e74 7374  -name my-eventst
-00000fa0: 6f72 6564 6220 2d69 7420 2d70 2032 3131  oredb -it -p 211
-00000fb0: 333a 3231 3133 2065 7665 6e74 7374 6f72  3:2113 eventstor
-00000fc0: 652f 6576 656e 7473 746f 7265 3a32 322e  e/eventstore:22.
-00000fd0: 3130 2e30 2d62 7573 7465 722d 736c 696d  10.0-buster-slim
-00000fe0: 202d 2d69 6e73 6563 7572 650a 0a54 6f20   --insecure..To 
-00000ff0: 636f 6e6e 6563 7420 746f 2074 6865 2022  connect to the "
-00001000: 696e 7365 6375 7265 2220 6c6f 6361 6c20  insecure" local 
-00001010: 7365 7276 6572 2075 7369 6e67 2074 6865  server using the
-00001020: 2063 6c69 656e 7420 696e 2074 6869 7320   client in this 
-00001030: 7061 636b 6167 652c 2079 6f75 206a 7573  package, you jus
-00001040: 7420 6e65 6564 0a74 6f20 6b6e 6f77 2074  t need.to know t
-00001050: 6865 206c 6f63 616c 2068 6f73 746e 616d  he local hostnam
-00001060: 6520 616e 6420 7468 6520 706f 7274 206e  e and the port n
-00001070: 756d 6265 722e 2054 6f20 636f 6e6e 6563  umber. To connec
-00001080: 7420 746f 2074 6865 2022 7365 6375 7265  t to the "secure
-00001090: 2220 6c6f 6361 6c0a 6465 7665 6c6f 706d  " local.developm
-000010a0: 656e 7420 7365 7276 6572 2c20 796f 7520  ent server, you 
-000010b0: 7769 6c6c 2061 6c73 6f20 6e65 6564 2074  will also need t
-000010c0: 6f20 6b6e 6f77 2074 6861 7420 7468 6520  o know that the 
-000010d0: 7573 6572 6e61 6d65 2069 7320 2261 646d  username is "adm
-000010e0: 696e 2220 616e 640a 7468 6520 7061 7373  in" and.the pass
-000010f0: 776f 7264 2069 7320 2263 6861 6e67 6569  word is "changei
-00001100: 7422 2e20 596f 7520 7769 6c6c 2061 6c73  t". You will als
-00001110: 6f20 6e65 6564 2074 6f20 6765 7420 7468  o need to get th
-00001120: 6520 5353 4c2f 544c 5320 6365 7274 6966  e SSL/TLS certif
-00001130: 6963 6174 6520 6672 6f6d 0a74 6865 2073  icate from.the s
-00001140: 6572 7665 722e 2059 6f75 2063 616e 2067  erver. You can g
-00001150: 6574 2074 6865 2073 6572 7665 7220 6365  et the server ce
-00001160: 7274 6966 6963 6174 6520 7769 7468 2074  rtificate with t
-00001170: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00001180: 6d61 6e64 2e0a 0a20 2020 2024 2070 7974  mand...    $ pyt
-00001190: 686f 6e20 2d63 2022 696d 706f 7274 2073  hon -c "import s
-000011a0: 736c 3b20 7072 696e 7428 6765 745f 7365  sl; print(get_se
-000011b0: 7276 6572 5f63 6572 7469 6669 6361 7465  rver_certificate
-000011c0: 2861 6464 723d 2827 6c6f 6361 6c68 6f73  (addr=('localhos
-000011d0: 7427 2c20 3231 3133 2929 2922 0a0a 0a23  t', 2113)))"...#
-000011e0: 2323 2053 746f 7020 4576 656e 7453 746f  ## Stop EventSto
-000011f0: 7265 4442 0a0a 546f 2073 746f 7020 616e  reDB..To stop an
-00001200: 6420 7265 6d6f 7665 2074 6865 2060 6d79  d remove the `my
-00001210: 2d65 7665 6e74 7374 6f72 6564 6260 2063  -eventstoredb` c
-00001220: 6f6e 7461 696e 6572 2063 7265 6174 6564  ontainer created
-00001230: 2061 626f 7665 2c20 7573 6520 7468 6520   above, use the 
-00001240: 666f 6c6c 6f77 696e 6720 446f 636b 6572  following Docker
-00001250: 2063 6f6d 6d61 6e64 732e 0a0a 2020 2020   commands...    
-00001260: 2420 646f 636b 6572 2073 746f 7020 6d79  $ docker stop my
-00001270: 2d65 7665 6e74 7374 6f72 6564 620a 0924  -eventstoredb..$
-00001280: 2064 6f63 6b65 7220 726d 206d 792d 6576   docker rm my-ev
-00001290: 656e 7473 746f 7265 6462 0a0a 0a23 2320  entstoredb...## 
-000012a0: 436c 6965 6e74 0a0a 5468 6520 6045 7364  Client..The `Esd
-000012b0: 6243 6c69 656e 7460 2063 6c61 7373 2063  bClient` class c
-000012c0: 616e 2062 6520 696d 706f 7274 6564 2066  an be imported f
-000012d0: 726f 6d20 7468 6520 6065 7364 6263 6c69  rom the `esdbcli
-000012e0: 656e 7460 2070 6163 6b61 6765 2e0a 0a60  ent` package...`
-000012f0: 6060 7079 7468 6f6e 0a66 726f 6d20 6573  ``python.from es
-00001300: 6462 636c 6965 6e74 2069 6d70 6f72 7420  dbclient import 
-00001310: 4573 6462 436c 6965 6e74 0a60 6060 0a0a  EsdbClient.```..
-00001320: 5468 6520 6045 7364 6243 6c69 656e 7460  The `EsdbClient`
-00001330: 2063 6c61 7373 2063 616e 2062 6520 636f   class can be co
-00001340: 6e73 7472 7563 7465 6420 7769 7468 2060  nstructed with `
-00001350: 686f 7374 6020 616e 6420 6070 6f72 7460  host` and `port`
-00001360: 2061 7267 756d 656e 7473 2e0a 5468 6520   arguments..The 
-00001370: 6068 6f73 7460 2061 6e64 2060 706f 7274  `host` and `port
-00001380: 6020 6172 6775 6d65 6e74 7320 696e 6469  ` arguments indi
-00001390: 6361 7465 2074 6865 2068 6f73 746e 616d  cate the hostnam
-000013a0: 6520 616e 6420 706f 7274 206e 756d 6265  e and port numbe
-000013b0: 7220 6f66 2074 6865 0a45 7665 6e74 5374  r of the.EventSt
-000013c0: 6f72 6544 4220 7365 7276 6572 2e0a 0a49  oreDB server...I
-000013d0: 6620 7468 6520 4576 656e 7453 746f 7265  f the EventStore
-000013e0: 4442 2073 6572 7665 7220 6973 2022 7365  DB server is "se
-000013f0: 6375 7265 222c 2074 6865 6e20 616c 736f  cure", then also
-00001400: 2075 7365 2074 6865 2060 7365 7276 6572   use the `server
-00001410: 5f63 6572 7460 2c0a 6075 7365 726e 616d  _cert`,.`usernam
-00001420: 6560 2061 6e64 2060 7061 7373 776f 7264  e` and `password
-00001430: 6020 6172 6775 6d65 6e74 732e 0a0a 5468  ` arguments...Th
-00001440: 6520 6068 6f73 7460 2061 7267 756d 656e  e `host` argumen
-00001450: 7420 6973 2065 7870 6563 7465 6420 746f  t is expected to
-00001460: 2062 6520 6120 5079 7468 6f6e 2060 7374   be a Python `st
-00001470: 7260 2e20 5468 6520 6070 6f72 7460 2061  r`. The `port` a
-00001480: 7267 756d 656e 7420 6973 2065 7870 6563  rgument is expec
-00001490: 7465 640a 746f 2062 6520 6120 5079 7468  ted.to be a Pyth
-000014a0: 6f6e 2060 696e 7460 2e20 5468 6520 6073  on `int`. The `s
-000014b0: 6572 7665 725f 6365 7274 6020 6973 2065  erver_cert` is e
-000014c0: 7870 6563 7465 6420 746f 2062 6520 6120  xpected to be a 
-000014d0: 5079 7468 6f6e 2060 7374 7260 2063 6f6e  Python `str` con
-000014e0: 7461 696e 696e 670a 7468 6520 5045 4d20  taining.the PEM 
-000014f0: 656e 636f 6465 6420 5353 4c2f 544c 5320  encoded SSL/TLS 
-00001500: 7365 7276 6572 2063 6572 7469 6669 6361  server certifica
-00001510: 7465 2e20 426f 7468 2060 7573 6572 6e61  te. Both `userna
-00001520: 6d65 6020 616e 6420 6070 6173 7377 6f72  me` and `passwor
-00001530: 6460 2061 7265 2065 7870 6563 7465 640a  d` are expected.
-00001540: 746f 2062 6520 6120 5079 7468 6f6e 2060  to be a Python `
-00001550: 7374 7260 2e0a 0a49 6e20 7468 6520 6578  str`...In the ex
-00001560: 616d 706c 6520 6265 6c6f 772c 2074 6865  ample below, the
-00001570: 2063 6f6e 7374 7275 6374 6f72 2061 7267   constructor arg
-00001580: 756d 656e 7420 7661 6c75 6573 2061 7265  ument values are
-00001590: 2074 616b 656e 2066 726f 6d20 7468 6520   taken from the 
-000015a0: 6f70 6572 6174 696e 670a 7379 7374 656d  operating.system
-000015b0: 2065 6e76 6972 6f6e 6d65 6e74 2c20 6265   environment, be
-000015c0: 6361 7573 6520 7468 6520 6578 616d 706c  cause the exampl
-000015d0: 6573 2069 6e20 7468 6973 2064 6f63 756d  es in this docum
-000015e0: 656e 7420 6172 6520 7465 7374 6564 2077  ent are tested w
-000015f0: 6974 6820 626f 7468 0a61 2022 7365 6375  ith both.a "secu
-00001600: 7265 2220 616e 6420 616e 2022 696e 7365  re" and an "inse
-00001610: 6375 7265 2220 7365 7276 6572 2e0a 0a60  cure" server...`
-00001620: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-00001630: 6f73 0a0a 636c 6965 6e74 203d 2045 7364  os..client = Esd
-00001640: 6243 6c69 656e 7428 0a20 2020 2068 6f73  bClient(.    hos
-00001650: 743d 6f73 2e67 6574 656e 7628 2245 5344  t=os.getenv("ESD
-00001660: 425f 484f 5354 2229 2c0a 2020 2020 706f  B_HOST"),.    po
-00001670: 7274 3d69 6e74 286f 732e 6765 7465 6e76  rt=int(os.getenv
-00001680: 2822 4553 4442 5f50 4f52 5422 2929 2c0a  ("ESDB_PORT")),.
-00001690: 2020 2020 7365 7276 6572 5f63 6572 743d      server_cert=
-000016a0: 6f73 2e67 6574 656e 7628 2245 5344 425f  os.getenv("ESDB_
-000016b0: 5345 5256 4552 5f43 4552 5422 292c 0a20  SERVER_CERT"),. 
-000016c0: 2020 2075 7365 726e 616d 653d 6f73 2e67     username=os.g
-000016d0: 6574 656e 7628 2245 5344 425f 5553 4552  etenv("ESDB_USER
-000016e0: 4e41 4d45 2229 2c0a 2020 2020 7061 7373  NAME"),.    pass
-000016f0: 776f 7264 3d6f 732e 6765 7465 6e76 2822  word=os.getenv("
-00001700: 4553 4442 5f50 4153 5357 4f52 4422 292c  ESDB_PASSWORD"),
-00001710: 0a29 0a60 6060 0a0a 2323 2053 7472 6561  .).```..## Strea
-00001720: 6d73 0a0a 496e 2045 7665 6e74 5374 6f72  ms..In EventStor
-00001730: 6544 422c 2061 2022 7374 7265 616d 2220  eDB, a "stream" 
-00001740: 6973 2061 2073 6571 7565 6e63 6520 6f66  is a sequence of
-00001750: 2072 6563 6f72 6465 6420 6576 656e 7473   recorded events
-00001760: 2074 6861 7420 616c 6c20 6861 7665 0a74   that all have.t
-00001770: 6865 2073 616d 6520 2273 7472 6561 6d20  he same "stream 
-00001780: 6e61 6d65 222e 2045 6163 6820 7265 636f  name". Each reco
-00001790: 7264 6564 2065 7665 6e74 2068 6173 2061  rded event has a
-000017a0: 2022 706f 7369 7469 6f6e 2220 696e 2069   "position" in i
-000017b0: 7473 2073 7472 6561 6d2e 0a54 6865 2070  ts stream..The p
-000017c0: 6f73 6974 696f 6e73 206f 6620 7468 6520  ositions of the 
-000017d0: 7265 636f 7264 6564 2065 7665 6e74 7320  recorded events 
-000017e0: 696e 2061 2073 7472 6561 6d20 6973 2061  in a stream is a
-000017f0: 2067 6170 6c65 7373 2073 6571 7565 6e63   gapless sequenc
-00001800: 6520 7374 6172 7469 6e67 0a66 726f 6d20  e starting.from 
-00001810: 7a65 726f 2e0a 0a23 2323 2041 7070 656e  zero...### Appen
-00001820: 6420 6576 656e 7473 0a0a 5468 6520 636c  d events..The cl
-00001830: 6965 6e74 2068 6173 2061 6e20 6061 7070  ient has an `app
-00001840: 656e 645f 6576 656e 7473 2829 6020 6d65  end_events()` me
-00001850: 7468 6f64 2c20 7768 6963 6820 6361 6e20  thod, which can 
-00001860: 6265 2075 7365 6420 746f 2061 7070 656e  be used to appen
-00001870: 640a 6e65 7720 6576 656e 7473 2074 6f20  d.new events to 
-00001880: 6120 2273 7472 6561 6d22 2e0a 0a54 6872  a "stream"...Thr
-00001890: 6565 2061 7267 756d 656e 7473 2061 7265  ee arguments are
-000018a0: 2072 6571 7569 7265 642c 2060 7374 7265   required, `stre
-000018b0: 616d 5f6e 616d 6560 2c20 6065 7870 6563  am_name`, `expec
-000018c0: 7465 645f 706f 7369 7469 6f6e 600a 616e  ted_position`.an
-000018d0: 6420 6065 7665 6e74 7360 2e0a 0a54 6865  d `events`...The
-000018e0: 2060 7374 7265 616d 5f6e 616d 6560 2061   `stream_name` a
-000018f0: 7267 756d 656e 7420 6973 2072 6571 7569  rgument is requi
-00001900: 7265 642c 2061 6e64 2069 7320 6578 7065  red, and is expe
-00001910: 6374 6564 2074 6f20 6265 2061 2050 7974  cted to be a Pyt
-00001920: 686f 6e0a 6073 7472 6020 6f62 6a65 6374  hon.`str` object
-00001930: 2074 6861 7420 756e 6971 7565 6c79 2069   that uniquely i
-00001940: 6465 6e74 6966 6965 7320 7468 6520 7374  dentifies the st
-00001950: 7265 616d 2069 6e20 7468 6520 6461 7461  ream in the data
-00001960: 6261 7365 2e0a 0a54 6865 2060 6578 7065  base...The `expe
-00001970: 6374 6564 5f70 6f73 6974 696f 6e60 2061  cted_position` a
-00001980: 7267 756d 656e 7420 6973 2072 6571 7569  rgument is requi
-00001990: 7265 642c 2069 7320 6578 7065 6374 6564  red, is expected
-000019a0: 2074 6f20 6265 3a20 6569 7468 6572 2060   to be: either `
-000019b0: 4e6f 6e65 600a 6966 206e 6577 2065 7665  None`.if new eve
-000019c0: 6e74 7320 6172 6520 6265 696e 6720 6170  nts are being ap
-000019d0: 7065 6e64 6564 2074 6f20 6120 6e65 7720  pended to a new 
-000019e0: 7374 7265 616d 2c20 6f72 2061 6e20 696e  stream, or an in
-000019f0: 7465 6765 7220 6571 7561 6c20 746f 2074  teger equal to t
-00001a00: 6865 0a70 6f73 6974 696f 6e20 7468 6520  he.position the 
-00001a10: 6c61 7374 2072 6563 6f72 6465 6420 6576  last recorded ev
-00001a20: 656e 7420 696e 2074 6865 2073 7472 6561  ent in the strea
-00001a30: 6d2e 0a0a 5468 6520 7374 7265 616d 2070  m...The stream p
-00001a40: 6f73 6974 696f 6e73 206f 6620 7265 636f  ositions of reco
-00001a50: 7264 6564 2065 7665 6e74 7320 7374 6172  rded events star
-00001a60: 7420 6672 6f6d 207a 6572 6f2e 2041 6e64  t from zero. And
-00001a70: 2073 6f2c 2077 6865 6e20 6170 7065 6e64   so, when append
-00001a80: 696e 670a 7468 6520 7365 636f 6e64 206e  ing.the second n
-00001a90: 6577 2065 7665 6e74 2074 6f20 6120 7374  ew event to a st
-00001aa0: 7265 616d 2074 6861 7420 6861 7320 6f6e  ream that has on
-00001ab0: 6520 7265 636f 7264 6564 2065 7665 6e74  e recorded event
-00001ac0: 2c20 7468 6520 636f 7272 6563 7420 7661  , the correct va
-00001ad0: 6c75 650a 6f66 2074 6865 2060 6578 7065  lue.of the `expe
-00001ae0: 6374 6564 5f70 6f73 6974 696f 6e60 2061  cted_position` a
-00001af0: 7267 756d 656e 7420 6973 2060 3060 2e20  rgument is `0`. 
-00001b00: 5369 6d69 6c61 726c 792c 2077 6865 6e20  Similarly, when 
-00001b10: 6170 7065 6e64 696e 6720 7468 6520 7468  appending the th
-00001b20: 6972 640a 6e65 7720 6576 656e 7420 746f  ird.new event to
-00001b30: 2061 2073 7472 6561 6d20 7468 6174 2068   a stream that h
-00001b40: 6173 2074 776f 2072 6563 6f72 6465 6420  as two recorded 
-00001b50: 6576 656e 7473 2c20 7468 6520 636f 7272  events, the corr
-00001b60: 6563 7420 7661 6c75 650a 6f66 2074 6865  ect value.of the
-00001b70: 2060 6578 7065 6374 6564 5f70 6f73 6974   `expected_posit
-00001b80: 696f 6e60 2061 7267 756d 656e 7420 6973  ion` argument is
-00001b90: 2060 3160 2e0a 0a53 7472 6561 6d73 2061   `1`...Streams a
-00001ba0: 7265 2063 7265 6174 6564 2062 7920 6170  re created by ap
-00001bb0: 7065 6e64 696e 6720 6576 656e 7473 2e20  pending events. 
-00001bc0: 5468 6520 636f 7272 6563 7420 7661 6c75  The correct valu
-00001bd0: 6520 6f66 2074 6865 2060 6578 7065 6374  e of the `expect
-00001be0: 6564 5f70 6f73 6974 696f 6e60 0a61 7267  ed_position`.arg
-00001bf0: 756d 656e 7420 7768 656e 2061 7070 656e  ument when appen
-00001c00: 6469 6e67 2074 6865 2066 6972 7374 2065  ding the first e
-00001c10: 7665 6e74 206f 6620 6120 6e65 7720 7374  vent of a new st
-00001c20: 7265 616d 2028 6120 7374 7265 616d 2077  ream (a stream w
-00001c30: 6974 6820 7a65 726f 2072 6563 6f72 6465  ith zero recorde
-00001c40: 640a 6576 656e 7473 2920 6973 2060 4e6f  d.events) is `No
-00001c50: 6e65 602e 2050 6c65 6173 6520 6e6f 7465  ne`. Please note
-00001c60: 2c20 6974 2069 7320 6e6f 7420 706f 7373  , it is not poss
-00001c70: 6962 6c65 2074 6f20 6372 6561 7465 2061  ible to create a
-00001c80: 6e20 2265 6d70 7479 2220 7374 7265 616d  n "empty" stream
-00001c90: 2069 6e0a 4576 656e 7453 746f 7265 4442   in.EventStoreDB
-00001ca0: 2e0a 0a49 6620 7468 6572 6520 6973 2061  ...If there is a
-00001cb0: 206d 6973 6d61 7463 6820 6265 7477 6565   mismatch betwee
-00001cc0: 6e20 7468 6520 6769 7665 6e20 7661 6c75  n the given valu
-00001cd0: 6520 6f66 2074 6865 2060 6578 7065 6374  e of the `expect
-00001ce0: 6564 5f70 6f73 6974 696f 6e60 2061 7267  ed_position` arg
-00001cf0: 756d 656e 740a 616e 6420 7468 6520 706f  ument.and the po
-00001d00: 7369 7469 6f6e 206f 6620 7468 6520 6c61  sition of the la
-00001d10: 7374 2072 6563 6f72 6465 6420 6576 656e  st recorded even
-00001d20: 7420 696e 2061 2073 7472 6561 6d2c 2074  t in a stream, t
-00001d30: 6865 6e20 616e 2060 4578 7065 6374 6564  hen an `Expected
-00001d40: 506f 7369 7469 6f6e 4572 726f 7260 0a65  PositionError`.e
-00001d50: 7863 6570 7469 6f6e 2077 696c 6c20 6265  xception will be
-00001d60: 2072 6169 7365 642e 2054 6869 7320 6566   raised. This ef
-00001d70: 6665 6374 6976 656c 7920 6163 636f 6d70  fectively accomp
-00001d80: 6c69 7368 6573 206f 7074 696d 6973 7469  lishes optimisti
-00001d90: 6320 636f 6e63 7572 7265 6e63 7920 636f  c concurrency co
-00001da0: 6e74 726f 6c2e 0a0a 4966 2079 6f75 2077  ntrol...If you w
-00001db0: 6973 6820 746f 2064 6973 6162 6c65 206f  ish to disable o
-00001dc0: 7074 696d 6973 7469 6320 636f 6e63 7572  ptimistic concur
-00001dd0: 7265 6e63 7920 636f 6e74 726f 6c20 7768  rency control wh
-00001de0: 656e 2061 7070 656e 6469 6e67 206e 6577  en appending new
-00001df0: 2065 7665 6e74 732c 2079 6f75 0a63 616e   events, you.can
-00001e00: 2073 6574 2074 6865 2060 6578 7065 6374   set the `expect
-00001e10: 6564 5f70 6f73 6974 696f 6e60 2074 6f20  ed_position` to 
-00001e20: 6120 6e65 6761 7469 7665 2069 6e74 6567  a negative integ
-00001e30: 6572 2e0a 0a49 6620 796f 7520 6e65 6564  er...If you need
-00001e40: 2074 6f20 6469 7363 6f76 6572 2074 6865   to discover the
-00001e50: 2063 7572 7265 6e74 2070 6f73 6974 696f   current positio
-00001e60: 6e20 6f66 2074 6865 206c 6173 7420 7265  n of the last re
-00001e70: 636f 7264 6564 2065 7665 6e74 2069 6e20  corded event in 
-00001e80: 6120 7374 7265 616d 2c0a 796f 7520 6361  a stream,.you ca
-00001e90: 6e20 7573 6520 7468 6520 6067 6574 5f73  n use the `get_s
-00001ea0: 7472 6561 6d5f 706f 7369 7469 6f6e 2829  tream_position()
-00001eb0: 6020 6d65 7468 6f64 2028 7365 6520 6265  ` method (see be
-00001ec0: 6c6f 7729 2e0a 0a54 6865 2060 6576 656e  low)...The `even
-00001ed0: 7473 6020 6172 6775 6d65 6e74 2069 7320  ts` argument is 
-00001ee0: 7265 7175 6972 6564 2c20 616e 6420 6973  required, and is
-00001ef0: 2065 7870 6563 7465 6420 746f 2062 6520   expected to be 
-00001f00: 6120 7365 7175 656e 6365 206f 6620 6e65  a sequence of ne
-00001f10: 770a 6576 656e 7420 6f62 6a65 6374 7320  w.event objects 
-00001f20: 746f 2062 6520 6170 7065 6e64 6564 2074  to be appended t
-00001f30: 6f20 7468 6520 6e61 6d65 6420 7374 7265  o the named stre
-00001f40: 616d 2e20 5468 6520 604e 6577 4576 656e  am. The `NewEven
-00001f50: 7460 2063 6c61 7373 2073 686f 756c 640a  t` class should.
-00001f60: 6265 2075 7365 6420 746f 2063 6f6e 7374  be used to const
-00001f70: 7275 6374 206e 6577 2065 7665 6e74 206f  ruct new event o
-00001f80: 626a 6563 7473 2028 7365 6520 6265 6c6f  bjects (see belo
-00001f90: 7729 2e0a 0a50 6c65 6173 6520 6e6f 7465  w)...Please note
-00001fa0: 2c20 7468 6520 6170 7065 6e64 2065 7665  , the append eve
-00001fb0: 6e74 7320 6f70 6572 6174 696f 6e20 6973  nts operation is
-00001fc0: 2061 746f 6d69 632c 2073 6f20 7468 6174   atomic, so that
-00001fd0: 2065 6974 6865 7220 616c 6c0a 6f72 206e   either all.or n
-00001fe0: 6f6e 6520 6f66 2074 6865 2067 6976 656e  one of the given
-00001ff0: 206e 6577 2065 7665 6e74 7320 7769 6c6c   new events will
-00002000: 2062 6520 7265 636f 7264 6564 2e20 4279   be recorded. By
-00002010: 2064 6573 6967 6e2c 2069 7420 6973 206f   design, it is o
-00002020: 6e6c 790a 706f 7373 6962 6c65 2077 6974  nly.possible wit
-00002030: 6820 4576 656e 7453 746f 7265 4442 2074  h EventStoreDB t
-00002040: 6f20 6174 6f6d 6963 616c 6c79 2072 6563  o atomically rec
-00002050: 6f72 6420 6e65 7720 6576 656e 7473 2069  ord new events i
-00002060: 6e20 6f6e 6520 7374 7265 616d 2e0a 0a49  n one stream...I
-00002070: 6e20 7468 6520 6578 616d 706c 6520 6265  n the example be
-00002080: 6c6f 772c 2061 206e 6577 2065 7665 6e74  low, a new event
-00002090: 2069 7320 6170 7065 6e64 6564 2074 6f20   is appended to 
-000020a0: 6120 6e65 7720 7374 7265 616d 2e0a 0a60  a new stream...`
-000020b0: 6060 7079 7468 6f6e 0a66 726f 6d20 7575  ``python.from uu
-000020c0: 6964 2069 6d70 6f72 7420 5555 4944 2c20  id import UUID, 
-000020d0: 7575 6964 340a 0a66 726f 6d20 6573 6462  uuid4..from esdb
-000020e0: 636c 6965 6e74 2069 6d70 6f72 7420 4e65  client import Ne
-000020f0: 7745 7665 6e74 0a0a 2320 436f 6e73 7472  wEvent..# Constr
-00002100: 7563 7420 6e65 7720 6576 656e 7420 6f62  uct new event ob
-00002110: 6a65 6374 2e0a 6576 656e 7431 203d 204e  ject..event1 = N
-00002120: 6577 4576 656e 7428 0a20 2020 2074 7970  ewEvent(.    typ
-00002130: 653d 274f 7264 6572 4372 6561 7465 6427  e='OrderCreated'
-00002140: 2c0a 2020 2020 6461 7461 3d62 2764 6174  ,.    data=b'dat
-00002150: 6131 272c 0a29 0a0a 2320 4465 6669 6e65  a1',.)..# Define
-00002160: 2073 7472 6561 6d20 6e61 6d65 2e0a 7374   stream name..st
-00002170: 7265 616d 5f6e 616d 6531 203d 2073 7472  ream_name1 = str
-00002180: 2875 7569 6434 2829 290a 0a23 2041 7070  (uuid4())..# App
-00002190: 656e 6420 6c69 7374 206f 6620 6576 656e  end list of even
-000021a0: 7473 2074 6f20 6e65 7720 7374 7265 616d  ts to new stream
-000021b0: 2e0a 636f 6d6d 6974 5f70 6f73 6974 696f  ..commit_positio
-000021c0: 6e31 203d 2063 6c69 656e 742e 6170 7065  n1 = client.appe
-000021d0: 6e64 5f65 7665 6e74 7328 0a20 2020 2073  nd_events(.    s
-000021e0: 7472 6561 6d5f 6e61 6d65 3d73 7472 6561  tream_name=strea
-000021f0: 6d5f 6e61 6d65 312c 0a20 2020 2065 7870  m_name1,.    exp
-00002200: 6563 7465 645f 706f 7369 7469 6f6e 3d4e  ected_position=N
-00002210: 6f6e 652c 0a20 2020 2065 7665 6e74 733d  one,.    events=
-00002220: 5b65 7665 6e74 315d 2c0a 290a 6060 600a  [event1],.).```.
-00002230: 0a49 6e20 7468 6520 6578 616d 706c 6520  .In the example 
-00002240: 6265 6c6f 772c 2074 776f 2073 7562 7365  below, two subse
-00002250: 7175 656e 7420 6576 656e 7473 2061 7265  quent events are
-00002260: 2061 7070 656e 6465 6420 746f 2061 6e20   appended to an 
-00002270: 6578 6973 7469 6e67 0a73 7472 6561 6d2e  existing.stream.
-00002280: 0a0a 6060 6070 7974 686f 6e0a 6576 656e  ..```python.even
-00002290: 7432 203d 204e 6577 4576 656e 7428 0a20  t2 = NewEvent(. 
-000022a0: 2020 2074 7970 653d 274f 7264 6572 5570     type='OrderUp
-000022b0: 6461 7465 6427 2c0a 2020 2020 6461 7461  dated',.    data
-000022c0: 3d62 2764 6174 6132 272c 0a29 0a65 7665  =b'data2',.).eve
-000022d0: 6e74 3320 3d20 4e65 7745 7665 6e74 280a  nt3 = NewEvent(.
-000022e0: 2020 2020 7479 7065 3d27 4f72 6465 7244      type='OrderD
-000022f0: 656c 6574 6564 272c 0a20 2020 2064 6174  eleted',.    dat
-00002300: 613d 6227 6461 7461 3327 2c0a 290a 0a63  a=b'data3',.)..c
-00002310: 6f6d 6d69 745f 706f 7369 7469 6f6e 3220  ommit_position2 
-00002320: 3d20 636c 6965 6e74 2e61 7070 656e 645f  = client.append_
-00002330: 6576 656e 7473 280a 2020 2020 7374 7265  events(.    stre
-00002340: 616d 5f6e 616d 653d 7374 7265 616d 5f6e  am_name=stream_n
-00002350: 616d 6531 2c0a 2020 2020 6578 7065 6374  ame1,.    expect
-00002360: 6564 5f70 6f73 6974 696f 6e3d 302c 0a20  ed_position=0,. 
-00002370: 2020 2065 7665 6e74 733d 5b65 7665 6e74     events=[event
-00002380: 322c 2065 7665 6e74 335d 2c0a 290a 6060  2, event3],.).``
-00002390: 600a 0a49 6620 7468 6520 6170 7065 6e64  `..If the append
-000023a0: 206f 7065 7261 7469 6f6e 2069 7320 7375   operation is su
-000023b0: 6363 6573 7366 756c 2c20 7468 6973 206d  ccessful, this m
-000023c0: 6574 686f 6420 7265 7475 726e 7320 616e  ethod returns an
-000023d0: 2069 6e74 6567 6572 0a72 6570 7265 7365   integer.represe
-000023e0: 6e74 696e 6720 7468 6520 6f76 6572 616c  nting the overal
-000023f0: 6c20 2263 6f6d 6d69 7420 706f 7369 7469  l "commit positi
-00002400: 6f6e 2220 6173 2069 7420 7761 7320 7768  on" as it was wh
-00002410: 656e 2074 6865 206f 7065 7261 7469 6f6e  en the operation
-00002420: 0a77 6173 2063 6f6d 706c 6574 6564 2e20  .was completed. 
-00002430: 4f74 6865 7277 6973 652c 2061 6e20 6578  Otherwise, an ex
-00002440: 6365 7074 696f 6e20 7769 6c6c 2062 6520  ception will be 
-00002450: 7261 6973 6564 2e0a 0a41 2022 636f 6d6d  raised...A "comm
-00002460: 6974 2070 6f73 6974 696f 6e22 2069 7320  it position" is 
-00002470: 6120 6d6f 6e6f 746f 6e69 6361 6c6c 7920  a monotonically 
-00002480: 696e 6372 6561 7369 6e67 2069 6e74 6567  increasing integ
-00002490: 6572 2072 6570 7265 7365 6e74 696e 670a  er representing.
-000024a0: 7468 6520 706f 7369 7469 6f6e 206f 6620  the position of 
-000024b0: 7468 6520 7265 636f 7264 6564 2065 7665  the recorded eve
-000024c0: 6e74 2069 6e20 6120 2274 6f74 616c 206f  nt in a "total o
-000024d0: 7264 6572 2220 6f66 2061 6c6c 2072 6563  rder" of all rec
-000024e0: 6f72 6465 640a 6576 656e 7473 2069 6e20  orded.events in 
-000024f0: 7468 6520 6461 7461 6261 7365 2061 6372  the database acr
-00002500: 6f73 7320 616c 6c20 7374 7265 616d 732e  oss all streams.
-00002510: 2049 7420 6973 2074 6865 2061 6374 7561   It is the actua
-00002520: 6c20 706f 7369 7469 6f6e 0a6f 6620 7468  l position.of th
-00002530: 6520 6576 656e 7420 7265 636f 7264 206f  e event record o
-00002540: 6e20 6469 736b 2c20 616e 6420 7468 6572  n disk, and ther
-00002550: 6520 6172 6520 7573 7561 6c6c 7920 6c61  e are usually la
-00002560: 7267 6520 6469 6666 6572 656e 6365 730a  rge differences.
-00002570: 6265 7477 6565 6e20 7375 6363 6573 7369  between successi
-00002580: 7665 2063 6f6d 6d69 7473 2e20 5468 6520  ve commits. The 
-00002590: 7365 7175 656e 6365 206f 6620 636f 6d6d  sequence of comm
-000025a0: 6974 2070 6f73 6974 696f 6e73 0a69 7320  it positions.is 
-000025b0: 4e4f 5420 6761 706c 6573 732e 0a0a 5468  NOT gapless...Th
-000025c0: 6520 2263 6f6d 6d69 7420 706f 7369 7469  e "commit positi
-000025d0: 6f6e 2220 7265 7475 726e 6564 2062 7920  on" returned by 
-000025e0: 6061 7070 656e 645f 6576 656e 7473 2829  `append_events()
-000025f0: 6020 6973 2074 6861 7420 6f66 2074 6865  ` is that of the
-00002600: 206c 6173 740a 7265 636f 7264 6564 2065   last.recorded e
-00002610: 7665 6e74 2069 6e20 7468 6520 6769 7665  vent in the give
-00002620: 6e20 7365 7175 656e 6365 206f 6620 6e65  n sequence of ne
-00002630: 7720 6576 656e 7473 2e0a 0a54 6865 2022  w events...The "
-00002640: 636f 6d6d 6974 2070 6f73 6974 696f 6e22  commit position"
-00002650: 2072 6574 7572 6e65 6420 696e 2074 6869   returned in thi
-00002660: 7320 7761 7920 6361 6e20 7468 6572 6566  s way can theref
-00002670: 6f72 6520 6265 2075 7365 6420 746f 2077  ore be used to w
-00002680: 6169 740a 666f 7220 6120 646f 776e 7374  ait.for a downst
-00002690: 7265 616d 2063 6f6d 706f 6e65 6e74 2074  ream component t
-000026a0: 6f20 6861 7665 2070 726f 6365 7373 6564  o have processed
-000026b0: 2061 6c6c 2074 6865 2065 7665 6e74 7320   all the events 
-000026c0: 7468 6174 2077 6572 6520 7265 636f 7264  that were record
-000026d0: 6564 2e0a 0a46 6f72 2065 7861 6d70 6c65  ed...For example
-000026e0: 2c20 636f 6e73 6964 6572 2061 2075 7365  , consider a use
-000026f0: 7220 696e 7465 7266 6163 6520 636f 6d6d  r interface comm
-00002700: 616e 6420 7468 6174 2072 6573 756c 7473  and that results
-00002710: 2069 6e20 7468 6520 7265 636f 7264 696e   in the recordin
-00002720: 670a 6f66 206e 6577 2065 7665 6e74 732c  g.of new events,
-00002730: 2061 6e64 2061 2071 7565 7279 2069 6e74   and a query int
-00002740: 6f20 616e 2065 7665 6e74 7561 6c6c 7920  o an eventually 
-00002750: 636f 6e73 6973 7465 6e74 206d 6174 6572  consistent mater
-00002760: 6961 6c69 7a65 640a 7669 6577 2069 6e20  ialized.view in 
-00002770: 6120 646f 776e 7374 7265 616d 2063 6f6d  a downstream com
-00002780: 706f 6e65 6e74 2074 6861 7420 6973 2075  ponent that is u
-00002790: 7064 6174 6564 2066 726f 6d20 7468 6573  pdated from thes
-000027a0: 6520 6576 656e 7473 2e20 4966 2074 6865  e events. If the
-000027b0: 206e 6577 0a65 7665 6e74 7320 6861 7665   new.events have
-000027c0: 206e 6f74 2079 6574 2062 6565 6e20 7072   not yet been pr
-000027d0: 6f63 6573 7365 642c 2074 6865 2076 6965  ocessed, the vie
-000027e0: 7720 776f 756c 6420 6265 2073 7461 6c65  w would be stale
-000027f0: 2e20 5468 6520 2263 6f6d 6d69 7420 706f  . The "commit po
-00002800: 7369 7469 6f6e 220a 6361 6e20 6265 2075  sition".can be u
-00002810: 7365 6420 6279 2074 6865 2075 7365 7220  sed by the user 
-00002820: 696e 7465 7266 6163 6520 746f 2070 6f6c  interface to pol
-00002830: 6c20 7468 6520 646f 776e 7374 7265 616d  l the downstream
-00002840: 2063 6f6d 706f 6e65 6e74 2075 6e74 696c   component until
-00002850: 2069 7420 6861 730a 7072 6f63 6573 7365   it has.processe
-00002860: 6420 7468 6520 6e65 7720 6576 656e 7473  d the new events
-00002870: 2c20 6166 7465 7220 7768 6963 6820 7469  , after which ti
-00002880: 6d65 2074 6865 2076 6965 7720 7769 6c6c  me the view will
-00002890: 206e 6f74 2062 6520 7374 616c 652e 0a0a   not be stale...
-000028a0: 2323 2320 4765 7420 6375 7272 656e 7420  ### Get current 
-000028b0: 7374 7265 616d 2070 6f73 6974 696f 6e0a  stream position.
-000028c0: 0a54 6865 2063 6c69 656e 7420 6861 7320  .The client has 
-000028d0: 6120 6067 6574 5f73 7472 6561 6d5f 706f  a `get_stream_po
-000028e0: 7369 7469 6f6e 2829 6020 6d65 7468 6f64  sition()` method
-000028f0: 2c20 7768 6963 6820 6361 6e20 6265 2075  , which can be u
-00002900: 7365 6420 746f 0a67 6574 2074 6865 2063  sed to.get the c
-00002910: 7572 7265 6e74 2022 7374 7265 616d 2070  urrent "stream p
-00002920: 6f73 6974 696f 6e22 206f 6620 6120 7374  osition" of a st
-00002930: 7265 616d 2028 7468 6520 706f 7369 7469  ream (the positi
-00002940: 6f6e 2069 6e20 7468 650a 7374 7265 616d  on in the.stream
-00002950: 206f 6620 7468 6520 6c61 7374 2072 6563   of the last rec
-00002960: 6f72 6465 6420 6576 656e 7420 696e 2074  orded event in t
-00002970: 6861 7420 7374 7265 616d 292e 0a0a 5468  hat stream)...Th
-00002980: 6973 206d 6574 686f 6420 6861 7320 6120  is method has a 
-00002990: 6073 7472 6561 6d5f 6e61 6d65 6020 6172  `stream_name` ar
-000029a0: 6775 6d65 6e74 2c20 7768 6963 6820 6973  gument, which is
-000029b0: 2072 6571 7569 7265 642e 0a0a 5468 6973   required...This
-000029c0: 206d 6574 686f 6420 616c 736f 2074 616b   method also tak
-000029d0: 6573 2061 6e20 6f70 7469 6f6e 616c 2060  es an optional `
-000029e0: 7469 6d65 6f75 7460 2061 7267 756d 656e  timeout` argumen
-000029f0: 742c 2074 6861 740a 6973 2065 7870 6563  t, that.is expec
-00002a00: 7465 6420 746f 2062 6520 6120 5079 7468  ted to be a Pyth
-00002a10: 6f6e 2060 666c 6f61 7460 2c20 7768 6963  on `float`, whic
-00002a20: 6820 7365 7473 2061 2064 6561 646c 696e  h sets a deadlin
-00002a30: 650a 666f 7220 7468 6520 636f 6d70 6c65  e.for the comple
-00002a40: 7469 6f6e 206f 6620 7468 6520 6752 5043  tion of the gRPC
-00002a50: 206f 7065 7261 7469 6f6e 2e0a 0a54 6865   operation...The
-00002a60: 2073 6571 7565 6e63 6520 6f66 2070 6f73   sequence of pos
-00002a70: 6974 696f 6e73 2069 6e20 6120 7374 7265  itions in a stre
-00002a80: 616d 2069 7320 6761 706c 6573 732e 2049  am is gapless. I
-00002a90: 7420 6973 207a 6572 6f2d 6261 7365 642c  t is zero-based,
-00002aa0: 0a73 6f20 7468 6174 2061 2073 7472 6561  .so that a strea
-00002ab0: 6d20 7769 7468 206f 6e65 2072 6563 6f72  m with one recor
-00002ac0: 6465 6420 6576 656e 7420 6861 7320 6120  ded event has a 
-00002ad0: 6375 7272 656e 7420 7374 7265 616d 0a70  current stream.p
-00002ae0: 6f73 6974 696f 6e20 6f66 2060 3060 2e20  osition of `0`. 
-00002af0: 5468 6520 6375 7272 656e 7420 7374 7265  The current stre
-00002b00: 616d 2070 6f73 6974 696f 6e20 6973 2060  am position is `
-00002b10: 3160 2077 6865 6e20 6120 7374 7265 616d  1` when a stream
-00002b20: 2068 6173 0a74 776f 2065 7665 6e74 732c   has.two events,
-00002b30: 2061 6e64 2069 7420 6973 2060 3260 2077   and it is `2` w
-00002b40: 6865 6e20 7468 6572 6520 6172 6520 6576  hen there are ev
-00002b50: 656e 7473 2c20 616e 6420 736f 206f 6e2e  ents, and so on.
-00002b60: 0a0a 496e 2074 6865 2065 7861 6d70 6c65  ..In the example
-00002b70: 2062 656c 6f77 2c20 7468 6520 6375 7272   below, the curr
-00002b80: 656e 7420 7374 7265 616d 2070 6f73 6974  ent stream posit
-00002b90: 696f 6e20 6973 206f 6274 6169 6e65 6420  ion is obtained 
-00002ba0: 6f66 2074 6865 0a73 7472 6561 6d20 746f  of the.stream to
-00002bb0: 2077 6869 6368 2065 7665 6e74 7320 7765   which events we
-00002bc0: 7265 2061 7070 656e 6465 6420 696e 2074  re appended in t
-00002bd0: 6865 2065 7861 6d70 6c65 7320 6162 6f76  he examples abov
-00002be0: 652e 0a42 6563 6175 7365 2074 6865 2073  e..Because the s
-00002bf0: 6571 7565 6e63 6520 6f66 2073 7472 6561  equence of strea
-00002c00: 6d20 706f 7369 7469 6f6e 7320 6973 207a  m positions is z
-00002c10: 6572 6f2d 6261 7365 642c 2061 6e64 2062  ero-based, and b
-00002c20: 6563 6175 7365 0a74 6872 6565 2065 7665  ecause.three eve
-00002c30: 6e74 7320 7765 7265 2061 7070 656e 6465  nts were appende
-00002c40: 642c 2073 6f20 7468 6520 6375 7272 656e  d, so the curren
-00002c50: 7420 7374 7265 616d 2070 6f73 6974 696f  t stream positio
-00002c60: 6e20 6973 2060 3260 2e0a 0a60 6060 7079  n is `2`...```py
-00002c70: 7468 6f6e 0a73 7472 6561 6d5f 706f 7369  thon.stream_posi
-00002c80: 7469 6f6e 203d 2063 6c69 656e 742e 6765  tion = client.ge
-00002c90: 745f 7374 7265 616d 5f70 6f73 6974 696f  t_stream_positio
-00002ca0: 6e28 0a20 2020 2073 7472 6561 6d5f 6e61  n(.    stream_na
-00002cb0: 6d65 3d73 7472 6561 6d5f 6e61 6d65 310a  me=stream_name1.
-00002cc0: 290a 0a61 7373 6572 7420 7374 7265 616d  )..assert stream
-00002cd0: 5f70 6f73 6974 696f 6e20 3d3d 2032 0a60  _position == 2.`
-00002ce0: 6060 0a0a 4966 2061 2073 7472 6561 6d20  ``..If a stream 
-00002cf0: 646f 6573 206e 6f74 2065 7869 7374 2c20  does not exist, 
-00002d00: 7468 6520 7265 7475 726e 6564 2073 7472  the returned str
-00002d10: 6561 6d20 706f 7369 7469 6f6e 2076 616c  eam position val
-00002d20: 7565 2069 7320 604e 6f6e 6560 2c0a 7768  ue is `None`,.wh
-00002d30: 6963 6820 6d61 7463 6865 7320 7468 6520  ich matches the 
-00002d40: 7265 7175 6972 6564 2065 7870 6563 7465  required expecte
-00002d50: 6420 706f 7369 7469 6f6e 2077 6865 6e20  d position when 
-00002d60: 6170 7065 6e64 696e 6720 7468 6520 6669  appending the fi
-00002d70: 7273 7420 6576 656e 740a 6f66 2061 206e  rst event.of a n
-00002d80: 6577 2073 7472 6561 6d20 2873 6565 2061  ew stream (see a
-00002d90: 626f 7665 292e 0a0a 6060 6070 7974 686f  bove)...```pytho
-00002da0: 6e0a 7374 7265 616d 5f70 6f73 6974 696f  n.stream_positio
-00002db0: 6e20 3d20 636c 6965 6e74 2e67 6574 5f73  n = client.get_s
-00002dc0: 7472 6561 6d5f 706f 7369 7469 6f6e 280a  tream_position(.
-00002dd0: 2020 2020 7374 7265 616d 5f6e 616d 653d      stream_name=
-00002de0: 7374 7228 7575 6964 3428 2929 0a29 0a0a  str(uuid4()).)..
-00002df0: 6173 7365 7274 2073 7472 6561 6d5f 706f  assert stream_po
-00002e00: 7369 7469 6f6e 203d 3d20 4e6f 6e65 0a60  sition == None.`
-00002e10: 6060 0a0a 5468 6973 206d 6574 686f 6420  ``..This method 
-00002e20: 7461 6b65 7320 616e 206f 7074 696f 6e61  takes an optiona
-00002e30: 6c20 6172 6775 6d65 6e74 2060 7469 6d65  l argument `time
-00002e40: 6f75 7460 2077 6869 6368 2069 7320 6120  out` which is a 
-00002e50: 666c 6f61 7420 7468 6174 2073 6574 730a  float that sets.
-00002e60: 6120 6465 6164 6c69 6e65 2066 6f72 2074  a deadline for t
-00002e70: 6865 2063 6f6d 706c 6574 696f 6e20 6f66  he completion of
-00002e80: 2074 6865 2067 5250 4320 6f70 6572 6174   the gRPC operat
-00002e90: 696f 6e2e 0a0a 0a23 2323 2052 6561 6420  ion....### Read 
-00002ea0: 7374 7265 616d 2065 7665 6e74 730a 0a54  stream events..T
-00002eb0: 6865 2063 6c69 656e 7420 6861 7320 6120  he client has a 
-00002ec0: 6072 6561 645f 7374 7265 616d 5f65 7665  `read_stream_eve
-00002ed0: 6e74 7328 2960 206d 6574 686f 642c 2077  nts()` method, w
-00002ee0: 6869 6368 2063 616e 2062 6520 7573 6564  hich can be used
-00002ef0: 2074 6f20 7265 6164 0a74 6865 2065 7665   to read.the eve
-00002f00: 6e74 7320 6f66 2061 2073 7472 6561 6d2e  nts of a stream.
-00002f10: 0a0a 5468 6973 206d 6574 686f 6420 7265  ..This method re
-00002f20: 7475 726e 7320 6e6e 2069 7465 7261 626c  turns nn iterabl
-00002f30: 6520 6f62 6a65 6374 2074 6861 7420 7969  e object that yi
-00002f40: 656c 6473 2072 6563 6f72 6465 6420 6576  elds recorded ev
-00002f50: 656e 7420 6f62 6a65 6374 732e 0a54 6865  ent objects..The
-00002f60: 7365 2072 6563 6f72 6465 6420 6576 656e  se recorded even
-00002f70: 7420 6f62 6a65 6374 7320 6172 6520 696e  t objects are in
-00002f80: 7374 616e 6365 7320 6f66 2074 6865 2060  stances of the `
-00002f90: 5265 636f 7264 6564 4576 656e 7460 2063  RecordedEvent` c
-00002fa0: 6c61 7373 2028 7365 6520 6265 6c6f 7729  lass (see below)
-00002fb0: 0a0a 5468 6973 206d 6574 686f 6420 6861  ..This method ha
-00002fc0: 7320 6f6e 6520 7265 7175 6972 6564 2061  s one required a
-00002fd0: 7267 756d 656e 742c 2060 7374 7265 616d  rgument, `stream
-00002fe0: 5f6e 616d 6560 2c20 7768 6963 6820 6973  _name`, which is
-00002ff0: 2074 6865 206e 616d 6520 6f66 0a74 6865   the name of.the
-00003000: 2073 7472 6561 6d20 746f 2062 6520 7265   stream to be re
-00003010: 6164 2e20 4279 2064 6566 6175 6c74 2c20  ad. By default, 
-00003020: 7468 6520 7265 636f 7264 6564 2065 7665  the recorded eve
-00003030: 6e74 7320 696e 2074 6865 2073 7472 6561  nts in the strea
-00003040: 6d0a 6172 6520 7265 7475 726e 6564 2069  m.are returned i
-00003050: 6e20 7468 6520 6f72 6465 7220 7468 6579  n the order they
-00003060: 2077 6572 6520 7265 636f 7264 6564 2e0a   were recorded..
-00003070: 0a54 6865 2065 7861 6d70 6c65 2062 656c  .The example bel
-00003080: 6f77 2073 686f 7773 2068 6f77 2074 6f20  ow shows how to 
-00003090: 7265 6164 2074 6865 2072 6563 6f72 6465  read the recorde
-000030a0: 6420 6576 656e 7473 206f 6620 6120 7374  d events of a st
-000030b0: 7265 616d 0a66 6f72 7761 7264 7320 6672  ream.forwards fr
-000030c0: 6f6d 2074 6865 2073 7461 7274 206f 6620  om the start of 
-000030d0: 7468 6520 7374 7265 616d 2074 6f20 7468  the stream to th
-000030e0: 6520 656e 6420 6f66 2074 6865 2073 7472  e end of the str
-000030f0: 6561 6d2e 2054 6865 0a6e 616d 6520 6f66  eam. The.name of
-00003100: 2061 2073 7472 6561 6d20 6973 2067 6976   a stream is giv
-00003110: 656e 2077 6865 6e20 6361 6c6c 696e 6720  en when calling 
-00003120: 7468 6520 6d65 7468 6f64 2e20 496e 2074  the method. In t
-00003130: 6869 7320 6578 616d 706c 652c 0a74 6865  his example,.the
-00003140: 2069 7465 7261 626c 6520 7265 7370 6f6e   iterable respon
-00003150: 7365 206f 626a 6563 7420 6973 2063 6f6e  se object is con
-00003160: 7665 7274 6564 2069 6e74 6f20 6120 5079  verted into a Py
-00003170: 7468 6f6e 2060 6c69 7374 602c 2077 6869  thon `list`, whi
-00003180: 6368 0a63 6f6e 7461 696e 7320 616c 6c20  ch.contains all 
-00003190: 7468 6520 7265 636f 7264 6564 2065 7665  the recorded eve
-000031a0: 6e74 206f 626a 6563 7473 2074 6861 7420  nt objects that 
-000031b0: 7765 7265 2072 6561 6420 6672 6f6d 2074  were read from t
-000031c0: 6865 2073 7472 6561 6d2e 0a0a 6060 6070  he stream...```p
-000031d0: 7974 686f 6e0a 7265 7370 6f6e 7365 203d  ython.response =
-000031e0: 2063 6c69 656e 742e 7265 6164 5f73 7472   client.read_str
-000031f0: 6561 6d5f 6576 656e 7473 280a 2020 2020  eam_events(.    
-00003200: 7374 7265 616d 5f6e 616d 653d 7374 7265  stream_name=stre
-00003210: 616d 5f6e 616d 6531 0a29 0a0a 6576 656e  am_name1.)..even
-00003220: 7473 203d 206c 6973 7428 7265 7370 6f6e  ts = list(respon
-00003230: 7365 290a 6060 600a 0a4e 6f77 2074 6861  se).```..Now tha
-00003240: 7420 7765 2068 6176 6520 6120 6c69 7374  t we have a list
-00003250: 206f 6620 6576 656e 7420 6f62 6a65 6374   of event object
-00003260: 732c 2077 6520 6361 6e20 6368 6563 6b20  s, we can check 
-00003270: 7765 2067 6f74 2074 6865 0a74 6872 6565  we got the.three
-00003280: 2065 7665 6e74 7320 7468 6174 2077 6572   events that wer
-00003290: 6520 6170 7065 6e64 6564 2074 6f20 7468  e appended to th
-000032a0: 6520 7374 7265 616d 2c20 616e 6420 7468  e stream, and th
-000032b0: 6174 2074 6865 7920 6172 650a 6f72 6465  at they are.orde
-000032c0: 7265 6420 6578 6163 746c 7920 6173 2074  red exactly as t
-000032d0: 6865 7920 7765 7265 2061 7070 656e 6465  hey were appende
-000032e0: 642e 0a0a 6060 6070 7974 686f 6e0a 6173  d...```python.as
-000032f0: 7365 7274 206c 656e 2865 7665 6e74 7329  sert len(events)
-00003300: 203d 3d20 330a 0a61 7373 6572 7420 6576   == 3..assert ev
-00003310: 656e 7473 5b30 5d2e 7374 7265 616d 5f6e  ents[0].stream_n
-00003320: 616d 6520 3d3d 2073 7472 6561 6d5f 6e61  ame == stream_na
-00003330: 6d65 310a 6173 7365 7274 2065 7665 6e74  me1.assert event
-00003340: 735b 305d 2e73 7472 6561 6d5f 706f 7369  s[0].stream_posi
-00003350: 7469 6f6e 203d 3d20 300a 6173 7365 7274  tion == 0.assert
-00003360: 2065 7665 6e74 735b 305d 2e74 7970 6520   events[0].type 
-00003370: 3d3d 2065 7665 6e74 312e 7479 7065 0a61  == event1.type.a
-00003380: 7373 6572 7420 6576 656e 7473 5b30 5d2e  ssert events[0].
-00003390: 6461 7461 203d 3d20 6576 656e 7431 2e64  data == event1.d
-000033a0: 6174 610a 0a61 7373 6572 7420 6576 656e  ata..assert even
-000033b0: 7473 5b31 5d2e 7374 7265 616d 5f6e 616d  ts[1].stream_nam
-000033c0: 6520 3d3d 2073 7472 6561 6d5f 6e61 6d65  e == stream_name
-000033d0: 310a 6173 7365 7274 2065 7665 6e74 735b  1.assert events[
-000033e0: 315d 2e73 7472 6561 6d5f 706f 7369 7469  1].stream_positi
-000033f0: 6f6e 203d 3d20 310a 6173 7365 7274 2065  on == 1.assert e
-00003400: 7665 6e74 735b 315d 2e74 7970 6520 3d3d  vents[1].type ==
-00003410: 2065 7665 6e74 322e 7479 7065 0a61 7373   event2.type.ass
-00003420: 6572 7420 6576 656e 7473 5b31 5d2e 6461  ert events[1].da
-00003430: 7461 203d 3d20 6576 656e 7432 2e64 6174  ta == event2.dat
-00003440: 610a 0a61 7373 6572 7420 6576 656e 7473  a..assert events
-00003450: 5b32 5d2e 7374 7265 616d 5f6e 616d 6520  [2].stream_name 
-00003460: 3d3d 2073 7472 6561 6d5f 6e61 6d65 310a  == stream_name1.
-00003470: 6173 7365 7274 2065 7665 6e74 735b 325d  assert events[2]
-00003480: 2e73 7472 6561 6d5f 706f 7369 7469 6f6e  .stream_position
-00003490: 203d 3d20 320a 6173 7365 7274 2065 7665   == 2.assert eve
-000034a0: 6e74 735b 325d 2e74 7970 6520 3d3d 2065  nts[2].type == e
-000034b0: 7665 6e74 332e 7479 7065 0a61 7373 6572  vent3.type.asser
-000034c0: 7420 6576 656e 7473 5b32 5d2e 6461 7461  t events[2].data
-000034d0: 203d 3d20 6576 656e 7433 2e64 6174 610a   == event3.data.
-000034e0: 6060 600a 0a54 6865 206d 6574 686f 6420  ```..The method 
-000034f0: 6072 6561 645f 7374 7265 616d 5f65 7665  `read_stream_eve
-00003500: 6e74 7328 2960 2061 6c73 6f20 7375 7070  nts()` also supp
-00003510: 6f72 7473 2066 6f75 7220 6f70 7469 6f6e  orts four option
-00003520: 616c 2061 7267 756d 656e 7473 2c0a 6070  al arguments,.`p
-00003530: 6f73 6974 696f 6e60 2c20 6062 6163 6b77  osition`, `backw
-00003540: 6172 6473 602c 2060 6c69 6d69 7460 2c20  ards`, `limit`, 
-00003550: 616e 6420 6074 696d 656f 7574 602e 0a0a  and `timeout`...
-00003560: 5468 6520 6f70 7469 6f6e 616c 2060 706f  The optional `po
-00003570: 7369 7469 6f6e 6020 6172 6775 6d65 6e74  sition` argument
-00003580: 2069 7320 616e 206f 7074 696f 6e61 6c20   is an optional 
-00003590: 696e 7465 6765 7220 7468 6174 2063 616e  integer that can
-000035a0: 2062 6520 7573 6564 2074 6f20 696e 6469   be used to indi
-000035b0: 6361 7465 0a74 6865 2070 6f73 6974 696f  cate.the positio
-000035c0: 6e20 696e 2074 6865 2073 7472 6561 6d20  n in the stream 
-000035d0: 6672 6f6d 2077 6869 6368 2074 6f20 7374  from which to st
-000035e0: 6172 7420 7265 6164 696e 672e 2054 6869  art reading. Thi
-000035f0: 7320 6172 6775 6d65 6e74 2069 7320 604e  s argument is `N
-00003600: 6f6e 6560 0a62 7920 6465 6661 756c 742c  one`.by default,
-00003610: 2077 6869 6368 206d 6561 6e73 2074 6865   which means the
-00003620: 2073 7472 6561 6d20 7769 6c6c 2062 6520   stream will be 
-00003630: 7265 6164 2065 6974 6865 7220 6672 6f6d  read either from
-00003640: 2074 6865 2073 7461 7274 206f 6620 7468   the start of th
-00003650: 650a 7374 7265 616d 2028 7468 6520 6465  e.stream (the de
-00003660: 6661 756c 7420 6265 6861 7669 6f75 7229  fault behaviour)
-00003670: 2c20 6f72 2066 726f 6d20 7468 6520 656e  , or from the en
-00003680: 6420 6f66 2074 6865 2073 7472 6561 6d20  d of the stream 
-00003690: 6966 2060 6261 636b 7761 7264 7360 2069  if `backwards` i
-000036a0: 730a 6054 7275 6560 2028 7365 6520 6265  s.`True` (see be
-000036b0: 6c6f 7729 2e20 5768 656e 2072 6561 6469  low). When readi
-000036c0: 6e67 2061 2073 7472 6561 6d20 6672 6f6d  ng a stream from
-000036d0: 2061 2073 7065 6369 6669 6320 706f 7369   a specific posi
-000036e0: 7469 6f6e 2069 6e20 7468 6520 7374 7265  tion in the stre
-000036f0: 616d 2c20 7468 650a 7265 636f 7264 6564  am, the.recorded
-00003700: 2065 7665 6e74 2061 7420 7468 6174 2070   event at that p
-00003710: 6f73 6974 696f 6e20 5749 4c4c 2062 6520  osition WILL be 
-00003720: 696e 636c 7564 6564 2c20 626f 7468 2077  included, both w
-00003730: 6865 6e20 7265 6164 696e 6720 666f 7277  hen reading forw
-00003740: 6172 6473 0a66 726f 6d20 7468 6174 2070  ards.from that p
-00003750: 6f73 6974 696f 6e2c 2061 6e64 2077 6865  osition, and whe
-00003760: 6e20 7265 6164 696e 6720 6261 636b 7761  n reading backwa
-00003770: 7264 7320 6672 6f6d 2074 6861 7420 706f  rds from that po
-00003780: 7369 7469 6f6e 2e0a 0a54 6865 206f 7074  sition...The opt
-00003790: 696f 6e61 6c20 6172 6775 6d65 6e74 2060  ional argument `
-000037a0: 6261 636b 7761 7264 7360 2069 7320 6120  backwards` is a 
-000037b0: 626f 6f6c 6561 6e2c 2062 7920 6465 6661  boolean, by defa
-000037c0: 756c 7420 6046 616c 7365 602c 2077 6869  ult `False`, whi
-000037d0: 6368 206d 6561 6e73 2074 6865 0a73 7472  ch means the.str
-000037e0: 6561 6d20 7769 6c6c 2062 6520 7265 6164  eam will be read
-000037f0: 2066 6f72 7761 7264 7320 6279 2064 6566   forwards by def
-00003800: 6175 6c74 2c20 736f 2074 6861 7420 6576  ault, so that ev
-00003810: 656e 7473 2061 7265 2072 6574 7572 6e65  ents are returne
-00003820: 6420 696e 2074 6865 0a6f 7264 6572 2074  d in the.order t
-00003830: 6865 7920 7765 7265 2061 7070 656e 6465  hey were appende
-00003840: 642c 2049 6620 6062 6163 6b77 6172 6473  d, If `backwards
-00003850: 6020 6973 2060 5472 7565 602c 2074 6865  ` is `True`, the
-00003860: 2073 7472 6561 6d20 7769 6c6c 2062 6520   stream will be 
-00003870: 7265 6164 0a62 6163 6b77 6172 6473 2c20  read.backwards, 
-00003880: 736f 2074 6861 7420 6576 656e 7473 2061  so that events a
-00003890: 7265 2072 6574 7572 6e65 6420 696e 2072  re returned in r
-000038a0: 6576 6572 7365 206f 7264 6572 2e0a 0a54  everse order...T
-000038b0: 6865 206f 7074 696f 6e61 6c20 6172 6775  he optional argu
-000038c0: 6d65 6e74 2060 6c69 6d69 7460 2069 7320  ment `limit` is 
-000038d0: 616e 2069 6e74 6567 6572 2077 6869 6368  an integer which
-000038e0: 206c 696d 6974 7320 7468 6520 6e75 6d62   limits the numb
-000038f0: 6572 206f 6620 6576 656e 7473 2074 6861  er of events tha
-00003900: 7420 7769 6c6c 0a62 6520 7265 7475 726e  t will.be return
-00003910: 6564 2e20 5468 6520 6465 6661 756c 7420  ed. The default 
-00003920: 7661 6c75 6520 6973 2060 7379 732e 6d61  value is `sys.ma
-00003930: 7869 6e74 602e 0a0a 5468 6520 6f70 7469  xint`...The opti
-00003940: 6f6e 616c 2061 7267 756d 656e 7420 6074  onal argument `t
-00003950: 696d 656f 7574 6020 6973 2061 2066 6c6f  imeout` is a flo
-00003960: 6174 2077 6869 6368 2073 6574 7320 6120  at which sets a 
-00003970: 6465 6164 6c69 6e65 2066 6f72 2074 6865  deadline for the
-00003980: 2063 6f6d 706c 6574 696f 6e20 6f66 0a74   completion of.t
-00003990: 6865 2067 5250 4320 6f70 6572 6174 696f  he gRPC operatio
-000039a0: 6e2e 0a0a 5468 6520 6578 616d 706c 6520  n...The example 
-000039b0: 6265 6c6f 7720 7368 6f77 7320 686f 7720  below shows how 
-000039c0: 746f 2072 6561 6420 7265 636f 7264 6564  to read recorded
-000039d0: 2065 7665 6e74 7320 696e 2061 2073 7472   events in a str
-000039e0: 6561 6d20 666f 7277 6172 6473 2066 726f  eam forwards fro
-000039f0: 6d0a 6120 7370 6563 6966 6963 2073 7472  m.a specific str
-00003a00: 6561 6d20 706f 7369 7469 6f6e 2074 6f20  eam position to 
-00003a10: 7468 6520 656e 6420 6f66 2074 6865 2073  the end of the s
-00003a20: 7472 6561 6d2e 0a0a 6060 6070 7974 686f  tream...```pytho
-00003a30: 6e0a 6576 656e 7473 203d 206c 6973 7428  n.events = list(
-00003a40: 0a20 2020 2063 6c69 656e 742e 7265 6164  .    client.read
-00003a50: 5f73 7472 6561 6d5f 6576 656e 7473 280a  _stream_events(.
-00003a60: 2020 2020 2020 2020 7374 7265 616d 5f6e          stream_n
-00003a70: 616d 653d 7374 7265 616d 5f6e 616d 6531  ame=stream_name1
-00003a80: 2c0a 2020 2020 2020 2020 706f 7369 7469  ,.        positi
-00003a90: 6f6e 3d31 2c0a 2020 2020 290a 290a 0a61  on=1,.    ).)..a
-00003aa0: 7373 6572 7420 6c65 6e28 6576 656e 7473  ssert len(events
-00003ab0: 2920 3d3d 2032 0a0a 6173 7365 7274 2065  ) == 2..assert e
-00003ac0: 7665 6e74 735b 305d 2e73 7472 6561 6d5f  vents[0].stream_
-00003ad0: 6e61 6d65 203d 3d20 7374 7265 616d 5f6e  name == stream_n
-00003ae0: 616d 6531 0a61 7373 6572 7420 6576 656e  ame1.assert even
-00003af0: 7473 5b30 5d2e 7374 7265 616d 5f70 6f73  ts[0].stream_pos
-00003b00: 6974 696f 6e20 3d3d 2031 0a61 7373 6572  ition == 1.asser
-00003b10: 7420 6576 656e 7473 5b30 5d2e 7479 7065  t events[0].type
-00003b20: 203d 3d20 6576 656e 7432 2e74 7970 650a   == event2.type.
-00003b30: 6173 7365 7274 2065 7665 6e74 735b 305d  assert events[0]
-00003b40: 2e64 6174 6120 3d3d 2065 7665 6e74 322e  .data == event2.
-00003b50: 6461 7461 0a0a 6173 7365 7274 2065 7665  data..assert eve
-00003b60: 6e74 735b 315d 2e73 7472 6561 6d5f 6e61  nts[1].stream_na
-00003b70: 6d65 203d 3d20 7374 7265 616d 5f6e 616d  me == stream_nam
-00003b80: 6531 0a61 7373 6572 7420 6576 656e 7473  e1.assert events
-00003b90: 5b31 5d2e 7374 7265 616d 5f70 6f73 6974  [1].stream_posit
-00003ba0: 696f 6e20 3d3d 2032 0a61 7373 6572 7420  ion == 2.assert 
-00003bb0: 6576 656e 7473 5b31 5d2e 7479 7065 203d  events[1].type =
-00003bc0: 3d20 6576 656e 7433 2e74 7970 650a 6173  = event3.type.as
-00003bd0: 7365 7274 2065 7665 6e74 735b 315d 2e64  sert events[1].d
-00003be0: 6174 6120 3d3d 2065 7665 6e74 332e 6461  ata == event3.da
-00003bf0: 7461 0a60 6060 0a0a 5468 6520 6578 616d  ta.```..The exam
-00003c00: 706c 6520 6265 6c6f 7720 7368 6f77 7320  ple below shows 
-00003c10: 686f 7720 746f 2072 6561 6420 7468 6520  how to read the 
-00003c20: 7265 636f 7264 6564 2065 7665 6e74 7320  recorded events 
-00003c30: 696e 2061 2073 7472 6561 6d20 6261 636b  in a stream back
-00003c40: 7761 7264 7320 6672 6f6d 0a74 6865 2065  wards from.the e
-00003c50: 6e64 206f 6620 7468 6520 7374 7265 616d  nd of the stream
-00003c60: 2074 6f20 7468 6520 7374 6172 7420 6f66   to the start of
-00003c70: 2074 6865 2073 7472 6561 6d2e 0a0a 6060   the stream...``
-00003c80: 6070 7974 686f 6e0a 6576 656e 7473 203d  `python.events =
-00003c90: 206c 6973 7428 0a20 2020 2063 6c69 656e   list(.    clien
-00003ca0: 742e 7265 6164 5f73 7472 6561 6d5f 6576  t.read_stream_ev
-00003cb0: 656e 7473 280a 2020 2020 2020 2020 7374  ents(.        st
-00003cc0: 7265 616d 5f6e 616d 653d 7374 7265 616d  ream_name=stream
-00003cd0: 5f6e 616d 6531 2c0a 2020 2020 2020 2020  _name1,.        
-00003ce0: 6261 636b 7761 7264 733d 5472 7565 2c0a  backwards=True,.
-00003cf0: 2020 2020 290a 290a 0a61 7373 6572 7420      ).)..assert 
-00003d00: 6c65 6e28 6576 656e 7473 2920 3d3d 2033  len(events) == 3
-00003d10: 0a0a 6173 7365 7274 2065 7665 6e74 735b  ..assert events[
-00003d20: 305d 2e73 7472 6561 6d5f 6e61 6d65 203d  0].stream_name =
-00003d30: 3d20 7374 7265 616d 5f6e 616d 6531 0a61  = stream_name1.a
-00003d40: 7373 6572 7420 6576 656e 7473 5b30 5d2e  ssert events[0].
-00003d50: 7374 7265 616d 5f70 6f73 6974 696f 6e20  stream_position 
-00003d60: 3d3d 2032 0a61 7373 6572 7420 6576 656e  == 2.assert even
-00003d70: 7473 5b30 5d2e 7479 7065 203d 3d20 6576  ts[0].type == ev
-00003d80: 656e 7433 2e74 7970 650a 6173 7365 7274  ent3.type.assert
-00003d90: 2065 7665 6e74 735b 305d 2e64 6174 6120   events[0].data 
-00003da0: 3d3d 2065 7665 6e74 332e 6461 7461 0a0a  == event3.data..
-00003db0: 6173 7365 7274 2065 7665 6e74 735b 315d  assert events[1]
-00003dc0: 2e73 7472 6561 6d5f 6e61 6d65 203d 3d20  .stream_name == 
-00003dd0: 7374 7265 616d 5f6e 616d 6531 0a61 7373  stream_name1.ass
-00003de0: 6572 7420 6576 656e 7473 5b31 5d2e 7374  ert events[1].st
-00003df0: 7265 616d 5f70 6f73 6974 696f 6e20 3d3d  ream_position ==
-00003e00: 2031 0a61 7373 6572 7420 6576 656e 7473   1.assert events
-00003e10: 5b31 5d2e 7479 7065 203d 3d20 6576 656e  [1].type == even
-00003e20: 7432 2e74 7970 650a 6173 7365 7274 2065  t2.type.assert e
-00003e30: 7665 6e74 735b 315d 2e64 6174 6120 3d3d  vents[1].data ==
-00003e40: 2065 7665 6e74 322e 6461 7461 0a60 6060   event2.data.```
-00003e50: 0a0a 5468 6520 6578 616d 706c 6520 6265  ..The example be
-00003e60: 6c6f 7720 7368 6f77 7320 686f 7720 746f  low shows how to
-00003e70: 2072 6561 6420 6120 6c69 6d69 7465 6420   read a limited 
-00003e80: 6e75 6d62 6572 2028 7477 6f29 206f 6620  number (two) of 
-00003e90: 7468 6520 7265 636f 7264 6564 2065 7665  the recorded eve
-00003ea0: 6e74 730a 696e 2061 2073 7472 6561 6d20  nts.in a stream 
-00003eb0: 666f 7277 6172 6473 2066 726f 6d20 7468  forwards from th
-00003ec0: 6520 7374 6172 7420 6f66 2074 6865 2073  e start of the s
-00003ed0: 7472 6561 6d2e 0a0a 6060 6070 7974 686f  tream...```pytho
-00003ee0: 6e0a 6576 656e 7473 203d 206c 6973 7428  n.events = list(
-00003ef0: 0a20 2020 2063 6c69 656e 742e 7265 6164  .    client.read
-00003f00: 5f73 7472 6561 6d5f 6576 656e 7473 280a  _stream_events(.
-00003f10: 2020 2020 2020 2020 7374 7265 616d 5f6e          stream_n
-00003f20: 616d 653d 7374 7265 616d 5f6e 616d 6531  ame=stream_name1
-00003f30: 2c0a 2020 2020 2020 2020 6c69 6d69 743d  ,.        limit=
-00003f40: 322c 0a20 2020 2029 0a29 0a0a 6173 7365  2,.    ).)..asse
-00003f50: 7274 206c 656e 2865 7665 6e74 7329 203d  rt len(events) =
-00003f60: 3d20 320a 0a61 7373 6572 7420 6576 656e  = 2..assert even
-00003f70: 7473 5b30 5d2e 7374 7265 616d 5f6e 616d  ts[0].stream_nam
-00003f80: 6520 3d3d 2073 7472 6561 6d5f 6e61 6d65  e == stream_name
-00003f90: 310a 6173 7365 7274 2065 7665 6e74 735b  1.assert events[
-00003fa0: 305d 2e73 7472 6561 6d5f 706f 7369 7469  0].stream_positi
-00003fb0: 6f6e 203d 3d20 300a 6173 7365 7274 2065  on == 0.assert e
-00003fc0: 7665 6e74 735b 305d 2e74 7970 6520 3d3d  vents[0].type ==
-00003fd0: 2065 7665 6e74 312e 7479 7065 0a61 7373   event1.type.ass
-00003fe0: 6572 7420 6576 656e 7473 5b30 5d2e 6461  ert events[0].da
-00003ff0: 7461 203d 3d20 6576 656e 7431 2e64 6174  ta == event1.dat
-00004000: 610a 0a61 7373 6572 7420 6576 656e 7473  a..assert events
-00004010: 5b31 5d2e 7374 7265 616d 5f6e 616d 6520  [1].stream_name 
-00004020: 3d3d 2073 7472 6561 6d5f 6e61 6d65 310a  == stream_name1.
-00004030: 6173 7365 7274 2065 7665 6e74 735b 315d  assert events[1]
-00004040: 2e73 7472 6561 6d5f 706f 7369 7469 6f6e  .stream_position
-00004050: 203d 3d20 310a 6173 7365 7274 2065 7665   == 1.assert eve
-00004060: 6e74 735b 315d 2e74 7970 6520 3d3d 2065  nts[1].type == e
-00004070: 7665 6e74 322e 7479 7065 0a61 7373 6572  vent2.type.asser
-00004080: 7420 6576 656e 7473 5b31 5d2e 6461 7461  t events[1].data
-00004090: 203d 3d20 6576 656e 7432 2e64 6174 610a   == event2.data.
-000040a0: 6060 600a 0a54 6865 2065 7861 6d70 6c65  ```..The example
-000040b0: 2062 656c 6f77 2073 686f 7773 2068 6f77   below shows how
-000040c0: 2074 6f20 7265 6164 2061 206c 696d 6974   to read a limit
-000040d0: 6564 206e 756d 6265 7220 286f 6e65 2920  ed number (one) 
-000040e0: 6f66 2074 6865 2072 6563 6f72 6465 640a  of the recorded.
-000040f0: 6576 656e 7473 2069 6e20 6120 7374 7265  events in a stre
-00004100: 616d 2062 6163 6b77 6172 6473 2066 726f  am backwards fro
-00004110: 6d20 6120 6769 7665 6e20 7374 7265 616d  m a given stream
-00004120: 2070 6f73 6974 696f 6e2e 0a0a 6060 6070   position...```p
-00004130: 7974 686f 6e0a 6576 656e 7473 203d 206c  ython.events = l
-00004140: 6973 7428 0a20 2020 2063 6c69 656e 742e  ist(.    client.
-00004150: 7265 6164 5f73 7472 6561 6d5f 6576 656e  read_stream_even
-00004160: 7473 280a 2020 2020 2020 2020 7374 7265  ts(.        stre
-00004170: 616d 5f6e 616d 653d 7374 7265 616d 5f6e  am_name=stream_n
-00004180: 616d 6531 2c0a 2020 2020 2020 2020 706f  ame1,.        po
-00004190: 7369 7469 6f6e 3d32 2c0a 2020 2020 2020  sition=2,.      
-000041a0: 2020 6261 636b 7761 7264 733d 5472 7565    backwards=True
-000041b0: 2c0a 2020 2020 2020 2020 6c69 6d69 743d  ,.        limit=
-000041c0: 312c 0a20 2020 2029 0a29 0a0a 6173 7365  1,.    ).)..asse
-000041d0: 7274 206c 656e 2865 7665 6e74 7329 203d  rt len(events) =
-000041e0: 3d20 310a 0a61 7373 6572 7420 6576 656e  = 1..assert even
-000041f0: 7473 5b30 5d2e 7374 7265 616d 5f6e 616d  ts[0].stream_nam
-00004200: 6520 3d3d 2073 7472 6561 6d5f 6e61 6d65  e == stream_name
-00004210: 310a 6173 7365 7274 2065 7665 6e74 735b  1.assert events[
-00004220: 305d 2e73 7472 6561 6d5f 706f 7369 7469  0].stream_positi
-00004230: 6f6e 203d 3d20 320a 6173 7365 7274 2065  on == 2.assert e
-00004240: 7665 6e74 735b 305d 2e74 7970 6520 3d3d  vents[0].type ==
-00004250: 2065 7665 6e74 332e 7479 7065 0a61 7373   event3.type.ass
-00004260: 6572 7420 6576 656e 7473 5b30 5d2e 6461  ert events[0].da
-00004270: 7461 203d 3d20 6576 656e 7433 2e64 6174  ta == event3.dat
-00004280: 610a 6060 600a 0a23 2323 2049 6465 6d70  a.```..### Idemp
-00004290: 6f74 656e 7420 7772 6974 6573 0a0a 4e6f  otent writes..No
-000042a0: 7720 7468 6174 2077 6520 6361 6e20 626f  w that we can bo
-000042b0: 7468 2061 7070 656e 6420 6576 656e 7473  th append events
-000042c0: 2061 6e64 2072 6561 6420 6672 6f6d 2061   and read from a
-000042d0: 2073 7472 6561 6d2c 2077 6520 6361 6e20   stream, we can 
-000042e0: 6465 6d6f 6e73 7472 6174 650a 7468 6520  demonstrate.the 
-000042f0: 6964 656d 706f 7465 6e74 206e 6174 7572  idempotent natur
-00004300: 6520 6f66 2074 6865 2060 6170 7065 6e64  e of the `append
-00004310: 5f65 7665 6e74 7328 2960 206f 7065 7261  _events()` opera
-00004320: 7469 6f6e 2e0a 0a53 6f6d 6574 696d 6573  tion...Sometimes
-00004330: 2069 7420 6d61 7920 6861 7070 656e 2074   it may happen t
-00004340: 6861 7420 6120 6e65 7720 6576 656e 7420  hat a new event 
-00004350: 6973 2073 7563 6365 7373 6675 6c6c 7920  is successfully 
-00004360: 7265 636f 7264 6564 2061 6e64 2074 6865  recorded and the
-00004370: 6e20 736f 6d65 686f 770a 7468 6520 636f  n somehow.the co
-00004380: 6e6e 6563 7469 6f6e 2074 6f20 7468 6520  nnection to the 
-00004390: 6461 7461 6261 7365 2067 6574 7320 696e  database gets in
-000043a0: 7465 7272 7570 7465 6420 6265 666f 7265  terrupted before
-000043b0: 2074 6865 2073 7563 6365 7373 6675 6c20   the successful 
-000043c0: 6361 6c6c 2063 616e 2072 6574 7572 6e0a  call can return.
-000043d0: 7375 6363 6573 7366 756c 6c79 2074 6f20  successfully to 
-000043e0: 7468 6520 636c 6965 6e74 2e20 496e 2063  the client. In c
-000043f0: 6173 6520 6f66 2061 6e20 6572 726f 7220  ase of an error 
-00004400: 7768 656e 2061 7070 656e 6469 6e67 2061  when appending a
-00004410: 6e20 6576 656e 742c 2069 7420 6d61 7920  n event, it may 
-00004420: 6265 0a64 6573 6972 6162 6c65 2074 6f20  be.desirable to 
-00004430: 7265 7472 7920 6170 7065 6e64 696e 6720  retry appending 
-00004440: 7468 6520 7361 6d65 2065 7665 6e74 2061  the same event a
-00004450: 7420 7468 6520 7361 6d65 2070 6f73 6974  t the same posit
-00004460: 696f 6e2e 2049 6620 7468 6520 6576 656e  ion. If the even
-00004470: 7420 7761 730a 696e 2066 6163 7420 7375  t was.in fact su
-00004480: 6363 6573 7366 756c 6c79 2072 6563 6f72  ccessfully recor
-00004490: 6465 642c 2069 7420 6973 2063 6f6e 7665  ded, it is conve
-000044a0: 6e69 656e 7420 666f 7220 7468 6520 7265  nient for the re
-000044b0: 7472 7920 746f 2072 6574 7572 6e20 7375  try to return su
-000044c0: 6363 6573 7366 756c 6c79 0a77 6974 686f  ccessfully.witho
-000044d0: 7574 2072 6169 7369 6e67 2061 6e20 6572  ut raising an er
-000044e0: 726f 7220 6475 6520 746f 206f 7074 696d  ror due to optim
-000044f0: 6973 7469 6320 636f 6e63 7572 7265 6e63  istic concurrenc
-00004500: 7920 636f 6e74 726f 6c20 2861 7320 6465  y control (as de
-00004510: 7363 7269 6265 6420 6162 6f76 6529 2e0a  scribed above)..
-00004520: 0a54 6865 2065 7861 6d70 6c65 2062 656c  .The example bel
-00004530: 6f77 2073 686f 7773 2074 6865 2060 6170  ow shows the `ap
-00004540: 7065 6e64 5f65 7665 6e74 7328 2960 206d  pend_events()` m
-00004550: 6574 686f 6420 6265 696e 6720 6361 6c6c  ethod being call
-00004560: 6564 2061 6761 696e 2077 6974 680a 6065  ed again with.`e
-00004570: 7665 6e74 3360 2061 6e64 2060 6578 7065  vent3` and `expe
-00004580: 6374 6564 5f70 6f73 6974 696f 6e3d 3260  cted_position=2`
-00004590: 2e0a 0a60 6060 7079 7468 6f6e 0a23 2052  ...```python.# R
-000045a0: 6574 7279 2061 7070 656e 6469 6e67 2065  etry appending e
-000045b0: 7665 6e74 332e 0a63 6f6d 6d69 745f 706f  vent3..commit_po
-000045c0: 7369 7469 6f6e 5f72 6574 7279 203d 2063  sition_retry = c
-000045d0: 6c69 656e 742e 6170 7065 6e64 5f65 7665  lient.append_eve
-000045e0: 6e74 7328 0a20 2020 2073 7472 6561 6d5f  nts(.    stream_
-000045f0: 6e61 6d65 3d73 7472 6561 6d5f 6e61 6d65  name=stream_name
-00004600: 312c 0a20 2020 2065 7870 6563 7465 645f  1,.    expected_
-00004610: 706f 7369 7469 6f6e 3d30 2c0a 2020 2020  position=0,.    
-00004620: 6576 656e 7473 3d5b 6576 656e 7432 2c20  events=[event2, 
-00004630: 6576 656e 7433 5d2c 0a29 0a60 6060 0a0a  event3],.).```..
-00004640: 5765 2063 616e 2073 6565 2074 6861 7420  We can see that 
-00004650: 7468 6520 7361 6d65 2063 6f6d 6d69 7420  the same commit 
-00004660: 706f 7369 7469 6f6e 2069 7320 7265 7475  position is retu
-00004670: 726e 6564 2061 7320 6162 6f76 652e 0a0a  rned as above...
-00004680: 6060 6070 7974 686f 6e0a 6173 7365 7274  ```python.assert
-00004690: 2063 6f6d 6d69 745f 706f 7369 7469 6f6e   commit_position
-000046a0: 5f72 6574 7279 203d 3d20 636f 6d6d 6974  _retry == commit
-000046b0: 5f70 6f73 6974 696f 6e32 0a60 6060 0a0a  _position2.```..
-000046c0: 5468 6973 2077 6f72 6b73 2062 6563 6175  This works becau
-000046d0: 7365 2074 6865 2060 4e65 7745 7665 6e74  se the `NewEvent
-000046e0: 6020 636c 6173 7320 6861 7320 616e 2060  ` class has an `
-000046f0: 6964 6020 6174 7472 6962 7574 6520 7468  id` attribute th
-00004700: 6174 0a69 7320 7375 7070 6c69 6564 2077  at.is supplied w
-00004710: 6974 6820 6120 6e65 7720 7665 7273 696f  ith a new versio
-00004720: 6e2d 3420 5555 4944 2077 6865 6e20 616e  n-4 UUID when an
-00004730: 2069 6e73 7461 6e63 6520 6973 2063 6f6e   instance is con
-00004740: 7374 7275 6374 6564 2e0a 0a60 6060 7079  structed...```py
-00004750: 7468 6f6e 0a61 7373 6572 7420 6973 696e  thon.assert isin
-00004760: 7374 616e 6365 2865 7665 6e74 312e 6964  stance(event1.id
-00004770: 2c20 5555 4944 290a 6173 7365 7274 2069  , UUID).assert i
-00004780: 7369 6e73 7461 6e63 6528 6576 656e 7432  sinstance(event2
-00004790: 2e69 642c 2055 5549 4429 0a61 7373 6572  .id, UUID).asser
-000047a0: 7420 6973 696e 7374 616e 6365 2865 7665  t isinstance(eve
-000047b0: 6e74 332e 6964 2c20 5555 4944 290a 0a61  nt3.id, UUID)..a
-000047c0: 7373 6572 7420 6576 656e 7431 2e69 6420  ssert event1.id 
-000047d0: 213d 2065 7665 6e74 322e 6964 0a61 7373  != event2.id.ass
-000047e0: 6572 7420 6576 656e 7432 2e69 6420 213d  ert event2.id !=
-000047f0: 2065 7665 6e74 332e 6964 0a60 6060 0a0a   event3.id.```..
-00004800: 4974 2069 7320 706f 7373 6962 6c65 2074  It is possible t
-00004810: 6f20 7072 6f76 6964 6520 616e 2060 6964  o provide an `id
-00004820: 6020 7661 6c75 6520 7768 656e 2063 6f6e  ` value when con
-00004830: 7374 7275 6374 696e 6720 696e 7374 616e  structing instan
-00004840: 6365 7320 6f66 0a60 4e65 7745 7665 6e74  ces of.`NewEvent
-00004850: 602c 2062 7574 2069 6e20 7468 6520 6578  `, but in the ex
-00004860: 616d 706c 6573 2061 626f 7665 2077 6520  amples above we 
-00004870: 6861 7665 2062 6565 6e20 7573 696e 6720  have been using 
-00004880: 7468 6520 6465 6661 756c 7420 6265 6861  the default beha
-00004890: 7669 6f75 722e 0a0a 5765 2063 616e 2073  viour...We can s
-000048a0: 6565 2074 6861 7420 7468 6520 6061 7070  ee that the `app
-000048b0: 656e 645f 6576 656e 7473 2829 6020 6d65  end_events()` me
-000048c0: 7468 6f64 2072 6574 7572 6e73 2073 7563  thod returns suc
-000048d0: 6365 7373 6675 6c6c 792c 2061 6e64 0a74  cessfully, and.t
-000048e0: 6861 7420 7468 6520 7374 7265 616d 2068  hat the stream h
-000048f0: 6173 2062 6565 6e20 756e 6368 616e 6765  as been unchange
-00004900: 6420 6279 2063 616c 6c69 6e67 2074 6865  d by calling the
-00004910: 206d 6574 686f 6420 7477 6963 6520 7769   method twice wi
-00004920: 7468 2074 6865 0a73 616d 6520 6172 6775  th the.same argu
-00004930: 6d65 6e74 732e 0a0a 6060 6070 7974 686f  ments...```pytho
-00004940: 6e0a 7265 7370 6f6e 7365 203d 2063 6c69  n.response = cli
-00004950: 656e 742e 7265 6164 5f73 7472 6561 6d5f  ent.read_stream_
-00004960: 6576 656e 7473 280a 2020 2020 7374 7265  events(.    stre
-00004970: 616d 5f6e 616d 653d 7374 7265 616d 5f6e  am_name=stream_n
-00004980: 616d 6531 0a29 0a0a 6576 656e 7473 203d  ame1.)..events =
-00004990: 206c 6973 7428 7265 7370 6f6e 7365 290a   list(response).
-000049a0: 6173 7365 7274 2065 7665 6e74 735b 305d  assert events[0]
-000049b0: 2e69 6420 3d3d 2065 7665 6e74 312e 6964  .id == event1.id
-000049c0: 0a61 7373 6572 7420 6576 656e 7473 5b31  .assert events[1
-000049d0: 5d2e 6964 203d 3d20 6576 656e 7432 2e69  ].id == event2.i
-000049e0: 640a 6173 7365 7274 2065 7665 6e74 735b  d.assert events[
-000049f0: 325d 2e69 6420 3d3d 2065 7665 6e74 332e  2].id == event3.
-00004a00: 6964 0a60 6060 0a0a 0a23 2323 2052 6561  id.```...### Rea
-00004a10: 6420 616c 6c20 7265 636f 7264 6564 2065  d all recorded e
-00004a20: 7665 6e74 730a 0a54 6865 206d 6574 686f  vents..The metho
-00004a30: 6420 6072 6561 645f 616c 6c5f 6576 656e  d `read_all_even
-00004a40: 7473 2829 6020 6361 6e20 6265 2075 7365  ts()` can be use
-00004a50: 6420 746f 2072 6561 6420 616c 6c20 7265  d to read all re
-00004a60: 636f 7264 6564 2065 7665 6e74 730a 696e  corded events.in
-00004a70: 2074 6865 2064 6174 6162 6173 6520 696e   the database in
-00004a80: 2074 6865 206f 7264 6572 2074 6865 7920   the order they 
-00004a90: 7765 7265 2072 6563 6f72 6465 642e 2041  were recorded. A
-00004aa0: 6e20 6974 6572 6162 6c65 206f 626a 6563  n iterable objec
-00004ab0: 7420 6f66 0a72 6563 6f72 6465 6420 6576  t of.recorded ev
-00004ac0: 656e 7473 2069 7320 7265 7475 726e 6564  ents is returned
-00004ad0: 2e20 5468 6973 2069 7465 7261 626c 6520  . This iterable 
-00004ae0: 6f62 6a65 6374 2077 696c 6c20 7374 6f70  object will stop
-00004af0: 2077 6865 6e20 6974 2068 6173 0a79 6965   when it has.yie
-00004b00: 6c64 6564 2074 6865 206c 6173 7420 7265  lded the last re
-00004b10: 636f 7264 6564 2065 7665 6e74 2e0a 0a54  corded event...T
-00004b20: 6865 206d 6574 686f 6420 6072 6561 645f  he method `read_
-00004b30: 7374 7265 616d 5f65 7665 6e74 7328 2960  stream_events()`
-00004b40: 2073 7570 706f 7274 7320 7369 7820 6f70   supports six op
-00004b50: 7469 6f6e 616c 2061 7267 756d 656e 7473  tional arguments
-00004b60: 2c0a 6063 6f6d 6d69 745f 706f 7369 7469  ,.`commit_positi
-00004b70: 6f6e 602c 2060 6261 636b 7761 7264 7360  on`, `backwards`
-00004b80: 2c20 6066 696c 7465 725f 6578 636c 7564  , `filter_exclud
-00004b90: 6560 2c20 6066 696c 7465 725f 696e 636c  e`, `filter_incl
-00004ba0: 7564 6560 2c20 606c 696d 6974 602c 0a61  ude`, `limit`,.a
-00004bb0: 6e64 2060 7469 6d65 6f75 7460 2e0a 0a54  nd `timeout`...T
-00004bc0: 6865 206f 7074 696f 6e61 6c20 6172 6775  he optional argu
-00004bd0: 6d65 6e74 2060 706f 7369 7469 6f6e 6020  ment `position` 
-00004be0: 6973 2061 6e20 6f70 7469 6f6e 616c 2069  is an optional i
-00004bf0: 6e74 6567 6572 2074 6861 7420 6361 6e20  nteger that can 
-00004c00: 6265 2075 7365 6420 746f 2073 7065 6369  be used to speci
-00004c10: 6679 0a74 6865 2063 6f6d 6d69 7420 706f  fy.the commit po
-00004c20: 7369 7469 6f6e 2066 726f 6d20 7768 6963  sition from whic
-00004c30: 6820 746f 2073 7461 7274 2072 6561 6469  h to start readi
-00004c40: 6e67 2e20 5468 6973 2061 7267 756d 656e  ng. This argumen
-00004c50: 7420 6973 2060 4e6f 6e65 6020 6279 0a64  t is `None` by.d
-00004c60: 6566 6175 6c74 2c20 6d65 616e 696e 6720  efault, meaning 
-00004c70: 7468 6174 2061 6c6c 2074 6865 2065 7665  that all the eve
-00004c80: 6e74 7320 7769 6c6c 2062 6520 7265 6164  nts will be read
-00004c90: 2065 6974 6865 7220 6672 6f6d 2074 6865   either from the
-00004ca0: 2073 7461 7274 2c20 6f72 0a66 726f 6d20   start, or.from 
-00004cb0: 7468 6520 656e 6420 6966 2060 6261 636b  the end if `back
-00004cc0: 7761 7264 7360 2069 7320 6054 7275 6560  wards` is `True`
-00004cd0: 2028 7365 6520 6265 6c6f 7729 2e20 506c   (see below). Pl
-00004ce0: 6561 7365 206e 6f74 652c 2069 6620 7370  ease note, if sp
-00004cf0: 6563 6966 6965 642c 0a74 6865 2073 7065  ecified,.the spe
-00004d00: 6369 6669 6564 2070 6f73 6974 696f 6e20  cified position 
-00004d10: 6d75 7374 2062 6520 616e 2061 6374 7561  must be an actua
-00004d20: 6c6c 7920 6578 6973 7469 6e67 2063 6f6d  lly existing com
-00004d30: 6d69 7420 706f 7369 7469 6f6e 2c20 6265  mit position, be
-00004d40: 6361 7573 650a 616e 7920 6f74 6865 7220  cause.any other 
-00004d50: 6e75 6d62 6572 2077 696c 6c20 7265 7375  number will resu
-00004d60: 6c74 2069 6e20 6120 7365 7276 6572 2065  lt in a server e
-00004d70: 7272 6f72 2028 6174 206c 6561 7374 2069  rror (at least i
-00004d80: 6e20 4576 656e 7453 746f 7265 4442 2076  n EventStoreDB v
-00004d90: 3231 2e31 3029 2e0a 0a50 6c65 6173 6520  21.10)...Please 
-00004da0: 616c 736f 206e 6f74 652c 2077 6865 6e20  also note, when 
-00004db0: 7265 6164 696e 6720 666f 7277 6172 6473  reading forwards
-00004dc0: 2066 726f 6d20 6120 7370 6563 6966 6963   from a specific
-00004dd0: 2063 6f6d 6d69 7420 706f 7369 7469 6f6e   commit position
-00004de0: 2c20 7468 6520 6576 656e 740a 6174 2074  , the event.at t
-00004df0: 6865 2073 7065 6369 6669 6564 2070 6f73  he specified pos
-00004e00: 6974 696f 6e20 5749 4c4c 2062 6520 696e  ition WILL be in
-00004e10: 636c 7564 6564 2e20 486f 7765 7665 722c  cluded. However,
-00004e20: 2077 6865 6e20 7265 6164 696e 6720 6261   when reading ba
-00004e30: 636b 7761 7264 732c 2074 6865 0a65 7665  ckwards, the.eve
-00004e40: 6e74 2061 7420 7468 6520 7370 6563 6966  nt at the specif
-00004e50: 6965 6420 706f 7369 7469 6f6e 2077 696c  ied position wil
-00004e60: 6c20 4e4f 5420 6265 2069 6e63 6c75 6465  l NOT be include
-00004e70: 642e 2028 5468 6973 206e 6f6e 2d69 6e63  d. (This non-inc
-00004e80: 6c75 7369 7665 2062 6568 6176 696f 7572  lusive behaviour
-00004e90: 0a6f 6620 6578 636c 7564 696e 6720 7468  .of excluding th
-00004ea0: 6520 7370 6563 6966 6965 6420 636f 6d6d  e specified comm
-00004eb0: 6974 2070 6f73 6974 696f 6e20 7768 656e  it position when
-00004ec0: 2072 6561 6469 6e67 2061 6c6c 2073 7472   reading all str
-00004ed0: 6561 6d73 2064 6966 6665 7273 2066 726f  eams differs fro
-00004ee0: 6d20 7468 650a 6265 6861 7669 6f75 7220  m the.behaviour 
-00004ef0: 7768 656e 2072 6561 6469 6e67 2061 206e  when reading a n
-00004f00: 616d 6564 2073 7472 6561 6d20 6261 636b  amed stream back
-00004f10: 7761 7264 7320 6672 6f6d 2061 2073 7065  wards from a spe
-00004f20: 6369 6669 6320 7374 7265 616d 2070 6f73  cific stream pos
-00004f30: 6974 696f 6e2c 2049 276d 0a6e 6f74 2073  ition, I'm.not s
-00004f40: 7572 6520 7768 792e 290a 0a54 6865 206f  ure why.)..The o
-00004f50: 7074 696f 6e61 6c20 6172 6775 6d65 6e74  ptional argument
-00004f60: 2060 6261 636b 7761 7264 7360 2069 7320   `backwards` is 
-00004f70: 6120 626f 6f6c 6561 6e20 7768 6963 6820  a boolean which 
-00004f80: 6973 2062 7920 6465 6661 756c 7420 6046  is by default `F
-00004f90: 616c 7365 6020 6d65 616e 696e 6720 7468  alse` meaning th
-00004fa0: 650a 6576 656e 7473 2077 696c 6c20 6265  e.events will be
-00004fb0: 2072 6561 6420 666f 7277 6172 6473 2062   read forwards b
-00004fc0: 7920 6465 6661 756c 742c 2073 6f20 7468  y default, so th
-00004fd0: 6174 2065 7665 6e74 7320 6172 6520 7265  at events are re
-00004fe0: 7475 726e 6564 2069 6e20 7468 650a 6f72  turned in the.or
-00004ff0: 6465 7220 7468 6579 2077 6572 6520 636f  der they were co
-00005000: 6d6d 6974 7465 642c 2049 6620 6062 6163  mmitted, If `bac
-00005010: 6b77 6172 6473 6020 6973 2060 5472 7565  kwards` is `True
-00005020: 602c 2074 6865 2065 7665 6e74 7320 7769  `, the events wi
-00005030: 6c6c 2062 6520 7265 6164 0a62 6163 6b77  ll be read.backw
-00005040: 6172 6473 2c20 736f 2074 6861 7420 6576  ards, so that ev
-00005050: 656e 7473 2061 7265 2072 6574 7572 6e65  ents are returne
-00005060: 6420 696e 2072 6576 6572 7365 206f 7264  d in reverse ord
-00005070: 6572 2e0a 0a54 6865 206f 7074 696f 6e61  er...The optiona
-00005080: 6c20 6172 6775 6d65 6e74 2060 6669 6c74  l argument `filt
-00005090: 6572 5f65 7863 6c75 6465 6020 6973 2061  er_exclude` is a
-000050a0: 2073 6571 7565 6e63 6520 6f66 2072 6567   sequence of reg
-000050b0: 756c 6172 2065 7870 7265 7373 696f 6e73  ular expressions
-000050c0: 2074 6861 740a 6d61 7463 6820 7468 6520   that.match the 
-000050d0: 7479 7065 2073 7472 696e 6773 206f 6620  type strings of 
-000050e0: 7265 636f 7264 6564 2065 7665 6e74 7320  recorded events 
-000050f0: 7468 6174 2073 686f 756c 6420 6e6f 7420  that should not 
-00005100: 6265 2069 6e63 6c75 6465 642e 2042 7920  be included. By 
-00005110: 6465 6661 756c 742c 0a74 6869 7320 6172  default,.this ar
-00005120: 6775 6d65 6e74 2077 696c 6c20 6d61 7463  gument will matc
-00005130: 6820 2273 7973 7465 6d20 6576 656e 7473  h "system events
-00005140: 222c 2073 6f20 7468 6174 2074 6865 7920  ", so that they 
-00005150: 7769 6c6c 206e 6f74 2062 6520 696e 636c  will not be incl
-00005160: 7564 6564 2e0a 5468 6973 2061 7267 756d  uded..This argum
-00005170: 656e 7420 6973 2069 676e 6f72 6564 2069  ent is ignored i
-00005180: 6620 6066 696c 7465 725f 696e 636c 7564  f `filter_includ
-00005190: 6560 2069 7320 7365 7420 746f 2061 206e  e` is set to a n
-000051a0: 6f6e 2d65 6d70 7479 2073 6571 7565 6e63  on-empty sequenc
-000051b0: 652e 0a0a 5468 6520 6f70 7469 6f6e 616c  e...The optional
-000051c0: 2061 7267 756d 656e 7420 6066 696c 7465   argument `filte
-000051d0: 725f 696e 636c 7564 6560 2069 7320 6120  r_include` is a 
-000051e0: 7365 7175 656e 6365 206f 6620 7265 6775  sequence of regu
-000051f0: 6c61 7220 6578 7072 6573 7369 6f6e 730a  lar expressions.
-00005200: 7468 6174 206d 6174 6368 2074 6865 2074  that match the t
-00005210: 7970 6520 7374 7269 6e67 7320 6f66 2072  ype strings of r
-00005220: 6563 6f72 6465 6420 6576 656e 7473 2074  ecorded events t
-00005230: 6861 7420 7368 6f75 6c64 2062 6520 696e  hat should be in
-00005240: 636c 7564 6564 2e20 4279 0a64 6566 6175  cluded. By.defau
-00005250: 6c74 2c20 7468 6973 2061 7267 756d 656e  lt, this argumen
-00005260: 7420 6973 2061 6e20 656d 7074 7920 7475  t is an empty tu
-00005270: 706c 652e 2049 6620 7468 6973 2061 7267  ple. If this arg
-00005280: 756d 656e 7420 6973 2073 6574 2074 6f20  ument is set to 
-00005290: 610a 6e6f 6e2d 656d 7074 7920 7365 7175  a.non-empty sequ
-000052a0: 656e 6365 2c20 7468 6520 6066 696c 7465  ence, the `filte
-000052b0: 725f 6578 636c 7564 6560 2061 7267 756d  r_exclude` argum
-000052c0: 656e 7420 6973 2069 676e 6f72 6564 2e0a  ent is ignored..
-000052d0: 0a50 6c65 6173 6520 6e6f 7465 2c20 7468  .Please note, th
-000052e0: 6520 6669 6c74 6572 696e 6720 6861 7070  e filtering happ
-000052f0: 656e 7320 6f6e 2074 6865 2045 7665 6e74  ens on the Event
-00005300: 5374 6f72 6544 4220 7365 7276 6572 2c20  StoreDB server, 
-00005310: 616e 6420 7468 650a 606c 696d 6974 6020  and the.`limit` 
-00005320: 6172 6775 6d65 6e74 2069 7320 6170 706c  argument is appl
-00005330: 6965 6420 6f6e 2074 6865 2073 6572 7665  ied on the serve
-00005340: 7220 6166 7465 7220 6669 6c74 6572 696e  r after filterin
-00005350: 672e 2053 6565 2062 656c 6f77 2066 6f72  g. See below for
-00005360: 0a6d 6f72 6520 696e 666f 726d 6174 696f  .more informatio
-00005370: 6e20 6162 6f75 7420 6669 6c74 6572 2072  n about filter r
-00005380: 6567 756c 6172 2065 7870 7265 7373 696f  egular expressio
-00005390: 6e73 2e0a 0a54 6865 206f 7074 696f 6e61  ns...The optiona
-000053a0: 6c20 6172 6775 6d65 6e74 2060 6c69 6d69  l argument `limi
-000053b0: 7460 2069 7320 616e 2069 6e74 6567 6572  t` is an integer
-000053c0: 2077 6869 6368 206c 696d 6974 7320 7468   which limits th
-000053d0: 6520 6e75 6d62 6572 206f 6620 6576 656e  e number of even
-000053e0: 7473 2074 6861 7420 7769 6c6c 0a62 6520  ts that will.be 
-000053f0: 7265 7475 726e 6564 2e20 5468 6520 6465  returned. The de
-00005400: 6661 756c 7420 7661 6c75 6520 6973 2060  fault value is `
-00005410: 7379 732e 6d61 7869 6e74 602e 0a0a 5468  sys.maxint`...Th
-00005420: 6520 6f70 7469 6f6e 616c 2061 7267 756d  e optional argum
-00005430: 656e 7420 6074 696d 656f 7574 6020 6973  ent `timeout` is
-00005440: 2061 2066 6c6f 6174 2077 6869 6368 2073   a float which s
-00005450: 6574 7320 6120 6465 6164 6c69 6e65 2066  ets a deadline f
-00005460: 6f72 2074 6865 2063 6f6d 706c 6574 696f  or the completio
-00005470: 6e20 6f66 0a74 6865 2067 5250 4320 6f70  n of.the gRPC op
-00005480: 6572 6174 696f 6e2e 0a0a 5468 6520 6578  eration...The ex
-00005490: 616d 706c 6520 6265 6c6f 7720 7368 6f77  ample below show
-000054a0: 7320 686f 7720 746f 2072 6561 6420 616c  s how to read al
-000054b0: 6c20 6576 656e 7473 2069 6e20 7468 6520  l events in the 
-000054c0: 6461 7461 6261 7365 2069 6e20 7468 650a  database in the.
-000054d0: 6f72 6465 7220 7468 6579 2077 6572 6520  order they were 
-000054e0: 7265 636f 7264 6564 2e0a 0a60 6060 7079  recorded...```py
-000054f0: 7468 6f6e 0a65 7665 6e74 7320 3d20 6c69  thon.events = li
-00005500: 7374 2863 6c69 656e 742e 7265 6164 5f61  st(client.read_a
-00005510: 6c6c 5f65 7665 6e74 7328 2929 0a0a 6173  ll_events())..as
-00005520: 7365 7274 206c 656e 2865 7665 6e74 7329  sert len(events)
-00005530: 203e 3d20 330a 6060 600a 0a54 6865 2065   >= 3.```..The e
-00005540: 7861 6d70 6c65 2062 656c 6f77 2073 686f  xample below sho
-00005550: 7773 2068 6f77 2074 6f20 7265 6164 2061  ws how to read a
-00005560: 6c6c 2072 6563 6f72 6465 6420 6576 656e  ll recorded even
-00005570: 7473 2066 726f 6d20 6120 7061 7274 6963  ts from a partic
-00005580: 756c 6172 2063 6f6d 6d69 7420 706f 7369  ular commit posi
-00005590: 7469 6f6e 2e0a 0a60 6060 7079 7468 6f6e  tion...```python
-000055a0: 0a65 7665 6e74 7320 3d20 6c69 7374 280a  .events = list(.
-000055b0: 2020 2020 636c 6965 6e74 2e72 6561 645f      client.read_
-000055c0: 616c 6c5f 6576 656e 7473 280a 2020 2020  all_events(.    
-000055d0: 2020 2020 636f 6d6d 6974 5f70 6f73 6974      commit_posit
-000055e0: 696f 6e3d 636f 6d6d 6974 5f70 6f73 6974  ion=commit_posit
-000055f0: 696f 6e31 0a20 2020 2029 0a29 0a0a 6173  ion1.    ).)..as
-00005600: 7365 7274 206c 656e 2865 7665 6e74 7329  sert len(events)
-00005610: 203d 3d20 330a 0a61 7373 6572 7420 6576   == 3..assert ev
-00005620: 656e 7473 5b30 5d2e 7374 7265 616d 5f6e  ents[0].stream_n
-00005630: 616d 6520 3d3d 2073 7472 6561 6d5f 6e61  ame == stream_na
-00005640: 6d65 310a 6173 7365 7274 2065 7665 6e74  me1.assert event
-00005650: 735b 305d 2e73 7472 6561 6d5f 706f 7369  s[0].stream_posi
-00005660: 7469 6f6e 203d 3d20 300a 6173 7365 7274  tion == 0.assert
-00005670: 2065 7665 6e74 735b 305d 2e74 7970 6520   events[0].type 
-00005680: 3d3d 2065 7665 6e74 312e 7479 7065 0a61  == event1.type.a
-00005690: 7373 6572 7420 6576 656e 7473 5b30 5d2e  ssert events[0].
-000056a0: 6461 7461 203d 3d20 6576 656e 7431 2e64  data == event1.d
-000056b0: 6174 610a 0a61 7373 6572 7420 6576 656e  ata..assert even
-000056c0: 7473 5b31 5d2e 7374 7265 616d 5f6e 616d  ts[1].stream_nam
-000056d0: 6520 3d3d 2073 7472 6561 6d5f 6e61 6d65  e == stream_name
-000056e0: 310a 6173 7365 7274 2065 7665 6e74 735b  1.assert events[
-000056f0: 315d 2e73 7472 6561 6d5f 706f 7369 7469  1].stream_positi
-00005700: 6f6e 203d 3d20 310a 6173 7365 7274 2065  on == 1.assert e
-00005710: 7665 6e74 735b 315d 2e74 7970 6520 3d3d  vents[1].type ==
-00005720: 2065 7665 6e74 322e 7479 7065 0a61 7373   event2.type.ass
-00005730: 6572 7420 6576 656e 7473 5b31 5d2e 6461  ert events[1].da
-00005740: 7461 203d 3d20 6576 656e 7432 2e64 6174  ta == event2.dat
-00005750: 610a 0a61 7373 6572 7420 6576 656e 7473  a..assert events
-00005760: 5b32 5d2e 7374 7265 616d 5f6e 616d 6520  [2].stream_name 
-00005770: 3d3d 2073 7472 6561 6d5f 6e61 6d65 310a  == stream_name1.
-00005780: 6173 7365 7274 2065 7665 6e74 735b 325d  assert events[2]
-00005790: 2e73 7472 6561 6d5f 706f 7369 7469 6f6e  .stream_position
-000057a0: 203d 3d20 320a 6173 7365 7274 2065 7665   == 2.assert eve
-000057b0: 6e74 735b 325d 2e74 7970 6520 3d3d 2065  nts[2].type == e
-000057c0: 7665 6e74 332e 7479 7065 0a61 7373 6572  vent3.type.asser
-000057d0: 7420 6576 656e 7473 5b32 5d2e 6461 7461  t events[2].data
-000057e0: 203d 3d20 6576 656e 7433 2e64 6174 610a   == event3.data.
-000057f0: 6060 600a 0a54 6865 2065 7861 6d70 6c65  ```..The example
-00005800: 2062 656c 6f77 2073 686f 7773 2068 6f77   below shows how
-00005810: 2074 6f20 7265 6164 2061 6c6c 2072 6563   to read all rec
-00005820: 6f72 6465 6420 6576 656e 7473 2069 6e20  orded events in 
-00005830: 7265 7665 7273 6520 6f72 6465 722e 0a0a  reverse order...
-00005840: 6060 6070 7974 686f 6e0a 6576 656e 7473  ```python.events
-00005850: 203d 206c 6973 7428 0a20 2020 2063 6c69   = list(.    cli
-00005860: 656e 742e 7265 6164 5f61 6c6c 5f65 7665  ent.read_all_eve
-00005870: 6e74 7328 0a20 2020 2020 2020 2062 6163  nts(.        bac
-00005880: 6b77 6172 6473 3d54 7275 650a 2020 2020  kwards=True.    
-00005890: 290a 290a 0a61 7373 6572 7420 6c65 6e28  ).)..assert len(
-000058a0: 6576 656e 7473 2920 3e3d 2033 0a0a 6173  events) >= 3..as
-000058b0: 7365 7274 2065 7665 6e74 735b 305d 2e73  sert events[0].s
-000058c0: 7472 6561 6d5f 6e61 6d65 203d 3d20 7374  tream_name == st
-000058d0: 7265 616d 5f6e 616d 6531 0a61 7373 6572  ream_name1.asser
-000058e0: 7420 6576 656e 7473 5b30 5d2e 7374 7265  t events[0].stre
-000058f0: 616d 5f70 6f73 6974 696f 6e20 3d3d 2032  am_position == 2
-00005900: 0a61 7373 6572 7420 6576 656e 7473 5b30  .assert events[0
-00005910: 5d2e 7479 7065 203d 3d20 6576 656e 7433  ].type == event3
-00005920: 2e74 7970 650a 6173 7365 7274 2065 7665  .type.assert eve
-00005930: 6e74 735b 305d 2e64 6174 6120 3d3d 2065  nts[0].data == e
-00005940: 7665 6e74 332e 6461 7461 0a0a 6173 7365  vent3.data..asse
-00005950: 7274 2065 7665 6e74 735b 315d 2e73 7472  rt events[1].str
-00005960: 6561 6d5f 6e61 6d65 203d 3d20 7374 7265  eam_name == stre
-00005970: 616d 5f6e 616d 6531 0a61 7373 6572 7420  am_name1.assert 
-00005980: 6576 656e 7473 5b31 5d2e 7374 7265 616d  events[1].stream
-00005990: 5f70 6f73 6974 696f 6e20 3d3d 2031 0a61  _position == 1.a
-000059a0: 7373 6572 7420 6576 656e 7473 5b31 5d2e  ssert events[1].
-000059b0: 7479 7065 203d 3d20 6576 656e 7432 2e74  type == event2.t
-000059c0: 7970 650a 6173 7365 7274 2065 7665 6e74  ype.assert event
-000059d0: 735b 315d 2e64 6174 6120 3d3d 2065 7665  s[1].data == eve
-000059e0: 6e74 322e 6461 7461 0a0a 6173 7365 7274  nt2.data..assert
-000059f0: 2065 7665 6e74 735b 325d 2e73 7472 6561   events[2].strea
-00005a00: 6d5f 6e61 6d65 203d 3d20 7374 7265 616d  m_name == stream
-00005a10: 5f6e 616d 6531 0a61 7373 6572 7420 6576  _name1.assert ev
-00005a20: 656e 7473 5b32 5d2e 7374 7265 616d 5f70  ents[2].stream_p
-00005a30: 6f73 6974 696f 6e20 3d3d 2030 0a61 7373  osition == 0.ass
-00005a40: 6572 7420 6576 656e 7473 5b32 5d2e 7479  ert events[2].ty
-00005a50: 7065 203d 3d20 6576 656e 7431 2e74 7970  pe == event1.typ
-00005a60: 650a 6173 7365 7274 2065 7665 6e74 735b  e.assert events[
-00005a70: 325d 2e64 6174 6120 3d3d 2065 7665 6e74  2].data == event
-00005a80: 312e 6461 7461 0a60 6060 0a0a 5468 6520  1.data.```..The 
-00005a90: 6578 616d 706c 6520 6265 6c6f 7720 7368  example below sh
-00005aa0: 6f77 7320 686f 7720 746f 2072 6561 6420  ows how to read 
-00005ab0: 6120 6c69 6d69 7465 6420 6e75 6d62 6572  a limited number
-00005ac0: 2028 6f6e 6529 206f 6620 7468 6520 7265   (one) of the re
-00005ad0: 636f 7264 6564 2065 7665 6e74 730a 696e  corded events.in
-00005ae0: 2074 6865 2064 6174 6162 6173 6520 666f   the database fo
-00005af0: 7277 6172 6473 2066 726f 6d20 6120 7370  rwards from a sp
-00005b00: 6563 6966 6963 2063 6f6d 6d69 7420 706f  ecific commit po
-00005b10: 7369 7469 6f6e 2e20 506c 6561 7365 206e  sition. Please n
-00005b20: 6f74 652c 2077 6865 6e20 7265 6164 696e  ote, when readin
-00005b30: 670a 616c 6c20 6576 656e 7473 2066 6f72  g.all events for
-00005b40: 7761 7264 7320 6672 6f6d 2061 2073 7065  wards from a spe
-00005b50: 6369 6669 6320 636f 6d6d 6974 2070 6f73  cific commit pos
-00005b60: 6974 696f 6e2c 2074 6865 2065 7665 6e74  ition, the event
-00005b70: 2061 7420 7468 6520 7370 6563 6966 6965   at the specifie
-00005b80: 640a 706f 7369 7469 6f6e 2057 494c 4c20  d.position WILL 
-00005b90: 6265 2069 6e63 6c75 6465 642e 0a0a 0a60  be included....`
-00005ba0: 6060 7079 7468 6f6e 0a65 7665 6e74 7320  ``python.events 
-00005bb0: 3d20 6c69 7374 280a 2020 2020 636c 6965  = list(.    clie
-00005bc0: 6e74 2e72 6561 645f 616c 6c5f 6576 656e  nt.read_all_even
-00005bd0: 7473 280a 2020 2020 2020 2020 636f 6d6d  ts(.        comm
-00005be0: 6974 5f70 6f73 6974 696f 6e3d 636f 6d6d  it_position=comm
-00005bf0: 6974 5f70 6f73 6974 696f 6e31 2c0a 2020  it_position1,.  
-00005c00: 2020 2020 2020 6c69 6d69 743d 312c 0a20        limit=1,. 
-00005c10: 2020 2029 0a29 0a0a 6173 7365 7274 206c     ).)..assert l
-00005c20: 656e 2865 7665 6e74 7329 203d 3d20 310a  en(events) == 1.
-00005c30: 0a61 7373 6572 7420 6576 656e 7473 5b30  .assert events[0
-00005c40: 5d2e 7374 7265 616d 5f6e 616d 6520 3d3d  ].stream_name ==
-00005c50: 2073 7472 6561 6d5f 6e61 6d65 310a 6173   stream_name1.as
-00005c60: 7365 7274 2065 7665 6e74 735b 305d 2e73  sert events[0].s
-00005c70: 7472 6561 6d5f 706f 7369 7469 6f6e 203d  tream_position =
-00005c80: 3d20 300a 6173 7365 7274 2065 7665 6e74  = 0.assert event
-00005c90: 735b 305d 2e74 7970 6520 3d3d 2065 7665  s[0].type == eve
-00005ca0: 6e74 312e 7479 7065 0a61 7373 6572 7420  nt1.type.assert 
-00005cb0: 6576 656e 7473 5b30 5d2e 6461 7461 203d  events[0].data =
-00005cc0: 3d20 6576 656e 7431 2e64 6174 610a 0a61  = event1.data..a
-00005cd0: 7373 6572 7420 6576 656e 7473 5b30 5d2e  ssert events[0].
-00005ce0: 636f 6d6d 6974 5f70 6f73 6974 696f 6e20  commit_position 
-00005cf0: 3d3d 2063 6f6d 6d69 745f 706f 7369 7469  == commit_positi
-00005d00: 6f6e 310a 6060 600a 0a54 6865 2065 7861  on1.```..The exa
-00005d10: 6d70 6c65 2062 656c 6f77 2073 686f 7773  mple below shows
-00005d20: 2068 6f77 2074 6f20 7265 6164 2061 206c   how to read a l
-00005d30: 696d 6974 6564 206e 756d 6265 7220 286f  imited number (o
-00005d40: 6e65 2920 6f66 2074 6865 2072 6563 6f72  ne) of the recor
-00005d50: 6465 6420 6576 656e 7473 0a69 6e20 7468  ded events.in th
-00005d60: 6520 6461 7461 6261 7365 2062 6163 6b77  e database backw
-00005d70: 6172 6473 2066 726f 6d20 7468 6520 656e  ards from the en
-00005d80: 642e 2054 6869 7320 6769 7665 7320 7468  d. This gives th
-00005d90: 6520 6c61 7374 2072 6563 6f72 6465 6420  e last recorded 
-00005da0: 6576 656e 742e 0a0a 6060 6070 7974 686f  event...```pytho
-00005db0: 6e0a 6576 656e 7473 203d 206c 6973 7428  n.events = list(
-00005dc0: 0a20 2020 2063 6c69 656e 742e 7265 6164  .    client.read
-00005dd0: 5f61 6c6c 5f65 7665 6e74 7328 0a20 2020  _all_events(.   
-00005de0: 2020 2020 2062 6163 6b77 6172 6473 3d54       backwards=T
-00005df0: 7275 652c 0a20 2020 2020 2020 206c 696d  rue,.        lim
-00005e00: 6974 3d31 2c0a 2020 2020 290a 290a 0a61  it=1,.    ).)..a
-00005e10: 7373 6572 7420 6c65 6e28 6576 656e 7473  ssert len(events
-00005e20: 2920 3d3d 2031 0a0a 6173 7365 7274 2065  ) == 1..assert e
-00005e30: 7665 6e74 735b 305d 2e73 7472 6561 6d5f  vents[0].stream_
-00005e40: 6e61 6d65 203d 3d20 7374 7265 616d 5f6e  name == stream_n
-00005e50: 616d 6531 0a61 7373 6572 7420 6576 656e  ame1.assert even
-00005e60: 7473 5b30 5d2e 7374 7265 616d 5f70 6f73  ts[0].stream_pos
-00005e70: 6974 696f 6e20 3d3d 2032 0a61 7373 6572  ition == 2.asser
-00005e80: 7420 6576 656e 7473 5b30 5d2e 7479 7065  t events[0].type
-00005e90: 203d 3d20 6576 656e 7433 2e74 7970 650a   == event3.type.
-00005ea0: 6173 7365 7274 2065 7665 6e74 735b 305d  assert events[0]
-00005eb0: 2e64 6174 6120 3d3d 2065 7665 6e74 332e  .data == event3.
-00005ec0: 6461 7461 0a60 6060 0a0a 5468 6520 6578  data.```..The ex
-00005ed0: 616d 706c 6520 6265 6c6f 7720 7368 6f77  ample below show
-00005ee0: 7320 686f 7720 746f 2072 6561 6420 6120  s how to read a 
-00005ef0: 6c69 6d69 7465 6420 6e75 6d62 6572 2028  limited number (
-00005f00: 6f6e 6529 206f 6620 7468 6520 7265 636f  one) of the reco
-00005f10: 7264 6564 2065 7665 6e74 730a 696e 2074  rded events.in t
-00005f20: 6865 2064 6174 6162 6173 6520 6261 636b  he database back
-00005f30: 7761 7264 7320 6672 6f6d 2061 2073 7065  wards from a spe
-00005f40: 6369 6669 6320 636f 6d6d 6974 2070 6f73  cific commit pos
-00005f50: 6974 696f 6e2e 2050 6c65 6173 6520 6e6f  ition. Please no
-00005f60: 7465 2c20 7768 656e 2072 6561 6469 6e67  te, when reading
-00005f70: 0a61 6c6c 2065 7665 6e74 7320 6261 636b  .all events back
-00005f80: 7761 7264 7320 6672 6f6d 2061 2073 7065  wards from a spe
-00005f90: 6369 6669 6320 636f 6d6d 6974 2070 6f73  cific commit pos
-00005fa0: 6974 696f 6e2c 2074 6865 2065 7665 6e74  ition, the event
-00005fb0: 2061 7420 7468 6520 7370 6563 6966 6965   at the specifie
-00005fc0: 640a 706f 7369 7469 6f6e 2057 494c 4c20  d.position WILL 
-00005fd0: 4e4f 5420 6265 2069 6e63 6c75 6465 642e  NOT be included.
-00005fe0: 0a0a 6060 6070 7974 686f 6e0a 6576 656e  ..```python.even
-00005ff0: 7473 203d 206c 6973 7428 0a20 2020 2063  ts = list(.    c
-00006000: 6c69 656e 742e 7265 6164 5f61 6c6c 5f65  lient.read_all_e
-00006010: 7665 6e74 7328 0a20 2020 2020 2020 2063  vents(.        c
-00006020: 6f6d 6d69 745f 706f 7369 7469 6f6e 3d63  ommit_position=c
-00006030: 6f6d 6d69 745f 706f 7369 7469 6f6e 322c  ommit_position2,
-00006040: 0a20 2020 2020 2020 2062 6163 6b77 6172  .        backwar
-00006050: 6473 3d54 7275 652c 0a20 2020 2020 2020  ds=True,.       
-00006060: 206c 696d 6974 3d31 2c0a 2020 2020 290a   limit=1,.    ).
-00006070: 290a 0a61 7373 6572 7420 6c65 6e28 6576  )..assert len(ev
-00006080: 656e 7473 2920 3d3d 2031 0a0a 6173 7365  ents) == 1..asse
-00006090: 7274 2065 7665 6e74 735b 305d 2e63 6f6d  rt events[0].com
-000060a0: 6d69 745f 706f 7369 7469 6f6e 203c 2063  mit_position < c
-000060b0: 6f6d 6d69 745f 706f 7369 7469 6f6e 320a  ommit_position2.
-000060c0: 6060 600a 0a23 2323 2047 6574 2063 7572  ```..### Get cur
-000060d0: 7265 6e74 2063 6f6d 6d69 7420 706f 7369  rent commit posi
-000060e0: 7469 6f6e 0a0a 2a6f 6e6c 7920 7375 7070  tion..*only supp
-000060f0: 6f72 7465 6420 696e 2045 7665 6e74 5374  orted in EventSt
-00006100: 6f72 6544 4220 7665 7273 696f 6e20 3e3d  oreDB version >=
-00006110: 2032 322e 3130 2a0a 0a54 6865 206d 6574   22.10*..The met
-00006120: 686f 6420 6067 6574 5f63 6f6d 6d69 745f  hod `get_commit_
-00006130: 706f 7369 7469 6f6e 2829 6020 6361 6e20  position()` can 
-00006140: 6265 2075 7365 6420 746f 2067 6574 2074  be used to get t
-00006150: 6865 2063 7572 7265 6e74 0a63 6f6d 6d69  he current.commi
-00006160: 7420 706f 7369 7469 6f6e 206f 6620 7468  t position of th
-00006170: 6520 6461 7461 6261 7365 2e0a 0a60 6060  e database...```
-00006180: 7079 7468 6f6e 0a63 6f6d 6d69 745f 706f  python.commit_po
-00006190: 7369 7469 6f6e 203d 2063 6c69 656e 742e  sition = client.
-000061a0: 6765 745f 636f 6d6d 6974 5f70 6f73 6974  get_commit_posit
-000061b0: 696f 6e28 290a 6060 600a 0a54 6869 7320  ion().```..This 
-000061c0: 6d65 7468 6f64 2074 616b 6573 2061 6e20  method takes an 
-000061d0: 6f70 7469 6f6e 616c 2061 7267 756d 656e  optional argumen
-000061e0: 7420 6074 696d 656f 7574 6020 7768 6963  t `timeout` whic
-000061f0: 6820 6973 2061 2066 6c6f 6174 2074 6861  h is a float tha
-00006200: 7420 7365 7473 0a61 2064 6561 646c 696e  t sets.a deadlin
-00006210: 6520 666f 7220 7468 6520 636f 6d70 6c65  e for the comple
-00006220: 7469 6f6e 206f 6620 7468 6520 6752 5043  tion of the gRPC
-00006230: 206f 7065 7261 7469 6f6e 2e0a 0a54 6869   operation...Thi
-00006240: 7320 6d65 7468 6f64 2063 616e 2062 6520  s method can be 
-00006250: 7573 6566 756c 2074 6f20 6d65 6173 7572  useful to measur
-00006260: 6520 7072 6f67 7265 7373 206f 6620 6120  e progress of a 
-00006270: 646f 776e 7374 7265 616d 2063 6f6d 706f  downstream compo
-00006280: 6e65 6e74 0a74 6861 7420 6973 2070 726f  nent.that is pro
-00006290: 6365 7373 696e 6720 616c 6c20 7265 636f  cessing all reco
-000062a0: 7264 6564 2065 7665 6e74 732c 2062 7920  rded events, by 
-000062b0: 636f 6d70 6172 696e 6720 7468 6520 6375  comparing the cu
-000062c0: 7272 656e 7420 636f 6d6d 6974 0a70 6f73  rrent commit.pos
-000062d0: 6974 696f 6e20 7769 7468 2074 6865 2072  ition with the r
-000062e0: 6563 6f72 6465 6420 636f 6d6d 6974 2070  ecorded commit p
-000062f0: 6f73 6974 696f 6e20 6f66 2074 6865 206c  osition of the l
-00006300: 6173 7420 7375 6363 6573 7366 756c 6c79  ast successfully
-00006310: 2070 726f 6365 7373 6564 0a65 7665 6e74   processed.event
-00006320: 2069 6e20 6120 646f 776e 7374 7265 616d   in a downstream
-00006330: 2063 6f6d 706f 6e65 6e74 2e0a 0a54 6865   component...The
-00006340: 2076 616c 7565 206f 6620 7468 6520 6063   value of the `c
-00006350: 6f6d 6d69 745f 706f 7369 7469 6f6e 6020  ommit_position` 
-00006360: 6172 6775 6d65 6e74 2077 6865 6e20 7265  argument when re
-00006370: 6164 696e 6720 6576 656e 7473 2065 6974  ading events eit
-00006380: 6865 7220 6279 2075 7369 6e67 0a74 6865  her by using.the
-00006390: 2060 7265 6164 5f61 6c6c 5f65 7665 6e74   `read_all_event
-000063a0: 7328 2960 206d 6574 686f 6420 6f72 2062  s()` method or b
-000063b0: 7920 7573 696e 6720 6120 6361 7463 682d  y using a catch-
-000063c0: 7570 2073 7562 7363 7269 7074 696f 6e20  up subscription 
-000063d0: 776f 756c 6420 7573 7561 6c6c 790a 6265  would usually.be
-000063e0: 2064 6574 6572 6d69 6e65 6420 6279 2074   determined by t
-000063f0: 6865 2072 6563 6f72 6465 6420 636f 6d6d  he recorded comm
-00006400: 6974 2070 6f73 6974 696f 6e20 6f66 2074  it position of t
-00006410: 6865 206c 6173 7420 7375 6363 6573 7366  he last successf
-00006420: 756c 6c79 2070 726f 6365 7373 6564 0a65  ully processed.e
-00006430: 7665 6e74 2069 6e20 6120 646f 776e 7374  vent in a downst
-00006440: 7265 616d 2063 6f6d 706f 6e65 6e74 2e0a  ream component..
-00006450: 0a23 2320 5375 6273 6372 6970 7469 6f6e  .## Subscription
-00006460: 730a 0a23 2323 2043 6174 6368 2d75 7020  s..### Catch-up 
-00006470: 7375 6273 6372 6970 7469 6f6e 730a 0a54  subscriptions..T
-00006480: 6865 2063 6c69 656e 7420 6861 7320 6120  he client has a 
-00006490: 6073 7562 7363 7269 6265 5f61 6c6c 5f65  `subscribe_all_e
-000064a0: 7665 6e74 7328 2960 206d 6574 686f 642c  vents()` method,
-000064b0: 2077 6869 6368 2063 616e 2062 6520 7573   which can be us
-000064c0: 6564 0a74 6f20 7374 6172 7420 6120 2263  ed.to start a "c
-000064d0: 6174 6368 2d75 7022 2073 7562 7363 7269  atch-up" subscri
-000064e0: 7074 696f 6e2e 0a0a 4d61 6e79 2063 6174  ption...Many cat
-000064f0: 6368 2d75 7020 7375 6273 6372 6970 7469  ch-up subscripti
-00006500: 6f6e 7320 6361 6e20 6265 2063 7265 6174  ons can be creat
-00006510: 6564 2c20 636f 6e63 7572 7265 6e74 6c79  ed, concurrently
-00006520: 206f 720a 7375 6363 6573 7369 7665 6c79   or.successively
-00006530: 2c20 616e 6420 616c 6c20 7769 6c6c 2072  , and all will r
-00006540: 6563 6569 7665 2061 6c6c 2074 6865 2065  eceive all the e
-00006550: 7665 6e74 7320 7468 6579 2061 7265 0a73  vents they are.s
-00006560: 7562 7363 7269 6265 6420 746f 2072 6563  ubscribed to rec
-00006570: 6569 7665 2e0a 0a54 6869 7320 6d65 7468  eive...This meth
-00006580: 6f64 2072 6574 7572 6e73 2061 6e20 6974  od returns an it
-00006590: 6572 6174 6f72 206f 626a 6563 7420 7768  erator object wh
-000065a0: 6963 6820 7969 656c 6473 2072 6563 6f72  ich yields recor
-000065b0: 6465 6420 6576 656e 7473 2c0a 696e 636c  ded events,.incl
-000065c0: 7564 696e 6720 6576 656e 7473 2074 6861  uding events tha
-000065d0: 7420 6172 6520 7265 636f 7264 6564 2061  t are recorded a
-000065e0: 6674 6572 2074 6865 2073 7562 7363 7269  fter the subscri
-000065f0: 7074 696f 6e20 7761 7320 6372 6561 7465  ption was create
-00006600: 642e 0a54 6869 7320 6974 6572 6174 6f72  d..This iterator
-00006610: 206f 626a 6563 7420 7769 6c6c 2074 6865   object will the
-00006620: 7265 666f 7265 206e 6f74 2073 746f 702c  refore not stop,
-00006630: 2075 6e6c 6573 7320 7468 6520 636f 6e6e   unless the conn
-00006640: 6563 7469 6f6e 0a74 6f20 7468 6520 6461  ection.to the da
-00006650: 7461 6261 7365 2069 7320 6c6f 7374 2e20  tabase is lost. 
-00006660: 5468 6520 636f 6e6e 6563 7469 6f6e 2077  The connection w
-00006670: 696c 6c20 6265 2063 6c6f 7365 6420 7768  ill be closed wh
-00006680: 656e 2074 6865 0a69 7465 7261 746f 7220  en the.iterator 
-00006690: 6f62 6a65 6374 2069 7320 6465 6c65 7465  object is delete
-000066a0: 6420 6672 6f6d 206d 656d 6f72 792c 2077  d from memory, w
-000066b0: 6869 6368 2077 696c 6c20 6861 7070 656e  hich will happen
-000066c0: 2077 6865 6e20 7468 650a 6974 6572 6174   when the.iterat
-000066d0: 6f72 206f 626a 6563 7420 676f 6573 206f  or object goes o
-000066e0: 7574 206f 6620 7363 6f70 6520 6973 2065  ut of scope is e
-000066f0: 7870 6c69 6369 746c 7920 6465 6c65 7465  xplicitly delete
-00006700: 6420 2873 6565 2062 656c 6f77 292c 0a61  d (see below),.a
-00006710: 6e64 2074 6865 2063 6f6e 6e65 6374 696f  nd the connectio
-00006720: 6e20 6d61 7920 6265 2063 6c6f 7365 6420  n may be closed 
-00006730: 6279 2074 6865 2073 6572 7665 722e 0a0a  by the server...
-00006740: 5468 6973 206d 6574 686f 6420 7461 6b65  This method take
-00006750: 7320 616e 206f 7074 696f 6e61 6c20 6063  s an optional `c
-00006760: 6f6d 6d69 745f 706f 7369 7469 6f6e 6020  ommit_position` 
-00006770: 6172 6775 6d65 6e74 2c20 7768 6963 6820  argument, which 
-00006780: 6361 6e20 6265 0a75 7365 6420 746f 2073  can be.used to s
-00006790: 7065 6369 6679 2061 2063 6f6d 6d69 7420  pecify a commit 
-000067a0: 706f 7369 7469 6f6e 2066 726f 6d20 7768  position from wh
-000067b0: 6963 6820 746f 2073 7562 7363 7269 6265  ich to subscribe
-000067c0: 2066 6f72 0a72 6563 6f72 6465 6420 6576   for.recorded ev
-000067d0: 656e 7473 2e20 5468 6520 6465 6661 756c  ents. The defaul
-000067e0: 7420 7661 6c75 6520 6973 2060 4e6f 6e65  t value is `None
-000067f0: 602c 2077 6869 6368 206d 6561 6e73 0a74  `, which means.t
-00006800: 6865 2073 7562 7363 7269 7074 696f 6e20  he subscription 
-00006810: 7769 6c6c 206f 7065 7261 7465 2066 726f  will operate fro
-00006820: 6d20 7468 6520 6669 7273 7420 7265 636f  m the first reco
-00006830: 7264 6564 2065 7665 6e74 0a69 6e20 7468  rded event.in th
-00006840: 6520 6461 7461 6261 7365 2e20 4966 2061  e database. If a
-00006850: 2063 6f6d 6d69 7420 706f 7369 7469 6f6e   commit position
-00006860: 2069 7320 6769 7665 6e2c 2069 7420 6d75   is given, it mu
-00006870: 7374 206d 6174 6368 0a61 6e20 6163 7475  st match.an actu
-00006880: 616c 6c79 2065 7869 7374 696e 6720 636f  ally existing co
-00006890: 6d6d 6974 2070 6f73 6974 696f 6e20 696e  mmit position in
-000068a0: 2074 6865 2064 6174 6162 6173 652e 2054   the database. T
-000068b0: 6865 2065 7665 6e74 730a 7468 6174 2061  he events.that a
-000068c0: 7265 206f 6274 6169 6e65 6420 7769 6c6c  re obtained will
-000068d0: 206e 6f74 2069 6e63 6c75 6465 2074 6865   not include the
-000068e0: 2065 7665 6e74 2072 6563 6f72 6465 6420   event recorded 
-000068f0: 6174 2074 6861 7420 636f 6d6d 6974 0a70  at that commit.p
-00006900: 6f73 6974 696f 6e2e 0a0a 5468 6973 206d  osition...This m
-00006910: 6574 686f 6420 616c 736f 2074 616b 6573  ethod also takes
-00006920: 2074 6872 6565 206f 7468 6572 206f 7074   three other opt
-00006930: 696f 6e61 6c20 6172 6775 6d65 6e74 732c  ional arguments,
-00006940: 2060 6669 6c74 6572 5f65 7863 6c75 6465   `filter_exclude
-00006950: 602c 0a60 6669 6c74 6572 5f69 6e63 6c75  `,.`filter_inclu
-00006960: 6465 602c 2061 6e64 2060 7469 6d65 6f75  de`, and `timeou
-00006970: 7460 2e0a 0a54 6865 2061 7267 756d 656e  t`...The argumen
-00006980: 7420 6066 696c 7465 725f 6578 636c 7564  t `filter_exclud
-00006990: 6560 2069 7320 6120 7365 7175 656e 6365  e` is a sequence
-000069a0: 206f 6620 7265 6775 6c61 7220 6578 7072   of regular expr
-000069b0: 6573 7369 6f6e 7320 6d61 7463 6869 6e67  essions matching
-000069c0: 0a74 6865 2074 7970 6520 7374 7269 6e67  .the type string
-000069d0: 7320 6f66 2072 6563 6f72 6465 6420 6576  s of recorded ev
-000069e0: 656e 7473 2074 6861 7420 7368 6f75 6c64  ents that should
-000069f0: 2062 6520 6578 636c 7564 6564 2e20 4279   be excluded. By
-00006a00: 2064 6566 6175 6c74 2c0a 7468 6973 2061   default,.this a
-00006a10: 7267 756d 656e 7420 7769 6c6c 206d 6174  rgument will mat
-00006a20: 6368 2022 7379 7374 656d 2065 7665 6e74  ch "system event
-00006a30: 7322 2c20 736f 2074 6861 7420 7468 6579  s", so that they
-00006a40: 2077 696c 6c20 6e6f 7420 6265 2069 6e63   will not be inc
-00006a50: 6c75 6465 642e 0a54 6869 7320 6172 6775  luded..This argu
-00006a60: 6d65 6e74 2069 7320 6967 6e6f 7265 6420  ment is ignored 
-00006a70: 6966 2060 6669 6c74 6572 5f69 6e63 6c75  if `filter_inclu
-00006a80: 6465 6020 6973 2073 6574 2074 6f20 6120  de` is set to a 
-00006a90: 6e6f 6e2d 656d 7074 7920 7365 7175 656e  non-empty sequen
-00006aa0: 6365 2e0a 0a54 6865 2061 7267 756d 656e  ce...The argumen
-00006ab0: 7420 6066 696c 7465 725f 696e 636c 7564  t `filter_includ
-00006ac0: 6560 2069 7320 6120 7365 7175 656e 6365  e` is a sequence
-00006ad0: 206f 6620 7265 6775 6c61 7220 6578 7072   of regular expr
-00006ae0: 6573 7369 6f6e 730a 6d61 7463 6869 6e67  essions.matching
-00006af0: 2074 6865 2074 7970 6520 7374 7269 6e67   the type string
-00006b00: 7320 6f66 2072 6563 6f72 6465 6420 6576  s of recorded ev
-00006b10: 656e 7473 2074 6861 7420 7368 6f75 6c64  ents that should
-00006b20: 2062 6520 696e 636c 7564 6564 2e20 4279   be included. By
-00006b30: 0a64 6566 6175 6c74 2c20 7468 6973 2061  .default, this a
-00006b40: 7267 756d 656e 7420 6973 2061 6e20 656d  rgument is an em
-00006b50: 7074 7920 7475 706c 652e 2049 6620 7468  pty tuple. If th
-00006b60: 6973 2061 7267 756d 656e 7420 6973 2073  is argument is s
-00006b70: 6574 2074 6f20 610a 6e6f 6e2d 656d 7074  et to a.non-empt
-00006b80: 7920 7365 7175 656e 6365 2c20 7468 6520  y sequence, the 
-00006b90: 6066 696c 7465 725f 6578 636c 7564 6560  `filter_exclude`
-00006ba0: 2061 7267 756d 656e 7420 6973 2069 676e   argument is ign
-00006bb0: 6f72 6564 2e0a 0a50 6c65 6173 6520 6e6f  ored...Please no
-00006bc0: 7465 2c20 7468 6520 6669 6c74 6572 696e  te, the filterin
-00006bd0: 6720 6861 7070 656e 7320 6f6e 2074 6865  g happens on the
-00006be0: 2045 7665 6e74 5374 6f72 6544 4220 7365   EventStoreDB se
-00006bf0: 7276 6572 2c20 616e 6420 7468 650a 606c  rver, and the.`l
-00006c00: 696d 6974 6020 6172 6775 6d65 6e74 2069  imit` argument i
-00006c10: 7320 6170 706c 6965 6420 6f6e 2074 6865  s applied on the
-00006c20: 2073 6572 7665 7220 6166 7465 7220 6669   server after fi
-00006c30: 6c74 6572 696e 672e 2053 6565 2062 656c  ltering. See bel
-00006c40: 6f77 2066 6f72 0a6d 6f72 6520 696e 666f  ow for.more info
-00006c50: 726d 6174 696f 6e20 6162 6f75 7420 6669  rmation about fi
-00006c60: 6c74 6572 2072 6567 756c 6172 2065 7870  lter regular exp
-00006c70: 7265 7373 696f 6e73 2e0a 0a54 6865 2061  ressions...The a
-00006c80: 7267 756d 656e 7420 6074 696d 656f 7574  rgument `timeout
-00006c90: 6020 6973 2061 2066 6c6f 6174 2077 6869  ` is a float whi
-00006ca0: 6368 2073 6574 7320 6120 6465 6164 6c69  ch sets a deadli
-00006cb0: 6e65 2066 6f72 2074 6865 2063 6f6d 706c  ne for the compl
-00006cc0: 6574 696f 6e20 6f66 0a74 6865 2067 5250  etion of.the gRP
-00006cd0: 4320 6f70 6572 6174 696f 6e2e 2054 6869  C operation. Thi
-00006ce0: 7320 7072 6f62 6162 6c79 2069 736e 2774  s probably isn't
-00006cf0: 2076 6572 7920 7573 6566 756c 2c20 6275   very useful, bu
-00006d00: 7420 6973 2069 6e63 6c75 6465 6420 666f  t is included fo
-00006d10: 720a 636f 6d70 6c65 7465 6e65 7373 2061  r.completeness a
-00006d20: 6e64 2063 6f6e 7369 7374 656e 6379 2077  nd consistency w
-00006d30: 6974 6820 7468 6520 6f74 6865 7220 6d65  ith the other me
-00006d40: 7468 6f64 732e 0a0a 5468 6520 6578 616d  thods...The exam
-00006d50: 706c 6520 6265 6c6f 7720 7368 6f77 7320  ple below shows 
-00006d60: 686f 7720 746f 2073 7562 7363 7269 6265  how to subscribe
-00006d70: 2074 6f20 7265 6365 6976 6520 616c 6c20   to receive all 
-00006d80: 7265 636f 7264 6564 0a65 7665 6e74 7320  recorded.events 
-00006d90: 6672 6f6d 2061 2073 7065 6369 6669 6320  from a specific 
-00006da0: 636f 6d6d 6974 2070 6f73 6974 696f 6e2e  commit position.
-00006db0: 2054 6872 6565 2061 6c72 6561 6479 2d72   Three already-r
-00006dc0: 6563 6f72 6465 640a 6576 656e 7473 2061  ecorded.events a
-00006dd0: 7265 2072 6563 6569 7665 642c 2061 6e64  re received, and
-00006de0: 2074 6865 6e20 7468 7265 6520 6e65 7720   then three new 
-00006df0: 6576 656e 7473 2061 7265 2072 6563 6f72  events are recor
-00006e00: 6465 642c 2077 6869 6368 0a61 7265 2074  ded, which.are t
-00006e10: 6865 6e20 7265 6365 6976 6564 2076 6961  hen received via
-00006e20: 2074 6865 2073 7562 7363 7269 7074 696f   the subscriptio
-00006e30: 6e2e 0a0a 6060 6070 7974 686f 6e0a 0a23  n...```python..#
-00006e40: 2047 6574 2074 6865 2063 6f6d 6d69 7420   Get the commit 
-00006e50: 706f 7369 7469 6f6e 2028 7573 7561 6c6c  position (usuall
-00006e60: 7920 6672 6f6d 2064 6174 6162 6173 6520  y from database 
-00006e70: 6f66 206d 6174 6572 6961 6c69 7365 6420  of materialised 
-00006e80: 7669 6577 7329 2e0a 636f 6d6d 6974 5f70  views)..commit_p
-00006e90: 6f73 6974 696f 6e20 3d20 636c 6965 6e74  osition = client
-00006ea0: 2e67 6574 5f63 6f6d 6d69 745f 706f 7369  .get_commit_posi
-00006eb0: 7469 6f6e 2829 0a0a 2320 4170 7065 6e64  tion()..# Append
-00006ec0: 2074 6872 6565 2065 7665 6e74 7320 746f   three events to
-00006ed0: 2061 6e6f 7468 6572 2073 7472 6561 6d2e   another stream.
-00006ee0: 0a73 7472 6561 6d5f 6e61 6d65 3220 3d20  .stream_name2 = 
-00006ef0: 7374 7228 7575 6964 3428 2929 0a65 7665  str(uuid4()).eve
-00006f00: 6e74 3420 3d20 4e65 7745 7665 6e74 280a  nt4 = NewEvent(.
-00006f10: 2020 2020 7479 7065 3d27 4f72 6465 7243      type='OrderC
-00006f20: 7265 6174 6564 272c 0a20 2020 2064 6174  reated',.    dat
-00006f30: 613d 6227 6461 7461 3427 2c0a 290a 6576  a=b'data4',.).ev
-00006f40: 656e 7435 203d 204e 6577 4576 656e 7428  ent5 = NewEvent(
-00006f50: 0a20 2020 2074 7970 653d 274f 7264 6572  .    type='Order
-00006f60: 5570 6461 7465 6427 2c0a 2020 2020 6461  Updated',.    da
-00006f70: 7461 3d62 2764 6174 6135 272c 0a29 0a65  ta=b'data5',.).e
-00006f80: 7665 6e74 3620 3d20 4e65 7745 7665 6e74  vent6 = NewEvent
-00006f90: 280a 2020 2020 7479 7065 3d27 4f72 6465  (.    type='Orde
-00006fa0: 7244 656c 6574 6564 272c 0a20 2020 2064  rDeleted',.    d
-00006fb0: 6174 613d 6227 6461 7461 3627 2c0a 290a  ata=b'data6',.).
-00006fc0: 636c 6965 6e74 2e61 7070 656e 645f 6576  client.append_ev
-00006fd0: 656e 7473 280a 2020 2020 7374 7265 616d  ents(.    stream
-00006fe0: 5f6e 616d 653d 7374 7265 616d 5f6e 616d  _name=stream_nam
-00006ff0: 6532 2c0a 2020 2020 6578 7065 6374 6564  e2,.    expected
-00007000: 5f70 6f73 6974 696f 6e3d 4e6f 6e65 2c0a  _position=None,.
-00007010: 2020 2020 6576 656e 7473 3d5b 6576 656e      events=[even
-00007020: 7434 2c20 6576 656e 7435 2c20 6576 656e  t4, event5, even
-00007030: 7436 5d2c 0a29 0a0a 2320 5375 6273 6372  t6],.)..# Subscr
-00007040: 6962 6520 6672 6f6d 2074 6865 2063 6f6d  ibe from the com
-00007050: 6d69 7420 706f 7369 7469 6f6e 2e0a 7375  mit position..su
-00007060: 6273 6372 6970 7469 6f6e 203d 2063 6c69  bscription = cli
-00007070: 656e 742e 7375 6273 6372 6962 655f 616c  ent.subscribe_al
-00007080: 6c5f 6576 656e 7473 280a 2020 2020 636f  l_events(.    co
-00007090: 6d6d 6974 5f70 6f73 6974 696f 6e3d 636f  mmit_position=co
-000070a0: 6d6d 6974 5f70 6f73 6974 696f 6e0a 290a  mmit_position.).
-000070b0: 0a23 2043 6174 6368 2075 7020 6279 2072  .# Catch up by r
-000070c0: 6563 6569 7669 6e67 2074 6865 2074 6872  eceiving the thr
-000070d0: 6565 2065 7665 6e74 7320 6672 6f6d 2074  ee events from t
-000070e0: 6865 2073 7562 7363 7269 7074 696f 6e2e  he subscription.
-000070f0: 0a65 7665 6e74 7320 3d20 5b5d 0a66 6f72  .events = [].for
-00007100: 2065 7665 6e74 2069 6e20 7375 6273 6372   event in subscr
-00007110: 6970 7469 6f6e 3a0a 2020 2020 6576 656e  iption:.    even
-00007120: 7473 2e61 7070 656e 6428 6576 656e 7429  ts.append(event)
-00007130: 0a20 2020 2069 6620 6576 656e 742e 6461  .    if event.da
-00007140: 7461 203d 3d20 6576 656e 7436 2e64 6174  ta == event6.dat
-00007150: 6120 616e 6420 6576 656e 742e 7374 7265  a and event.stre
-00007160: 616d 5f6e 616d 653a 0a20 2020 2020 2020  am_name:.       
-00007170: 2062 7265 616b 0a0a 6173 7365 7274 2065   break..assert e
-00007180: 7665 6e74 735b 305d 2e64 6174 6120 3d3d  vents[0].data ==
-00007190: 2065 7665 6e74 342e 6461 7461 0a61 7373   event4.data.ass
-000071a0: 6572 7420 6576 656e 7473 5b31 5d2e 6461  ert events[1].da
-000071b0: 7461 203d 3d20 6576 656e 7435 2e64 6174  ta == event5.dat
-000071c0: 610a 6173 7365 7274 2065 7665 6e74 735b  a.assert events[
-000071d0: 325d 2e64 6174 6120 3d3d 2065 7665 6e74  2].data == event
-000071e0: 362e 6461 7461 0a0a 0a23 2041 7070 656e  6.data...# Appen
-000071f0: 6420 7468 7265 6520 6d6f 7265 2065 7665  d three more eve
-00007200: 6e74 732e 0a73 7472 6561 6d5f 6e61 6d65  nts..stream_name
-00007210: 3320 3d20 7374 7228 7575 6964 3428 2929  3 = str(uuid4())
-00007220: 0a65 7665 6e74 3720 3d20 4e65 7745 7665  .event7 = NewEve
-00007230: 6e74 280a 2020 2020 7479 7065 3d27 4f72  nt(.    type='Or
-00007240: 6465 7243 7265 6174 6564 272c 0a20 2020  derCreated',.   
-00007250: 2064 6174 613d 6227 6461 7461 3727 2c0a   data=b'data7',.
-00007260: 290a 6576 656e 7438 203d 204e 6577 4576  ).event8 = NewEv
-00007270: 656e 7428 0a20 2020 2074 7970 653d 274f  ent(.    type='O
-00007280: 7264 6572 5570 6461 7465 6427 2c0a 2020  rderUpdated',.  
-00007290: 2020 6461 7461 3d62 2764 6174 6138 272c    data=b'data8',
-000072a0: 0a29 0a65 7665 6e74 3920 3d20 4e65 7745  .).event9 = NewE
-000072b0: 7665 6e74 280a 2020 2020 7479 7065 3d27  vent(.    type='
-000072c0: 4f72 6465 7244 656c 6574 6564 272c 0a20  OrderDeleted',. 
-000072d0: 2020 2064 6174 613d 6227 6461 7461 3927     data=b'data9'
-000072e0: 2c0a 290a 0a63 6c69 656e 742e 6170 7065  ,.)..client.appe
-000072f0: 6e64 5f65 7665 6e74 7328 0a20 2020 2073  nd_events(.    s
-00007300: 7472 6561 6d5f 6e61 6d65 3d73 7472 6561  tream_name=strea
-00007310: 6d5f 6e61 6d65 332c 0a20 2020 2065 7870  m_name3,.    exp
-00007320: 6563 7465 645f 706f 7369 7469 6f6e 3d4e  ected_position=N
-00007330: 6f6e 652c 0a20 2020 2065 7665 6e74 733d  one,.    events=
-00007340: 5b65 7665 6e74 372c 2065 7665 6e74 382c  [event7, event8,
-00007350: 2065 7665 6e74 395d 2c0a 290a 0a23 2052   event9],.)..# R
-00007360: 6563 6569 7665 2074 6865 2074 6872 6565  eceive the three
-00007370: 206e 6577 2065 7665 6e74 7320 6672 6f6d   new events from
-00007380: 2074 6865 2073 616d 6520 7375 6273 6372   the same subscr
-00007390: 6970 7469 6f6e 2e0a 666f 7220 6576 656e  iption..for even
-000073a0: 7420 696e 2073 7562 7363 7269 7074 696f  t in subscriptio
-000073b0: 6e3a 0a20 2020 2023 2043 6865 636b 2074  n:.    # Check t
-000073c0: 6865 2073 7472 6561 6d20 6e61 6d65 2e0a  he stream name..
-000073d0: 2020 2020 6576 656e 7473 2e61 7070 656e      events.appen
-000073e0: 6428 6576 656e 7429 0a20 2020 2069 6620  d(event).    if 
-000073f0: 6576 656e 742e 7374 7265 616d 5f6e 616d  event.stream_nam
-00007400: 6520 3d3d 2073 7472 6561 6d5f 6e61 6d65  e == stream_name
-00007410: 333a 0a20 2020 2020 2020 2069 6620 6576  3:.        if ev
-00007420: 656e 742e 6461 7461 203d 3d20 6576 656e  ent.data == even
-00007430: 7439 2e64 6174 613a 0a20 2020 2020 2020  t9.data:.       
-00007440: 2020 2020 2062 7265 616b 0a0a 6173 7365       break..asse
-00007450: 7274 2065 7665 6e74 735b 335d 2e64 6174  rt events[3].dat
-00007460: 6120 3d3d 2065 7665 6e74 372e 6461 7461  a == event7.data
-00007470: 0a61 7373 6572 7420 6576 656e 7473 5b34  .assert events[4
-00007480: 5d2e 6461 7461 203d 3d20 6576 656e 7438  ].data == event8
-00007490: 2e64 6174 610a 6173 7365 7274 2065 7665  .data.assert eve
-000074a0: 6e74 735b 355d 2e64 6174 6120 3d3d 2065  nts[5].data == e
-000074b0: 7665 6e74 392e 6461 7461 0a60 6060 0a0a  vent9.data.```..
-000074c0: 4361 7463 682d 7570 2073 7562 7363 7269  Catch-up subscri
-000074d0: 7074 696f 6e73 2061 7265 206e 6f74 2072  ptions are not r
-000074e0: 6567 6973 7465 7265 6420 696e 2045 7665  egistered in Eve
-000074f0: 6e74 5374 6f72 6544 4220 2874 6865 7920  ntStoreDB (they 
-00007500: 6172 6520 6e6f 740a 2270 6572 7369 7374  are not."persist
-00007510: 656e 7422 2073 7562 7363 7269 7074 696f  ent" subscriptio
-00007520: 6e73 292e 2049 7420 6973 2073 696d 706c  ns). It is simpl
-00007530: 7920 6120 7374 7265 616d 696e 6720 6752  y a streaming gR
-00007540: 5043 2063 616c 6c20 7768 6963 6820 6973  PC call which is
-00007550: 0a6b 6570 7420 6f70 656e 2062 7920 7468  .kept open by th
-00007560: 6520 7365 7276 6572 2c20 7769 7468 206e  e server, with n
-00007570: 6577 6c79 2072 6563 6f72 6465 6420 6576  ewly recorded ev
-00007580: 656e 7473 2073 656e 7420 746f 2074 6865  ents sent to the
-00007590: 2063 6c69 656e 740a 6173 2074 6865 2063   client.as the c
-000075a0: 6c69 656e 7420 6974 6572 6174 6573 206f  lient iterates o
-000075b0: 7665 7220 7468 6520 7375 6273 6372 6970  ver the subscrip
-000075c0: 7469 6f6e 2e20 5468 6973 206b 696e 6420  tion. This kind 
-000075d0: 6f66 2073 7562 7363 7269 7074 696f 6e0a  of subscription.
-000075e0: 6973 2063 6c6f 7365 6420 6173 2073 6f6f  is closed as soo
-000075f0: 6e20 6173 2074 6865 2073 7562 7363 7269  n as the subscri
-00007600: 7074 696f 6e20 6f62 6a65 6374 2067 6f65  ption object goe
-00007610: 7320 6f75 7420 6f66 206d 656d 6f72 792e  s out of memory.
-00007620: 0a0a 6060 6070 7974 686f 6e0a 2320 456e  ..```python.# En
-00007630: 6420 7468 6520 7375 6273 6372 6970 7469  d the subscripti
-00007640: 6f6e 2e0a 6465 6c20 7375 6273 6372 6970  on..del subscrip
-00007650: 7469 6f6e 0a60 6060 0a0a 506c 6561 7365  tion.```..Please
-00007660: 206e 6f74 652c 2077 6865 6e20 7072 6f63   note, when proc
-00007670: 6573 7369 6e67 2065 7665 6e74 7320 696e  essing events in
-00007680: 2061 2064 6f77 6e73 7472 6561 6d20 636f   a downstream co
-00007690: 6d70 6f6e 656e 742c 2074 6865 2063 6f6d  mponent, the com
-000076a0: 6d69 7420 706f 7369 7469 6f6e 206f 660a  mit position of.
-000076b0: 7468 6520 6c61 7374 2073 7563 6365 7373  the last success
-000076c0: 6675 6c6c 7920 7072 6f63 6573 7365 6420  fully processed 
-000076d0: 6576 656e 7420 6973 2075 7365 6675 6c6c  event is usefull
-000076e0: 7920 7265 636f 7264 6564 2062 7920 7468  y recorded by th
-000076f0: 6520 646f 776e 7374 7265 616d 2063 6f6d  e downstream com
-00007700: 706f 6e65 6e74 0a73 6f20 7468 6174 2074  ponent.so that t
-00007710: 6865 2063 6f6d 6d69 7420 706f 7369 7469  he commit positi
-00007720: 6f6e 2063 616e 2062 6520 6465 7465 726d  on can be determ
-00007730: 696e 6564 2062 7920 7468 6520 646f 776e  ined by the down
-00007740: 7374 7265 616d 2063 6f6d 706f 6e65 6e74  stream component
-00007750: 2066 726f 6d20 6974 7320 6f77 6e0a 7265   from its own.re
-00007760: 636f 7264 6564 2077 6865 6e20 6974 2069  corded when it i
-00007770: 7320 7265 7374 6172 7465 642e 2054 6869  s restarted. Thi
-00007780: 7320 636f 6d6d 6974 2070 6f73 6974 696f  s commit positio
-00007790: 6e20 6361 6e20 6265 2075 7365 6420 746f  n can be used to
-000077a0: 2073 7065 6369 6679 2074 6865 2063 6f6d   specify the com
-000077b0: 6d69 740a 706f 7369 7469 6f6e 2066 726f  mit.position fro
-000077c0: 6d20 7768 6963 6820 746f 2073 7562 7363  m which to subsc
-000077d0: 7269 6265 2e20 5369 6e63 6520 7468 6973  ribe. Since this
-000077e0: 2063 6f6d 6d69 7420 706f 7369 7469 6f6e   commit position
-000077f0: 2072 6570 7265 7365 6e74 7320 7468 6520   represents the 
-00007800: 706f 7369 7469 6f6e 206f 660a 7468 6520  position of.the 
-00007810: 6c61 7374 2073 7563 6365 7373 6675 6c6c  last successfull
-00007820: 7920 7072 6f63 6573 7365 6420 6576 656e  y processed even
-00007830: 7420 696e 2061 2064 6f77 6e73 7472 6561  t in a downstrea
-00007840: 6d20 636f 6d70 6f6e 656e 742c 2073 6f20  m component, so 
-00007850: 6974 2077 696c 6c20 6265 2075 7375 616c  it will be usual
-00007860: 2074 6f0a 7761 6e74 2074 6865 206e 6578   to.want the nex
-00007870: 7420 6576 656e 7420 6166 7465 7220 7468  t event after th
-00007880: 6973 2070 6f73 6974 696f 6e2c 2062 6563  is position, bec
-00007890: 6175 7365 2074 6861 7420 6973 2074 6865  ause that is the
-000078a0: 206e 6578 7420 6576 656e 7420 7468 6174   next event that
-000078b0: 206e 6565 6473 2074 6f0a 6265 2070 726f   needs to.be pro
-000078c0: 6365 7373 6564 2e20 5768 656e 2073 7562  cessed. When sub
-000078d0: 7363 7269 6269 6e67 2066 6f72 2065 7665  scribing for eve
-000078e0: 6e74 7320 7573 696e 6720 6120 6361 7463  nts using a catc
-000078f0: 6875 702d 7375 6273 6372 6970 7469 6f6e  hup-subscription
-00007900: 0a69 6e20 4576 656e 7453 746f 7265 4442  .in EventStoreDB
-00007910: 2c20 7468 6520 6576 656e 7420 6174 2074  , the event at t
-00007920: 6865 2073 7065 6369 6669 6564 2063 6f6d  he specified com
-00007930: 6d69 7420 706f 7369 7469 6f6e 2077 696c  mit position wil
-00007940: 6c20 4e4f 5420 6265 2069 6e63 6c75 6465  l NOT be include
-00007950: 6420 696e 0a74 6865 2073 6571 7565 6e63  d in.the sequenc
-00007960: 6520 6f66 2072 6563 6f72 6465 6420 6576  e of recorded ev
-00007970: 656e 7473 2e0a 0a54 6f20 6163 636f 6d70  ents...To accomp
-00007980: 6c69 7368 2022 6578 6163 746c 7920 6f6e  lish "exactly on
-00007990: 6365 2220 7072 6f63 6573 7369 6e67 206f  ce" processing o
-000079a0: 6620 7468 6520 6576 656e 7473 2c20 7468  f the events, th
-000079b0: 6520 636f 6d6d 6974 2070 6f73 6974 696f  e commit positio
-000079c0: 6e0a 6f66 2061 2072 6563 6f72 6465 6420  n.of a recorded 
-000079d0: 6576 656e 7420 7368 6f75 6c64 2062 6520  event should be 
-000079e0: 7265 636f 7264 6564 2061 746f 6d69 6361  recorded atomica
-000079f0: 6c6c 7920 616e 6420 756e 6971 7565 6c79  lly and uniquely
-00007a00: 2061 6c6f 6e67 2077 6974 680a 7468 6520   along with.the 
-00007a10: 7265 7375 6c74 206f 6620 7072 6f63 6573  result of proces
-00007a20: 7369 6e67 2072 6563 6f72 6465 6420 6576  sing recorded ev
-00007a30: 656e 7473 2c20 666f 7220 6578 616d 706c  ents, for exampl
-00007a40: 6520 696e 2074 6865 2073 616d 6520 6461  e in the same da
-00007a50: 7461 6261 7365 0a61 7320 6d61 7465 7269  tabase.as materi
-00007a60: 616c 6973 6564 2076 6965 7773 2077 6865  alised views whe
-00007a70: 6e20 696d 706c 656d 656e 7469 6e67 2065  n implementing e
-00007a80: 7665 6e74 7561 6c6c 792d 636f 6e73 6973  ventually-consis
-00007a90: 7465 6e74 2043 5152 532c 206f 7220 696e  tent CQRS, or in
-00007aa0: 0a74 6865 2073 616d 6520 6461 7461 6261  .the same databa
-00007ab0: 7365 2061 7320 6120 646f 776e 7374 7265  se as a downstre
-00007ac0: 616d 2061 6e61 6c79 7469 6373 206f 7220  am analytics or 
-00007ad0: 7265 706f 7274 696e 6720 6f72 2061 7263  reporting or arc
-00007ae0: 6869 7669 6e67 0a61 7070 6c69 6361 7469  hiving.applicati
-00007af0: 6f6e 2e20 5468 6973 2061 766f 6964 7320  on. This avoids 
-00007b00: 2264 7561 6c20 7772 6974 696e 6722 2069  "dual writing" i
-00007b10: 6e20 7468 6520 7072 6f63 6573 7369 6e67  n the processing
-00007b20: 206f 6620 6576 656e 7473 2e0a 0a52 6563   of events...Rec
-00007b30: 6f72 6465 6420 6576 656e 7473 2072 6563  orded events rec
-00007b40: 6569 7665 6420 6672 6f6d 2061 2063 6174  eived from a cat
-00007b50: 6368 2d75 7020 7375 6273 6372 6970 7469  ch-up subscripti
-00007b60: 6f6e 2063 616e 6e6f 7420 6265 2061 636b  on cannot be ack
-00007b70: 6e6f 776c 6564 6765 6420 6261 636b 0a74  nowledged back.t
-00007b80: 6f20 7468 6520 4576 656e 7453 746f 7265  o the EventStore
-00007b90: 4442 2073 6572 7665 7220 2874 6865 7265  DB server (there
-00007ba0: 2069 7320 6e6f 206e 6565 6420 746f 2064   is no need to d
-00007bb0: 6f20 7468 6973 292e 2041 636b 6e6f 776c  o this). Acknowl
-00007bc0: 6564 6769 6e67 2065 7665 6e74 7320 6973  edging events is
-00007bd0: 0a61 6e20 6173 7065 6374 206f 6620 2270  .an aspect of "p
-00007be0: 6572 7369 7374 656e 7420 7375 6273 6372  ersistent subscr
-00007bf0: 6970 7469 6f6e 7322 2028 7365 6520 6265  iptions" (see be
-00007c00: 6c6f 7729 2e0a 0a54 6865 2073 7562 7363  low)...The subsc
-00007c10: 7269 7074 696f 6e20 6f62 6a65 6374 206d  ription object m
-00007c20: 6967 6874 2062 6520 7573 6564 2064 6972  ight be used dir
-00007c30: 6563 746c 7920 7768 656e 2070 726f 6365  ectly when proce
-00007c40: 7373 696e 6720 6576 656e 7473 2e20 4974  ssing events. It
-00007c50: 206d 6967 6874 0a61 6c73 6f20 6265 2075   might.also be u
-00007c60: 7365 6420 7769 7468 696e 2061 2074 6872  sed within a thr
-00007c70: 6561 6420 6465 6469 6361 7465 6420 746f  ead dedicated to
-00007c80: 2072 6563 6569 7669 6e67 2065 7665 6e74   receiving event
-00007c90: 732c 2077 6974 6820 7265 636f 7264 6564  s, with recorded
-00007ca0: 2065 7665 6e74 730a 7075 7420 6f6e 2061   events.put on a
-00007cb0: 2071 7565 7565 2066 6f72 2070 726f 6365   queue for proce
-00007cc0: 7373 696e 6720 696e 2061 2064 6966 6665  ssing in a diffe
-00007cd0: 7265 6e74 2074 6872 6561 642e 2054 6869  rent thread. Thi
-00007ce0: 7320 7061 636b 6167 6520 646f 6573 6e27  s package doesn'
-00007cf0: 7420 7072 6f76 6964 650a 7375 6368 2074  t provide.such t
-00007d00: 6872 6561 6420 6f72 2071 7565 7565 206f  hread or queue o
-00007d10: 626a 6563 7473 2c20 796f 7520 776f 756c  bjects, you woul
-00007d20: 6420 6e65 6564 2074 6f20 646f 2074 6861  d need to do tha
-00007d30: 7420 796f 7572 7365 6c66 2e20 4a75 7374  t yourself. Just
-00007d40: 206d 616b 6520 7375 7265 0a74 6f20 7265   make sure.to re
-00007d50: 636f 6e73 7472 7563 7420 7468 6520 7375  construct the su
-00007d60: 6273 6372 6970 7469 6f6e 2028 616e 6420  bscription (and 
-00007d70: 7468 6520 7175 6575 6529 2075 7369 6e67  the queue) using
-00007d80: 2079 6f75 7220 6c61 7374 2072 6563 6f72   your last recor
-00007d90: 6465 6420 636f 6d6d 6974 0a70 6f73 6974  ded commit.posit
-00007da0: 696f 6e20 7768 656e 2072 6573 756d 696e  ion when resumin
-00007db0: 6720 7468 6520 7375 6273 6372 6970 7469  g the subscripti
-00007dc0: 6f6e 2061 6674 6572 2061 6e20 6572 726f  on after an erro
-00007dd0: 722c 2074 6f20 6265 2073 7572 6520 616c  r, to be sure al
-00007de0: 6c20 6576 656e 7473 0a61 7265 2070 726f  l events.are pro
-00007df0: 6365 7373 6564 206f 6e63 652e 0a0a 2323  cessed once...##
-00007e00: 2320 5065 7273 6973 7465 6e74 2073 7562  # Persistent sub
-00007e10: 7363 7269 7074 696f 6e73 0a0a 5468 6520  scriptions..The 
-00007e20: 6d65 7468 6f64 2060 6372 6561 7465 5f73  method `create_s
-00007e30: 7562 7363 7269 7074 696f 6e28 2960 2063  ubscription()` c
-00007e40: 616e 2062 6520 7573 6564 2074 6f20 6372  an be used to cr
-00007e50: 6561 7465 2061 0a22 7065 7273 6973 7465  eate a."persiste
-00007e60: 6e74 2073 7562 7363 7269 7074 696f 6e22  nt subscription"
-00007e70: 2074 6f20 4576 656e 7453 746f 7265 4442   to EventStoreDB
-00007e80: 2e0a 0a54 6869 7320 6d65 7468 6f64 2074  ...This method t
-00007e90: 616b 6573 2061 2072 6571 7569 7265 6420  akes a required 
-00007ea0: 6067 726f 7570 5f6e 616d 6560 2061 7267  `group_name` arg
-00007eb0: 756d 656e 742c 2077 6869 6368 2069 7320  ument, which is 
-00007ec0: 7468 650a 6e61 6d65 206f 6620 6120 2267  the.name of a "g
-00007ed0: 726f 7570 2220 6f66 2063 6f6e 7375 6d65  roup" of consume
-00007ee0: 7273 206f 6620 7468 6520 7375 6273 6372  rs of the subscr
-00007ef0: 6970 7469 6f6e 2e0a 0a54 6869 7320 6d65  iption...This me
-00007f00: 7468 6f64 2074 616b 6573 2061 6e20 6f70  thod takes an op
-00007f10: 7469 6f6e 616c 2060 6672 6f6d 5f65 6e64  tional `from_end
-00007f20: 6020 6172 6775 6d65 6e74 2c20 7768 6963  ` argument, whic
-00007f30: 6820 6361 6e20 6265 0a75 7365 6420 746f  h can be.used to
-00007f40: 2073 7065 6369 6679 2074 6861 7420 7468   specify that th
-00007f50: 6520 6772 6f75 7020 6f66 2063 6f6e 7375  e group of consu
-00007f60: 6d65 7273 206f 6620 7468 6520 7375 6273  mers of the subs
-00007f70: 6372 6970 7469 6f6e 2073 686f 756c 640a  cription should.
-00007f80: 6f6e 6c79 2072 6563 6569 7665 2065 7665  only receive eve
-00007f90: 6e74 7320 7468 6174 2077 6572 6520 7265  nts that were re
-00007fa0: 636f 7264 6564 2061 6674 6572 2074 6865  corded after the
-00007fb0: 2073 7562 7363 7269 7074 696f 6e20 7761   subscription wa
-00007fc0: 7320 6372 6561 7465 642e 0a0a 5468 6973  s created...This
-00007fd0: 206d 6574 686f 6420 7461 6b65 7320 616e   method takes an
-00007fe0: 206f 7074 696f 6e61 6c20 6063 6f6d 6d69   optional `commi
-00007ff0: 745f 706f 7369 7469 6f6e 6020 6172 6775  t_position` argu
-00008000: 6d65 6e74 2c20 7768 6963 6820 6361 6e20  ment, which can 
-00008010: 6265 0a75 7365 6420 746f 2073 7065 6369  be.used to speci
-00008020: 6679 2061 2063 6f6d 6d69 7420 706f 7369  fy a commit posi
-00008030: 7469 6f6e 2066 726f 6d20 7768 6963 6820  tion from which 
-00008040: 7468 6520 6772 6f75 7020 6f66 2063 6f6e  the group of con
-00008050: 7375 6d65 7273 206f 660a 7468 6520 7375  sumers of.the su
-00008060: 6273 6372 6970 7469 6f6e 2073 686f 756c  bscription shoul
-00008070: 6420 7265 6365 6976 6520 6576 656e 7473  d receive events
-00008080: 2e20 506c 6561 7365 206e 6f74 652c 2074  . Please note, t
-00008090: 6865 2072 6563 6f72 6465 6420 6576 656e  he recorded even
-000080a0: 740a 6174 2074 6865 2073 7065 6369 6669  t.at the specifi
-000080b0: 6564 2063 6f6d 6d69 7420 706f 7369 7469  ed commit positi
-000080c0: 6f6e 204d 4159 2062 6520 696e 636c 7564  on MAY be includ
-000080d0: 6564 2069 6e20 7468 6520 7265 636f 7264  ed in the record
-000080e0: 6564 2065 7665 6e74 730a 7265 6365 6976  ed events.receiv
-000080f0: 6564 2062 7920 7468 6520 6772 6f75 7020  ed by the group 
-00008100: 6f66 2063 6f6e 7375 6d65 7273 2e0a 0a49  of consumers...I
-00008110: 6620 6e65 6974 6865 7220 6066 726f 6d5f  f neither `from_
-00008120: 656e 6460 206f 7220 6070 6f73 6974 696f  end` or `positio
-00008130: 6e60 2061 7265 2073 7065 6369 6669 6564  n` are specified
-00008140: 2c20 7468 6520 6772 6f75 7020 6f66 2063  , the group of c
-00008150: 6f6e 7375 6d65 7273 0a6f 6620 7468 6520  onsumers.of the 
-00008160: 7375 6273 6372 6970 7469 6f6e 2077 696c  subscription wil
-00008170: 6c20 7265 6365 6976 6520 616c 6c20 7265  l receive all re
-00008180: 636f 7264 6564 2065 7665 6e74 732e 0a0a  corded events...
-00008190: 5468 6973 206d 6574 686f 6420 616c 736f  This method also
-000081a0: 2074 616b 6573 206f 7074 696f 6e20 6066   takes option `f
-000081b0: 696c 7465 725f 6578 636c 7564 6560 2c20  ilter_exclude`, 
-000081c0: 6066 696c 7465 725f 696e 636c 7564 6560  `filter_include`
-000081d0: 0a61 7267 756d 656e 7473 2c20 7768 6963  .arguments, whic
-000081e0: 6820 776f 726b 2069 6e20 7468 6520 7361  h work in the sa
-000081f0: 6d65 2077 6179 2061 7320 7468 6579 2064  me way as they d
-00008200: 6f20 696e 2074 6865 2060 7375 6273 6372  o in the `subscr
-00008210: 6962 655f 616c 6c5f 6576 656e 7473 2829  ibe_all_events()
-00008220: 600a 6d65 7468 6f64 2e0a 0a54 6869 7320  `.method...This 
-00008230: 6d65 7468 6f64 2061 6c73 6f20 7461 6b65  method also take
-00008240: 7320 616e 206f 7074 696f 6e61 6c20 6074  s an optional `t
-00008250: 696d 656f 7574 6020 6172 6775 6d65 6e74  imeout` argument
-00008260: 2c20 7468 6174 0a69 7320 6578 7065 6374  , that.is expect
-00008270: 6564 2074 6f20 6265 2061 2050 7974 686f  ed to be a Pytho
-00008280: 6e20 6066 6c6f 6174 602c 2077 6869 6368  n `float`, which
-00008290: 2073 6574 7320 6120 6465 6164 6c69 6e65   sets a deadline
-000082a0: 0a66 6f72 2074 6865 2063 6f6d 706c 6574  .for the complet
-000082b0: 696f 6e20 6f66 2074 6865 2067 5250 4320  ion of the gRPC 
-000082c0: 6f70 6572 6174 696f 6e2e 0a0a 5468 6520  operation...The 
-000082d0: 6d65 7468 6f64 2060 6372 6561 7465 5f73  method `create_s
-000082e0: 7562 7363 7269 7074 696f 6e28 2960 2064  ubscription()` d
-000082f0: 6f65 7320 6e6f 7420 7265 7475 726e 2061  oes not return a
-00008300: 2076 616c 7565 2c20 6265 6361 7573 650a   value, because.
-00008310: 7265 636f 7264 6564 2065 7665 6e74 7320  recorded events 
-00008320: 6172 6520 6f62 7461 696e 6564 2062 7920  are obtained by 
-00008330: 7468 6520 6772 6f75 7020 6f66 2063 6f6e  the group of con
-00008340: 7375 6d65 7273 206f 6620 7468 6520 7375  sumers of the su
-00008350: 6273 6372 6970 7469 6f6e 0a75 7369 6e67  bscription.using
-00008360: 2074 6865 2060 7265 6164 5f73 7562 7363   the `read_subsc
-00008370: 7269 7074 696f 6e28 2960 206d 6574 686f  ription()` metho
-00008380: 642e 0a0a 496e 2074 6865 2065 7861 6d70  d...In the examp
-00008390: 6c65 2062 656c 6f77 2c20 6120 7065 7273  le below, a pers
-000083a0: 6973 7465 6e74 2073 7562 7363 7269 7074  istent subscript
-000083b0: 696f 6e20 6973 2063 7265 6174 6564 2e0a  ion is created..
-000083c0: 0a60 6060 7079 7468 6f6e 0a23 2043 7265  .```python.# Cre
-000083d0: 6174 6520 6120 7065 7273 6973 7465 6e74  ate a persistent
-000083e0: 2073 7562 7363 7269 7074 696f 6e2e 0a67   subscription..g
-000083f0: 726f 7570 5f6e 616d 6520 3d20 6622 6772  roup_name = f"gr
-00008400: 6f75 702d 7b75 7569 6434 2829 7d22 0a63  oup-{uuid4()}".c
-00008410: 6c69 656e 742e 6372 6561 7465 5f73 7562  lient.create_sub
-00008420: 7363 7269 7074 696f 6e28 6772 6f75 705f  scription(group_
-00008430: 6e61 6d65 3d67 726f 7570 5f6e 616d 6529  name=group_name)
-00008440: 0a60 6060 0a0a 5468 6520 6d65 7468 6f64  .```..The method
-00008450: 2060 7265 6164 5f73 7562 7363 7269 7074   `read_subscript
-00008460: 696f 6e28 2960 2063 616e 2062 6520 7573  ion()` can be us
-00008470: 6564 2062 7920 6120 6772 6f75 7020 6f66  ed by a group of
-00008480: 2063 6f6e 7375 6d65 7273 2074 6f20 7265   consumers to re
-00008490: 6365 6976 650a 7265 636f 7264 6564 2065  ceive.recorded e
-000084a0: 7665 6e74 7320 6672 6f6d 2061 2070 6572  vents from a per
-000084b0: 7369 7374 656e 7420 7375 6273 6372 6970  sistent subscrip
-000084c0: 7469 6f6e 2063 7265 6174 6564 2075 7369  tion created usi
-000084d0: 6e67 2060 6372 6561 7465 5f73 7562 7363  ng `create_subsc
-000084e0: 7269 7074 696f 6e60 2e0a 0a54 6869 7320  ription`...This 
-000084f0: 6d65 7468 6f64 2074 616b 6573 2061 2072  method takes a r
-00008500: 6571 7569 7265 6420 6067 726f 7570 5f6e  equired `group_n
-00008510: 616d 6560 2061 7267 756d 656e 742c 2077  ame` argument, w
-00008520: 6869 6368 2069 730a 7468 6520 6e61 6d65  hich is.the name
-00008530: 206f 6620 6120 2267 726f 7570 2220 6f66   of a "group" of
-00008540: 2063 6f6e 7375 6d65 7273 206f 6620 7468   consumers of th
-00008550: 6520 7375 6273 6372 6970 7469 6f6e 2073  e subscription s
-00008560: 7065 6369 6669 6564 0a77 6865 6e20 6063  pecified.when `c
-00008570: 7265 6174 655f 7375 6273 6372 6970 7469  reate_subscripti
-00008580: 6f6e 2829 6020 7761 7320 6361 6c6c 6564  on()` was called
-00008590: 2e0a 0a54 6869 7320 6d65 7468 6f64 2061  ...This method a
-000085a0: 6c73 6f20 7461 6b65 7320 616e 206f 7074  lso takes an opt
-000085b0: 696f 6e61 6c20 6074 696d 656f 7574 6020  ional `timeout` 
-000085c0: 6172 6775 6d65 6e74 2c20 7468 6174 0a69  argument, that.i
-000085d0: 7320 6578 7065 6374 6564 2074 6f20 6265  s expected to be
-000085e0: 2061 2050 7974 686f 6e20 6066 6c6f 6174   a Python `float
-000085f0: 602c 2077 6869 6368 2073 6574 7320 6120  `, which sets a 
-00008600: 6465 6164 6c69 6e65 0a66 6f72 2074 6865  deadline.for the
-00008610: 2063 6f6d 706c 6574 696f 6e20 6f66 2074   completion of t
-00008620: 6865 2067 5250 4320 6f70 6572 6174 696f  he gRPC operatio
-00008630: 6e2e 0a0a 5468 6973 206d 6574 686f 6420  n...This method 
-00008640: 7265 7475 726e 7320 6120 322d 7475 706c  returns a 2-tupl
-00008650: 653a 2061 2022 7265 6164 2072 6571 7565  e: a "read reque
-00008660: 7374 2220 6f62 6a65 6374 2061 6e64 2061  st" object and a
-00008670: 2022 7265 6164 2072 6573 706f 6e73 6522   "read response"
-00008680: 206f 626a 6563 742e 0a0a 6060 6070 7974   object...```pyt
-00008690: 686f 6e0a 7265 6164 5f72 6571 2c20 7265  hon.read_req, re
-000086a0: 6164 5f72 6573 7020 3d20 636c 6965 6e74  ad_resp = client
-000086b0: 2e72 6561 645f 7375 6273 6372 6970 7469  .read_subscripti
-000086c0: 6f6e 2867 726f 7570 5f6e 616d 653d 6772  on(group_name=gr
-000086d0: 6f75 705f 6e61 6d65 290a 6060 600a 0a54  oup_name).```..T
-000086e0: 6865 2022 7265 6164 2072 6573 706f 6e73  he "read respons
-000086f0: 6522 206f 626a 6563 7420 6973 2061 6e20  e" object is an 
-00008700: 6974 6572 6174 6f72 2074 6861 7420 7969  iterator that yi
-00008710: 656c 6473 2072 6563 6f72 6465 6420 6576  elds recorded ev
-00008720: 656e 7473 2066 726f 6d0a 7468 6520 7370  ents from.the sp
-00008730: 6563 6966 6965 6420 636f 6d6d 6974 2070  ecified commit p
-00008740: 6f73 6974 696f 6e2e 0a0a 5468 6520 2272  osition...The "r
-00008750: 6561 6420 7265 7175 6573 7422 206f 626a  ead request" obj
-00008760: 6563 7420 6861 7320 616e 2060 6163 6b28  ect has an `ack(
-00008770: 2960 206d 6574 686f 6420 7468 6174 2063  )` method that c
-00008780: 616e 2062 6520 7573 6564 2062 7920 6120  an be used by a 
-00008790: 636f 6e73 756d 6572 0a69 6e20 6120 6772  consumer.in a gr
-000087a0: 6f75 7020 746f 2061 636b 6e6f 776c 6564  oup to acknowled
-000087b0: 6765 2074 6f20 7468 6520 7365 7276 6572  ge to the server
-000087c0: 2074 6861 7420 6974 2068 6173 2072 6563   that it has rec
-000087d0: 6569 7665 6420 616e 6420 7375 6363 6573  eived and succes
-000087e0: 7366 756c 6c79 0a70 726f 6365 7373 6564  sfully.processed
-000087f0: 2061 2072 6563 6f72 6465 6420 6576 656e   a recorded even
-00008800: 742e 2054 6869 7320 7769 6c6c 2070 7265  t. This will pre
-00008810: 7665 6e74 2074 6861 7420 7265 636f 7264  vent that record
-00008820: 6564 2065 7665 6e74 2062 6569 6e67 2072  ed event being r
-00008830: 6563 6569 7665 640a 6279 2061 6e6f 7468  eceived.by anoth
-00008840: 6572 2063 6f6e 7375 6d65 7220 696e 2074  er consumer in t
-00008850: 6865 2073 616d 6520 6772 6f75 702e 2054  he same group. T
-00008860: 6865 2060 6163 6b28 2960 206d 6574 686f  he `ack()` metho
-00008870: 6420 7461 6b65 7320 616e 2060 6576 656e  d takes an `even
-00008880: 745f 6964 600a 6172 6775 6d65 6e74 2c20  t_id`.argument, 
-00008890: 7768 6963 6820 6973 2074 6865 2049 4420  which is the ID 
-000088a0: 6f66 2074 6865 2072 6563 6f72 6465 6420  of the recorded 
-000088b0: 6576 656e 7420 7468 6174 2068 6173 2062  event that has b
-000088c0: 6565 6e20 7265 6365 6976 6564 2e0a 0a54  een received...T
-000088d0: 6865 2065 7861 6d70 6c65 2062 656c 6f77  he example below
-000088e0: 2069 7465 7261 7465 7320 6f76 6572 2074   iterates over t
-000088f0: 6865 2022 7265 6164 2072 6573 706f 6e73  he "read respons
-00008900: 6522 206f 626a 6563 742c 2061 6e64 2063  e" object, and c
-00008910: 616c 6c73 2060 6163 6b28 2960 0a6f 6e20  alls `ack()`.on 
-00008920: 7468 6520 2272 6561 6420 7265 7370 6f6e  the "read respon
-00008930: 7365 2220 6f62 6a65 6374 2e20 5468 6520  se" object. The 
-00008940: 666f 7220 6c6f 6f70 2062 7265 616b 7320  for loop breaks 
-00008950: 7768 656e 2077 6520 6861 7665 2072 6563  when we have rec
-00008960: 6569 7665 640a 7468 6520 6c61 7374 2065  eived.the last e
-00008970: 7665 6e74 2c20 736f 2074 6861 7420 7765  vent, so that we
-00008980: 2063 616e 2063 6f6e 7469 6e75 6520 7769   can continue wi
-00008990: 7468 2074 6865 2065 7861 6d70 6c65 7320  th the examples 
-000089a0: 6265 6c6f 772e 0a0a 6060 6070 7974 686f  below...```pytho
-000089b0: 6e0a 6576 656e 7473 203d 205b 5d0a 666f  n.events = [].fo
-000089c0: 7220 6576 656e 7420 696e 2072 6561 645f  r event in read_
-000089d0: 7265 7370 3a0a 2020 2020 6576 656e 7473  resp:.    events
-000089e0: 2e61 7070 656e 6428 6576 656e 7429 0a0a  .append(event)..
-000089f0: 2020 2020 2320 4163 6b6e 6f77 6c65 6467      # Acknowledg
-00008a00: 6520 7468 6520 7265 6365 6976 6564 2065  e the received e
-00008a10: 7665 6e74 2e0a 2020 2020 7265 6164 5f72  vent..    read_r
-00008a20: 6571 2e61 636b 2865 7665 6e74 5f69 643d  eq.ack(event_id=
-00008a30: 6576 656e 742e 6964 290a 0a20 2020 2023  event.id)..    #
-00008a40: 2042 7265 616b 2077 6865 6e20 7468 6520   Break when the 
-00008a50: 6c61 7374 2065 7665 6e74 2068 6173 2062  last event has b
-00008a60: 6565 6e20 7265 6365 6976 6564 2e0a 2020  een received..  
-00008a70: 2020 6966 2065 7665 6e74 2e73 7472 6561    if event.strea
-00008a80: 6d5f 6e61 6d65 203d 3d20 7374 7265 616d  m_name == stream
-00008a90: 5f6e 616d 6533 3a0a 2020 2020 2020 2020  _name3:.        
-00008aa0: 6966 2065 7665 6e74 2e64 6174 6120 3d3d  if event.data ==
-00008ab0: 2065 7665 6e74 392e 6461 7461 3a0a 2020   event9.data:.  
-00008ac0: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-00008ad0: 6060 600a 0a54 6865 2072 6563 6569 7665  ```..The receive
-00008ae0: 6420 6576 656e 7473 2061 7265 2074 6865  d events are the
-00008af0: 2065 7665 6e74 7320 7765 2061 7070 656e   events we appen
-00008b00: 6465 6420 6162 6f76 652e 0a0a 6060 6070  ded above...```p
-00008b10: 7974 686f 6e0a 6173 7365 7274 2065 7665  ython.assert eve
-00008b20: 6e74 735b 2d39 5d2e 6461 7461 203d 3d20  nts[-9].data == 
-00008b30: 6576 656e 7431 2e64 6174 610a 6173 7365  event1.data.asse
-00008b40: 7274 2065 7665 6e74 735b 2d38 5d2e 6461  rt events[-8].da
-00008b50: 7461 203d 3d20 6576 656e 7432 2e64 6174  ta == event2.dat
-00008b60: 610a 6173 7365 7274 2065 7665 6e74 735b  a.assert events[
-00008b70: 2d37 5d2e 6461 7461 203d 3d20 6576 656e  -7].data == even
-00008b80: 7433 2e64 6174 610a 6173 7365 7274 2065  t3.data.assert e
-00008b90: 7665 6e74 735b 2d36 5d2e 6461 7461 203d  vents[-6].data =
-00008ba0: 3d20 6576 656e 7434 2e64 6174 610a 6173  = event4.data.as
-00008bb0: 7365 7274 2065 7665 6e74 735b 2d35 5d2e  sert events[-5].
-00008bc0: 6461 7461 203d 3d20 6576 656e 7435 2e64  data == event5.d
-00008bd0: 6174 610a 6173 7365 7274 2065 7665 6e74  ata.assert event
-00008be0: 735b 2d34 5d2e 6461 7461 203d 3d20 6576  s[-4].data == ev
-00008bf0: 656e 7436 2e64 6174 610a 6173 7365 7274  ent6.data.assert
-00008c00: 2065 7665 6e74 735b 2d33 5d2e 6461 7461   events[-3].data
-00008c10: 203d 3d20 6576 656e 7437 2e64 6174 610a   == event7.data.
-00008c20: 6173 7365 7274 2065 7665 6e74 735b 2d32  assert events[-2
-00008c30: 5d2e 6461 7461 203d 3d20 6576 656e 7438  ].data == event8
-00008c40: 2e64 6174 610a 6173 7365 7274 2065 7665  .data.assert eve
-00008c50: 6e74 735b 2d31 5d2e 6461 7461 203d 3d20  nts[-1].data == 
-00008c60: 6576 656e 7439 2e64 6174 610a 6060 600a  event9.data.```.
-00008c70: 0a54 6865 2022 7265 6164 2072 6571 7565  .The "read reque
-00008c80: 7374 2220 6f62 6a65 6374 2061 6c73 6f20  st" object also 
-00008c90: 6861 7320 616e 2060 6e61 636b 2829 6020  has an `nack()` 
-00008ca0: 6d65 7468 6f64 2074 6861 7420 6361 6e20  method that can 
-00008cb0: 6265 2075 7365 6420 6279 2061 2063 6f6e  be used by a con
-00008cc0: 7375 6d65 720a 696e 2061 2067 726f 7570  sumer.in a group
-00008cd0: 2074 6f20 6163 6b6e 6f77 6c65 6467 6520   to acknowledge 
-00008ce0: 746f 2074 6865 2073 6572 7665 7220 7468  to the server th
-00008cf0: 6174 2069 7420 6861 7320 6661 696c 6564  at it has failed
-00008d00: 2073 7563 6365 7373 6675 6c6c 7920 746f   successfully to
-00008d10: 0a70 726f 6365 7373 2061 2072 6563 6f72  .process a recor
-00008d20: 6465 6420 6576 656e 742e 2054 6869 7320  ded event. This 
-00008d30: 7769 6c6c 2061 6c6c 6f77 2074 6861 7420  will allow that 
-00008d40: 7265 636f 7264 6564 2065 7665 6e74 2074  recorded event t
-00008d50: 6f20 6265 2072 6563 6569 7665 640a 6279  o be received.by
-00008d60: 2074 6869 7320 6f72 2061 6e6f 7468 6572   this or another
-00008d70: 2063 6f6e 7375 6d65 7220 696e 2074 6865   consumer in the
-00008d80: 2073 616d 6520 6772 6f75 702e 0a0a 4974   same group...It
-00008d90: 206d 6967 6874 2062 6520 6d6f 7265 2075   might be more u
-00008da0: 7365 6675 6c20 746f 2065 6e63 6170 7375  seful to encapsu
-00008db0: 6c61 7465 2074 6865 2072 6571 7565 7374  late the request
-00008dc0: 2061 6e64 2072 6573 706f 6e73 6520 6f62   and response ob
-00008dd0: 6a65 6374 7320 616e 6420 746f 2069 7465  jects and to ite
-00008de0: 7261 7465 0a6f 7665 7220 7468 6520 2272  rate.over the "r
-00008df0: 6561 6420 7265 7370 6f6e 7365 2220 696e  ead response" in
-00008e00: 2061 2073 6570 6172 6174 6520 7468 7265   a separate thre
-00008e10: 6164 2c20 746f 2063 616c 6c20 6261 636b  ad, to call back
-00008e20: 2074 6f20 6120 6861 6e64 6c65 7220 6675   to a handler fu
-00008e30: 6e63 7469 6f6e 2077 6865 6e0a 6120 7265  nction when.a re
-00008e40: 636f 7264 6564 2065 7665 6e74 2069 7320  corded event is 
-00008e50: 7265 6365 6976 6564 2c20 616e 6420 6361  received, and ca
-00008e60: 6c6c 2060 6163 6b28 2960 2069 6620 7468  ll `ack()` if th
-00008e70: 6520 6861 6e64 6c65 7220 646f 6573 206e  e handler does n
-00008e80: 6f74 2072 6169 7365 2061 6e0a 6578 6365  ot raise an.exce
-00008e90: 7074 696f 6e2c 2061 6e64 2074 6f20 6361  ption, and to ca
-00008ea0: 6c6c 2060 6e61 636b 2829 6020 6966 2061  ll `nack()` if a
-00008eb0: 6e20 6578 6365 7074 696f 6e20 6973 2072  n exception is r
-00008ec0: 6169 7365 642e 2054 6865 2065 7861 6d70  aised. The examp
-00008ed0: 6c65 2062 656c 6f77 2073 686f 7773 2068  le below shows h
-00008ee0: 6f77 0a74 6869 7320 6d69 6768 7420 6265  ow.this might be
-00008ef0: 2064 6f6e 652e 0a0a 6060 6070 7974 686f   done...```pytho
-00008f00: 6e0a 6672 6f6d 2074 6872 6561 6469 6e67  n.from threading
-00008f10: 2069 6d70 6f72 7420 5468 7265 6164 0a0a   import Thread..
-00008f20: 0a63 6c61 7373 2053 7562 7363 7269 7074  .class Subscript
-00008f30: 696f 6e52 6561 6465 723a 0a20 2020 2064  ionReader:.    d
-00008f40: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00008f50: 2c20 636c 6965 6e74 2c20 6772 6f75 705f  , client, group_
-00008f60: 6e61 6d65 2c20 6361 6c6c 6261 636b 293a  name, callback):
-00008f70: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
-00008f80: 6965 6e74 203d 2063 6c69 656e 740a 2020  ient = client.  
-00008f90: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
-00008fa0: 5f6e 616d 6520 3d20 6772 6f75 705f 6e61  _name = group_na
-00008fb0: 6d65 0a20 2020 2020 2020 2073 656c 662e  me.        self.
-00008fc0: 6361 6c6c 6261 636b 203d 2063 616c 6c62  callback = callb
-00008fd0: 6163 6b0a 2020 2020 2020 2020 7365 6c66  ack.        self
-00008fe0: 2e74 6872 6561 6420 3d20 5468 7265 6164  .thread = Thread
-00008ff0: 2874 6172 6765 743d 7365 6c66 2e72 6561  (target=self.rea
-00009000: 645f 7375 6273 6372 6970 7469 6f6e 2c20  d_subscription, 
-00009010: 6461 656d 6f6e 3d54 7275 6529 0a20 2020  daemon=True).   
-00009020: 2020 2020 2073 656c 662e 6572 726f 7220       self.error 
-00009030: 3d20 4e6f 6e65 0a0a 2020 2020 6465 6620  = None..    def 
-00009040: 7374 6172 7428 7365 6c66 293a 0a20 2020  start(self):.   
-00009050: 2020 2020 2073 656c 662e 7468 7265 6164       self.thread
-00009060: 2e73 7461 7274 2829 0a0a 2020 2020 6465  .start()..    de
-00009070: 6620 6a6f 696e 2873 656c 6629 3a0a 2020  f join(self):.  
-00009080: 2020 2020 2020 7365 6c66 2e74 6872 6561        self.threa
-00009090: 642e 6a6f 696e 2829 0a0a 2020 2020 6465  d.join()..    de
-000090a0: 6620 7265 6164 5f73 7562 7363 7269 7074  f read_subscript
-000090b0: 696f 6e28 7365 6c66 293a 0a20 2020 2020  ion(self):.     
-000090c0: 2020 2072 6571 2c20 7265 7370 203d 2073     req, resp = s
-000090d0: 656c 662e 636c 6965 6e74 2e72 6561 645f  elf.client.read_
-000090e0: 7375 6273 6372 6970 7469 6f6e 2867 726f  subscription(gro
-000090f0: 7570 5f6e 616d 653d 7365 6c66 2e67 726f  up_name=self.gro
-00009100: 7570 5f6e 616d 6529 0a20 2020 2020 2020  up_name).       
-00009110: 2066 6f72 2065 7665 6e74 2069 6e20 7265   for event in re
-00009120: 7370 3a0a 2020 2020 2020 2020 2020 2020  sp:.            
-00009130: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00009140: 2020 2020 2073 656c 662e 6361 6c6c 6261       self.callba
-00009150: 636b 2865 7665 6e74 290a 2020 2020 2020  ck(event).      
-00009160: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00009170: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
-00009180: 2020 2020 2020 2020 2020 2020 2023 2072               # r
-00009190: 6571 2e6e 6163 6b28 6576 656e 742e 6964  eq.nack(event.id
-000091a0: 2920 2023 206e 6f74 2079 6574 2069 6d70  )  # not yet imp
-000091b0: 6c65 6d65 6e74 6564 2e2e 2e2e 0a20 2020  lemented.....   
-000091c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000091d0: 662e 6572 726f 7220 3d20 650a 2020 2020  f.error = e.    
-000091e0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-000091f0: 6b0a 2020 2020 2020 2020 2020 2020 656c  k.            el
-00009200: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00009210: 2020 2020 7265 712e 6163 6b28 6576 656e      req.ack(even
-00009220: 742e 6964 290a 0a0a 2320 4372 6561 7465  t.id)...# Create
-00009230: 2061 6e6f 7468 6572 2070 6572 7369 7374   another persist
-00009240: 656e 7420 7375 6273 6372 6970 7469 6f6e  ent subscription
-00009250: 2e0a 6772 6f75 705f 6e61 6d65 203d 2066  ..group_name = f
-00009260: 2267 726f 7570 2d7b 7575 6964 3428 297d  "group-{uuid4()}
-00009270: 220a 636c 6965 6e74 2e63 7265 6174 655f  ".client.create_
-00009280: 7375 6273 6372 6970 7469 6f6e 2867 726f  subscription(gro
-00009290: 7570 5f6e 616d 653d 6772 6f75 705f 6e61  up_name=group_na
-000092a0: 6d65 290a 0a65 7665 6e74 7320 3d20 5b5d  me)..events = []
-000092b0: 0a0a 6465 6620 6861 6e64 6c65 5f65 7665  ..def handle_eve
-000092c0: 6e74 2865 7665 6e74 293a 0a20 2020 2065  nt(event):.    e
-000092d0: 7665 6e74 732e 6170 7065 6e64 2865 7665  vents.append(eve
-000092e0: 6e74 290a 2020 2020 6966 2065 7665 6e74  nt).    if event
-000092f0: 2e73 7472 6561 6d5f 6e61 6d65 203d 3d20  .stream_name == 
-00009300: 7374 7265 616d 5f6e 616d 6533 3a0a 2020  stream_name3:.  
-00009310: 2020 2020 2020 6966 2065 7665 6e74 2e64        if event.d
-00009320: 6174 6120 3d3d 2065 7665 6e74 392e 6461  ata == event9.da
-00009330: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00009340: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
-00009350: 290a 0a0a 7265 6164 6572 203d 2053 7562  )...reader = Sub
-00009360: 7363 7269 7074 696f 6e52 6561 6465 7228  scriptionReader(
-00009370: 0a20 2020 2063 6c69 656e 743d 636c 6965  .    client=clie
-00009380: 6e74 2c0a 2020 2020 6772 6f75 705f 6e61  nt,.    group_na
-00009390: 6d65 3d67 726f 7570 5f6e 616d 652c 0a20  me=group_name,. 
-000093a0: 2020 2063 616c 6c62 6163 6b3d 6861 6e64     callback=hand
-000093b0: 6c65 5f65 7665 6e74 0a29 0a0a 7265 6164  le_event.)..read
-000093c0: 6572 2e73 7461 7274 2829 0a72 6561 6465  er.start().reade
-000093d0: 722e 6a6f 696e 2829 0a0a 6173 7365 7274  r.join()..assert
-000093e0: 2065 7665 6e74 735b 2d31 5d2e 6461 7461   events[-1].data
-000093f0: 203d 3d20 6576 656e 7439 2e64 6174 610a   == event9.data.
-00009400: 6060 600a 0a50 6c65 6173 6520 6e6f 7465  ```..Please note
-00009410: 2c20 7768 656e 2070 726f 6365 7373 696e  , when processin
-00009420: 6720 6576 656e 7473 2069 6e20 6120 646f  g events in a do
-00009430: 776e 7374 7265 616d 2063 6f6d 706f 6e65  wnstream compone
-00009440: 6e74 2c20 7468 6520 636f 6d6d 6974 2070  nt, the commit p
-00009450: 6f73 6974 696f 6e20 6f66 0a74 6865 206c  osition of.the l
-00009460: 6173 7420 7375 6363 6573 7366 756c 6c79  ast successfully
-00009470: 2070 726f 6365 7373 6564 2065 7665 6e74   processed event
-00009480: 2069 7320 7573 6566 756c 6c79 2072 6563   is usefully rec
-00009490: 6f72 6465 6420 6279 2074 6865 2064 6f77  orded by the dow
-000094a0: 6e73 7472 6561 6d20 636f 6d70 6f6e 656e  nstream componen
-000094b0: 740a 736f 2074 6861 7420 7468 6520 636f  t.so that the co
-000094c0: 6d6d 6974 2070 6f73 6974 696f 6e20 6361  mmit position ca
-000094d0: 6e20 6265 2064 6574 6572 6d69 6e65 6420  n be determined 
-000094e0: 6279 2074 6865 2064 6f77 6e73 7472 6561  by the downstrea
-000094f0: 6d20 636f 6d70 6f6e 656e 7420 6672 6f6d  m component from
-00009500: 2069 7473 206f 776e 0a72 6563 6f72 6465   its own.recorde
-00009510: 6420 7768 656e 2069 7420 6973 2072 6573  d when it is res
-00009520: 7461 7274 6564 2e20 5468 6973 2063 6f6d  tarted. This com
-00009530: 6d69 7420 706f 7369 7469 6f6e 2063 616e  mit position can
-00009540: 2062 6520 7573 6564 2074 6f20 7370 6563   be used to spec
-00009550: 6966 7920 7468 6520 636f 6d6d 6974 0a70  ify the commit.p
-00009560: 6f73 6974 696f 6e20 6672 6f6d 2077 6869  osition from whi
-00009570: 6368 2074 6f20 7375 6273 6372 6962 652e  ch to subscribe.
-00009580: 2053 696e 6365 2074 6869 7320 636f 6d6d   Since this comm
-00009590: 6974 2070 6f73 6974 696f 6e20 7265 7072  it position repr
-000095a0: 6573 656e 7473 2074 6865 2070 6f73 6974  esents the posit
-000095b0: 696f 6e20 6f66 0a74 6865 206c 6173 7420  ion of.the last 
-000095c0: 7375 6363 6573 7366 756c 6c79 2070 726f  successfully pro
-000095d0: 6365 7373 6564 2065 7665 6e74 2069 6e20  cessed event in 
-000095e0: 6120 646f 776e 7374 7265 616d 2063 6f6d  a downstream com
-000095f0: 706f 6e65 6e74 2c20 736f 2069 7420 7769  ponent, so it wi
-00009600: 6c6c 2062 6520 7573 7561 6c20 746f 0a77  ll be usual to.w
-00009610: 616e 7420 746f 2072 6561 6420 6672 6f6d  ant to read from
-00009620: 2074 6865 206e 6578 7420 6576 656e 7420   the next event 
-00009630: 6166 7465 7220 7468 6973 2070 6f73 6974  after this posit
-00009640: 696f 6e2c 2062 6563 6175 7365 2074 6861  ion, because tha
-00009650: 7420 6973 2074 6865 206e 6578 7420 6576  t is the next ev
-00009660: 656e 740a 7468 6174 206e 6565 6473 2074  ent.that needs t
-00009670: 6f20 6265 2070 726f 6365 7373 6564 2e20  o be processed. 
-00009680: 486f 7765 7665 722c 2077 6865 6e20 7375  However, when su
-00009690: 6273 6372 6962 696e 6720 666f 7220 6576  bscribing for ev
-000096a0: 656e 7473 2075 7369 6e67 2061 2070 6572  ents using a per
-000096b0: 7369 7374 656e 740a 7375 6273 6372 6970  sistent.subscrip
-000096c0: 7469 6f6e 2069 6e20 4576 656e 7453 746f  tion in EventSto
-000096d0: 7265 4442 2c20 7468 6520 6576 656e 7420  reDB, the event 
-000096e0: 6174 2074 6865 2073 7065 6369 6669 6564  at the specified
-000096f0: 2063 6f6d 6d69 7420 706f 7369 7469 6f6e   commit position
-00009700: 204d 4159 2062 6520 7265 7475 726e 6564   MAY be returned
-00009710: 0a61 7320 7468 6520 6669 7273 7420 6576  .as the first ev
-00009720: 656e 7420 696e 2074 6865 2072 6563 6569  ent in the recei
-00009730: 7665 6420 7365 7175 656e 6365 206f 6620  ved sequence of 
-00009740: 7265 636f 7264 6564 2065 7665 6e74 732c  recorded events,
-00009750: 2061 6e64 2073 6f20 6974 206d 6179 0a62   and so it may.b
-00009760: 6520 6e65 6365 7373 6172 7920 746f 2063  e necessary to c
-00009770: 6865 636b 2074 6865 2063 6f6d 6d69 7420  heck the commit 
-00009780: 706f 7369 7469 6f6e 206f 6620 7468 6520  position of the 
-00009790: 7265 6365 6976 6564 2065 7665 6e74 7320  received events 
-000097a0: 616e 6420 746f 2064 6973 6361 7264 0a61  and to discard.a
-000097b0: 6e79 2020 7265 636f 7264 6564 2065 7665  ny  recorded eve
-000097c0: 6e74 206f 626a 6563 7420 7468 6174 2068  nt object that h
-000097d0: 6173 2061 2063 6f6d 6d69 7420 706f 7369  as a commit posi
-000097e0: 7469 6f6e 2065 7175 616c 2074 6f20 7468  tion equal to th
-000097f0: 6520 636f 6d6d 6974 2070 6f73 6974 696f  e commit positio
-00009800: 6e0a 7370 6563 6966 6965 6420 696e 2074  n.specified in t
-00009810: 6865 2072 6571 7565 7374 2e0a 0a57 6869  he request...Whi
-00009820: 6c73 7420 7468 6572 6520 6172 6520 736f  lst there are so
-00009830: 6d65 2061 6476 616e 7461 6765 7320 6f66  me advantages of
-00009840: 2070 6572 7369 7374 656e 7420 7375 6273   persistent subs
-00009850: 6372 6970 7469 6f6e 732c 2062 7920 7472  criptions, by tr
-00009860: 6163 6b69 6e67 2069 6e20 7468 650a 7570  acking in the.up
-00009870: 7374 7265 616d 2073 6572 7665 7220 7468  stream server th
-00009880: 6520 706f 7369 7469 6f6e 2069 6e20 7468  e position in th
-00009890: 6520 636f 6d6d 6974 2073 6571 7565 6e63  e commit sequenc
-000098a0: 6520 6f66 2065 7665 6e74 7320 7468 6174  e of events that
-000098b0: 2068 6176 6520 6265 656e 2070 726f 6365   have been proce
-000098c0: 7373 6564 2c0a 7468 6572 6520 6973 2061  ssed,.there is a
-000098d0: 2064 616e 6765 7220 6f66 2022 6475 616c   danger of "dual
-000098e0: 2077 7269 7469 6e67 2220 696e 2074 6865   writing" in the
-000098f0: 2063 6f6e 7375 6d70 7469 6f6e 206f 6620   consumption of 
-00009900: 6576 656e 7473 2e20 5468 6520 6461 6e67  events. The dang
-00009910: 6572 2069 7320 7468 6174 2069 660a 616e  er is that if.an
-00009920: 2065 7665 6e74 2069 7320 7375 6363 6573   event is succes
-00009930: 7366 756c 6c79 2070 726f 6365 7373 6564  sfully processed
-00009940: 2062 7574 2074 6865 6e20 7468 6520 6163   but then the ac
-00009950: 6b6e 6f77 6c65 6467 6d65 6e74 2066 6169  knowledgment fai
-00009960: 6c73 2c20 7468 6520 6576 656e 7420 6d61  ls, the event ma
-00009970: 7920 6265 0a72 6563 6569 7665 6420 6d6f  y be.received mo
-00009980: 7265 2074 6861 6e20 6f6e 6365 2e20 4f6e  re than once. On
-00009990: 2074 6865 206f 7468 6572 2068 616e 642c   the other hand,
-000099a0: 2069 6620 7468 6520 6163 6b6e 6f77 6c65   if the acknowle
-000099b0: 6467 6d65 6e74 2069 7320 7375 6363 6573  dgment is succes
-000099c0: 7366 756c 2062 7574 0a74 6865 6e20 7468  sful but.then th
-000099d0: 6520 7072 6f63 6573 7369 6e67 2066 6169  e processing fai
-000099e0: 6c73 2c20 7468 6520 6576 656e 7420 6d61  ls, the event ma
-000099f0: 7920 6566 6665 6374 6976 656c 7920 6e6f  y effectively no
-00009a00: 7420 6265 2062 6565 6e20 7072 6f63 6573  t be been proces
-00009a10: 7365 642e 2042 7920 6569 7468 6572 0a70  sed. By either.p
-00009a20: 726f 6365 7373 696e 6720 616e 2065 7665  rocessing an eve
-00009a30: 6e74 7320 6d6f 7265 2074 6861 6e20 6f6e  nts more than on
-00009a40: 6365 2c20 6f72 2066 6169 6c69 6e67 2074  ce, or failing t
-00009a50: 6f20 7072 6f63 6573 7320 616e 2065 7665  o process an eve
-00009a60: 6e74 2c20 7468 6520 7265 7375 6c74 696e  nt, the resultin
-00009a70: 6720 7374 6174 650a 6f66 2074 6865 2070  g state.of the p
-00009a80: 726f 6365 7373 696e 6720 6f66 2074 6865  rocessing of the
-00009a90: 2072 6563 6f72 6465 6420 6576 656e 7473   recorded events
-00009aa0: 206d 6967 6874 2062 6520 696e 6163 6375   might be inaccu
-00009ab0: 7261 7465 2c20 6f72 2070 6f73 7369 626c  rate, or possibl
-00009ac0: 790a 696e 636f 6e73 6973 7465 6e74 2c20  y.inconsistent, 
-00009ad0: 616e 6420 7065 7268 6170 7320 6361 7461  and perhaps cata
-00009ae0: 7374 726f 7068 6963 616c 6c79 2073 6f2e  strophically so.
-00009af0: 2041 6e79 2072 656c 6174 6976 656c 7920   Any relatively 
-00009b00: 6d69 6e6f 7220 636f 6e73 6571 7565 6e63  minor consequenc
-00009b10: 6573 206d 6179 206f 720a 6d61 7920 6e6f  es may or.may no
-00009b20: 7420 6d61 7474 6572 2069 6e20 796f 7572  t matter in your
-00009b30: 2073 6974 7561 7469 6f6e 2e20 4275 7420   situation. But 
-00009b40: 736f 6d65 7469 6d65 7320 696e 636f 6e73  sometimes incons
-00009b50: 6973 7465 6e63 6965 7320 6d61 7920 6861  istencies may ha
-00009b60: 6c74 2070 726f 6365 7373 696e 670a 756e  lt processing.un
-00009b70: 7469 6c20 7468 6520 6973 7375 6520 6973  til the issue is
-00009b80: 2072 6573 6f6c 7665 642e 2059 6f75 2063   resolved. You c
-00009b90: 616e 2061 766f 6964 2022 6475 616c 2077  an avoid "dual w
-00009ba0: 7269 7469 6e67 2220 696e 2074 6865 2063  riting" in the c
-00009bb0: 6f6e 7375 6d70 7469 6f6e 206f 6620 6576  onsumption of ev
-00009bc0: 656e 7473 0a62 7920 6174 6f6d 6963 616c  ents.by atomical
-00009bd0: 6c79 2072 6563 6f72 6469 6e67 2074 6865  ly recording the
-00009be0: 2063 6f6d 6d69 7420 706f 7369 7469 6f6e   commit position
-00009bf0: 206f 6620 616e 2065 7665 6e74 2074 6861   of an event tha
-00009c00: 7420 6861 7320 6265 656e 2070 726f 6365  t has been proce
-00009c10: 7373 6564 2061 6c6f 6e67 0a77 6974 6820  ssed along.with 
-00009c20: 7468 6520 7265 7375 6c74 7320 6f66 2070  the results of p
-00009c30: 726f 6365 7373 696e 6720 7468 6174 2065  rocessing that e
-00009c40: 7665 6e74 2028 7468 6174 2069 732c 2077  vent (that is, w
-00009c50: 6974 6820 626f 7468 2074 6869 6e67 7320  ith both things 
-00009c60: 6265 696e 6720 7265 636f 7264 6564 2069  being recorded i
-00009c70: 6e0a 7468 6520 7361 6d65 2074 7261 6e73  n.the same trans
-00009c80: 6163 7469 6f6e 292c 2061 6e64 206d 616b  action), and mak
-00009c90: 696e 6720 7468 6573 6520 7265 636f 7264  ing these record
-00009ca0: 7320 756e 6971 7565 2073 6f20 7468 6174  s unique so that
-00009cb0: 2074 7261 6e73 6163 7469 6f6e 7320 7769   transactions wi
-00009cc0: 6c6c 2062 650a 726f 6c6c 6564 2062 6163  ll be.rolled bac
-00009cd0: 6b20 7072 6576 656e 7469 6e67 2074 6865  k preventing the
-00009ce0: 2072 6573 756c 7473 206f 6620 7265 7072   results of repr
-00009cf0: 6f63 6573 7369 6e67 2074 6865 2065 7665  ocessing the eve
-00009d00: 6e74 2062 6569 6e67 2063 6f6d 6d69 7474  nt being committ
-00009d10: 6564 2e0a 0a23 2320 4e6f 7465 730a 0a23  ed...## Notes..#
-00009d20: 2323 2052 6567 756c 6172 2065 7870 7265  ## Regular expre
-00009d30: 7373 696f 6e20 6669 6c74 6572 730a 0a54  ssion filters..T
-00009d40: 6865 2066 696c 7465 7220 6172 6775 6d65  he filter argume
-00009d50: 6e74 7320 696e 2060 7265 6164 5f61 6c6c  nts in `read_all
-00009d60: 5f65 7665 6e74 7328 2960 2c20 6073 7562  _events()`, `sub
-00009d70: 7363 7269 6265 5f61 6c6c 5f65 7665 6e74  scribe_all_event
-00009d80: 7328 2960 2c0a 6063 7265 6174 655f 7375  s()`,.`create_su
-00009d90: 6273 6372 6970 7469 6f6e 2829 6020 616e  bscription()` an
-00009da0: 6420 6063 6f6d 6d69 745f 706f 7369 7469  d `commit_positi
-00009db0: 6f6e 2829 6020 6172 6520 6170 706c 6965  on()` are applie
-00009dc0: 6420 746f 2074 6865 2060 7479 7065 600a  d to the `type`.
-00009dd0: 6174 7472 6962 7574 6520 6f66 2072 6563  attribute of rec
-00009de0: 6f72 6465 6420 6576 656e 7473 2e0a 0a54  orded events...T
-00009df0: 6865 2064 6566 6175 6c74 2076 616c 7565  he default value
-00009e00: 206f 6620 7468 6520 6066 696c 7465 725f   of the `filter_
-00009e10: 6578 636c 7564 6560 2061 7267 756d 656e  exclude` argumen
-00009e20: 7473 2069 7320 6465 7369 676e 6564 2074  ts is designed t
-00009e30: 6f20 6578 636c 7564 650a 4576 656e 7453  o exclude.EventS
-00009e40: 746f 7265 4442 2022 7379 7374 656d 2220  toreDB "system" 
-00009e50: 616e 6420 2270 6572 7369 7374 656e 6365  and "persistence
-00009e60: 2073 7562 7363 7269 7074 696f 6e20 636f   subscription co
-00009e70: 6e66 6967 2220 6576 656e 7473 2c20 7768  nfig" events, wh
-00009e80: 6963 680a 6f74 6865 7277 6973 6520 776f  ich.otherwise wo
-00009e90: 756c 6420 6265 2069 6e63 6c75 6465 642e  uld be included.
-00009ea0: 2053 7973 7465 6d20 6576 656e 7473 2067   System events g
-00009eb0: 656e 6572 6174 6564 2062 7920 4576 656e  enerated by Even
-00009ec0: 7453 746f 7265 4442 2061 6c6c 0a68 6176  tStoreDB all.hav
-00009ed0: 6520 6074 7970 6560 2073 7472 696e 6773  e `type` strings
-00009ee0: 2074 6861 7420 7374 6172 7420 7769 7468   that start with
-00009ef0: 2074 6865 2060 2460 2073 6967 6e2e 2050   the `$` sign. P
-00009f00: 6572 7369 7374 656e 6365 2073 7562 7363  ersistence subsc
-00009f10: 7269 7074 696f 6e0a 6576 656e 7473 2067  ription.events g
-00009f20: 656e 6572 6174 6564 2077 6865 6e20 6d61  enerated when ma
-00009f30: 6e69 7075 6c61 7469 6e67 2070 6572 7369  nipulating persi
-00009f40: 7374 656e 6365 2073 7562 7363 7269 7074  stence subscript
-00009f50: 696f 6e73 2061 6c6c 2068 6176 6520 6074  ions all have `t
-00009f60: 7970 6560 0a73 7472 696e 6773 2074 6861  ype`.strings tha
-00009f70: 7420 7374 6172 7420 7769 7468 2060 5065  t start with `Pe
-00009f80: 7273 6973 7465 6e74 436f 6e66 6967 602e  rsistentConfig`.
-00009f90: 0a0a 466f 7220 6578 616d 706c 652c 2074  ..For example, t
-00009fa0: 6f20 6d61 7463 6820 7468 6520 7479 7065  o match the type
-00009fb0: 206f 6620 4576 656e 7453 746f 7265 4442   of EventStoreDB
-00009fc0: 2073 7973 7465 6d20 6576 656e 7473 2c20   system events, 
-00009fd0: 7573 6520 7468 6520 7265 6775 6c61 720a  use the regular.
-00009fe0: 6578 7072 6573 7369 6f6e 2060 7227 5c24  expression `r'\$
-00009ff0: 2e2b 2760 2e20 506c 6561 7365 206e 6f74  .+'`. Please not
-0000a000: 652c 2074 6865 2063 6f6e 7374 616e 7420  e, the constant 
-0000a010: 6045 5344 425f 5359 5354 454d 5f45 5645  `ESDB_SYSTEM_EVE
-0000a020: 4e54 535f 5245 4745 5860 2069 730a 7365  NTS_REGEX` is.se
-0000a030: 7420 746f 2060 7227 5c24 2e2b 2760 2e20  t to `r'\$.+'`. 
-0000a040: 596f 7520 6361 6e20 696d 706f 7274 2074  You can import t
-0000a050: 6869 7320 7661 6c75 650a 2860 6672 6f6d  his value.(`from
-0000a060: 2065 7364 6263 6c69 656e 7420 696d 706f   esdbclient impo
-0000a070: 7274 2045 5344 425f 5359 5354 454d 5f45  rt ESDB_SYSTEM_E
-0000a080: 5645 4e54 535f 5245 4745 5860 2920 616e  VENTS_REGEX`) an
-0000a090: 6420 7573 650a 6974 2077 6865 6e20 6275  d use.it when bu
-0000a0a0: 696c 6469 6e67 206c 6f6e 6765 7220 7365  ilding longer se
-0000a0b0: 7175 656e 6365 7320 6f66 2072 6567 756c  quences of regul
-0000a0c0: 6172 2065 7870 7265 7373 696f 6e73 2e0a  ar expressions..
-0000a0d0: 0a53 696d 696c 6172 6c79 2c20 746f 206d  .Similarly, to m
-0000a0e0: 6174 6368 2074 6865 2074 7970 6520 6f66  atch the type of
-0000a0f0: 2045 7665 6e74 5374 6f72 6544 4220 7065   EventStoreDB pe
-0000a100: 7273 6973 7465 6e63 6520 7375 6273 6372  rsistence subscr
-0000a110: 6970 7469 6f6e 2065 7665 6e74 732c 2075  iption events, u
-0000a120: 7365 2074 6865 0a72 6567 756c 6172 2065  se the.regular e
-0000a130: 7870 7265 7373 696f 6e20 6072 2750 6572  xpression `r'Per
-0000a140: 7369 7374 656e 7443 6f6e 6669 675c 642b  sistentConfig\d+
-0000a150: 2760 2e20 5468 6520 636f 6e73 7461 6e74  '`. The constant
-0000a160: 2060 4553 4442 5f50 4552 5349 5354 454e   `ESDB_PERSISTEN
-0000a170: 545f 434f 4e46 4947 5f45 5645 4e54 535f  T_CONFIG_EVENTS_
-0000a180: 5245 4745 5860 0a69 7320 7365 7420 746f  REGEX`.is set to
-0000a190: 2060 7227 5065 7273 6973 7465 6e74 436f   `r'PersistentCo
-0000a1a0: 6e66 6967 5c64 2b27 602e 2059 6f75 2063  nfig\d+'`. You c
-0000a1b0: 616e 2061 6c73 6f20 696d 706f 7274 2074  an also import t
-0000a1c0: 6869 7320 7661 6c75 650a 2860 6672 6f6d  his value.(`from
-0000a1d0: 2065 7364 6263 6c69 656e 7420 696d 706f   esdbclient impo
-0000a1e0: 7274 2045 5344 425f 5045 5253 4953 5445  rt ESDB_PERSISTE
-0000a1f0: 4e54 5f43 4f4e 4649 475f 4556 454e 5453  NT_CONFIG_EVENTS
-0000a200: 5f52 4547 4558 6029 2061 6e64 2075 7365  _REGEX`) and use
-0000a210: 2069 7420 7768 656e 2062 7569 6c64 696e   it when buildin
-0000a220: 670a 6c6f 6e67 6572 2073 6571 7565 6e63  g.longer sequenc
-0000a230: 6573 206f 6620 7265 6775 6c61 7220 6578  es of regular ex
-0000a240: 7072 6573 7369 6f6e 732e 0a0a 5468 6520  pressions...The 
-0000a250: 636f 6e73 7461 6e74 2060 4445 4641 554c  constant `DEFAUL
-0000a260: 545f 4558 434c 5544 455f 4649 4c54 4552  T_EXCLUDE_FILTER
-0000a270: 6020 6973 2061 2073 6571 7565 6e63 6520  ` is a sequence 
-0000a280: 6f66 2072 6567 756c 6172 2065 7870 7265  of regular expre
-0000a290: 7373 696f 6e73 2074 6861 7420 6d61 7463  ssions that matc
-0000a2a0: 680a 7468 6520 6576 656e 7473 2074 6861  h.the events tha
-0000a2b0: 7420 4576 656e 7453 746f 7265 4442 2067  t EventStoreDB g
-0000a2c0: 656e 6572 6174 6573 2069 6e74 6572 6e61  enerates interna
-0000a2d0: 6c6c 792c 2065 7665 6e74 7320 7468 6174  lly, events that
-0000a2e0: 2061 7265 2065 7874 7261 6e65 6f75 7320   are extraneous 
-0000a2f0: 746f 2074 686f 7365 0a77 6869 6368 2079  to those.which y
-0000a300: 6f75 2061 7070 656e 6420 7573 696e 6720  ou append using 
-0000a310: 7468 6520 6061 7070 656e 645f 6576 656e  the `append_even
-0000a320: 7473 2829 6020 6d65 7468 6f64 2e0a 0a46  ts()` method...F
-0000a330: 6f72 2065 7861 6d70 6c65 2c20 746f 2065  or example, to e
-0000a340: 7863 6c75 6465 2073 7973 7465 6d20 6576  xclude system ev
-0000a350: 656e 7473 2061 6e64 2070 6572 7369 7374  ents and persist
-0000a360: 656e 6365 2073 7562 7363 7269 7074 696f  ence subscriptio
-0000a370: 6e20 636f 6e66 6967 7572 6174 696f 6e20  n configuration 
-0000a380: 6576 656e 7473 2c0a 616e 6420 736e 6170  events,.and snap
-0000a390: 7368 6f74 732c 2079 6f75 206d 6967 6874  shots, you might
-0000a3a0: 2075 7365 2074 6865 2073 6571 7565 6e63   use the sequenc
-0000a3b0: 6520 6044 4546 4155 4c54 5f45 5843 4c55  e `DEFAULT_EXCLU
-0000a3c0: 4445 5f46 494c 5445 5220 2b20 5b27 2e2a  DE_FILTER + ['.*
-0000a3d0: 536e 6170 7368 6f74 275d 6020 6173 0a74  Snapshot']` as.t
-0000a3e0: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
-0000a3f0: 6066 696c 7465 725f 6578 636c 7564 6560  `filter_exclude`
-0000a400: 2061 7267 756d 656e 7420 7768 656e 2063   argument when c
-0000a410: 616c 6c69 6e67 2060 7265 6164 5f61 6c6c  alling `read_all
-0000a420: 5f65 7665 6e74 7328 2960 2c0a 6073 7562  _events()`,.`sub
-0000a430: 7363 7269 6265 5f61 6c6c 5f65 7665 6e74  scribe_all_event
-0000a440: 7328 2960 2c20 6063 7265 6174 655f 7375  s()`, `create_su
-0000a450: 6273 6372 6970 7469 6f6e 2829 6020 6f72  bscription()` or
-0000a460: 2060 6765 745f 636f 6d6d 6974 5f70 6f73   `get_commit_pos
-0000a470: 6974 696f 6e28 2960 2e0a 0a23 2323 2054  ition()`...### T
-0000a480: 6865 204e 6577 4576 656e 7420 636c 6173  he NewEvent clas
-0000a490: 730a 0a54 6865 2060 4e65 7745 7665 6e74  s..The `NewEvent
-0000a4a0: 6020 636c 6173 7320 6973 2075 7365 6420  ` class is used 
-0000a4b0: 7768 656e 2061 7070 656e 6469 6e67 2065  when appending e
-0000a4c0: 7665 6e74 732e 0a0a 5468 6520 7265 7175  vents...The requ
-0000a4d0: 6972 6564 2061 7267 756d 656e 7420 6074  ired argument `t
-0000a4e0: 7970 6560 2069 7320 6120 5079 7468 6f6e  ype` is a Python
-0000a4f0: 2060 7374 7260 206f 626a 6563 742c 2075   `str` object, u
-0000a500: 7365 6420 746f 2069 6e64 6963 6174 6520  sed to indicate 
-0000a510: 7468 6520 7479 7065 206f 660a 7468 6520  the type of.the 
-0000a520: 6576 656e 7420 7468 6174 2077 696c 6c20  event that will 
-0000a530: 6265 2072 6563 6f72 6465 642e 0a0a 5468  be recorded...Th
-0000a540: 6520 7265 7175 6972 6564 2061 7267 756d  e required argum
-0000a550: 656e 7420 6064 6174 6160 2069 7320 6120  ent `data` is a 
-0000a560: 5079 7468 6f6e 2060 6279 7465 7360 206f  Python `bytes` o
-0000a570: 626a 6563 742c 2075 7365 6420 746f 2069  bject, used to i
-0000a580: 6e64 6963 6174 6520 7468 6520 6461 7461  ndicate the data
-0000a590: 206f 660a 7468 6520 6576 656e 7420 7468   of.the event th
-0000a5a0: 6174 2077 696c 6c20 6265 2072 6563 6f72  at will be recor
-0000a5b0: 6465 642e 0a0a 5468 6520 6f70 7469 6f6e  ded...The option
-0000a5c0: 616c 2061 7267 756d 656e 7420 606d 6574  al argument `met
-0000a5d0: 6164 6174 6160 2069 7320 6120 5079 7468  adata` is a Pyth
-0000a5e0: 6f6e 2060 6279 7465 7360 206f 626a 6563  on `bytes` objec
-0000a5f0: 742c 2075 7365 6420 746f 2069 6e64 6963  t, used to indic
-0000a600: 6174 6520 616e 790a 6d65 7461 6461 7461  ate any.metadata
-0000a610: 206f 6620 7468 6520 6576 656e 7420 7468   of the event th
-0000a620: 6174 2077 696c 6c20 6265 2072 6563 6f72  at will be recor
-0000a630: 6465 642e 2054 6865 2064 6566 6175 6c74  ded. The default
-0000a640: 2076 616c 7565 2069 7320 616e 2065 6d70   value is an emp
-0000a650: 7479 2060 6279 7465 7360 0a6f 626a 6563  ty `bytes`.objec
-0000a660: 742e 0a0a 5468 6520 6f70 7469 6f6e 616c  t...The optional
-0000a670: 2061 7267 756d 656e 7420 6063 6f6e 7465   argument `conte
-0000a680: 6e74 5f74 7970 6560 2069 7320 6120 5079  nt_type` is a Py
-0000a690: 7468 6f6e 2060 7374 7260 206f 626a 6563  thon `str` objec
-0000a6a0: 742c 2075 7365 6420 746f 2069 6e64 6963  t, used to indic
-0000a6b0: 6174 6520 7468 650a 7479 7065 206f 6620  ate the.type of 
-0000a6c0: 7468 6520 6461 7461 2074 6861 7420 7769  the data that wi
-0000a6d0: 6c6c 2062 6520 7265 636f 7264 6564 2066  ll be recorded f
-0000a6e0: 6f72 2074 6869 7320 6576 656e 742e 2054  or this event. T
-0000a6f0: 6865 2064 6566 6175 6c74 2076 616c 7565  he default value
-0000a700: 2069 730a 6061 7070 6c69 6361 7469 6f6e   is.`application
-0000a710: 2f6a 736f 6e60 2c20 7768 6963 6820 696e  /json`, which in
-0000a720: 6469 6361 7465 7320 7468 6174 2074 6865  dicates that the
-0000a730: 2060 6461 7461 6020 7761 7320 7365 7269   `data` was seri
-0000a740: 616c 6973 6564 2075 7369 6e67 204a 534f  alised using JSO
-0000a750: 4e2e 0a41 6e20 616c 7465 726e 6174 6976  N..An alternativ
-0000a760: 6520 7661 6c75 6520 666f 7220 7468 6973  e value for this
-0000a770: 2061 7267 756d 656e 7420 6973 2060 6170   argument is `ap
-0000a780: 706c 6963 6174 696f 6e2f 6f63 7465 742d  plication/octet-
-0000a790: 7374 7265 616d 602e 0a0a 5468 6520 6f70  stream`...The op
-0000a7a0: 7469 6f6e 616c 2061 7267 756d 656e 7420  tional argument 
-0000a7b0: 6069 6460 2069 7320 6120 5079 7468 6f6e  `id` is a Python
-0000a7c0: 2060 5555 4944 6020 6f62 6a65 6374 2c20   `UUID` object, 
-0000a7d0: 7573 6564 2074 6f20 7370 6563 6966 7920  used to specify 
-0000a7e0: 7468 6520 756e 6971 7565 2049 440a 6f66  the unique ID.of
-0000a7f0: 2074 6865 2065 7665 6e74 2074 6861 7420   the event that 
-0000a800: 7769 6c6c 2062 6520 7265 636f 7264 6564  will be recorded
-0000a810: 2e20 5468 6973 2076 616c 7565 2077 696c  . This value wil
-0000a820: 6c20 6465 6661 756c 7420 746f 2061 206e  l default to a n
-0000a830: 6577 2076 6572 7369 6f6e 2d34 2055 5549  ew version-4 UUI
-0000a840: 442e 0a0a 6060 6070 7974 686f 6e0a 6e65  D...```python.ne
-0000a850: 775f 6576 656e 7431 203d 204e 6577 4576  w_event1 = NewEv
-0000a860: 656e 7428 0a20 2020 2074 7970 653d 274f  ent(.    type='O
-0000a870: 7264 6572 4372 6561 7465 6427 2c0a 2020  rderCreated',.  
-0000a880: 2020 6461 7461 3d62 277b 226e 616d 6522    data=b'{"name"
-0000a890: 3a20 2247 7265 6722 7d27 2c0a 290a 6173  : "Greg"}',.).as
-0000a8a0: 7365 7274 206e 6577 5f65 7665 6e74 312e  sert new_event1.
-0000a8b0: 7479 7065 203d 3d20 274f 7264 6572 4372  type == 'OrderCr
-0000a8c0: 6561 7465 6427 0a61 7373 6572 7420 6e65  eated'.assert ne
-0000a8d0: 775f 6576 656e 7431 2e64 6174 6120 3d3d  w_event1.data ==
-0000a8e0: 2062 277b 226e 616d 6522 3a20 2247 7265   b'{"name": "Gre
-0000a8f0: 6722 7d27 0a61 7373 6572 7420 6e65 775f  g"}'.assert new_
-0000a900: 6576 656e 7431 2e6d 6574 6164 6174 6120  event1.metadata 
-0000a910: 3d3d 2062 2727 0a61 7373 6572 7420 6e65  == b''.assert ne
-0000a920: 775f 6576 656e 7431 2e63 6f6e 7465 6e74  w_event1.content
-0000a930: 5f74 7970 6520 3d3d 2027 6170 706c 6963  _type == 'applic
-0000a940: 6174 696f 6e2f 6a73 6f6e 270a 6173 7365  ation/json'.asse
-0000a950: 7274 2069 7369 6e73 7461 6e63 6528 6e65  rt isinstance(ne
-0000a960: 775f 6576 656e 7431 2e69 642c 2055 5549  w_event1.id, UUI
-0000a970: 4429 0a0a 6576 656e 745f 6964 203d 2075  D)..event_id = u
-0000a980: 7569 6434 2829 0a6e 6577 5f65 7665 6e74  uid4().new_event
-0000a990: 3220 3d20 4e65 7745 7665 6e74 280a 2020  2 = NewEvent(.  
-0000a9a0: 2020 7479 7065 3d27 496d 6167 6543 7265    type='ImageCre
-0000a9b0: 6174 6564 272c 0a20 2020 2064 6174 613d  ated',.    data=
-0000a9c0: 6227 3031 3031 3031 3031 3031 3031 3031  b'01010101010101
-0000a9d0: 272c 0a20 2020 206d 6574 6164 6174 613d  ',.    metadata=
-0000a9e0: 6227 7b22 6122 3a20 317d 272c 0a20 2020  b'{"a": 1}',.   
-0000a9f0: 2063 6f6e 7465 6e74 5f74 7970 653d 2761   content_type='a
-0000aa00: 7070 6c69 6361 7469 6f6e 2f6f 6374 6574  pplication/octet
-0000aa10: 2d73 7472 6561 6d27 2c0a 2020 2020 6964  -stream',.    id
-0000aa20: 3d65 7665 6e74 5f69 642c 0a29 0a61 7373  =event_id,.).ass
-0000aa30: 6572 7420 6e65 775f 6576 656e 7432 2e74  ert new_event2.t
-0000aa40: 7970 6520 3d3d 2027 496d 6167 6543 7265  ype == 'ImageCre
-0000aa50: 6174 6564 270a 6173 7365 7274 206e 6577  ated'.assert new
-0000aa60: 5f65 7665 6e74 322e 6461 7461 203d 3d20  _event2.data == 
-0000aa70: 6227 3031 3031 3031 3031 3031 3031 3031  b'01010101010101
-0000aa80: 270a 6173 7365 7274 206e 6577 5f65 7665  '.assert new_eve
-0000aa90: 6e74 322e 6d65 7461 6461 7461 203d 3d20  nt2.metadata == 
-0000aaa0: 6227 7b22 6122 3a20 317d 270a 6173 7365  b'{"a": 1}'.asse
-0000aab0: 7274 206e 6577 5f65 7665 6e74 322e 636f  rt new_event2.co
-0000aac0: 6e74 656e 745f 7479 7065 203d 3d20 2761  ntent_type == 'a
-0000aad0: 7070 6c69 6361 7469 6f6e 2f6f 6374 6574  pplication/octet
-0000aae0: 2d73 7472 6561 6d27 0a61 7373 6572 7420  -stream'.assert 
-0000aaf0: 6e65 775f 6576 656e 7432 2e69 6420 3d3d  new_event2.id ==
-0000ab00: 2065 7665 6e74 5f69 640a 6060 600a 0a23   event_id.```..#
-0000ab10: 2323 2054 6865 2052 6563 6f72 6465 6445  ## The RecordedE
-0000ab20: 7665 6e74 2063 6c61 7373 0a0a 5468 6520  vent class..The 
-0000ab30: 6052 6563 6f72 6465 6445 7665 6e74 6020  `RecordedEvent` 
-0000ab40: 636c 6173 7320 6973 2075 7365 6420 7768  class is used wh
-0000ab50: 656e 2072 6561 6469 6e67 2065 7665 6e74  en reading event
-0000ab60: 732e 0a0a 5468 6520 6174 7472 6962 7574  s...The attribut
-0000ab70: 6520 6074 7970 6560 2069 7320 6120 5079  e `type` is a Py
-0000ab80: 7468 6f6e 2060 7374 7260 206f 626a 6563  thon `str` objec
-0000ab90: 742c 2075 7365 6420 746f 2069 6e64 6963  t, used to indic
-0000aba0: 6174 6520 7468 6520 7479 7065 206f 6620  ate the type of 
-0000abb0: 6576 656e 740a 7468 6174 2077 6173 2072  event.that was r
-0000abc0: 6563 6f72 6465 642e 0a0a 5468 6520 6174  ecorded...The at
-0000abd0: 7472 6962 7574 6520 6064 6174 6160 2069  tribute `data` i
-0000abe0: 7320 6120 5079 7468 6f6e 2060 6279 7465  s a Python `byte
-0000abf0: 7360 206f 626a 6563 742c 2075 7365 6420  s` object, used 
-0000ac00: 746f 2069 6e64 6963 6174 6520 7468 6520  to indicate the 
-0000ac10: 6461 7461 206f 6620 7468 650a 6576 656e  data of the.even
-0000ac20: 7420 7468 6174 2077 6173 2072 6563 6f72  t that was recor
-0000ac30: 6465 642e 0a0a 5468 6520 6174 7472 6962  ded...The attrib
-0000ac40: 7574 6520 606d 6574 6164 6174 6160 2069  ute `metadata` i
-0000ac50: 7320 6120 5079 7468 6f6e 2060 6279 7465  s a Python `byte
-0000ac60: 7360 206f 626a 6563 742c 2075 7365 6420  s` object, used 
-0000ac70: 746f 2069 6e64 6963 6174 6520 7468 6520  to indicate the 
-0000ac80: 6d65 7461 6461 7461 206f 660a 7468 6520  metadata of.the 
-0000ac90: 6576 656e 7420 7468 6174 2077 6173 2072  event that was r
-0000aca0: 6563 6f72 6465 642e 0a0a 5468 6520 6174  ecorded...The at
-0000acb0: 7472 6962 7574 6520 6063 6f6e 7465 6e74  tribute `content
-0000acc0: 5f74 7970 6560 2069 7320 6120 5079 7468  _type` is a Pyth
-0000acd0: 6f6e 2060 7374 7260 206f 626a 6563 742c  on `str` object,
-0000ace0: 2075 7365 6420 746f 2069 6e64 6963 6174   used to indicat
-0000acf0: 6520 7468 6520 7479 7065 206f 660a 6461  e the type of.da
-0000ad00: 7461 2074 6861 7420 7761 7320 7265 636f  ta that was reco
-0000ad10: 7264 6564 2066 6f72 2074 6869 7320 6576  rded for this ev
-0000ad20: 656e 7420 2875 7375 616c 6c79 2060 6170  ent (usually `ap
-0000ad30: 706c 6963 6174 696f 6e2f 6a73 6f6e 6020  plication/json` 
-0000ad40: 746f 2069 6e64 6963 6174 6520 7468 6174  to indicate that
-0000ad50: 0a74 6869 7320 6461 7461 2063 616e 2062  .this data can b
-0000ad60: 6520 7061 7273 6564 2061 7320 4a53 4f4e  e parsed as JSON
-0000ad70: 2c20 6275 7420 616c 7465 726e 6174 6976  , but alternativ
-0000ad80: 656c 7920 6061 7070 6c69 6361 7469 6f6e  ely `application
-0000ad90: 2f6f 6374 6574 2d73 7472 6561 6d60 2074  /octet-stream` t
-0000ada0: 6f0a 696e 6469 6361 7465 2074 6861 7420  o.indicate that 
-0000adb0: 6974 2069 7320 736f 6d65 7468 696e 6720  it is something 
-0000adc0: 656c 7365 292e 0a0a 5468 6520 6174 7472  else)...The attr
-0000add0: 6962 7574 6520 6069 6460 2069 7320 6120  ibute `id` is a 
-0000ade0: 5079 7468 6f6e 2060 5555 4944 6020 6f62  Python `UUID` ob
-0000adf0: 6a65 6374 2c20 7573 6564 2074 6f20 696e  ject, used to in
-0000ae00: 6469 6361 7465 2074 6865 2075 6e69 7175  dicate the uniqu
-0000ae10: 6520 4944 206f 6620 7468 650a 6576 656e  e ID of the.even
-0000ae20: 7420 7468 6174 2077 6173 2072 6563 6f72  t that was recor
-0000ae30: 6465 642e 2050 6c65 6173 6520 6e6f 7465  ded. Please note
-0000ae40: 2c20 7768 656e 2072 6563 6f72 6465 6420  , when recorded 
-0000ae50: 6576 656e 7473 2061 7265 2072 6574 7572  events are retur
-0000ae60: 6e65 6420 6672 6f6d 2061 2063 616c 6c0a  ned from a call.
-0000ae70: 746f 2060 7265 6164 5f73 7472 6561 6d5f  to `read_stream_
-0000ae80: 6576 656e 7473 2829 6020 696e 2045 7665  events()` in Eve
-0000ae90: 6e74 5374 6f72 6544 4220 7632 312e 3130  ntStoreDB v21.10
-0000aea0: 2c20 7468 6520 636f 6d6d 6974 2070 6f73  , the commit pos
-0000aeb0: 6974 696f 6e20 6973 206e 6f74 2061 6374  ition is not act
-0000aec0: 7561 6c6c 790a 7365 7420 696e 2074 6865  ually.set in the
-0000aed0: 2072 6573 706f 6e73 652e 2046 6f72 2074   response. For t
-0000aee0: 6869 7320 7265 6173 6f6e 2c20 7468 6973  his reason, this
-0000aef0: 2061 7474 7269 6275 7465 2069 7320 6163   attribute is ac
-0000af00: 7475 616c 6c79 2074 7970 6564 2061 7320  tually typed as 
-0000af10: 616e 206f 7074 696f 6e61 6c0a 7661 6c75  an optional.valu
-0000af20: 6520 2860 4f70 7469 6f6e 616c 5b55 5549  e (`Optional[UUI
-0000af30: 445d 6029 2c20 616e 6420 7468 6973 2063  D]`), and this c
-0000af40: 6173 6520 7468 6520 7661 6c75 6520 6f66  ase the value of
-0000af50: 2074 6869 7320 6174 7472 6962 7574 6520   this attribute 
-0000af60: 7769 6c6c 2062 6520 604e 6f6e 6560 2e0a  will be `None`..
-0000af70: 0a54 6865 2061 7474 7269 6275 7465 2060  .The attribute `
-0000af80: 7374 7265 616d 5f6e 616d 6560 2069 7320  stream_name` is 
-0000af90: 6120 5079 7468 6f6e 2060 7374 7260 206f  a Python `str` o
-0000afa0: 626a 6563 742c 2075 7365 6420 746f 2069  bject, used to i
-0000afb0: 6e64 6963 6174 6520 7468 6520 6e61 6d65  ndicate the name
-0000afc0: 206f 6620 7468 650a 7374 7265 616d 2069   of the.stream i
-0000afd0: 6e20 7768 6963 6820 7468 6520 6576 656e  n which the even
-0000afe0: 7420 7761 7320 7265 636f 7264 6564 2e0a  t was recorded..
-0000aff0: 0a54 6865 2061 7474 7269 6275 7465 2060  .The attribute `
-0000b000: 7374 7265 616d 5f70 6f73 6974 696f 6e60  stream_position`
-0000b010: 2069 7320 6120 5079 7468 6f6e 2060 696e   is a Python `in
-0000b020: 7460 2c20 7573 6564 2074 6f20 696e 6469  t`, used to indi
-0000b030: 6361 7465 2074 6865 2070 6f73 6974 696f  cate the positio
-0000b040: 6e20 696e 2074 6865 0a73 7472 6561 6d20  n in the.stream 
-0000b050: 6174 2077 6869 6368 2074 6865 2065 7665  at which the eve
-0000b060: 6e74 2077 6173 2072 6563 6f72 6465 642e  nt was recorded.
-0000b070: 0a0a 5468 6520 6174 7472 6962 7574 6520  ..The attribute 
-0000b080: 6063 6f6d 6d69 745f 706f 7369 7469 6f6e  `commit_position
-0000b090: 6020 6973 2061 2050 7974 686f 6e20 6069  ` is a Python `i
-0000b0a0: 6e74 602c 2075 7365 6420 746f 2069 6e64  nt`, used to ind
-0000b0b0: 6963 6174 6520 7468 6520 636f 6d6d 6974  icate the commit
-0000b0c0: 2070 6f73 6974 696f 6e0a 6174 2077 6869   position.at whi
-0000b0d0: 6368 2074 6865 2065 7665 6e74 2077 6173  ch the event was
-0000b0e0: 2072 6563 6f72 6465 642e 0a0a 6060 6070   recorded...```p
-0000b0f0: 7974 686f 6e0a 6672 6f6d 2065 7364 6263  ython.from esdbc
-0000b100: 6c69 656e 742e 6576 656e 7473 2069 6d70  lient.events imp
-0000b110: 6f72 7420 5265 636f 7264 6564 4576 656e  ort RecordedEven
-0000b120: 740a 0a72 6563 6f72 6465 645f 6576 656e  t..recorded_even
-0000b130: 7420 3d20 5265 636f 7264 6564 4576 656e  t = RecordedEven
-0000b140: 7428 0a20 2020 2074 7970 653d 274f 7264  t(.    type='Ord
-0000b150: 6572 4372 6561 7465 6427 2c0a 2020 2020  erCreated',.    
-0000b160: 6461 7461 3d62 277b 7d27 2c0a 2020 2020  data=b'{}',.    
-0000b170: 6d65 7461 6461 7461 3d62 2727 2c0a 2020  metadata=b'',.  
-0000b180: 2020 636f 6e74 656e 745f 7479 7065 3d27    content_type='
-0000b190: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-0000b1a0: 272c 0a20 2020 2069 643d 7575 6964 3428  ',.    id=uuid4(
-0000b1b0: 292c 0a20 2020 2073 7472 6561 6d5f 6e61  ),.    stream_na
-0000b1c0: 6d65 3d27 7374 7265 616d 3127 2c0a 2020  me='stream1',.  
-0000b1d0: 2020 7374 7265 616d 5f70 6f73 6974 696f    stream_positio
-0000b1e0: 6e3d 302c 0a20 2020 2063 6f6d 6d69 745f  n=0,.    commit_
-0000b1f0: 706f 7369 7469 6f6e 3d35 3132 2c0a 290a  position=512,.).
-0000b200: 6060 600a 0a23 2320 436f 6e74 7269 6275  ```..## Contribu
-0000b210: 746f 7273 0a0a 2323 2320 496e 7374 616c  tors..### Instal
-0000b220: 6c20 506f 6574 7279 0a0a 5468 6520 6669  l Poetry..The fi
-0000b230: 7273 7420 7468 696e 6720 6973 2074 6f20  rst thing is to 
-0000b240: 6368 6563 6b20 796f 7520 6861 7665 2050  check you have P
-0000b250: 6f65 7472 7920 696e 7374 616c 6c65 642e  oetry installed.
-0000b260: 0a0a 2020 2020 2420 706f 6574 7279 202d  ..    $ poetry -
-0000b270: 2d76 6572 7369 6f6e 0a0a 4966 2079 6f75  -version..If you
-0000b280: 2064 6f6e 2774 2c20 7468 656e 2070 6c65   don't, then ple
-0000b290: 6173 6520 5b69 6e73 7461 6c6c 2050 6f65  ase [install Poe
-0000b2a0: 7472 795d 2868 7474 7073 3a2f 2f70 7974  try](https://pyt
-0000b2b0: 686f 6e2d 706f 6574 7279 2e6f 7267 2f64  hon-poetry.org/d
-0000b2c0: 6f63 732f 2369 6e73 7461 6c6c 696e 672d  ocs/#installing-
-0000b2d0: 7769 7468 2d74 6865 2d6f 6666 6963 6961  with-the-officia
-0000b2e0: 6c2d 696e 7374 616c 6c65 7229 2e0a 0a20  l-installer)... 
-0000b2f0: 2020 2024 2063 7572 6c20 2d73 534c 2068     $ curl -sSL h
-0000b300: 7474 7073 3a2f 2f69 6e73 7461 6c6c 2e70  ttps://install.p
-0000b310: 7974 686f 6e2d 706f 6574 7279 2e6f 7267  ython-poetry.org
-0000b320: 207c 2070 7974 686f 6e33 202d 0a0a 4974   | python3 -..It
-0000b330: 2077 696c 6c20 6865 6c70 2074 6f20 6d61   will help to ma
-0000b340: 6b65 2073 7572 6520 506f 6574 7279 2773  ke sure Poetry's
-0000b350: 2062 696e 2064 6972 6563 746f 7279 2069   bin directory i
-0000b360: 7320 696e 2079 6f75 7220 6050 4154 4860  s in your `PATH`
-0000b370: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
-0000b380: 6961 626c 652e 0a0a 4275 7420 696e 2061  iable...But in a
-0000b390: 6e79 2063 6173 652c 206d 616b 6520 7375  ny case, make su
-0000b3a0: 7265 2079 6f75 206b 6e6f 7720 7468 6520  re you know the 
-0000b3b0: 7061 7468 2074 6f20 7468 6520 6070 6f65  path to the `poe
-0000b3c0: 7472 7960 2065 7865 6375 7461 626c 652e  try` executable.
-0000b3d0: 2054 6865 2050 6f65 7472 790a 696e 7374   The Poetry.inst
-0000b3e0: 616c 6c65 7220 7465 6c6c 7320 796f 7520  aller tells you 
-0000b3f0: 7768 6572 6520 6974 2068 6173 2062 6565  where it has bee
-0000b400: 6e20 696e 7374 616c 6c65 642c 2061 6e64  n installed, and
-0000b410: 2068 6f77 2074 6f20 636f 6e66 6967 7572   how to configur
-0000b420: 6520 796f 7572 2073 6865 6c6c 2e0a 0a50  e your shell...P
-0000b430: 6c65 6173 6520 7265 6665 7220 746f 2074  lease refer to t
-0000b440: 6865 205b 506f 6574 7279 2064 6f63 735d  he [Poetry docs]
-0000b450: 2868 7474 7073 3a2f 2f70 7974 686f 6e2d  (https://python-
-0000b460: 706f 6574 7279 2e6f 7267 2f64 6f63 732f  poetry.org/docs/
-0000b470: 2920 666f 7220 6775 6964 616e 6365 206f  ) for guidance o
-0000b480: 6e0a 7573 696e 6720 506f 6574 7279 2e0a  n.using Poetry..
-0000b490: 0a23 2323 2053 6574 7570 2066 6f72 2050  .### Setup for P
-0000b4a0: 7943 6861 726d 2075 7365 7273 0a0a 596f  yCharm users..Yo
-0000b4b0: 7520 6361 6e20 6561 7369 6c79 206f 6274  u can easily obt
-0000b4c0: 6169 6e20 7468 6520 7072 6f6a 6563 7420  ain the project 
-0000b4d0: 6669 6c65 7320 7573 696e 6720 5079 4368  files using PyCh
-0000b4e0: 6172 6d20 286d 656e 7520 2247 6974 203e  arm (menu "Git >
-0000b4f0: 2043 6c6f 6e65 2e2e 2e22 292e 0a50 7943   Clone...")..PyC
-0000b500: 6861 726d 2077 696c 6c20 7468 656e 2075  harm will then u
-0000b510: 7375 616c 6c79 2070 726f 6d70 7420 796f  sually prompt yo
-0000b520: 7520 746f 206f 7065 6e20 7468 6520 7072  u to open the pr
-0000b530: 6f6a 6563 742e 0a0a 4f70 656e 2074 6865  oject...Open the
-0000b540: 2070 726f 6a65 6374 2069 6e20 6120 6e65   project in a ne
-0000b550: 7720 7769 6e64 6f77 2e20 5079 4368 6172  w window. PyChar
-0000b560: 6d20 7769 6c6c 2074 6865 6e20 7573 7561  m will then usua
-0000b570: 6c6c 7920 7072 6f6d 7074 2079 6f75 2074  lly prompt you t
-0000b580: 6f20 6372 6561 7465 0a61 206e 6577 2076  o create.a new v
-0000b590: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
-0000b5a0: 6e74 2e0a 0a43 7265 6174 6520 6120 6e65  nt...Create a ne
-0000b5b0: 7720 506f 6574 7279 2076 6972 7475 616c  w Poetry virtual
-0000b5c0: 2065 6e76 6972 6f6e 6d65 6e74 2066 6f72   environment for
-0000b5d0: 2074 6865 2070 726f 6a65 6374 2e20 4966   the project. If
-0000b5e0: 2050 7943 6861 726d 2064 6f65 736e 2774   PyCharm doesn't
-0000b5f0: 2061 6c72 6561 6479 0a6b 6e6f 7720 7768   already.know wh
-0000b600: 6572 6520 796f 7572 2060 706f 6574 7279  ere your `poetry
-0000b610: 6020 6578 6563 7574 6162 6c65 2069 732c  ` executable is,
-0000b620: 2074 6865 6e20 7365 7420 7468 6520 7061   then set the pa
-0000b630: 7468 2074 6f20 796f 7572 2060 706f 6574  th to your `poet
-0000b640: 7279 6020 6578 6563 7574 6162 6c65 0a69  ry` executable.i
-0000b650: 6e20 7468 6520 224e 6577 2050 6f65 7472  n the "New Poetr
-0000b660: 7920 456e 7669 726f 6e6d 656e 7422 2066  y Environment" f
-0000b670: 6f72 6d20 696e 7075 7420 6669 656c 6420  orm input field 
-0000b680: 6c61 6265 6c6c 6564 2022 506f 6574 7279  labelled "Poetry
-0000b690: 2065 7865 6375 7461 626c 6522 2e20 496e   executable". In
-0000b6a0: 2074 6865 0a22 4e65 7720 506f 6574 7279   the."New Poetry
-0000b6b0: 2045 6e76 6972 6f6e 6d65 6e74 2220 666f   Environment" fo
-0000b6c0: 726d 2c20 796f 7520 7769 6c6c 2061 6c73  rm, you will als
-0000b6d0: 6f20 6861 7665 2074 6865 206f 7070 6f72  o have the oppor
-0000b6e0: 7475 6e69 7479 2074 6f20 7365 6c65 6374  tunity to select
-0000b6f0: 2077 6869 6368 0a50 7974 686f 6e20 6578   which.Python ex
-0000b700: 6563 7574 6162 6c65 2077 696c 6c20 6265  ecutable will be
-0000b710: 2075 7365 6420 6279 2074 6865 2076 6972   used by the vir
-0000b720: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
-0000b730: 2e0a 0a50 7943 6861 726d 2077 696c 6c20  ...PyCharm will 
-0000b740: 7468 656e 2063 7265 6174 6520 6120 6e65  then create a ne
-0000b750: 7720 506f 6574 7279 2076 6972 7475 616c  w Poetry virtual
-0000b760: 2065 6e76 6972 6f6e 6d65 6e74 2066 6f72   environment for
-0000b770: 2079 6f75 7220 7072 6f6a 6563 742c 2075   your project, u
-0000b780: 7369 6e67 0a61 2070 6172 7469 6375 6c61  sing.a particula
-0000b790: 7220 7665 7273 696f 6e20 6f66 2050 7974  r version of Pyt
-0000b7a0: 686f 6e2c 2061 6e64 2061 6c73 6f20 696e  hon, and also in
-0000b7b0: 7374 616c 6c20 696e 746f 2074 6869 7320  stall into this 
-0000b7c0: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
-0000b7d0: 656e 7420 7468 650a 7072 6f6a 6563 7427  ent the.project'
-0000b7e0: 7320 7061 636b 6167 6520 6465 7065 6e64  s package depend
-0000b7f0: 656e 6369 6573 2061 6363 6f72 6469 6e67  encies according
-0000b800: 2074 6f20 7468 6520 6070 7970 726f 6a65   to the `pyproje
-0000b810: 6374 2e74 6f6d 6c60 2066 696c 652c 206f  ct.toml` file, o
-0000b820: 7220 7468 650a 6070 6f65 7472 792e 6c6f  r the.`poetry.lo
-0000b830: 636b 6020 6669 6c65 2069 6620 7468 6174  ck` file if that
-0000b840: 2065 7869 7374 7320 696e 2074 6865 2070   exists in the p
-0000b850: 726f 6a65 6374 2066 696c 6573 2e0a 0a59  roject files...Y
-0000b860: 6f75 2063 616e 2061 6464 2064 6966 6665  ou can add diffe
-0000b870: 7265 6e74 2050 6f65 7472 7920 656e 7669  rent Poetry envi
-0000b880: 726f 6e6d 656e 7473 2066 6f72 2064 6966  ronments for dif
-0000b890: 6665 7265 6e74 2050 7974 686f 6e20 7665  ferent Python ve
-0000b8a0: 7273 696f 6e73 2c20 616e 6420 7377 6974  rsions, and swit
-0000b8b0: 6368 0a62 6574 7765 656e 2074 6865 6d20  ch.between them 
-0000b8c0: 7573 696e 6720 7468 6520 2250 7974 686f  using the "Pytho
-0000b8d0: 6e20 496e 7465 7270 7265 7465 7222 2073  n Interpreter" s
-0000b8e0: 6574 7469 6e67 7320 6f66 2050 7943 6861  ettings of PyCha
-0000b8f0: 726d 2e20 4966 2079 6f75 2077 616e 7420  rm. If you want 
-0000b900: 746f 2075 7365 0a61 2076 6572 7369 6f6e  to use.a version
-0000b910: 206f 6620 5079 7468 6f6e 2074 6861 7420   of Python that 
-0000b920: 6973 6e27 7420 696e 7374 616c 6c65 642c  isn't installed,
-0000b930: 2065 6974 6865 7220 7573 6520 796f 7572   either use your
-0000b940: 2066 6176 6f75 7269 7465 2070 6163 6b61   favourite packa
-0000b950: 6765 206d 616e 6167 6572 2c0a 6f72 2069  ge manager,.or i
-0000b960: 6e73 7461 6c6c 2050 7974 686f 6e20 6279  nstall Python by
-0000b970: 2064 6f77 6e6c 6f61 6469 6e67 2061 6e20   downloading an 
-0000b980: 696e 7374 616c 6c65 7220 666f 7220 7265  installer for re
-0000b990: 6365 6e74 2076 6572 7369 6f6e 7320 6f66  cent versions of
-0000b9a0: 2050 7974 686f 6e20 6469 7265 6374 6c79   Python directly
-0000b9b0: 0a66 726f 6d20 7468 6520 5b50 7974 686f  .from the [Pytho
-0000b9c0: 6e20 7765 6273 6974 655d 2868 7474 7073  n website](https
-0000b9d0: 3a2f 2f77 7777 2e70 7974 686f 6e2e 6f72  ://www.python.or
-0000b9e0: 672f 646f 776e 6c6f 6164 732f 292e 0a0a  g/downloads/)...
-0000b9f0: 4f6e 6365 2070 726f 6a65 6374 2064 6570  Once project dep
-0000ba00: 656e 6465 6e63 6965 7320 6861 7665 2062  endencies have b
-0000ba10: 6565 6e20 696e 7374 616c 6c65 642c 2079  een installed, y
-0000ba20: 6f75 2073 686f 756c 6420 6265 2061 626c  ou should be abl
-0000ba30: 6520 746f 2072 756e 2074 6573 7473 0a66  e to run tests.f
-0000ba40: 726f 6d20 7769 7468 696e 2050 7943 6861  rom within PyCha
-0000ba50: 726d 2028 7269 6768 742d 636c 6963 6b20  rm (right-click 
-0000ba60: 6f6e 2074 6865 2060 7465 7374 7360 2066  on the `tests` f
-0000ba70: 6f6c 6465 7220 616e 6420 7365 6c65 6374  older and select
-0000ba80: 2074 6865 2027 5275 6e27 206f 7074 696f   the 'Run' optio
-0000ba90: 6e29 2e0a 0a42 6563 6175 7365 206f 6620  n)...Because of 
-0000baa0: 6120 636f 6e66 6c69 6374 2062 6574 7765  a conflict betwe
-0000bab0: 656e 2070 7974 6573 7420 616e 6420 5079  en pytest and Py
-0000bac0: 4368 6172 6d27 7320 6465 6275 6767 6572  Charm's debugger
-0000bad0: 2061 6e64 2074 6865 2063 6f76 6572 6167   and the coverag
-0000bae0: 6520 746f 6f6c 2c0a 796f 7520 6d61 7920  e tool,.you may 
-0000baf0: 6e65 6564 2074 6f20 6164 6420 6060 2d2d  need to add ``--
-0000bb00: 6e6f 2d63 6f76 6060 2061 7320 616e 206f  no-cov`` as an o
-0000bb10: 7074 696f 6e20 746f 2074 6865 2074 6573  ption to the tes
-0000bb20: 7420 7275 6e6e 6572 2074 656d 706c 6174  t runner templat
-0000bb30: 652e 2041 6c74 6572 6e61 7469 7665 6c79  e. Alternatively
-0000bb40: 2c0a 6a75 7374 2075 7365 2074 6865 2050  ,.just use the P
-0000bb50: 7974 686f 6e20 5374 616e 6461 7264 204c  ython Standard L
-0000bb60: 6962 7261 7279 2773 2060 6075 6e69 7474  ibrary's ``unitt
-0000bb70: 6573 7460 6020 6d6f 6475 6c65 2e0a 0a59  est`` module...Y
-0000bb80: 6f75 2073 686f 756c 6420 616c 736f 2062  ou should also b
-0000bb90: 6520 6162 6c65 2074 6f20 6f70 656e 2061  e able to open a
-0000bba0: 2074 6572 6d69 6e61 6c20 7769 6e64 6f77   terminal window
-0000bbb0: 2069 6e20 5079 4368 6172 6d2c 2061 6e64   in PyCharm, and
-0000bbc0: 2072 756e 2074 6865 2070 726f 6a65 6374   run the project
-0000bbd0: 2773 0a4d 616b 6566 696c 6520 636f 6d6d  's.Makefile comm
-0000bbe0: 616e 6473 2066 726f 6d20 7468 6520 636f  ands from the co
-0000bbf0: 6d6d 616e 6420 6c69 6e65 2028 7365 6520  mmand line (see 
-0000bc00: 6265 6c6f 7729 2e0a 0a23 2323 2053 6574  below)...### Set
-0000bc10: 7570 2066 726f 6d20 636f 6d6d 616e 6420  up from command 
-0000bc20: 6c69 6e65 0a0a 4f62 7461 696e 2074 6865  line..Obtain the
-0000bc30: 2070 726f 6a65 6374 2066 696c 6573 2c20   project files, 
-0000bc40: 7573 696e 6720 4769 7420 6f72 2073 7569  using Git or sui
-0000bc50: 7461 626c 6520 616c 7465 726e 6174 6976  table alternativ
-0000bc60: 652e 0a0a 496e 2061 2074 6572 6d69 6e61  e...In a termina
-0000bc70: 6c20 6170 706c 6963 6174 696f 6e2c 2063  l application, c
-0000bc80: 6861 6e67 6520 796f 7572 2063 7572 7265  hange your curre
-0000bc90: 6e74 2077 6f72 6b69 6e67 2064 6972 6563  nt working direc
-0000bca0: 746f 7279 0a74 6f20 7468 6520 726f 6f74  tory.to the root
-0000bcb0: 2066 6f6c 6465 7220 6f66 2074 6865 2070   folder of the p
-0000bcc0: 726f 6a65 6374 2066 696c 6573 2e20 5468  roject files. Th
-0000bcd0: 6572 6520 7368 6f75 6c64 2062 6520 6120  ere should be a 
-0000bce0: 4d61 6b65 6669 6c65 0a69 6e20 7468 6973  Makefile.in this
-0000bcf0: 2066 6f6c 6465 722e 0a0a 5573 6520 7468   folder...Use th
-0000bd00: 6520 4d61 6b65 6669 6c65 2074 6f20 6372  e Makefile to cr
-0000bd10: 6561 7465 2061 206e 6577 2050 6f65 7472  eate a new Poetr
-0000bd20: 7920 7669 7274 7561 6c20 656e 7669 726f  y virtual enviro
-0000bd30: 6e6d 656e 7420 666f 7220 7468 650a 7072  nment for the.pr
-0000bd40: 6f6a 6563 7420 616e 6420 696e 7374 616c  oject and instal
-0000bd50: 6c20 7468 6520 7072 6f6a 6563 7427 7320  l the project's 
-0000bd60: 7061 636b 6167 6520 6465 7065 6e64 656e  package dependen
-0000bd70: 6369 6573 2069 6e74 6f20 6974 2c0a 7573  cies into it,.us
-0000bd80: 696e 6720 7468 6520 666f 6c6c 6f77 696e  ing the followin
-0000bd90: 6720 636f 6d6d 616e 642e 0a0a 2020 2020  g command...    
-0000bda0: 2420 6d61 6b65 2069 6e73 7461 6c6c 2d70  $ make install-p
-0000bdb0: 6163 6b61 6765 730a 0a49 7427 7320 616c  ackages..It's al
-0000bdc0: 736f 2070 6f73 7369 626c 6520 746f 2061  so possible to a
-0000bdd0: 6c73 6f20 696e 7374 616c 6c20 7468 6520  lso install the 
-0000bde0: 7072 6f6a 6563 7420 696e 2027 6564 6974  project in 'edit
-0000bdf0: 6162 6c65 206d 6f64 6527 2e0a 0a20 2020  able mode'...   
-0000be00: 2024 206d 616b 6520 696e 7374 616c 6c0a   $ make install.
-0000be10: 0a50 6c65 6173 6520 6e6f 7465 2c20 6966  .Please note, if
-0000be20: 2079 6f75 2063 7265 6174 6520 7468 6520   you create the 
-0000be30: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
-0000be40: 656e 7420 696e 2074 6869 7320 7761 792c  ent in this way,
-0000be50: 2061 6e64 2074 6865 6e20 7472 7920 746f   and then try to
-0000be60: 0a6f 7065 6e20 7468 6520 7072 6f6a 6563  .open the projec
-0000be70: 7420 696e 2050 7943 6861 726d 2061 6e64  t in PyCharm and
-0000be80: 2063 6f6e 6669 6775 7265 2074 6865 2070   configure the p
-0000be90: 726f 6a65 6374 2074 6f20 7573 6520 7468  roject to use th
-0000bea0: 6973 2076 6972 7475 616c 0a65 6e76 6972  is virtual.envir
-0000beb0: 6f6e 6d65 6e74 2061 7320 616e 2022 4578  onment as an "Ex
-0000bec0: 6973 7469 6e67 2050 6f65 7472 7920 456e  isting Poetry En
-0000bed0: 7669 726f 6e6d 656e 7422 2c20 5079 4368  vironment", PyCh
-0000bee0: 6172 6d20 736f 6d65 7469 6d65 7320 6861  arm sometimes ha
-0000bef0: 7320 736f 6d65 0a69 7373 7565 7320 2864  s some.issues (d
-0000bf00: 6f6e 2774 206b 6e6f 7720 7768 7929 2077  on't know why) w
-0000bf10: 6869 6368 206d 6967 6874 2062 6520 7072  hich might be pr
-0000bf20: 6f62 6c65 6d61 7469 632e 2049 6620 796f  oblematic. If yo
-0000bf30: 7520 656e 636f 756e 7465 7220 7375 6368  u encounter such
-0000bf40: 0a69 7373 7565 732c 2079 6f75 2063 616e  .issues, you can
-0000bf50: 2072 6573 6f6c 7665 2074 6865 7365 2069   resolve these i
-0000bf60: 7373 7565 7320 6279 2064 656c 6574 696e  ssues by deletin
-0000bf70: 6720 7468 6520 7669 7274 7561 6c20 656e  g the virtual en
-0000bf80: 7669 726f 6e6d 656e 740a 616e 6420 6372  vironment.and cr
-0000bf90: 6561 7469 6e67 2074 6865 2050 6f65 7472  eating the Poetr
-0000bfa0: 7920 7669 7274 7561 6c20 656e 7669 726f  y virtual enviro
-0000bfb0: 6e6d 656e 7420 7573 696e 6720 5079 4368  nment using PyCh
-0000bfc0: 6172 6d20 2873 6565 2061 626f 7665 292e  arm (see above).
-0000bfd0: 0a0a 2323 2320 5072 6f6a 6563 7420 4d61  ..### Project Ma
-0000bfe0: 6b65 6669 6c65 2063 6f6d 6d61 6e64 730a  kefile commands.
-0000bff0: 0a59 6f75 2063 616e 2073 7461 7274 2045  .You can start E
-0000c000: 7665 6e74 5374 6f72 6544 4220 7573 696e  ventStoreDB usin
-0000c010: 6720 7468 6520 666f 6c6c 6f77 696e 6720  g the following 
-0000c020: 636f 6d6d 616e 642e 0a0a 2020 2020 2420  command...    $ 
-0000c030: 6d61 6b65 2073 7461 7274 2d65 7665 6e74  make start-event
-0000c040: 7374 6f72 6564 620a 0a59 6f75 2063 616e  storedb..You can
-0000c050: 2072 756e 2074 6573 7473 2075 7369 6e67   run tests using
-0000c060: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-0000c070: 6f6d 6d61 6e64 2028 6e65 6564 7320 4576  ommand (needs Ev
-0000c080: 656e 7453 746f 7265 4442 2074 6f20 6265  entStoreDB to be
-0000c090: 2072 756e 6e69 6e67 292e 0a0a 2020 2020   running)...    
-0000c0a0: 2420 6d61 6b65 2074 6573 740a 0a59 6f75  $ make test..You
-0000c0b0: 2063 616e 2073 746f 7020 4576 656e 7453   can stop EventS
-0000c0c0: 746f 7265 4442 2075 7369 6e67 2074 6865  toreDB using the
-0000c0d0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-0000c0e0: 6e64 2e0a 0a20 2020 2024 206d 616b 6520  nd...    $ make 
-0000c0f0: 7374 6f70 2d65 7665 6e74 7374 6f72 6564  stop-eventstored
-0000c100: 620a 0a59 6f75 2063 616e 2063 6865 636b  b..You can check
-0000c110: 2074 6865 2066 6f72 6d61 7474 696e 6720   the formatting 
-0000c120: 6f66 2074 6865 2063 6f64 6520 7573 696e  of the code usin
-0000c130: 6720 7468 6520 666f 6c6c 6f77 696e 6720  g the following 
-0000c140: 636f 6d6d 616e 642e 0a0a 2020 2020 2420  command...    $ 
-0000c150: 6d61 6b65 206c 696e 740a 0a59 6f75 2063  make lint..You c
-0000c160: 616e 2072 6566 6f72 6d61 7420 7468 6520  an reformat the 
-0000c170: 636f 6465 2075 7369 6e67 2074 6865 2066  code using the f
-0000c180: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-0000c190: 2e0a 0a20 2020 2024 206d 616b 6520 666d  ...    $ make fm
-0000c1a0: 740a 0a54 6573 7473 2062 656c 6f6e 6720  t..Tests belong 
-0000c1b0: 696e 2060 2e2f 7465 7374 7360 2e20 436f  in `./tests`. Co
-0000c1c0: 6465 2d75 6e64 6572 2d74 6573 7420 6265  de-under-test be
-0000c1d0: 6c6f 6e67 7320 696e 2060 2e2f 6573 6462  longs in `./esdb
-0000c1e0: 636c 6965 6e74 602e 0a0a 4564 6974 2070  client`...Edit p
-0000c1f0: 6163 6b61 6765 2064 6570 656e 6465 6e63  ackage dependenc
-0000c200: 6965 7320 696e 2060 7079 7072 6f6a 6563  ies in `pyprojec
-0000c210: 742e 746f 6d6c 602e 2055 7064 6174 6520  t.toml`. Update 
-0000c220: 696e 7374 616c 6c65 6420 7061 636b 6167  installed packag
-0000c230: 6573 2028 616e 6420 7468 650a 6070 6f65  es (and the.`poe
-0000c240: 7472 792e 6c6f 636b 6020 6669 6c65 2920  try.lock` file) 
-0000c250: 7573 696e 6720 7468 6520 666f 6c6c 6f77  using the follow
-0000c260: 696e 6720 636f 6d6d 616e 642e 0a0a 2020  ing command...  
-0000c270: 2020 2420 6d61 6b65 2075 7064 6174 652d    $ make update-
-0000c280: 7061 636b 6167 6573 0a0a                 packages..
+00000030: 312e 3061 310a 5375 6d6d 6172 793a 2050  1.0a1.Summary: P
+00000040: 7974 686f 6e20 6752 5043 2043 6c69 656e  ython gRPC Clien
+00000050: 7420 666f 7220 4576 656e 7453 746f 7265  t for EventStore
+00000060: 4442 0a48 6f6d 652d 7061 6765 3a20 6874  DB.Home-page: ht
+00000070: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000080: 2f70 7965 7665 6e74 736f 7572 6369 6e67  /pyeventsourcing
+00000090: 2f65 7364 6263 6c69 656e 740a 4c69 6365  /esdbclient.Lice
+000000a0: 6e73 653a 2042 5344 2033 2d43 6c61 7573  nse: BSD 3-Claus
+000000b0: 650a 4175 7468 6f72 3a20 4a6f 686e 2042  e.Author: John B
+000000c0: 7977 6174 6572 0a41 7574 686f 722d 656d  ywater.Author-em
+000000d0: 6169 6c3a 206a 6f68 6e2e 6279 7761 7465  ail: john.bywate
+000000e0: 7240 6170 7072 6f70 7269 6174 6573 6f66  r@appropriatesof
+000000f0: 7477 6172 652e 6e65 740a 5265 7175 6972  tware.net.Requir
+00000100: 6573 2d50 7974 686f 6e3a 203e 3d33 2e37  es-Python: >=3.7
+00000110: 2c3c 342e 300a 436c 6173 7369 6669 6572  ,<4.0.Classifier
+00000120: 3a20 4465 7665 6c6f 706d 656e 7420 5374  : Development St
+00000130: 6174 7573 203a 3a20 3320 2d20 416c 7068  atus :: 3 - Alph
+00000140: 610a 436c 6173 7369 6669 6572 3a20 4c69  a.Classifier: Li
+00000150: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000160: 726f 7665 6420 3a3a 2042 5344 204c 6963  roved :: BSD Lic
+00000170: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
+00000180: 204c 6963 656e 7365 203a 3a20 4f74 6865   License :: Othe
+00000190: 722f 5072 6f70 7269 6574 6172 7920 4c69  r/Proprietary Li
+000001a0: 6365 6e73 650a 436c 6173 7369 6669 6572  cense.Classifier
+000001b0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000001c0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001d0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000001e0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001f0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000200: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000210: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000220: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000230: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
+00000240: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000250: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000260: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
+00000270: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000280: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000290: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
+000002a0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000002b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002c0: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
+000002d0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000002e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000002f0: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
+00000300: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000310: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000320: 2050 7974 686f 6e20 3a3a 2033 0a43 6c61   Python :: 3.Cla
+00000330: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000340: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000350: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+00000360: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000370: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000380: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000390: 3131 0a43 6c61 7373 6966 6965 723a 2050  11.Classifier: P
+000003a0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000003b0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000003c0: 2033 2e37 0a43 6c61 7373 6966 6965 723a   3.7.Classifier:
+000003d0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+000003e0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000003f0: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
+00000400: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000410: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000420: 6e20 3a3a 2033 2e39 0a52 6571 7569 7265  n :: 3.9.Require
+00000430: 732d 4469 7374 3a20 646e 7370 7974 686f  s-Dist: dnspytho
+00000440: 6e20 283e 3d32 2e33 2e30 2c3c 332e 302e  n (>=2.3.0,<3.0.
+00000450: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000460: 3a20 6772 7063 696f 2028 3e3d 312e 3531  : grpcio (>=1.51
+00000470: 2e30 2c21 3d31 2e35 322e 2a29 0a52 6571  .0,!=1.52.*).Req
+00000480: 7569 7265 732d 4469 7374 3a20 7072 6f74  uires-Dist: prot
+00000490: 6f62 7566 2028 3e3d 332e 3131 2e30 290a  obuf (>=3.11.0).
+000004a0: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+000004b0: 7970 696e 675f 6578 7465 6e73 696f 6e73  yping_extensions
+000004c0: 0a50 726f 6a65 6374 2d55 524c 3a20 5265  .Project-URL: Re
+000004d0: 706f 7369 746f 7279 2c20 6874 7470 733a  pository, https:
+000004e0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7965  //github.com/pye
+000004f0: 7665 6e74 736f 7572 6369 6e67 2f65 7364  ventsourcing/esd
+00000500: 6263 6c69 656e 740a 4465 7363 7269 7074  bclient.Descript
+00000510: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
+00000520: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
+00000530: 0a23 2050 7974 686f 6e20 6752 5043 2043  .# Python gRPC C
+00000540: 6c69 656e 7420 666f 7220 4576 656e 7453  lient for EventS
+00000550: 746f 7265 4442 0a0a 5468 6973 205b 5079  toreDB..This [Py
+00000560: 7468 6f6e 2070 6163 6b61 6765 5d28 6874  thon package](ht
+00000570: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000580: 726f 6a65 6374 2f65 7364 6263 6c69 656e  roject/esdbclien
+00000590: 742f 2920 7072 6f76 6964 6573 2061 2050  t/) provides a P
+000005a0: 7974 686f 6e0a 6752 5043 2063 6c69 656e  ython.gRPC clien
+000005b0: 7420 666f 7220 5b45 7665 6e74 5374 6f72  t for [EventStor
+000005c0: 6544 425d 2868 7474 7073 3a2f 2f77 7777  eDB](https://www
+000005d0: 2e65 7665 6e74 7374 6f72 652e 636f 6d2f  .eventstore.com/
+000005e0: 292e 0a0a 5468 6973 2063 6c69 656e 7420  )...This client 
+000005f0: 6861 7320 6265 656e 2064 6576 656c 6f70  has been develop
+00000600: 6564 2069 6e20 636f 6c6c 6162 6f72 6174  ed in collaborat
+00000610: 696f 6e20 7769 7468 2074 6865 2045 7665  ion with the Eve
+00000620: 6e74 5374 6f72 6544 420a 7465 616d 2e20  ntStoreDB.team. 
+00000630: 416c 7468 6f75 6768 206e 6f74 2061 6c6c  Although not all
+00000640: 2074 6865 2066 6561 7475 7265 7320 6f66   the features of
+00000650: 2045 7665 6e74 5374 6f72 6544 4220 6172   EventStoreDB ar
+00000660: 6520 7375 7070 6f72 7465 640a 6279 2074  e supported.by t
+00000670: 6869 7320 636c 6965 6e74 2c20 6d61 6e79  his client, many
+00000680: 206f 6620 7468 6520 6d6f 7374 2075 7365   of the most use
+00000690: 6675 6c20 6f6e 6573 2061 7265 2070 7265  ful ones are pre
+000006a0: 7365 6e74 6564 0a69 6e20 616e 2065 6173  sented.in an eas
+000006b0: 792d 746f 2d75 7365 2069 6e74 6572 6661  y-to-use interfa
+000006c0: 6365 2e0a 0a54 6869 7320 636c 6965 6e74  ce...This client
+000006d0: 2068 6173 2062 6565 6e20 7465 7374 6564   has been tested
+000006e0: 2074 6f20 776f 726b 2077 6974 6820 4576   to work with Ev
+000006f0: 656e 7453 746f 7265 4442 204c 5453 2076  entStoreDB LTS v
+00000700: 6572 7369 6f6e 7320 3231 2e31 302c 0a77  ersions 21.10,.w
+00000710: 6974 686f 7574 2061 6e64 2077 6974 686f  ithout and witho
+00000720: 7574 2053 534c 2f54 4c53 2c20 616e 6420  ut SSL/TLS, and 
+00000730: 7769 7468 2050 7974 686f 6e20 7665 7273  with Python vers
+00000740: 696f 6e73 2033 2e37 2074 6f20 332e 3131  ions 3.7 to 3.11
+00000750: 2e20 5468 6572 650a 6973 2031 3030 2520  . There.is 100% 
+00000760: 7465 7374 2063 6f76 6572 6167 652e 2054  test coverage. T
+00000770: 6865 2063 6f64 6520 6861 7320 7479 7069  he code has typi
+00000780: 6e67 2061 6e6e 6f74 6174 696f 6e73 2c20  ng annotations, 
+00000790: 6368 6563 6b65 6420 7769 7468 206d 7970  checked with myp
+000007a0: 792e 0a54 6865 2063 6f64 6520 6973 2066  y..The code is f
+000007b0: 6f72 6d61 7474 6564 2077 6974 6820 626c  ormatted with bl
+000007c0: 6163 6b20 616e 6420 6973 6f72 742c 2061  ack and isort, a
+000007d0: 6e64 2063 6865 636b 6564 2077 6974 6820  nd checked with 
+000007e0: 666c 616b 6538 2e20 506f 6574 7279 0a69  flake8. Poetry.i
+000007f0: 7320 7573 6564 2066 6f72 2070 6163 6b61  s used for packa
+00000800: 6765 206d 616e 6167 656d 656e 7420 6475  ge management du
+00000810: 7269 6e67 2064 6576 656c 6f70 6d65 6e74  ring development
+00000820: 2c20 616e 6420 666f 7220 6275 696c 6469  , and for buildi
+00000830: 6e67 2061 6e64 0a70 7562 6c69 7368 696e  ng and.publishin
+00000840: 6720 6469 7374 7269 6275 7469 6f6e 7320  g distributions 
+00000850: 746f 205b 5079 5049 5d28 6874 7470 733a  to [PyPI](https:
+00000860: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000870: 6374 2f65 7364 6263 6c69 656e 742f 292e  ct/esdbclient/).
+00000880: 0a0a 2323 2053 796e 6f70 7369 730a 0a54  ..## Synopsis..T
+00000890: 6865 2060 4553 4442 436c 6965 6e74 6020  he `ESDBClient` 
+000008a0: 636c 6173 7320 6361 6e20 6265 2069 6d70  class can be imp
+000008b0: 6f72 7465 6420 6672 6f6d 2074 6865 2060  orted from the `
+000008c0: 6573 6462 636c 6965 6e74 6020 7061 636b  esdbclient` pack
+000008d0: 6167 652e 0a0a 546f 2072 756e 2074 6865  age...To run the
+000008e0: 2063 6c69 656e 742c 2079 6f75 2077 696c   client, you wil
+000008f0: 6c20 6e65 6564 2061 2063 6f6e 6e65 6374  l need a connect
+00000900: 696f 6e20 7374 7269 6e67 2055 5249 2e20  ion string URI. 
+00000910: 416e 642c 2074 6f0a 636f 6e6e 6563 7420  And, to.connect 
+00000920: 746f 2061 2022 7365 6375 7265 2220 4576  to a "secure" Ev
+00000930: 656e 7453 746f 7265 4442 2073 6572 7665  entStoreDB serve
+00000940: 722c 2079 6f75 2077 696c 6c20 616c 736f  r, you will also
+00000950: 206e 6565 6420 616e 0a53 534c 2f54 4c53   need an.SSL/TLS
+00000960: 2063 6572 7469 6669 6361 7465 2e0a 0a50   certificate...P
+00000970: 726f 6261 626c 7920 7468 6520 7468 7265  robably the thre
+00000980: 6520 6d6f 7374 2075 7365 6675 6c20 6d65  e most useful me
+00000990: 7468 6f64 7320 6f66 2060 4553 4442 436c  thods of `ESDBCl
+000009a0: 6965 6e74 6020 6172 653a 0a0a 2a20 6061  ient` are:..* `a
+000009b0: 7070 656e 645f 6576 656e 7473 2829 6020  ppend_events()` 
+000009c0: 5468 6973 206d 6574 686f 6420 6361 6e20  This method can 
+000009d0: 6265 2075 7365 6420 746f 2072 6563 6f72  be used to recor
+000009e0: 640a 6576 656e 7473 2069 6e20 6120 7061  d.events in a pa
+000009f0: 7274 6963 756c 6172 2022 7374 7265 616d  rticular "stream
+00000a00: 222e 2054 6869 7320 6973 2075 7365 6675  ". This is usefu
+00000a10: 6c20 7768 656e 2065 7865 6375 7469 6e67  l when executing
+00000a20: 2061 2063 6f6d 6d61 6e64 0a69 6e20 616e   a command.in an
+00000a30: 2061 7070 6c69 6361 7469 6f6e 2e20 4569   application. Ei
+00000a40: 7468 6572 2061 6c6c 206f 7220 6e6f 6e65  ther all or none
+00000a50: 206f 6620 7468 6520 6576 656e 7473 2077   of the events w
+00000a60: 696c 6c20 6265 2072 6563 6f72 6465 642e  ill be recorded.
+00000a70: 0a0a 2a20 6072 6561 645f 7374 7265 616d  ..* `read_stream
+00000a80: 5f65 7665 6e74 7328 2960 2054 6869 7320  _events()` This 
+00000a90: 6d65 7468 6f64 2063 616e 2062 6520 7573  method can be us
+00000aa0: 6564 2074 6f20 7265 7472 6965 7665 2061  ed to retrieve a
+00000ab0: 6c6c 2074 6865 2072 6563 6f72 6465 640a  ll the recorded.
+00000ac0: 6576 656e 7473 2069 6e20 6120 2273 7472  events in a "str
+00000ad0: 6561 6d22 2e20 5468 6973 2069 7320 7573  eam". This is us
+00000ae0: 6566 756c 2066 6f72 2072 6563 6f6e 7374  eful for reconst
+00000af0: 7275 6374 696e 6720 616e 2061 6767 7265  ructing an aggre
+00000b00: 6761 7465 2062 6566 6f72 650a 6578 6563  gate before.exec
+00000b10: 7574 696e 6720 6120 636f 6d6d 616e 6420  uting a command 
+00000b20: 696e 2061 6e20 6170 706c 6963 6174 696f  in an applicatio
+00000b30: 6e2e 0a0a 2a20 6073 7562 7363 7269 6265  n...* `subscribe
+00000b40: 5f61 6c6c 5f65 7665 6e74 7328 2960 2054  _all_events()` T
+00000b50: 6869 7320 6d65 7468 6f64 2063 616e 2062  his method can b
+00000b60: 6520 7573 6564 2074 6f20 7265 6365 6976  e used to receiv
+00000b70: 6520 616c 6c20 7265 636f 7264 6564 0a65  e all recorded.e
+00000b80: 7665 6e74 7320 6163 726f 7373 2061 6c6c  vents across all
+00000b90: 2022 7374 7265 616d 7322 2e20 5468 6973   "streams". This
+00000ba0: 2069 7320 7573 6566 756c 2069 6e20 6576   is useful in ev
+00000bb0: 656e 742d 7072 6f63 6573 7369 6e67 2063  ent-processing c
+00000bc0: 6f6d 706f 6e65 6e74 732c 0a61 6e64 2073  omponents,.and s
+00000bd0: 7570 706f 7274 7320 7072 6f63 6573 7369  upports processi
+00000be0: 6e67 2065 7665 6e74 7320 7769 7468 2022  ng events with "
+00000bf0: 6578 6163 746c 792d 6f6e 6365 2220 7365  exactly-once" se
+00000c00: 6d61 6e74 6963 732e 0a0a 5468 6520 6578  mantics...The ex
+00000c10: 616d 706c 6520 6265 6c6f 7720 7573 6573  ample below uses
+00000c20: 2061 6e20 2269 6e73 6563 7572 6522 2045   an "insecure" E
+00000c30: 7665 6e74 5374 6f72 6544 4220 7365 7276  ventStoreDB serv
+00000c40: 6572 2072 756e 6e69 6e67 206c 6f63 616c  er running local
+00000c50: 6c79 206f 6e20 706f 7274 2032 3131 342e  ly on port 2114.
+00000c60: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00000c70: 7274 2065 7364 6263 6c69 656e 742c 2075  rt esdbclient, u
+00000c80: 7569 640a 0a0a 2320 436f 6e73 7472 7563  uid...# Construc
+00000c90: 7420 4553 4442 436c 6965 6e74 2077 6974  t ESDBClient wit
+00000ca0: 6820 616e 2045 7665 6e74 5374 6f72 6544  h an EventStoreD
+00000cb0: 4220 5552 492e 0a0a 636c 6965 6e74 203d  B URI...client =
+00000cc0: 2065 7364 6263 6c69 656e 742e 4553 4442   esdbclient.ESDB
+00000cd0: 436c 6965 6e74 2875 7269 3d22 6573 6462  Client(uri="esdb
+00000ce0: 3a2f 2f6c 6f63 616c 686f 7374 3a32 3131  ://localhost:211
+00000cf0: 343f 546c 733d 6661 6c73 6522 290a 0a0a  4?Tls=false")...
+00000d00: 2320 4170 7065 6e64 2065 7665 6e74 7320  # Append events 
+00000d10: 746f 2061 206e 6577 2073 7472 6561 6d2e  to a new stream.
+00000d20: 0a0a 7374 7265 616d 5f6e 616d 6520 3d20  ..stream_name = 
+00000d30: 7374 7228 7575 6964 2e75 7569 6434 2829  str(uuid.uuid4()
+00000d40: 290a 0a65 7665 6e74 3120 3d20 6573 6462  )..event1 = esdb
+00000d50: 636c 6965 6e74 2e4e 6577 4576 656e 7428  client.NewEvent(
+00000d60: 7479 7065 3d27 4f72 6465 7243 7265 6174  type='OrderCreat
+00000d70: 6564 272c 2064 6174 613d 6227 6461 7461  ed', data=b'data
+00000d80: 3127 290a 0a63 6c69 656e 742e 6170 7065  1')..client.appe
+00000d90: 6e64 5f65 7665 6e74 7328 0a20 2020 2073  nd_events(.    s
+00000da0: 7472 6561 6d5f 6e61 6d65 3d73 7472 6561  tream_name=strea
+00000db0: 6d5f 6e61 6d65 2c0a 2020 2020 6578 7065  m_name,.    expe
+00000dc0: 6374 6564 5f70 6f73 6974 696f 6e3d 4e6f  cted_position=No
+00000dd0: 6e65 2c0a 2020 2020 6576 656e 7473 3d5b  ne,.    events=[
+00000de0: 6576 656e 7431 5d2c 0a29 0a0a 0a23 2041  event1],.)...# A
+00000df0: 7070 656e 6420 6d6f 7265 2065 7665 6e74  ppend more event
+00000e00: 7320 746f 2061 6e20 6578 6973 7469 6e67  s to an existing
+00000e10: 2073 7472 6561 6d2e 0a0a 6576 656e 7432   stream...event2
+00000e20: 203d 2065 7364 6263 6c69 656e 742e 4e65   = esdbclient.Ne
+00000e30: 7745 7665 6e74 2874 7970 653d 274f 7264  wEvent(type='Ord
+00000e40: 6572 5570 6461 7465 6427 2c20 6461 7461  erUpdated', data
+00000e50: 3d62 2764 6174 6132 2729 0a65 7665 6e74  =b'data2').event
+00000e60: 3320 3d20 6573 6462 636c 6965 6e74 2e4e  3 = esdbclient.N
+00000e70: 6577 4576 656e 7428 7479 7065 3d27 4f72  ewEvent(type='Or
+00000e80: 6465 7244 656c 6574 6564 272c 2064 6174  derDeleted', dat
+00000e90: 613d 6227 6461 7461 3327 290a 0a63 6c69  a=b'data3')..cli
+00000ea0: 656e 742e 6170 7065 6e64 5f65 7665 6e74  ent.append_event
+00000eb0: 7328 0a20 2020 2073 7472 6561 6d5f 6e61  s(.    stream_na
+00000ec0: 6d65 3d73 7472 6561 6d5f 6e61 6d65 2c0a  me=stream_name,.
+00000ed0: 2020 2020 6578 7065 6374 6564 5f70 6f73      expected_pos
+00000ee0: 6974 696f 6e3d 302c 0a20 2020 2065 7665  ition=0,.    eve
+00000ef0: 6e74 733d 5b65 7665 6e74 322c 2065 7665  nts=[event2, eve
+00000f00: 6e74 335d 2c0a 290a 0a0a 2320 5265 6164  nt3],.)...# Read
+00000f10: 2061 6c6c 2065 7665 6e74 7320 7265 636f   all events reco
+00000f20: 7264 6564 2069 6e20 6120 7374 7265 616d  rded in a stream
+00000f30: 2e0a 0a72 6563 6f72 6465 6420 3d20 6c69  ...recorded = li
+00000f40: 7374 280a 2020 2020 636c 6965 6e74 2e72  st(.    client.r
+00000f50: 6561 645f 7374 7265 616d 5f65 7665 6e74  ead_stream_event
+00000f60: 7328 0a20 2020 2020 2020 2073 7472 6561  s(.        strea
+00000f70: 6d5f 6e61 6d65 3d73 7472 6561 6d5f 6e61  m_name=stream_na
+00000f80: 6d65 0a20 2020 2029 0a29 0a0a 6173 7365  me.    ).)..asse
+00000f90: 7274 206c 656e 2872 6563 6f72 6465 6429  rt len(recorded)
+00000fa0: 203d 3d20 330a 6173 7365 7274 2072 6563   == 3.assert rec
+00000fb0: 6f72 6465 645b 305d 2e64 6174 6120 3d3d  orded[0].data ==
+00000fc0: 2065 7665 6e74 312e 6461 7461 0a61 7373   event1.data.ass
+00000fd0: 6572 7420 7265 636f 7264 6564 5b31 5d2e  ert recorded[1].
+00000fe0: 6461 7461 203d 3d20 6576 656e 7432 2e64  data == event2.d
+00000ff0: 6174 610a 6173 7365 7274 2072 6563 6f72  ata.assert recor
+00001000: 6465 645b 325d 2e64 6174 6120 3d3d 2065  ded[2].data == e
+00001010: 7665 6e74 332e 6461 7461 0a61 7373 6572  vent3.data.asser
+00001020: 7420 7265 636f 7264 6564 5b30 5d2e 7479  t recorded[0].ty
+00001030: 7065 203d 3d20 6576 656e 7431 2e74 7970  pe == event1.typ
+00001040: 650a 6173 7365 7274 2072 6563 6f72 6465  e.assert recorde
+00001050: 645b 315d 2e74 7970 6520 3d3d 2065 7665  d[1].type == eve
+00001060: 6e74 322e 7479 7065 0a61 7373 6572 7420  nt2.type.assert 
+00001070: 7265 636f 7264 6564 5b32 5d2e 7479 7065  recorded[2].type
+00001080: 203d 3d20 6576 656e 7433 2e74 7970 650a   == event3.type.
+00001090: 0a0a 2320 496e 2061 6e20 6576 656e 742d  ..# In an event-
+000010a0: 7072 6f63 6573 7369 6e67 2063 6f6d 706f  processing compo
+000010b0: 6e65 6e74 2c20 7573 6520 6120 2263 6174  nent, use a "cat
+000010c0: 6368 2d75 7022 2073 7562 7363 7269 7074  ch-up" subscript
+000010d0: 696f 6e0a 2320 746f 2072 6563 6569 7665  ion.# to receive
+000010e0: 2061 6c6c 2065 7665 6e74 7320 6163 726f   all events acro
+000010f0: 7373 2061 6c6c 2073 7472 6561 6d73 2c20  ss all streams, 
+00001100: 696e 636c 7564 696e 6720 6576 656e 7473  including events
+00001110: 2074 6861 740a 2320 6861 7665 206e 6f74   that.# have not
+00001120: 2079 6574 2062 6565 6e20 7265 636f 7264   yet been record
+00001130: 6564 2c20 7374 6172 7469 6e67 2066 726f  ed, starting fro
+00001140: 6d20 7468 6520 636f 6d70 6f6e 656e 7427  m the component'
+00001150: 7320 6c61 7374 0a23 2073 6176 6564 2022  s last.# saved "
+00001160: 636f 6d6d 6974 2070 6f73 6974 696f 6e22  commit position"
+00001170: 2e0a 0a6c 6173 745f 7361 7665 645f 636f  ...last_saved_co
+00001180: 6d6d 6974 5f70 6f73 6974 696f 6e20 3d20  mmit_position = 
+00001190: 300a 0a73 7562 7363 7269 7074 696f 6e20  0..subscription 
+000011a0: 3d20 636c 6965 6e74 2e73 7562 7363 7269  = client.subscri
+000011b0: 6265 5f61 6c6c 5f65 7665 6e74 7328 0a20  be_all_events(. 
+000011c0: 2020 2063 6f6d 6d69 745f 706f 7369 7469     commit_positi
+000011d0: 6f6e 3d6c 6173 745f 7361 7665 645f 636f  on=last_saved_co
+000011e0: 6d6d 6974 5f70 6f73 6974 696f 6e0a 290a  mmit_position.).
+000011f0: 0a23 2054 6f20 696d 706c 656d 656e 7420  .# To implement 
+00001200: 2265 7861 6374 6c79 2d6f 6e63 6522 2073  "exactly-once" s
+00001210: 656d 616e 7469 6373 2c20 6974 6572 6174  emantics, iterat
+00001220: 6520 6f76 6572 2074 6865 0a23 2022 6361  e over the.# "ca
+00001230: 7463 682d 7570 2220 7375 6273 6372 6970  tch-up" subscrip
+00001240: 7469 6f6e 2e20 5072 6f63 6573 7320 6561  tion. Process ea
+00001250: 6368 2072 6563 6569 7665 6420 6576 656e  ch received even
+00001260: 742c 0a23 2069 6e20 7475 726e 2c20 7468  t,.# in turn, th
+00001270: 726f 7567 6820 616e 2065 7665 6e74 2d70  rough an event-p
+00001280: 726f 6365 7373 696e 6720 706f 6c69 6379  rocessing policy
+00001290: 2e20 5361 7665 2074 6865 0a23 2076 616c  . Save the.# val
+000012a0: 7565 206f 6620 7468 6520 636f 6d6d 6974  ue of the commit
+000012b0: 5f70 6f73 6974 696f 6e20 6174 7472 6962  _position attrib
+000012c0: 7574 6520 6f66 2074 6865 2070 726f 6365  ute of the proce
+000012d0: 7373 6564 0a23 2065 7665 6e74 2077 6974  ssed.# event wit
+000012e0: 6820 6e65 7720 7374 6174 6520 6765 6e65  h new state gene
+000012f0: 7261 7465 6420 6279 2074 6865 2070 6f6c  rated by the pol
+00001300: 6963 7920 696e 2074 6865 2073 616d 650a  icy in the same.
+00001310: 2320 6174 6f6d 6963 2074 7261 6e73 6163  # atomic transac
+00001320: 7469 6f6e 2e20 5573 6520 7468 6520 6c61  tion. Use the la
+00001330: 7374 2073 6176 6564 2022 636f 6d6d 6974  st saved "commit
+00001340: 2070 6f73 6974 696f 6e22 0a23 2077 6865   position".# whe
+00001350: 6e20 7265 7374 6172 7469 6e67 2074 6865  n restarting the
+00001360: 2022 6361 7463 682d 7570 2220 7375 6273   "catch-up" subs
+00001370: 6372 6970 7469 6f6e 2e0a 0a72 6563 6569  cription...recei
+00001380: 7665 6420 3d20 5b5d 0a66 6f72 2065 7665  ved = [].for eve
+00001390: 6e74 2069 6e20 7375 6273 6372 6970 7469  nt in subscripti
+000013a0: 6f6e 3a0a 2020 2020 7265 6365 6976 6564  on:.    received
+000013b0: 2e61 7070 656e 6428 6576 656e 7429 0a20  .append(event). 
+000013c0: 2020 2069 6620 6576 656e 742e 6964 203d     if event.id =
+000013d0: 3d20 6576 656e 7433 2e69 643a 0a20 2020  = event3.id:.   
+000013e0: 2020 2020 2062 7265 616b 0a0a 6173 7365       break..asse
+000013f0: 7274 2072 6563 6569 7665 645b 2d33 5d2e  rt received[-3].
+00001400: 6461 7461 203d 3d20 6576 656e 7431 2e64  data == event1.d
+00001410: 6174 610a 6173 7365 7274 2072 6563 6569  ata.assert recei
+00001420: 7665 645b 2d32 5d2e 6461 7461 203d 3d20  ved[-2].data == 
+00001430: 6576 656e 7432 2e64 6174 610a 6173 7365  event2.data.asse
+00001440: 7274 2072 6563 6569 7665 645b 2d31 5d2e  rt received[-1].
+00001450: 6461 7461 203d 3d20 6576 656e 7433 2e64  data == event3.d
+00001460: 6174 610a 6173 7365 7274 2072 6563 6569  ata.assert recei
+00001470: 7665 645b 2d33 5d2e 7479 7065 203d 3d20  ved[-3].type == 
+00001480: 6576 656e 7431 2e74 7970 650a 6173 7365  event1.type.asse
+00001490: 7274 2072 6563 6569 7665 645b 2d32 5d2e  rt received[-2].
+000014a0: 7479 7065 203d 3d20 6576 656e 7432 2e74  type == event2.t
+000014b0: 7970 650a 6173 7365 7274 2072 6563 6569  ype.assert recei
+000014c0: 7665 645b 2d31 5d2e 7479 7065 203d 3d20  ved[-1].type == 
+000014d0: 6576 656e 7433 2e74 7970 650a 0a61 7373  event3.type..ass
+000014e0: 6572 7420 7265 6365 6976 6564 5b2d 335d  ert received[-3]
+000014f0: 2e63 6f6d 6d69 745f 706f 7369 7469 6f6e  .commit_position
+00001500: 203e 2030 0a61 7373 6572 7420 7265 6365   > 0.assert rece
+00001510: 6976 6564 5b2d 325d 2e63 6f6d 6d69 745f  ived[-2].commit_
+00001520: 706f 7369 7469 6f6e 203e 2072 6563 6569  position > recei
+00001530: 7665 645b 2d33 5d2e 636f 6d6d 6974 5f70  ved[-3].commit_p
+00001540: 6f73 6974 696f 6e0a 6173 7365 7274 2072  osition.assert r
+00001550: 6563 6569 7665 645b 2d31 5d2e 636f 6d6d  eceived[-1].comm
+00001560: 6974 5f70 6f73 6974 696f 6e20 3e20 7265  it_position > re
+00001570: 6365 6976 6564 5b2d 325d 2e63 6f6d 6d69  ceived[-2].commi
+00001580: 745f 706f 7369 7469 6f6e 0a0a 0a23 2043  t_position...# C
+00001590: 6c6f 7365 2074 6865 2063 6c69 656e 7420  lose the client 
+000015a0: 6166 7465 7220 7573 652e 0a0a 636c 6965  after use...clie
+000015b0: 6e74 2e63 6c6f 7365 2829 0a60 6060 0a0a  nt.close().```..
+000015c0: 5365 6520 6265 6c6f 7720 666f 7220 6d6f  See below for mo
+000015d0: 7265 2064 6574 6169 6c73 2e0a 0a46 6f72  re details...For
+000015e0: 2061 6e20 6578 616d 706c 6520 6f66 2075   an example of u
+000015f0: 7361 6765 2c20 7365 6520 7468 6520 5b65  sage, see the [e
+00001600: 7665 6e74 736f 7572 6369 6e67 2d65 7665  ventsourcing-eve
+00001610: 6e74 7374 6f72 6564 625d 280a 6874 7470  ntstoredb](.http
+00001620: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00001630: 7965 7665 6e74 736f 7572 6369 6e67 2f65  yeventsourcing/e
+00001640: 7665 6e74 736f 7572 6369 6e67 2d65 7665  ventsourcing-eve
+00001650: 6e74 7374 6f72 6564 6229 2070 6163 6b61  ntstoredb) packa
+00001660: 6765 2e0a 0a23 2320 5461 626c 6520 6f66  ge...## Table of
+00001670: 2063 6f6e 7465 6e74 730a 0a3c 212d 2d20   contents..<!-- 
+00001680: 544f 4320 2d2d 3e0a 2a20 5b49 6e73 7461  TOC -->.* [Insta
+00001690: 6c6c 2070 6163 6b61 6765 5d28 2369 6e73  ll package](#ins
+000016a0: 7461 6c6c 2d70 6163 6b61 6765 290a 2020  tall-package).  
+000016b0: 2a20 5b46 726f 6d20 5079 5049 5d28 2366  * [From PyPI](#f
+000016c0: 726f 6d2d 7079 7069 290a 2020 2a20 5b57  rom-pypi).  * [W
+000016d0: 6974 6820 506f 6574 7279 5d28 2377 6974  ith Poetry](#wit
+000016e0: 682d 706f 6574 7279 290a 2a20 5b45 7665  h-poetry).* [Eve
+000016f0: 6e74 5374 6f72 6544 4220 7365 7276 6572  ntStoreDB server
+00001700: 5d28 2365 7665 6e74 7374 6f72 6564 622d  ](#eventstoredb-
+00001710: 7365 7276 6572 290a 2020 2a20 5b52 756e  server).  * [Run
+00001720: 2063 6f6e 7461 696e 6572 5d28 2372 756e   container](#run
+00001730: 2d63 6f6e 7461 696e 6572 290a 2020 2a20  -container).  * 
+00001740: 5b53 746f 7020 636f 6e74 6169 6e65 725d  [Stop container]
+00001750: 2823 7374 6f70 2d63 6f6e 7461 696e 6572  (#stop-container
+00001760: 290a 2a20 5b45 7665 6e74 5374 6f72 6544  ).* [EventStoreD
+00001770: 4220 636c 6965 6e74 5d28 2365 7665 6e74  B client](#event
+00001780: 7374 6f72 6564 622d 636c 6965 6e74 290a  storedb-client).
+00001790: 2020 2a20 5b49 6d70 6f72 7420 636c 6173    * [Import clas
+000017a0: 735d 2823 696d 706f 7274 2d63 6c61 7373  s](#import-class
+000017b0: 290a 2020 2a20 5b43 6f6e 7374 7275 6374  ).  * [Construct
+000017c0: 2063 6c69 656e 745d 2823 636f 6e73 7472   client](#constr
+000017d0: 7563 742d 636c 6965 6e74 290a 2a20 5b53  uct-client).* [S
+000017e0: 7472 6561 6d73 5d28 2373 7472 6561 6d73  treams](#streams
+000017f0: 290a 2020 2a20 5b41 7070 656e 6420 6576  ).  * [Append ev
+00001800: 656e 7473 5d28 2361 7070 656e 642d 6576  ents](#append-ev
+00001810: 656e 7473 290a 2020 2a20 5b41 7070 656e  ents).  * [Appen
+00001820: 6420 6576 656e 745d 2823 6170 7065 6e64  d event](#append
+00001830: 2d65 7665 6e74 290a 2020 2a20 5b49 6465  -event).  * [Ide
+00001840: 6d70 6f74 656e 7420 6170 7065 6e64 206f  mpotent append o
+00001850: 7065 7261 7469 6f6e 735d 2823 6964 656d  perations](#idem
+00001860: 706f 7465 6e74 2d61 7070 656e 642d 6f70  potent-append-op
+00001870: 6572 6174 696f 6e73 290a 2020 2a20 5b52  erations).  * [R
+00001880: 6561 6420 7374 7265 616d 2065 7665 6e74  ead stream event
+00001890: 735d 2823 7265 6164 2d73 7472 6561 6d2d  s](#read-stream-
+000018a0: 6576 656e 7473 290a 2020 2a20 5b52 6561  events).  * [Rea
+000018b0: 6420 616c 6c20 6576 656e 7473 5d28 2372  d all events](#r
+000018c0: 6561 642d 616c 6c2d 6576 656e 7473 290a  ead-all-events).
+000018d0: 2020 2a20 5b47 6574 2063 7572 7265 6e74    * [Get current
+000018e0: 2073 7472 6561 6d20 706f 7369 7469 6f6e   stream position
+000018f0: 5d28 2367 6574 2d63 7572 7265 6e74 2d73  ](#get-current-s
+00001900: 7472 6561 6d2d 706f 7369 7469 6f6e 290a  tream-position).
+00001910: 2020 2a20 5b47 6574 2063 7572 7265 6e74    * [Get current
+00001920: 2063 6f6d 6d69 7420 706f 7369 7469 6f6e   commit position
+00001930: 5d28 2367 6574 2d63 7572 7265 6e74 2d63  ](#get-current-c
+00001940: 6f6d 6d69 742d 706f 7369 7469 6f6e 290a  ommit-position).
+00001950: 2020 2a20 5b47 6574 2073 7472 6561 6d20    * [Get stream 
+00001960: 6d65 7461 6461 7461 5d28 2367 6574 2d73  metadata](#get-s
+00001970: 7472 6561 6d2d 6d65 7461 6461 7461 290a  tream-metadata).
+00001980: 2020 2a20 5b53 6574 2073 7472 6561 6d20    * [Set stream 
+00001990: 6d65 7461 6461 7461 5d28 2373 6574 2d73  metadata](#set-s
+000019a0: 7472 6561 6d2d 6d65 7461 6461 7461 290a  tream-metadata).
+000019b0: 2020 2a20 5b44 656c 6574 6520 7374 7265    * [Delete stre
+000019c0: 616d 5d28 2364 656c 6574 652d 7374 7265  am](#delete-stre
+000019d0: 616d 290a 2020 2a20 5b54 6f6d 6273 746f  am).  * [Tombsto
+000019e0: 6e65 2073 7472 6561 6d5d 2823 746f 6d62  ne stream](#tomb
+000019f0: 7374 6f6e 652d 7374 7265 616d 290a 2a20  stone-stream).* 
+00001a00: 5b43 6174 6368 2d75 7020 7375 6273 6372  [Catch-up subscr
+00001a10: 6970 7469 6f6e 735d 2823 6361 7463 682d  iptions](#catch-
+00001a20: 7570 2d73 7562 7363 7269 7074 696f 6e73  up-subscriptions
+00001a30: 290a 2020 2a20 5b48 6f77 2074 6f20 696d  ).  * [How to im
+00001a40: 706c 656d 656e 7420 6578 6163 746c 792d  plement exactly-
+00001a50: 6f6e 6365 2065 7665 6e74 2070 726f 6365  once event proce
+00001a60: 7373 696e 675d 2823 686f 772d 746f 2d69  ssing](#how-to-i
+00001a70: 6d70 6c65 6d65 6e74 2d65 7861 6374 6c79  mplement-exactly
+00001a80: 2d6f 6e63 652d 6576 656e 742d 7072 6f63  -once-event-proc
+00001a90: 6573 7369 6e67 290a 2020 2a20 5b53 7562  essing).  * [Sub
+00001aa0: 7363 7269 6265 2061 6c6c 2065 7665 6e74  scribe all event
+00001ab0: 735d 2823 7375 6273 6372 6962 652d 616c  s](#subscribe-al
+00001ac0: 6c2d 6576 656e 7473 290a 2020 2a20 5b53  l-events).  * [S
+00001ad0: 7562 7363 7269 6265 2073 7472 6561 6d20  ubscribe stream 
+00001ae0: 6576 656e 7473 5d28 2373 7562 7363 7269  events](#subscri
+00001af0: 6265 2d73 7472 6561 6d2d 6576 656e 7473  be-stream-events
+00001b00: 290a 2a20 5b50 6572 7369 7374 656e 7420  ).* [Persistent 
+00001b10: 7375 6273 6372 6970 7469 6f6e 735d 2823  subscriptions](#
+00001b20: 7065 7273 6973 7465 6e74 2d73 7562 7363  persistent-subsc
+00001b30: 7269 7074 696f 6e73 290a 2020 2a20 5b43  riptions).  * [C
+00001b40: 7265 6174 6520 7375 6273 6372 6970 7469  reate subscripti
+00001b50: 6f6e 5d28 2363 7265 6174 652d 7375 6273  on](#create-subs
+00001b60: 6372 6970 7469 6f6e 290a 2020 2a20 5b52  cription).  * [R
+00001b70: 6561 6420 7375 6273 6372 6970 7469 6f6e  ead subscription
+00001b80: 5d28 2372 6561 642d 7375 6273 6372 6970  ](#read-subscrip
+00001b90: 7469 6f6e 290a 2020 2a20 5b47 6574 2073  tion).  * [Get s
+00001ba0: 7562 7363 7269 7074 696f 6e20 696e 666f  ubscription info
+00001bb0: 5d28 2367 6574 2d73 7562 7363 7269 7074  ](#get-subscript
+00001bc0: 696f 6e2d 696e 666f 290a 2020 2a20 5b4c  ion-info).  * [L
+00001bd0: 6973 7420 7375 6273 6372 6970 7469 6f6e  ist subscription
+00001be0: 735d 2823 6c69 7374 2d73 7562 7363 7269  s](#list-subscri
+00001bf0: 7074 696f 6e73 290a 2020 2a20 5b44 656c  ptions).  * [Del
+00001c00: 6574 6520 7375 6273 6372 6970 7469 6f6e  ete subscription
+00001c10: 5d28 2364 656c 6574 652d 7375 6273 6372  ](#delete-subscr
+00001c20: 6970 7469 6f6e 290a 2020 2a20 5b43 7265  iption).  * [Cre
+00001c30: 6174 6520 7374 7265 616d 2073 7562 7363  ate stream subsc
+00001c40: 7269 7074 696f 6e5d 2823 6372 6561 7465  ription](#create
+00001c50: 2d73 7472 6561 6d2d 7375 6273 6372 6970  -stream-subscrip
+00001c60: 7469 6f6e 290a 2020 2a20 5b52 6561 6420  tion).  * [Read 
+00001c70: 7374 7265 616d 2073 7562 7363 7269 7074  stream subscript
+00001c80: 696f 6e5d 2823 7265 6164 2d73 7472 6561  ion](#read-strea
+00001c90: 6d2d 7375 6273 6372 6970 7469 6f6e 290a  m-subscription).
+00001ca0: 2020 2a20 5b47 6574 2073 7472 6561 6d20    * [Get stream 
+00001cb0: 7375 6273 6372 6970 7469 6f6e 2069 6e66  subscription inf
+00001cc0: 6f5d 2823 6765 742d 7374 7265 616d 2d73  o](#get-stream-s
+00001cd0: 7562 7363 7269 7074 696f 6e2d 696e 666f  ubscription-info
+00001ce0: 290a 2020 2a20 5b4c 6973 7420 7374 7265  ).  * [List stre
+00001cf0: 616d 2073 7562 7363 7269 7074 696f 6e73  am subscriptions
+00001d00: 5d28 236c 6973 742d 7374 7265 616d 2d73  ](#list-stream-s
+00001d10: 7562 7363 7269 7074 696f 6e73 290a 2020  ubscriptions).  
+00001d20: 2a20 5b44 656c 6574 6520 7374 7265 616d  * [Delete stream
+00001d30: 2073 7562 7363 7269 7074 696f 6e5d 2823   subscription](#
+00001d40: 6465 6c65 7465 2d73 7472 6561 6d2d 7375  delete-stream-su
+00001d50: 6273 6372 6970 7469 6f6e 290a 2a20 5b43  bscription).* [C
+00001d60: 6f6e 6e65 6374 696f 6e5d 2823 636f 6e6e  onnection](#conn
+00001d70: 6563 7469 6f6e 290a 2020 2a20 5b52 6563  ection).  * [Rec
+00001d80: 6f6e 6e65 6374 5d28 2372 6563 6f6e 6e65  onnect](#reconne
+00001d90: 6374 290a 2020 2a20 5b43 6c6f 7365 5d28  ct).  * [Close](
+00001da0: 2363 6c6f 7365 290a 2a20 5b4e 6f74 6573  #close).* [Notes
+00001db0: 5d28 236e 6f74 6573 290a 2020 2a20 5b43  ](#notes).  * [C
+00001dc0: 6f6e 6e65 6374 696f 6e20 7374 7269 6e67  onnection string
+00001dd0: 735d 2823 636f 6e6e 6563 7469 6f6e 2d73  s](#connection-s
+00001de0: 7472 696e 6773 290a 2020 2a20 5b52 6567  trings).  * [Reg
+00001df0: 756c 6172 2065 7870 7265 7373 696f 6e20  ular expression 
+00001e00: 6669 6c74 6572 735d 2823 7265 6775 6c61  filters](#regula
+00001e10: 722d 6578 7072 6573 7369 6f6e 2d66 696c  r-expression-fil
+00001e20: 7465 7273 290a 2020 2a20 5b4e 6577 2065  ters).  * [New e
+00001e30: 7665 6e74 206f 626a 6563 7473 5d28 236e  vent objects](#n
+00001e40: 6577 2d65 7665 6e74 2d6f 626a 6563 7473  ew-event-objects
+00001e50: 290a 2020 2a20 5b52 6563 6f72 6465 6420  ).  * [Recorded 
+00001e60: 6576 656e 7420 6f62 6a65 6374 735d 2823  event objects](#
+00001e70: 7265 636f 7264 6564 2d65 7665 6e74 2d6f  recorded-event-o
+00001e80: 626a 6563 7473 290a 2a20 5b43 6f6e 7472  bjects).* [Contr
+00001e90: 6962 7574 6f72 735d 2823 636f 6e74 7269  ibutors](#contri
+00001ea0: 6275 746f 7273 290a 2020 2a20 5b49 6e73  butors).  * [Ins
+00001eb0: 7461 6c6c 2050 6f65 7472 795d 2823 696e  tall Poetry](#in
+00001ec0: 7374 616c 6c2d 706f 6574 7279 290a 2020  stall-poetry).  
+00001ed0: 2a20 5b53 6574 7570 2066 6f72 2050 7943  * [Setup for PyC
+00001ee0: 6861 726d 2075 7365 7273 5d28 2373 6574  harm users](#set
+00001ef0: 7570 2d66 6f72 2d70 7963 6861 726d 2d75  up-for-pycharm-u
+00001f00: 7365 7273 290a 2020 2a20 5b53 6574 7570  sers).  * [Setup
+00001f10: 2066 726f 6d20 636f 6d6d 616e 6420 6c69   from command li
+00001f20: 6e65 5d28 2373 6574 7570 2d66 726f 6d2d  ne](#setup-from-
+00001f30: 636f 6d6d 616e 642d 6c69 6e65 290a 2020  command-line).  
+00001f40: 2a20 5b50 726f 6a65 6374 204d 616b 6566  * [Project Makef
+00001f50: 696c 6520 636f 6d6d 616e 6473 5d28 2370  ile commands](#p
+00001f60: 726f 6a65 6374 2d6d 616b 6566 696c 652d  roject-makefile-
+00001f70: 636f 6d6d 616e 6473 290a 3c21 2d2d 2054  commands).<!-- T
+00001f80: 4f43 202d 2d3e 0a0a 2323 2049 6e73 7461  OC -->..## Insta
+00001f90: 6c6c 2070 6163 6b61 6765 0a0a 4974 2069  ll package..It i
+00001fa0: 7320 7265 636f 6d6d 656e 6465 6420 746f  s recommended to
+00001fb0: 2069 6e73 7461 6c6c 2050 7974 686f 6e20   install Python 
+00001fc0: 7061 636b 6167 6573 2069 6e74 6f20 6120  packages into a 
+00001fd0: 5079 7468 6f6e 2076 6972 7475 616c 2065  Python virtual e
+00001fe0: 6e76 6972 6f6e 6d65 6e74 2e0a 0a23 2323  nvironment...###
+00001ff0: 2046 726f 6d20 5079 5049 0a0a 596f 7520   From PyPI..You 
+00002000: 6361 6e20 7573 6520 7069 7020 746f 2069  can use pip to i
+00002010: 6e73 7461 6c6c 2074 6869 7320 7061 636b  nstall this pack
+00002020: 6167 6520 6469 7265 6374 6c79 2066 726f  age directly fro
+00002030: 6d0a 5b74 6865 2050 7974 686f 6e20 5061  m.[the Python Pa
+00002040: 636b 6167 6520 496e 6465 785d 2868 7474  ckage Index](htt
+00002050: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+00002060: 6f6a 6563 742f 6573 6462 636c 6965 6e74  oject/esdbclient
+00002070: 2f29 2e0a 0a20 2020 2024 2070 6970 2069  /)...    $ pip i
+00002080: 6e73 7461 6c6c 2065 7364 6263 6c69 656e  nstall esdbclien
+00002090: 740a 0a23 2323 2057 6974 6820 506f 6574  t..### With Poet
+000020a0: 7279 0a0a 596f 7520 6361 6e20 7573 6520  ry..You can use 
+000020b0: 506f 6574 7279 2074 6f20 6164 6420 7468  Poetry to add th
+000020c0: 6973 2070 6163 6b61 6765 2074 6f20 796f  is package to yo
+000020d0: 7572 2070 7970 726f 6a65 6374 2e74 6f6d  ur pyproject.tom
+000020e0: 6c20 616e 6420 696e 7374 616c 6c20 6974  l and install it
+000020f0: 2e0a 0a20 2020 2024 2070 6f65 7472 7920  ...    $ poetry 
+00002100: 6164 6420 6573 6462 636c 6965 6e74 0a0a  add esdbclient..
+00002110: 2323 2045 7665 6e74 5374 6f72 6544 4220  ## EventStoreDB 
+00002120: 7365 7276 6572 0a0a 5468 6520 4576 656e  server..The Even
+00002130: 7453 746f 7265 4442 2073 6572 7665 7220  tStoreDB server 
+00002140: 6361 6e20 6265 2072 756e 206c 6f63 616c  can be run local
+00002150: 6c79 2075 7369 6e67 2074 6865 206f 6666  ly using the off
+00002160: 6963 6961 6c20 446f 636b 6572 2063 6f6e  icial Docker con
+00002170: 7461 696e 6572 2069 6d61 6765 2e0a 0a23  tainer image...#
+00002180: 2323 2052 756e 2063 6f6e 7461 696e 6572  ## Run container
+00002190: 0a0a 466f 7220 6465 7665 6c6f 706d 656e  ..For developmen
+000021a0: 742c 2079 6f75 2063 616e 2072 756e 2061  t, you can run a
+000021b0: 2022 7365 6375 7265 2220 4576 656e 7453   "secure" EventS
+000021c0: 746f 7265 4442 2073 6572 7665 7220 7573  toreDB server us
+000021d0: 696e 6720 7468 6520 666f 6c6c 6f77 696e  ing the followin
+000021e0: 6720 636f 6d6d 616e 642e 0a0a 2020 2020  g command...    
+000021f0: 2420 646f 636b 6572 2072 756e 202d 6420  $ docker run -d 
+00002200: 2d2d 6e61 6d65 2065 7665 6e74 7374 6f72  --name eventstor
+00002210: 6564 622d 7365 6375 7265 202d 6974 202d  edb-secure -it -
+00002220: 7020 3231 3133 3a32 3131 3320 2d2d 656e  p 2113:2113 --en
+00002230: 7620 2248 4f4d 453d 2f74 6d70 2220 6576  v "HOME=/tmp" ev
+00002240: 656e 7473 746f 7265 2f65 7665 6e74 7374  entstore/eventst
+00002250: 6f72 653a 3231 2e31 302e 392d 6275 7374  ore:21.10.9-bust
+00002260: 6572 2d73 6c69 6d20 2d2d 6465 760a 0a54  er-slim --dev..T
+00002270: 6865 2063 6f6e 6e65 6374 696f 6e20 7374  he connection st
+00002280: 7269 6e67 2066 6f72 2074 6869 7320 2273  ring for this "s
+00002290: 6563 7572 6522 2045 7665 6e74 5374 6f72  ecure" EventStor
+000022a0: 6544 4220 7365 7276 6572 2077 6f75 6c64  eDB server would
+000022b0: 2062 653a 0a0a 2020 2020 6573 6462 3a2f   be:..    esdb:/
+000022c0: 2f61 646d 696e 3a63 6861 6e67 6569 7440  /admin:changeit@
+000022d0: 6c6f 6361 6c68 6f73 743a 3231 3133 0a0a  localhost:2113..
+000022e0: 4173 2077 6520 7769 6c6c 2073 6565 2c20  As we will see, 
+000022f0: 7468 6520 636c 6965 6e74 206e 6565 6473  the client needs
+00002300: 2061 6e20 4576 656e 7453 746f 7265 4442   an EventStoreDB
+00002310: 2063 6f6e 6e65 6374 696f 6e20 7374 7269   connection stri
+00002320: 6e67 2061 7320 7468 6520 7661 6c75 6520  ng as the value 
+00002330: 6f66 0a69 7473 2060 7572 6960 2063 6f6e  of.its `uri` con
+00002340: 7374 7275 6374 6f72 2061 7267 756d 656e  structor argumen
+00002350: 742e 0a0a 546f 2063 6f6e 6e65 6374 2074  t...To connect t
+00002360: 6f20 6120 2273 6563 7572 6522 2073 6572  o a "secure" ser
+00002370: 7665 722c 2079 6f75 2077 696c 6c20 7573  ver, you will us
+00002380: 7573 616c 6c79 206e 6565 6420 746f 2069  usally need to i
+00002390: 6e63 6c75 6465 2061 2022 7573 6572 6e61  nclude a "userna
+000023a0: 6d65 220a 616e 6420 6120 2270 6173 7377  me".and a "passw
+000023b0: 6f72 6422 2069 6e20 7468 6520 636f 6e6e  ord" in the conn
+000023c0: 6563 7469 6f6e 2073 7472 696e 672c 2073  ection string, s
+000023d0: 6f20 7468 6174 2074 6865 2073 6572 7665  o that the serve
+000023e0: 7220 6361 6e20 6175 7468 656e 7469 6361  r can authentica
+000023f0: 7465 2074 6865 0a63 6c69 656e 742e 2054  te the.client. T
+00002400: 6865 2064 6566 6175 6c74 2075 7365 726e  he default usern
+00002410: 616d 6520 6973 2022 6164 6d69 6e22 2061  ame is "admin" a
+00002420: 6e64 2074 6865 2064 6566 6175 6c74 2070  nd the default p
+00002430: 6173 7377 6f72 6420 6973 2022 6368 616e  assword is "chan
+00002440: 6765 6974 222e 0a0a 5365 6520 7468 6520  geit"...See the 
+00002450: 4e6f 7465 7320 7365 6374 696f 6e20 6265  Notes section be
+00002460: 6c6f 7720 666f 7220 6d6f 7265 2069 6e66  low for more inf
+00002470: 6f72 6d61 7469 6f6e 2061 626f 7574 2045  ormation about E
+00002480: 7665 6e74 5374 6f72 6544 4220 636f 6e6e  ventStoreDB conn
+00002490: 6563 7469 6f6e 2073 7472 696e 6773 2e0a  ection strings..
+000024a0: 0a54 6f20 636f 6e6e 6563 7420 746f 2061  .To connect to a
+000024b0: 2022 7365 6375 7265 2220 7365 7276 6572   "secure" server
+000024c0: 2c20 796f 7520 7769 6c6c 2061 6c73 6f20  , you will also 
+000024d0: 6e65 6564 2061 6e20 5353 4c2f 544c 5320  need an SSL/TLS 
+000024e0: 6365 7274 6966 6963 6174 652c 2073 6f20  certificate, so 
+000024f0: 7468 6174 2074 6865 0a63 6c69 656e 7420  that the.client 
+00002500: 6361 6e20 6175 7468 656e 7469 6361 7465  can authenticate
+00002510: 2074 6865 2073 6572 7665 722e 2046 6f72   the server. For
+00002520: 2064 6576 656c 6f70 6d65 6e74 2c20 796f   development, yo
+00002530: 7520 6361 6e20 6569 7468 6572 2075 7365  u can either use
+00002540: 2074 6865 2053 534c 2f54 4c53 0a63 6572   the SSL/TLS.cer
+00002550: 7469 6669 6361 7465 206f 6620 7468 6520  tificate of the 
+00002560: 6365 7274 6966 6963 6174 6520 6175 7468  certificate auth
+00002570: 6f72 6974 7920 7573 6564 2074 6f20 6372  ority used to cr
+00002580: 6561 7465 2074 6865 2073 6572 7665 7227  eate the server'
+00002590: 7320 6365 7274 6966 6963 6174 652c 206f  s certificate, o
+000025a0: 720a 7768 656e 2075 7369 6e67 2061 2073  r.when using a s
+000025b0: 696e 676c 652d 6e6f 6465 2063 6c75 7374  ingle-node clust
+000025c0: 6572 2c20 796f 7520 6361 6e20 6765 7420  er, you can get 
+000025d0: 7468 6520 6365 7274 6966 6963 6174 6520  the certificate 
+000025e0: 6672 6f6d 2074 6865 2073 6572 7665 722e  from the server.
+000025f0: 2059 6f75 2063 616e 0a67 6574 2074 6865   You can.get the
+00002600: 2073 6572 7665 7220 6365 7274 6966 6963   server certific
+00002610: 6174 6520 7769 7468 2074 6865 2066 6f6c  ate with the fol
+00002620: 6c6f 7769 6e67 2050 7974 686f 6e20 636f  lowing Python co
+00002630: 6465 2e0a 0a41 7320 7765 2077 696c 6c20  de...As we will 
+00002640: 7365 652c 2077 6865 6e20 636f 6e6e 6563  see, when connec
+00002650: 7469 6e67 2074 6f20 6120 2273 6563 7572  ting to a "secur
+00002660: 6522 2073 6572 7665 722c 2074 6865 2063  e" server, the c
+00002670: 6c69 656e 7420 6e65 6564 7320 616e 2053  lient needs an S
+00002680: 534c 2f54 4c53 0a63 6572 7469 6669 6361  SL/TLS.certifica
+00002690: 7465 2061 7320 7468 6520 7661 6c75 6520  te as the value 
+000026a0: 6f66 2069 7473 2060 726f 6f74 5f63 6572  of its `root_cer
+000026b0: 7469 6669 6361 7465 7360 2063 6f6e 7374  tificates` const
+000026c0: 7275 6374 6f72 2061 7267 756d 656e 742e  ructor argument.
+000026d0: 0a0a 0a60 6060 7079 7468 6f6e 0a69 6d70  ...```python.imp
+000026e0: 6f72 7420 7373 6c0a 0a0a 7365 7276 6572  ort ssl...server
+000026f0: 5f63 6572 7469 6669 6361 7465 203d 2073  _certificate = s
+00002700: 736c 2e67 6574 5f73 6572 7665 725f 6365  sl.get_server_ce
+00002710: 7274 6966 6963 6174 6528 6164 6472 3d28  rtificate(addr=(
+00002720: 276c 6f63 616c 686f 7374 272c 2032 3131  'localhost', 211
+00002730: 3329 290a 6060 600a 0a59 6f75 2063 616e  3)).```..You can
+00002740: 2061 6c73 6f20 7374 6172 7420 616e 2022   also start an "
+00002750: 696e 7365 6375 7265 2220 7365 7276 6572  insecure" server
+00002760: 2075 7369 6e67 2074 6865 2066 6f6c 6c6f   using the follo
+00002770: 7769 6e67 2063 6f6d 6d61 6e64 2e0a 0a20  wing command... 
+00002780: 2020 2024 2064 6f63 6b65 7220 7275 6e20     $ docker run 
+00002790: 2d64 202d 2d6e 616d 6520 6576 656e 7473  -d --name events
+000027a0: 746f 7265 6462 2d69 6e73 6563 7572 6520  toredb-insecure 
+000027b0: 2d69 7420 2d70 2032 3131 343a 3231 3133  -it -p 2114:2113
+000027c0: 2065 7665 6e74 7374 6f72 652f 6576 656e   eventstore/even
+000027d0: 7473 746f 7265 3a32 312e 3130 2e39 2d62  tstore:21.10.9-b
+000027e0: 7573 7465 722d 736c 696d 202d 2d69 6e73  uster-slim --ins
+000027f0: 6563 7572 650a 0a54 6865 2063 6f6e 6e65  ecure..The conne
+00002800: 6374 696f 6e20 7374 7269 6e67 2055 5249  ction string URI
+00002810: 2066 6f72 2074 6869 7320 2269 6e73 6563   for this "insec
+00002820: 7572 6522 2073 6572 7665 7220 776f 756c  ure" server woul
+00002830: 6420 6265 3a0a 0a20 2020 2065 7364 623a  d be:..    esdb:
+00002840: 2f2f 6c6f 6361 6c68 6f73 743a 3231 3134  //localhost:2114
+00002850: 3f54 6c73 3d66 616c 7365 0a0a 4173 2077  ?Tls=false..As w
+00002860: 6520 7769 6c6c 2073 6565 2c20 7768 656e  e will see, when
+00002870: 2063 6f6e 6e65 6374 696e 6720 746f 2061   connecting to a
+00002880: 6e20 2269 6e73 6563 7572 6522 2073 6572  n "insecure" ser
+00002890: 7665 722c 2074 6865 7265 2069 7320 6e6f  ver, there is no
+000028a0: 206e 6565 6420 746f 2069 6e63 6c75 6465   need to include
+000028b0: 0a61 2022 7573 6572 6e61 6d65 2220 616e  .a "username" an
+000028c0: 6420 6120 2270 6173 7377 6f72 6422 2069  d a "password" i
+000028d0: 6e20 7468 6520 636f 6e6e 6563 7469 6f6e  n the connection
+000028e0: 2073 7472 696e 672e 2049 6620 796f 7520   string. If you 
+000028f0: 646f 2c20 7468 6573 6520 7661 6c75 6573  do, these values
+00002900: 2077 696c 6c0a 6265 2069 676e 6f72 6564   will.be ignored
+00002910: 2062 7920 7468 6520 636c 6965 6e74 2c20   by the client, 
+00002920: 736f 2074 6861 7420 7468 6579 2077 696c  so that they wil
+00002930: 6c20 6e6f 7420 6265 2073 656e 7420 746f  l not be sent to
+00002940: 2074 6865 2073 6572 7665 7220 6f76 6572   the server over
+00002950: 2061 6e0a 696e 7365 6375 7265 2063 6861   an.insecure cha
+00002960: 6e6e 656c 2e0a 0a50 6c65 6173 6520 6e6f  nnel...Please no
+00002970: 7465 2c20 7468 6520 2269 6e73 6563 7572  te, the "insecur
+00002980: 6522 2063 6f6e 6e65 6374 696f 6e20 7374  e" connection st
+00002990: 7269 6e67 2075 7365 7320 7468 6520 7175  ring uses the qu
+000029a0: 6572 7920 7374 7269 6e67 2060 3f54 6c73  ery string `?Tls
+000029b0: 3d66 616c 7365 602e 2054 6865 0a76 616c  =false`. The.val
+000029c0: 7565 206f 6620 7468 6973 2066 6965 6c64  ue of this field
+000029d0: 2069 7320 6279 2064 6566 6175 6c74 2060   is by default `
+000029e0: 7472 7565 602e 2053 6565 2074 6865 204e  true`. See the N
+000029f0: 6f74 6573 2073 6563 7469 6f6e 2062 656c  otes section bel
+00002a00: 6f77 2066 6f72 206d 6f72 650a 696e 666f  ow for more.info
+00002a10: 726d 6174 696f 6e20 6162 6f75 7420 4576  rmation about Ev
+00002a20: 656e 7453 746f 7265 4442 2063 6f6e 6e65  entStoreDB conne
+00002a30: 6374 696f 6e20 7374 7269 6e67 7320 616e  ction strings an
+00002a40: 6420 7468 6520 6669 656c 6473 2074 6861  d the fields tha
+00002a50: 7420 6361 6e20 6265 2075 7365 640a 696e  t can be used.in
+00002a60: 2074 6865 2071 7565 7279 2073 7472 696e   the query strin
+00002a70: 6720 746f 2073 7065 6369 6679 2063 6f6e  g to specify con
+00002a80: 6e65 6374 696f 6e20 6f70 7469 6f6e 732e  nection options.
+00002a90: 0a0a 2323 2320 5374 6f70 2063 6f6e 7461  ..### Stop conta
+00002aa0: 696e 6572 0a0a 546f 2073 746f 7020 616e  iner..To stop an
+00002ab0: 6420 7265 6d6f 7665 2074 6865 2022 7365  d remove the "se
+00002ac0: 6375 7265 2220 636f 6e74 6169 6e65 722c  cure" container,
+00002ad0: 2075 7365 2074 6865 2066 6f6c 6c6f 7769   use the followi
+00002ae0: 6e67 2044 6f63 6b65 7220 636f 6d6d 616e  ng Docker comman
+00002af0: 6473 2e0a 0a20 2020 2024 2064 6f63 6b65  ds...    $ docke
+00002b00: 7220 7374 6f70 2065 7665 6e74 7374 6f72  r stop eventstor
+00002b10: 6564 622d 7365 6375 7265 0a09 2420 646f  edb-secure..$ do
+00002b20: 636b 6572 2072 6d20 6576 656e 7473 746f  cker rm eventsto
+00002b30: 7265 6462 2d73 6563 7572 650a 0a54 6f20  redb-secure..To 
+00002b40: 7374 6f70 2061 6e64 2072 656d 6f76 6520  stop and remove 
+00002b50: 7468 6520 2269 6e73 6563 7572 6522 2063  the "insecure" c
+00002b60: 6f6e 7461 696e 6572 2c20 7573 6520 7468  ontainer, use th
+00002b70: 6520 666f 6c6c 6f77 696e 6720 446f 636b  e following Dock
+00002b80: 6572 2063 6f6d 6d61 6e64 732e 0a0a 2020  er commands...  
+00002b90: 2020 2420 646f 636b 6572 2073 746f 7020    $ docker stop 
+00002ba0: 6576 656e 7473 746f 7265 6462 2d69 6e73  eventstoredb-ins
+00002bb0: 6563 7572 650a 0924 2064 6f63 6b65 7220  ecure..$ docker 
+00002bc0: 726d 2065 7665 6e74 7374 6f72 6564 622d  rm eventstoredb-
+00002bd0: 696e 7365 6375 7265 0a0a 0a23 2320 4576  insecure...## Ev
+00002be0: 656e 7453 746f 7265 4442 2063 6c69 656e  entStoreDB clien
+00002bf0: 740a 0a54 6869 7320 4576 656e 7453 746f  t..This EventSto
+00002c00: 7265 4442 2063 6c69 656e 7420 6973 2069  reDB client is i
+00002c10: 6d70 6c65 6d65 6e74 6564 2069 6e20 7468  mplemented in th
+00002c20: 6520 6065 7364 6263 6c69 656e 7460 2070  e `esdbclient` p
+00002c30: 6163 6b61 6765 2077 6974 680a 7468 6520  ackage with.the 
+00002c40: 6045 5344 4243 6c69 656e 7460 2063 6c61  `ESDBClient` cla
+00002c50: 7373 2e0a 0a23 2323 2049 6d70 6f72 7420  ss...### Import 
+00002c60: 636c 6173 730a 0a54 6865 2060 4553 4442  class..The `ESDB
+00002c70: 436c 6965 6e74 6020 636c 6173 7320 6361  Client` class ca
+00002c80: 6e20 6265 2069 6d70 6f72 7465 6420 6672  n be imported fr
+00002c90: 6f6d 2074 6865 2060 6573 6462 636c 6965  om the `esdbclie
+00002ca0: 6e74 6020 7061 636b 6167 652e 0a0a 6060  nt` package...``
+00002cb0: 6070 7974 686f 6e0a 6672 6f6d 2065 7364  `python.from esd
+00002cc0: 6263 6c69 656e 7420 696d 706f 7274 2045  bclient import E
+00002cd0: 5344 4243 6c69 656e 740a 6060 600a 0a23  SDBClient.```..#
+00002ce0: 2323 2043 6f6e 7374 7275 6374 2063 6c69  ## Construct cli
+00002cf0: 656e 740a 0a54 6865 2060 4553 4442 436c  ent..The `ESDBCl
+00002d00: 6965 6e74 6020 636c 6173 7320 6361 6e20  ient` class can 
+00002d10: 6265 2063 6f6e 7374 7275 6374 6564 2077  be constructed w
+00002d20: 6974 6820 6120 6075 7269 6020 6172 6775  ith a `uri` argu
+00002d30: 6d65 6e74 2c20 7768 6963 6820 6973 2072  ment, which is r
+00002d40: 6571 7569 7265 642e 0a41 6e64 2c20 746f  equired..And, to
+00002d50: 2063 6f6e 6e65 6374 2074 6f20 6120 2273   connect to a "s
+00002d60: 6563 7572 6522 2045 7665 6e74 5374 6f72  ecure" EventStor
+00002d70: 6544 4220 7365 7276 6572 2c20 7468 6520  eDB server, the 
+00002d80: 6f70 7469 6f6e 616c 2060 726f 6f74 5f63  optional `root_c
+00002d90: 6572 7469 6669 6361 7465 7360 0a61 7267  ertificates`.arg
+00002da0: 756d 656e 7420 6973 2061 6c73 6f20 7265  ument is also re
+00002db0: 7175 6972 6564 2e0a 0a54 6865 2060 7572  quired...The `ur
+00002dc0: 6960 2061 7267 756d 656e 7420 6973 2065  i` argument is e
+00002dd0: 7870 6563 7465 6420 746f 2062 6520 616e  xpected to be an
+00002de0: 2045 7665 6e74 5374 6f72 6544 4220 636f   EventStoreDB co
+00002df0: 6e6e 6563 7469 6f6e 2073 7472 696e 6720  nnection string 
+00002e00: 5552 4920 7468 6174 0a63 6f6e 666f 726d  URI that.conform
+00002e10: 7320 7769 7468 2074 6865 2073 7461 6e64  s with the stand
+00002e20: 6172 6420 4576 656e 7453 746f 7265 4442  ard EventStoreDB
+00002e30: 2022 6573 6462 2220 6f72 2022 6573 6462   "esdb" or "esdb
+00002e40: 2b64 6973 636f 7665 7222 2055 5249 2073  +discover" URI s
+00002e50: 6368 656d 6573 2e20 5468 650a 7379 6e74  chemes. The.synt
+00002e60: 6178 2061 6e64 2073 656d 616e 7469 6373  ax and semantics
+00002e70: 206f 6620 4576 656e 7453 746f 7265 4442   of EventStoreDB
+00002e80: 2063 6f6e 6e65 6374 696f 6e20 7374 7269   connection stri
+00002e90: 6e67 7320 6172 6520 6578 706c 6169 6e65  ngs are explaine
+00002ea0: 6420 696e 2074 6865 204e 6f74 6573 0a73  d in the Notes.s
+00002eb0: 6563 7469 6f6e 2062 656c 6f77 2e0a 0a46  ection below...F
+00002ec0: 6f72 2065 7861 6d70 6c65 2c20 7468 6520  or example, the 
+00002ed0: 666f 6c6c 6f77 696e 6720 636f 6e6e 6563  following connec
+00002ee0: 7469 6f6e 2073 7472 696e 6720 7370 6563  tion string spec
+00002ef0: 6966 6965 7320 7468 6174 2074 6865 2063  ifies that the c
+00002f00: 6c69 656e 7420 7368 6f75 6c64 0a61 7474  lient should.att
+00002f10: 656d 7074 2074 6f20 6372 6561 6520 6120  empt to creae a 
+00002f20: 2273 6563 7572 6522 2063 6f6e 6e65 6374  "secure" connect
+00002f30: 696f 6e20 746f 2070 6f72 7420 3231 3133  ion to port 2113
+00002f40: 206f 6e20 226c 6f63 616c 686f 7374 222c   on "localhost",
+00002f50: 2061 6e64 2075 7365 2074 6865 0a63 7265   and use the.cre
+00002f60: 6465 6e74 6961 6c73 2022 7573 6572 6e61  dentials "userna
+00002f70: 6d65 2220 616e 6420 2270 6173 7377 6f72  me" and "passwor
+00002f80: 6422 2077 6865 6e20 6d61 6b69 6e67 2063  d" when making c
+00002f90: 616c 6c73 2074 6f20 7468 6520 7365 7276  alls to the serv
+00002fa0: 6572 2e0a 0a20 2020 2065 7364 623a 2f2f  er...    esdb://
+00002fb0: 7573 6572 6e61 6d65 3a70 6173 7377 6f72  username:passwor
+00002fc0: 6440 6c6f 6361 6c68 6f73 743a 3231 3133  d@localhost:2113
+00002fd0: 0a0a 5468 6520 636c 6965 6e74 206d 7573  ..The client mus
+00002fe0: 7420 6265 2063 6f6e 6669 6775 7265 6420  t be configured 
+00002ff0: 746f 2063 7265 6174 6520 6120 2273 6563  to create a "sec
+00003000: 7572 6522 2063 6f6e 6e65 6374 696f 6e20  ure" connection 
+00003010: 746f 2061 2022 7365 6375 7265 2220 7365  to a "secure" se
+00003020: 7276 6572 2c0a 616e 6420 616e 2022 696e  rver,.and an "in
+00003030: 7365 6375 7265 2220 636f 6e6e 6563 7469  secure" connecti
+00003040: 6f6e 2074 6f20 616e 2022 696e 7365 6375  on to an "insecu
+00003050: 7265 2220 7365 7276 6572 2e20 4279 2064  re" server. By d
+00003060: 6566 6175 6c74 2c20 7468 6520 636c 6965  efault, the clie
+00003070: 6e74 2077 696c 6c0a 6174 7465 6d70 7420  nt will.attempt 
+00003080: 746f 2063 7265 6174 6520 6120 2273 6563  to create a "sec
+00003090: 7572 6522 2063 6f6e 6e65 6374 696f 6e2e  ure" connection.
+000030a0: 2041 6e64 2073 6f2c 2077 6865 6e20 7573   And so, when us
+000030b0: 696e 6720 616e 2022 696e 7365 6375 7265  ing an "insecure
+000030c0: 2220 7365 7276 6572 2c0a 7468 6520 636f  " server,.the co
+000030d0: 6e6e 6563 7469 6f6e 2073 7472 696e 6720  nnection string 
+000030e0: 6d75 7374 2073 7065 6369 6679 2074 6861  must specify tha
+000030f0: 7420 7468 6520 636c 6965 6e74 2073 686f  t the client sho
+00003100: 756c 6420 6174 7465 6d70 7420 746f 206d  uld attempt to m
+00003110: 616b 6520 616e 2022 696e 7365 6375 7265  ake an "insecure
+00003120: 220a 636f 6e6e 6563 7469 6f6e 2e0a 0a54  ".connection...T
+00003130: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6e  he following con
+00003140: 6e65 6374 696f 6e20 7374 7269 6e67 2073  nection string s
+00003150: 7065 6369 6669 6573 2074 6861 7420 7468  pecifies that th
+00003160: 6520 636c 6965 6e74 2073 686f 756c 640a  e client should.
+00003170: 6174 7465 6d70 7420 746f 2063 7265 6165  attempt to creae
+00003180: 2061 6e20 2269 6e73 6563 7572 6522 2063   an "insecure" c
+00003190: 6f6e 6e65 6374 696f 6e20 746f 2070 6f72  onnection to por
+000031a0: 7420 3231 3134 206f 6e20 226c 6f63 616c  t 2114 on "local
+000031b0: 686f 7374 222e 0a57 6865 6e20 636f 6e6e  host"..When conn
+000031c0: 6563 7469 6e67 2074 6f20 616e 2022 696e  ecting to an "in
+000031d0: 7365 6375 7265 2220 7365 7276 6572 2c20  secure" server, 
+000031e0: 7468 6520 636c 6965 6e74 2077 696c 6c20  the client will 
+000031f0: 6967 6e6f 7265 2061 6e79 0a75 7365 726e  ignore any.usern
+00003200: 616d 6520 616e 6420 7061 7373 776f 7264  ame and password
+00003210: 2069 6e66 6f72 6d61 7469 6f6e 2069 6e63   information inc
+00003220: 6c75 6465 6420 696e 2074 6865 2063 6f6e  luded in the con
+00003230: 6e65 6374 696f 6e20 7374 7269 6e67 2e0a  nection string..
+00003240: 0a20 2020 2065 7364 623a 2f2f 6c6f 6361  .    esdb://loca
+00003250: 6c68 6f73 743a 3231 3134 3f54 6c73 3d66  lhost:2114?Tls=f
+00003260: 616c 7365 0a0a 556e 6c65 7373 2074 6865  alse..Unless the
+00003270: 2063 6f6e 6e65 6374 696f 6e20 7374 7269   connection stri
+00003280: 6e67 2055 5249 2069 6e63 6c75 6465 7320  ng URI includes 
+00003290: 7468 6520 6669 656c 642d 7661 6c75 6520  the field-value 
+000032a0: 6054 6c73 3d66 616c 7365 6020 696e 0a74  `Tls=false` in.t
+000032b0: 6865 2071 7565 7279 2073 7472 696e 672c  he query string,
+000032c0: 2074 6865 2060 726f 6f74 5f63 6572 7469   the `root_certi
+000032d0: 6669 6361 7465 7360 2063 6f6e 7374 7275  ficates` constru
+000032e0: 6374 6f72 2061 7267 756d 656e 7420 6973  ctor argument is
+000032f0: 2061 6c73 6f20 7265 7175 6972 6564 2e0a   also required..
+00003300: 0a57 6865 6e20 636f 6e6e 6563 7469 6e67  .When connecting
+00003310: 2074 6f20 6120 2273 6563 7572 6522 2073   to a "secure" s
+00003320: 6572 7665 722c 2074 6865 2060 726f 6f74  erver, the `root
+00003330: 5f63 6572 7469 6669 6361 7465 7360 2061  _certificates` a
+00003340: 7267 756d 656e 7420 6973 2065 7870 6563  rgument is expec
+00003350: 7465 6420 746f 0a62 6520 6120 5079 7468  ted to.be a Pyth
+00003360: 6f6e 2060 7374 7260 2063 6f6e 7461 696e  on `str` contain
+00003370: 696e 6720 5045 4d20 656e 636f 6465 6420  ing PEM encoded 
+00003380: 5353 4c2f 544c 5320 726f 6f74 2063 6572  SSL/TLS root cer
+00003390: 7469 6669 6361 7465 732c 2061 6e64 2069  tificates, and i
+000033a0: 7420 6973 2075 7365 6420 666f 720a 6175  t is used for.au
+000033b0: 7468 656e 7469 6361 7469 6e67 2074 6865  thenticating the
+000033c0: 2073 6572 7665 7220 746f 2074 6865 2063   server to the c
+000033d0: 6c69 656e 742e 2054 6869 7320 7661 6c75  lient. This valu
+000033e0: 6520 6973 2070 6173 7365 6420 6469 7265  e is passed dire
+000033f0: 6374 6c79 2074 6f0a 6067 7270 632e 7373  ctly to.`grpc.ss
+00003400: 6c5f 6368 616e 6e65 6c5f 6372 6564 656e  l_channel_creden
+00003410: 7469 616c 7328 2960 2e20 4974 2069 7320  tials()`. It is 
+00003420: 636f 6d6d 6f6e 6c79 2074 6865 2063 6572  commonly the cer
+00003430: 7469 6669 6361 7465 206f 6620 7468 6520  tificate of the 
+00003440: 6365 7274 6966 6963 6174 650a 6175 7468  certificate.auth
+00003450: 6f72 6974 7920 7468 6174 2077 6173 2072  ority that was r
+00003460: 6573 706f 6e73 6962 6c65 2066 6f72 2067  esponsible for g
+00003470: 656e 6572 6174 696e 6720 7468 6520 5353  enerating the SS
+00003480: 4c2f 544c 5320 6365 7274 6966 6963 6174  L/TLS certificat
+00003490: 6520 7573 6564 2062 7920 7468 650a 4576  e used by the.Ev
+000034a0: 656e 7453 746f 7265 4442 2073 6572 7665  entStoreDB serve
+000034b0: 722e 2042 7574 2c20 616c 7465 726e 6174  r. But, alternat
+000034c0: 6976 656c 7920 666f 7220 6465 7665 6c6f  ively for develo
+000034d0: 706d 656e 742c 2079 6f75 2063 616e 2075  pment, you can u
+000034e0: 7365 2074 6865 2073 6572 7665 7227 730a  se the server's.
+000034f0: 6365 7274 6966 6963 6174 6520 6974 7365  certificate itse
+00003500: 6c66 2e0a 0a49 6e20 7468 6520 6578 616d  lf...In the exam
+00003510: 706c 6520 6265 6c6f 772c 2074 6865 2063  ple below, the c
+00003520: 6f6e 7374 7275 6374 6f72 2061 7267 756d  onstructor argum
+00003530: 656e 7420 7661 6c75 6573 2061 7265 2074  ent values are t
+00003540: 616b 656e 2066 726f 6d20 7468 6520 6f70  aken from the op
+00003550: 6572 6174 696e 670a 7379 7374 656d 2065  erating.system e
+00003560: 6e76 6972 6f6e 6d65 6e74 2e20 5468 6973  nvironment. This
+00003570: 2069 7320 6120 7479 7069 6361 6c20 6172   is a typical ar
+00003580: 7261 6e67 656d 656e 7420 696e 2061 2070  rangement in a p
+00003590: 726f 6475 6374 696f 6e20 656e 7669 726f  roduction enviro
+000035a0: 6e6d 656e 742e 0a0a 6060 6070 7974 686f  nment...```pytho
+000035b0: 6e0a 696d 706f 7274 206f 730a 0a63 6c69  n.import os..cli
+000035c0: 656e 7420 3d20 4553 4442 436c 6965 6e74  ent = ESDBClient
+000035d0: 280a 2020 2020 7572 693d 6f73 2e67 6574  (.    uri=os.get
+000035e0: 656e 7628 2245 5344 425f 5552 4922 292c  env("ESDB_URI"),
+000035f0: 0a20 2020 2072 6f6f 745f 6365 7274 6966  .    root_certif
+00003600: 6963 6174 6573 3d6f 732e 6765 7465 6e76  icates=os.getenv
+00003610: 2822 4553 4442 5f52 4f4f 545f 4345 5254  ("ESDB_ROOT_CERT
+00003620: 4946 4943 4154 4553 2229 2c0a 290a 6060  IFICATES"),.).``
+00003630: 600a 0a0a 2323 2053 7472 6561 6d73 0a0a  `...## Streams..
+00003640: 496e 2045 7665 6e74 5374 6f72 6544 422c  In EventStoreDB,
+00003650: 2061 2022 7374 7265 616d 2220 6973 2061   a "stream" is a
+00003660: 2073 6571 7565 6e63 6520 6f66 2072 6563   sequence of rec
+00003670: 6f72 6465 6420 6576 656e 7473 2074 6861  orded events tha
+00003680: 7420 616c 6c20 6861 7665 0a74 6865 2073  t all have.the s
+00003690: 616d 6520 2273 7472 6561 6d20 6e61 6d65  ame "stream name
+000036a0: 222e 2054 6865 7265 2077 696c 6c20 6e6f  ". There will no
+000036b0: 726d 616c 6c79 2062 6520 6d61 6e79 2073  rmally be many s
+000036c0: 7472 6561 6d73 2069 6e20 6120 6461 7461  treams in a data
+000036d0: 6261 7365 2e0a 4561 6368 2072 6563 6f72  base..Each recor
+000036e0: 6465 6420 6576 656e 7420 6861 7320 6120  ded event has a 
+000036f0: 2273 7472 6561 6d20 706f 7369 7469 6f6e  "stream position
+00003700: 2220 696e 2069 7473 2073 7472 6561 6d2c  " in its stream,
+00003710: 2061 6e64 2061 2022 636f 6d6d 6974 2070   and a "commit p
+00003720: 6f73 6974 696f 6e22 0a69 6e20 7468 6520  osition".in the 
+00003730: 6461 7461 6261 7365 2e20 5468 6520 7374  database. The st
+00003740: 7265 616d 2070 6f73 6974 696f 6e73 206f  ream positions o
+00003750: 6620 7468 6520 7265 636f 7264 6564 2065  f the recorded e
+00003760: 7665 6e74 7320 696e 2061 2073 7472 6561  vents in a strea
+00003770: 6d20 6973 2061 2067 6170 6c65 7373 0a73  m is a gapless.s
+00003780: 6571 7565 6e63 6520 7374 6172 7469 6e67  equence starting
+00003790: 2066 726f 6d20 7a65 726f 2e20 5468 6520   from zero. The 
+000037a0: 636f 6d6d 6974 2070 6f73 6974 696f 6e73  commit positions
+000037b0: 206f 6620 7468 6520 7265 636f 7264 6564   of the recorded
+000037c0: 2065 7665 6e74 7320 696e 2074 6865 2064   events in the d
+000037d0: 6174 6162 6173 650a 666f 726d 2061 2073  atabase.form a s
+000037e0: 6571 7565 6e63 6520 7468 6174 2069 7320  equence that is 
+000037f0: 6e6f 7420 6761 706c 6573 732e 0a0a 5468  not gapless...Th
+00003800: 6520 6d65 7468 6f64 7320 6061 7070 656e  e methods `appen
+00003810: 645f 6576 656e 7473 2829 602c 2060 7265  d_events()`, `re
+00003820: 6164 5f73 7472 6561 6d5f 6576 656e 7473  ad_stream_events
+00003830: 2829 6020 616e 6420 6072 6561 645f 616c  ()` and `read_al
+00003840: 6c5f 6576 656e 7473 2829 6020 6361 6e0a  l_events()` can.
+00003850: 6265 2075 7365 6420 746f 2072 6563 6f72  be used to recor
+00003860: 6420 616e 6420 7265 6164 2065 7665 6e74  d and read event
+00003870: 7320 696e 2074 6865 2064 6174 6162 6173  s in the databas
+00003880: 652e 0a0a 2323 2320 4170 7065 6e64 2065  e...### Append e
+00003890: 7665 6e74 730a 0a54 6865 2060 6170 7065  vents..The `appe
+000038a0: 6e64 5f65 7665 6e74 7328 2960 206d 6574  nd_events()` met
+000038b0: 686f 6420 6361 6e20 6265 2075 7365 6420  hod can be used 
+000038c0: 746f 2077 7269 7465 2061 2073 6571 7565  to write a seque
+000038d0: 6e63 6520 6f66 206e 6577 2065 7665 6e74  nce of new event
+000038e0: 7320 6174 6f6d 6963 616c 6c79 0a74 6f20  s atomically.to 
+000038f0: 6120 2273 7472 6561 6d22 2e20 5772 6974  a "stream". Writ
+00003900: 696e 6720 6e65 7720 6576 656e 7473 2065  ing new events e
+00003910: 6974 6865 7220 6372 6561 7465 7320 6120  ither creates a 
+00003920: 7374 7265 616d 2c20 6f72 2061 7070 656e  stream, or appen
+00003930: 6473 2065 7665 6e74 7320 746f 2074 6865  ds events to the
+00003940: 2065 6e64 0a6f 6620 6120 7374 7265 616d   end.of a stream
+00003950: 2e20 5468 6973 206d 6574 686f 6420 6973  . This method is
+00003960: 2069 6465 6d70 6f74 656e 7420 2873 6565   idempotent (see
+00003970: 2062 656c 6f77 292e 0a0a 5468 6973 206d   below)...This m
+00003980: 6574 686f 6420 6361 6e20 6265 2075 7365  ethod can be use
+00003990: 6420 746f 2072 6563 6f72 6420 6174 6f6d  d to record atom
+000039a0: 6963 616c 6c79 2061 6c6c 2074 6865 206e  ically all the n
+000039b0: 6577 0a65 7665 6e74 7320 7468 6174 2061  ew.events that a
+000039c0: 7265 2067 656e 6572 6174 6564 2077 6865  re generated whe
+000039d0: 6e20 6578 6563 7574 696e 6720 6120 636f  n executing a co
+000039e0: 6d6d 616e 6420 696e 2061 6e20 6170 706c  mmand in an appl
+000039f0: 6963 6174 696f 6e2e 0a0a 5468 7265 6520  ication...Three 
+00003a00: 6172 6775 6d65 6e74 7320 6172 6520 7265  arguments are re
+00003a10: 7175 6972 6564 2c20 6073 7472 6561 6d5f  quired, `stream_
+00003a20: 6e61 6d65 602c 2060 6578 7065 6374 6564  name`, `expected
+00003a30: 5f70 6f73 6974 696f 6e60 0a61 6e64 2060  _position`.and `
+00003a40: 6576 656e 7473 602e 0a0a 5468 6520 6073  events`...The `s
+00003a50: 7472 6561 6d5f 6e61 6d65 6020 6172 6775  tream_name` argu
+00003a60: 6d65 6e74 2069 7320 7265 7175 6972 6564  ment is required
+00003a70: 2c20 616e 6420 6973 2065 7870 6563 7465  , and is expecte
+00003a80: 6420 746f 2062 6520 6120 5079 7468 6f6e  d to be a Python
+00003a90: 0a60 7374 7260 206f 626a 6563 7420 7468  .`str` object th
+00003aa0: 6174 2075 6e69 7175 656c 7920 6964 656e  at uniquely iden
+00003ab0: 7469 6669 6573 2074 6865 2073 7472 6561  tifies the strea
+00003ac0: 6d20 696e 2074 6865 2064 6174 6162 6173  m in the databas
+00003ad0: 652e 0a0a 5468 6520 6065 7870 6563 7465  e...The `expecte
+00003ae0: 645f 706f 7369 7469 6f6e 6020 6172 6775  d_position` argu
+00003af0: 6d65 6e74 2069 7320 7265 7175 6972 6564  ment is required
+00003b00: 2c20 6973 2065 7870 6563 7465 6420 746f  , is expected to
+00003b10: 2062 653a 2060 4e6f 6e65 600a 6966 2065   be: `None`.if e
+00003b20: 7665 6e74 7320 6172 6520 6265 696e 6720  vents are being 
+00003b30: 7772 6974 7465 6e20 746f 2061 206e 6577  written to a new
+00003b40: 2073 7472 6561 6d2c 2061 6e64 206f 7468   stream, and oth
+00003b50: 6572 7769 7365 2061 6e20 5079 7468 6f6e  erwise an Python
+00003b60: 2060 696e 7460 0a65 7175 616c 2074 6f20   `int`.equal to 
+00003b70: 7468 6520 706f 7369 7469 6f6e 2069 6e20  the position in 
+00003b80: 7468 6520 7374 7265 616d 206f 6620 7468  the stream of th
+00003b90: 6520 6c61 7374 2072 6563 6f72 6465 6420  e last recorded 
+00003ba0: 6576 656e 7420 696e 2074 6865 2073 7472  event in the str
+00003bb0: 6561 6d2e 0a0a 5468 6520 6065 7665 6e74  eam...The `event
+00003bc0: 7360 2061 7267 756d 656e 7420 6973 2072  s` argument is r
+00003bd0: 6571 7569 7265 642c 2061 6e64 2069 7320  equired, and is 
+00003be0: 6578 7065 6374 6564 2074 6f20 6265 2061  expected to be a
+00003bf0: 2073 6571 7565 6e63 6520 6f66 206e 6577   sequence of new
+00003c00: 0a65 7665 6e74 206f 626a 6563 7473 2074  .event objects t
+00003c10: 6f20 6265 2061 7070 656e 6465 6420 746f  o be appended to
+00003c20: 2074 6865 206e 616d 6564 2073 7472 6561   the named strea
+00003c30: 6d2e 2054 6865 2060 4e65 7745 7665 6e74  m. The `NewEvent
+00003c40: 6020 636c 6173 7320 7368 6f75 6c64 0a62  ` class should.b
+00003c50: 6520 7573 6564 2074 6f20 636f 6e73 7472  e used to constr
+00003c60: 7563 7420 6e65 7720 6576 656e 7420 6f62  uct new event ob
+00003c70: 6a65 6374 7320 2873 6565 2062 656c 6f77  jects (see below
+00003c80: 292e 0a0a 5468 6973 206d 6574 686f 6420  )...This method 
+00003c90: 7461 6b65 7320 616e 206f 7074 696f 6e61  takes an optiona
+00003ca0: 6c20 6074 696d 656f 7574 6020 6172 6775  l `timeout` argu
+00003cb0: 6d65 6e74 2c20 7768 6963 6820 6973 2061  ment, which is a
+00003cc0: 2050 7974 686f 6e20 6066 6c6f 6174 6020   Python `float` 
+00003cd0: 7468 6174 2073 6574 730a 6120 6465 6164  that sets.a dead
+00003ce0: 6c69 6e65 2066 6f72 2074 6865 2063 6f6d  line for the com
+00003cf0: 706c 6574 696f 6e20 6f66 2074 6865 2067  pletion of the g
+00003d00: 5250 4320 6f70 6572 6174 696f 6e2e 0a0a  RPC operation...
+00003d10: 5374 7265 616d 7320 6172 6520 6372 6561  Streams are crea
+00003d20: 7465 6420 6279 2077 7269 7469 6e67 2065  ted by writing e
+00003d30: 7665 6e74 732e 2054 6865 2063 6f72 7265  vents. The corre
+00003d40: 6374 2076 616c 7565 206f 6620 7468 6520  ct value of the 
+00003d50: 6065 7870 6563 7465 645f 706f 7369 7469  `expected_positi
+00003d60: 6f6e 600a 6172 6775 6d65 6e74 2077 6865  on`.argument whe
+00003d70: 6e20 7772 6974 696e 6720 7468 6520 6669  n writing the fi
+00003d80: 7273 7420 6576 656e 7420 6f66 2061 206e  rst event of a n
+00003d90: 6577 2073 7472 6561 6d20 6973 2060 4e6f  ew stream is `No
+00003da0: 6e65 602e 2050 6c65 6173 6520 6e6f 7465  ne`. Please note
+00003db0: 2c20 6974 2069 730a 6e6f 7420 706f 7373  , it is.not poss
+00003dc0: 6962 6c65 2074 6f20 736f 6d65 686f 7720  ible to somehow 
+00003dd0: 6372 6561 7465 2061 6e20 2265 6d70 7479  create an "empty
+00003de0: 2220 7374 7265 616d 2069 6e20 4576 656e  " stream in Even
+00003df0: 7453 746f 7265 4442 2e0a 0a54 6865 2073  tStoreDB...The s
+00003e00: 7472 6561 6d20 706f 7369 7469 6f6e 7320  tream positions 
+00003e10: 6f66 2072 6563 6f72 6465 6420 6576 656e  of recorded even
+00003e20: 7473 2069 6e20 6120 7374 7265 616d 2073  ts in a stream s
+00003e30: 7461 7274 2066 726f 6d20 7a65 726f 2c20  tart from zero, 
+00003e40: 616e 6420 666f 726d 2061 2067 6170 6c65  and form a gaple
+00003e50: 7373 0a73 6571 7565 6e63 6520 6f66 2069  ss.sequence of i
+00003e60: 6e74 6567 6572 732e 2054 6865 2073 7472  ntegers. The str
+00003e70: 6561 6d20 706f 7369 7469 6f6e 206f 6620  eam position of 
+00003e80: 7468 6520 6669 7273 7420 7265 636f 7264  the first record
+00003e90: 6564 2065 7665 6e74 2069 6e20 6120 7374  ed event in a st
+00003ea0: 7265 616d 2069 730a 6030 602e 2041 6e64  ream is.`0`. And
+00003eb0: 2073 6f20 7768 656e 2061 7070 656e 6469   so when appendi
+00003ec0: 6e67 2074 6865 2073 6563 6f6e 6420 6e65  ng the second ne
+00003ed0: 7720 6576 656e 7420 746f 2061 2073 7472  w event to a str
+00003ee0: 6561 6d20 7468 6174 2068 6173 206f 6e65  eam that has one
+00003ef0: 2072 6563 6f72 6465 6420 6576 656e 742c   recorded event,
+00003f00: 0a74 6865 2063 6f72 7265 6374 2076 616c  .the correct val
+00003f10: 7565 206f 6620 7468 6520 6065 7870 6563  ue of the `expec
+00003f20: 7465 645f 706f 7369 7469 6f6e 6020 6172  ted_position` ar
+00003f30: 6775 6d65 6e74 2069 7320 6030 602e 2053  gument is `0`. S
+00003f40: 696d 696c 6172 6c79 2c20 7468 6520 7374  imilarly, the st
+00003f50: 7265 616d 0a70 6f73 6974 696f 6e20 6f66  ream.position of
+00003f60: 2074 6865 2073 6563 6f6e 6420 7265 636f   the second reco
+00003f70: 7264 6564 2065 7665 6e74 2069 6e20 6120  rded event in a 
+00003f80: 7374 7265 616d 2069 7320 6031 602c 2061  stream is `1`, a
+00003f90: 6e64 2073 6f20 7768 656e 2061 7070 656e  nd so when appen
+00003fa0: 6469 6e67 2074 6865 0a74 6869 7264 206e  ding the.third n
+00003fb0: 6577 2065 7665 6e74 2074 6f20 6120 7374  ew event to a st
+00003fc0: 7265 616d 2074 6861 7420 6861 7320 7477  ream that has tw
+00003fd0: 6f20 7265 636f 7264 6564 2065 7665 6e74  o recorded event
+00003fe0: 732c 2074 6865 2063 6f72 7265 6374 2076  s, the correct v
+00003ff0: 616c 7565 206f 6620 7468 650a 6065 7870  alue of the.`exp
+00004000: 6563 7465 645f 706f 7369 7469 6f6e 6020  ected_position` 
+00004010: 6172 6775 6d65 6e74 2069 7320 6031 602e  argument is `1`.
+00004020: 2041 6e64 2073 6f20 6f6e 2e2e 2e20 2854   And so on... (T
+00004030: 6865 7265 2069 7320 6120 7468 656f 7265  here is a theore
+00004040: 7469 6361 6c20 6d61 7869 6d75 6d0a 6e75  tical maximum.nu
+00004050: 6d62 6572 206f 6620 7265 636f 7264 6564  mber of recorded
+00004060: 2065 7665 6e74 7320 7468 6174 2061 6e79   events that any
+00004070: 2073 7472 6561 6d20 6361 6e20 6861 7665   stream can have
+00004080: 2c20 6275 7420 4927 6d20 6e6f 7420 7375  , but I'm not su
+00004090: 7265 2077 6861 7420 6974 2069 733b 0a6d  re what it is;.m
+000040a0: 6179 6265 2039 2c32 3233 2c33 3732 2c30  aybe 9,223,372,0
+000040b0: 3336 2c38 3534 2c37 3735 2c38 3037 2062  36,854,775,807 b
+000040c0: 6563 6175 7365 2069 7420 6973 2069 6d70  ecause it is imp
+000040d0: 6c65 6d65 6e74 6564 2061 7320 6120 606c  lemented as a `l
+000040e0: 6f6e 6760 2069 6e20 4323 3f29 0a0a 4966  ong` in C#?)..If
+000040f0: 2074 6865 7265 2069 7320 6120 6d69 736d   there is a mism
+00004100: 6174 6368 2062 6574 7765 656e 2074 6865  atch between the
+00004110: 2067 6976 656e 2076 616c 7565 206f 6620   given value of 
+00004120: 7468 6520 6065 7870 6563 7465 645f 706f  the `expected_po
+00004130: 7369 7469 6f6e 6020 6172 6775 6d65 6e74  sition` argument
+00004140: 0a61 6e64 2074 6865 2070 6f73 6974 696f  .and the positio
+00004150: 6e20 6f66 2074 6865 206c 6173 7420 7265  n of the last re
+00004160: 636f 7264 6564 2065 7665 6e74 2069 6e20  corded event in 
+00004170: 6120 7374 7265 616d 2c20 7468 656e 2061  a stream, then a
+00004180: 6e20 6045 7870 6563 7465 6450 6f73 6974  n `ExpectedPosit
+00004190: 696f 6e45 7272 6f72 600a 6578 6365 7074  ionError`.except
+000041a0: 696f 6e20 7769 6c6c 2062 6520 7261 6973  ion will be rais
+000041b0: 6564 2e20 5468 6973 2065 6666 6563 7469  ed. This effecti
+000041c0: 7665 6c79 2061 6363 6f6d 706c 6973 6865  vely accomplishe
+000041d0: 7320 6f70 7469 6d69 7374 6963 2063 6f6e  s optimistic con
+000041e0: 6375 7272 656e 6379 2063 6f6e 7472 6f6c  currency control
+000041f0: 2e0a 0a49 6620 796f 7520 7769 7368 2074  ...If you wish t
+00004200: 6f20 6469 7361 626c 6520 6f70 7469 6d69  o disable optimi
+00004210: 7374 6963 2063 6f6e 6375 7272 656e 6379  stic concurrency
+00004220: 2063 6f6e 7472 6f6c 2077 6865 6e20 6170   control when ap
+00004230: 7065 6e64 696e 6720 6e65 7720 6576 656e  pending new even
+00004240: 7473 2c20 796f 750a 6361 6e20 7365 7420  ts, you.can set 
+00004250: 7468 6520 6065 7870 6563 7465 645f 706f  the `expected_po
+00004260: 7369 7469 6f6e 6020 746f 2061 206e 6567  sition` to a neg
+00004270: 6174 6976 6520 696e 7465 6765 722e 0a0a  ative integer...
+00004280: 4966 2079 6f75 206e 6565 6420 746f 2064  If you need to d
+00004290: 6973 636f 7665 7220 7468 6520 6375 7272  iscover the curr
+000042a0: 656e 7420 706f 7369 7469 6f6e 206f 6620  ent position of 
+000042b0: 7468 6520 6c61 7374 2072 6563 6f72 6465  the last recorde
+000042c0: 6420 6576 656e 7420 696e 2061 2073 7472  d event in a str
+000042d0: 6561 6d2c 0a79 6f75 2063 616e 2075 7365  eam,.you can use
+000042e0: 2074 6865 2060 6765 745f 7374 7265 616d   the `get_stream
+000042f0: 5f70 6f73 6974 696f 6e28 2960 206d 6574  _position()` met
+00004300: 686f 6420 2873 6565 2062 656c 6f77 292e  hod (see below).
+00004310: 0a0a 506c 6561 7365 206e 6f74 652c 2074  ..Please note, t
+00004320: 6865 2061 7070 656e 6420 6576 656e 7473  he append events
+00004330: 206f 7065 7261 7469 6f6e 2069 7320 6174   operation is at
+00004340: 6f6d 6963 2c20 736f 2074 6861 7420 6569  omic, so that ei
+00004350: 7468 6572 2061 6c6c 0a6f 7220 6e6f 6e65  ther all.or none
+00004360: 206f 6620 7468 6520 6769 7665 6e20 6e65   of the given ne
+00004370: 7720 6576 656e 7473 2077 696c 6c20 6265  w events will be
+00004380: 2072 6563 6f72 6465 642e 2042 7920 6465   recorded. By de
+00004390: 7369 676e 2c20 6974 2069 7320 6f6e 6c79  sign, it is only
+000043a0: 0a70 6f73 7369 626c 6520 7769 7468 2045  .possible with E
+000043b0: 7665 6e74 5374 6f72 6544 4220 746f 2061  ventStoreDB to a
+000043c0: 746f 6d69 6361 6c6c 7920 7265 636f 7264  tomically record
+000043d0: 206e 6577 2065 7665 6e74 7320 696e 206f   new events in o
+000043e0: 6e65 2073 7472 6561 6d2e 0a0a 496e 2074  ne stream...In t
+000043f0: 6865 2065 7861 6d70 6c65 2062 656c 6f77  he example below
+00004400: 2c20 6120 6e65 7720 6576 656e 7420 6973  , a new event is
+00004410: 2061 7070 656e 6465 6420 746f 2061 206e   appended to a n
+00004420: 6577 2073 7472 6561 6d2e 0a0a 6060 6070  ew stream...```p
+00004430: 7974 686f 6e0a 6672 6f6d 2075 7569 6420  ython.from uuid 
+00004440: 696d 706f 7274 2075 7569 6434 0a0a 6672  import uuid4..fr
+00004450: 6f6d 2065 7364 6263 6c69 656e 7420 696d  om esdbclient im
+00004460: 706f 7274 204e 6577 4576 656e 740a 0a23  port NewEvent..#
+00004470: 2043 6f6e 7374 7275 6374 206e 6577 2065   Construct new e
+00004480: 7665 6e74 206f 626a 6563 742e 0a65 7665  vent object..eve
+00004490: 6e74 3120 3d20 4e65 7745 7665 6e74 2874  nt1 = NewEvent(t
+000044a0: 7970 653d 274f 7264 6572 4372 6561 7465  ype='OrderCreate
+000044b0: 6427 2c20 6461 7461 3d62 2764 6174 6131  d', data=b'data1
+000044c0: 2729 0a0a 2320 4465 6669 6e65 2073 7472  ')..# Define str
+000044d0: 6561 6d20 6e61 6d65 2e0a 7374 7265 616d  eam name..stream
+000044e0: 5f6e 616d 6531 203d 2073 7472 2875 7569  _name1 = str(uui
+000044f0: 6434 2829 290a 0a23 2041 7070 656e 6420  d4())..# Append 
+00004500: 6c69 7374 206f 6620 6576 656e 7473 2074  list of events t
+00004510: 6f20 6e65 7720 7374 7265 616d 2e0a 636f  o new stream..co
+00004520: 6d6d 6974 5f70 6f73 6974 696f 6e31 203d  mmit_position1 =
+00004530: 2063 6c69 656e 742e 6170 7065 6e64 5f65   client.append_e
+00004540: 7665 6e74 7328 0a20 2020 2073 7472 6561  vents(.    strea
+00004550: 6d5f 6e61 6d65 3d73 7472 6561 6d5f 6e61  m_name=stream_na
+00004560: 6d65 312c 0a20 2020 2065 7870 6563 7465  me1,.    expecte
+00004570: 645f 706f 7369 7469 6f6e 3d4e 6f6e 652c  d_position=None,
+00004580: 0a20 2020 2065 7665 6e74 733d 5b65 7665  .    events=[eve
+00004590: 6e74 315d 2c0a 290a 6060 600a 0a49 6e20  nt1],.).```..In 
+000045a0: 7468 6520 6578 616d 706c 6520 6265 6c6f  the example belo
+000045b0: 772c 2074 776f 2073 7562 7365 7175 656e  w, two subsequen
+000045c0: 7420 6576 656e 7473 2061 7265 2061 7070  t events are app
+000045d0: 656e 6465 6420 746f 2061 6e20 6578 6973  ended to an exis
+000045e0: 7469 6e67 0a73 7472 6561 6d2e 0a0a 6060  ting.stream...``
+000045f0: 6070 7974 686f 6e0a 6576 656e 7432 203d  `python.event2 =
+00004600: 204e 6577 4576 656e 7428 7479 7065 3d27   NewEvent(type='
+00004610: 4f72 6465 7255 7064 6174 6564 272c 2064  OrderUpdated', d
+00004620: 6174 613d 6227 6461 7461 3227 290a 6576  ata=b'data2').ev
+00004630: 656e 7433 203d 204e 6577 4576 656e 7428  ent3 = NewEvent(
+00004640: 7479 7065 3d27 4f72 6465 7244 656c 6574  type='OrderDelet
+00004650: 6564 272c 2064 6174 613d 6227 6461 7461  ed', data=b'data
+00004660: 3327 290a 0a63 6f6d 6d69 745f 706f 7369  3')..commit_posi
+00004670: 7469 6f6e 3220 3d20 636c 6965 6e74 2e61  tion2 = client.a
+00004680: 7070 656e 645f 6576 656e 7473 280a 2020  ppend_events(.  
+00004690: 2020 7374 7265 616d 5f6e 616d 653d 7374    stream_name=st
+000046a0: 7265 616d 5f6e 616d 6531 2c0a 2020 2020  ream_name1,.    
+000046b0: 6578 7065 6374 6564 5f70 6f73 6974 696f  expected_positio
+000046c0: 6e3d 302c 0a20 2020 2065 7665 6e74 733d  n=0,.    events=
+000046d0: 5b65 7665 6e74 322c 2065 7665 6e74 335d  [event2, event3]
+000046e0: 2c0a 290a 6060 600a 0a49 6620 7468 6520  ,.).```..If the 
+000046f0: 6f70 6572 6174 696f 6e20 6973 2073 7563  operation is suc
+00004700: 6365 7373 6675 6c2c 2074 6869 7320 6d65  cessful, this me
+00004710: 7468 6f64 2072 6574 7572 6e73 2061 6e20  thod returns an 
+00004720: 696e 7465 6765 720a 7265 7072 6573 656e  integer.represen
+00004730: 7469 6e67 2074 6865 206f 7665 7261 6c6c  ting the overall
+00004740: 2022 636f 6d6d 6974 2070 6f73 6974 696f   "commit positio
+00004750: 6e22 2061 7320 6974 2077 6173 2077 6865  n" as it was whe
+00004760: 6e20 7468 6520 6f70 6572 6174 696f 6e0a  n the operation.
+00004770: 7761 7320 636f 6d70 6c65 7465 642e 204f  was completed. O
+00004780: 7468 6572 7769 7365 2c20 616e 2065 7863  therwise, an exc
+00004790: 6570 7469 6f6e 2077 696c 6c20 6265 2072  eption will be r
+000047a0: 6169 7365 642e 0a0a 4120 2263 6f6d 6d69  aised...A "commi
+000047b0: 7420 706f 7369 7469 6f6e 2220 6973 2061  t position" is a
+000047c0: 206d 6f6e 6f74 6f6e 6963 616c 6c79 2069   monotonically i
+000047d0: 6e63 7265 6173 696e 6720 696e 7465 6765  ncreasing intege
+000047e0: 7220 7265 7072 6573 656e 7469 6e67 0a74  r representing.t
+000047f0: 6865 2070 6f73 6974 696f 6e20 6f66 2074  he position of t
+00004800: 6865 2072 6563 6f72 6465 6420 6576 656e  he recorded even
+00004810: 7420 696e 2061 2022 746f 7461 6c20 6f72  t in a "total or
+00004820: 6465 7222 206f 6620 616c 6c20 7265 636f  der" of all reco
+00004830: 7264 6564 0a65 7665 6e74 7320 696e 2074  rded.events in t
+00004840: 6865 2064 6174 6162 6173 6520 6163 726f  he database acro
+00004850: 7373 2061 6c6c 2073 7472 6561 6d73 2e20  ss all streams. 
+00004860: 4974 2069 7320 7468 6520 6163 7475 616c  It is the actual
+00004870: 2070 6f73 6974 696f 6e0a 6f66 2074 6865   position.of the
+00004880: 2065 7665 6e74 2072 6563 6f72 6420 6f6e   event record on
+00004890: 2064 6973 6b2c 2061 6e64 2074 6865 7265   disk, and there
+000048a0: 2061 7265 2075 7375 616c 6c79 206c 6172   are usually lar
+000048b0: 6765 2064 6966 6665 7265 6e63 6573 0a62  ge differences.b
+000048c0: 6574 7765 656e 2073 7563 6365 7373 6976  etween successiv
+000048d0: 6520 636f 6d6d 6974 732e 2049 6e20 636f  e commits. In co
+000048e0: 6e73 6571 7565 6e63 652c 2074 6865 2073  nsequence, the s
+000048f0: 6571 7565 6e63 6520 6f66 2063 6f6d 6d69  equence of commi
+00004900: 740a 706f 7369 7469 6f6e 7320 6973 206e  t.positions is n
+00004910: 6f74 2067 6170 6c65 7373 2e20 496e 6465  ot gapless. Inde
+00004920: 6564 2c20 7468 6572 6520 6172 6520 7573  ed, there are us
+00004930: 7561 6c6c 7920 6c61 7267 6520 6469 6666  ually large diff
+00004940: 6572 656e 6365 730a 6265 7477 6565 6e20  erences.between 
+00004950: 7468 6520 636f 6d6d 6974 2070 6f73 6974  the commit posit
+00004960: 696f 6e73 206f 6620 7375 6363 6573 7369  ions of successi
+00004970: 7665 2072 6563 6f72 6465 6420 6576 656e  ve recorded even
+00004980: 7473 2e0a 0a54 6865 2022 636f 6d6d 6974  ts...The "commit
+00004990: 2070 6f73 6974 696f 6e22 2072 6574 7572   position" retur
+000049a0: 6e65 6420 6279 2060 6170 7065 6e64 5f65  ned by `append_e
+000049b0: 7665 6e74 7328 2960 2069 7320 7468 6174  vents()` is that
+000049c0: 206f 6620 7468 6520 6c61 7374 0a72 6563   of the last.rec
+000049d0: 6f72 6465 6420 6576 656e 7420 696e 2074  orded event in t
+000049e0: 6865 2067 6976 656e 2062 6174 6368 206f  he given batch o
+000049f0: 6620 6e65 7720 6576 656e 7473 2e0a 0a54  f new events...T
+00004a00: 6865 2022 636f 6d6d 6974 2070 6f73 6974  he "commit posit
+00004a10: 696f 6e22 2072 6574 7572 6e65 6420 696e  ion" returned in
+00004a20: 2074 6869 7320 7761 7920 6361 6e20 7468   this way can th
+00004a30: 6572 6566 6f72 6520 6265 2075 7365 6420  erefore be used 
+00004a40: 746f 2077 6169 740a 666f 7220 6120 646f  to wait.for a do
+00004a50: 776e 7374 7265 616d 2063 6f6d 706f 6e65  wnstream compone
+00004a60: 6e74 2074 6f20 6861 7665 2070 726f 6365  nt to have proce
+00004a70: 7373 6564 2061 6c6c 2074 6865 2065 7665  ssed all the eve
+00004a80: 6e74 7320 7468 6174 2077 6572 6520 7265  nts that were re
+00004a90: 636f 7264 6564 2e0a 0a46 6f72 2065 7861  corded...For exa
+00004aa0: 6d70 6c65 2c20 636f 6e73 6964 6572 2061  mple, consider a
+00004ab0: 2075 7365 7220 696e 7465 7266 6163 6520   user interface 
+00004ac0: 636f 6d6d 616e 6420 7468 6174 2072 6573  command that res
+00004ad0: 756c 7473 2069 6e20 7468 6520 7265 636f  ults in the reco
+00004ae0: 7264 696e 670a 6f66 206e 6577 2065 7665  rding.of new eve
+00004af0: 6e74 732c 2061 6e64 2061 2071 7565 7279  nts, and a query
+00004b00: 2069 6e74 6f20 616e 2065 7665 6e74 7561   into an eventua
+00004b10: 6c6c 7920 636f 6e73 6973 7465 6e74 206d  lly consistent m
+00004b20: 6174 6572 6961 6c69 7a65 640a 7669 6577  aterialized.view
+00004b30: 2069 6e20 6120 646f 776e 7374 7265 616d   in a downstream
+00004b40: 2063 6f6d 706f 6e65 6e74 2074 6861 7420   component that 
+00004b50: 6973 2075 7064 6174 6564 2066 726f 6d20  is updated from 
+00004b60: 7468 6573 6520 6576 656e 7473 2e20 4966  these events. If
+00004b70: 2074 6865 206e 6577 0a65 7665 6e74 7320   the new.events 
+00004b80: 6861 7665 206e 6f74 2079 6574 2062 6565  have not yet bee
+00004b90: 6e20 7072 6f63 6573 7365 642c 2074 6865  n processed, the
+00004ba0: 2076 6965 7720 776f 756c 6420 6265 2073   view would be s
+00004bb0: 7461 6c65 2e20 5468 6520 2263 6f6d 6d69  tale. The "commi
+00004bc0: 7420 706f 7369 7469 6f6e 220a 6361 6e20  t position".can 
+00004bd0: 6265 2075 7365 6420 6279 2074 6865 2075  be used by the u
+00004be0: 7365 7220 696e 7465 7266 6163 6520 746f  ser interface to
+00004bf0: 2070 6f6c 6c20 7468 6520 646f 776e 7374   poll the downst
+00004c00: 7265 616d 2063 6f6d 706f 6e65 6e74 2075  ream component u
+00004c10: 6e74 696c 2069 7420 6861 730a 7072 6f63  ntil it has.proc
+00004c20: 6573 7365 6420 7468 6f73 6520 6e65 7720  essed those new 
+00004c30: 6576 656e 7473 2c20 6166 7465 7220 7768  events, after wh
+00004c40: 6963 6820 7469 6d65 2074 6865 2076 6965  ich time the vie
+00004c50: 7720 7769 6c6c 206e 6f74 2062 6520 7374  w will not be st
+00004c60: 616c 652e 0a0a 0a23 2323 2041 7070 656e  ale....### Appen
+00004c70: 6420 6576 656e 740a 0a54 6865 2060 6170  d event..The `ap
+00004c80: 7065 6e64 5f65 7665 6e74 2829 6020 6d65  pend_event()` me
+00004c90: 7468 6f64 2063 616e 2062 6520 7573 6564  thod can be used
+00004ca0: 2074 6f20 7772 6974 6520 6120 7369 6e67   to write a sing
+00004cb0: 6c65 206e 6577 2065 7665 6e74 2074 6f20  le new event to 
+00004cc0: 6120 7374 7265 616d 2e0a 0a54 6872 6565  a stream...Three
+00004cd0: 2061 7267 756d 656e 7473 2061 7265 2072   arguments are r
+00004ce0: 6571 7569 7265 642c 2060 7374 7265 616d  equired, `stream
+00004cf0: 5f6e 616d 6560 2c20 6065 7870 6563 7465  _name`, `expecte
+00004d00: 645f 706f 7369 7469 6f6e 6020 616e 6420  d_position` and 
+00004d10: 6065 7665 6e74 602e 0a0a 5468 6973 206d  `event`...This m
+00004d20: 6574 686f 6420 776f 726b 7320 696e 2074  ethod works in t
+00004d30: 6865 2073 616d 6520 7761 7920 6173 2060  he same way as `
+00004d40: 6170 7065 6e64 5f65 7665 6e74 7328 2960  append_events()`
+00004d50: 2c20 686f 7765 7665 7220 6065 7665 6e74  , however `event
+00004d60: 6020 6973 2065 7870 6563 7465 640a 746f  ` is expected.to
+00004d70: 2062 6520 6120 7369 6e67 6c65 2060 4e65   be a single `Ne
+00004d80: 7745 7665 6e74 602e 0a0a 5468 6973 206d  wEvent`...This m
+00004d90: 6574 686f 6420 7461 6b65 7320 616e 206f  ethod takes an o
+00004da0: 7074 696f 6e61 6c20 6074 696d 656f 7574  ptional `timeout
+00004db0: 6020 6172 6775 6d65 6e74 2c20 7768 6963  ` argument, whic
+00004dc0: 6820 6973 2061 2050 7974 686f 6e20 6066  h is a Python `f
+00004dd0: 6c6f 6174 6020 7468 6174 2073 6574 730a  loat` that sets.
+00004de0: 6120 6465 6164 6c69 6e65 2066 6f72 2074  a deadline for t
+00004df0: 6865 2063 6f6d 706c 6574 696f 6e20 6f66  he completion of
+00004e00: 2074 6865 2067 5250 4320 6f70 6572 6174   the gRPC operat
+00004e10: 696f 6e2e 0a0a 5369 6e63 6520 7468 6520  ion...Since the 
+00004e20: 6861 6e64 6c69 6e67 206f 6620 6120 636f  handling of a co
+00004e30: 6d6d 616e 6420 696e 2079 6f75 7220 6170  mmand in your ap
+00004e40: 706c 6963 6174 696f 6e20 6d61 7920 7265  plication may re
+00004e50: 7375 6c74 2069 6e20 6f6e 6520 6f72 206d  sult in one or m
+00004e60: 616e 790a 6e65 7720 6576 656e 7473 2c20  any.new events, 
+00004e70: 616e 6420 7468 6520 7265 7375 6c74 7320  and the results 
+00004e80: 6f66 2068 616e 646c 696e 6720 6120 636f  of handling a co
+00004e90: 6d6d 616e 6420 7368 6f75 6c64 2062 6520  mmand should be 
+00004ea0: 7265 636f 7264 6564 2061 746f 6d69 6361  recorded atomica
+00004eb0: 6c6c 792c 0a61 6e64 2074 6865 2077 7269  lly,.and the wri
+00004ec0: 7469 6e67 206f 6620 6e65 7720 6576 656e  ting of new even
+00004ed0: 7473 2067 656e 6572 6174 6564 2062 7920  ts generated by 
+00004ee0: 6120 636f 6d6d 616e 6420 6861 6e64 6c65  a command handle
+00004ef0: 7220 6973 2075 7375 616c 6c79 2061 2063  r is usually a c
+00004f00: 6f6e 6365 726e 0a74 6861 7420 6973 2066  oncern.that is f
+00004f10: 6163 746f 7265 6420 6f75 7420 616e 6420  actored out and 
+00004f20: 7573 6564 2065 7665 7279 7768 6572 6520  used everywhere 
+00004f30: 696e 2061 2070 726f 6a65 6374 2c20 6974  in a project, it
+00004f40: 2069 7320 7175 6974 6520 7573 7561 6c20   is quite usual 
+00004f50: 696e 2061 2070 726f 6a65 6374 0a74 6f20  in a project.to 
+00004f60: 6f6e 6c79 2075 7365 2060 6170 7065 6e64  only use `append
+00004f70: 5f65 7665 6e74 7328 2960 2074 6f20 7265  _events()` to re
+00004f80: 636f 7264 206e 6577 2065 7665 6e74 732e  cord new events.
+00004f90: 2046 6f72 2074 6869 7320 7265 6173 6f6e   For this reason
+00004fa0: 2c20 616e 2065 7861 6d70 6c65 2069 730a  , an example is.
+00004fb0: 6e6f 7420 7072 6f76 6964 6564 2068 6572  not provided her
+00004fc0: 652e 0a0a 0a23 2323 2049 6465 6d70 6f74  e....### Idempot
+00004fd0: 656e 7420 6170 7065 6e64 206f 7065 7261  ent append opera
+00004fe0: 7469 6f6e 730a 0a53 6f6d 6574 696d 6573  tions..Sometimes
+00004ff0: 2069 7420 6d61 7920 6861 7070 656e 2074   it may happen t
+00005000: 6861 7420 6120 6e65 7720 6576 656e 7420  hat a new event 
+00005010: 6973 2073 7563 6365 7373 6675 6c6c 7920  is successfully 
+00005020: 7265 636f 7264 6564 2061 6e64 2074 6865  recorded and the
+00005030: 6e20 736f 6d65 686f 770a 7468 6520 636f  n somehow.the co
+00005040: 6e6e 6563 7469 6f6e 2074 6f20 7468 6520  nnection to the 
+00005050: 6461 7461 6261 7365 2067 6574 7320 696e  database gets in
+00005060: 7465 7272 7570 7465 6420 6265 666f 7265  terrupted before
+00005070: 2074 6865 2073 7563 6365 7373 6675 6c20   the successful 
+00005080: 6361 6c6c 2063 616e 2072 6574 7572 6e0a  call can return.
+00005090: 7375 6363 6573 7366 756c 6c79 2074 6f20  successfully to 
+000050a0: 7468 6520 636c 6965 6e74 2e20 496e 2063  the client. In c
+000050b0: 6173 6520 6f66 2061 6e20 6572 726f 7220  ase of an error 
+000050c0: 7768 656e 2061 7070 656e 6469 6e67 2061  when appending a
+000050d0: 6e20 6576 656e 742c 2069 7420 6d61 7920  n event, it may 
+000050e0: 6265 0a64 6573 6972 6162 6c65 2074 6f20  be.desirable to 
+000050f0: 7265 7472 7920 6170 7065 6e64 696e 6720  retry appending 
+00005100: 7468 6520 7361 6d65 2065 7665 6e74 2061  the same event a
+00005110: 7420 7468 6520 7361 6d65 2070 6f73 6974  t the same posit
+00005120: 696f 6e2e 2049 6620 7468 6520 6576 656e  ion. If the even
+00005130: 7420 7761 730a 696e 2066 6163 7420 7375  t was.in fact su
+00005140: 6363 6573 7366 756c 6c79 2072 6563 6f72  ccessfully recor
+00005150: 6465 642c 2069 7420 6973 2063 6f6e 7665  ded, it is conve
+00005160: 6e69 656e 7420 666f 7220 7468 6520 7265  nient for the re
+00005170: 7472 7920 746f 2072 6574 7572 6e20 7375  try to return su
+00005180: 6363 6573 7366 756c 6c79 0a77 6974 686f  ccessfully.witho
+00005190: 7574 2072 6169 7369 6e67 2061 6e20 6572  ut raising an er
+000051a0: 726f 7220 6475 6520 746f 206f 7074 696d  ror due to optim
+000051b0: 6973 7469 6320 636f 6e63 7572 7265 6e63  istic concurrenc
+000051c0: 7920 636f 6e74 726f 6c20 2861 7320 6465  y control (as de
+000051d0: 7363 7269 6265 6420 6162 6f76 6529 2e0a  scribed above)..
+000051e0: 0a54 6865 2065 7861 6d70 6c65 2062 656c  .The example bel
+000051f0: 6f77 2073 686f 7773 2074 6865 2060 6170  ow shows the `ap
+00005200: 7065 6e64 5f65 7665 6e74 7328 2960 206d  pend_events()` m
+00005210: 6574 686f 6420 6265 696e 6720 6361 6c6c  ethod being call
+00005220: 6564 2061 6761 696e 2077 6974 680a 6065  ed again with.`e
+00005230: 7665 6e74 3360 2061 6e64 2060 6578 7065  vent3` and `expe
+00005240: 6374 6564 5f70 6f73 6974 696f 6e3d 3260  cted_position=2`
+00005250: 2e20 5765 2063 616e 2073 6565 2074 6861  . We can see tha
+00005260: 7420 7265 7065 6174 696e 6720 7468 6520  t repeating the 
+00005270: 6361 6c6c 2074 6f0a 6061 7070 656e 645f  call to.`append_
+00005280: 6576 656e 7473 2829 6020 7265 7475 726e  events()` return
+00005290: 7320 7375 6363 6573 7366 756c 6c79 2e0a  s successfully..
+000052a0: 0a60 6060 7079 7468 6f6e 0a23 2052 6574  .```python.# Ret
+000052b0: 7279 2061 7070 656e 6469 6e67 2065 7665  ry appending eve
+000052c0: 6e74 332e 0a63 6f6d 6d69 745f 706f 7369  nt3..commit_posi
+000052d0: 7469 6f6e 5f72 6574 7279 203d 2063 6c69  tion_retry = cli
+000052e0: 656e 742e 6170 7065 6e64 5f65 7665 6e74  ent.append_event
+000052f0: 7328 0a20 2020 2073 7472 6561 6d5f 6e61  s(.    stream_na
+00005300: 6d65 3d73 7472 6561 6d5f 6e61 6d65 312c  me=stream_name1,
+00005310: 0a20 2020 2065 7870 6563 7465 645f 706f  .    expected_po
+00005320: 7369 7469 6f6e 3d30 2c0a 2020 2020 6576  sition=0,.    ev
+00005330: 656e 7473 3d5b 6576 656e 7432 2c20 6576  ents=[event2, ev
+00005340: 656e 7433 5d2c 0a29 0a60 6060 0a0a 5765  ent3],.).```..We
+00005350: 2063 616e 2073 6565 2074 6861 7420 7468   can see that th
+00005360: 6520 7361 6d65 2063 6f6d 6d69 7420 706f  e same commit po
+00005370: 7369 7469 6f6e 2069 7320 7265 7475 726e  sition is return
+00005380: 6564 2061 7320 6162 6f76 652e 0a0a 6060  ed as above...``
+00005390: 6070 7974 686f 6e0a 6173 7365 7274 2063  `python.assert c
+000053a0: 6f6d 6d69 745f 706f 7369 7469 6f6e 5f72  ommit_position_r
+000053b0: 6574 7279 203d 3d20 636f 6d6d 6974 5f70  etry == commit_p
+000053c0: 6f73 6974 696f 6e32 0a60 6060 0a0a 5765  osition2.```..We
+000053d0: 2063 616e 2061 6c73 6f20 7365 6520 7468   can also see th
+000053e0: 6520 7374 7265 616d 2068 6173 2062 6565  e stream has bee
+000053f0: 6e20 756e 6368 616e 6765 6420 6465 7370  n unchanged desp
+00005400: 6974 6520 6361 6c6c 696e 6720 7468 6520  ite calling the 
+00005410: 6170 7065 6e64 5f65 7665 6e74 7328 290a  append_events().
+00005420: 7477 6963 6520 7769 7468 2074 6865 2073  twice with the s
+00005430: 616d 6520 6172 6775 6d65 6e74 732c 2062  ame arguments, b
+00005440: 7920 6361 6c6c 696e 6720 6072 6561 645f  y calling `read_
+00005450: 7374 7265 616d 5f65 7665 6e74 7328 2960  stream_events()`
+00005460: 2e20 5468 6174 2069 732c 2074 6865 7265  . That is, there
+00005470: 0a61 7265 2073 7469 6c6c 206f 6e6c 7920  .are still only 
+00005480: 7468 7265 6520 6576 656e 7473 2069 6e20  three events in 
+00005490: 7468 6520 7374 7265 616d 2e0a 0a60 6060  the stream...```
+000054a0: 7079 7468 6f6e 0a72 6573 706f 6e73 6520  python.response 
+000054b0: 3d20 636c 6965 6e74 2e72 6561 645f 7374  = client.read_st
+000054c0: 7265 616d 5f65 7665 6e74 7328 0a20 2020  ream_events(.   
+000054d0: 2073 7472 6561 6d5f 6e61 6d65 3d73 7472   stream_name=str
+000054e0: 6561 6d5f 6e61 6d65 310a 290a 0a65 7665  eam_name1.)..eve
+000054f0: 6e74 7320 3d20 6c69 7374 2872 6573 706f  nts = list(respo
+00005500: 6e73 6529 0a61 7373 6572 7420 6c65 6e28  nse).assert len(
+00005510: 6576 656e 7473 2920 3d3d 2033 0a60 6060  events) == 3.```
+00005520: 0a0a 5468 6973 2069 6465 6d70 6f74 656e  ..This idempoten
+00005530: 7420 6265 6861 7669 6f75 7220 6973 2061  t behaviour is a
+00005540: 6374 6976 6174 6564 2062 6563 6175 7365  ctivated because
+00005550: 2074 6865 2060 4e65 7745 7665 6e74 6020   the `NewEvent` 
+00005560: 636c 6173 7320 6861 7320 616e 2060 6964  class has an `id
+00005570: 600a 6174 7472 6962 7574 6520 7468 6174  `.attribute that
+00005580: 2c20 6279 2064 6566 6175 6c74 2c20 6973  , by default, is
+00005590: 2061 7373 6967 6e65 6420 6120 6e65 7720   assigned a new 
+000055a0: 616e 6420 756e 6971 7565 2076 6572 7369  and unique versi
+000055b0: 6f6e 2d34 2055 5549 4420 7768 656e 2061  on-4 UUID when a
+000055c0: 6e0a 696e 7374 616e 6365 206f 6620 604e  n.instance of `N
+000055d0: 6577 4576 656e 7460 2069 7320 636f 6e73  ewEvent` is cons
+000055e0: 7472 7563 7465 642e 2049 6620 6576 656e  tructed. If even
+000055f0: 7473 2077 6974 6820 7468 6520 7361 6d65  ts with the same
+00005600: 2060 6964 6020 6172 6520 6170 7065 6e64   `id` are append
+00005610: 6564 0a61 7420 7468 6520 7361 6d65 2060  ed.at the same `
+00005620: 6578 7065 6374 6564 5f70 6f73 6974 696f  expected_positio
+00005630: 6e60 2c20 7468 6520 7374 7265 616d 2077  n`, the stream w
+00005640: 696c 6c20 6265 2075 6e63 6861 6e67 6564  ill be unchanged
+00005650: 2c20 7468 6520 6f70 6572 6174 696f 6e20  , the operation 
+00005660: 7769 6c6c 0a63 6f6d 706c 6574 6520 7375  will.complete su
+00005670: 6363 6573 7366 756c 6c79 2c20 616e 6420  ccessfully, and 
+00005680: 7468 6520 7361 6d65 2063 6f6d 6d69 7420  the same commit 
+00005690: 706f 7369 7469 6f6e 2077 696c 6c20 6265  position will be
+000056a0: 2072 6574 7572 6e65 6420 746f 2074 6865   returned to the
+000056b0: 2063 616c 6c65 722e 0a0a 6060 6070 7974   caller...```pyt
+000056c0: 686f 6e0a 6672 6f6d 2075 7569 6420 696d  hon.from uuid im
+000056d0: 706f 7274 2055 5549 440a 0a0a 6173 7365  port UUID...asse
+000056e0: 7274 2069 7369 6e73 7461 6e63 6528 6576  rt isinstance(ev
+000056f0: 656e 7431 2e69 642c 2055 5549 4429 0a61  ent1.id, UUID).a
+00005700: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+00005710: 2865 7665 6e74 322e 6964 2c20 5555 4944  (event2.id, UUID
+00005720: 290a 6173 7365 7274 2069 7369 6e73 7461  ).assert isinsta
+00005730: 6e63 6528 6576 656e 7433 2e69 642c 2055  nce(event3.id, U
+00005740: 5549 4429 0a0a 6173 7365 7274 2065 7665  UID)..assert eve
+00005750: 6e74 312e 6964 2021 3d20 6576 656e 7432  nt1.id != event2
+00005760: 2e69 640a 6173 7365 7274 2065 7665 6e74  .id.assert event
+00005770: 322e 6964 2021 3d20 6576 656e 7433 2e69  2.id != event3.i
+00005780: 640a 0a61 7373 6572 7420 6576 656e 7473  d..assert events
+00005790: 5b30 5d2e 6964 203d 3d20 6576 656e 7431  [0].id == event1
+000057a0: 2e69 640a 6173 7365 7274 2065 7665 6e74  .id.assert event
+000057b0: 735b 315d 2e69 6420 3d3d 2065 7665 6e74  s[1].id == event
+000057c0: 322e 6964 0a61 7373 6572 7420 6576 656e  2.id.assert even
+000057d0: 7473 5b32 5d2e 6964 203d 3d20 6576 656e  ts[2].id == even
+000057e0: 7433 2e69 640a 6060 600a 0a49 7420 6973  t3.id.```..It is
+000057f0: 2070 6f73 7369 626c 6520 746f 2073 6574   possible to set
+00005800: 2074 6865 2060 6964 6020 636f 6e73 7472   the `id` constr
+00005810: 7563 746f 7220 6172 6775 6d65 6e74 206f  uctor argument o
+00005820: 6620 604e 6577 4576 656e 7460 2077 6865  f `NewEvent` whe
+00005830: 6e20 696e 7374 616e 7469 6174 696e 670a  n instantiating.
+00005840: 7468 6520 604e 6577 4576 656e 7460 2063  the `NewEvent` c
+00005850: 6c61 7373 2c20 6275 7420 696e 2074 6865  lass, but in the
+00005860: 2065 7861 6d70 6c65 7320 6162 6f76 6520   examples above 
+00005870: 7765 2068 6176 6520 6265 656e 2075 7369  we have been usi
+00005880: 6e67 2074 6865 2064 6566 6175 6c74 0a62  ng the default.b
+00005890: 6568 6176 696f 7572 2c20 7768 6963 6820  ehaviour, which 
+000058a0: 6973 2074 6861 7420 7468 6520 6069 6460  is that the `id`
+000058b0: 2076 616c 7565 2069 7320 6765 6e65 7261   value is genera
+000058c0: 7465 6420 7768 656e 2074 6865 2060 4e65  ted when the `Ne
+000058d0: 7745 7665 6e74 6020 636c 6173 7320 6973  wEvent` class is
+000058e0: 0a69 6e73 7461 6e74 6961 7465 642e 0a0a  .instantiated...
+000058f0: 0a23 2323 2052 6561 6420 7374 7265 616d  .### Read stream
+00005900: 2065 7665 6e74 730a 0a54 6865 2060 7265   events..The `re
+00005910: 6164 5f73 7472 6561 6d5f 6576 656e 7473  ad_stream_events
+00005920: 2829 6020 6d65 7468 6f64 2063 616e 2062  ()` method can b
+00005930: 6520 7573 6564 2074 6f20 7265 6164 2074  e used to read t
+00005940: 6865 2072 6563 6f72 6465 6420 6576 656e  he recorded even
+00005950: 7473 206f 6620 6120 7374 7265 616d 2e0a  ts of a stream..
+00005960: 0a54 6869 7320 6d65 7468 6f64 2063 616e  .This method can
+00005970: 2062 6520 7573 6564 2074 6f20 7265 7472   be used to retr
+00005980: 6965 7665 2061 6c6c 2074 6865 2072 6563  ieve all the rec
+00005990: 6f72 6465 6420 6576 656e 7473 2066 6f72  orded events for
+000059a0: 2061 6e20 6167 6772 6567 6174 6520 6265   an aggregate be
+000059b0: 666f 7265 0a65 7865 6375 7469 6e67 2061  fore.executing a
+000059c0: 2063 6f6d 6d61 6e64 2069 6e20 616e 2061   command in an a
+000059d0: 7070 6c69 6361 7469 6f6e 2e0a 0a54 6869  pplication...Thi
+000059e0: 7320 6d65 7468 6f64 2068 6173 206f 6e65  s method has one
+000059f0: 2072 6571 7569 7265 6420 6172 6775 6d65   required argume
+00005a00: 6e74 2c20 6073 7472 6561 6d5f 6e61 6d65  nt, `stream_name
+00005a10: 602c 2077 6869 6368 2069 7320 7468 6520  `, which is the 
+00005a20: 6e61 6d65 206f 660a 7468 6520 7374 7265  name of.the stre
+00005a30: 616d 2066 726f 6d20 7768 6963 6820 746f  am from which to
+00005a40: 2072 6561 6420 6576 656e 7473 2e20 4279   read events. By
+00005a50: 2064 6566 6175 6c74 2c20 7468 6520 7265   default, the re
+00005a60: 636f 7264 6564 2065 7665 6e74 7320 696e  corded events in
+00005a70: 2074 6865 0a73 7472 6561 6d20 6172 6520   the.stream are 
+00005a80: 7265 7475 726e 6564 2069 6e20 7468 6520  returned in the 
+00005a90: 6f72 6465 7220 7468 6579 2077 6572 6520  order they were 
+00005aa0: 7265 636f 7264 6564 2e0a 0a54 6865 206d  recorded...The m
+00005ab0: 6574 686f 6420 6072 6561 645f 7374 7265  ethod `read_stre
+00005ac0: 616d 5f65 7665 6e74 7328 2960 2061 6c73  am_events()` als
+00005ad0: 6f20 7375 7070 6f72 7473 2066 6f75 7220  o supports four 
+00005ae0: 6f70 7469 6f6e 616c 2061 7267 756d 656e  optional argumen
+00005af0: 7473 2c0a 6073 7472 6561 6d5f 706f 7369  ts,.`stream_posi
+00005b00: 7469 6f6e 602c 2060 6261 636b 7761 7264  tion`, `backward
+00005b10: 7360 2c20 606c 696d 6974 602c 2061 6e64  s`, `limit`, and
+00005b20: 2060 7469 6d65 6f75 7460 2e0a 0a54 6865   `timeout`...The
+00005b30: 206f 7074 696f 6e61 6c20 6073 7472 6561   optional `strea
+00005b40: 6d5f 706f 7369 7469 6f6e 6020 6172 6775  m_position` argu
+00005b50: 6d65 6e74 2069 7320 616e 206f 7074 696f  ment is an optio
+00005b60: 6e61 6c20 696e 7465 6765 7220 7468 6174  nal integer that
+00005b70: 2063 616e 2062 6520 7573 6564 2074 6f0a   can be used to.
+00005b80: 696e 6469 6361 7465 2074 6865 2070 6f73  indicate the pos
+00005b90: 6974 696f 6e20 696e 2074 6865 2073 7472  ition in the str
+00005ba0: 6561 6d20 6672 6f6d 2077 6869 6368 2074  eam from which t
+00005bb0: 6f20 7374 6172 7420 7265 6164 696e 672e  o start reading.
+00005bc0: 2054 6869 7320 6172 6775 6d65 6e74 2069   This argument i
+00005bd0: 730a 604e 6f6e 6560 2062 7920 6465 6661  s.`None` by defa
+00005be0: 756c 742c 2077 6869 6368 206d 6561 6e73  ult, which means
+00005bf0: 2074 6865 2073 7472 6561 6d20 7769 6c6c   the stream will
+00005c00: 2062 6520 7265 6164 2065 6974 6865 7220   be read either 
+00005c10: 6672 6f6d 2074 6865 2073 7461 7274 206f  from the start o
+00005c20: 6620 7468 650a 7374 7265 616d 2028 7468  f the.stream (th
+00005c30: 6520 6465 6661 756c 7420 6265 6861 7669  e default behavi
+00005c40: 6f75 7229 2c20 6f72 2066 726f 6d20 7468  our), or from th
+00005c50: 6520 656e 6420 6f66 2074 6865 2073 7472  e end of the str
+00005c60: 6561 6d20 6966 2060 6261 636b 7761 7264  eam if `backward
+00005c70: 7360 2069 730a 6054 7275 6560 2028 7365  s` is.`True` (se
+00005c80: 6520 6265 6c6f 7729 2e20 5768 656e 2072  e below). When r
+00005c90: 6561 6469 6e67 2061 2073 7472 6561 6d20  eading a stream 
+00005ca0: 6672 6f6d 2061 2073 7065 6369 6669 6320  from a specific 
+00005cb0: 706f 7369 7469 6f6e 2069 6e20 7468 6520  position in the 
+00005cc0: 7374 7265 616d 2c20 7468 650a 7265 636f  stream, the.reco
+00005cd0: 7264 6564 2065 7665 6e74 2061 7420 7468  rded event at th
+00005ce0: 6174 2070 6f73 6974 696f 6e20 5749 4c4c  at position WILL
+00005cf0: 2062 6520 696e 636c 7564 6564 2c20 626f   be included, bo
+00005d00: 7468 2077 6865 6e20 7265 6164 696e 6720  th when reading 
+00005d10: 666f 7277 6172 6473 0a66 726f 6d20 7468  forwards.from th
+00005d20: 6174 2070 6f73 6974 696f 6e2c 2061 6e64  at position, and
+00005d30: 2077 6865 6e20 7265 6164 696e 6720 6261   when reading ba
+00005d40: 636b 7761 7264 7320 6672 6f6d 2074 6861  ckwards from tha
+00005d50: 7420 706f 7369 7469 6f6e 2e0a 0a54 6865  t position...The
+00005d60: 206f 7074 696f 6e61 6c20 6172 6775 6d65   optional argume
+00005d70: 6e74 2060 6261 636b 7761 7264 7360 2069  nt `backwards` i
+00005d80: 7320 6120 626f 6f6c 6561 6e2c 2062 7920  s a boolean, by 
+00005d90: 6465 6661 756c 7420 6046 616c 7365 602c  default `False`,
+00005da0: 2077 6869 6368 206d 6561 6e73 2074 6865   which means the
+00005db0: 0a73 7472 6561 6d20 7769 6c6c 2062 6520  .stream will be 
+00005dc0: 7265 6164 2066 6f72 7761 7264 7320 6279  read forwards by
+00005dd0: 2064 6566 6175 6c74 2c20 736f 2074 6861   default, so tha
+00005de0: 7420 6576 656e 7473 2061 7265 2072 6574  t events are ret
+00005df0: 7572 6e65 6420 696e 2074 6865 0a6f 7264  urned in the.ord
+00005e00: 6572 2074 6865 7920 7765 7265 2061 7070  er they were app
+00005e10: 656e 6465 642c 2049 6620 6062 6163 6b77  ended, If `backw
+00005e20: 6172 6473 6020 6973 2060 5472 7565 602c  ards` is `True`,
+00005e30: 2074 6865 2073 7472 6561 6d20 7769 6c6c   the stream will
+00005e40: 2062 6520 7265 6164 0a62 6163 6b77 6172   be read.backwar
+00005e50: 6473 2c20 736f 2074 6861 7420 6576 656e  ds, so that even
+00005e60: 7473 2061 7265 2072 6574 7572 6e65 6420  ts are returned 
+00005e70: 696e 2072 6576 6572 7365 206f 7264 6572  in reverse order
+00005e80: 2e0a 0a54 6865 206f 7074 696f 6e61 6c20  ...The optional 
+00005e90: 6172 6775 6d65 6e74 2060 6c69 6d69 7460  argument `limit`
+00005ea0: 2069 7320 616e 2069 6e74 6567 6572 2077   is an integer w
+00005eb0: 6869 6368 206c 696d 6974 7320 7468 6520  hich limits the 
+00005ec0: 6e75 6d62 6572 206f 6620 6576 656e 7473  number of events
+00005ed0: 2074 6861 7420 7769 6c6c 0a62 6520 7265   that will.be re
+00005ee0: 7475 726e 6564 2e20 5468 6520 6465 6661  turned. The defa
+00005ef0: 756c 7420 7661 6c75 6520 6973 2060 7379  ult value is `sy
+00005f00: 732e 6d61 7869 6e74 602e 0a0a 5468 6520  s.maxint`...The 
+00005f10: 6f70 7469 6f6e 616c 2061 7267 756d 656e  optional argumen
+00005f20: 7420 6074 696d 656f 7574 6020 6973 2061  t `timeout` is a
+00005f30: 2050 7974 686f 6e20 6066 6c6f 6174 6020   Python `float` 
+00005f40: 7768 6963 6820 7365 7473 2061 2064 6561  which sets a dea
+00005f50: 646c 696e 6520 666f 7220 7468 6520 636f  dline for the co
+00005f60: 6d70 6c65 7469 6f6e 206f 660a 7468 6520  mpletion of.the 
+00005f70: 6752 5043 206f 7065 7261 7469 6f6e 2e0a  gRPC operation..
+00005f80: 0a54 6869 7320 6d65 7468 6f64 2072 6574  .This method ret
+00005f90: 7572 6e73 2061 2050 7974 686f 6e20 6974  urns a Python it
+00005fa0: 6572 6162 6c65 206f 626a 6563 7420 7468  erable object th
+00005fb0: 6174 2079 6965 6c64 7320 6052 6563 6f72  at yields `Recor
+00005fc0: 6465 6445 7665 6e74 6020 6f62 6a65 6374  dedEvent` object
+00005fd0: 732e 0a54 6865 7365 2072 6563 6f72 6465  s..These recorde
+00005fe0: 6420 6576 656e 7420 6f62 6a65 6374 7320  d event objects 
+00005ff0: 6172 6520 696e 7374 616e 6365 7320 6f66  are instances of
+00006000: 2074 6865 2060 5265 636f 7264 6564 4576   the `RecordedEv
+00006010: 656e 7460 2063 6c61 7373 2028 7365 6520  ent` class (see 
+00006020: 6265 6c6f 7729 0a0a 5468 6520 6578 616d  below)..The exam
+00006030: 706c 6520 6265 6c6f 7720 7368 6f77 7320  ple below shows 
+00006040: 686f 7720 746f 2072 6561 6420 7468 6520  how to read the 
+00006050: 7265 636f 7264 6564 2065 7665 6e74 7320  recorded events 
+00006060: 6f66 2061 2073 7472 6561 6d0a 666f 7277  of a stream.forw
+00006070: 6172 6473 2066 726f 6d20 7468 6520 7374  ards from the st
+00006080: 6172 7420 6f66 2074 6865 2073 7472 6561  art of the strea
+00006090: 6d20 746f 2074 6865 2065 6e64 206f 6620  m to the end of 
+000060a0: 7468 6520 7374 7265 616d 2e20 5468 650a  the stream. The.
+000060b0: 6e61 6d65 206f 6620 6120 7374 7265 616d  name of a stream
+000060c0: 2069 7320 6769 7665 6e20 7768 656e 2063   is given when c
+000060d0: 616c 6c69 6e67 2074 6865 206d 6574 686f  alling the metho
+000060e0: 642e 2049 6e20 7468 6973 2065 7861 6d70  d. In this examp
+000060f0: 6c65 2c0a 7468 6520 6974 6572 6162 6c65  le,.the iterable
+00006100: 2072 6573 706f 6e73 6520 6f62 6a65 6374   response object
+00006110: 2069 7320 636f 6e76 6572 7465 6420 696e   is converted in
+00006120: 746f 2061 2050 7974 686f 6e20 606c 6973  to a Python `lis
+00006130: 7460 2c20 7768 6963 680a 636f 6e74 6169  t`, which.contai
+00006140: 6e73 2061 6c6c 2074 6865 2072 6563 6f72  ns all the recor
+00006150: 6465 6420 6576 656e 7420 6f62 6a65 6374  ded event object
+00006160: 7320 7468 6174 2077 6572 6520 7265 6164  s that were read
+00006170: 2066 726f 6d20 7468 6520 7374 7265 616d   from the stream
+00006180: 2e0a 0a60 6060 7079 7468 6f6e 0a72 6573  ...```python.res
+00006190: 706f 6e73 6520 3d20 636c 6965 6e74 2e72  ponse = client.r
+000061a0: 6561 645f 7374 7265 616d 5f65 7665 6e74  ead_stream_event
+000061b0: 7328 0a20 2020 2073 7472 6561 6d5f 6e61  s(.    stream_na
+000061c0: 6d65 3d73 7472 6561 6d5f 6e61 6d65 310a  me=stream_name1.
+000061d0: 290a 0a65 7665 6e74 7320 3d20 6c69 7374  )..events = list
+000061e0: 2872 6573 706f 6e73 6529 0a60 6060 0a0a  (response).```..
+000061f0: 4e6f 7720 7468 6174 2077 6520 6861 7665  Now that we have
+00006200: 2061 206c 6973 7420 6f66 2065 7665 6e74   a list of event
+00006210: 206f 626a 6563 7473 2c20 7765 2063 616e   objects, we can
+00006220: 2063 6865 636b 2077 6520 676f 7420 7468   check we got th
+00006230: 650a 7468 7265 6520 6576 656e 7473 2074  e.three events t
+00006240: 6861 7420 7765 7265 2061 7070 656e 6465  hat were appende
+00006250: 6420 746f 2074 6865 2073 7472 6561 6d2c  d to the stream,
+00006260: 2061 6e64 2074 6861 7420 7468 6579 2061   and that they a
+00006270: 7265 0a6f 7264 6572 6564 2065 7861 6374  re.ordered exact
+00006280: 6c79 2061 7320 7468 6579 2077 6572 6520  ly as they were 
+00006290: 6170 7065 6e64 6564 2e0a 0a60 6060 7079  appended...```py
+000062a0: 7468 6f6e 0a61 7373 6572 7420 6c65 6e28  thon.assert len(
+000062b0: 6576 656e 7473 2920 3d3d 2033 0a0a 6173  events) == 3..as
+000062c0: 7365 7274 2065 7665 6e74 735b 305d 2e73  sert events[0].s
+000062d0: 7472 6561 6d5f 6e61 6d65 203d 3d20 7374  tream_name == st
+000062e0: 7265 616d 5f6e 616d 6531 0a61 7373 6572  ream_name1.asser
+000062f0: 7420 6576 656e 7473 5b30 5d2e 7374 7265  t events[0].stre
+00006300: 616d 5f70 6f73 6974 696f 6e20 3d3d 2030  am_position == 0
+00006310: 0a61 7373 6572 7420 6576 656e 7473 5b30  .assert events[0
+00006320: 5d2e 7479 7065 203d 3d20 6576 656e 7431  ].type == event1
+00006330: 2e74 7970 650a 6173 7365 7274 2065 7665  .type.assert eve
+00006340: 6e74 735b 305d 2e64 6174 6120 3d3d 2065  nts[0].data == e
+00006350: 7665 6e74 312e 6461 7461 0a0a 6173 7365  vent1.data..asse
+00006360: 7274 2065 7665 6e74 735b 315d 2e73 7472  rt events[1].str
+00006370: 6561 6d5f 6e61 6d65 203d 3d20 7374 7265  eam_name == stre
+00006380: 616d 5f6e 616d 6531 0a61 7373 6572 7420  am_name1.assert 
+00006390: 6576 656e 7473 5b31 5d2e 7374 7265 616d  events[1].stream
+000063a0: 5f70 6f73 6974 696f 6e20 3d3d 2031 0a61  _position == 1.a
+000063b0: 7373 6572 7420 6576 656e 7473 5b31 5d2e  ssert events[1].
+000063c0: 7479 7065 203d 3d20 6576 656e 7432 2e74  type == event2.t
+000063d0: 7970 650a 6173 7365 7274 2065 7665 6e74  ype.assert event
+000063e0: 735b 315d 2e64 6174 6120 3d3d 2065 7665  s[1].data == eve
+000063f0: 6e74 322e 6461 7461 0a0a 6173 7365 7274  nt2.data..assert
+00006400: 2065 7665 6e74 735b 325d 2e73 7472 6561   events[2].strea
+00006410: 6d5f 6e61 6d65 203d 3d20 7374 7265 616d  m_name == stream
+00006420: 5f6e 616d 6531 0a61 7373 6572 7420 6576  _name1.assert ev
+00006430: 656e 7473 5b32 5d2e 7374 7265 616d 5f70  ents[2].stream_p
+00006440: 6f73 6974 696f 6e20 3d3d 2032 0a61 7373  osition == 2.ass
+00006450: 6572 7420 6576 656e 7473 5b32 5d2e 7479  ert events[2].ty
+00006460: 7065 203d 3d20 6576 656e 7433 2e74 7970  pe == event3.typ
+00006470: 650a 6173 7365 7274 2065 7665 6e74 735b  e.assert events[
+00006480: 325d 2e64 6174 6120 3d3d 2065 7665 6e74  2].data == event
+00006490: 332e 6461 7461 0a60 6060 0a0a 5468 6520  3.data.```..The 
+000064a0: 6578 616d 706c 6520 6265 6c6f 7720 7368  example below sh
+000064b0: 6f77 7320 686f 7720 746f 2072 6561 6420  ows how to read 
+000064c0: 7265 636f 7264 6564 2065 7665 6e74 7320  recorded events 
+000064d0: 696e 2061 2073 7472 6561 6d20 666f 7277  in a stream forw
+000064e0: 6172 6473 2066 726f 6d0a 6120 7370 6563  ards from.a spec
+000064f0: 6966 6963 2073 7472 6561 6d20 706f 7369  ific stream posi
+00006500: 7469 6f6e 2074 6f20 7468 6520 656e 6420  tion to the end 
+00006510: 6f66 2074 6865 2073 7472 6561 6d2e 0a0a  of the stream...
+00006520: 6060 6070 7974 686f 6e0a 6576 656e 7473  ```python.events
+00006530: 203d 206c 6973 7428 0a20 2020 2063 6c69   = list(.    cli
+00006540: 656e 742e 7265 6164 5f73 7472 6561 6d5f  ent.read_stream_
+00006550: 6576 656e 7473 280a 2020 2020 2020 2020  events(.        
+00006560: 7374 7265 616d 5f6e 616d 653d 7374 7265  stream_name=stre
+00006570: 616d 5f6e 616d 6531 2c0a 2020 2020 2020  am_name1,.      
+00006580: 2020 7374 7265 616d 5f70 6f73 6974 696f    stream_positio
+00006590: 6e3d 312c 0a20 2020 2029 0a29 0a0a 6173  n=1,.    ).)..as
+000065a0: 7365 7274 206c 656e 2865 7665 6e74 7329  sert len(events)
+000065b0: 203d 3d20 320a 0a61 7373 6572 7420 6576   == 2..assert ev
+000065c0: 656e 7473 5b30 5d2e 7374 7265 616d 5f6e  ents[0].stream_n
+000065d0: 616d 6520 3d3d 2073 7472 6561 6d5f 6e61  ame == stream_na
+000065e0: 6d65 310a 6173 7365 7274 2065 7665 6e74  me1.assert event
+000065f0: 735b 305d 2e73 7472 6561 6d5f 706f 7369  s[0].stream_posi
+00006600: 7469 6f6e 203d 3d20 310a 6173 7365 7274  tion == 1.assert
+00006610: 2065 7665 6e74 735b 305d 2e74 7970 6520   events[0].type 
+00006620: 3d3d 2065 7665 6e74 322e 7479 7065 0a61  == event2.type.a
+00006630: 7373 6572 7420 6576 656e 7473 5b30 5d2e  ssert events[0].
+00006640: 6461 7461 203d 3d20 6576 656e 7432 2e64  data == event2.d
+00006650: 6174 610a 0a61 7373 6572 7420 6576 656e  ata..assert even
+00006660: 7473 5b31 5d2e 7374 7265 616d 5f6e 616d  ts[1].stream_nam
+00006670: 6520 3d3d 2073 7472 6561 6d5f 6e61 6d65  e == stream_name
+00006680: 310a 6173 7365 7274 2065 7665 6e74 735b  1.assert events[
+00006690: 315d 2e73 7472 6561 6d5f 706f 7369 7469  1].stream_positi
+000066a0: 6f6e 203d 3d20 320a 6173 7365 7274 2065  on == 2.assert e
+000066b0: 7665 6e74 735b 315d 2e74 7970 6520 3d3d  vents[1].type ==
+000066c0: 2065 7665 6e74 332e 7479 7065 0a61 7373   event3.type.ass
+000066d0: 6572 7420 6576 656e 7473 5b31 5d2e 6461  ert events[1].da
+000066e0: 7461 203d 3d20 6576 656e 7433 2e64 6174  ta == event3.dat
+000066f0: 610a 6060 600a 0a54 6865 2065 7861 6d70  a.```..The examp
+00006700: 6c65 2062 656c 6f77 2073 686f 7773 2068  le below shows h
+00006710: 6f77 2074 6f20 7265 6164 2074 6865 2072  ow to read the r
+00006720: 6563 6f72 6465 6420 6576 656e 7473 2069  ecorded events i
+00006730: 6e20 6120 7374 7265 616d 2062 6163 6b77  n a stream backw
+00006740: 6172 6473 2066 726f 6d0a 7468 6520 656e  ards from.the en
+00006750: 6420 6f66 2074 6865 2073 7472 6561 6d20  d of the stream 
+00006760: 746f 2074 6865 2073 7461 7274 206f 6620  to the start of 
+00006770: 7468 6520 7374 7265 616d 2e0a 0a60 6060  the stream...```
+00006780: 7079 7468 6f6e 0a65 7665 6e74 7320 3d20  python.events = 
+00006790: 6c69 7374 280a 2020 2020 636c 6965 6e74  list(.    client
+000067a0: 2e72 6561 645f 7374 7265 616d 5f65 7665  .read_stream_eve
+000067b0: 6e74 7328 0a20 2020 2020 2020 2073 7472  nts(.        str
+000067c0: 6561 6d5f 6e61 6d65 3d73 7472 6561 6d5f  eam_name=stream_
+000067d0: 6e61 6d65 312c 0a20 2020 2020 2020 2062  name1,.        b
+000067e0: 6163 6b77 6172 6473 3d54 7275 652c 0a20  ackwards=True,. 
+000067f0: 2020 2029 0a29 0a0a 6173 7365 7274 206c     ).)..assert l
+00006800: 656e 2865 7665 6e74 7329 203d 3d20 330a  en(events) == 3.
+00006810: 0a61 7373 6572 7420 6576 656e 7473 5b30  .assert events[0
+00006820: 5d2e 7374 7265 616d 5f6e 616d 6520 3d3d  ].stream_name ==
+00006830: 2073 7472 6561 6d5f 6e61 6d65 310a 6173   stream_name1.as
+00006840: 7365 7274 2065 7665 6e74 735b 305d 2e73  sert events[0].s
+00006850: 7472 6561 6d5f 706f 7369 7469 6f6e 203d  tream_position =
+00006860: 3d20 320a 6173 7365 7274 2065 7665 6e74  = 2.assert event
+00006870: 735b 305d 2e74 7970 6520 3d3d 2065 7665  s[0].type == eve
+00006880: 6e74 332e 7479 7065 0a61 7373 6572 7420  nt3.type.assert 
+00006890: 6576 656e 7473 5b30 5d2e 6461 7461 203d  events[0].data =
+000068a0: 3d20 6576 656e 7433 2e64 6174 610a 0a61  = event3.data..a
+000068b0: 7373 6572 7420 6576 656e 7473 5b31 5d2e  ssert events[1].
+000068c0: 7374 7265 616d 5f6e 616d 6520 3d3d 2073  stream_name == s
+000068d0: 7472 6561 6d5f 6e61 6d65 310a 6173 7365  tream_name1.asse
+000068e0: 7274 2065 7665 6e74 735b 315d 2e73 7472  rt events[1].str
+000068f0: 6561 6d5f 706f 7369 7469 6f6e 203d 3d20  eam_position == 
+00006900: 310a 6173 7365 7274 2065 7665 6e74 735b  1.assert events[
+00006910: 315d 2e74 7970 6520 3d3d 2065 7665 6e74  1].type == event
+00006920: 322e 7479 7065 0a61 7373 6572 7420 6576  2.type.assert ev
+00006930: 656e 7473 5b31 5d2e 6461 7461 203d 3d20  ents[1].data == 
+00006940: 6576 656e 7432 2e64 6174 610a 6060 600a  event2.data.```.
+00006950: 0a54 6865 2065 7861 6d70 6c65 2062 656c  .The example bel
+00006960: 6f77 2073 686f 7773 2068 6f77 2074 6f20  ow shows how to 
+00006970: 7265 6164 2061 206c 696d 6974 6564 206e  read a limited n
+00006980: 756d 6265 7220 2874 776f 2920 6f66 2074  umber (two) of t
+00006990: 6865 2072 6563 6f72 6465 6420 6576 656e  he recorded even
+000069a0: 7473 0a69 6e20 6120 7374 7265 616d 2066  ts.in a stream f
+000069b0: 6f72 7761 7264 7320 6672 6f6d 2074 6865  orwards from the
+000069c0: 2073 7461 7274 206f 6620 7468 6520 7374   start of the st
+000069d0: 7265 616d 2e0a 0a60 6060 7079 7468 6f6e  ream...```python
+000069e0: 0a65 7665 6e74 7320 3d20 6c69 7374 280a  .events = list(.
+000069f0: 2020 2020 636c 6965 6e74 2e72 6561 645f      client.read_
+00006a00: 7374 7265 616d 5f65 7665 6e74 7328 0a20  stream_events(. 
+00006a10: 2020 2020 2020 2073 7472 6561 6d5f 6e61         stream_na
+00006a20: 6d65 3d73 7472 6561 6d5f 6e61 6d65 312c  me=stream_name1,
+00006a30: 0a20 2020 2020 2020 206c 696d 6974 3d32  .        limit=2
+00006a40: 2c0a 2020 2020 290a 290a 0a61 7373 6572  ,.    ).)..asser
+00006a50: 7420 6c65 6e28 6576 656e 7473 2920 3d3d  t len(events) ==
+00006a60: 2032 0a0a 6173 7365 7274 2065 7665 6e74   2..assert event
+00006a70: 735b 305d 2e73 7472 6561 6d5f 6e61 6d65  s[0].stream_name
+00006a80: 203d 3d20 7374 7265 616d 5f6e 616d 6531   == stream_name1
+00006a90: 0a61 7373 6572 7420 6576 656e 7473 5b30  .assert events[0
+00006aa0: 5d2e 7374 7265 616d 5f70 6f73 6974 696f  ].stream_positio
+00006ab0: 6e20 3d3d 2030 0a61 7373 6572 7420 6576  n == 0.assert ev
+00006ac0: 656e 7473 5b30 5d2e 7479 7065 203d 3d20  ents[0].type == 
+00006ad0: 6576 656e 7431 2e74 7970 650a 6173 7365  event1.type.asse
+00006ae0: 7274 2065 7665 6e74 735b 305d 2e64 6174  rt events[0].dat
+00006af0: 6120 3d3d 2065 7665 6e74 312e 6461 7461  a == event1.data
+00006b00: 0a0a 6173 7365 7274 2065 7665 6e74 735b  ..assert events[
+00006b10: 315d 2e73 7472 6561 6d5f 6e61 6d65 203d  1].stream_name =
+00006b20: 3d20 7374 7265 616d 5f6e 616d 6531 0a61  = stream_name1.a
+00006b30: 7373 6572 7420 6576 656e 7473 5b31 5d2e  ssert events[1].
+00006b40: 7374 7265 616d 5f70 6f73 6974 696f 6e20  stream_position 
+00006b50: 3d3d 2031 0a61 7373 6572 7420 6576 656e  == 1.assert even
+00006b60: 7473 5b31 5d2e 7479 7065 203d 3d20 6576  ts[1].type == ev
+00006b70: 656e 7432 2e74 7970 650a 6173 7365 7274  ent2.type.assert
+00006b80: 2065 7665 6e74 735b 315d 2e64 6174 6120   events[1].data 
+00006b90: 3d3d 2065 7665 6e74 322e 6461 7461 0a60  == event2.data.`
+00006ba0: 6060 0a0a 5468 6520 6578 616d 706c 6520  ``..The example 
+00006bb0: 6265 6c6f 7720 7368 6f77 7320 686f 7720  below shows how 
+00006bc0: 746f 2072 6561 6420 6120 6c69 6d69 7465  to read a limite
+00006bd0: 6420 6e75 6d62 6572 2028 6f6e 6529 206f  d number (one) o
+00006be0: 6620 7468 6520 7265 636f 7264 6564 0a65  f the recorded.e
+00006bf0: 7665 6e74 7320 696e 2061 2073 7472 6561  vents in a strea
+00006c00: 6d20 6261 636b 7761 7264 7320 6672 6f6d  m backwards from
+00006c10: 2061 2067 6976 656e 2073 7472 6561 6d20   a given stream 
+00006c20: 706f 7369 7469 6f6e 2e0a 0a60 6060 7079  position...```py
+00006c30: 7468 6f6e 0a65 7665 6e74 7320 3d20 6c69  thon.events = li
+00006c40: 7374 280a 2020 2020 636c 6965 6e74 2e72  st(.    client.r
+00006c50: 6561 645f 7374 7265 616d 5f65 7665 6e74  ead_stream_event
+00006c60: 7328 0a20 2020 2020 2020 2073 7472 6561  s(.        strea
+00006c70: 6d5f 6e61 6d65 3d73 7472 6561 6d5f 6e61  m_name=stream_na
+00006c80: 6d65 312c 0a20 2020 2020 2020 2073 7472  me1,.        str
+00006c90: 6561 6d5f 706f 7369 7469 6f6e 3d32 2c0a  eam_position=2,.
+00006ca0: 2020 2020 2020 2020 6261 636b 7761 7264          backward
+00006cb0: 733d 5472 7565 2c0a 2020 2020 2020 2020  s=True,.        
+00006cc0: 6c69 6d69 743d 312c 0a20 2020 2029 0a29  limit=1,.    ).)
+00006cd0: 0a0a 6173 7365 7274 206c 656e 2865 7665  ..assert len(eve
+00006ce0: 6e74 7329 203d 3d20 310a 0a61 7373 6572  nts) == 1..asser
+00006cf0: 7420 6576 656e 7473 5b30 5d2e 7374 7265  t events[0].stre
+00006d00: 616d 5f6e 616d 6520 3d3d 2073 7472 6561  am_name == strea
+00006d10: 6d5f 6e61 6d65 310a 6173 7365 7274 2065  m_name1.assert e
+00006d20: 7665 6e74 735b 305d 2e73 7472 6561 6d5f  vents[0].stream_
+00006d30: 706f 7369 7469 6f6e 203d 3d20 320a 6173  position == 2.as
+00006d40: 7365 7274 2065 7665 6e74 735b 305d 2e74  sert events[0].t
+00006d50: 7970 6520 3d3d 2065 7665 6e74 332e 7479  ype == event3.ty
+00006d60: 7065 0a61 7373 6572 7420 6576 656e 7473  pe.assert events
+00006d70: 5b30 5d2e 6461 7461 203d 3d20 6576 656e  [0].data == even
+00006d80: 7433 2e64 6174 610a 6060 600a 0a23 2323  t3.data.```..###
+00006d90: 2052 6561 6420 616c 6c20 6576 656e 7473   Read all events
+00006da0: 0a0a 5468 6520 6d65 7468 6f64 2060 7265  ..The method `re
+00006db0: 6164 5f61 6c6c 5f65 7665 6e74 7328 2960  ad_all_events()`
+00006dc0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+00006dd0: 7265 6164 2061 6c6c 2072 6563 6f72 6465  read all recorde
+00006de0: 6420 6576 656e 7473 0a69 6e20 7468 6520  d events.in the 
+00006df0: 6461 7461 6261 7365 2069 6e20 7468 6520  database in the 
+00006e00: 6f72 6465 7220 7468 6579 2077 6572 6520  order they were 
+00006e10: 7265 636f 7264 6564 2e20 416e 2069 7465  recorded. An ite
+00006e20: 7261 626c 6520 6f62 6a65 6374 206f 660a  rable object of.
+00006e30: 7265 636f 7264 6564 2065 7665 6e74 7320  recorded events 
+00006e40: 6973 2072 6574 7572 6e65 642e 2054 6869  is returned. Thi
+00006e50: 7320 6974 6572 6162 6c65 206f 626a 6563  s iterable objec
+00006e60: 7420 7769 6c6c 2073 746f 7020 7768 656e  t will stop when
+00006e70: 2069 7420 6861 730a 7969 656c 6465 6420   it has.yielded 
+00006e80: 7468 6520 6c61 7374 2072 6563 6f72 6465  the last recorde
+00006e90: 6420 6576 656e 742e 0a0a 5468 6973 206d  d event...This m
+00006ea0: 6574 686f 6420 7375 7070 6f72 7473 2073  ethod supports s
+00006eb0: 6978 206f 7074 696f 6e61 6c20 6172 6775  ix optional argu
+00006ec0: 6d65 6e74 732c 2060 636f 6d6d 6974 5f70  ments, `commit_p
+00006ed0: 6f73 6974 696f 6e60 2c20 6062 6163 6b77  osition`, `backw
+00006ee0: 6172 6473 602c 0a60 6669 6c74 6572 5f65  ards`,.`filter_e
+00006ef0: 7863 6c75 6465 602c 2060 6669 6c74 6572  xclude`, `filter
+00006f00: 5f69 6e63 6c75 6465 602c 2060 6c69 6d69  _include`, `limi
+00006f10: 7460 2c20 616e 6420 6074 696d 656f 7574  t`, and `timeout
+00006f20: 602e 0a0a 5468 6520 6f70 7469 6f6e 616c  `...The optional
+00006f30: 2061 7267 756d 656e 7420 6063 6f6d 6d69   argument `commi
+00006f40: 745f 706f 7369 7469 6f6e 6020 6973 2061  t_position` is a
+00006f50: 6e20 6f70 7469 6f6e 616c 2069 6e74 6567  n optional integ
+00006f60: 6572 2074 6861 7420 6361 6e20 6265 2075  er that can be u
+00006f70: 7365 6420 746f 0a73 7065 6369 6679 2074  sed to.specify t
+00006f80: 6865 2063 6f6d 6d69 7420 706f 7369 7469  he commit positi
+00006f90: 6f6e 2066 726f 6d20 7768 6963 6820 746f  on from which to
+00006fa0: 2073 7461 7274 2072 6561 6469 6e67 2e20   start reading. 
+00006fb0: 5468 6973 2061 7267 756d 656e 7420 6973  This argument is
+00006fc0: 2060 4e6f 6e65 6020 6279 0a64 6566 6175   `None` by.defau
+00006fd0: 6c74 2c20 6d65 616e 696e 6720 7468 6174  lt, meaning that
+00006fe0: 2061 6c6c 2074 6865 2065 7665 6e74 7320   all the events 
+00006ff0: 7769 6c6c 2062 6520 7265 6164 2065 6974  will be read eit
+00007000: 6865 7220 6672 6f6d 2074 6865 2073 7461  her from the sta
+00007010: 7274 2c20 6f72 0a66 726f 6d20 7468 6520  rt, or.from the 
+00007020: 656e 6420 6966 2060 6261 636b 7761 7264  end if `backward
+00007030: 7360 2069 7320 6054 7275 6560 2028 7365  s` is `True` (se
+00007040: 6520 6265 6c6f 7729 2e20 506c 6561 7365  e below). Please
+00007050: 206e 6f74 652c 2069 6620 7370 6563 6966   note, if specif
+00007060: 6965 642c 0a74 6865 2073 7065 6369 6669  ied,.the specifi
+00007070: 6564 2070 6f73 6974 696f 6e20 6d75 7374  ed position must
+00007080: 2062 6520 616e 2061 6374 7561 6c6c 7920   be an actually 
+00007090: 6578 6973 7469 6e67 2063 6f6d 6d69 7420  existing commit 
+000070a0: 706f 7369 7469 6f6e 2c20 6265 6361 7573  position, becaus
+000070b0: 650a 616e 7920 6f74 6865 7220 6e75 6d62  e.any other numb
+000070c0: 6572 2077 696c 6c20 7265 7375 6c74 2069  er will result i
+000070d0: 6e20 6120 7365 7276 6572 2065 7272 6f72  n a server error
+000070e0: 2028 6174 206c 6561 7374 2069 6e20 4576   (at least in Ev
+000070f0: 656e 7453 746f 7265 4442 2076 3231 2e31  entStoreDB v21.1
+00007100: 3029 2e0a 0a54 6865 206f 7074 696f 6e61  0)...The optiona
+00007110: 6c20 6172 6775 6d65 6e74 2060 6261 636b  l argument `back
+00007120: 7761 7264 7360 2069 7320 6120 626f 6f6c  wards` is a bool
+00007130: 6561 6e20 7768 6963 6820 6973 2062 7920  ean which is by 
+00007140: 6465 6661 756c 7420 6046 616c 7365 6020  default `False` 
+00007150: 6d65 616e 696e 6720 7468 650a 6576 656e  meaning the.even
+00007160: 7473 2077 696c 6c20 6265 2072 6561 6420  ts will be read 
+00007170: 666f 7277 6172 6473 2062 7920 6465 6661  forwards by defa
+00007180: 756c 742c 2073 6f20 7468 6174 2065 7665  ult, so that eve
+00007190: 6e74 7320 6172 6520 7265 7475 726e 6564  nts are returned
+000071a0: 2069 6e20 7468 650a 6f72 6465 7220 7468   in the.order th
+000071b0: 6579 2077 6572 6520 636f 6d6d 6974 7465  ey were committe
+000071c0: 642c 2049 6620 6062 6163 6b77 6172 6473  d, If `backwards
+000071d0: 6020 6973 2060 5472 7565 602c 2074 6865  ` is `True`, the
+000071e0: 2065 7665 6e74 7320 7769 6c6c 2062 6520   events will be 
+000071f0: 7265 6164 0a62 6163 6b77 6172 6473 2c20  read.backwards, 
+00007200: 736f 2074 6861 7420 6576 656e 7473 2061  so that events a
+00007210: 7265 2072 6574 7572 6e65 6420 696e 2072  re returned in r
+00007220: 6576 6572 7365 206f 7264 6572 2e0a 0a54  everse order...T
+00007230: 6865 206f 7074 696f 6e61 6c20 6172 6775  he optional argu
+00007240: 6d65 6e74 2060 6669 6c74 6572 5f65 7863  ment `filter_exc
+00007250: 6c75 6465 6020 6973 2061 2073 6571 7565  lude` is a seque
+00007260: 6e63 6520 6f66 2072 6567 756c 6172 2065  nce of regular e
+00007270: 7870 7265 7373 696f 6e73 2074 6861 740a  xpressions that.
+00007280: 6d61 7463 6820 7468 6520 7479 7065 2073  match the type s
+00007290: 7472 696e 6773 206f 6620 7265 636f 7264  trings of record
+000072a0: 6564 2065 7665 6e74 7320 7468 6174 2073  ed events that s
+000072b0: 686f 756c 6420 6e6f 7420 6265 2069 6e63  hould not be inc
+000072c0: 6c75 6465 642e 2042 7920 6465 6661 756c  luded. By defaul
+000072d0: 742c 0a74 6869 7320 6172 6775 6d65 6e74  t,.this argument
+000072e0: 2077 696c 6c20 6d61 7463 6820 2273 7973   will match "sys
+000072f0: 7465 6d20 6576 656e 7473 222c 2073 6f20  tem events", so 
+00007300: 7468 6174 2074 6865 7920 7769 6c6c 206e  that they will n
+00007310: 6f74 2062 6520 696e 636c 7564 6564 2e0a  ot be included..
+00007320: 5468 6973 2061 7267 756d 656e 7420 6973  This argument is
+00007330: 2069 676e 6f72 6564 2069 6620 6066 696c   ignored if `fil
+00007340: 7465 725f 696e 636c 7564 6560 2069 7320  ter_include` is 
+00007350: 7365 7420 746f 2061 206e 6f6e 2d65 6d70  set to a non-emp
+00007360: 7479 2073 6571 7565 6e63 652e 0a0a 5468  ty sequence...Th
+00007370: 6520 6f70 7469 6f6e 616c 2061 7267 756d  e optional argum
+00007380: 656e 7420 6066 696c 7465 725f 696e 636c  ent `filter_incl
+00007390: 7564 6560 2069 7320 6120 7365 7175 656e  ude` is a sequen
+000073a0: 6365 206f 6620 7265 6775 6c61 7220 6578  ce of regular ex
+000073b0: 7072 6573 7369 6f6e 730a 7468 6174 206d  pressions.that m
+000073c0: 6174 6368 2074 6865 2074 7970 6520 7374  atch the type st
+000073d0: 7269 6e67 7320 6f66 2072 6563 6f72 6465  rings of recorde
+000073e0: 6420 6576 656e 7473 2074 6861 7420 7368  d events that sh
+000073f0: 6f75 6c64 2062 6520 696e 636c 7564 6564  ould be included
+00007400: 2e20 4279 0a64 6566 6175 6c74 2c20 7468  . By.default, th
+00007410: 6973 2061 7267 756d 656e 7420 6973 2061  is argument is a
+00007420: 6e20 656d 7074 7920 7475 706c 652e 2049  n empty tuple. I
+00007430: 6620 7468 6973 2061 7267 756d 656e 7420  f this argument 
+00007440: 6973 2073 6574 2074 6f20 610a 6e6f 6e2d  is set to a.non-
+00007450: 656d 7074 7920 7365 7175 656e 6365 2c20  empty sequence, 
+00007460: 7468 6520 6066 696c 7465 725f 6578 636c  the `filter_excl
+00007470: 7564 6560 2061 7267 756d 656e 7420 6973  ude` argument is
+00007480: 2069 676e 6f72 6564 2e0a 0a54 6865 206f   ignored...The o
+00007490: 7074 696f 6e61 6c20 6172 6775 6d65 6e74  ptional argument
+000074a0: 2060 6c69 6d69 7460 2069 7320 616e 2069   `limit` is an i
+000074b0: 6e74 6567 6572 2077 6869 6368 206c 696d  nteger which lim
+000074c0: 6974 7320 7468 6520 6e75 6d62 6572 206f  its the number o
+000074d0: 6620 6576 656e 7473 2074 6861 7420 7769  f events that wi
+000074e0: 6c6c 0a62 6520 7265 7475 726e 6564 2e20  ll.be returned. 
+000074f0: 5468 6520 6465 6661 756c 7420 7661 6c75  The default valu
+00007500: 6520 6973 2060 7379 732e 6d61 7869 6e74  e is `sys.maxint
+00007510: 602e 0a0a 5468 6520 6f70 7469 6f6e 616c  `...The optional
+00007520: 2061 7267 756d 656e 7420 6074 696d 656f   argument `timeo
+00007530: 7574 6020 6973 2061 2050 7974 686f 6e20  ut` is a Python 
+00007540: 6066 6c6f 6174 6020 7768 6963 6820 7365  `float` which se
+00007550: 7473 2061 2064 6561 646c 696e 6520 666f  ts a deadline fo
+00007560: 7220 7468 6520 636f 6d70 6c65 7469 6f6e  r the completion
+00007570: 206f 660a 7468 6520 6752 5043 206f 7065   of.the gRPC ope
+00007580: 7261 7469 6f6e 2e0a 0a54 6865 2066 696c  ration...The fil
+00007590: 7465 7269 6e67 206f 6620 6576 656e 7473  tering of events
+000075a0: 2069 7320 646f 6e65 206f 6e20 7468 6520   is done on the 
+000075b0: 4576 656e 7453 746f 7265 4442 2073 6572  EventStoreDB ser
+000075c0: 7665 722e 2054 6865 0a60 6c69 6d69 7460  ver. The.`limit`
+000075d0: 2061 7267 756d 656e 7420 6973 2061 7070   argument is app
+000075e0: 6c69 6564 206f 6e20 7468 6520 7365 7276  lied on the serv
+000075f0: 6572 2061 6674 6572 2066 696c 7465 7269  er after filteri
+00007600: 6e67 2e20 5365 6520 6265 6c6f 7720 666f  ng. See below fo
+00007610: 720a 6d6f 7265 2069 6e66 6f72 6d61 7469  r.more informati
+00007620: 6f6e 2061 626f 7574 2066 696c 7465 7220  on about filter 
+00007630: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
+00007640: 6f6e 732e 0a0a 5768 656e 2072 6561 6469  ons...When readi
+00007650: 6e67 2066 6f72 7761 7264 7320 6672 6f6d  ng forwards from
+00007660: 2061 2073 7065 6369 6669 6320 636f 6d6d   a specific comm
+00007670: 6974 2070 6f73 6974 696f 6e2c 2074 6865  it position, the
+00007680: 2065 7665 6e74 2061 7420 7468 6520 7370   event at the sp
+00007690: 6563 6966 6965 640a 706f 7369 7469 6f6e  ecified.position
+000076a0: 2057 494c 4c20 6265 2069 6e63 6c75 6465   WILL be include
+000076b0: 642e 2048 6f77 6576 6572 2c20 7768 656e  d. However, when
+000076c0: 2072 6561 6469 6e67 2062 6163 6b77 6172   reading backwar
+000076d0: 6473 2c20 7468 6520 6576 656e 7420 6174  ds, the event at
+000076e0: 2074 6865 0a73 7065 6369 6669 6564 2070   the.specified p
+000076f0: 6f73 6974 696f 6e20 7769 6c6c 204e 4f54  osition will NOT
+00007700: 2062 6520 696e 636c 7564 6564 2e20 2854   be included. (T
+00007710: 6869 7320 6e6f 6e2d 696e 636c 7573 6976  his non-inclusiv
+00007720: 6520 6265 6861 7669 6f75 722c 206f 6620  e behaviour, of 
+00007730: 6578 636c 7564 696e 670a 7468 6520 7370  excluding.the sp
+00007740: 6563 6966 6965 6420 636f 6d6d 6974 2070  ecified commit p
+00007750: 6f73 6974 696f 6e20 7768 656e 2072 6561  osition when rea
+00007760: 6469 6e67 2061 6c6c 2073 7472 6561 6d73  ding all streams
+00007770: 2062 6163 6b77 6172 6473 2c20 6469 6666   backwards, diff
+00007780: 6572 7320 6672 6f6d 2074 6865 0a62 6568  ers from the.beh
+00007790: 6176 696f 7572 2077 6865 6e20 7265 6164  aviour when read
+000077a0: 696e 6720 6120 7374 7265 616d 2062 6163  ing a stream bac
+000077b0: 6b77 6172 6473 2066 726f 6d20 6120 7370  kwards from a sp
+000077c0: 6563 6966 6963 2073 7472 6561 6d20 706f  ecific stream po
+000077d0: 7369 7469 6f6e 2c20 4927 6d0a 6e6f 7420  sition, I'm.not 
+000077e0: 7375 7265 2077 6879 2e29 0a0a 5468 6520  sure why.)..The 
+000077f0: 6578 616d 706c 6520 6265 6c6f 7720 7368  example below sh
+00007800: 6f77 7320 686f 7720 746f 2072 6561 6420  ows how to read 
+00007810: 616c 6c20 6576 656e 7473 2069 6e20 7468  all events in th
+00007820: 6520 6461 7461 6261 7365 2069 6e20 7468  e database in th
+00007830: 650a 6f72 6465 7220 7468 6579 2077 6572  e.order they wer
+00007840: 6520 7265 636f 7264 6564 2e0a 0a60 6060  e recorded...```
+00007850: 7079 7468 6f6e 0a65 7665 6e74 7320 3d20  python.events = 
+00007860: 6c69 7374 2863 6c69 656e 742e 7265 6164  list(client.read
+00007870: 5f61 6c6c 5f65 7665 6e74 7328 2929 0a0a  _all_events())..
+00007880: 6173 7365 7274 206c 656e 2865 7665 6e74  assert len(event
+00007890: 7329 203e 3d20 330a 6060 600a 0a54 6865  s) >= 3.```..The
+000078a0: 2065 7861 6d70 6c65 2062 656c 6f77 2073   example below s
+000078b0: 686f 7773 2068 6f77 2074 6f20 7265 6164  hows how to read
+000078c0: 2061 6c6c 2072 6563 6f72 6465 6420 6576   all recorded ev
+000078d0: 656e 7473 2066 726f 6d20 6120 7370 6563  ents from a spec
+000078e0: 6966 6963 2063 6f6d 6d69 7420 706f 7369  ific commit posi
+000078f0: 7469 6f6e 2e0a 0a60 6060 7079 7468 6f6e  tion...```python
+00007900: 0a65 7665 6e74 7320 3d20 6c69 7374 280a  .events = list(.
+00007910: 2020 2020 636c 6965 6e74 2e72 6561 645f      client.read_
+00007920: 616c 6c5f 6576 656e 7473 280a 2020 2020  all_events(.    
+00007930: 2020 2020 636f 6d6d 6974 5f70 6f73 6974      commit_posit
+00007940: 696f 6e3d 636f 6d6d 6974 5f70 6f73 6974  ion=commit_posit
+00007950: 696f 6e31 0a20 2020 2029 0a29 0a0a 6173  ion1.    ).)..as
+00007960: 7365 7274 206c 656e 2865 7665 6e74 7329  sert len(events)
+00007970: 203d 3d20 330a 0a61 7373 6572 7420 6576   == 3..assert ev
+00007980: 656e 7473 5b30 5d2e 7374 7265 616d 5f6e  ents[0].stream_n
+00007990: 616d 6520 3d3d 2073 7472 6561 6d5f 6e61  ame == stream_na
+000079a0: 6d65 310a 6173 7365 7274 2065 7665 6e74  me1.assert event
+000079b0: 735b 305d 2e73 7472 6561 6d5f 706f 7369  s[0].stream_posi
+000079c0: 7469 6f6e 203d 3d20 300a 6173 7365 7274  tion == 0.assert
+000079d0: 2065 7665 6e74 735b 305d 2e74 7970 6520   events[0].type 
+000079e0: 3d3d 2065 7665 6e74 312e 7479 7065 0a61  == event1.type.a
+000079f0: 7373 6572 7420 6576 656e 7473 5b30 5d2e  ssert events[0].
+00007a00: 6461 7461 203d 3d20 6576 656e 7431 2e64  data == event1.d
+00007a10: 6174 610a 0a61 7373 6572 7420 6576 656e  ata..assert even
+00007a20: 7473 5b31 5d2e 7374 7265 616d 5f6e 616d  ts[1].stream_nam
+00007a30: 6520 3d3d 2073 7472 6561 6d5f 6e61 6d65  e == stream_name
+00007a40: 310a 6173 7365 7274 2065 7665 6e74 735b  1.assert events[
+00007a50: 315d 2e73 7472 6561 6d5f 706f 7369 7469  1].stream_positi
+00007a60: 6f6e 203d 3d20 310a 6173 7365 7274 2065  on == 1.assert e
+00007a70: 7665 6e74 735b 315d 2e74 7970 6520 3d3d  vents[1].type ==
+00007a80: 2065 7665 6e74 322e 7479 7065 0a61 7373   event2.type.ass
+00007a90: 6572 7420 6576 656e 7473 5b31 5d2e 6461  ert events[1].da
+00007aa0: 7461 203d 3d20 6576 656e 7432 2e64 6174  ta == event2.dat
+00007ab0: 610a 0a61 7373 6572 7420 6576 656e 7473  a..assert events
+00007ac0: 5b32 5d2e 7374 7265 616d 5f6e 616d 6520  [2].stream_name 
+00007ad0: 3d3d 2073 7472 6561 6d5f 6e61 6d65 310a  == stream_name1.
+00007ae0: 6173 7365 7274 2065 7665 6e74 735b 325d  assert events[2]
+00007af0: 2e73 7472 6561 6d5f 706f 7369 7469 6f6e  .stream_position
+00007b00: 203d 3d20 320a 6173 7365 7274 2065 7665   == 2.assert eve
+00007b10: 6e74 735b 325d 2e74 7970 6520 3d3d 2065  nts[2].type == e
+00007b20: 7665 6e74 332e 7479 7065 0a61 7373 6572  vent3.type.asser
+00007b30: 7420 6576 656e 7473 5b32 5d2e 6461 7461  t events[2].data
+00007b40: 203d 3d20 6576 656e 7433 2e64 6174 610a   == event3.data.
+00007b50: 6060 600a 0a54 6865 2065 7861 6d70 6c65  ```..The example
+00007b60: 2062 656c 6f77 2073 686f 7773 2068 6f77   below shows how
+00007b70: 2074 6f20 7265 6164 2061 6c6c 2072 6563   to read all rec
+00007b80: 6f72 6465 6420 6576 656e 7473 2069 6e20  orded events in 
+00007b90: 7265 7665 7273 6520 6f72 6465 722e 0a0a  reverse order...
+00007ba0: 6060 6070 7974 686f 6e0a 6576 656e 7473  ```python.events
+00007bb0: 203d 206c 6973 7428 0a20 2020 2063 6c69   = list(.    cli
+00007bc0: 656e 742e 7265 6164 5f61 6c6c 5f65 7665  ent.read_all_eve
+00007bd0: 6e74 7328 0a20 2020 2020 2020 2062 6163  nts(.        bac
+00007be0: 6b77 6172 6473 3d54 7275 650a 2020 2020  kwards=True.    
+00007bf0: 290a 290a 0a61 7373 6572 7420 6c65 6e28  ).)..assert len(
+00007c00: 6576 656e 7473 2920 3e3d 2033 0a0a 6173  events) >= 3..as
+00007c10: 7365 7274 2065 7665 6e74 735b 305d 2e73  sert events[0].s
+00007c20: 7472 6561 6d5f 6e61 6d65 203d 3d20 7374  tream_name == st
+00007c30: 7265 616d 5f6e 616d 6531 0a61 7373 6572  ream_name1.asser
+00007c40: 7420 6576 656e 7473 5b30 5d2e 7374 7265  t events[0].stre
+00007c50: 616d 5f70 6f73 6974 696f 6e20 3d3d 2032  am_position == 2
+00007c60: 0a61 7373 6572 7420 6576 656e 7473 5b30  .assert events[0
+00007c70: 5d2e 7479 7065 203d 3d20 6576 656e 7433  ].type == event3
+00007c80: 2e74 7970 650a 6173 7365 7274 2065 7665  .type.assert eve
+00007c90: 6e74 735b 305d 2e64 6174 6120 3d3d 2065  nts[0].data == e
+00007ca0: 7665 6e74 332e 6461 7461 0a0a 6173 7365  vent3.data..asse
+00007cb0: 7274 2065 7665 6e74 735b 315d 2e73 7472  rt events[1].str
+00007cc0: 6561 6d5f 6e61 6d65 203d 3d20 7374 7265  eam_name == stre
+00007cd0: 616d 5f6e 616d 6531 0a61 7373 6572 7420  am_name1.assert 
+00007ce0: 6576 656e 7473 5b31 5d2e 7374 7265 616d  events[1].stream
+00007cf0: 5f70 6f73 6974 696f 6e20 3d3d 2031 0a61  _position == 1.a
+00007d00: 7373 6572 7420 6576 656e 7473 5b31 5d2e  ssert events[1].
+00007d10: 7479 7065 203d 3d20 6576 656e 7432 2e74  type == event2.t
+00007d20: 7970 650a 6173 7365 7274 2065 7665 6e74  ype.assert event
+00007d30: 735b 315d 2e64 6174 6120 3d3d 2065 7665  s[1].data == eve
+00007d40: 6e74 322e 6461 7461 0a0a 6173 7365 7274  nt2.data..assert
+00007d50: 2065 7665 6e74 735b 325d 2e73 7472 6561   events[2].strea
+00007d60: 6d5f 6e61 6d65 203d 3d20 7374 7265 616d  m_name == stream
+00007d70: 5f6e 616d 6531 0a61 7373 6572 7420 6576  _name1.assert ev
+00007d80: 656e 7473 5b32 5d2e 7374 7265 616d 5f70  ents[2].stream_p
+00007d90: 6f73 6974 696f 6e20 3d3d 2030 0a61 7373  osition == 0.ass
+00007da0: 6572 7420 6576 656e 7473 5b32 5d2e 7479  ert events[2].ty
+00007db0: 7065 203d 3d20 6576 656e 7431 2e74 7970  pe == event1.typ
+00007dc0: 650a 6173 7365 7274 2065 7665 6e74 735b  e.assert events[
+00007dd0: 325d 2e64 6174 6120 3d3d 2065 7665 6e74  2].data == event
+00007de0: 312e 6461 7461 0a60 6060 0a0a 5468 6520  1.data.```..The 
+00007df0: 6578 616d 706c 6520 6265 6c6f 7720 7368  example below sh
+00007e00: 6f77 7320 686f 7720 746f 2072 6561 6420  ows how to read 
+00007e10: 6120 6c69 6d69 7465 6420 6e75 6d62 6572  a limited number
+00007e20: 2028 6f6e 6529 206f 6620 7468 6520 7265   (one) of the re
+00007e30: 636f 7264 6564 2065 7665 6e74 730a 696e  corded events.in
+00007e40: 2074 6865 2064 6174 6162 6173 6520 666f   the database fo
+00007e50: 7277 6172 6473 2066 726f 6d20 6120 7370  rwards from a sp
+00007e60: 6563 6966 6963 2063 6f6d 6d69 7420 706f  ecific commit po
+00007e70: 7369 7469 6f6e 2e20 506c 6561 7365 206e  sition. Please n
+00007e80: 6f74 652c 2077 6865 6e20 7265 6164 696e  ote, when readin
+00007e90: 670a 616c 6c20 6576 656e 7473 2066 6f72  g.all events for
+00007ea0: 7761 7264 7320 6672 6f6d 2061 2073 7065  wards from a spe
+00007eb0: 6369 6669 6320 636f 6d6d 6974 2070 6f73  cific commit pos
+00007ec0: 6974 696f 6e2c 2074 6865 2065 7665 6e74  ition, the event
+00007ed0: 2061 7420 7468 6520 7370 6563 6966 6965   at the specifie
+00007ee0: 640a 706f 7369 7469 6f6e 2057 494c 4c20  d.position WILL 
+00007ef0: 6265 2069 6e63 6c75 6465 642e 0a0a 0a60  be included....`
+00007f00: 6060 7079 7468 6f6e 0a65 7665 6e74 7320  ``python.events 
+00007f10: 3d20 6c69 7374 280a 2020 2020 636c 6965  = list(.    clie
+00007f20: 6e74 2e72 6561 645f 616c 6c5f 6576 656e  nt.read_all_even
+00007f30: 7473 280a 2020 2020 2020 2020 636f 6d6d  ts(.        comm
+00007f40: 6974 5f70 6f73 6974 696f 6e3d 636f 6d6d  it_position=comm
+00007f50: 6974 5f70 6f73 6974 696f 6e31 2c0a 2020  it_position1,.  
+00007f60: 2020 2020 2020 6c69 6d69 743d 312c 0a20        limit=1,. 
+00007f70: 2020 2029 0a29 0a0a 6173 7365 7274 206c     ).)..assert l
+00007f80: 656e 2865 7665 6e74 7329 203d 3d20 310a  en(events) == 1.
+00007f90: 0a61 7373 6572 7420 6576 656e 7473 5b30  .assert events[0
+00007fa0: 5d2e 7374 7265 616d 5f6e 616d 6520 3d3d  ].stream_name ==
+00007fb0: 2073 7472 6561 6d5f 6e61 6d65 310a 6173   stream_name1.as
+00007fc0: 7365 7274 2065 7665 6e74 735b 305d 2e73  sert events[0].s
+00007fd0: 7472 6561 6d5f 706f 7369 7469 6f6e 203d  tream_position =
+00007fe0: 3d20 300a 6173 7365 7274 2065 7665 6e74  = 0.assert event
+00007ff0: 735b 305d 2e74 7970 6520 3d3d 2065 7665  s[0].type == eve
+00008000: 6e74 312e 7479 7065 0a61 7373 6572 7420  nt1.type.assert 
+00008010: 6576 656e 7473 5b30 5d2e 6461 7461 203d  events[0].data =
+00008020: 3d20 6576 656e 7431 2e64 6174 610a 0a61  = event1.data..a
+00008030: 7373 6572 7420 6576 656e 7473 5b30 5d2e  ssert events[0].
+00008040: 636f 6d6d 6974 5f70 6f73 6974 696f 6e20  commit_position 
+00008050: 3d3d 2063 6f6d 6d69 745f 706f 7369 7469  == commit_positi
+00008060: 6f6e 310a 6060 600a 0a54 6865 2065 7861  on1.```..The exa
+00008070: 6d70 6c65 2062 656c 6f77 2073 686f 7773  mple below shows
+00008080: 2068 6f77 2074 6f20 7265 6164 2061 206c   how to read a l
+00008090: 696d 6974 6564 206e 756d 6265 7220 286f  imited number (o
+000080a0: 6e65 2920 6f66 2074 6865 2072 6563 6f72  ne) of the recor
+000080b0: 6465 6420 6576 656e 7473 0a69 6e20 7468  ded events.in th
+000080c0: 6520 6461 7461 6261 7365 2062 6163 6b77  e database backw
+000080d0: 6172 6473 2066 726f 6d20 7468 6520 656e  ards from the en
+000080e0: 642e 2054 6869 7320 6769 7665 7320 7468  d. This gives th
+000080f0: 6520 6c61 7374 2072 6563 6f72 6465 6420  e last recorded 
+00008100: 6576 656e 742e 0a0a 6060 6070 7974 686f  event...```pytho
+00008110: 6e0a 6576 656e 7473 203d 206c 6973 7428  n.events = list(
+00008120: 0a20 2020 2063 6c69 656e 742e 7265 6164  .    client.read
+00008130: 5f61 6c6c 5f65 7665 6e74 7328 0a20 2020  _all_events(.   
+00008140: 2020 2020 2062 6163 6b77 6172 6473 3d54       backwards=T
+00008150: 7275 652c 0a20 2020 2020 2020 206c 696d  rue,.        lim
+00008160: 6974 3d31 2c0a 2020 2020 290a 290a 0a61  it=1,.    ).)..a
+00008170: 7373 6572 7420 6c65 6e28 6576 656e 7473  ssert len(events
+00008180: 2920 3d3d 2031 0a0a 6173 7365 7274 2065  ) == 1..assert e
+00008190: 7665 6e74 735b 305d 2e73 7472 6561 6d5f  vents[0].stream_
+000081a0: 6e61 6d65 203d 3d20 7374 7265 616d 5f6e  name == stream_n
+000081b0: 616d 6531 0a61 7373 6572 7420 6576 656e  ame1.assert even
+000081c0: 7473 5b30 5d2e 7374 7265 616d 5f70 6f73  ts[0].stream_pos
+000081d0: 6974 696f 6e20 3d3d 2032 0a61 7373 6572  ition == 2.asser
+000081e0: 7420 6576 656e 7473 5b30 5d2e 7479 7065  t events[0].type
+000081f0: 203d 3d20 6576 656e 7433 2e74 7970 650a   == event3.type.
+00008200: 6173 7365 7274 2065 7665 6e74 735b 305d  assert events[0]
+00008210: 2e64 6174 6120 3d3d 2065 7665 6e74 332e  .data == event3.
+00008220: 6461 7461 0a60 6060 0a0a 5468 6520 6578  data.```..The ex
+00008230: 616d 706c 6520 6265 6c6f 7720 7368 6f77  ample below show
+00008240: 7320 686f 7720 746f 2072 6561 6420 6120  s how to read a 
+00008250: 6c69 6d69 7465 6420 6e75 6d62 6572 2028  limited number (
+00008260: 6f6e 6529 206f 6620 7468 6520 7265 636f  one) of the reco
+00008270: 7264 6564 2065 7665 6e74 730a 696e 2074  rded events.in t
+00008280: 6865 2064 6174 6162 6173 6520 6261 636b  he database back
+00008290: 7761 7264 7320 6672 6f6d 2061 2073 7065  wards from a spe
+000082a0: 6369 6669 6320 636f 6d6d 6974 2070 6f73  cific commit pos
+000082b0: 6974 696f 6e2e 2050 6c65 6173 6520 6e6f  ition. Please no
+000082c0: 7465 2c20 7768 656e 2072 6561 6469 6e67  te, when reading
+000082d0: 0a61 6c6c 2065 7665 6e74 7320 6261 636b  .all events back
+000082e0: 7761 7264 7320 6672 6f6d 2061 2073 7065  wards from a spe
+000082f0: 6369 6669 6320 636f 6d6d 6974 2070 6f73  cific commit pos
+00008300: 6974 696f 6e2c 2074 6865 2065 7665 6e74  ition, the event
+00008310: 2061 7420 7468 6520 7370 6563 6966 6965   at the specifie
+00008320: 640a 706f 7369 7469 6f6e 2057 494c 4c20  d.position WILL 
+00008330: 4e4f 5420 6265 2069 6e63 6c75 6465 642e  NOT be included.
+00008340: 0a0a 6060 6070 7974 686f 6e0a 6576 656e  ..```python.even
+00008350: 7473 203d 206c 6973 7428 0a20 2020 2063  ts = list(.    c
+00008360: 6c69 656e 742e 7265 6164 5f61 6c6c 5f65  lient.read_all_e
+00008370: 7665 6e74 7328 0a20 2020 2020 2020 2063  vents(.        c
+00008380: 6f6d 6d69 745f 706f 7369 7469 6f6e 3d63  ommit_position=c
+00008390: 6f6d 6d69 745f 706f 7369 7469 6f6e 322c  ommit_position2,
+000083a0: 0a20 2020 2020 2020 2062 6163 6b77 6172  .        backwar
+000083b0: 6473 3d54 7275 652c 0a20 2020 2020 2020  ds=True,.       
+000083c0: 206c 696d 6974 3d31 2c0a 2020 2020 290a   limit=1,.    ).
+000083d0: 290a 0a61 7373 6572 7420 6c65 6e28 6576  )..assert len(ev
+000083e0: 656e 7473 2920 3d3d 2031 0a0a 6173 7365  ents) == 1..asse
+000083f0: 7274 2065 7665 6e74 735b 305d 2e63 6f6d  rt events[0].com
+00008400: 6d69 745f 706f 7369 7469 6f6e 203c 2063  mit_position < c
+00008410: 6f6d 6d69 745f 706f 7369 7469 6f6e 320a  ommit_position2.
+00008420: 6060 600a 0a0a 2323 2320 4765 7420 6375  ```...### Get cu
+00008430: 7272 656e 7420 7374 7265 616d 2070 6f73  rrent stream pos
+00008440: 6974 696f 6e0a 0a54 6865 2060 6765 745f  ition..The `get_
+00008450: 7374 7265 616d 5f70 6f73 6974 696f 6e28  stream_position(
+00008460: 2960 206d 6574 686f 6420 6361 6e20 6265  )` method can be
+00008470: 2075 7365 6420 746f 0a67 6574 2074 6865   used to.get the
+00008480: 2022 7374 7265 616d 2070 6f73 6974 696f   "stream positio
+00008490: 6e22 206f 6620 7468 6520 6c61 7374 2072  n" of the last r
+000084a0: 6563 6f72 6465 6420 6576 656e 7420 696e  ecorded event in
+000084b0: 2061 2073 7472 6561 6d2e 0a0a 5468 6973   a stream...This
+000084c0: 206d 6574 686f 6420 6861 7320 6120 6073   method has a `s
+000084d0: 7472 6561 6d5f 6e61 6d65 6020 6172 6775  tream_name` argu
+000084e0: 6d65 6e74 2c20 7768 6963 6820 6973 2072  ment, which is r
+000084f0: 6571 7569 7265 642e 0a0a 5468 6973 206d  equired...This m
+00008500: 6574 686f 6420 616c 736f 2074 616b 6573  ethod also takes
+00008510: 2061 6e20 6f70 7469 6f6e 616c 2060 7469   an optional `ti
+00008520: 6d65 6f75 7460 2061 7267 756d 656e 742c  meout` argument,
+00008530: 2074 6861 740a 6973 2065 7870 6563 7465   that.is expecte
+00008540: 6420 746f 2062 6520 6120 5079 7468 6f6e  d to be a Python
+00008550: 2060 666c 6f61 7460 2c20 7768 6963 6820   `float`, which 
+00008560: 7365 7473 2061 2064 6561 646c 696e 650a  sets a deadline.
+00008570: 666f 7220 7468 6520 636f 6d70 6c65 7469  for the completi
+00008580: 6f6e 206f 6620 7468 6520 6752 5043 206f  on of the gRPC o
+00008590: 7065 7261 7469 6f6e 2e0a 0a54 6865 2073  peration...The s
+000085a0: 6571 7565 6e63 6520 6f66 2070 6f73 6974  equence of posit
+000085b0: 696f 6e73 2069 6e20 6120 7374 7265 616d  ions in a stream
+000085c0: 2069 7320 6761 706c 6573 732e 2049 7420   is gapless. It 
+000085d0: 6973 207a 6572 6f2d 6261 7365 642c 0a73  is zero-based,.s
+000085e0: 6f20 7468 6174 2061 2073 7472 6561 6d20  o that a stream 
+000085f0: 7769 7468 206f 6e65 2072 6563 6f72 6465  with one recorde
+00008600: 6420 6576 656e 7420 6861 7320 6120 6375  d event has a cu
+00008610: 7272 656e 7420 7374 7265 616d 0a70 6f73  rrent stream.pos
+00008620: 6974 696f 6e20 6f66 2060 3060 2e20 5468  ition of `0`. Th
+00008630: 6520 6375 7272 656e 7420 7374 7265 616d  e current stream
+00008640: 2070 6f73 6974 696f 6e20 6973 2060 3160   position is `1`
+00008650: 2077 6865 6e20 6120 7374 7265 616d 2068   when a stream h
+00008660: 6173 0a74 776f 2065 7665 6e74 732c 2061  as.two events, a
+00008670: 6e64 2069 7420 6973 2060 3260 2077 6865  nd it is `2` whe
+00008680: 6e20 7468 6572 6520 6172 6520 6576 656e  n there are even
+00008690: 7473 2c20 616e 6420 736f 206f 6e2e 0a0a  ts, and so on...
+000086a0: 496e 2074 6865 2065 7861 6d70 6c65 2062  In the example b
+000086b0: 656c 6f77 2c20 7468 6520 6375 7272 656e  elow, the curren
+000086c0: 7420 7374 7265 616d 2070 6f73 6974 696f  t stream positio
+000086d0: 6e20 6973 206f 6274 6169 6e65 6420 6f66  n is obtained of
+000086e0: 2074 6865 0a73 7472 6561 6d20 746f 2077   the.stream to w
+000086f0: 6869 6368 2065 7665 6e74 7320 7765 7265  hich events were
+00008700: 2061 7070 656e 6465 6420 696e 2074 6865   appended in the
+00008710: 2065 7861 6d70 6c65 7320 6162 6f76 652e   examples above.
+00008720: 0a42 6563 6175 7365 2074 6865 2073 6571  .Because the seq
+00008730: 7565 6e63 6520 6f66 2073 7472 6561 6d20  uence of stream 
+00008740: 706f 7369 7469 6f6e 7320 6973 207a 6572  positions is zer
+00008750: 6f2d 6261 7365 642c 2061 6e64 2062 6563  o-based, and bec
+00008760: 6175 7365 0a74 6872 6565 2065 7665 6e74  ause.three event
+00008770: 7320 7765 7265 2061 7070 656e 6465 642c  s were appended,
+00008780: 2073 6f20 7468 6520 6375 7272 656e 7420   so the current 
+00008790: 7374 7265 616d 2070 6f73 6974 696f 6e20  stream position 
+000087a0: 6973 2060 3260 2e0a 0a60 6060 7079 7468  is `2`...```pyth
+000087b0: 6f6e 0a73 7472 6561 6d5f 706f 7369 7469  on.stream_positi
+000087c0: 6f6e 203d 2063 6c69 656e 742e 6765 745f  on = client.get_
+000087d0: 7374 7265 616d 5f70 6f73 6974 696f 6e28  stream_position(
+000087e0: 0a20 2020 2073 7472 6561 6d5f 6e61 6d65  .    stream_name
+000087f0: 3d73 7472 6561 6d5f 6e61 6d65 310a 290a  =stream_name1.).
+00008800: 0a61 7373 6572 7420 7374 7265 616d 5f70  .assert stream_p
+00008810: 6f73 6974 696f 6e20 3d3d 2032 0a60 6060  osition == 2.```
+00008820: 0a0a 4966 2061 2073 7472 6561 6d20 646f  ..If a stream do
+00008830: 6573 206e 6f74 2065 7869 7374 2c20 7468  es not exist, th
+00008840: 6520 7265 7475 726e 6564 2073 7472 6561  e returned strea
+00008850: 6d20 706f 7369 7469 6f6e 2076 616c 7565  m position value
+00008860: 2069 7320 604e 6f6e 6560 2c0a 7768 6963   is `None`,.whic
+00008870: 6820 6d61 7463 6865 7320 7468 6520 7265  h matches the re
+00008880: 7175 6972 6564 2065 7870 6563 7465 6420  quired expected 
+00008890: 706f 7369 7469 6f6e 2077 6865 6e20 6170  position when ap
+000088a0: 7065 6e64 696e 6720 7468 6520 6669 7273  pending the firs
+000088b0: 7420 6576 656e 740a 6f66 2061 206e 6577  t event.of a new
+000088c0: 2073 7472 6561 6d20 2873 6565 2061 626f   stream (see abo
+000088d0: 7665 292e 0a0a 6060 6070 7974 686f 6e0a  ve)...```python.
+000088e0: 7374 7265 616d 5f70 6f73 6974 696f 6e20  stream_position 
+000088f0: 3d20 636c 6965 6e74 2e67 6574 5f73 7472  = client.get_str
+00008900: 6561 6d5f 706f 7369 7469 6f6e 280a 2020  eam_position(.  
+00008910: 2020 7374 7265 616d 5f6e 616d 653d 7374    stream_name=st
+00008920: 7228 7575 6964 3428 2929 0a29 0a0a 6173  r(uuid4()).)..as
+00008930: 7365 7274 2073 7472 6561 6d5f 706f 7369  sert stream_posi
+00008940: 7469 6f6e 203d 3d20 4e6f 6e65 0a60 6060  tion == None.```
+00008950: 0a0a 5468 6973 206d 6574 686f 6420 7461  ..This method ta
+00008960: 6b65 7320 616e 206f 7074 696f 6e61 6c20  kes an optional 
+00008970: 6172 6775 6d65 6e74 2060 7469 6d65 6f75  argument `timeou
+00008980: 7460 2077 6869 6368 2069 7320 6120 5079  t` which is a Py
+00008990: 7468 6f6e 2060 666c 6f61 7460 2074 6861  thon `float` tha
+000089a0: 7420 7365 7473 0a61 2064 6561 646c 696e  t sets.a deadlin
+000089b0: 6520 666f 7220 7468 6520 636f 6d70 6c65  e for the comple
+000089c0: 7469 6f6e 206f 6620 7468 6520 6752 5043  tion of the gRPC
+000089d0: 206f 7065 7261 7469 6f6e 2e0a 0a0a 2323   operation....##
+000089e0: 2320 4765 7420 6375 7272 656e 7420 636f  # Get current co
+000089f0: 6d6d 6974 2070 6f73 6974 696f 6e0a 0a54  mmit position..T
+00008a00: 6865 206d 6574 686f 6420 6067 6574 5f63  he method `get_c
+00008a10: 6f6d 6d69 745f 706f 7369 7469 6f6e 2829  ommit_position()
+00008a20: 6020 6361 6e20 6265 2075 7365 6420 746f  ` can be used to
+00008a30: 2067 6574 2074 6865 2063 7572 7265 6e74   get the current
+00008a40: 0a63 6f6d 6d69 7420 706f 7369 7469 6f6e  .commit position
+00008a50: 206f 6620 7468 6520 6461 7461 6261 7365   of the database
+00008a60: 2e0a 0a60 6060 7079 7468 6f6e 0a63 6f6d  ...```python.com
+00008a70: 6d69 745f 706f 7369 7469 6f6e 203d 2063  mit_position = c
+00008a80: 6c69 656e 742e 6765 745f 636f 6d6d 6974  lient.get_commit
+00008a90: 5f70 6f73 6974 696f 6e28 290a 6060 600a  _position().```.
+00008aa0: 0a54 6869 7320 6d65 7468 6f64 2074 616b  .This method tak
+00008ab0: 6573 2061 6e20 6f70 7469 6f6e 616c 2061  es an optional a
+00008ac0: 7267 756d 656e 7420 6074 696d 656f 7574  rgument `timeout
+00008ad0: 6020 7768 6963 6820 6973 2061 2050 7974  ` which is a Pyt
+00008ae0: 686f 6e20 6066 6c6f 6174 6020 7468 6174  hon `float` that
+00008af0: 2073 6574 730a 6120 6465 6164 6c69 6e65   sets.a deadline
+00008b00: 2066 6f72 2074 6865 2063 6f6d 706c 6574   for the complet
+00008b10: 696f 6e20 6f66 2074 6865 2067 5250 4320  ion of the gRPC 
+00008b20: 6f70 6572 6174 696f 6e2e 0a0a 5468 6973  operation...This
+00008b30: 206d 6574 686f 6420 6361 6e20 6265 2075   method can be u
+00008b40: 7365 6675 6c20 746f 206d 6561 7375 7265  seful to measure
+00008b50: 2070 726f 6772 6573 7320 6f66 2061 2064   progress of a d
+00008b60: 6f77 6e73 7472 6561 6d20 636f 6d70 6f6e  ownstream compon
+00008b70: 656e 740a 7468 6174 2069 7320 7072 6f63  ent.that is proc
+00008b80: 6573 7369 6e67 2061 6c6c 2072 6563 6f72  essing all recor
+00008b90: 6465 6420 6576 656e 7473 2c20 6279 2063  ded events, by c
+00008ba0: 6f6d 7061 7269 6e67 2074 6865 2063 7572  omparing the cur
+00008bb0: 7265 6e74 2063 6f6d 6d69 740a 706f 7369  rent commit.posi
+00008bc0: 7469 6f6e 2077 6974 6820 7468 6520 7265  tion with the re
+00008bd0: 636f 7264 6564 2063 6f6d 6d69 7420 706f  corded commit po
+00008be0: 7369 7469 6f6e 206f 6620 7468 6520 6c61  sition of the la
+00008bf0: 7374 2073 7563 6365 7373 6675 6c6c 7920  st successfully 
+00008c00: 7072 6f63 6573 7365 640a 6576 656e 7420  processed.event 
+00008c10: 696e 2061 2064 6f77 6e73 7472 6561 6d20  in a downstream 
+00008c20: 636f 6d70 6f6e 656e 742e 0a0a 5468 6520  component...The 
+00008c30: 7661 6c75 6520 6f66 2074 6865 2060 636f  value of the `co
+00008c40: 6d6d 6974 5f70 6f73 6974 696f 6e60 2061  mmit_position` a
+00008c50: 7267 756d 656e 7420 7768 656e 2072 6561  rgument when rea
+00008c60: 6469 6e67 2065 7665 6e74 7320 6569 7468  ding events eith
+00008c70: 6572 2062 7920 7573 696e 670a 7468 6520  er by using.the 
+00008c80: 6072 6561 645f 616c 6c5f 6576 656e 7473  `read_all_events
+00008c90: 2829 6020 6d65 7468 6f64 206f 7220 6279  ()` method or by
+00008ca0: 2075 7369 6e67 2061 2063 6174 6368 2d75   using a catch-u
+00008cb0: 7020 7375 6273 6372 6970 7469 6f6e 2077  p subscription w
+00008cc0: 6f75 6c64 2075 7375 616c 6c79 0a62 6520  ould usually.be 
+00008cd0: 6465 7465 726d 696e 6564 2062 7920 7468  determined by th
+00008ce0: 6520 7265 636f 7264 6564 2063 6f6d 6d69  e recorded commi
+00008cf0: 7420 706f 7369 7469 6f6e 206f 6620 7468  t position of th
+00008d00: 6520 6c61 7374 2073 7563 6365 7373 6675  e last successfu
+00008d10: 6c6c 7920 7072 6f63 6573 7365 640a 6576  lly processed.ev
+00008d20: 656e 7420 696e 2061 2064 6f77 6e73 7472  ent in a downstr
+00008d30: 6561 6d20 636f 6d70 6f6e 656e 742e 0a0a  eam component...
+00008d40: 0a0a 2323 2320 4765 7420 7374 7265 616d  ..### Get stream
+00008d50: 206d 6574 6164 6174 610a 0a54 6865 206d   metadata..The m
+00008d60: 6574 686f 6420 6067 6574 5f73 7472 6561  ethod `get_strea
+00008d70: 6d5f 6d65 7461 6461 7461 2829 6020 6765  m_metadata()` ge
+00008d80: 7473 2074 6865 206d 6574 6164 6174 6120  ts the metadata 
+00008d90: 666f 7220 6120 7374 7265 616d 2c20 616c  for a stream, al
+00008da0: 6f6e 670a 7769 7468 2074 6865 2076 6572  ong.with the ver
+00008db0: 7369 6f6e 206f 6620 7468 6520 7374 7265  sion of the stre
+00008dc0: 616d 206d 6574 6164 6174 612e 0a0a 6060  am metadata...``
+00008dd0: 6070 7974 686f 6e0a 6d65 7461 6461 7461  `python.metadata
+00008de0: 2c20 6d65 7461 6461 7461 5f76 6572 7369  , metadata_versi
+00008df0: 6f6e 203d 2063 6c69 656e 742e 6765 745f  on = client.get_
+00008e00: 7374 7265 616d 5f6d 6574 6164 6174 6128  stream_metadata(
+00008e10: 7374 7265 616d 5f6e 616d 653d 7374 7265  stream_name=stre
+00008e20: 616d 5f6e 616d 6531 290a 6060 600a 0a54  am_name1).```..T
+00008e30: 6865 2072 6574 7572 6e65 6420 606d 6574  he returned `met
+00008e40: 6164 6174 6160 2076 616c 7565 2069 7320  adata` value is 
+00008e50: 6120 5079 7468 6f6e 2060 6469 6374 602e  a Python `dict`.
+00008e60: 2054 6865 2072 6574 7572 6e65 6420 606d   The returned `m
+00008e70: 6574 6164 6174 615f 7665 7273 696f 6e60  etadata_version`
+00008e80: 0a76 616c 7565 2069 7320 6569 7468 6572  .value is either
+00008e90: 2061 6e20 6069 6e74 602c 206f 7220 604e   an `int`, or `N
+00008ea0: 6f6e 6560 2069 6620 7468 6520 7374 7265  one` if the stre
+00008eb0: 616d 2064 6f65 7320 6e6f 7420 6578 6973  am does not exis
+00008ec0: 742e 2054 6865 7365 2076 616c 7565 7320  t. These values 
+00008ed0: 6361 6e0a 6265 2070 6173 7365 6420 696e  can.be passed in
+00008ee0: 746f 2060 7365 745f 7374 7265 616d 5f6d  to `set_stream_m
+00008ef0: 6574 6164 6174 6128 2960 2e0a 0a0a 2323  etadata()`....##
+00008f00: 2320 5365 7420 7374 7265 616d 206d 6574  # Set stream met
+00008f10: 6164 6174 610a 0a54 6865 206d 6574 686f  adata..The metho
+00008f20: 6420 6073 6574 5f73 7472 6561 6d5f 6d65  d `set_stream_me
+00008f30: 7461 6461 7461 2829 6020 7365 7473 2074  tadata()` sets t
+00008f40: 6865 206d 6574 6164 6174 6120 666f 7220  he metadata for 
+00008f50: 6120 7374 7265 616d 2c20 616c 6f6e 670a  a stream, along.
+00008f60: 7769 7468 2074 6865 2076 6572 7369 6f6e  with the version
+00008f70: 206f 6620 7468 6520 7374 7265 616d 206d   of the stream m
+00008f80: 6574 6164 6174 612e 0a0a 6060 6070 7974  etadata...```pyt
+00008f90: 686f 6e0a 6d65 7461 6461 7461 5b22 666f  hon.metadata["fo
+00008fa0: 6f22 5d20 3d20 2262 6172 220a 0a63 6c69  o"] = "bar"..cli
+00008fb0: 656e 742e 7365 745f 7374 7265 616d 5f6d  ent.set_stream_m
+00008fc0: 6574 6164 6174 6128 0a20 2020 2073 7472  etadata(.    str
+00008fd0: 6561 6d5f 6e61 6d65 3d73 7472 6561 6d5f  eam_name=stream_
+00008fe0: 6e61 6d65 312c 0a20 2020 206d 6574 6164  name1,.    metad
+00008ff0: 6174 613d 6d65 7461 6461 7461 2c0a 2020  ata=metadata,.  
+00009000: 2020 6578 7065 6374 6564 5f70 6f73 6974    expected_posit
+00009010: 696f 6e3d 6d65 7461 6461 7461 5f76 6572  ion=metadata_ver
+00009020: 7369 6f6e 2c0a 290a 6060 600a 0a54 6865  sion,.).```..The
+00009030: 2060 6578 7065 6374 6564 5f70 6f73 6974   `expected_posit
+00009040: 696f 6e60 2061 7267 756d 656e 7420 7368  ion` argument sh
+00009050: 6f75 6c64 2062 6520 7468 6520 6375 7272  ould be the curr
+00009060: 656e 7420 7665 7273 696f 6e20 6f66 2074  ent version of t
+00009070: 6865 2073 7472 6561 6d20 6d65 7461 6461  he stream metada
+00009080: 7461 2e0a 0a50 6c65 6173 6520 7265 6665  ta...Please refe
+00009090: 7220 746f 2074 6865 2045 7665 6e74 5374  r to the EventSt
+000090a0: 6f72 6544 4220 646f 6375 6d65 6e74 6174  oreDB documentat
+000090b0: 696f 6e20 666f 7220 6d6f 7265 2069 6e66  ion for more inf
+000090c0: 6f72 6d61 7469 6f6e 2061 626f 7574 2073  ormation about s
+000090d0: 7472 6561 6d0a 6d65 7461 6461 7461 2e0a  tream.metadata..
+000090e0: 0a23 2323 2044 656c 6574 6520 7374 7265  .### Delete stre
+000090f0: 616d 0a0a 5468 6520 6d65 7468 6f64 2060  am..The method `
+00009100: 6465 6c65 7465 5f73 7472 6561 6d28 2960  delete_stream()`
+00009110: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+00009120: 2264 656c 6574 6522 2061 2073 7472 6561  "delete" a strea
+00009130: 6d2e 0a0a 6060 6070 7974 686f 6e0a 636f  m...```python.co
+00009140: 6d6d 6974 5f70 6f73 6974 696f 6e20 3d20  mmit_position = 
+00009150: 636c 6965 6e74 2e64 656c 6574 655f 7374  client.delete_st
+00009160: 7265 616d 2873 7472 6561 6d5f 6e61 6d65  ream(stream_name
+00009170: 3d73 7472 6561 6d5f 6e61 6d65 312c 2065  =stream_name1, e
+00009180: 7870 6563 7465 645f 706f 7369 7469 6f6e  xpected_position
+00009190: 3d32 290a 6060 600a 0a41 6674 6572 2064  =2).```..After d
+000091a0: 656c 6574 696e 6720 6120 7374 7265 616d  eleting a stream
+000091b0: 2c20 6974 2773 2073 7469 6c6c 2070 6f73  , it's still pos
+000091c0: 7369 626c 6520 746f 2061 7070 656e 6420  sible to append 
+000091d0: 6e65 7720 6576 656e 7473 2e20 5265 6164  new events. Read
+000091e0: 696e 6720 6672 6f6d 2061 0a64 656c 6574  ing from a.delet
+000091f0: 6564 2073 7472 6561 6d20 7769 6c6c 2072  ed stream will r
+00009200: 6574 7572 6e20 6f6e 6c79 2065 7665 6e74  eturn only event
+00009210: 7320 7468 6174 2068 6176 6520 6265 656e  s that have been
+00009220: 2061 7070 656e 6465 6420 6166 7465 7220   appended after 
+00009230: 6974 2077 6173 0a64 656c 6574 6564 2e0a  it was.deleted..
+00009240: 0a23 2323 2054 6f6d 6273 746f 6e65 2073  .### Tombstone s
+00009250: 7472 6561 6d0a 0a54 6865 206d 6574 686f  tream..The metho
+00009260: 6420 6074 6f6d 6273 746f 6e65 5f73 7472  d `tombstone_str
+00009270: 6561 6d28 2960 2063 616e 2062 6520 7573  eam()` can be us
+00009280: 6564 2074 6f20 2274 6f6d 6273 746f 6e65  ed to "tombstone
+00009290: 2220 6120 7374 7265 616d 2e0a 0a60 6060  " a stream...```
+000092a0: 7079 7468 6f6e 0a63 6f6d 6d69 745f 706f  python.commit_po
+000092b0: 7369 7469 6f6e 203d 2063 6c69 656e 742e  sition = client.
+000092c0: 746f 6d62 7374 6f6e 655f 7374 7265 616d  tombstone_stream
+000092d0: 2873 7472 6561 6d5f 6e61 6d65 3d73 7472  (stream_name=str
+000092e0: 6561 6d5f 6e61 6d65 312c 2065 7870 6563  eam_name1, expec
+000092f0: 7465 645f 706f 7369 7469 6f6e 3d32 290a  ted_position=2).
+00009300: 6060 600a 0a41 6674 6572 2074 6f6d 6273  ```..After tombs
+00009310: 746f 6e69 6e67 2061 2073 7472 6561 6d2c  toning a stream,
+00009320: 2069 7427 7320 6e6f 7420 706f 7373 6962   it's not possib
+00009330: 6c65 2074 6f20 6170 7065 6e64 206e 6577  le to append new
+00009340: 2065 7665 6e74 732e 0a0a 0a23 2320 4361   events....## Ca
+00009350: 7463 682d 7570 2073 7562 7363 7269 7074  tch-up subscript
+00009360: 696f 6e73 0a0a 4120 2263 6174 6368 2d75  ions..A "catch-u
+00009370: 7020 7375 6273 6372 6970 7469 6f6e 2220  p subscription" 
+00009380: 6361 6e20 6265 2075 7365 6420 746f 2072  can be used to r
+00009390: 6563 6569 7665 2061 6c72 6561 6479 2072  eceive already r
+000093a0: 6563 6f72 6465 6420 6576 656e 7473 2c20  ecorded events, 
+000093b0: 6275 740a 6974 2077 696c 6c20 616c 736f  but.it will also
+000093c0: 2072 6574 7572 6e20 6576 656e 7473 2074   return events t
+000093d0: 6861 7420 6172 6520 7265 636f 7264 6564  hat are recorded
+000093e0: 2061 6674 6572 2074 6865 2073 7562 7363   after the subsc
+000093f0: 7269 7074 696f 6e20 7761 7320 7374 6172  ription was star
+00009400: 7465 642e 0a0a 5468 6520 6d65 7468 6f64  ted...The method
+00009410: 2060 7375 6273 6372 6962 655f 616c 6c5f   `subscribe_all_
+00009420: 6576 656e 7473 2829 6020 7374 6172 7473  events()` starts
+00009430: 2061 2063 6174 6368 2d75 7020 7375 6273   a catch-up subs
+00009440: 6372 6970 7469 6f6e 2074 6f20 7265 6365  cription to rece
+00009450: 6976 6520 616c 6c0a 6576 656e 7473 2069  ive all.events i
+00009460: 6e20 7468 6520 6461 7461 6261 7365 2e20  n the database. 
+00009470: 5468 6520 6d65 7468 6f64 2060 7375 6273  The method `subs
+00009480: 6372 6962 655f 7374 7265 616d 5f65 7665  cribe_stream_eve
+00009490: 6e74 7328 2960 2073 7461 7274 7320 6120  nts()` starts a 
+000094a0: 6361 7463 682d 7570 0a73 7562 7363 7269  catch-up.subscri
+000094b0: 7074 696f 6e20 746f 2072 6563 6569 7665  ption to receive
+000094c0: 2065 7665 6e74 7320 6672 6f6d 2061 2073   events from a s
+000094d0: 7065 6369 6669 6320 7374 7265 616d 2e0a  pecific stream..
+000094e0: 0a43 6174 6368 2d75 7020 7375 6273 6372  .Catch-up subscr
+000094f0: 6970 7469 6f6e 7320 6172 6520 7369 6d70  iptions are simp
+00009500: 6c79 2061 2073 7472 6561 6d69 6e67 2067  ly a streaming g
+00009510: 5250 4320 6361 6c6c 2077 6869 6368 2069  RPC call which i
+00009520: 730a 6b65 7074 206f 7065 6e20 6279 2074  s.kept open by t
+00009530: 6865 2073 6572 7665 722c 2077 6974 6820  he server, with 
+00009540: 6e65 776c 7920 7265 636f 7264 6564 2065  newly recorded e
+00009550: 7665 6e74 7320 7365 6e74 2074 6f20 7468  vents sent to th
+00009560: 6520 636c 6965 6e74 0a61 7320 7468 6520  e client.as the 
+00009570: 636c 6965 6e74 2069 7465 7261 7465 7320  client iterates 
+00009580: 6f76 6572 2074 6865 2073 7562 7363 7269  over the subscri
+00009590: 7074 696f 6e2e 0a0a 4d61 6e79 2063 6174  ption...Many cat
+000095a0: 6368 2d75 7020 7375 6273 6372 6970 7469  ch-up subscripti
+000095b0: 6f6e 7320 6361 6e20 6265 2063 7265 6174  ons can be creat
+000095c0: 6564 2c20 636f 6e63 7572 7265 6e74 6c79  ed, concurrently
+000095d0: 206f 7220 7375 6363 6573 7369 7665 6c79   or successively
+000095e0: 2c20 616e 6420 616c 6c0a 7769 6c6c 2072  , and all.will r
+000095f0: 6563 6569 7665 2061 6c6c 2074 6865 2072  eceive all the r
+00009600: 6563 6f72 6465 6420 6576 656e 7473 2074  ecorded events t
+00009610: 6865 7920 6861 7665 2062 6565 6e20 7265  hey have been re
+00009620: 7175 6573 7465 6420 746f 2072 6563 6569  quested to recei
+00009630: 7665 2e0a 0a52 6563 6569 7665 6420 7265  ve...Received re
+00009640: 636f 7264 6564 2065 7665 6e74 7320 6172  corded events ar
+00009650: 6520 696e 7374 616e 6365 7320 6f66 2074  e instances of t
+00009660: 6865 2060 5265 636f 7264 6564 4576 656e  he `RecordedEven
+00009670: 7460 2063 6c61 7373 2028 7365 6520 6265  t` class (see be
+00009680: 6c6f 7729 2e0a 5265 636f 7264 6564 2065  low)..Recorded e
+00009690: 7665 6e74 206f 626a 6563 7473 2068 6176  vent objects hav
+000096a0: 6520 6120 636f 6d6d 6974 2070 6f73 6974  e a commit posit
+000096b0: 696f 6e2c 2061 6d6f 6e73 7420 6f74 6865  ion, amonst othe
+000096c0: 7220 6174 7472 6962 7574 6573 2e0a 0a23  r attributes...#
+000096d0: 2323 2048 6f77 2074 6f20 696d 706c 656d  ## How to implem
+000096e0: 656e 7420 6578 6163 746c 792d 6f6e 6365  ent exactly-once
+000096f0: 2065 7665 6e74 2070 726f 6365 7373 696e   event processin
+00009700: 670a 0a54 6865 2063 6f6d 6d69 7420 706f  g..The commit po
+00009710: 7369 7469 6f6e 7320 6f66 2072 6563 6f72  sitions of recor
+00009720: 6465 6420 6576 656e 7473 2074 6861 7420  ded events that 
+00009730: 6172 6520 7265 6365 6976 6564 2061 6e64  are received and
+00009740: 2070 726f 6365 7373 6564 2062 7920 610a   processed by a.
+00009750: 646f 776e 7374 7265 616d 2063 6f6d 706f  downstream compo
+00009760: 6e65 6e74 2061 7265 2075 7365 6675 6c6c  nent are usefull
+00009770: 7920 7265 636f 7264 6564 2062 7920 7468  y recorded by th
+00009780: 6520 646f 776e 7374 7265 616d 2063 6f6d  e downstream com
+00009790: 706f 6e65 6e74 2073 6f20 7468 6174 0a74  ponent so that.t
+000097a0: 6865 2063 6f6d 6d69 7420 706f 7369 7469  he commit positi
+000097b0: 6f6e 206f 6620 6c61 7374 2070 726f 6365  on of last proce
+000097c0: 7373 6564 2065 7665 6e74 2063 616e 2062  ssed event can b
+000097d0: 6520 6465 7465 726d 696e 6564 2e0a 0a54  e determined...T
+000097e0: 6865 206c 6173 7420 7265 636f 7264 6564  he last recorded
+000097f0: 2063 6f6d 6d69 7420 706f 7369 7469 6f6e   commit position
+00009800: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+00009810: 7370 6563 6966 7920 7468 6520 636f 6d6d  specify the comm
+00009820: 6974 2070 6f73 6974 696f 6e20 6672 6f6d  it position from
+00009830: 2077 6869 6368 0a74 6f20 7375 6273 6372   which.to subscr
+00009840: 6962 6520 7768 656e 2070 726f 6365 7373  ibe when process
+00009850: 696e 6720 6973 2072 6573 756d 6564 2e20  ing is resumed. 
+00009860: 5369 6e63 6520 7468 6973 2063 6f6d 6d69  Since this commi
+00009870: 7420 706f 7369 7469 6f6e 2077 696c 6c20  t position will 
+00009880: 7265 7072 6573 656e 7420 7468 650a 706f  represent the.po
+00009890: 7369 7469 6f6e 206f 6620 7468 6520 6c61  sition of the la
+000098a0: 7374 2073 7563 6365 7373 6675 6c6c 7920  st successfully 
+000098b0: 7072 6f63 6573 7365 6420 6576 656e 7420  processed event 
+000098c0: 696e 2061 2064 6f77 6e73 7472 6561 6d20  in a downstream 
+000098d0: 636f 6d70 6f6e 656e 742c 2073 6f20 6974  component, so it
+000098e0: 0a77 696c 6c20 6265 2075 7375 616c 2074  .will be usual t
+000098f0: 6f20 7761 6e74 2074 6865 206e 6578 7420  o want the next 
+00009900: 6576 656e 7420 6166 7465 7220 7468 6973  event after this
+00009910: 2070 6f73 6974 696f 6e2c 2062 6563 6175   position, becau
+00009920: 7365 2074 6861 7420 6973 2074 6865 206e  se that is the n
+00009930: 6578 740a 6576 656e 7420 7468 6174 2068  ext.event that h
+00009940: 6173 206e 6f74 2079 6574 2062 6565 6e20  as not yet been 
+00009950: 7072 6f63 6573 7365 642e 2046 6f72 2074  processed. For t
+00009960: 6869 7320 7265 6173 6f6e 2c20 7768 656e  his reason, when
+00009970: 2073 7562 7363 7269 6269 6e67 2066 6f72   subscribing for
+00009980: 2065 7665 6e74 730a 6672 6f6d 2061 2073   events.from a s
+00009990: 7065 6369 6669 6320 636f 6d6d 6974 2070  pecific commit p
+000099a0: 6f73 6974 696f 6e20 7573 696e 6720 6120  osition using a 
+000099b0: 6361 7463 682d 7570 2073 7562 7363 7269  catch-up subscri
+000099c0: 7074 696f 6e20 696e 2045 7665 6e74 5374  ption in EventSt
+000099d0: 6f72 6544 422c 2074 6865 0a72 6563 6f72  oreDB, the.recor
+000099e0: 6465 6420 6576 656e 7420 6174 2074 6865  ded event at the
+000099f0: 2073 7065 6369 6669 6564 2063 6f6d 6d69   specified commi
+00009a00: 7420 706f 7369 7469 6f6e 2077 696c 6c20  t position will 
+00009a10: 4e4f 5420 6265 2069 6e63 6c75 6465 6420  NOT be included 
+00009a20: 696e 2074 6865 2073 6571 7565 6e63 650a  in the sequence.
+00009a30: 6f66 2072 6563 6f72 6465 6420 6576 656e  of recorded even
+00009a40: 7473 2074 6861 7420 6172 6520 7265 6365  ts that are rece
+00009a50: 6976 6564 2e0a 0a54 6f20 6163 636f 6d70  ived...To accomp
+00009a60: 6c69 7368 2022 6578 6163 746c 792d 6f6e  lish "exactly-on
+00009a70: 6365 2220 7072 6f63 6573 7369 6e67 206f  ce" processing o
+00009a80: 6620 7265 636f 7264 6564 2065 7665 6e74  f recorded event
+00009a90: 7320 696e 2061 2064 6f77 6e73 7472 6561  s in a downstrea
+00009aa0: 6d0a 636f 6d70 6f6e 656e 7420 7768 656e  m.component when
+00009ab0: 2075 7369 6e67 2061 2063 6174 6368 2d75   using a catch-u
+00009ac0: 7020 7375 6273 6372 6970 7469 6f6e 2c20  p subscription, 
+00009ad0: 7468 6520 636f 6d6d 6974 2070 6f73 6974  the commit posit
+00009ae0: 696f 6e20 6f66 2061 2072 6563 6f72 6465  ion of a recorde
+00009af0: 640a 6576 656e 7420 7368 6f75 6c64 2062  d.event should b
+00009b00: 6520 7265 636f 7264 6564 2061 746f 6d69  e recorded atomi
+00009b10: 6361 6c6c 7920 616e 6420 756e 6971 7565  cally and unique
+00009b20: 6c79 2061 6c6f 6e67 2077 6974 6820 7468  ly along with th
+00009b30: 6520 7265 7375 6c74 206f 6620 7072 6f63  e result of proc
+00009b40: 6573 7369 6e67 0a72 6563 6f72 6465 6420  essing.recorded 
+00009b50: 6576 656e 7473 2c20 666f 7220 6578 616d  events, for exam
+00009b60: 706c 6520 696e 2074 6865 2073 616d 6520  ple in the same 
+00009b70: 6461 7461 6261 7365 2061 7320 6d61 7465  database as mate
+00009b80: 7269 616c 6973 6564 2076 6965 7773 2077  rialised views w
+00009b90: 6865 6e0a 696d 706c 656d 656e 7469 6e67  hen.implementing
+00009ba0: 2065 7665 6e74 7561 6c6c 792d 636f 6e73   eventually-cons
+00009bb0: 6973 7465 6e74 2043 5152 532c 206f 7220  istent CQRS, or 
+00009bc0: 696e 2074 6865 2073 616d 6520 6461 7461  in the same data
+00009bd0: 6261 7365 2061 7320 6120 646f 776e 7374  base as a downst
+00009be0: 7265 616d 0a61 6e61 6c79 7469 6373 206f  ream.analytics o
+00009bf0: 7220 7265 706f 7274 696e 6720 6f72 2061  r reporting or a
+00009c00: 7263 6869 7669 6e67 2061 7070 6c69 6361  rchiving applica
+00009c10: 7469 6f6e 2e20 4279 2072 6563 6f72 6469  tion. By recordi
+00009c20: 6e67 2074 6865 2063 6f6d 6d69 7420 706f  ng the commit po
+00009c30: 7369 7469 6f6e 0a6f 6620 7265 636f 7264  sition.of record
+00009c40: 6564 2065 7665 6e74 7320 6174 6f6d 6963  ed events atomic
+00009c50: 616c 6c79 2077 6974 6820 7468 6520 6e65  ally with the ne
+00009c60: 7720 7374 6174 6520 7468 6174 2072 6573  w state that res
+00009c70: 756c 7473 2066 726f 6d20 7072 6f63 6573  ults from proces
+00009c80: 7369 6e67 0a72 6563 6f72 6465 6420 6576  sing.recorded ev
+00009c90: 656e 7473 2c20 2264 7561 6c20 7772 6974  ents, "dual writ
+00009ca0: 696e 6722 2069 6e20 7468 6520 636f 6e73  ing" in the cons
+00009cb0: 756d 7074 696f 6e20 6f66 2072 6563 6f72  umption of recor
+00009cc0: 6465 6420 6576 656e 7473 2063 616e 2062  ded events can b
+00009cd0: 650a 6176 6f69 6465 642e 2042 7920 616c  e.avoided. By al
+00009ce0: 736f 2072 6563 6f72 6469 6e67 2074 6865  so recording the
+00009cf0: 2063 6f6d 6d69 7420 706f 7369 7469 6f6e   commit position
+00009d00: 2075 6e69 7175 656c 792c 2074 6865 206e   uniquely, the n
+00009d10: 6577 2073 7461 7465 2063 616e 6e6f 7420  ew state cannot 
+00009d20: 6265 0a72 6563 6f72 6465 6420 7477 6963  be.recorded twic
+00009d30: 652c 2061 6e64 2068 656e 6365 2074 6865  e, and hence the
+00009d40: 2072 6563 6f72 6465 6420 7374 6174 6520   recorded state 
+00009d50: 6f66 2074 6865 2064 6f77 6e73 7472 6561  of the downstrea
+00009d60: 6d20 636f 6d70 6f6e 656e 7420 7769 6c6c  m component will
+00009d70: 2062 650a 7570 6461 7465 6420 6f6e 6c79   be.updated only
+00009d80: 206f 6e63 6520 666f 7220 616e 7920 7265   once for any re
+00009d90: 636f 7264 6564 2065 7665 6e74 2e20 4279  corded event. By
+00009da0: 2075 7369 6e67 2074 6865 2067 7265 6174   using the great
+00009db0: 6573 7420 7265 636f 7264 6564 2063 6f6d  est recorded com
+00009dc0: 6d69 740a 706f 7369 7469 6f6e 2074 6f20  mit.position to 
+00009dd0: 7265 7375 6d65 2061 2063 6174 6368 2d75  resume a catch-u
+00009de0: 7020 7375 6273 6372 6970 7469 6f6e 2c20  p subscription, 
+00009df0: 616c 6c20 7265 636f 7264 6564 2065 7665  all recorded eve
+00009e00: 6e74 7320 7769 6c6c 2065 7665 6e74 7561  nts will eventua
+00009e10: 6c6c 790a 6265 2070 726f 6365 7373 6564  lly.be processed
+00009e20: 2e20 5468 6520 636f 6d62 696e 6174 696f  . The combinatio
+00009e30: 6e20 6f66 2074 6865 2022 6174 2d6d 6f73  n of the "at-mos
+00009e40: 742d 6f6e 6365 2220 636f 6e64 6974 696f  t-once" conditio
+00009e50: 6e20 616e 6420 7468 6520 2261 742d 6c65  n and the "at-le
+00009e60: 6173 742d 6f6e 6365 220a 636f 6e64 6974  ast-once".condit
+00009e70: 696f 6e20 6769 7665 7320 7468 6520 2265  ion gives the "e
+00009e80: 7861 6374 6c79 2d6f 6e63 6522 2063 6f6e  xactly-once" con
+00009e90: 6469 7469 6f6e 2e0a 0a54 6865 2064 616e  dition...The dan
+00009ea0: 6765 7220 7769 7468 2022 6475 616c 2077  ger with "dual w
+00009eb0: 7269 7469 6e67 2220 696e 2074 6865 2063  riting" in the c
+00009ec0: 6f6e 7375 6d70 7469 6f6e 206f 6620 7265  onsumption of re
+00009ed0: 636f 7264 6564 2065 7665 6e74 7320 6973  corded events is
+00009ee0: 2074 6861 7420 6966 2061 0a72 6563 6f72   that if a.recor
+00009ef0: 6465 6420 6576 656e 7420 6973 2073 7563  ded event is suc
+00009f00: 6365 7373 6675 6c6c 7920 7072 6f63 6573  cessfully proces
+00009f10: 7365 6420 616e 6420 6e65 7720 7374 6174  sed and new stat
+00009f20: 6520 7265 636f 7264 6564 2061 746f 6d69  e recorded atomi
+00009f30: 6361 6c6c 7920 696e 206f 6e65 0a74 7261  cally in one.tra
+00009f40: 6e73 6163 7469 6f6e 2077 6974 6820 7468  nsaction with th
+00009f50: 6520 636f 6d6d 6974 2070 6f73 6974 696f  e commit positio
+00009f60: 6e20 7265 636f 7264 6564 2069 6e20 6120  n recorded in a 
+00009f70: 7365 7061 7261 7465 2074 7261 6e73 6163  separate transac
+00009f80: 7469 6f6e 2c20 6f6e 6520 6d61 790a 6861  tion, one may.ha
+00009f90: 7070 656e 2061 6e64 206e 6f74 2074 6865  ppen and not the
+00009fa0: 206f 7468 6572 2e20 4966 2074 6865 206e   other. If the n
+00009fb0: 6577 2073 7461 7465 2069 7320 7265 636f  ew state is reco
+00009fc0: 7264 6564 2062 7574 2074 6865 2070 6f73  rded but the pos
+00009fd0: 6974 696f 6e20 6973 206c 6f73 742c 0a61  ition is lost,.a
+00009fe0: 6e64 2074 6865 6e20 7468 6520 7072 6f63  nd then the proc
+00009ff0: 6573 7369 6e67 2069 7320 7374 6f70 7065  essing is stoppe
+0000a000: 6420 616e 6420 7265 7375 6d65 642c 2074  d and resumed, t
+0000a010: 6865 2072 6563 6f72 6465 6420 6576 656e  he recorded even
+0000a020: 7420 6d61 7920 6265 2070 726f 6365 7373  t may be process
+0000a030: 6564 0a74 7769 6365 2e20 4f6e 2074 6865  ed.twice. On the
+0000a040: 206f 7468 6572 2068 616e 642c 2069 6620   other hand, if 
+0000a050: 7468 6520 636f 6d6d 6974 2070 6f73 6974  the commit posit
+0000a060: 696f 6e20 6973 2072 6563 6f72 6465 6420  ion is recorded 
+0000a070: 6275 7420 7468 6520 6e65 7720 7374 6174  but the new stat
+0000a080: 6520 6973 0a6c 6f73 742c 2074 6865 2072  e is.lost, the r
+0000a090: 6563 6f72 6465 6420 6576 656e 7420 6d61  ecorded event ma
+0000a0a0: 7920 6566 6665 6374 6976 656c 7920 6e6f  y effectively no
+0000a0b0: 7420 6265 2070 726f 6365 7373 6564 2061  t be processed a
+0000a0c0: 7420 616c 6c2e 2042 7920 6569 7468 6572  t all. By either
+0000a0d0: 0a70 726f 6365 7373 696e 6720 616e 2065  .processing an e
+0000a0e0: 7665 6e74 206d 6f72 6520 7468 616e 206f  vent more than o
+0000a0f0: 6e63 652c 206f 7220 6279 2066 6169 6c69  nce, or by faili
+0000a100: 6e67 2074 6f20 7072 6f63 6573 7320 616e  ng to process an
+0000a110: 2065 7665 6e74 2c20 7468 6520 7265 636f   event, the reco
+0000a120: 7264 6564 0a73 7461 7465 206f 6620 7468  rded.state of th
+0000a130: 6520 646f 776e 7374 7265 616d 2063 6f6d  e downstream com
+0000a140: 706f 6e65 6e74 206d 6967 6874 2062 6520  ponent might be 
+0000a150: 696e 6163 6375 7261 7465 2c20 6f72 2070  inaccurate, or p
+0000a160: 6f73 7369 626c 7920 696e 636f 6e73 6973  ossibly inconsis
+0000a170: 7465 6e74 2c20 616e 640a 7065 7268 6170  tent, and.perhap
+0000a180: 7320 6361 7461 7374 726f 7068 6963 616c  s catastrophical
+0000a190: 6c79 2073 6f2e 2053 7563 6820 636f 6e73  ly so. Such cons
+0000a1a0: 6571 7565 6e63 6573 206d 6179 206f 7220  equences may or 
+0000a1b0: 6d61 7920 6e6f 7420 6d61 7474 6572 2069  may not matter i
+0000a1c0: 6e20 796f 7572 2073 6974 7561 7469 6f6e  n your situation
+0000a1d0: 2e0a 4275 7420 736f 6d65 7469 6d65 7320  ..But sometimes 
+0000a1e0: 696e 636f 6e73 6973 7465 6e63 6965 7320  inconsistencies 
+0000a1f0: 6d61 7920 6861 6c74 2070 726f 6365 7373  may halt process
+0000a200: 696e 6720 756e 7469 6c20 7468 6520 6973  ing until the is
+0000a210: 7375 6520 6973 2072 6573 6f6c 7665 642e  sue is resolved.
+0000a220: 2059 6f75 2063 616e 0a61 766f 6964 2022   You can.avoid "
+0000a230: 6475 616c 2077 7269 7469 6e67 2220 696e  dual writing" in
+0000a240: 2074 6865 2063 6f6e 7375 6d70 7469 6f6e   the consumption
+0000a250: 206f 6620 6576 656e 7473 2062 7920 6174   of events by at
+0000a260: 6f6d 6963 616c 6c79 2072 6563 6f72 6469  omically recordi
+0000a270: 6e67 2074 6865 2063 6f6d 6d69 740a 706f  ng the commit.po
+0000a280: 7369 7469 6f6e 206f 6620 6120 7265 636f  sition of a reco
+0000a290: 7264 6564 2065 7665 6e74 2061 6c6f 6e67  rded event along
+0000a2a0: 2077 6974 6820 7468 6520 6e65 7720 7374   with the new st
+0000a2b0: 6174 6520 7468 6174 2072 6573 756c 7473  ate that results
+0000a2c0: 2066 726f 6d20 7072 6f63 6573 7369 6e67   from processing
+0000a2d0: 2074 6861 740a 6576 656e 7420 696e 2074   that.event in t
+0000a2e0: 6865 2073 616d 6520 6174 6f6d 6963 2074  he same atomic t
+0000a2f0: 7261 6e73 6163 7469 6f6e 2e20 4279 206d  ransaction. By m
+0000a300: 616b 696e 6720 7468 6520 7265 636f 7264  aking the record
+0000a310: 696e 6720 6f66 2074 6865 2063 6f6d 6d69  ing of the commi
+0000a320: 7420 706f 7369 7469 6f6e 730a 756e 6971  t positions.uniq
+0000a330: 7565 2c20 736f 2074 6861 7420 7472 616e  ue, so that tran
+0000a340: 7361 6374 696f 6e73 2077 696c 6c20 6265  sactions will be
+0000a350: 2072 6f6c 6c65 6420 6261 636b 2077 6865   rolled back whe
+0000a360: 6e20 7468 6572 6520 6973 2061 2063 6f6e  n there is a con
+0000a370: 666c 6963 742c 2079 6f75 2077 696c 6c0a  flict, you will.
+0000a380: 7072 6576 656e 7420 7468 6520 7265 7375  prevent the resu
+0000a390: 6c74 7320 6f66 2061 6e79 2064 7570 6c69  lts of any dupli
+0000a3a0: 6361 7465 2070 726f 6365 7373 696e 6720  cate processing 
+0000a3b0: 6f66 2061 2072 6563 6f72 6465 6420 6576  of a recorded ev
+0000a3c0: 656e 7420 6265 696e 6720 636f 6d6d 6974  ent being commit
+0000a3d0: 7465 642e 0a0a 5265 636f 7264 6564 2065  ted...Recorded e
+0000a3e0: 7665 6e74 7320 7265 6365 6976 6564 2066  vents received f
+0000a3f0: 726f 6d20 6120 6361 7463 682d 7570 2073  rom a catch-up s
+0000a400: 7562 7363 7269 7074 696f 6e20 6361 6e6e  ubscription cann
+0000a410: 6f74 2062 6520 6163 6b6e 6f77 6c65 6467  ot be acknowledg
+0000a420: 6564 2062 6163 6b0a 746f 2074 6865 2045  ed back.to the E
+0000a430: 7665 6e74 5374 6f72 6544 4220 7365 7276  ventStoreDB serv
+0000a440: 6572 2e20 4163 6b6e 6f77 6c65 6467 696e  er. Acknowledgin
+0000a450: 6720 6576 656e 7473 2c20 686f 7765 7665  g events, howeve
+0000a460: 722c 2069 7320 616e 2061 7370 6563 7420  r, is an aspect 
+0000a470: 6f66 2022 7065 7273 6973 7465 6e74 0a73  of "persistent.s
+0000a480: 7562 7363 7269 7074 696f 6e73 2220 2873  ubscriptions" (s
+0000a490: 6565 2062 656c 6f77 292e 2048 6f70 696e  ee below). Hopin
+0000a4a0: 6720 746f 2072 656c 7920 6f6e 2061 636b  g to rely on ack
+0000a4b0: 6e6f 776c 6564 6769 6e67 2065 7665 6e74  nowledging event
+0000a4c0: 7320 746f 2061 6e20 7570 7374 7265 616d  s to an upstream
+0000a4d0: 0a63 6f6d 706f 6e65 6e74 2069 7320 616e  .component is an
+0000a4e0: 2065 7861 6d70 6c65 206f 6620 6475 616c   example of dual
+0000a4f0: 2077 7269 7469 6e67 2e0a 0a23 2323 2053   writing...### S
+0000a500: 7562 7363 7269 6265 2061 6c6c 2065 7665  ubscribe all eve
+0000a510: 6e74 730a 0a54 6865 6073 7562 7363 7269  nts..The`subscri
+0000a520: 6265 5f61 6c6c 5f65 7665 6e74 7328 2960  be_all_events()`
+0000a530: 206d 6574 686f 6420 6361 6e20 6265 2075   method can be u
+0000a540: 7365 6420 746f 2073 7461 7274 2061 2022  sed to start a "
+0000a550: 6361 7463 682d 7570 2220 7375 6273 6372  catch-up" subscr
+0000a560: 6970 7469 6f6e 0a74 6861 7420 6361 6e20  iption.that can 
+0000a570: 7265 7475 726e 2061 6c6c 2065 7665 6e74  return all event
+0000a580: 7320 696e 2074 6865 2064 6174 6162 6173  s in the databas
+0000a590: 652e 0a0a 5468 6973 206d 6574 686f 6420  e...This method 
+0000a5a0: 6361 6e20 6265 2075 7365 6420 6279 2061  can be used by a
+0000a5b0: 2064 6f77 6e73 7472 6561 6d20 636f 6d70   downstream comp
+0000a5c0: 6f6e 656e 740a 746f 2070 726f 6365 7373  onent.to process
+0000a5d0: 2072 6563 6f72 6465 6420 6576 656e 7473   recorded events
+0000a5e0: 2077 6974 6820 6578 6163 746c 792d 6f6e   with exactly-on
+0000a5f0: 6365 2073 656d 616e 7469 6373 2e0a 0a54  ce semantics...T
+0000a600: 6869 7320 6d65 7468 6f64 2074 616b 6573  his method takes
+0000a610: 2061 6e20 6f70 7469 6f6e 616c 2060 636f   an optional `co
+0000a620: 6d6d 6974 5f70 6f73 6974 696f 6e60 2061  mmit_position` a
+0000a630: 7267 756d 656e 742c 2077 6869 6368 2063  rgument, which c
+0000a640: 616e 2062 650a 7573 6564 2074 6f20 7370  an be.used to sp
+0000a650: 6563 6966 7920 6120 636f 6d6d 6974 2070  ecify a commit p
+0000a660: 6f73 6974 696f 6e20 6672 6f6d 2077 6869  osition from whi
+0000a670: 6368 2074 6f20 7375 6273 6372 6962 6520  ch to subscribe 
+0000a680: 666f 720a 7265 636f 7264 6564 2065 7665  for.recorded eve
+0000a690: 6e74 732e 2054 6865 2064 6566 6175 6c74  nts. The default
+0000a6a0: 2076 616c 7565 2069 7320 604e 6f6e 6560   value is `None`
+0000a6b0: 2c20 7768 6963 6820 6d65 616e 730a 7468  , which means.th
+0000a6c0: 6520 7375 6273 6372 6970 7469 6f6e 2077  e subscription w
+0000a6d0: 696c 6c20 6f70 6572 6174 6520 6672 6f6d  ill operate from
+0000a6e0: 2074 6865 2066 6972 7374 2072 6563 6f72   the first recor
+0000a6f0: 6465 6420 6576 656e 740a 696e 2074 6865  ded event.in the
+0000a700: 2064 6174 6162 6173 652e 2049 6620 6120   database. If a 
+0000a710: 636f 6d6d 6974 2070 6f73 6974 696f 6e20  commit position 
+0000a720: 6973 2067 6976 656e 2c20 6974 206d 7573  is given, it mus
+0000a730: 7420 6d61 7463 680a 616e 2061 6374 7561  t match.an actua
+0000a740: 6c6c 7920 6578 6973 7469 6e67 2063 6f6d  lly existing com
+0000a750: 6d69 7420 706f 7369 7469 6f6e 2069 6e20  mit position in 
+0000a760: 7468 6520 6461 7461 6261 7365 2e20 5468  the database. Th
+0000a770: 6520 6576 656e 7473 0a74 6861 7420 6172  e events.that ar
+0000a780: 6520 6f62 7461 696e 6564 2077 696c 6c20  e obtained will 
+0000a790: 6e6f 7420 696e 636c 7564 6520 7468 6520  not include the 
+0000a7a0: 6576 656e 7420 7265 636f 7264 6564 2061  event recorded a
+0000a7b0: 7420 7468 6174 2063 6f6d 6d69 740a 706f  t that commit.po
+0000a7c0: 7369 7469 6f6e 2e0a 0a54 6869 7320 6d65  sition...This me
+0000a7d0: 7468 6f64 2061 6c73 6f20 7461 6b65 7320  thod also takes 
+0000a7e0: 7468 7265 6520 6f74 6865 7220 6f70 7469  three other opti
+0000a7f0: 6f6e 616c 2061 7267 756d 656e 7473 2c20  onal arguments, 
+0000a800: 6066 696c 7465 725f 6578 636c 7564 6560  `filter_exclude`
+0000a810: 2c0a 6066 696c 7465 725f 696e 636c 7564  ,.`filter_includ
+0000a820: 6560 2c20 616e 6420 6074 696d 656f 7574  e`, and `timeout
+0000a830: 602e 0a0a 5468 6520 6172 6775 6d65 6e74  `...The argument
+0000a840: 2060 6669 6c74 6572 5f65 7863 6c75 6465   `filter_exclude
+0000a850: 6020 6973 2061 2073 6571 7565 6e63 6520  ` is a sequence 
+0000a860: 6f66 2072 6567 756c 6172 2065 7870 7265  of regular expre
+0000a870: 7373 696f 6e73 206d 6174 6368 696e 670a  ssions matching.
+0000a880: 7468 6520 7479 7065 2073 7472 696e 6773  the type strings
+0000a890: 206f 6620 7265 636f 7264 6564 2065 7665   of recorded eve
+0000a8a0: 6e74 7320 7468 6174 2073 686f 756c 6420  nts that should 
+0000a8b0: 6265 2065 7863 6c75 6465 642e 2042 7920  be excluded. By 
+0000a8c0: 6465 6661 756c 742c 0a74 6869 7320 6172  default,.this ar
+0000a8d0: 6775 6d65 6e74 2077 696c 6c20 6d61 7463  gument will matc
+0000a8e0: 6820 2273 7973 7465 6d20 6576 656e 7473  h "system events
+0000a8f0: 222c 2073 6f20 7468 6174 2074 6865 7920  ", so that they 
+0000a900: 7769 6c6c 206e 6f74 2062 6520 696e 636c  will not be incl
+0000a910: 7564 6564 2e0a 5468 6973 2061 7267 756d  uded..This argum
+0000a920: 656e 7420 6973 2069 676e 6f72 6564 2069  ent is ignored i
+0000a930: 6620 6066 696c 7465 725f 696e 636c 7564  f `filter_includ
+0000a940: 6560 2069 7320 7365 7420 746f 2061 206e  e` is set to a n
+0000a950: 6f6e 2d65 6d70 7479 2073 6571 7565 6e63  on-empty sequenc
+0000a960: 652e 0a0a 5468 6520 6172 6775 6d65 6e74  e...The argument
+0000a970: 2060 6669 6c74 6572 5f69 6e63 6c75 6465   `filter_include
+0000a980: 6020 6973 2061 2073 6571 7565 6e63 6520  ` is a sequence 
+0000a990: 6f66 2072 6567 756c 6172 2065 7870 7265  of regular expre
+0000a9a0: 7373 696f 6e73 0a6d 6174 6368 696e 6720  ssions.matching 
+0000a9b0: 7468 6520 7479 7065 2073 7472 696e 6773  the type strings
+0000a9c0: 206f 6620 7265 636f 7264 6564 2065 7665   of recorded eve
+0000a9d0: 6e74 7320 7468 6174 2073 686f 756c 6420  nts that should 
+0000a9e0: 6265 2069 6e63 6c75 6465 642e 2042 790a  be included. By.
+0000a9f0: 6465 6661 756c 742c 2074 6869 7320 6172  default, this ar
+0000aa00: 6775 6d65 6e74 2069 7320 616e 2065 6d70  gument is an emp
+0000aa10: 7479 2074 7570 6c65 2e20 4966 2074 6869  ty tuple. If thi
+0000aa20: 7320 6172 6775 6d65 6e74 2069 7320 7365  s argument is se
+0000aa30: 7420 746f 2061 0a6e 6f6e 2d65 6d70 7479  t to a.non-empty
+0000aa40: 2073 6571 7565 6e63 652c 2074 6865 2060   sequence, the `
+0000aa50: 6669 6c74 6572 5f65 7863 6c75 6465 6020  filter_exclude` 
+0000aa60: 6172 6775 6d65 6e74 2069 7320 6967 6e6f  argument is igno
+0000aa70: 7265 642e 0a0a 506c 6561 7365 206e 6f74  red...Please not
+0000aa80: 652c 2074 6865 2066 696c 7465 7269 6e67  e, the filtering
+0000aa90: 2068 6170 7065 6e73 206f 6e20 7468 6520   happens on the 
+0000aaa0: 4576 656e 7453 746f 7265 4442 2073 6572  EventStoreDB ser
+0000aab0: 7665 722c 2061 6e64 2074 6865 0a60 6c69  ver, and the.`li
+0000aac0: 6d69 7460 2061 7267 756d 656e 7420 6973  mit` argument is
+0000aad0: 2061 7070 6c69 6564 206f 6e20 7468 6520   applied on the 
+0000aae0: 7365 7276 6572 2061 6674 6572 2066 696c  server after fil
+0000aaf0: 7465 7269 6e67 2e20 5365 6520 6265 6c6f  tering. See belo
+0000ab00: 7720 666f 720a 6d6f 7265 2069 6e66 6f72  w for.more infor
+0000ab10: 6d61 7469 6f6e 2061 626f 7574 2066 696c  mation about fil
+0000ab20: 7465 7220 7265 6775 6c61 7220 6578 7072  ter regular expr
+0000ab30: 6573 7369 6f6e 732e 0a0a 5468 6520 6172  essions...The ar
+0000ab40: 6775 6d65 6e74 2060 7469 6d65 6f75 7460  gument `timeout`
+0000ab50: 2069 7320 6120 5079 7468 6f6e 2060 666c   is a Python `fl
+0000ab60: 6f61 7460 2077 6869 6368 2073 6574 7320  oat` which sets 
+0000ab70: 6120 6465 6164 6c69 6e65 2066 6f72 2074  a deadline for t
+0000ab80: 6865 2063 6f6d 706c 6574 696f 6e20 6f66  he completion of
+0000ab90: 0a74 6865 2067 5250 4320 6f70 6572 6174  .the gRPC operat
+0000aba0: 696f 6e2e 2054 6869 7320 7072 6f62 6162  ion. This probab
+0000abb0: 6c79 2069 736e 2774 2076 6572 7920 7573  ly isn't very us
+0000abc0: 6566 756c 2c20 6275 7420 6973 2069 6e63  eful, but is inc
+0000abd0: 6c75 6465 6420 666f 720a 636f 6d70 6c65  luded for.comple
+0000abe0: 7465 6e65 7373 2061 6e64 2063 6f6e 7369  teness and consi
+0000abf0: 7374 656e 6379 2077 6974 6820 7468 6520  stency with the 
+0000ac00: 6f74 6865 7220 6d65 7468 6f64 732e 0a0a  other methods...
+0000ac10: 5468 6973 206d 6574 686f 6420 7265 7475  This method retu
+0000ac20: 726e 7320 6120 5079 7468 6f6e 2069 7465  rns a Python ite
+0000ac30: 7261 746f 7220 7468 6174 2079 6965 6c64  rator that yield
+0000ac40: 7320 7265 636f 7264 6564 2065 7665 6e74  s recorded event
+0000ac50: 732c 2069 6e63 6c75 6469 6e67 2065 7665  s, including eve
+0000ac60: 6e74 730a 7468 6174 2061 7265 2072 6563  nts.that are rec
+0000ac70: 6f72 6465 6420 6166 7465 7220 7468 6520  orded after the 
+0000ac80: 7375 6273 6372 6970 7469 6f6e 2077 6173  subscription was
+0000ac90: 2063 7265 6174 6564 2e20 4974 6572 6174   created. Iterat
+0000aca0: 696e 6720 6f76 6572 2074 6869 7320 6f62  ing over this ob
+0000acb0: 6a65 6374 2077 696c 6c0a 7468 6572 6566  ject will.theref
+0000acc0: 6f72 6520 6e6f 7420 7374 6f70 2c20 756e  ore not stop, un
+0000acd0: 6c65 7373 2074 6865 2063 6f6e 6e65 6374  less the connect
+0000ace0: 696f 6e20 746f 2074 6865 2064 6174 6162  ion to the datab
+0000acf0: 6173 6520 6973 206c 6f73 742e 2054 6865  ase is lost. The
+0000ad00: 2063 6f6e 6e65 6374 696f 6e20 7769 6c6c   connection will
+0000ad10: 0a62 6520 636c 6f73 6564 2077 6865 6e20  .be closed when 
+0000ad20: 7468 6520 6974 6572 6174 6f72 206f 626a  the iterator obj
+0000ad30: 6563 7420 6973 2064 656c 6574 6564 2066  ect is deleted f
+0000ad40: 726f 6d20 6d65 6d6f 7279 2c20 7768 6963  rom memory, whic
+0000ad50: 6820 7769 6c6c 2068 6170 7065 6e20 7768  h will happen wh
+0000ad60: 656e 2074 6865 0a69 7465 7261 746f 7220  en the.iterator 
+0000ad70: 6f62 6a65 6374 2067 6f65 7320 6f75 7420  object goes out 
+0000ad80: 6f66 2073 636f 7065 206f 7220 6973 2065  of scope or is e
+0000ad90: 7870 6c69 6369 746c 7920 6465 6c65 7465  xplicitly delete
+0000ada0: 6420 2873 6565 2062 656c 6f77 292e 2054  d (see below). T
+0000adb0: 6865 2063 6f6e 6e65 6374 696f 6e0a 6d61  he connection.ma
+0000adc0: 7920 616c 736f 2062 6520 636c 6f73 6564  y also be closed
+0000add0: 2062 7920 7468 6520 7365 7276 6572 2e0a   by the server..
+0000ade0: 0a54 6865 2073 7562 7363 7269 7074 696f  .The subscriptio
+0000adf0: 6e20 6f62 6a65 6374 2063 616e 2062 6520  n object can be 
+0000ae00: 7573 6564 2064 6972 6563 746c 792c 2062  used directly, b
+0000ae10: 7574 2069 7420 6d69 6768 7420 6265 2075  ut it might be u
+0000ae20: 7365 6420 7769 7468 696e 2061 2074 6872  sed within a thr
+0000ae30: 6561 6465 640a 6c6f 6f70 2064 6564 6963  eaded.loop dedic
+0000ae40: 6174 6564 2074 6f20 7265 6365 6976 696e  ated to receivin
+0000ae50: 6720 6576 656e 7473 2074 6861 7420 6361  g events that ca
+0000ae60: 6e20 6265 2073 746f 7070 6564 2069 6e20  n be stopped in 
+0000ae70: 6120 636f 6e74 726f 6c6c 6564 2077 6179  a controlled way
+0000ae80: 2c20 7769 7468 0a72 6563 6f72 6465 6420  , with.recorded 
+0000ae90: 6576 656e 7473 2070 7574 206f 6e20 6120  events put on a 
+0000aea0: 7175 6575 6520 666f 7220 7072 6f63 6573  queue for proces
+0000aeb0: 7369 6e67 2069 6e20 6120 6469 6666 6572  sing in a differ
+0000aec0: 656e 7420 7468 7265 6164 2e20 5468 6973  ent thread. This
+0000aed0: 2070 6163 6b61 6765 0a64 6f65 736e 2774   package.doesn't
+0000aee0: 2070 726f 7669 6465 2073 7563 6820 6120   provide such a 
+0000aef0: 7468 7265 6164 6564 206f 7220 7175 6575  threaded or queu
+0000af00: 696e 6720 6f62 6a65 6374 2063 6c61 7373  ing object class
+0000af10: 2e20 4a75 7374 206d 616b 6520 7375 7265  . Just make sure
+0000af20: 2074 6f20 7265 636f 6e73 7472 7563 740a   to reconstruct.
+0000af30: 7468 6520 7375 6273 6372 6970 7469 6f6e  the subscription
+0000af40: 2028 616e 6420 7468 6520 7175 6575 6529   (and the queue)
+0000af50: 2075 7369 6e67 2074 6865 206c 6173 7420   using the last 
+0000af60: 7265 636f 7264 6564 2063 6f6d 6d69 7420  recorded commit 
+0000af70: 706f 7369 7469 6f6e 2077 6865 6e20 7265  position when re
+0000af80: 7375 6d69 6e67 0a74 6865 2073 7562 7363  suming.the subsc
+0000af90: 7269 7074 696f 6e20 6166 7465 7220 616e  ription after an
+0000afa0: 2065 7272 6f72 2c20 746f 2062 6520 7375   error, to be su
+0000afb0: 7265 2061 6c6c 2065 7665 6e74 7320 6172  re all events ar
+0000afc0: 6520 7072 6f63 6573 7365 6420 6f6e 6365  e processed once
+0000afd0: 2e0a 0a54 6865 2065 7861 6d70 6c65 2062  ...The example b
+0000afe0: 656c 6f77 2073 686f 7773 2068 6f77 2074  elow shows how t
+0000aff0: 6f20 7375 6273 6372 6962 6520 746f 2072  o subscribe to r
+0000b000: 6563 6569 7665 2061 6c6c 2072 6563 6f72  eceive all recor
+0000b010: 6465 640a 6576 656e 7473 2066 726f 6d20  ded.events from 
+0000b020: 7468 6520 7374 6172 742c 2061 6e64 2074  the start, and t
+0000b030: 6865 6e20 7265 7375 6d69 6e67 2066 726f  hen resuming fro
+0000b040: 6d20 6120 7370 6563 6966 6963 2063 6f6d  m a specific com
+0000b050: 6d69 7420 706f 7369 7469 6f6e 2e0a 5468  mit position..Th
+0000b060: 7265 6520 616c 7265 6164 792d 7265 636f  ree already-reco
+0000b070: 7264 6564 2065 7665 6e74 7320 6172 6520  rded events are 
+0000b080: 7265 6365 6976 6564 2c20 616e 6420 7468  received, and th
+0000b090: 656e 2074 6872 6565 206e 6577 2065 7665  en three new eve
+0000b0a0: 6e74 7320 6172 650a 7265 636f 7264 6564  nts are.recorded
+0000b0b0: 2c20 7768 6963 6820 6172 6520 7468 656e  , which are then
+0000b0c0: 2072 6563 6569 7665 6420 7669 6120 7468   received via th
+0000b0d0: 6520 7375 6273 6372 6970 7469 6f6e 2e0a  e subscription..
+0000b0e0: 0a60 6060 7079 7468 6f6e 0a0a 2320 4170  .```python..# Ap
+0000b0f0: 7065 6e64 2061 6e20 6576 656e 7420 746f  pend an event to
+0000b100: 2061 206e 6577 2073 7472 6561 6d2e 0a73   a new stream..s
+0000b110: 7472 6561 6d5f 6e61 6d65 3220 3d20 7374  tream_name2 = st
+0000b120: 7228 7575 6964 3428 2929 0a65 7665 6e74  r(uuid4()).event
+0000b130: 3420 3d20 4e65 7745 7665 6e74 2874 7970  4 = NewEvent(typ
+0000b140: 653d 274f 7264 6572 4372 6561 7465 6427  e='OrderCreated'
+0000b150: 2c20 6461 7461 3d62 2764 6174 6134 2729  , data=b'data4')
+0000b160: 0a63 6c69 656e 742e 6170 7065 6e64 5f65  .client.append_e
+0000b170: 7665 6e74 7328 0a20 2020 2073 7472 6561  vents(.    strea
+0000b180: 6d5f 6e61 6d65 3d73 7472 6561 6d5f 6e61  m_name=stream_na
+0000b190: 6d65 322c 0a20 2020 2065 7870 6563 7465  me2,.    expecte
+0000b1a0: 645f 706f 7369 7469 6f6e 3d4e 6f6e 652c  d_position=None,
+0000b1b0: 0a20 2020 2065 7665 6e74 733d 5b65 7665  .    events=[eve
+0000b1c0: 6e74 345d 2c0a 290a 0a23 2053 7562 7363  nt4],.)..# Subsc
+0000b1d0: 7269 6265 2066 726f 6d20 7468 6520 6669  ribe from the fi
+0000b1e0: 7273 7420 7265 636f 7264 6564 2065 7665  rst recorded eve
+0000b1f0: 6e74 2069 6e20 7468 6520 6461 7461 6261  nt in the databa
+0000b200: 7365 2e0a 7375 6273 6372 6970 7469 6f6e  se..subscription
+0000b210: 203d 2063 6c69 656e 742e 7375 6273 6372   = client.subscr
+0000b220: 6962 655f 616c 6c5f 6576 656e 7473 2829  ibe_all_events()
+0000b230: 0a72 6563 6569 7665 645f 6576 656e 7473  .received_events
+0000b240: 203d 205b 5d0a 0a23 2050 726f 6365 7373   = []..# Process
+0000b250: 2065 7665 6e74 7320 7265 6365 6976 6564   events received
+0000b260: 2066 726f 6d20 7468 6520 6361 7463 682d   from the catch-
+0000b270: 7570 2073 7562 7363 7269 7074 696f 6e2e  up subscription.
+0000b280: 0a66 6f72 2065 7665 6e74 2069 6e20 7375  .for event in su
+0000b290: 6273 6372 6970 7469 6f6e 3a0a 2020 2020  bscription:.    
+0000b2a0: 6c61 7374 5f63 6f6d 6d69 745f 706f 7369  last_commit_posi
+0000b2b0: 7469 6f6e 203d 2065 7665 6e74 2e63 6f6d  tion = event.com
+0000b2c0: 6d69 745f 706f 7369 7469 6f6e 0a20 2020  mit_position.   
+0000b2d0: 2072 6563 6569 7665 645f 6576 656e 7473   received_events
+0000b2e0: 2e61 7070 656e 6428 6576 656e 7429 0a20  .append(event). 
+0000b2f0: 2020 2069 6620 6576 656e 742e 6964 203d     if event.id =
+0000b300: 3d20 6576 656e 7434 2e69 643a 0a20 2020  = event4.id:.   
+0000b310: 2020 2020 2062 7265 616b 0a0a 6173 7365       break..asse
+0000b320: 7274 2072 6563 6569 7665 645f 6576 656e  rt received_even
+0000b330: 7473 5b2d 345d 2e69 6420 3d3d 2065 7665  ts[-4].id == eve
+0000b340: 6e74 312e 6964 0a61 7373 6572 7420 7265  nt1.id.assert re
+0000b350: 6365 6976 6564 5f65 7665 6e74 735b 2d33  ceived_events[-3
+0000b360: 5d2e 6964 203d 3d20 6576 656e 7432 2e69  ].id == event2.i
+0000b370: 640a 6173 7365 7274 2072 6563 6569 7665  d.assert receive
+0000b380: 645f 6576 656e 7473 5b2d 325d 2e69 6420  d_events[-2].id 
+0000b390: 3d3d 2065 7665 6e74 332e 6964 0a61 7373  == event3.id.ass
+0000b3a0: 6572 7420 7265 6365 6976 6564 5f65 7665  ert received_eve
+0000b3b0: 6e74 735b 2d31 5d2e 6964 203d 3d20 6576  nts[-1].id == ev
+0000b3c0: 656e 7434 2e69 640a 0a23 2041 7070 656e  ent4.id..# Appen
+0000b3d0: 6420 7375 6273 6571 7565 6e74 2065 7665  d subsequent eve
+0000b3e0: 6e74 7320 746f 2074 6865 2073 7472 6561  nts to the strea
+0000b3f0: 6d2e 0a65 7665 6e74 3520 3d20 4e65 7745  m..event5 = NewE
+0000b400: 7665 6e74 2874 7970 653d 274f 7264 6572  vent(type='Order
+0000b410: 5570 6461 7465 6427 2c20 6461 7461 3d62  Updated', data=b
+0000b420: 2764 6174 6135 2729 0a63 6c69 656e 742e  'data5').client.
+0000b430: 6170 7065 6e64 5f65 7665 6e74 7328 0a20  append_events(. 
+0000b440: 2020 2073 7472 6561 6d5f 6e61 6d65 3d73     stream_name=s
+0000b450: 7472 6561 6d5f 6e61 6d65 322c 0a20 2020  tream_name2,.   
+0000b460: 2065 7870 6563 7465 645f 706f 7369 7469   expected_positi
+0000b470: 6f6e 3d30 2c0a 2020 2020 6576 656e 7473  on=0,.    events
+0000b480: 3d5b 6576 656e 7435 5d2c 0a29 0a0a 2320  =[event5],.)..# 
+0000b490: 5265 6365 6976 6520 7375 6273 6571 7565  Receive subseque
+0000b4a0: 6e74 2065 7665 6e74 7320 6672 6f6d 2074  nt events from t
+0000b4b0: 6865 2073 7562 7363 7269 7074 696f 6e2e  he subscription.
+0000b4c0: 0a66 6f72 2065 7665 6e74 2069 6e20 7375  .for event in su
+0000b4d0: 6273 6372 6970 7469 6f6e 3a0a 2020 2020  bscription:.    
+0000b4e0: 6c61 7374 5f63 6f6d 6d69 745f 706f 7369  last_commit_posi
+0000b4f0: 7469 6f6e 203d 2065 7665 6e74 2e63 6f6d  tion = event.com
+0000b500: 6d69 745f 706f 7369 7469 6f6e 0a20 2020  mit_position.   
+0000b510: 2072 6563 6569 7665 645f 6576 656e 7473   received_events
+0000b520: 2e61 7070 656e 6428 6576 656e 7429 0a20  .append(event). 
+0000b530: 2020 2069 6620 6576 656e 742e 6964 203d     if event.id =
+0000b540: 3d20 6576 656e 7435 2e69 643a 0a20 2020  = event5.id:.   
+0000b550: 2020 2020 2062 7265 616b 0a0a 0a61 7373       break...ass
+0000b560: 6572 7420 7265 6365 6976 6564 5f65 7665  ert received_eve
+0000b570: 6e74 735b 2d35 5d2e 6964 203d 3d20 6576  nts[-5].id == ev
+0000b580: 656e 7431 2e69 640a 6173 7365 7274 2072  ent1.id.assert r
+0000b590: 6563 6569 7665 645f 6576 656e 7473 5b2d  eceived_events[-
+0000b5a0: 345d 2e69 6420 3d3d 2065 7665 6e74 322e  4].id == event2.
+0000b5b0: 6964 0a61 7373 6572 7420 7265 6365 6976  id.assert receiv
+0000b5c0: 6564 5f65 7665 6e74 735b 2d33 5d2e 6964  ed_events[-3].id
+0000b5d0: 203d 3d20 6576 656e 7433 2e69 640a 6173   == event3.id.as
+0000b5e0: 7365 7274 2072 6563 6569 7665 645f 6576  sert received_ev
+0000b5f0: 656e 7473 5b2d 325d 2e69 6420 3d3d 2065  ents[-2].id == e
+0000b600: 7665 6e74 342e 6964 0a61 7373 6572 7420  vent4.id.assert 
+0000b610: 7265 6365 6976 6564 5f65 7665 6e74 735b  received_events[
+0000b620: 2d31 5d2e 6964 203d 3d20 6576 656e 7435  -1].id == event5
+0000b630: 2e69 640a 0a0a 2320 4170 7065 6e64 206d  .id...# Append m
+0000b640: 6f72 6520 6576 656e 7473 2074 6f20 7468  ore events to th
+0000b650: 6520 7374 7265 616d 2e0a 6576 656e 7436  e stream..event6
+0000b660: 203d 204e 6577 4576 656e 7428 7479 7065   = NewEvent(type
+0000b670: 3d27 4f72 6465 7244 656c 6574 6564 272c  ='OrderDeleted',
+0000b680: 2064 6174 613d 6227 6461 7461 3627 290a   data=b'data6').
+0000b690: 636c 6965 6e74 2e61 7070 656e 645f 6576  client.append_ev
+0000b6a0: 656e 7473 280a 2020 2020 7374 7265 616d  ents(.    stream
+0000b6b0: 5f6e 616d 653d 7374 7265 616d 5f6e 616d  _name=stream_nam
+0000b6c0: 6532 2c0a 2020 2020 6578 7065 6374 6564  e2,.    expected
+0000b6d0: 5f70 6f73 6974 696f 6e3d 312c 0a20 2020  _position=1,.   
+0000b6e0: 2065 7665 6e74 733d 5b65 7665 6e74 365d   events=[event6]
+0000b6f0: 2c0a 290a 0a0a 2320 5265 7375 6d65 2073  ,.)...# Resume s
+0000b700: 7562 7363 7269 6269 6e67 2066 726f 6d20  ubscribing from 
+0000b710: 7468 6520 6c61 7374 2063 6f6d 6d69 7420  the last commit 
+0000b720: 706f 7369 7469 6f6e 2e0a 7375 6273 6372  position..subscr
+0000b730: 6970 7469 6f6e 203d 2063 6c69 656e 742e  iption = client.
+0000b740: 7375 6273 6372 6962 655f 616c 6c5f 6576  subscribe_all_ev
+0000b750: 656e 7473 280a 2020 2020 636f 6d6d 6974  ents(.    commit
+0000b760: 5f70 6f73 6974 696f 6e3d 6c61 7374 5f63  _position=last_c
+0000b770: 6f6d 6d69 745f 706f 7369 7469 6f6e 0a29  ommit_position.)
+0000b780: 0a0a 0a23 2043 6174 6368 2075 7020 6279  ...# Catch up by
+0000b790: 2072 6563 6569 7669 6e67 2074 6865 206e   receiving the n
+0000b7a0: 6577 2065 7665 6e74 2066 726f 6d20 7468  ew event from th
+0000b7b0: 6520 7375 6273 6372 6970 7469 6f6e 2e0a  e subscription..
+0000b7c0: 666f 7220 6576 656e 7420 696e 2073 7562  for event in sub
+0000b7d0: 7363 7269 7074 696f 6e3a 0a20 2020 2072  scription:.    r
+0000b7e0: 6563 6569 7665 645f 6576 656e 7473 2e61  eceived_events.a
+0000b7f0: 7070 656e 6428 6576 656e 7429 0a20 2020  ppend(event).   
+0000b800: 2069 6620 6576 656e 742e 6964 203d 3d20   if event.id == 
+0000b810: 6576 656e 7436 2e69 643a 0a20 2020 2020  event6.id:.     
+0000b820: 2020 2062 7265 616b 0a0a 6173 7365 7274     break..assert
+0000b830: 2072 6563 6569 7665 645f 6576 656e 7473   received_events
+0000b840: 5b2d 365d 2e69 6420 3d3d 2065 7665 6e74  [-6].id == event
+0000b850: 312e 6964 0a61 7373 6572 7420 7265 6365  1.id.assert rece
+0000b860: 6976 6564 5f65 7665 6e74 735b 2d35 5d2e  ived_events[-5].
+0000b870: 6964 203d 3d20 6576 656e 7432 2e69 640a  id == event2.id.
+0000b880: 6173 7365 7274 2072 6563 6569 7665 645f  assert received_
+0000b890: 6576 656e 7473 5b2d 345d 2e69 6420 3d3d  events[-4].id ==
+0000b8a0: 2065 7665 6e74 332e 6964 0a61 7373 6572   event3.id.asser
+0000b8b0: 7420 7265 6365 6976 6564 5f65 7665 6e74  t received_event
+0000b8c0: 735b 2d33 5d2e 6964 203d 3d20 6576 656e  s[-3].id == even
+0000b8d0: 7434 2e69 640a 6173 7365 7274 2072 6563  t4.id.assert rec
+0000b8e0: 6569 7665 645f 6576 656e 7473 5b2d 325d  eived_events[-2]
+0000b8f0: 2e69 6420 3d3d 2065 7665 6e74 352e 6964  .id == event5.id
+0000b900: 0a61 7373 6572 7420 7265 6365 6976 6564  .assert received
+0000b910: 5f65 7665 6e74 735b 2d31 5d2e 6964 203d  _events[-1].id =
+0000b920: 3d20 6576 656e 7436 2e69 640a 0a0a 2320  = event6.id...# 
+0000b930: 4170 7065 6e64 2074 6872 6565 206d 6f72  Append three mor
+0000b940: 6520 6576 656e 7473 2074 6f20 6120 6e65  e events to a ne
+0000b950: 7720 7374 7265 616d 2e0a 7374 7265 616d  w stream..stream
+0000b960: 5f6e 616d 6533 203d 2073 7472 2875 7569  _name3 = str(uui
+0000b970: 6434 2829 290a 6576 656e 7437 203d 204e  d4()).event7 = N
+0000b980: 6577 4576 656e 7428 7479 7065 3d27 4f72  ewEvent(type='Or
+0000b990: 6465 7243 7265 6174 6564 272c 2064 6174  derCreated', dat
+0000b9a0: 613d 6227 6461 7461 3727 290a 6576 656e  a=b'data7').even
+0000b9b0: 7438 203d 204e 6577 4576 656e 7428 7479  t8 = NewEvent(ty
+0000b9c0: 7065 3d27 4f72 6465 7255 7064 6174 6564  pe='OrderUpdated
+0000b9d0: 272c 2064 6174 613d 6227 6461 7461 3827  ', data=b'data8'
+0000b9e0: 290a 6576 656e 7439 203d 204e 6577 4576  ).event9 = NewEv
+0000b9f0: 656e 7428 7479 7065 3d27 4f72 6465 7244  ent(type='OrderD
+0000ba00: 656c 6574 6564 272c 2064 6174 613d 6227  eleted', data=b'
+0000ba10: 6461 7461 3927 290a 0a63 6c69 656e 742e  data9')..client.
+0000ba20: 6170 7065 6e64 5f65 7665 6e74 7328 0a20  append_events(. 
+0000ba30: 2020 2073 7472 6561 6d5f 6e61 6d65 3d73     stream_name=s
+0000ba40: 7472 6561 6d5f 6e61 6d65 332c 0a20 2020  tream_name3,.   
+0000ba50: 2065 7870 6563 7465 645f 706f 7369 7469   expected_positi
+0000ba60: 6f6e 3d4e 6f6e 652c 0a20 2020 2065 7665  on=None,.    eve
+0000ba70: 6e74 733d 5b65 7665 6e74 372c 2065 7665  nts=[event7, eve
+0000ba80: 6e74 382c 2065 7665 6e74 395d 2c0a 290a  nt8, event9],.).
+0000ba90: 0a23 2052 6563 6569 7665 2074 6865 2074  .# Receive the t
+0000baa0: 6872 6565 206e 6577 2065 7665 6e74 7320  hree new events 
+0000bab0: 6672 6f6d 2074 6865 2072 6573 756d 6564  from the resumed
+0000bac0: 2073 7562 7363 7269 7074 696f 6e2e 0a66   subscription..f
+0000bad0: 6f72 2065 7665 6e74 2069 6e20 7375 6273  or event in subs
+0000bae0: 6372 6970 7469 6f6e 3a0a 2020 2020 7265  cription:.    re
+0000baf0: 6365 6976 6564 5f65 7665 6e74 732e 6170  ceived_events.ap
+0000bb00: 7065 6e64 2865 7665 6e74 290a 2020 2020  pend(event).    
+0000bb10: 6966 2065 7665 6e74 2e69 6420 3d3d 2065  if event.id == e
+0000bb20: 7665 6e74 392e 6964 3a0a 2020 2020 2020  vent9.id:.      
+0000bb30: 2020 6272 6561 6b0a 0a61 7373 6572 7420    break..assert 
+0000bb40: 7265 6365 6976 6564 5f65 7665 6e74 735b  received_events[
+0000bb50: 2d39 5d2e 6964 203d 3d20 6576 656e 7431  -9].id == event1
+0000bb60: 2e69 640a 6173 7365 7274 2072 6563 6569  .id.assert recei
+0000bb70: 7665 645f 6576 656e 7473 5b2d 385d 2e69  ved_events[-8].i
+0000bb80: 6420 3d3d 2065 7665 6e74 322e 6964 0a61  d == event2.id.a
+0000bb90: 7373 6572 7420 7265 6365 6976 6564 5f65  ssert received_e
+0000bba0: 7665 6e74 735b 2d37 5d2e 6964 203d 3d20  vents[-7].id == 
+0000bbb0: 6576 656e 7433 2e69 640a 6173 7365 7274  event3.id.assert
+0000bbc0: 2072 6563 6569 7665 645f 6576 656e 7473   received_events
+0000bbd0: 5b2d 365d 2e69 6420 3d3d 2065 7665 6e74  [-6].id == event
+0000bbe0: 342e 6964 0a61 7373 6572 7420 7265 6365  4.id.assert rece
+0000bbf0: 6976 6564 5f65 7665 6e74 735b 2d35 5d2e  ived_events[-5].
+0000bc00: 6964 203d 3d20 6576 656e 7435 2e69 640a  id == event5.id.
+0000bc10: 6173 7365 7274 2072 6563 6569 7665 645f  assert received_
+0000bc20: 6576 656e 7473 5b2d 345d 2e69 6420 3d3d  events[-4].id ==
+0000bc30: 2065 7665 6e74 362e 6964 0a61 7373 6572   event6.id.asser
+0000bc40: 7420 7265 6365 6976 6564 5f65 7665 6e74  t received_event
+0000bc50: 735b 2d33 5d2e 6964 203d 3d20 6576 656e  s[-3].id == even
+0000bc60: 7437 2e69 640a 6173 7365 7274 2072 6563  t7.id.assert rec
+0000bc70: 6569 7665 645f 6576 656e 7473 5b2d 325d  eived_events[-2]
+0000bc80: 2e69 6420 3d3d 2065 7665 6e74 382e 6964  .id == event8.id
+0000bc90: 0a61 7373 6572 7420 7265 6365 6976 6564  .assert received
+0000bca0: 5f65 7665 6e74 735b 2d31 5d2e 6964 203d  _events[-1].id =
+0000bcb0: 3d20 6576 656e 7439 2e69 640a 6060 600a  = event9.id.```.
+0000bcc0: 0a54 6865 2063 6174 6368 2d75 7020 7375  .The catch-up su
+0000bcd0: 6273 6372 6970 7469 6f6e 2067 5250 4320  bscription gRPC 
+0000bce0: 6f70 6572 6174 696f 6e20 6973 2065 6e64  operation is end
+0000bcf0: 6564 2061 7320 736f 6f6e 2061 7320 7468  ed as soon as th
+0000bd00: 6520 7375 6273 6372 6970 7469 6f6e 206f  e subscription o
+0000bd10: 626a 6563 740a 676f 6573 206f 7574 206f  bject.goes out o
+0000bd20: 6620 7363 6f70 6520 6f72 2069 7320 6578  f scope or is ex
+0000bd30: 706c 6963 6974 6c79 2064 656c 6574 6564  plicitly deleted
+0000bd40: 2066 726f 6d20 6d65 6d6f 7279 2e0a 0a60   from memory...`
+0000bd50: 6060 7079 7468 6f6e 0a23 2045 6e64 2074  ``python.# End t
+0000bd60: 6865 2073 7562 7363 7269 7074 696f 6e2e  he subscription.
+0000bd70: 0a64 656c 2073 7562 7363 7269 7074 696f  .del subscriptio
+0000bd80: 6e0a 6060 600a 0a23 2323 2053 7562 7363  n.```..### Subsc
+0000bd90: 7269 6265 2073 7472 6561 6d20 6576 656e  ribe stream even
+0000bda0: 7473 0a0a 5468 6560 7375 6273 6372 6962  ts..The`subscrib
+0000bdb0: 655f 7374 7265 616d 5f65 7665 6e74 7328  e_stream_events(
+0000bdc0: 2960 206d 6574 686f 6420 6361 6e20 6265  )` method can be
+0000bdd0: 2075 7365 6420 746f 2073 7461 7274 2061   used to start a
+0000bde0: 2022 6361 7463 682d 7570 2220 7375 6273   "catch-up" subs
+0000bdf0: 6372 6970 7469 6f6e 0a74 6861 7420 6361  cription.that ca
+0000be00: 6e20 7265 7475 726e 2061 6c6c 2065 7665  n return all eve
+0000be10: 6e74 7320 696e 2061 2073 7472 6561 6d2e  nts in a stream.
+0000be20: 0a0a 5468 6973 206d 6574 686f 6420 7461  ..This method ta
+0000be30: 6b65 7320 6120 6073 7472 6561 6d5f 6e61  kes a `stream_na
+0000be40: 6d65 6020 6172 6775 6d65 6e74 2c20 7768  me` argument, wh
+0000be50: 6963 6820 7370 6563 6966 6965 7320 7468  ich specifies th
+0000be60: 6520 6e61 6d65 206f 6620 7468 6520 7374  e name of the st
+0000be70: 7265 616d 0a66 726f 6d20 7768 6963 6820  ream.from which 
+0000be80: 7265 636f 7264 6564 2065 7665 6e74 7320  recorded events 
+0000be90: 7769 6c6c 2062 6520 7265 6365 6976 6564  will be received
+0000bea0: 2e0a 0a54 6869 7320 6d65 7468 6f64 2074  ...This method t
+0000beb0: 616b 6573 2061 6e20 6f70 7469 6f6e 616c  akes an optional
+0000bec0: 2060 7374 7265 616d 5f70 6f73 6974 696f   `stream_positio
+0000bed0: 6e60 2061 7267 756d 656e 742c 2077 6869  n` argument, whi
+0000bee0: 6368 2073 7065 6369 6669 6573 2061 0a73  ch specifies a.s
+0000bef0: 7472 6561 6d20 706f 7369 7469 6f6e 2069  tream position i
+0000bf00: 6e20 7468 6520 7374 7265 616d 2066 726f  n the stream fro
+0000bf10: 6d20 7768 6963 6820 7265 636f 7264 6564  m which recorded
+0000bf20: 2065 7665 6e74 7320 7769 6c6c 2062 6520   events will be 
+0000bf30: 7265 6365 6976 6564 2e20 5468 650a 6576  received. The.ev
+0000bf40: 656e 7420 6174 2074 6865 2073 7065 6369  ent at the speci
+0000bf50: 6669 6564 2073 7472 6561 6d20 706f 7369  fied stream posi
+0000bf60: 7469 6f6e 2077 696c 6c20 6e6f 7420 6265  tion will not be
+0000bf70: 2069 6e63 6c75 6465 642e 0a0a 5468 6973   included...This
+0000bf80: 206d 6574 686f 6420 7461 6b65 7320 616e   method takes an
+0000bf90: 206f 7074 696f 6e61 6c20 6074 696d 656f   optional `timeo
+0000bfa0: 7574 6020 6172 6775 6d65 6e74 2c20 7768  ut` argument, wh
+0000bfb0: 6963 6820 6973 2061 2050 7974 686f 6e20  ich is a Python 
+0000bfc0: 6066 6c6f 6174 6020 7468 6174 2073 6574  `float` that set
+0000bfd0: 730a 6120 6465 6164 6c69 6e65 2066 6f72  s.a deadline for
+0000bfe0: 2074 6865 2063 6f6d 706c 6574 696f 6e20   the completion 
+0000bff0: 6f66 2074 6865 2067 5250 4320 6f70 6572  of the gRPC oper
+0000c000: 6174 696f 6e2e 0a0a 5468 6520 6578 616d  ation...The exam
+0000c010: 706c 6520 6265 6c6f 7720 7368 6f77 7320  ple below shows 
+0000c020: 686f 7720 746f 2073 7461 7274 2061 2063  how to start a c
+0000c030: 6174 6368 2d75 7020 7375 6273 6372 6970  atch-up subscrip
+0000c040: 7469 6f6e 2074 6f20 6120 7374 7265 616d  tion to a stream
+0000c050: 2e0a 0a60 6060 7079 7468 6f6e 0a0a 2320  ...```python..# 
+0000c060: 5375 6273 6372 6962 6520 746f 2065 7665  Subscribe to eve
+0000c070: 6e74 7320 6672 6f6d 2073 7472 6561 6d32  nts from stream2
+0000c080: 2c20 6672 6f6d 2074 6865 2073 7461 7274  , from the start
+0000c090: 2e0a 7375 6273 6372 6970 7469 6f6e 203d  ..subscription =
+0000c0a0: 2063 6c69 656e 742e 7375 6273 6372 6962   client.subscrib
+0000c0b0: 655f 7374 7265 616d 5f65 7665 6e74 7328  e_stream_events(
+0000c0c0: 7374 7265 616d 5f6e 616d 653d 7374 7265  stream_name=stre
+0000c0d0: 616d 5f6e 616d 6532 290a 0a23 2052 6561  am_name2)..# Rea
+0000c0e0: 6420 6672 6f6d 2074 6865 2073 7562 7363  d from the subsc
+0000c0f0: 7269 7074 696f 6e2e 0a65 7665 6e74 7320  ription..events 
+0000c100: 3d20 5b5d 0a66 6f72 2065 7665 6e74 2069  = [].for event i
+0000c110: 6e20 7375 6273 6372 6970 7469 6f6e 3a0a  n subscription:.
+0000c120: 2020 2020 6576 656e 7473 2e61 7070 656e      events.appen
+0000c130: 6428 6576 656e 7429 0a20 2020 2069 6620  d(event).    if 
+0000c140: 6576 656e 742e 6964 203d 3d20 6576 656e  event.id == even
+0000c150: 7436 2e69 643a 0a20 2020 2020 2020 2062  t6.id:.        b
+0000c160: 7265 616b 0a0a 2320 4368 6563 6b20 7765  reak..# Check we
+0000c170: 2067 6f74 2065 7665 6e74 7320 6f6e 6c79   got events only
+0000c180: 2066 726f 6d20 7374 7265 616d 322e 0a61   from stream2..a
+0000c190: 7373 6572 7420 6c65 6e28 6576 656e 7473  ssert len(events
+0000c1a0: 2920 3d3d 2033 0a65 7665 6e74 735b 305d  ) == 3.events[0]
+0000c1b0: 2e73 7472 6561 6d5f 6e61 6d65 203d 3d20  .stream_name == 
+0000c1c0: 7374 7265 616d 5f6e 616d 6532 0a65 7665  stream_name2.eve
+0000c1d0: 6e74 735b 315d 2e73 7472 6561 6d5f 6e61  nts[1].stream_na
+0000c1e0: 6d65 203d 3d20 7374 7265 616d 5f6e 616d  me == stream_nam
+0000c1f0: 6532 0a65 7665 6e74 735b 325d 2e73 7472  e2.events[2].str
+0000c200: 6561 6d5f 6e61 6d65 203d 3d20 7374 7265  eam_name == stre
+0000c210: 616d 5f6e 616d 6532 0a0a 2320 4170 7065  am_name2..# Appe
+0000c220: 6e64 2061 6e6f 7468 6572 2065 7665 6e74  nd another event
+0000c230: 2074 6f20 7374 7265 616d 332e 0a65 7665   to stream3..eve
+0000c240: 6e74 3130 203d 204e 6577 4576 656e 7428  nt10 = NewEvent(
+0000c250: 7479 7065 3d22 4f72 6465 7255 6e64 656c  type="OrderUndel
+0000c260: 6574 6564 222c 2064 6174 613d 6227 6461  eted", data=b'da
+0000c270: 7461 3130 2729 0a63 6c69 656e 742e 6170  ta10').client.ap
+0000c280: 7065 6e64 5f65 7665 6e74 7328 0a20 2020  pend_events(.   
+0000c290: 2073 7472 6561 6d5f 6e61 6d65 3d73 7472   stream_name=str
+0000c2a0: 6561 6d5f 6e61 6d65 332c 0a20 2020 2065  eam_name3,.    e
+0000c2b0: 7870 6563 7465 645f 706f 7369 7469 6f6e  xpected_position
+0000c2c0: 3d32 2c0a 2020 2020 6576 656e 7473 3d5b  =2,.    events=[
+0000c2d0: 6576 656e 7431 305d 2c0a 290a 0a23 2041  event10],.)..# A
+0000c2e0: 7070 656e 6420 616e 6f74 6865 7220 6576  ppend another ev
+0000c2f0: 656e 7420 746f 2073 7472 6561 6d32 2e0a  ent to stream2..
+0000c300: 6576 656e 7431 3120 3d20 4e65 7745 7665  event11 = NewEve
+0000c310: 6e74 2874 7970 653d 224f 7264 6572 556e  nt(type="OrderUn
+0000c320: 6465 6c65 7465 6422 2c20 6461 7461 3d62  deleted", data=b
+0000c330: 2764 6174 6131 3127 290a 636c 6965 6e74  'data11').client
+0000c340: 2e61 7070 656e 645f 6576 656e 7473 280a  .append_events(.
+0000c350: 2020 2020 7374 7265 616d 5f6e 616d 653d      stream_name=
+0000c360: 7374 7265 616d 5f6e 616d 6532 2c0a 2020  stream_name2,.  
+0000c370: 2020 6578 7065 6374 6564 5f70 6f73 6974    expected_posit
+0000c380: 696f 6e3d 322c 0a20 2020 2065 7665 6e74  ion=2,.    event
+0000c390: 733d 5b65 7665 6e74 3131 5d0a 290a 0a23  s=[event11].)..#
+0000c3a0: 2043 6f6e 7469 6e75 6520 7265 6164 696e   Continue readin
+0000c3b0: 6720 6672 6f6d 2074 6865 2073 7562 7363  g from the subsc
+0000c3c0: 7269 7074 696f 6e2e 0a66 6f72 2065 7665  ription..for eve
+0000c3d0: 6e74 2069 6e20 7375 6273 6372 6970 7469  nt in subscripti
+0000c3e0: 6f6e 3a0a 2020 2020 6576 656e 7473 2e61  on:.    events.a
+0000c3f0: 7070 656e 6428 6576 656e 7429 0a20 2020  ppend(event).   
+0000c400: 2069 6620 6576 656e 742e 6964 203d 3d20   if event.id == 
+0000c410: 6576 656e 7431 312e 6964 3a0a 2020 2020  event11.id:.    
+0000c420: 2020 2020 6272 6561 6b0a 0a23 2043 6865      break..# Che
+0000c430: 636b 2077 6520 676f 7420 6576 656e 7473  ck we got events
+0000c440: 206f 6e6c 7920 6672 6f6d 2073 7472 6561   only from strea
+0000c450: 6d32 2e0a 6173 7365 7274 206c 656e 2865  m2..assert len(e
+0000c460: 7665 6e74 7329 203d 3d20 340a 6576 656e  vents) == 4.even
+0000c470: 7473 5b30 5d2e 7374 7265 616d 5f6e 616d  ts[0].stream_nam
+0000c480: 6520 3d3d 2073 7472 6561 6d5f 6e61 6d65  e == stream_name
+0000c490: 320a 6576 656e 7473 5b31 5d2e 7374 7265  2.events[1].stre
+0000c4a0: 616d 5f6e 616d 6520 3d3d 2073 7472 6561  am_name == strea
+0000c4b0: 6d5f 6e61 6d65 320a 6576 656e 7473 5b32  m_name2.events[2
+0000c4c0: 5d2e 7374 7265 616d 5f6e 616d 6520 3d3d  ].stream_name ==
+0000c4d0: 2073 7472 6561 6d5f 6e61 6d65 320a 6576   stream_name2.ev
+0000c4e0: 656e 7473 5b33 5d2e 7374 7265 616d 5f6e  ents[3].stream_n
+0000c4f0: 616d 6520 3d3d 2073 7472 6561 6d5f 6e61  ame == stream_na
+0000c500: 6d65 320a 6060 600a 0a54 6865 2065 7861  me2.```..The exa
+0000c510: 6d70 6c65 2062 656c 6f77 2073 686f 7773  mple below shows
+0000c520: 2068 6f77 2074 6f20 7374 6172 7420 6120   how to start a 
+0000c530: 6361 7463 682d 7570 2073 7562 7363 7269  catch-up subscri
+0000c540: 7074 696f 6e20 746f 2061 2073 7472 6561  ption to a strea
+0000c550: 6d20 6672 6f6d 2061 0a73 7065 6369 6669  m from a.specifi
+0000c560: 6320 7374 7265 616d 2070 6f73 6974 696f  c stream positio
+0000c570: 6e2e 0a0a 6060 6070 7974 686f 6e0a 0a23  n...```python..#
+0000c580: 2053 7562 7363 7269 6265 2074 6f20 6576   Subscribe to ev
+0000c590: 656e 7473 2066 726f 6d20 7374 7265 616d  ents from stream
+0000c5a0: 322c 2066 726f 6d20 7468 6520 7374 6172  2, from the star
+0000c5b0: 742e 0a73 7562 7363 7269 7074 696f 6e20  t..subscription 
+0000c5c0: 3d20 636c 6965 6e74 2e73 7562 7363 7269  = client.subscri
+0000c5d0: 6265 5f73 7472 6561 6d5f 6576 656e 7473  be_stream_events
+0000c5e0: 280a 2020 2020 7374 7265 616d 5f6e 616d  (.    stream_nam
+0000c5f0: 653d 7374 7265 616d 5f6e 616d 6532 2c0a  e=stream_name2,.
+0000c600: 2020 2020 7374 7265 616d 5f70 6f73 6974      stream_posit
+0000c610: 696f 6e3d 312c 0a29 0a0a 2320 5265 6164  ion=1,.)..# Read
+0000c620: 2065 7665 6e74 2066 726f 6d20 7468 6520   event from the 
+0000c630: 7375 6273 6372 6970 7469 6f6e 2e0a 6576  subscription..ev
+0000c640: 656e 7473 203d 205b 5d0a 666f 7220 6576  ents = [].for ev
+0000c650: 656e 7420 696e 2073 7562 7363 7269 7074  ent in subscript
+0000c660: 696f 6e3a 0a20 2020 2065 7665 6e74 732e  ion:.    events.
+0000c670: 6170 7065 6e64 2865 7665 6e74 290a 2020  append(event).  
+0000c680: 2020 6966 2065 7665 6e74 2e69 6420 3d3d    if event.id ==
+0000c690: 2065 7665 6e74 3131 2e69 643a 0a20 2020   event11.id:.   
+0000c6a0: 2020 2020 2062 7265 616b 0a0a 2320 4368       break..# Ch
+0000c6b0: 6563 6b20 7765 2067 6f74 2065 7665 6e74  eck we got event
+0000c6c0: 7320 6f6e 6c79 2061 6674 6572 2070 6f73  s only after pos
+0000c6d0: 6974 696f 6e20 312e 0a61 7373 6572 7420  ition 1..assert 
+0000c6e0: 6c65 6e28 6576 656e 7473 2920 3d3d 2032  len(events) == 2
+0000c6f0: 0a65 7665 6e74 735b 305d 2e69 6420 3d3d  .events[0].id ==
+0000c700: 2065 7665 6e74 362e 6964 0a65 7665 6e74   event6.id.event
+0000c710: 735b 305d 2e73 7472 6561 6d5f 706f 7369  s[0].stream_posi
+0000c720: 7469 6f6e 203d 3d20 320a 6576 656e 7473  tion == 2.events
+0000c730: 5b30 5d2e 7374 7265 616d 5f6e 616d 6520  [0].stream_name 
+0000c740: 3d3d 2073 7472 6561 6d5f 6e61 6d65 320a  == stream_name2.
+0000c750: 6576 656e 7473 5b31 5d2e 6964 203d 3d20  events[1].id == 
+0000c760: 6576 656e 7431 312e 6964 0a65 7665 6e74  event11.id.event
+0000c770: 735b 315d 2e73 7472 6561 6d5f 706f 7369  s[1].stream_posi
+0000c780: 7469 6f6e 203d 3d20 330a 6576 656e 7473  tion == 3.events
+0000c790: 5b31 5d2e 7374 7265 616d 5f6e 616d 6520  [1].stream_name 
+0000c7a0: 3d3d 2073 7472 6561 6d5f 6e61 6d65 320a  == stream_name2.
+0000c7b0: 6060 600a 0a23 2320 5065 7273 6973 7465  ```..## Persiste
+0000c7c0: 6e74 2073 7562 7363 7269 7074 696f 6e73  nt subscriptions
+0000c7d0: 0a0a 2323 2320 4372 6561 7465 2073 7562  ..### Create sub
+0000c7e0: 7363 7269 7074 696f 6e0a 0a54 6865 206d  scription..The m
+0000c7f0: 6574 686f 6420 6063 7265 6174 655f 7375  ethod `create_su
+0000c800: 6273 6372 6970 7469 6f6e 2829 6020 6361  bscription()` ca
+0000c810: 6e20 6265 2075 7365 6420 746f 2063 7265  n be used to cre
+0000c820: 6174 6520 610a 2270 6572 7369 7374 656e  ate a."persisten
+0000c830: 7420 7375 6273 6372 6970 7469 6f6e 2220  t subscription" 
+0000c840: 746f 2045 7665 6e74 5374 6f72 6544 422e  to EventStoreDB.
+0000c850: 0a0a 5468 6973 206d 6574 686f 6420 7461  ..This method ta
+0000c860: 6b65 7320 6120 7265 7175 6972 6564 2060  kes a required `
+0000c870: 6772 6f75 705f 6e61 6d65 6020 6172 6775  group_name` argu
+0000c880: 6d65 6e74 2c20 7768 6963 6820 6973 2074  ment, which is t
+0000c890: 6865 0a6e 616d 6520 6f66 2061 2022 6772  he.name of a "gr
+0000c8a0: 6f75 7022 206f 6620 636f 6e73 756d 6572  oup" of consumer
+0000c8b0: 7320 6f66 2074 6865 2073 7562 7363 7269  s of the subscri
+0000c8c0: 7074 696f 6e2e 0a0a 5468 6973 206d 6574  ption...This met
+0000c8d0: 686f 6420 7461 6b65 7320 616e 206f 7074  hod takes an opt
+0000c8e0: 696f 6e61 6c20 6066 726f 6d5f 656e 6460  ional `from_end`
+0000c8f0: 2061 7267 756d 656e 742c 2077 6869 6368   argument, which
+0000c900: 2063 616e 2062 650a 7573 6564 2074 6f20   can be.used to 
+0000c910: 7370 6563 6966 7920 7468 6174 2074 6865  specify that the
+0000c920: 2067 726f 7570 206f 6620 636f 6e73 756d   group of consum
+0000c930: 6572 7320 6f66 2074 6865 2073 7562 7363  ers of the subsc
+0000c940: 7269 7074 696f 6e20 7368 6f75 6c64 0a6f  ription should.o
+0000c950: 6e6c 7920 7265 6365 6976 6520 6576 656e  nly receive even
+0000c960: 7473 2074 6861 7420 7765 7265 2072 6563  ts that were rec
+0000c970: 6f72 6465 6420 6166 7465 7220 7468 6520  orded after the 
+0000c980: 7375 6273 6372 6970 7469 6f6e 2077 6173  subscription was
+0000c990: 2063 7265 6174 6564 2e0a 0a54 6869 7320   created...This 
+0000c9a0: 6d65 7468 6f64 2074 616b 6573 2061 6e20  method takes an 
+0000c9b0: 6f70 7469 6f6e 616c 2060 636f 6d6d 6974  optional `commit
+0000c9c0: 5f70 6f73 6974 696f 6e60 2061 7267 756d  _position` argum
+0000c9d0: 656e 742c 2077 6869 6368 2063 616e 2062  ent, which can b
+0000c9e0: 650a 7573 6564 2074 6f20 7370 6563 6966  e.used to specif
+0000c9f0: 7920 6120 636f 6d6d 6974 2070 6f73 6974  y a commit posit
+0000ca00: 696f 6e20 6672 6f6d 2077 6869 6368 2074  ion from which t
+0000ca10: 6865 2067 726f 7570 206f 6620 636f 6e73  he group of cons
+0000ca20: 756d 6572 7320 6f66 0a74 6865 2073 7562  umers of.the sub
+0000ca30: 7363 7269 7074 696f 6e20 7368 6f75 6c64  scription should
+0000ca40: 2072 6563 6569 7665 2065 7665 6e74 732e   receive events.
+0000ca50: 2050 6c65 6173 6520 6e6f 7465 2c20 7468   Please note, th
+0000ca60: 6520 7265 636f 7264 6564 2065 7665 6e74  e recorded event
+0000ca70: 0a61 7420 7468 6520 7370 6563 6966 6965  .at the specifie
+0000ca80: 6420 636f 6d6d 6974 2070 6f73 6974 696f  d commit positio
+0000ca90: 6e20 4d41 5920 6265 2069 6e63 6c75 6465  n MAY be include
+0000caa0: 6420 696e 2074 6865 2072 6563 6f72 6465  d in the recorde
+0000cab0: 6420 6576 656e 7473 0a72 6563 6569 7665  d events.receive
+0000cac0: 6420 6279 2074 6865 2067 726f 7570 206f  d by the group o
+0000cad0: 6620 636f 6e73 756d 6572 732e 0a0a 4966  f consumers...If
+0000cae0: 206e 6569 7468 6572 2060 6672 6f6d 5f65   neither `from_e
+0000caf0: 6e64 6020 6f72 2060 636f 6d6d 6974 5f70  nd` or `commit_p
+0000cb00: 6f73 6974 696f 6e60 2061 7265 2073 7065  osition` are spe
+0000cb10: 6369 6669 6564 2c20 7468 6520 6772 6f75  cified, the grou
+0000cb20: 7020 6f66 2063 6f6e 7375 6d65 7273 0a6f  p of consumers.o
+0000cb30: 6620 7468 6520 7375 6273 6372 6970 7469  f the subscripti
+0000cb40: 6f6e 2077 696c 6c20 7265 6365 6976 6520  on will receive 
+0000cb50: 616c 6c20 7265 636f 7264 6564 2065 7665  all recorded eve
+0000cb60: 6e74 732e 0a0a 5468 6973 206d 6574 686f  nts...This metho
+0000cb70: 6420 616c 736f 2074 616b 6573 206f 7074  d also takes opt
+0000cb80: 696f 6e20 6066 696c 7465 725f 6578 636c  ion `filter_excl
+0000cb90: 7564 6560 2c20 6066 696c 7465 725f 696e  ude`, `filter_in
+0000cba0: 636c 7564 6560 0a61 7267 756d 656e 7473  clude`.arguments
+0000cbb0: 2c20 7768 6963 6820 776f 726b 2069 6e20  , which work in 
+0000cbc0: 7468 6520 7361 6d65 2077 6179 2061 7320  the same way as 
+0000cbd0: 7468 6579 2064 6f20 696e 2074 6865 2060  they do in the `
+0000cbe0: 7375 6273 6372 6962 655f 616c 6c5f 6576  subscribe_all_ev
+0000cbf0: 656e 7473 2829 600a 6d65 7468 6f64 2e0a  ents()`.method..
+0000cc00: 0a54 6869 7320 6d65 7468 6f64 2061 6c73  .This method als
+0000cc10: 6f20 7461 6b65 7320 616e 206f 7074 696f  o takes an optio
+0000cc20: 6e61 6c20 6074 696d 656f 7574 6020 6172  nal `timeout` ar
+0000cc30: 6775 6d65 6e74 2c20 7468 6174 0a69 7320  gument, that.is 
+0000cc40: 6578 7065 6374 6564 2074 6f20 6265 2061  expected to be a
+0000cc50: 2050 7974 686f 6e20 6066 6c6f 6174 602c   Python `float`,
+0000cc60: 2077 6869 6368 2073 6574 7320 6120 6465   which sets a de
+0000cc70: 6164 6c69 6e65 0a66 6f72 2074 6865 2063  adline.for the c
+0000cc80: 6f6d 706c 6574 696f 6e20 6f66 2074 6865  ompletion of the
+0000cc90: 2067 5250 4320 6f70 6572 6174 696f 6e2e   gRPC operation.
+0000cca0: 0a0a 5468 6520 6d65 7468 6f64 2060 6372  ..The method `cr
+0000ccb0: 6561 7465 5f73 7562 7363 7269 7074 696f  eate_subscriptio
+0000ccc0: 6e28 2960 2064 6f65 7320 6e6f 7420 7265  n()` does not re
+0000ccd0: 7475 726e 2061 2076 616c 7565 2c20 6265  turn a value, be
+0000cce0: 6361 7573 650a 7265 636f 7264 6564 2065  cause.recorded e
+0000ccf0: 7665 6e74 7320 6172 6520 6f62 7461 696e  vents are obtain
+0000cd00: 6564 2062 7920 7468 6520 6772 6f75 7020  ed by the group 
+0000cd10: 6f66 2063 6f6e 7375 6d65 7273 206f 6620  of consumers of 
+0000cd20: 7468 6520 7375 6273 6372 6970 7469 6f6e  the subscription
+0000cd30: 0a75 7369 6e67 2074 6865 2060 7265 6164  .using the `read
+0000cd40: 5f73 7562 7363 7269 7074 696f 6e28 2960  _subscription()`
+0000cd50: 206d 6574 686f 642e 0a0a 2a50 6c65 6173   method...*Pleas
+0000cd60: 6520 6e6f 7465 2c20 696e 2074 6869 7320  e note, in this 
+0000cd70: 7665 7273 696f 6e20 6f66 2074 6869 7320  version of this 
+0000cd80: 636c 6965 6e74 2074 6865 2022 636f 6e73  client the "cons
+0000cd90: 756d 6572 2073 7472 6174 6567 7922 2069  umer strategy" i
+0000cda0: 730a 7365 7420 746f 2022 4469 7370 6174  s.set to "Dispat
+0000cdb0: 6368 546f 5369 6e67 6c65 222e 2053 7570  chToSingle". Sup
+0000cdc0: 706f 7274 2066 6f72 2063 686f 6f73 696e  port for choosin
+0000cdd0: 6720 6f74 6865 7220 636f 6e73 756d 6572  g other consumer
+0000cde0: 2073 7472 6174 6567 6965 730a 7375 7070   strategies.supp
+0000cdf0: 6f72 7465 6420 6279 2045 7665 6e74 5374  orted by EventSt
+0000ce00: 6f72 6544 4220 7769 6c6c 2069 6e20 6675  oreDB will in fu
+0000ce10: 7475 7265 2062 6520 7375 7070 6f72 7465  ture be supporte
+0000ce20: 6420 696e 2074 6869 7320 636c 6965 6e74  d in this client
+0000ce30: 2e2a 0a0a 496e 2074 6865 2065 7861 6d70  .*..In the examp
+0000ce40: 6c65 2062 656c 6f77 2c20 6120 7065 7273  le below, a pers
+0000ce50: 6973 7465 6e74 2073 7562 7363 7269 7074  istent subscript
+0000ce60: 696f 6e20 6973 2063 7265 6174 6564 2e0a  ion is created..
+0000ce70: 0a60 6060 7079 7468 6f6e 0a23 2043 7265  .```python.# Cre
+0000ce80: 6174 6520 6120 7065 7273 6973 7465 6e74  ate a persistent
+0000ce90: 2073 7562 7363 7269 7074 696f 6e2e 0a67   subscription..g
+0000cea0: 726f 7570 5f6e 616d 6520 3d20 6622 6772  roup_name = f"gr
+0000ceb0: 6f75 702d 7b75 7569 6434 2829 7d22 0a63  oup-{uuid4()}".c
+0000cec0: 6c69 656e 742e 6372 6561 7465 5f73 7562  lient.create_sub
+0000ced0: 7363 7269 7074 696f 6e28 6772 6f75 705f  scription(group_
+0000cee0: 6e61 6d65 3d67 726f 7570 5f6e 616d 6529  name=group_name)
+0000cef0: 0a60 6060 0a0a 2323 2320 5265 6164 2073  .```..### Read s
+0000cf00: 7562 7363 7269 7074 696f 6e0a 0a54 6865  ubscription..The
+0000cf10: 206d 6574 686f 6420 6072 6561 645f 7375   method `read_su
+0000cf20: 6273 6372 6970 7469 6f6e 2829 6020 6361  bscription()` ca
+0000cf30: 6e20 6265 2075 7365 6420 6279 2061 2067  n be used by a g
+0000cf40: 726f 7570 206f 6620 636f 6e73 756d 6572  roup of consumer
+0000cf50: 7320 746f 2072 6563 6569 7665 0a72 6563  s to receive.rec
+0000cf60: 6f72 6465 6420 6576 656e 7473 2066 726f  orded events fro
+0000cf70: 6d20 6120 7065 7273 6973 7465 6e74 2073  m a persistent s
+0000cf80: 7562 7363 7269 7074 696f 6e20 6372 6561  ubscription crea
+0000cf90: 7465 6420 7573 696e 6720 6063 7265 6174  ted using `creat
+0000cfa0: 655f 7375 6273 6372 6970 7469 6f6e 602e  e_subscription`.
+0000cfb0: 0a0a 5468 6973 206d 6574 686f 6420 7461  ..This method ta
+0000cfc0: 6b65 7320 6120 7265 7175 6972 6564 2060  kes a required `
+0000cfd0: 6772 6f75 705f 6e61 6d65 6020 6172 6775  group_name` argu
+0000cfe0: 6d65 6e74 2c20 7768 6963 6820 6973 0a74  ment, which is.t
+0000cff0: 6865 206e 616d 6520 6f66 2061 2022 6772  he name of a "gr
+0000d000: 6f75 7022 206f 6620 636f 6e73 756d 6572  oup" of consumer
+0000d010: 7320 6f66 2074 6865 2073 7562 7363 7269  s of the subscri
+0000d020: 7074 696f 6e20 7370 6563 6966 6965 640a  ption specified.
+0000d030: 7768 656e 2060 6372 6561 7465 5f73 7562  when `create_sub
+0000d040: 7363 7269 7074 696f 6e28 2960 2077 6173  scription()` was
+0000d050: 2063 616c 6c65 642e 0a0a 5468 6973 206d   called...This m
+0000d060: 6574 686f 6420 616c 736f 2074 616b 6573  ethod also takes
+0000d070: 2061 6e20 6f70 7469 6f6e 616c 2060 7469   an optional `ti
+0000d080: 6d65 6f75 7460 2061 7267 756d 656e 742c  meout` argument,
+0000d090: 2074 6861 740a 6973 2065 7870 6563 7465   that.is expecte
+0000d0a0: 6420 746f 2062 6520 6120 5079 7468 6f6e  d to be a Python
+0000d0b0: 2060 666c 6f61 7460 2c20 7768 6963 6820   `float`, which 
+0000d0c0: 7365 7473 2061 2064 6561 646c 696e 650a  sets a deadline.
+0000d0d0: 666f 7220 7468 6520 636f 6d70 6c65 7469  for the completi
+0000d0e0: 6f6e 206f 6620 7468 6520 6752 5043 206f  on of the gRPC o
+0000d0f0: 7065 7261 7469 6f6e 2e0a 0a54 6869 7320  peration...This 
+0000d100: 6d65 7468 6f64 2072 6574 7572 6e73 2061  method returns a
+0000d110: 2032 2d74 7570 6c65 3a20 6120 2272 6561   2-tuple: a "rea
+0000d120: 6420 7265 7175 6573 7422 206f 626a 6563  d request" objec
+0000d130: 7420 616e 6420 6120 2272 6561 6420 7265  t and a "read re
+0000d140: 7370 6f6e 7365 2220 6f62 6a65 6374 2e0a  sponse" object..
+0000d150: 0a60 6060 7079 7468 6f6e 0a72 6561 645f  .```python.read_
+0000d160: 7265 712c 2072 6561 645f 7265 7370 203d  req, read_resp =
+0000d170: 2063 6c69 656e 742e 7265 6164 5f73 7562   client.read_sub
+0000d180: 7363 7269 7074 696f 6e28 6772 6f75 705f  scription(group_
+0000d190: 6e61 6d65 3d67 726f 7570 5f6e 616d 6529  name=group_name)
+0000d1a0: 0a60 6060 0a0a 5468 6520 2272 6561 6420  .```..The "read 
+0000d1b0: 7265 7370 6f6e 7365 2220 6f62 6a65 6374  response" object
+0000d1c0: 2069 7320 616e 2069 7465 7261 746f 7220   is an iterator 
+0000d1d0: 7468 6174 2079 6965 6c64 7320 7265 636f  that yields reco
+0000d1e0: 7264 6564 2065 7665 6e74 7320 6672 6f6d  rded events from
+0000d1f0: 0a74 6865 2073 7065 6369 6669 6564 2063  .the specified c
+0000d200: 6f6d 6d69 7420 706f 7369 7469 6f6e 2e0a  ommit position..
+0000d210: 0a54 6865 2022 7265 6164 2072 6571 7565  .The "read reque
+0000d220: 7374 2220 6f62 6a65 6374 2068 6173 2061  st" object has a
+0000d230: 6e20 6061 636b 2829 6020 6d65 7468 6f64  n `ack()` method
+0000d240: 2074 6861 7420 6361 6e20 6265 2075 7365   that can be use
+0000d250: 6420 6279 2061 2063 6f6e 7375 6d65 720a  d by a consumer.
+0000d260: 696e 2061 2067 726f 7570 2074 6f20 6163  in a group to ac
+0000d270: 6b6e 6f77 6c65 6467 6520 746f 2074 6865  knowledge to the
+0000d280: 2073 6572 7665 7220 7468 6174 2069 7420   server that it 
+0000d290: 6861 7320 7265 6365 6976 6564 2061 6e64  has received and
+0000d2a0: 2073 7563 6365 7373 6675 6c6c 790a 7072   successfully.pr
+0000d2b0: 6f63 6573 7365 6420 6120 7265 636f 7264  ocessed a record
+0000d2c0: 6564 2065 7665 6e74 2e20 5468 6973 2077  ed event. This w
+0000d2d0: 696c 6c20 7072 6576 656e 7420 7468 6174  ill prevent that
+0000d2e0: 2072 6563 6f72 6465 6420 6576 656e 7420   recorded event 
+0000d2f0: 6265 696e 6720 7265 6365 6976 6564 0a62  being received.b
+0000d300: 7920 616e 6f74 6865 7220 636f 6e73 756d  y another consum
+0000d310: 6572 2069 6e20 7468 6520 7361 6d65 2067  er in the same g
+0000d320: 726f 7570 2e20 5468 6520 6061 636b 2829  roup. The `ack()
+0000d330: 6020 6d65 7468 6f64 2074 616b 6573 2061  ` method takes a
+0000d340: 6e20 6065 7665 6e74 5f69 6460 0a61 7267  n `event_id`.arg
+0000d350: 756d 656e 742c 2077 6869 6368 2069 7320  ument, which is 
+0000d360: 7468 6520 4944 206f 6620 7468 6520 7265  the ID of the re
+0000d370: 636f 7264 6564 2065 7665 6e74 2074 6861  corded event tha
+0000d380: 7420 6861 7320 6265 656e 2072 6563 6569  t has been recei
+0000d390: 7665 642e 0a0a 5468 6520 6578 616d 706c  ved...The exampl
+0000d3a0: 6520 6265 6c6f 7720 6974 6572 6174 6573  e below iterates
+0000d3b0: 206f 7665 7220 7468 6520 2272 6561 6420   over the "read 
+0000d3c0: 7265 7370 6f6e 7365 2220 6f62 6a65 6374  response" object
+0000d3d0: 2c20 616e 6420 6361 6c6c 7320 6061 636b  , and calls `ack
+0000d3e0: 2829 600a 6f6e 2074 6865 2022 7265 6164  ()`.on the "read
+0000d3f0: 2072 6573 706f 6e73 6522 206f 626a 6563   response" objec
+0000d400: 742e 2054 6865 2066 6f72 206c 6f6f 7020  t. The for loop 
+0000d410: 6272 6561 6b73 2077 6865 6e20 7765 2068  breaks when we h
+0000d420: 6176 6520 7265 6365 6976 6564 0a74 6865  ave received.the
+0000d430: 206c 6173 7420 6576 656e 742c 2073 6f20   last event, so 
+0000d440: 7468 6174 2077 6520 6361 6e20 636f 6e74  that we can cont
+0000d450: 696e 7565 2077 6974 6820 7468 6520 6578  inue with the ex
+0000d460: 616d 706c 6573 2062 656c 6f77 2e0a 0a60  amples below...`
+0000d470: 6060 7079 7468 6f6e 0a65 7665 6e74 7320  ``python.events 
+0000d480: 3d20 5b5d 0a66 6f72 2065 7665 6e74 2069  = [].for event i
+0000d490: 6e20 7265 6164 5f72 6573 703a 0a20 2020  n read_resp:.   
+0000d4a0: 2065 7665 6e74 732e 6170 7065 6e64 2865   events.append(e
+0000d4b0: 7665 6e74 290a 0a20 2020 2023 2041 636b  vent)..    # Ack
+0000d4c0: 6e6f 776c 6564 6765 2074 6865 2072 6563  nowledge the rec
+0000d4d0: 6569 7665 6420 6576 656e 742e 0a20 2020  eived event..   
+0000d4e0: 2072 6561 645f 7265 712e 6163 6b28 6576   read_req.ack(ev
+0000d4f0: 656e 745f 6964 3d65 7665 6e74 2e69 6429  ent_id=event.id)
+0000d500: 0a0a 2020 2020 2320 4272 6561 6b20 7768  ..    # Break wh
+0000d510: 656e 2074 6865 206c 6173 7420 6576 656e  en the last even
+0000d520: 7420 6861 7320 6265 656e 2072 6563 6569  t has been recei
+0000d530: 7665 642e 0a20 2020 2069 6620 6576 656e  ved..    if even
+0000d540: 742e 6964 203d 3d20 6576 656e 7431 312e  t.id == event11.
+0000d550: 6964 3a0a 2020 2020 2020 2020 6272 6561  id:.        brea
+0000d560: 6b0a 6060 600a 0a54 6865 2072 6563 6569  k.```..The recei
+0000d570: 7665 6420 6576 656e 7473 2061 7265 2074  ved events are t
+0000d580: 6865 2065 7665 6e74 7320 7765 2061 7070  he events we app
+0000d590: 656e 6465 6420 6162 6f76 652e 0a0a 6060  ended above...``
+0000d5a0: 6070 7974 686f 6e0a 6173 7365 7274 2065  `python.assert e
+0000d5b0: 7665 6e74 735b 2d31 315d 2e69 6420 3d3d  vents[-11].id ==
+0000d5c0: 2065 7665 6e74 312e 6964 0a61 7373 6572   event1.id.asser
+0000d5d0: 7420 6576 656e 7473 5b2d 3130 5d2e 6964  t events[-10].id
+0000d5e0: 203d 3d20 6576 656e 7432 2e69 640a 6173   == event2.id.as
+0000d5f0: 7365 7274 2065 7665 6e74 735b 2d39 5d2e  sert events[-9].
+0000d600: 6964 203d 3d20 6576 656e 7433 2e69 640a  id == event3.id.
+0000d610: 6173 7365 7274 2065 7665 6e74 735b 2d38  assert events[-8
+0000d620: 5d2e 6964 203d 3d20 6576 656e 7434 2e69  ].id == event4.i
+0000d630: 640a 6173 7365 7274 2065 7665 6e74 735b  d.assert events[
+0000d640: 2d37 5d2e 6964 203d 3d20 6576 656e 7435  -7].id == event5
+0000d650: 2e69 640a 6173 7365 7274 2065 7665 6e74  .id.assert event
+0000d660: 735b 2d36 5d2e 6964 203d 3d20 6576 656e  s[-6].id == even
+0000d670: 7436 2e69 640a 6173 7365 7274 2065 7665  t6.id.assert eve
+0000d680: 6e74 735b 2d35 5d2e 6964 203d 3d20 6576  nts[-5].id == ev
+0000d690: 656e 7437 2e69 640a 6173 7365 7274 2065  ent7.id.assert e
+0000d6a0: 7665 6e74 735b 2d34 5d2e 6964 203d 3d20  vents[-4].id == 
+0000d6b0: 6576 656e 7438 2e69 640a 6173 7365 7274  event8.id.assert
+0000d6c0: 2065 7665 6e74 735b 2d33 5d2e 6964 203d   events[-3].id =
+0000d6d0: 3d20 6576 656e 7439 2e69 640a 6173 7365  = event9.id.asse
+0000d6e0: 7274 2065 7665 6e74 735b 2d32 5d2e 6964  rt events[-2].id
+0000d6f0: 203d 3d20 6576 656e 7431 302e 6964 0a61   == event10.id.a
+0000d700: 7373 6572 7420 6576 656e 7473 5b2d 315d  ssert events[-1]
+0000d710: 2e69 6420 3d3d 2065 7665 6e74 3131 2e69  .id == event11.i
+0000d720: 640a 6060 600a 0a54 6865 2022 7265 6164  d.```..The "read
+0000d730: 2072 6571 7565 7374 2220 6f62 6a65 6374   request" object
+0000d740: 2061 6c73 6f20 6861 7320 616e 2060 6e61   also has an `na
+0000d750: 636b 2829 6020 6d65 7468 6f64 2074 6861  ck()` method tha
+0000d760: 7420 6361 6e20 6265 2075 7365 6420 6279  t can be used by
+0000d770: 2061 2063 6f6e 7375 6d65 720a 696e 2061   a consumer.in a
+0000d780: 2067 726f 7570 2074 6f20 6163 6b6e 6f77   group to acknow
+0000d790: 6c65 6467 6520 746f 2074 6865 2073 6572  ledge to the ser
+0000d7a0: 7665 7220 7468 6174 2069 7420 6861 7320  ver that it has 
+0000d7b0: 6661 696c 6564 2073 7563 6365 7373 6675  failed successfu
+0000d7c0: 6c6c 7920 746f 0a70 726f 6365 7373 2061  lly to.process a
+0000d7d0: 2072 6563 6f72 6465 6420 6576 656e 742e   recorded event.
+0000d7e0: 2054 6869 7320 7769 6c6c 2061 6c6c 6f77   This will allow
+0000d7f0: 2074 6861 7420 7265 636f 7264 6564 2065   that recorded e
+0000d800: 7665 6e74 2074 6f20 6265 2072 6563 6569  vent to be recei
+0000d810: 7665 640a 6279 2074 6869 7320 6f72 2061  ved.by this or a
+0000d820: 6e6f 7468 6572 2063 6f6e 7375 6d65 7220  nother consumer 
+0000d830: 696e 2074 6865 2073 616d 6520 6772 6f75  in the same grou
+0000d840: 702e 0a0a 4974 206d 6967 6874 2062 6520  p...It might be 
+0000d850: 6d6f 7265 2075 7365 6675 6c20 746f 2065  more useful to e
+0000d860: 6e63 6170 7375 6c61 7465 2074 6865 2072  ncapsulate the r
+0000d870: 6571 7565 7374 2061 6e64 2072 6573 706f  equest and respo
+0000d880: 6e73 6520 6f62 6a65 6374 7320 616e 6420  nse objects and 
+0000d890: 746f 2069 7465 7261 7465 0a6f 7665 7220  to iterate.over 
+0000d8a0: 7468 6520 2272 6561 6420 7265 7370 6f6e  the "read respon
+0000d8b0: 7365 2220 696e 2061 2073 6570 6172 6174  se" in a separat
+0000d8c0: 6520 7468 7265 6164 2c20 746f 2063 616c  e thread, to cal
+0000d8d0: 6c20 6261 636b 2074 6f20 6120 6861 6e64  l back to a hand
+0000d8e0: 6c65 7220 6675 6e63 7469 6f6e 2077 6865  ler function whe
+0000d8f0: 6e0a 6120 7265 636f 7264 6564 2065 7665  n.a recorded eve
+0000d900: 6e74 2069 7320 7265 6365 6976 6564 2c20  nt is received, 
+0000d910: 616e 6420 6361 6c6c 2060 6163 6b28 2960  and call `ack()`
+0000d920: 2069 6620 7468 6520 6861 6e64 6c65 7220   if the handler 
+0000d930: 646f 6573 206e 6f74 2072 6169 7365 2061  does not raise a
+0000d940: 6e0a 6578 6365 7074 696f 6e2c 2061 6e64  n.exception, and
+0000d950: 2074 6f20 6361 6c6c 2060 6e61 636b 2829   to call `nack()
+0000d960: 6020 6966 2061 6e20 6578 6365 7074 696f  ` if an exceptio
+0000d970: 6e20 6973 2072 6169 7365 642e 2054 6865  n is raised. The
+0000d980: 2065 7861 6d70 6c65 2062 656c 6f77 2073   example below s
+0000d990: 686f 7773 2068 6f77 0a74 6869 7320 6d69  hows how.this mi
+0000d9a0: 6768 7420 6265 2064 6f6e 652e 0a0a 6060  ght be done...``
+0000d9b0: 6070 7974 686f 6e0a 6672 6f6d 2074 6872  `python.from thr
+0000d9c0: 6561 6469 6e67 2069 6d70 6f72 7420 5468  eading import Th
+0000d9d0: 7265 6164 0a0a 0a63 6c61 7373 2053 7562  read...class Sub
+0000d9e0: 7363 7269 7074 696f 6e52 6561 6465 723a  scriptionReader:
+0000d9f0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0000da00: 5f28 7365 6c66 2c20 636c 6965 6e74 2c20  _(self, client, 
+0000da10: 6772 6f75 705f 6e61 6d65 2c20 6361 6c6c  group_name, call
+0000da20: 6261 636b 293a 0a20 2020 2020 2020 2073  back):.        s
+0000da30: 656c 662e 636c 6965 6e74 203d 2063 6c69  elf.client = cli
+0000da40: 656e 740a 2020 2020 2020 2020 7365 6c66  ent.        self
+0000da50: 2e67 726f 7570 5f6e 616d 6520 3d20 6772  .group_name = gr
+0000da60: 6f75 705f 6e61 6d65 0a20 2020 2020 2020  oup_name.       
+0000da70: 2073 656c 662e 6361 6c6c 6261 636b 203d   self.callback =
+0000da80: 2063 616c 6c62 6163 6b0a 2020 2020 2020   callback.      
+0000da90: 2020 7365 6c66 2e74 6872 6561 6420 3d20    self.thread = 
+0000daa0: 5468 7265 6164 2874 6172 6765 743d 7365  Thread(target=se
+0000dab0: 6c66 2e72 6561 645f 7375 6273 6372 6970  lf.read_subscrip
+0000dac0: 7469 6f6e 2c20 6461 656d 6f6e 3d54 7275  tion, daemon=Tru
+0000dad0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+0000dae0: 6572 726f 7220 3d20 4e6f 6e65 0a0a 2020  error = None..  
+0000daf0: 2020 6465 6620 7374 6172 7428 7365 6c66    def start(self
+0000db00: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0000db10: 7468 7265 6164 2e73 7461 7274 2829 0a0a  thread.start()..
+0000db20: 2020 2020 6465 6620 6a6f 696e 2873 656c      def join(sel
+0000db30: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+0000db40: 2e74 6872 6561 642e 6a6f 696e 2829 0a0a  .thread.join()..
+0000db50: 2020 2020 6465 6620 7265 6164 5f73 7562      def read_sub
+0000db60: 7363 7269 7074 696f 6e28 7365 6c66 293a  scription(self):
+0000db70: 0a20 2020 2020 2020 2072 6571 2c20 7265  .        req, re
+0000db80: 7370 203d 2073 656c 662e 636c 6965 6e74  sp = self.client
+0000db90: 2e72 6561 645f 7375 6273 6372 6970 7469  .read_subscripti
+0000dba0: 6f6e 2867 726f 7570 5f6e 616d 653d 7365  on(group_name=se
+0000dbb0: 6c66 2e67 726f 7570 5f6e 616d 6529 0a20  lf.group_name). 
+0000dbc0: 2020 2020 2020 2066 6f72 2065 7665 6e74         for event
+0000dbd0: 2069 6e20 7265 7370 3a0a 2020 2020 2020   in resp:.      
+0000dbe0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000dbf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000dc00: 6361 6c6c 6261 636b 2865 7665 6e74 290a  callback(event).
+0000dc10: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+0000dc20: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+0000dc30: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000dc40: 2020 2023 2072 6571 2e6e 6163 6b28 6576     # req.nack(ev
+0000dc50: 656e 742e 6964 2920 2023 206e 6f74 2079  ent.id)  # not y
+0000dc60: 6574 2069 6d70 6c65 6d65 6e74 6564 2e2e  et implemented..
+0000dc70: 2e2e 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000dc80: 2020 2073 656c 662e 6572 726f 7220 3d20     self.error = 
+0000dc90: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000dca0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+0000dcb0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000dcc0: 2020 2020 2020 2020 2020 7265 712e 6163            req.ac
+0000dcd0: 6b28 6576 656e 742e 6964 290a 0a0a 2320  k(event.id)...# 
+0000dce0: 4372 6561 7465 2061 6e6f 7468 6572 2070  Create another p
+0000dcf0: 6572 7369 7374 656e 7420 7375 6273 6372  ersistent subscr
+0000dd00: 6970 7469 6f6e 2e0a 6772 6f75 705f 6e61  iption..group_na
+0000dd10: 6d65 203d 2066 2267 726f 7570 2d7b 7575  me = f"group-{uu
+0000dd20: 6964 3428 297d 220a 636c 6965 6e74 2e63  id4()}".client.c
+0000dd30: 7265 6174 655f 7375 6273 6372 6970 7469  reate_subscripti
+0000dd40: 6f6e 2867 726f 7570 5f6e 616d 653d 6772  on(group_name=gr
+0000dd50: 6f75 705f 6e61 6d65 290a 0a65 7665 6e74  oup_name)..event
+0000dd60: 7320 3d20 5b5d 0a0a 6465 6620 6861 6e64  s = []..def hand
+0000dd70: 6c65 5f65 7665 6e74 2865 7665 6e74 293a  le_event(event):
+0000dd80: 0a20 2020 2065 7665 6e74 732e 6170 7065  .    events.appe
+0000dd90: 6e64 2865 7665 6e74 290a 2020 2020 6966  nd(event).    if
+0000dda0: 2065 7665 6e74 2e69 6420 3d3d 2065 7665   event.id == eve
+0000ddb0: 6e74 3131 2e69 643a 0a20 2020 2020 2020  nt11.id:.       
+0000ddc0: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
+0000ddd0: 2829 0a0a 0a72 6561 6465 7220 3d20 5375  ()...reader = Su
+0000dde0: 6273 6372 6970 7469 6f6e 5265 6164 6572  bscriptionReader
+0000ddf0: 280a 2020 2020 636c 6965 6e74 3d63 6c69  (.    client=cli
+0000de00: 656e 742c 0a20 2020 2067 726f 7570 5f6e  ent,.    group_n
+0000de10: 616d 653d 6772 6f75 705f 6e61 6d65 2c0a  ame=group_name,.
+0000de20: 2020 2020 6361 6c6c 6261 636b 3d68 616e      callback=han
+0000de30: 646c 655f 6576 656e 740a 290a 0a72 6561  dle_event.)..rea
+0000de40: 6465 722e 7374 6172 7428 290a 7265 6164  der.start().read
+0000de50: 6572 2e6a 6f69 6e28 290a 0a61 7373 6572  er.join()..asser
+0000de60: 7420 6576 656e 7473 5b2d 315d 2e69 6420  t events[-1].id 
+0000de70: 3d3d 2065 7665 6e74 3131 2e69 640a 6060  == event11.id.``
+0000de80: 600a 0a50 6c65 6173 6520 6e6f 7465 2c20  `..Please note, 
+0000de90: 7768 656e 2070 726f 6365 7373 696e 6720  when processing 
+0000dea0: 6576 656e 7473 2069 6e20 6120 646f 776e  events in a down
+0000deb0: 7374 7265 616d 2063 6f6d 706f 6e65 6e74  stream component
+0000dec0: 2c20 7468 6520 636f 6d6d 6974 2070 6f73  , the commit pos
+0000ded0: 6974 696f 6e20 6f66 0a74 6865 206c 6173  ition of.the las
+0000dee0: 7420 7375 6363 6573 7366 756c 6c79 2070  t successfully p
+0000def0: 726f 6365 7373 6564 2065 7665 6e74 2069  rocessed event i
+0000df00: 7320 7573 6566 756c 6c79 2072 6563 6f72  s usefully recor
+0000df10: 6465 6420 6279 2074 6865 2064 6f77 6e73  ded by the downs
+0000df20: 7472 6561 6d20 636f 6d70 6f6e 656e 740a  tream component.
+0000df30: 736f 2074 6861 7420 7468 6520 636f 6d6d  so that the comm
+0000df40: 6974 2070 6f73 6974 696f 6e20 6361 6e20  it position can 
+0000df50: 6265 2064 6574 6572 6d69 6e65 6420 6279  be determined by
+0000df60: 2074 6865 2064 6f77 6e73 7472 6561 6d20   the downstream 
+0000df70: 636f 6d70 6f6e 656e 7420 6672 6f6d 2069  component from i
+0000df80: 7473 206f 776e 0a72 6563 6f72 6465 6420  ts own.recorded 
+0000df90: 7768 656e 2069 7420 6973 2072 6573 7461  when it is resta
+0000dfa0: 7274 6564 2e20 5468 6973 2063 6f6d 6d69  rted. This commi
+0000dfb0: 7420 706f 7369 7469 6f6e 2063 616e 2062  t position can b
+0000dfc0: 6520 7573 6564 2074 6f20 7370 6563 6966  e used to specif
+0000dfd0: 7920 7468 6520 636f 6d6d 6974 0a70 6f73  y the commit.pos
+0000dfe0: 6974 696f 6e20 6672 6f6d 2077 6869 6368  ition from which
+0000dff0: 2074 6f20 7375 6273 6372 6962 652e 2053   to subscribe. S
+0000e000: 696e 6365 2074 6869 7320 636f 6d6d 6974  ince this commit
+0000e010: 2070 6f73 6974 696f 6e20 7265 7072 6573   position repres
+0000e020: 656e 7473 2074 6865 2070 6f73 6974 696f  ents the positio
+0000e030: 6e20 6f66 0a74 6865 206c 6173 7420 7375  n of.the last su
+0000e040: 6363 6573 7366 756c 6c79 2070 726f 6365  ccessfully proce
+0000e050: 7373 6564 2065 7665 6e74 2069 6e20 6120  ssed event in a 
+0000e060: 646f 776e 7374 7265 616d 2063 6f6d 706f  downstream compo
+0000e070: 6e65 6e74 2c20 736f 2069 7420 7769 6c6c  nent, so it will
+0000e080: 2062 6520 7573 7561 6c20 746f 0a77 616e   be usual to.wan
+0000e090: 7420 746f 2072 6561 6420 6672 6f6d 2074  t to read from t
+0000e0a0: 6865 206e 6578 7420 6576 656e 7420 6166  he next event af
+0000e0b0: 7465 7220 7468 6973 2070 6f73 6974 696f  ter this positio
+0000e0c0: 6e2c 2062 6563 6175 7365 2074 6861 7420  n, because that 
+0000e0d0: 6973 2074 6865 206e 6578 7420 6576 656e  is the next even
+0000e0e0: 740a 7468 6174 206e 6565 6473 2074 6f20  t.that needs to 
+0000e0f0: 6265 2070 726f 6365 7373 6564 2e20 486f  be processed. Ho
+0000e100: 7765 7665 722c 2077 6865 6e20 7375 6273  wever, when subs
+0000e110: 6372 6962 696e 6720 666f 7220 6576 656e  cribing for even
+0000e120: 7473 2075 7369 6e67 2061 2070 6572 7369  ts using a persi
+0000e130: 7374 656e 740a 7375 6273 6372 6970 7469  stent.subscripti
+0000e140: 6f6e 2069 6e20 4576 656e 7453 746f 7265  on in EventStore
+0000e150: 4442 2c20 7468 6520 6576 656e 7420 6174  DB, the event at
+0000e160: 2074 6865 2073 7065 6369 6669 6564 2063   the specified c
+0000e170: 6f6d 6d69 7420 706f 7369 7469 6f6e 204d  ommit position M
+0000e180: 4159 2062 6520 7265 7475 726e 6564 0a61  AY be returned.a
+0000e190: 7320 7468 6520 6669 7273 7420 6576 656e  s the first even
+0000e1a0: 7420 696e 2074 6865 2072 6563 6569 7665  t in the receive
+0000e1b0: 6420 7365 7175 656e 6365 206f 6620 7265  d sequence of re
+0000e1c0: 636f 7264 6564 2065 7665 6e74 732c 2061  corded events, a
+0000e1d0: 6e64 2073 6f20 6974 206d 6179 0a62 6520  nd so it may.be 
+0000e1e0: 6e65 6365 7373 6172 7920 746f 2063 6865  necessary to che
+0000e1f0: 636b 2074 6865 2063 6f6d 6d69 7420 706f  ck the commit po
+0000e200: 7369 7469 6f6e 206f 6620 7468 6520 7265  sition of the re
+0000e210: 6365 6976 6564 2065 7665 6e74 7320 616e  ceived events an
+0000e220: 6420 746f 2064 6973 6361 7264 0a61 6e79  d to discard.any
+0000e230: 2020 7265 636f 7264 6564 2065 7665 6e74    recorded event
+0000e240: 206f 626a 6563 7420 7468 6174 2068 6173   object that has
+0000e250: 2061 2063 6f6d 6d69 7420 706f 7369 7469   a commit positi
+0000e260: 6f6e 2065 7175 616c 2074 6f20 7468 6520  on equal to the 
+0000e270: 636f 6d6d 6974 2070 6f73 6974 696f 6e0a  commit position.
+0000e280: 7370 6563 6966 6965 6420 696e 2074 6865  specified in the
+0000e290: 2072 6571 7565 7374 2e0a 0a57 6869 6c73   request...Whils
+0000e2a0: 7420 7468 6572 6520 6172 6520 736f 6d65  t there are some
+0000e2b0: 2061 6476 616e 7461 6765 7320 6f66 2070   advantages of p
+0000e2c0: 6572 7369 7374 656e 7420 7375 6273 6372  ersistent subscr
+0000e2d0: 6970 7469 6f6e 732c 2069 6e20 7061 7274  iptions, in part
+0000e2e0: 6963 756c 6172 2074 6865 0a70 726f 6365  icular the.proce
+0000e2f0: 7373 696e 6720 6f66 2072 6563 6f72 6465  ssing of recorde
+0000e300: 6420 6576 656e 7473 2062 7920 6120 6772  d events by a gr
+0000e310: 6f75 7020 6f66 2063 6f6e 7375 6d65 7273  oup of consumers
+0000e320: 2c20 6279 2074 7261 636b 696e 6720 696e  , by tracking in
+0000e330: 2074 6865 0a75 7073 7472 6561 6d20 7365   the.upstream se
+0000e340: 7276 6572 2074 6865 2070 6f73 6974 696f  rver the positio
+0000e350: 6e20 696e 2074 6865 2063 6f6d 6d69 7420  n in the commit 
+0000e360: 7365 7175 656e 6365 206f 6620 6576 656e  sequence of even
+0000e370: 7473 2074 6861 7420 6861 7665 2062 6565  ts that have bee
+0000e380: 6e20 7072 6f63 6573 7365 642c 0a74 6865  n processed,.the
+0000e390: 7265 2069 7320 6120 6461 6e67 6572 206f  re is a danger o
+0000e3a0: 6620 2264 7561 6c20 7772 6974 696e 6722  f "dual writing"
+0000e3b0: 2069 6e20 7468 6520 636f 6e73 756d 7074   in the consumpt
+0000e3c0: 696f 6e20 6f66 2065 7665 6e74 732e 2052  ion of events. R
+0000e3d0: 656c 6961 6269 6c69 7479 0a69 6e20 7072  eliability.in pr
+0000e3e0: 6f63 6573 7369 6e67 206f 6620 7265 636f  ocessing of reco
+0000e3f0: 7264 6564 2065 7665 6e74 7320 6279 2061  rded events by a
+0000e400: 2067 726f 7570 206f 6620 636f 6e73 756d   group of consum
+0000e410: 6572 7320 7769 6c6c 2072 656c 7920 696e  ers will rely in
+0000e420: 7374 6561 6420 6f6e 0a69 6465 6d70 6f74  stead on.idempot
+0000e430: 656e 7420 6861 6e64 6c69 6e67 206f 6620  ent handling of 
+0000e440: 6475 706c 6963 6174 6520 6d65 7373 6167  duplicate messag
+0000e450: 6573 2c20 616e 6420 7265 7369 6c69 656e  es, and resilien
+0000e460: 6365 2074 6f20 6f75 742d 6f66 2d6f 7264  ce to out-of-ord
+0000e470: 6572 2064 656c 6976 6572 792e 0a0a 2323  er delivery...##
+0000e480: 2320 4765 7420 7375 6273 6372 6970 7469  # Get subscripti
+0000e490: 6f6e 2069 6e66 6f0a 0a54 6865 2060 6765  on info..The `ge
+0000e4a0: 745f 7375 6273 6372 6970 7469 6f6e 5f69  t_subscription_i
+0000e4b0: 6e66 6f28 2960 206d 6574 686f 6420 6361  nfo()` method ca
+0000e4c0: 6e20 6265 2075 7365 6420 746f 2067 6574  n be used to get
+0000e4d0: 2069 6e66 6f72 6d61 7469 6f6e 2066 6f72   information for
+0000e4e0: 2061 0a70 6572 7369 7374 656e 7420 7375   a.persistent su
+0000e4f0: 6273 6372 6970 7469 6f6e 2e0a 0a54 6869  bscription...Thi
+0000e500: 7320 6d65 7468 6f64 2068 6173 206f 6e65  s method has one
+0000e510: 2072 6571 7569 7265 6420 6172 6775 6d65   required argume
+0000e520: 6e74 2c20 6067 726f 7570 5f6e 616d 6560  nt, `group_name`
+0000e530: 2c20 7768 6963 680a 7368 6f75 6c64 206d  , which.should m
+0000e540: 6174 6368 2074 6865 2076 616c 7565 206f  atch the value o
+0000e550: 6620 7468 6520 6172 6775 6d65 6e74 2075  f the argument u
+0000e560: 7365 6420 7768 656e 2063 616c 6c69 6e67  sed when calling
+0000e570: 2060 6372 6561 7465 5f73 7562 7363 7269   `create_subscri
+0000e580: 7074 696f 6e28 2960 2e0a 0a54 6869 7320  ption()`...This 
+0000e590: 6d65 7468 6f64 2061 6c73 6f20 7461 6b65  method also take
+0000e5a0: 7320 616e 206f 7074 696f 6e61 6c20 6074  s an optional `t
+0000e5b0: 696d 656f 7574 6020 6172 6775 6d65 6e74  imeout` argument
+0000e5c0: 2c20 7468 6174 0a69 7320 6578 7065 6374  , that.is expect
+0000e5d0: 6564 2074 6f20 6265 2061 2050 7974 686f  ed to be a Pytho
+0000e5e0: 6e20 6066 6c6f 6174 602c 2077 6869 6368  n `float`, which
+0000e5f0: 2073 6574 7320 6120 6465 6164 6c69 6e65   sets a deadline
+0000e600: 0a66 6f72 2074 6865 2063 6f6d 706c 6574  .for the complet
+0000e610: 696f 6e20 6f66 2074 6865 2067 5250 4320  ion of the gRPC 
+0000e620: 6f70 6572 6174 696f 6e2e 0a0a 6060 6070  operation...```p
+0000e630: 7974 686f 6e0a 7375 6273 6372 6970 7469  ython.subscripti
+0000e640: 6f6e 5f69 6e66 6f20 3d20 636c 6965 6e74  on_info = client
+0000e650: 2e67 6574 5f73 7562 7363 7269 7074 696f  .get_subscriptio
+0000e660: 6e5f 696e 666f 280a 2020 2020 6772 6f75  n_info(.    grou
+0000e670: 705f 6e61 6d65 3d67 726f 7570 5f6e 616d  p_name=group_nam
+0000e680: 652c 0a29 0a60 6060 0a0a 5468 6520 7265  e,.).```..The re
+0000e690: 7475 726e 6564 2076 616c 7565 2069 7320  turned value is 
+0000e6a0: 6120 6053 7562 7363 7269 7074 696f 6e49  a `SubscriptionI
+0000e6b0: 6e66 6f60 206f 626a 6563 742e 0a0a 2323  nfo` object...##
+0000e6c0: 2320 4c69 7374 2073 7562 7363 7269 7074  # List subscript
+0000e6d0: 696f 6e73 0a0a 5468 6520 606c 6973 745f  ions..The `list_
+0000e6e0: 7375 6273 6372 6970 7469 6f6e 7328 2960  subscriptions()`
+0000e6f0: 206d 6574 686f 6420 6361 6e20 6265 2075   method can be u
+0000e700: 7365 6420 746f 2067 6574 2069 6e66 6f72  sed to get infor
+0000e710: 6d61 7469 6f6e 2066 6f72 2061 6c6c 0a65  mation for all.e
+0000e720: 7869 7374 696e 6720 7065 7273 6973 7465  xisting persiste
+0000e730: 6e74 2073 7562 7363 7269 7074 696f 6e73  nt subscriptions
+0000e740: 2e0a 0a54 6869 7320 6d65 7468 6f64 2074  ...This method t
+0000e750: 616b 6573 2061 6e20 6f70 7469 6f6e 616c  akes an optional
+0000e760: 2060 7469 6d65 6f75 7460 2061 7267 756d   `timeout` argum
+0000e770: 656e 742c 2074 6861 740a 6973 2065 7870  ent, that.is exp
+0000e780: 6563 7465 6420 746f 2062 6520 6120 5079  ected to be a Py
+0000e790: 7468 6f6e 2060 666c 6f61 7460 2c20 7768  thon `float`, wh
+0000e7a0: 6963 6820 7365 7473 2061 2064 6561 646c  ich sets a deadl
+0000e7b0: 696e 650a 666f 7220 7468 6520 636f 6d70  ine.for the comp
+0000e7c0: 6c65 7469 6f6e 206f 6620 7468 6520 6752  letion of the gR
+0000e7d0: 5043 206f 7065 7261 7469 6f6e 2e0a 0a60  PC operation...`
+0000e7e0: 6060 7079 7468 6f6e 0a73 7562 7363 7269  ``python.subscri
+0000e7f0: 7074 696f 6e73 203d 2063 6c69 656e 742e  ptions = client.
+0000e800: 6c69 7374 5f73 7562 7363 7269 7074 696f  list_subscriptio
+0000e810: 6e73 2829 0a60 6060 0a0a 5468 6520 7265  ns().```..The re
+0000e820: 7475 726e 6564 2076 616c 7565 2069 7320  turned value is 
+0000e830: 6120 6c69 7374 206f 6620 6053 7562 7363  a list of `Subsc
+0000e840: 7269 7074 696f 6e49 6e66 6f60 206f 626a  riptionInfo` obj
+0000e850: 6563 7473 2e0a 0a23 2323 2044 656c 6574  ects...### Delet
+0000e860: 6520 7375 6273 6372 6970 7469 6f6e 0a0a  e subscription..
+0000e870: 5468 6520 6064 656c 6574 655f 7375 6273  The `delete_subs
+0000e880: 6372 6970 7469 6f6e 2829 6020 6d65 7468  cription()` meth
+0000e890: 6f64 2063 616e 2062 6520 7573 6564 2074  od can be used t
+0000e8a0: 6f20 6465 6c65 7465 2061 2070 6572 7369  o delete a persi
+0000e8b0: 7374 656e 740a 7375 6273 6372 6970 7469  stent.subscripti
+0000e8c0: 6f6e 2e0a 0a54 6869 7320 6d65 7468 6f64  on...This method
+0000e8d0: 2068 6173 206f 6e65 2072 6571 7569 7265   has one require
+0000e8e0: 6420 6172 6775 6d65 6e74 2c20 6067 726f  d argument, `gro
+0000e8f0: 7570 5f6e 616d 6560 2c20 7768 6963 680a  up_name`, which.
+0000e900: 7368 6f75 6c64 206d 6174 6368 2074 6865  should match the
+0000e910: 2076 616c 7565 206f 6620 6172 6775 6d65   value of argume
+0000e920: 6e74 2075 7365 6420 7768 656e 2063 616c  nt used when cal
+0000e930: 6c69 6e67 2060 6372 6561 7465 5f73 7562  ling `create_sub
+0000e940: 7363 7269 7074 696f 6e28 2960 2e0a 0a54  scription()`...T
+0000e950: 6869 7320 6d65 7468 6f64 2061 6c73 6f20  his method also 
+0000e960: 7461 6b65 7320 616e 206f 7074 696f 6e61  takes an optiona
+0000e970: 6c20 6074 696d 656f 7574 6020 6172 6775  l `timeout` argu
+0000e980: 6d65 6e74 2c20 7468 6174 0a69 7320 6578  ment, that.is ex
+0000e990: 7065 6374 6564 2074 6f20 6265 2061 2050  pected to be a P
+0000e9a0: 7974 686f 6e20 6066 6c6f 6174 602c 2077  ython `float`, w
+0000e9b0: 6869 6368 2073 6574 7320 6120 6465 6164  hich sets a dead
+0000e9c0: 6c69 6e65 0a66 6f72 2074 6865 2063 6f6d  line.for the com
+0000e9d0: 706c 6574 696f 6e20 6f66 2074 6865 2067  pletion of the g
+0000e9e0: 5250 4320 6f70 6572 6174 696f 6e2e 0a0a  RPC operation...
+0000e9f0: 6060 6070 7974 686f 6e0a 636c 6965 6e74  ```python.client
+0000ea00: 2e64 656c 6574 655f 7375 6273 6372 6970  .delete_subscrip
+0000ea10: 7469 6f6e 280a 2020 2020 6772 6f75 705f  tion(.    group_
+0000ea20: 6e61 6d65 3d67 726f 7570 5f6e 616d 652c  name=group_name,
+0000ea30: 0a29 0a60 6060 0a0a 2323 2320 4372 6561  .).```..### Crea
+0000ea40: 7465 2073 7472 6561 6d20 7375 6273 6372  te stream subscr
+0000ea50: 6970 7469 6f6e 0a0a 5468 6520 6063 7265  iption..The `cre
+0000ea60: 6174 655f 7374 7265 616d 5f73 7562 7363  ate_stream_subsc
+0000ea70: 7269 7074 696f 6e28 2960 206d 6574 686f  ription()` metho
+0000ea80: 6420 6361 6e20 6265 2075 7365 6420 746f  d can be used to
+0000ea90: 2063 7265 6174 6520 6120 7065 7273 6973   create a persis
+0000eaa0: 7465 6e74 0a73 7562 7363 7269 7074 696f  tent.subscriptio
+0000eab0: 6e20 666f 7220 6120 7374 7265 616d 2e0a  n for a stream..
+0000eac0: 0a54 6869 7320 6d65 7468 6f64 2068 6173  .This method has
+0000ead0: 2074 776f 2072 6571 7569 7265 6420 6172   two required ar
+0000eae0: 6775 6d65 6e74 732c 2060 6772 6f75 705f  guments, `group_
+0000eaf0: 6e61 6d65 6020 616e 6420 6073 7472 6561  name` and `strea
+0000eb00: 6d5f 6e61 6d65 602e 2054 6865 0a60 6772  m_name`. The.`gr
+0000eb10: 6f75 705f 6e61 6d65 6020 6172 6775 6d65  oup_name` argume
+0000eb20: 6e74 206e 616d 6573 2074 6865 2067 726f  nt names the gro
+0000eb30: 7570 206f 6620 636f 6e73 756d 6572 7320  up of consumers 
+0000eb40: 7468 6174 2077 696c 6c20 7265 6365 6976  that will receiv
+0000eb50: 6520 6576 656e 7473 0a66 726f 6d20 7468  e events.from th
+0000eb60: 6973 2073 7562 7363 7269 7074 696f 6e2e  is subscription.
+0000eb70: 2054 6865 2060 7374 7265 616d 5f6e 616d   The `stream_nam
+0000eb80: 6560 2061 7267 756d 656e 7420 7370 6563  e` argument spec
+0000eb90: 6966 6965 7320 7768 6963 6820 7374 7265  ifies which stre
+0000eba0: 616d 0a74 6865 2073 7562 7363 7269 7074  am.the subscript
+0000ebb0: 696f 6e20 7769 6c6c 2066 6f6c 6c6f 772e  ion will follow.
+0000ebc0: 2054 6865 2076 616c 7565 7320 6f66 2062   The values of b
+0000ebd0: 6f74 6820 7468 6573 6520 6172 6775 6d65  oth these argume
+0000ebe0: 6e74 7320 6172 6520 6578 7065 6374 6564  nts are expected
+0000ebf0: 0a74 6f20 6265 2050 7974 686f 6e20 6073  .to be Python `s
+0000ec00: 7472 6020 6f62 6a65 6374 732e 0a0a 5468  tr` objects...Th
+0000ec10: 6973 206d 6574 686f 6420 6861 7320 616e  is method has an
+0000ec20: 206f 7074 696f 6e61 6c20 6073 7472 6561   optional `strea
+0000ec30: 6d5f 706f 7369 7469 6f6e 6020 6172 6775  m_position` argu
+0000ec40: 6d65 6e74 2c20 7768 6963 6820 7370 6563  ment, which spec
+0000ec50: 6966 6965 7320 610a 7374 7265 616d 2070  ifies a.stream p
+0000ec60: 6f73 6974 696f 6e20 6672 6f6d 2077 6869  osition from whi
+0000ec70: 6368 2074 6f20 7375 6273 6372 6962 652e  ch to subscribe.
+0000ec80: 2054 6865 2072 6563 6f72 6465 6420 6576   The recorded ev
+0000ec90: 656e 7420 6174 2074 6869 7320 7374 7265  ent at this stre
+0000eca0: 616d 0a70 6f73 6974 696f 6e20 7769 6c6c  am.position will
+0000ecb0: 2062 6520 7265 6365 6976 6564 2077 6865   be received whe
+0000ecc0: 6e20 7265 6164 696e 6720 7468 6520 7375  n reading the su
+0000ecd0: 6273 6372 6970 7469 6f6e 2e0a 0a54 6869  bscription...Thi
+0000ece0: 7320 6d65 7468 6f64 2068 6173 2061 6e20  s method has an 
+0000ecf0: 6f70 7469 6f6e 616c 2060 6672 6f6d 5f65  optional `from_e
+0000ed00: 6e64 6020 6172 6775 6d65 6e74 2c20 7768  nd` argument, wh
+0000ed10: 6963 6820 6973 2061 2050 7974 686f 6e20  ich is a Python 
+0000ed20: 6062 6f6f 6c60 2e0a 4279 2064 6566 6175  `bool`..By defau
+0000ed30: 6c74 2c20 7468 6520 7661 6c75 6520 6f66  lt, the value of
+0000ed40: 2074 6869 7320 6172 6775 6d65 6e74 2069   this argument i
+0000ed50: 7320 4661 6c73 652e 2049 6620 7468 6973  s False. If this
+0000ed60: 2061 7267 756d 656e 7420 6973 2073 6574   argument is set
+0000ed70: 0a74 6f20 6120 5472 7565 2076 616c 7565  .to a True value
+0000ed80: 2c20 7265 6164 696e 6720 6672 6f6d 2074  , reading from t
+0000ed90: 6865 2073 7562 7363 7269 7074 696f 6e20  he subscription 
+0000eda0: 7769 6c6c 2072 6563 6569 7665 206f 6e6c  will receive onl
+0000edb0: 7920 6576 656e 7473 0a72 6563 6f72 6465  y events.recorde
+0000edc0: 6420 6166 7465 7220 7468 6520 7375 6273  d after the subs
+0000edd0: 6372 6970 7469 6f6e 2077 6173 2063 7265  cription was cre
+0000ede0: 6174 6564 2e20 5468 6174 2069 732c 2069  ated. That is, i
+0000edf0: 7420 6973 206e 6f74 2069 6e63 6c75 7369  t is not inclusi
+0000ee00: 7665 0a6f 6620 7468 6520 6375 7272 656e  ve.of the curren
+0000ee10: 7420 7374 7265 616d 2070 6f73 6974 696f  t stream positio
+0000ee20: 6e2e 0a0a 5468 6973 206d 6574 686f 6420  n...This method 
+0000ee30: 616c 736f 2074 616b 6573 2061 6e20 6f70  also takes an op
+0000ee40: 7469 6f6e 616c 2060 7469 6d65 6f75 7460  tional `timeout`
+0000ee50: 2061 7267 756d 656e 742c 2074 6861 740a   argument, that.
+0000ee60: 6973 2065 7870 6563 7465 6420 746f 2062  is expected to b
+0000ee70: 6520 6120 5079 7468 6f6e 2060 666c 6f61  e a Python `floa
+0000ee80: 7460 2c20 7768 6963 6820 7365 7473 2061  t`, which sets a
+0000ee90: 2064 6561 646c 696e 650a 666f 7220 7468   deadline.for th
+0000eea0: 6520 636f 6d70 6c65 7469 6f6e 206f 6620  e completion of 
+0000eeb0: 7468 6520 6752 5043 206f 7065 7261 7469  the gRPC operati
+0000eec0: 6f6e 2e0a 0a54 6869 7320 6d65 7468 6f64  on...This method
+0000eed0: 2064 6f65 7320 6e6f 7420 7265 7475 726e   does not return
+0000eee0: 2061 2076 616c 7565 2e20 4576 656e 7473   a value. Events
+0000eef0: 2063 616e 2062 6520 7265 6365 6976 6564   can be received
+0000ef00: 2062 7920 6974 6572 6174 696e 670a 6f76   by iterating.ov
+0000ef10: 6572 2074 6865 2076 616c 7565 2072 6574  er the value ret
+0000ef20: 7572 6e65 6420 6279 2063 616c 6c69 6e67  urned by calling
+0000ef30: 2060 7265 6164 5f73 7472 6561 6d5f 7375   `read_stream_su
+0000ef40: 6273 6372 6970 7469 6f6e 2829 6020 2873  bscription()` (s
+0000ef50: 6565 2062 656c 6f77 292e 0a0a 5468 6520  ee below)...The 
+0000ef60: 6578 616d 706c 6520 6265 6c6f 7720 6372  example below cr
+0000ef70: 6561 7465 7320 6120 7065 7273 6973 7465  eates a persiste
+0000ef80: 6e74 2073 7472 6561 6d20 7375 6273 6372  nt stream subscr
+0000ef90: 6970 7469 6f6e 2066 726f 6d20 7468 6520  iption from the 
+0000efa0: 7374 6172 7420 6f66 2074 6865 2073 7472  start of the str
+0000efb0: 6561 6d2e 0a0a 6060 6070 7974 686f 6e0a  eam...```python.
+0000efc0: 2320 4372 6561 7465 2061 2070 6572 7369  # Create a persi
+0000efd0: 7374 656e 7420 7374 7265 616d 2073 7562  stent stream sub
+0000efe0: 7363 7269 7074 696f 6e20 6672 6f6d 2073  scription from s
+0000eff0: 7461 7274 206f 6620 7468 6520 7374 7265  tart of the stre
+0000f000: 616d 2e0a 6772 6f75 705f 6e61 6d65 3120  am..group_name1 
+0000f010: 3d20 6622 6772 6f75 702d 7b75 7569 6434  = f"group-{uuid4
+0000f020: 2829 7d22 0a63 6c69 656e 742e 6372 6561  ()}".client.crea
+0000f030: 7465 5f73 7472 6561 6d5f 7375 6273 6372  te_stream_subscr
+0000f040: 6970 7469 6f6e 280a 2020 2020 6772 6f75  iption(.    grou
+0000f050: 705f 6e61 6d65 3d67 726f 7570 5f6e 616d  p_name=group_nam
+0000f060: 6531 2c0a 2020 2020 7374 7265 616d 5f6e  e1,.    stream_n
+0000f070: 616d 653d 7374 7265 616d 5f6e 616d 6532  ame=stream_name2
+0000f080: 2c0a 290a 6060 600a 0a54 6865 2065 7861  ,.).```..The exa
+0000f090: 6d70 6c65 2062 656c 6f77 2063 7265 6174  mple below creat
+0000f0a0: 6573 2061 2070 6572 7369 7374 656e 7420  es a persistent 
+0000f0b0: 7374 7265 616d 2073 7562 7363 7269 7074  stream subscript
+0000f0c0: 696f 6e20 6672 6f6d 2061 2073 7472 6561  ion from a strea
+0000f0d0: 6d20 706f 7369 7469 6f6e 2e0a 0a60 6060  m position...```
+0000f0e0: 7079 7468 6f6e 0a23 2043 7265 6174 6520  python.# Create 
+0000f0f0: 6120 7065 7273 6973 7465 6e74 2073 7472  a persistent str
+0000f100: 6561 6d20 7375 6273 6372 6970 7469 6f6e  eam subscription
+0000f110: 2066 726f 6d20 6120 7374 7265 616d 2070   from a stream p
+0000f120: 6f73 6974 696f 6e2e 0a67 726f 7570 5f6e  osition..group_n
+0000f130: 616d 6532 203d 2066 2267 726f 7570 2d7b  ame2 = f"group-{
+0000f140: 7575 6964 3428 297d 220a 636c 6965 6e74  uuid4()}".client
+0000f150: 2e63 7265 6174 655f 7374 7265 616d 5f73  .create_stream_s
+0000f160: 7562 7363 7269 7074 696f 6e28 0a20 2020  ubscription(.   
+0000f170: 2067 726f 7570 5f6e 616d 653d 6772 6f75   group_name=grou
+0000f180: 705f 6e61 6d65 322c 0a20 2020 2073 7472  p_name2,.    str
+0000f190: 6561 6d5f 6e61 6d65 3d73 7472 6561 6d5f  eam_name=stream_
+0000f1a0: 6e61 6d65 322c 0a20 2020 2073 7472 6561  name2,.    strea
+0000f1b0: 6d5f 706f 7369 7469 6f6e 3d32 0a29 0a60  m_position=2.).`
+0000f1c0: 6060 0a0a 5468 6520 6578 616d 706c 6520  ``..The example 
+0000f1d0: 6265 6c6f 7720 6372 6561 7465 7320 6120  below creates a 
+0000f1e0: 7065 7273 6973 7465 6e74 2073 7472 6561  persistent strea
+0000f1f0: 6d20 7375 6273 6372 6970 7469 6f6e 2066  m subscription f
+0000f200: 726f 6d20 7468 6520 656e 6420 6f66 2074  rom the end of t
+0000f210: 6865 2073 7472 6561 6d2e 0a0a 6060 6070  he stream...```p
+0000f220: 7974 686f 6e0a 2320 4372 6561 7465 2061  ython.# Create a
+0000f230: 2070 6572 7369 7374 656e 7420 7374 7265   persistent stre
+0000f240: 616d 2073 7562 7363 7269 7074 696f 6e20  am subscription 
+0000f250: 6672 6f6d 2065 6e64 206f 6620 7468 6520  from end of the 
+0000f260: 7374 7265 616d 2e0a 6772 6f75 705f 6e61  stream..group_na
+0000f270: 6d65 3320 3d20 6622 6772 6f75 702d 7b75  me3 = f"group-{u
+0000f280: 7569 6434 2829 7d22 0a63 6c69 656e 742e  uid4()}".client.
+0000f290: 6372 6561 7465 5f73 7472 6561 6d5f 7375  create_stream_su
+0000f2a0: 6273 6372 6970 7469 6f6e 280a 2020 2020  bscription(.    
+0000f2b0: 6772 6f75 705f 6e61 6d65 3d67 726f 7570  group_name=group
+0000f2c0: 5f6e 616d 6533 2c0a 2020 2020 7374 7265  _name3,.    stre
+0000f2d0: 616d 5f6e 616d 653d 7374 7265 616d 5f6e  am_name=stream_n
+0000f2e0: 616d 6532 2c0a 2020 2020 6672 6f6d 5f65  ame2,.    from_e
+0000f2f0: 6e64 3d54 7275 650a 290a 6060 600a 0a23  nd=True.).```..#
+0000f300: 2323 2052 6561 6420 7374 7265 616d 2073  ## Read stream s
+0000f310: 7562 7363 7269 7074 696f 6e0a 0a54 6865  ubscription..The
+0000f320: 2060 7265 6164 5f73 7472 6561 6d5f 7375   `read_stream_su
+0000f330: 6273 6372 6970 7469 6f6e 2829 6020 6d65  bscription()` me
+0000f340: 7468 6f64 2063 616e 2062 6520 7573 6564  thod can be used
+0000f350: 2074 6f20 6372 6561 7465 2061 2070 6572   to create a per
+0000f360: 7369 7374 656e 740a 7375 6273 6372 6970  sistent.subscrip
+0000f370: 7469 6f6e 2066 6f72 2061 2073 7472 6561  tion for a strea
+0000f380: 6d2e 0a0a 5468 6973 206d 6574 686f 6420  m...This method 
+0000f390: 6861 7320 7477 6f20 7265 7175 6972 6564  has two required
+0000f3a0: 2061 7267 756d 656e 7473 2c20 6067 726f   arguments, `gro
+0000f3b0: 7570 5f6e 616d 6560 2061 6e64 2060 7374  up_name` and `st
+0000f3c0: 7265 616d 5f6e 616d 6560 2c20 7768 6963  ream_name`, whic
+0000f3d0: 680a 7368 6f75 6c64 206d 6174 6368 2074  h.should match t
+0000f3e0: 6865 2076 616c 7565 7320 6f66 2061 7267  he values of arg
+0000f3f0: 756d 656e 7473 2075 7365 6420 7768 656e  uments used when
+0000f400: 2063 616c 6c69 6e67 2060 6372 6561 7465   calling `create
+0000f410: 5f73 7472 6561 6d5f 7375 6273 6372 6970  _stream_subscrip
+0000f420: 7469 6f6e 2829 602e 0a0a 5468 6973 206d  tion()`...This m
+0000f430: 6574 686f 6420 616c 736f 2074 616b 6573  ethod also takes
+0000f440: 2061 6e20 6f70 7469 6f6e 616c 2060 7469   an optional `ti
+0000f450: 6d65 6f75 7460 2061 7267 756d 656e 742c  meout` argument,
+0000f460: 2074 6861 740a 6973 2065 7870 6563 7465   that.is expecte
+0000f470: 6420 746f 2062 6520 6120 5079 7468 6f6e  d to be a Python
+0000f480: 2060 666c 6f61 7460 2c20 7768 6963 6820   `float`, which 
+0000f490: 7365 7473 2061 2064 6561 646c 696e 650a  sets a deadline.
+0000f4a0: 666f 7220 7468 6520 636f 6d70 6c65 7469  for the completi
+0000f4b0: 6f6e 206f 6620 7468 6520 6752 5043 206f  on of the gRPC o
+0000f4c0: 7065 7261 7469 6f6e 2e0a 0a4a 7573 7420  peration...Just 
+0000f4d0: 6c69 6b65 2060 7265 6164 5f73 7562 7363  like `read_subsc
+0000f4e0: 7269 7074 696f 6e60 2c20 7468 6973 206d  ription`, this m
+0000f4f0: 6574 686f 6420 7265 7475 726e 7320 6120  ethod returns a 
+0000f500: 322d 7475 706c 653a 2061 2022 7265 6164  2-tuple: a "read
+0000f510: 2072 6571 7565 7374 2220 6f62 6a65 6374   request" object
+0000f520: 0a61 6e64 2061 2022 7265 6164 2072 6573  .and a "read res
+0000f530: 706f 6e73 6522 206f 626a 6563 742e 0a0a  ponse" object...
+0000f540: 6060 6070 7974 686f 6e0a 7265 6164 5f72  ```python.read_r
+0000f550: 6571 2c20 7265 6164 5f72 6573 7020 3d20  eq, read_resp = 
+0000f560: 636c 6965 6e74 2e72 6561 645f 7374 7265  client.read_stre
+0000f570: 616d 5f73 7562 7363 7269 7074 696f 6e28  am_subscription(
+0000f580: 0a20 2020 2067 726f 7570 5f6e 616d 653d  .    group_name=
+0000f590: 6772 6f75 705f 6e61 6d65 312c 0a20 2020  group_name1,.   
+0000f5a0: 2073 7472 6561 6d5f 6e61 6d65 3d73 7472   stream_name=str
+0000f5b0: 6561 6d5f 6e61 6d65 322c 0a29 0a60 6060  eam_name2,.).```
+0000f5c0: 0a0a 5468 6520 6578 616d 706c 6520 6265  ..The example be
+0000f5d0: 6c6f 7720 6974 6572 6174 6573 206f 7665  low iterates ove
+0000f5e0: 7220 7468 6520 2272 6561 6420 7265 7370  r the "read resp
+0000f5f0: 6f6e 7365 2220 6f62 6a65 6374 2c20 616e  onse" object, an
+0000f600: 6420 6361 6c6c 7320 6061 636b 2829 600a  d calls `ack()`.
+0000f610: 6f6e 2074 6865 2022 7265 6164 2072 6573  on the "read res
+0000f620: 706f 6e73 6522 206f 626a 6563 742e 2054  ponse" object. T
+0000f630: 6865 2066 6f72 206c 6f6f 7020 6272 6561  he for loop brea
+0000f640: 6b73 2077 6865 6e20 7765 2068 6176 6520  ks when we have 
+0000f650: 7265 6365 6976 6564 0a74 6865 206c 6173  received.the las
+0000f660: 7420 6576 656e 7420 696e 2074 6865 2073  t event in the s
+0000f670: 7472 6561 6d2c 2073 6f20 7468 6174 2077  tream, so that w
+0000f680: 6520 6361 6e20 6669 6e69 7368 2074 6865  e can finish the
+0000f690: 2065 7861 6d70 6c65 7320 696e 2074 6869   examples in thi
+0000f6a0: 730a 646f 6375 6d65 6e74 6174 696f 6e2e  s.documentation.
+0000f6b0: 0a0a 6060 6070 7974 686f 6e0a 6576 656e  ..```python.even
+0000f6c0: 7473 203d 205b 5d0a 666f 7220 6576 656e  ts = [].for even
+0000f6d0: 7420 696e 2072 6561 645f 7265 7370 3a0a  t in read_resp:.
+0000f6e0: 2020 2020 6576 656e 7473 2e61 7070 656e      events.appen
+0000f6f0: 6428 6576 656e 7429 0a0a 2020 2020 2320  d(event)..    # 
+0000f700: 4163 6b6e 6f77 6c65 6467 6520 7468 6520  Acknowledge the 
+0000f710: 7265 6365 6976 6564 2065 7665 6e74 2e0a  received event..
+0000f720: 2020 2020 7265 6164 5f72 6571 2e61 636b      read_req.ack
+0000f730: 2865 7665 6e74 5f69 643d 6576 656e 742e  (event_id=event.
+0000f740: 6964 290a 0a20 2020 2023 2042 7265 616b  id)..    # Break
+0000f750: 2077 6865 6e20 7468 6520 6c61 7374 2065   when the last e
+0000f760: 7665 6e74 2068 6173 2062 6565 6e20 7265  vent has been re
+0000f770: 6365 6976 6564 2e0a 2020 2020 6966 2065  ceived..    if e
+0000f780: 7665 6e74 2e69 6420 3d3d 2065 7665 6e74  vent.id == event
+0000f790: 3131 2e69 643a 0a20 2020 2020 2020 2062  11.id:.        b
+0000f7a0: 7265 616b 0a60 6060 0a0a 5765 2063 616e  reak.```..We can
+0000f7b0: 2063 6865 636b 2077 6520 7265 6365 6976   check we receiv
+0000f7c0: 6564 2061 6c6c 2074 6865 2065 7665 6e74  ed all the event
+0000f7d0: 7320 7468 6174 2077 6572 6520 6170 7065  s that were appe
+0000f7e0: 6e64 6564 2074 6f20 6073 7472 6561 6d5f  nded to `stream_
+0000f7f0: 6e61 6d65 3260 0a69 6e20 7468 6520 6578  name2`.in the ex
+0000f800: 616d 706c 6573 2061 626f 7665 2e0a 0a60  amples above...`
+0000f810: 6060 7079 7468 6f6e 0a61 7373 6572 7420  ``python.assert 
+0000f820: 6c65 6e28 6576 656e 7473 2920 3d3d 2034  len(events) == 4
+0000f830: 0a61 7373 6572 7420 6576 656e 7473 5b30  .assert events[0
+0000f840: 5d2e 7374 7265 616d 5f6e 616d 6520 3d3d  ].stream_name ==
+0000f850: 2073 7472 6561 6d5f 6e61 6d65 320a 6173   stream_name2.as
+0000f860: 7365 7274 2065 7665 6e74 735b 305d 2e69  sert events[0].i
+0000f870: 6420 3d3d 2065 7665 6e74 342e 6964 0a61  d == event4.id.a
+0000f880: 7373 6572 7420 6576 656e 7473 5b31 5d2e  ssert events[1].
+0000f890: 7374 7265 616d 5f6e 616d 6520 3d3d 2073  stream_name == s
+0000f8a0: 7472 6561 6d5f 6e61 6d65 320a 6173 7365  tream_name2.asse
+0000f8b0: 7274 2065 7665 6e74 735b 315d 2e69 6420  rt events[1].id 
+0000f8c0: 3d3d 2065 7665 6e74 352e 6964 0a61 7373  == event5.id.ass
+0000f8d0: 6572 7420 6576 656e 7473 5b32 5d2e 7374  ert events[2].st
+0000f8e0: 7265 616d 5f6e 616d 6520 3d3d 2073 7472  ream_name == str
+0000f8f0: 6561 6d5f 6e61 6d65 320a 6173 7365 7274  eam_name2.assert
+0000f900: 2065 7665 6e74 735b 325d 2e69 6420 3d3d   events[2].id ==
+0000f910: 2065 7665 6e74 362e 6964 0a61 7373 6572   event6.id.asser
+0000f920: 7420 6576 656e 7473 5b33 5d2e 7374 7265  t events[3].stre
+0000f930: 616d 5f6e 616d 6520 3d3d 2073 7472 6561  am_name == strea
+0000f940: 6d5f 6e61 6d65 320a 6173 7365 7274 2065  m_name2.assert e
+0000f950: 7665 6e74 735b 335d 2e69 6420 3d3d 2065  vents[3].id == e
+0000f960: 7665 6e74 3131 2e69 640a 6060 600a 0a23  vent11.id.```..#
+0000f970: 2323 2047 6574 2073 7472 6561 6d20 7375  ## Get stream su
+0000f980: 6273 6372 6970 7469 6f6e 2069 6e66 6f0a  bscription info.
+0000f990: 0a54 6865 2060 6765 745f 7374 7265 616d  .The `get_stream
+0000f9a0: 5f73 7562 7363 7269 7074 696f 6e5f 696e  _subscription_in
+0000f9b0: 666f 2829 6020 6d65 7468 6f64 2063 616e  fo()` method can
+0000f9c0: 2062 6520 7573 6564 2074 6f20 6765 7420   be used to get 
+0000f9d0: 696e 666f 726d 6174 696f 6e20 666f 7220  information for 
+0000f9e0: 610a 7065 7273 6973 7465 6e74 2073 7562  a.persistent sub
+0000f9f0: 7363 7269 7074 696f 6e20 666f 7220 6120  scription for a 
+0000fa00: 7374 7265 616d 2e0a 0a54 6869 7320 6d65  stream...This me
+0000fa10: 7468 6f64 2068 6173 2074 776f 2072 6571  thod has two req
+0000fa20: 7569 7265 6420 6172 6775 6d65 6e74 732c  uired arguments,
+0000fa30: 2060 6772 6f75 705f 6e61 6d65 6020 616e   `group_name` an
+0000fa40: 6420 6073 7472 6561 6d5f 6e61 6d65 602c  d `stream_name`,
+0000fa50: 2077 6869 6368 0a73 686f 756c 6420 6d61   which.should ma
+0000fa60: 7463 6820 7468 6520 7661 6c75 6573 206f  tch the values o
+0000fa70: 6620 6172 6775 6d65 6e74 7320 7573 6564  f arguments used
+0000fa80: 2077 6865 6e20 6361 6c6c 696e 6720 6063   when calling `c
+0000fa90: 7265 6174 655f 7374 7265 616d 5f73 7562  reate_stream_sub
+0000faa0: 7363 7269 7074 696f 6e28 2960 2e0a 0a54  scription()`...T
+0000fab0: 6869 7320 6d65 7468 6f64 2061 6c73 6f20  his method also 
+0000fac0: 7461 6b65 7320 616e 206f 7074 696f 6e61  takes an optiona
+0000fad0: 6c20 6074 696d 656f 7574 6020 6172 6775  l `timeout` argu
+0000fae0: 6d65 6e74 2c20 7468 6174 0a69 7320 6578  ment, that.is ex
+0000faf0: 7065 6374 6564 2074 6f20 6265 2061 2050  pected to be a P
+0000fb00: 7974 686f 6e20 6066 6c6f 6174 602c 2077  ython `float`, w
+0000fb10: 6869 6368 2073 6574 7320 6120 6465 6164  hich sets a dead
+0000fb20: 6c69 6e65 0a66 6f72 2074 6865 2063 6f6d  line.for the com
+0000fb30: 706c 6574 696f 6e20 6f66 2074 6865 2067  pletion of the g
+0000fb40: 5250 4320 6f70 6572 6174 696f 6e2e 0a0a  RPC operation...
+0000fb50: 6060 6070 7974 686f 6e0a 7375 6273 6372  ```python.subscr
+0000fb60: 6970 7469 6f6e 5f69 6e66 6f20 3d20 636c  iption_info = cl
+0000fb70: 6965 6e74 2e67 6574 5f73 7472 6561 6d5f  ient.get_stream_
+0000fb80: 7375 6273 6372 6970 7469 6f6e 5f69 6e66  subscription_inf
+0000fb90: 6f28 0a20 2020 2067 726f 7570 5f6e 616d  o(.    group_nam
+0000fba0: 653d 6772 6f75 705f 6e61 6d65 312c 0a20  e=group_name1,. 
+0000fbb0: 2020 2073 7472 6561 6d5f 6e61 6d65 3d73     stream_name=s
+0000fbc0: 7472 6561 6d5f 6e61 6d65 322c 0a29 0a60  tream_name2,.).`
+0000fbd0: 6060 0a0a 5468 6520 7265 7475 726e 6564  ``..The returned
+0000fbe0: 2076 616c 7565 2069 7320 6120 6053 7562   value is a `Sub
+0000fbf0: 7363 7269 7074 696f 6e49 6e66 6f60 206f  scriptionInfo` o
+0000fc00: 626a 6563 742e 0a0a 2323 2320 4c69 7374  bject...### List
+0000fc10: 2073 7472 6561 6d20 7375 6273 6372 6970   stream subscrip
+0000fc20: 7469 6f6e 730a 0a54 6865 2060 6c69 7374  tions..The `list
+0000fc30: 5f73 7472 6561 6d5f 7375 6273 6372 6970  _stream_subscrip
+0000fc40: 7469 6f6e 7328 2960 206d 6574 686f 6420  tions()` method 
+0000fc50: 6361 6e20 6265 2075 7365 6420 746f 2067  can be used to g
+0000fc60: 6574 2069 6e66 6f72 6d61 7469 6f6e 2066  et information f
+0000fc70: 6f72 2061 6c6c 0a74 6865 2070 6572 7369  or all.the persi
+0000fc80: 7374 656e 7420 7375 6273 6372 6970 7469  stent subscripti
+0000fc90: 6f6e 7320 666f 7220 6120 7374 7265 616d  ons for a stream
+0000fca0: 2e0a 0a54 6869 7320 6d65 7468 6f64 2068  ...This method h
+0000fcb0: 6173 206f 6e65 2072 6571 7569 7265 6420  as one required 
+0000fcc0: 6172 6775 6d65 6e74 2c20 6073 7472 6561  argument, `strea
+0000fcd0: 6d5f 6e61 6d65 602e 0a0a 5468 6973 206d  m_name`...This m
+0000fce0: 6574 686f 6420 616c 736f 2074 616b 6573  ethod also takes
+0000fcf0: 2061 6e20 6f70 7469 6f6e 616c 2060 7469   an optional `ti
+0000fd00: 6d65 6f75 7460 2061 7267 756d 656e 742c  meout` argument,
+0000fd10: 2074 6861 740a 6973 2065 7870 6563 7465   that.is expecte
+0000fd20: 6420 746f 2062 6520 6120 5079 7468 6f6e  d to be a Python
+0000fd30: 2060 666c 6f61 7460 2c20 7768 6963 6820   `float`, which 
+0000fd40: 7365 7473 2061 2064 6561 646c 696e 650a  sets a deadline.
+0000fd50: 666f 7220 7468 6520 636f 6d70 6c65 7469  for the completi
+0000fd60: 6f6e 206f 6620 7468 6520 6752 5043 206f  on of the gRPC o
+0000fd70: 7065 7261 7469 6f6e 2e0a 0a60 6060 7079  peration...```py
+0000fd80: 7468 6f6e 0a73 7562 7363 7269 7074 696f  thon.subscriptio
+0000fd90: 6e73 203d 2063 6c69 656e 742e 6c69 7374  ns = client.list
+0000fda0: 5f73 7472 6561 6d5f 7375 6273 6372 6970  _stream_subscrip
+0000fdb0: 7469 6f6e 7328 0a20 2020 2073 7472 6561  tions(.    strea
+0000fdc0: 6d5f 6e61 6d65 3d73 7472 6561 6d5f 6e61  m_name=stream_na
+0000fdd0: 6d65 322c 0a29 0a60 6060 0a0a 5468 6520  me2,.).```..The 
+0000fde0: 7265 7475 726e 6564 2076 616c 7565 2069  returned value i
+0000fdf0: 7320 6120 6c69 7374 206f 6620 6053 7562  s a list of `Sub
+0000fe00: 7363 7269 7074 696f 6e49 6e66 6f60 206f  scriptionInfo` o
+0000fe10: 626a 6563 7473 2e0a 0a23 2323 2044 656c  bjects...### Del
+0000fe20: 6574 6520 7374 7265 616d 2073 7562 7363  ete stream subsc
+0000fe30: 7269 7074 696f 6e0a 0a54 6865 2060 6465  ription..The `de
+0000fe40: 6c65 7465 5f73 7472 6561 6d5f 7375 6273  lete_stream_subs
+0000fe50: 6372 6970 7469 6f6e 2829 6020 6d65 7468  cription()` meth
+0000fe60: 6f64 2063 616e 2062 6520 7573 6564 2074  od can be used t
+0000fe70: 6f20 6465 6c65 7465 2061 2070 6572 7369  o delete a persi
+0000fe80: 7374 656e 740a 7375 6273 6372 6970 7469  stent.subscripti
+0000fe90: 6f6e 2066 6f72 2061 2073 7472 6561 6d2e  on for a stream.
+0000fea0: 0a0a 5468 6973 206d 6574 686f 6420 6861  ..This method ha
+0000feb0: 7320 7477 6f20 7265 7175 6972 6564 2061  s two required a
+0000fec0: 7267 756d 656e 7473 2c20 6067 726f 7570  rguments, `group
+0000fed0: 5f6e 616d 6560 2061 6e64 2060 7374 7265  _name` and `stre
+0000fee0: 616d 5f6e 616d 6560 2c20 7768 6963 680a  am_name`, which.
+0000fef0: 7368 6f75 6c64 206d 6174 6368 2074 6865  should match the
+0000ff00: 2076 616c 7565 7320 6f66 2061 7267 756d   values of argum
+0000ff10: 656e 7473 2075 7365 6420 7768 656e 2063  ents used when c
+0000ff20: 616c 6c69 6e67 2060 6372 6561 7465 5f73  alling `create_s
+0000ff30: 7472 6561 6d5f 7375 6273 6372 6970 7469  tream_subscripti
+0000ff40: 6f6e 2829 602e 0a0a 5468 6973 206d 6574  on()`...This met
+0000ff50: 686f 6420 616c 736f 2074 616b 6573 2061  hod also takes a
+0000ff60: 6e20 6f70 7469 6f6e 616c 2060 7469 6d65  n optional `time
+0000ff70: 6f75 7460 2061 7267 756d 656e 742c 2074  out` argument, t
+0000ff80: 6861 740a 6973 2065 7870 6563 7465 6420  hat.is expected 
+0000ff90: 746f 2062 6520 6120 5079 7468 6f6e 2060  to be a Python `
+0000ffa0: 666c 6f61 7460 2c20 7768 6963 6820 7365  float`, which se
+0000ffb0: 7473 2061 2064 6561 646c 696e 650a 666f  ts a deadline.fo
+0000ffc0: 7220 7468 6520 636f 6d70 6c65 7469 6f6e  r the completion
+0000ffd0: 206f 6620 7468 6520 6752 5043 206f 7065   of the gRPC ope
+0000ffe0: 7261 7469 6f6e 2e0a 0a60 6060 7079 7468  ration...```pyth
+0000fff0: 6f6e 0a63 6c69 656e 742e 6465 6c65 7465  on.client.delete
+00010000: 5f73 7472 6561 6d5f 7375 6273 6372 6970  _stream_subscrip
+00010010: 7469 6f6e 280a 2020 2020 6772 6f75 705f  tion(.    group_
+00010020: 6e61 6d65 3d67 726f 7570 5f6e 616d 6531  name=group_name1
+00010030: 2c0a 2020 2020 7374 7265 616d 5f6e 616d  ,.    stream_nam
+00010040: 653d 7374 7265 616d 5f6e 616d 6532 2c0a  e=stream_name2,.
+00010050: 290a 6060 600a 0a23 2320 436f 6e6e 6563  ).```..## Connec
+00010060: 7469 6f6e 0a0a 2323 2320 5265 636f 6e6e  tion..### Reconn
+00010070: 6563 740a 0a54 6865 2060 7265 636f 6e6e  ect..The `reconn
+00010080: 6563 7428 2960 206d 6574 686f 6420 6361  ect()` method ca
+00010090: 6e20 6265 2075 7365 6420 746f 206d 616e  n be used to man
+000100a0: 7561 6c6c 7920 7265 636f 6e6e 6563 7420  ually reconnect 
+000100b0: 7468 6520 636c 6965 6e74 2074 6f20 610a  the client to a.
+000100c0: 7375 6974 6162 6c65 2045 7665 6e74 5374  suitable EventSt
+000100d0: 6f72 6544 4220 6e6f 6465 2e20 5468 6973  oreDB node. This
+000100e0: 206d 6574 686f 6420 7573 6573 2074 6865   method uses the
+000100f0: 2073 616d 6520 726f 7574 696e 652c 2066   same routine, f
+00010100: 6f72 2064 6973 636f 7665 7269 6e67 2074  or discovering t
+00010110: 6865 0a63 6c75 7374 6572 206e 6f64 6573  he.cluster nodes
+00010120: 2061 6e64 2063 6f6e 6e65 6374 696e 6720   and connecting 
+00010130: 746f 2061 2073 7569 7461 626c 6520 6e6f  to a suitable no
+00010140: 6465 2061 6363 6f72 6469 6e67 2074 6f20  de according to 
+00010150: 7468 6520 6e6f 6465 2070 7265 6665 7265  the node prefere
+00010160: 6e63 650a 7370 6563 6966 6965 6420 696e  nce.specified in
+00010170: 2074 6865 2063 6f6e 6e65 6374 696f 6e20   the connection 
+00010180: 7374 7269 6e67 2c20 7468 6174 2069 7320  string, that is 
+00010190: 7573 6564 2077 6865 6e20 7468 6520 636c  used when the cl
+000101a0: 6965 6e74 2069 730a 696e 7374 616e 7469  ient is.instanti
+000101b0: 6174 6564 2e20 5468 6973 206d 6574 686f  ated. This metho
+000101c0: 6420 6973 2074 6872 6561 642d 7361 6665  d is thread-safe
+000101d0: 2c20 616e 6420 6974 2069 7320 2263 6f6e  , and it is "con
+000101e0: 7365 7276 6174 6976 6522 0a69 6e20 7468  servative".in th
+000101f0: 6174 206f 6e6c 7920 6f6e 6520 7265 636f  at only one reco
+00010200: 6e6e 6563 7469 6f6e 2077 696c 6c20 6f63  nnection will oc
+00010210: 6375 722e 2043 6f6e 6375 7272 656e 7420  cur. Concurrent 
+00010220: 6174 7465 6d70 7473 2074 6f20 7265 636f  attempts to reco
+00010230: 6e6e 6563 740a 7769 6c6c 2062 6c6f 636b  nnect.will block
+00010240: 2075 6e74 696c 2074 6865 2063 6c69 656e   until the clien
+00010250: 7420 6861 7320 7265 636f 6e6e 6563 7465  t has reconnecte
+00010260: 6420 7375 6363 6573 7366 756c 6c79 2c20  d successfully, 
+00010270: 616e 6420 7468 656e 2074 6865 7920 7769  and then they wi
+00010280: 6c6c 0a61 6c6c 2072 6574 7572 6e20 6e6f  ll.all return no
+00010290: 726d 616c 6c79 2e0a 0a60 6060 7079 7468  rmally...```pyth
+000102a0: 6f6e 0a63 6c69 656e 742e 7265 636f 6e6e  on.client.reconn
+000102b0: 6563 7428 290a 6060 600a 0a41 6e20 6578  ect().```..An ex
+000102c0: 616d 706c 6520 6f66 2077 6865 6e20 6974  ample of when it
+000102d0: 206d 6967 6874 2062 6520 6465 7369 7261   might be desira
+000102e0: 626c 6520 746f 2072 6563 6f6e 6e65 6374  ble to reconnect
+000102f0: 206d 616e 7561 6c6c 7920 6973 2077 6865   manually is whe
+00010300: 6e20 2866 6f72 2070 6572 666f 726d 616e  n (for performan
+00010310: 6365 0a72 6561 736f 6e73 2920 7468 6520  ce.reasons) the 
+00010320: 6e6f 6465 2070 7265 6665 7265 6e63 6520  node preference 
+00010330: 6973 2066 6f72 2074 6865 2063 6c69 656e  is for the clien
+00010340: 7420 746f 2062 6520 636f 6e6e 6563 7465  t to be connecte
+00010350: 6420 746f 2061 2066 6f6c 6c6f 7765 7220  d to a follower 
+00010360: 6e6f 6465 2069 6e20 7468 650a 636c 7573  node in the.clus
+00010370: 7465 722c 2061 6e64 2c20 6166 7465 7220  ter, and, after 
+00010380: 6120 636c 7573 7465 7220 6c65 6164 6572  a cluster leader
+00010390: 2065 6c65 6374 696f 6e2c 2074 6865 2066   election, the f
+000103a0: 6f6c 6c6f 7765 7220 6e6f 6465 2062 6563  ollower node bec
+000103b0: 6f6d 6573 2061 206c 6561 6465 7220 6e6f  omes a leader no
+000103c0: 6465 2e0a 5265 636f 6e6e 6563 7469 6e67  de..Reconnecting
+000103d0: 2074 6f20 6120 666f 6c6c 6f77 6572 206e   to a follower n
+000103e0: 6f64 6520 696e 2074 6869 7320 6361 7365  ode in this case
+000103f0: 2069 7320 6375 7272 656e 746c 7920 6265   is currently be
+00010400: 796f 6e64 2074 6865 2063 6170 6162 696c  yond the capabil
+00010410: 6974 6965 7320 6f66 0a74 6869 7320 636c  ities of.this cl
+00010420: 6965 6e74 2c20 6275 7420 7468 6973 2062  ient, but this b
+00010430: 6568 6176 696f 7220 6d69 6768 7420 6265  ehavior might be
+00010440: 2069 6d70 6c65 6d65 6e74 6564 2069 6e20   implemented in 
+00010450: 6120 6675 7475 7265 2072 656c 6561 7365  a future release
+00010460: 2e0a 0a50 6c65 6173 6520 6e6f 7465 2c20  ...Please note, 
+00010470: 616c 6c20 7468 6520 636c 6965 6e74 206d  all the client m
+00010480: 6574 686f 6473 2075 7365 2061 6e20 6040  ethods use an `@
+00010490: 6175 746f 7265 636f 6e6e 6563 7460 2064  autoreconnect` d
+000104a0: 6563 6f72 6174 6f72 2028 7768 6963 6820  ecorator (which 
+000104b0: 6361 6c6c 7320 7468 650a 6072 6563 6f6e  calls the.`recon
+000104c0: 6e65 6374 2829 6020 6d65 7468 6f64 2920  nect()` method) 
+000104d0: 616e 6420 6120 6040 7265 7472 7960 2064  and a `@retry` d
+000104e0: 6563 6f72 6174 6f72 2074 6861 7420 7769  ecorator that wi
+000104f0: 6c6c 2072 6574 7279 206f 7065 7261 7469  ll retry operati
+00010500: 6f6e 7320 7468 6174 2066 6169 6c0a 6475  ons that fail.du
+00010510: 6520 746f 2063 6f6e 6e65 6374 6976 6974  e to connectivit
+00010520: 7920 6973 7375 6573 2e20 5468 6973 206d  y issues. This m
+00010530: 6561 6e73 2c20 666f 7220 6578 616d 706c  eans, for exampl
+00010540: 652c 2074 6861 7420 7768 656e 2074 6865  e, that when the
+00010550: 206e 6f64 6520 7072 6566 6572 656e 6365   node preference
+00010560: 0a69 7320 666f 7220 7468 6520 636c 6965  .is for the clie
+00010570: 6e74 2074 6f20 6265 2063 6f6e 6e65 6374  nt to be connect
+00010580: 6564 2074 6f20 6120 6c65 6164 6572 2028  ed to a leader (
+00010590: 7768 6963 6820 6973 2074 6865 2064 6566  which is the def
+000105a0: 6175 6c74 2920 616e 6420 7768 656e 2c20  ault) and when, 
+000105b0: 6166 7465 7220 610a 636c 7573 7465 7220  after a.cluster 
+000105c0: 6c65 6164 6572 2065 6c65 6374 696f 6e2c  leader election,
+000105d0: 2074 6865 206e 6f64 6520 746f 2077 6869   the node to whi
+000105e0: 6368 2074 6865 2063 6c69 656e 7420 6973  ch the client is
+000105f0: 2063 6f6e 6e65 6374 6564 2062 6563 6f6d   connected becom
+00010600: 6573 2061 2066 6f6c 6c6f 7765 722c 0a73  es a follower,.s
+00010610: 6f20 7468 6174 2077 7269 7465 206f 7065  o that write ope
+00010620: 7261 7469 6f6e 7320 7769 6c6c 2062 6567  rations will beg
+00010630: 696e 2074 6f20 6661 696c 2062 6563 6175  in to fail becau
+00010640: 7365 2074 6865 2063 6c69 656e 7420 6973  se the client is
+00010650: 206e 6f20 6c6f 6e67 6572 2063 6f6e 6e65   no longer conne
+00010660: 6374 6564 0a74 6f20 6120 6c65 6164 6572  cted.to a leader
+00010670: 2c20 7468 656e 2074 6865 2063 6c69 656e  , then the clien
+00010680: 7420 7769 6c6c 2061 7574 6f6d 6174 6963  t will automatic
+00010690: 616c 6c79 2072 6563 6f6e 6e65 6374 2074  ally reconnect t
+000106a0: 6f20 7468 6520 6e65 7720 6c65 6164 6572  o the new leader
+000106b0: 2061 6e64 2061 6c73 6f0a 7468 6520 636c   and also.the cl
+000106c0: 6965 6e74 2077 696c 6c20 7265 7472 7920  ient will retry 
+000106d0: 7468 6520 6661 696c 6564 2077 7269 7465  the failed write
+000106e0: 206f 7065 7261 7469 6f6e 732e 2054 6865   operations. The
+000106f0: 2063 6c69 656e 7420 616c 736f 2077 696c   client also wil
+00010700: 6c20 7265 636f 6e6e 6563 740a 6163 636f  l reconnect.acco
+00010710: 7264 696e 6720 746f 2074 6865 206e 6f64  rding to the nod
+00010720: 6520 7072 6566 6572 656e 6365 2077 6865  e preference whe
+00010730: 6e20 7468 6572 6520 6172 6520 636f 6e6e  n there are conn
+00010740: 6563 7469 7669 7479 2069 7373 7565 7320  ectivity issues 
+00010750: 6361 7573 696e 6720 7265 6164 0a6f 7065  causing read.ope
+00010760: 7261 7469 6f6e 7320 746f 2066 6169 6c20  rations to fail 
+00010770: 7769 7468 2074 6865 2063 7572 7265 6e74  with the current
+00010780: 2063 6f6e 6e65 6374 696f 6e2e 0a0a 506c   connection...Pl
+00010790: 6561 7365 2061 6c73 6f20 6e6f 7465 2c20  ease also note, 
+000107a0: 616e 2065 7665 6e74 2d70 726f 6365 7373  an event-process
+000107b0: 696e 6720 636f 6d70 6f6e 656e 7420 7468  ing component th
+000107c0: 6174 2075 7365 7320 6120 6361 7463 682d  at uses a catch-
+000107d0: 7570 2073 7562 7363 7269 7074 696f 6e20  up subscription 
+000107e0: 7769 6c6c 0a6e 6565 6420 746f 2062 6520  will.need to be 
+000107f0: 6d6f 6e69 746f 7265 6420 666f 7220 6572  monitored for er
+00010800: 726f 7273 2c20 616e 642c 2069 6620 6974  rors, and, if it
+00010810: 2066 6169 6c73 2061 6674 6572 2074 6865   fails after the
+00010820: 2073 7562 7363 7269 7074 696f 6e20 7374   subscription st
+00010830: 6172 7465 642c 2069 740a 7769 6c6c 206e  arted, it.will n
+00010840: 6565 6420 746f 2062 6520 7265 7374 6172  eed to be restar
+00010850: 7465 6420 6672 6f6d 2074 6865 206c 6173  ted from the las
+00010860: 7420 7361 7665 6420 636f 6d6d 6974 2070  t saved commit p
+00010870: 6f73 6974 696f 6e2e 2049 6e20 7468 6973  osition. In this
+00010880: 2063 6173 652c 2074 6865 0a63 6c69 656e   case, the.clien
+00010890: 7420 7769 6c6c 2061 7574 6f6d 6174 6963  t will automatic
+000108a0: 616c 6c79 2072 6563 6f6e 6e65 6374 2074  ally reconnect t
+000108b0: 6f20 6120 6e6f 6465 2069 6e20 7468 6520  o a node in the 
+000108c0: 636c 7573 7465 7220 7768 656e 2074 6865  cluster when the
+000108d0: 2073 7562 7365 7175 656e 7420 6361 6c6c   subsequent call
+000108e0: 0a74 6f20 7374 6172 7420 6120 6361 7463  .to start a catc
+000108f0: 682d 7570 2073 7562 7363 7269 7074 696f  h-up subscriptio
+00010900: 6e20 6973 206d 6164 652e 2059 6f75 206a  n is made. You j
+00010910: 7573 7420 6e65 6564 2074 6f20 6361 7463  ust need to catc
+00010920: 6820 7468 6520 6572 726f 722c 2072 6561  h the error, rea
+00010930: 640a 7468 6520 6c61 7374 2073 6176 6564  d.the last saved
+00010940: 2063 6f6d 6d69 7420 706f 7369 7469 6f6e   commit position
+00010950: 2c20 616e 6420 7265 7374 6172 7420 7468  , and restart th
+00010960: 6520 6576 656e 7420 7072 6f63 6573 7369  e event processi
+00010970: 6e67 2c20 7573 696e 6720 7468 6520 7361  ng, using the sa
+00010980: 6d65 0a60 4553 4442 436c 6965 6e74 6020  me.`ESDBClient` 
+00010990: 696e 7374 616e 6365 2c20 6275 7420 7769  instance, but wi
+000109a0: 7468 2061 206e 6577 2063 616c 6c20 746f  th a new call to
+000109b0: 2060 7375 6273 6372 6962 655f 616c 6c5f   `subscribe_all_
+000109c0: 6576 656e 7473 2829 602e 0a0a 0a23 2323  events()`....###
+000109d0: 2043 6c6f 7365 0a0a 5468 6520 6063 6c6f   Close..The `clo
+000109e0: 7365 2829 6020 6d65 7468 6f64 2063 616e  se()` method can
+000109f0: 2062 6520 7573 6564 2074 6f20 636c 6561   be used to clea
+00010a00: 6e6c 7920 636c 6f73 6520 7468 6520 6752  nly close the gR
+00010a10: 5043 2063 6f6e 6e65 6374 696f 6e2e 0a0a  PC connection...
+00010a20: 6060 6070 7974 686f 6e0a 636c 6965 6e74  ```python.client
+00010a30: 2e63 6c6f 7365 2829 0a60 6060 0a0a 2323  .close().```..##
+00010a40: 204e 6f74 6573 0a0a 2323 2320 436f 6e6e   Notes..### Conn
+00010a50: 6563 7469 6f6e 2073 7472 696e 6773 0a0a  ection strings..
+00010a60: 5468 6520 4576 656e 7453 746f 7265 4442  The EventStoreDB
+00010a70: 2063 6f6e 6e65 6374 696f 6e20 7374 7269   connection stri
+00010a80: 6e67 2069 7320 6120 5552 4920 7468 6174  ng is a URI that
+00010a90: 2063 6f6e 666f 726d 7320 7769 7468 206f   conforms with o
+00010aa0: 6e65 206f 6620 7477 6f20 706f 7373 6962  ne of two possib
+00010ab0: 6c65 0a73 6368 656d 6573 2c20 6569 7468  le.schemes, eith
+00010ac0: 6572 2074 6865 2022 6573 6462 2220 7363  er the "esdb" sc
+00010ad0: 6865 6d65 206f 7220 7468 6520 2265 7364  heme or the "esd
+00010ae0: 622b 6469 7363 6f76 6572 2220 7363 6865  b+discover" sche
+00010af0: 6d65 2e20 5468 6520 7379 6e74 6178 2061  me. The syntax a
+00010b00: 6e64 0a73 656d 616e 7469 6373 206f 6620  nd.semantics of 
+00010b10: 7468 6520 4576 656e 7453 746f 7265 4442  the EventStoreDB
+00010b20: 2055 5249 2073 6368 656d 6573 2061 7265   URI schemes are
+00010b30: 2065 7870 6c61 696e 6564 2062 656c 6f77   explained below
+00010b40: 2e20 5468 6520 7379 6e74 6178 2069 730a  . The syntax is.
+00010b50: 6465 6669 6e65 6420 7573 696e 6720 5b45  defined using [E
+00010b60: 424e 465d 2868 7474 7073 3a2f 2f65 6e2e  BNF](https://en.
+00010b70: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
+00010b80: 6b69 2f45 7874 656e 6465 645f 4261 636b  ki/Extended_Back
+00010b90: 7573 e280 934e 6175 725f 666f 726d 292e  us...Naur_form).
+00010ba0: 0a0a 5468 6520 2265 7364 6222 2055 5249  ..The "esdb" URI
+00010bb0: 2073 6368 656d 6520 6361 6e20 6265 2064   scheme can be d
+00010bc0: 6566 696e 6564 2069 6e20 7468 6520 666f  efined in the fo
+00010bd0: 6c6c 6f77 696e 6720 7761 792e 0a0a 2020  llowing way...  
+00010be0: 2020 6573 6462 2d75 7269 203d 2022 6573    esdb-uri = "es
+00010bf0: 6462 3a2f 2f22 202c 205b 2075 7365 722d  db://" , [ user-
+00010c00: 696e 666f 202c 2022 4022 205d 202c 2067  info , "@" ] , g
+00010c10: 7270 632d 7461 7267 6574 2c20 7b20 222c  rpc-target, { ",
+00010c20: 2220 2c20 6772 7063 2d74 6172 6765 7420  " , grpc-target 
+00010c30: 7d20 2c20 5b20 223f 2220 2c20 7175 6572  } , [ "?" , quer
+00010c40: 792d 7374 7269 6e67 205d 203b 0a0a 496e  y-string ] ;..In
+00010c50: 2074 6865 2022 6573 6462 2220 5552 4920   the "esdb" URI 
+00010c60: 7363 6865 6d65 2c20 6166 7465 7220 7468  scheme, after th
+00010c70: 6520 6f70 7469 6f6e 616c 2075 7365 7220  e optional user 
+00010c80: 696e 666f 2073 7472 696e 672c 2074 6865  info string, the
+00010c90: 7265 206d 7573 7420 6265 2061 7420 6c65  re must be at le
+00010ca0: 6173 740a 6f6e 6520 6752 5043 2074 6172  ast.one gRPC tar
+00010cb0: 6765 742e 2049 6620 7468 6572 6520 6172  get. If there ar
+00010cc0: 6520 7365 7665 7261 6c20 6752 5043 2074  e several gRPC t
+00010cd0: 6172 6765 7473 2c20 7468 6579 206d 7573  argets, they mus
+00010ce0: 7420 6265 2073 6570 6172 6174 6564 2066  t be separated f
+00010cf0: 726f 6d20 6561 6368 0a6f 7468 6572 2077  rom each.other w
+00010d00: 6974 6820 7468 6520 222c 2220 6368 6172  ith the "," char
+00010d10: 6163 7465 722e 2045 6163 6820 6752 5043  acter. Each gRPC
+00010d20: 2074 6172 6765 7420 7368 6f75 6c64 2069   target should i
+00010d30: 6e64 6963 6174 6520 616e 2045 7665 6e74  ndicate an Event
+00010d40: 5374 6f72 6544 4220 6752 5043 0a73 6572  StoreDB gRPC.ser
+00010d50: 7665 7220 736f 636b 6574 2c20 6279 2073  ver socket, by s
+00010d60: 7065 6369 6679 696e 6720 6120 686f 7374  pecifying a host
+00010d70: 2061 6e64 2061 2070 6f72 7420 6e75 6d62   and a port numb
+00010d80: 6572 2073 6570 6172 6174 6564 2077 6974  er separated wit
+00010d90: 6820 7468 6520 223a 2220 6368 6172 6163  h the ":" charac
+00010da0: 7465 722e 0a54 6865 2068 6f73 7420 6d61  ter..The host ma
+00010db0: 7920 6265 2061 2068 6f73 746e 616d 6520  y be a hostname 
+00010dc0: 7468 6174 2063 616e 2062 6520 7265 736f  that can be reso
+00010dd0: 6c76 6564 2074 6f20 616e 2049 5020 6164  lved to an IP ad
+00010de0: 6472 6573 732c 206f 7220 616e 2049 5020  dress, or an IP 
+00010df0: 6164 6472 6573 732e 0a0a 2020 2020 6772  address...    gr
+00010e00: 7063 2d74 6172 6765 7420 3d20 2820 686f  pc-target = ( ho
+00010e10: 7374 6e61 6d65 207c 2069 702d 6164 6472  stname | ip-addr
+00010e20: 6573 7320 2920 2c20 223a 2220 2c20 706f  ess ) , ":" , po
+00010e30: 7274 2d6e 756d 6265 7220 3b0a 0a0a 5468  rt-number ;...Th
+00010e40: 6520 2265 7364 622b 6469 7363 6f76 6572  e "esdb+discover
+00010e50: 2220 5552 4920 7363 6865 6d65 2063 616e  " URI scheme can
+00010e60: 2062 6520 6465 6669 6e65 6420 696e 2074   be defined in t
+00010e70: 6865 2066 6f6c 6c6f 7769 6e67 2077 6179  he following way
+00010e80: 2e0a 0a20 2020 2065 7364 622d 6469 7363  ...    esdb-disc
+00010e90: 6f76 6572 2d75 7269 203d 2022 6573 6462  over-uri = "esdb
+00010ea0: 2b64 6973 636f 7665 723a 2f2f 2220 2c20  +discover://" , 
+00010eb0: 5b20 7573 6572 2d69 6e66 6f2c 2022 4022  [ user-info, "@"
+00010ec0: 205d 202c 2063 6c75 7374 6572 2d64 6f6d   ] , cluster-dom
+00010ed0: 6169 6e6e 616d 6520 2c20 5b20 223f 2220  ainname , [ "?" 
+00010ee0: 2c20 7175 6572 792d 7374 7269 6e67 205d  , query-string ]
+00010ef0: 203b 0a0a 496e 2074 6865 2022 6573 6462   ;..In the "esdb
+00010f00: 2b64 6973 636f 7665 7222 2055 5249 2073  +discover" URI s
+00010f10: 6368 656d 652c 2061 6674 6572 2074 6865  cheme, after the
+00010f20: 2075 7365 7220 696e 666f 2073 7472 696e   user info strin
+00010f30: 672c 2074 6865 7265 206d 7573 7420 6265  g, there must be
+00010f40: 2061 2064 6f6d 6169 6e0a 6e61 6d65 2077   a domain.name w
+00010f50: 6869 6368 2073 686f 756c 6420 6964 656e  hich should iden
+00010f60: 7469 6679 2061 2063 6c75 7374 6572 206f  tify a cluster o
+00010f70: 6620 4576 656e 7453 746f 7265 4442 2073  f EventStoreDB s
+00010f80: 6572 7665 7273 2e20 5468 6520 636c 6965  ervers. The clie
+00010f90: 6e74 2077 696c 6c20 7573 6520 6120 444e  nt will use a DN
+00010fa0: 530a 7365 7276 6572 2074 6f20 7265 736f  S.server to reso
+00010fb0: 6c76 6520 7468 6520 646f 6d61 696e 206e  lve the domain n
+00010fc0: 616d 6520 746f 2061 206c 6973 7420 6f66  ame to a list of
+00010fd0: 2061 6464 7265 7373 6573 206f 6620 4576   addresses of Ev
+00010fe0: 656e 7453 746f 7265 4442 2073 6572 7665  entStoreDB serve
+00010ff0: 7273 2c0a 6279 2071 7565 7279 696e 6720  rs,.by querying 
+00011000: 666f 7220 2741 2720 7265 636f 7264 732e  for 'A' records.
+00011010: 2049 6e20 7468 6973 2063 6173 652c 2074   In this case, t
+00011020: 6865 2070 6f72 7420 6e75 6d62 6572 2022  he port number "
+00011030: 3231 3133 2220 7769 6c6c 2062 6520 7573  2113" will be us
+00011040: 6564 2074 6f0a 636f 6e73 7472 7563 7420  ed to.construct 
+00011050: 6752 5043 2074 6172 6765 7473 2066 726f  gRPC targets fro
+00011060: 6d20 7468 6520 6164 6472 6573 7365 7320  m the addresses 
+00011070: 6f62 7461 696e 6564 2066 726f 6d20 2741  obtained from 'A
+00011080: 2720 7265 636f 7264 7320 7072 6f76 6964  ' records provid
+00011090: 6564 2062 7920 7468 650a 444e 5320 7365  ed by the.DNS se
+000110a0: 7276 6572 2e20 5468 6572 6566 6f72 652c  rver. Therefore,
+000110b0: 2069 6620 796f 7520 7761 6e74 2074 6f20   if you want to 
+000110c0: 7573 6520 7468 6520 2265 7364 622b 6469  use the "esdb+di
+000110d0: 7363 6f76 6572 2220 5552 4920 7363 6865  scover" URI sche
+000110e0: 6d65 2c20 796f 7520 7769 6c6c 0a6e 6565  me, you will.nee
+000110f0: 6420 746f 2063 6f6e 6669 6775 7265 2044  d to configure D
+00011100: 4e53 2077 6865 6e20 7365 7474 696e 6720  NS when setting 
+00011110: 7570 2079 6f75 7220 4576 656e 7453 746f  up your EventSto
+00011120: 7265 4442 2063 6c75 7374 6572 2e0a 0a57  reDB cluster...W
+00011130: 6974 6820 626f 7468 2074 6865 2022 6573  ith both the "es
+00011140: 6462 2220 616e 6420 2265 7364 622b 6469  db" and "esdb+di
+00011150: 736f 6376 6572 2220 5552 4920 7363 6865  socver" URI sche
+00011160: 6d65 732c 2074 6865 2063 6c69 656e 7420  mes, the client 
+00011170: 6669 7273 746c 7920 6f62 7461 696e 730a  firstly obtains.
+00011180: 6120 6c69 7374 206f 6620 6752 5043 2074  a list of gRPC t
+00011190: 6172 6765 7473 3a20 6569 7468 6572 2064  argets: either d
+000111a0: 6972 6563 746c 7920 6672 6f6d 2022 6573  irectly from "es
+000111b0: 6462 2220 636f 6e6e 6563 7469 6f6e 2073  db" connection s
+000111c0: 7472 696e 6773 3b20 6f72 2069 6e64 6972  trings; or indir
+000111d0: 6563 746c 790a 6672 6f6d 2022 6573 6462  ectly.from "esdb
+000111e0: 2b64 6973 636f 7665 7222 2063 6f6e 6e65  +discover" conne
+000111f0: 6374 696f 6e20 7374 7269 6e67 7320 7669  ction strings vi
+00011200: 6120 444e 532e 2054 6869 7320 6c69 7374  a DNS. This list
+00011210: 206f 6620 7461 7267 6574 7320 6973 206b   of targets is k
+00011220: 6e6f 776e 2061 7320 7468 650a 2267 6f73  nown as the."gos
+00011230: 7369 7020 7365 6564 222e 2054 6865 2063  sip seed". The c
+00011240: 6c69 656e 7420 7769 6c6c 2074 6865 6e20  lient will then 
+00011250: 6174 7465 6d70 7420 746f 2063 6f6e 6e65  attempt to conne
+00011260: 6374 2074 6f20 6561 6368 2067 5250 4320  ct to each gRPC 
+00011270: 7461 7267 6574 2069 6e20 7475 726e 2c0a  target in turn,.
+00011280: 6174 7465 6d70 7469 6e67 2074 6f20 6361  attempting to ca
+00011290: 6c6c 2074 6865 2045 7665 6e74 5374 6f72  ll the EventStor
+000112a0: 6544 4220 476f 7373 6970 2041 5049 2074  eDB Gossip API t
+000112b0: 6f20 6f62 7461 696e 2069 6e66 6f72 6d61  o obtain informa
+000112c0: 7469 6f6e 2061 626f 7574 2074 6865 0a45  tion about the.E
+000112d0: 7665 6e74 5374 6f72 6544 4220 636c 7573  ventStoreDB clus
+000112e0: 7465 722e 2041 206d 656d 6265 7220 6f66  ter. A member of
+000112f0: 2074 6865 2063 6c75 7374 6572 2069 7320   the cluster is 
+00011300: 7365 6c65 6374 6564 2062 7920 7468 6520  selected by the 
+00011310: 636c 6965 6e74 2c20 6163 636f 7264 696e  client, accordin
+00011320: 670a 746f 2074 6865 2022 6e6f 6465 2070  g.to the "node p
+00011330: 7265 6665 7265 6e63 6522 206f 7074 696f  reference" optio
+00011340: 6e20 2873 6565 2062 656c 6f77 292e 2054  n (see below). T
+00011350: 6865 2063 6c69 656e 7420 6d61 7920 7468  he client may th
+00011360: 656e 206e 6565 6420 746f 2063 6c6f 7365  en need to close
+00011370: 2069 7473 0a63 6f6e 6e65 6374 696f 6e20   its.connection 
+00011380: 616e 6420 7265 636f 6e6e 6563 7420 746f  and reconnect to
+00011390: 2074 6865 2073 656c 6563 7465 6420 7365   the selected se
+000113a0: 7276 6572 2e0a 0a49 6e20 626f 7468 2074  rver...In both t
+000113b0: 6865 2022 6573 6462 2220 616e 6420 2265  he "esdb" and "e
+000113c0: 7364 622b 6469 7363 6f76 6572 2220 7363  sdb+discover" sc
+000113d0: 6865 6d65 732c 2074 6865 2055 5249 206d  hemes, the URI m
+000113e0: 6179 2069 6e63 6c75 6465 2061 2075 7365  ay include a use
+000113f0: 7220 696e 666f 2073 7472 696e 672e 0a49  r info string..I
+00011400: 6620 6974 2065 7869 7374 7320 696e 2074  f it exists in t
+00011410: 6865 2055 5249 2c20 7468 6520 7573 6572  he URI, the user
+00011420: 2069 6e66 6f20 7374 7269 6e67 206d 7573   info string mus
+00011430: 7420 6265 2073 6570 6172 6174 6564 2066  t be separated f
+00011440: 726f 6d20 7468 6520 7265 7374 206f 6620  rom the rest of 
+00011450: 7468 6520 5552 490a 7769 7468 2074 6865  the URI.with the
+00011460: 2022 4022 2063 6861 7261 6374 6572 2e20   "@" character. 
+00011470: 5468 6520 7573 6572 2069 6e66 6f20 7374  The user info st
+00011480: 7269 6e67 206d 7573 7420 696e 636c 7564  ring must includ
+00011490: 6520 6120 7573 6572 6e61 6d65 2061 6e64  e a username and
+000114a0: 2061 2070 6173 7377 6f72 642c 0a73 6570   a password,.sep
+000114b0: 6172 6174 6564 2077 6974 6820 7468 6520  arated with the 
+000114c0: 223a 2220 6368 6172 6163 7465 722e 0a0a  ":" character...
+000114d0: 2020 2020 7573 6572 2d69 6e66 6f20 3d20      user-info = 
+000114e0: 7573 6572 6e61 6d65 202c 2022 3a22 202c  username , ":" ,
+000114f0: 2070 6173 7377 6f72 6420 3b0a 0a54 6865   password ;..The
+00011500: 2075 7365 7220 696e 666f 2069 7320 7365   user info is se
+00011510: 6e74 2062 7920 7468 6520 636c 6965 6e74  nt by the client
+00011520: 2061 7320 2263 616c 6c20 6372 6564 656e   as "call creden
+00011530: 7469 616c 7322 2069 6e20 6561 6368 2063  tials" in each c
+00011540: 616c 6c20 746f 2061 2022 7365 6375 7265  all to a "secure
+00011550: 220a 7365 7276 6572 2c20 696e 2061 2022  ".server, in a "
+00011560: 6261 7369 6320 6175 7468 2220 6175 7468  basic auth" auth
+00011570: 6f72 697a 6174 696f 6e20 6865 6164 6572  orization header
+00011580: 2e20 5468 6973 2061 7574 686f 7269 7a61  . This authoriza
+00011590: 7469 6f6e 2068 6561 6465 7220 6973 2075  tion header is u
+000115a0: 7365 6420 6279 0a74 6865 2073 6572 7665  sed by.the serve
+000115b0: 7220 746f 2061 7574 6865 6e74 6963 6174  r to authenticat
+000115c0: 6520 7468 6520 636c 6965 6e74 2e20 5468  e the client. Th
+000115d0: 6520 6175 7468 6f72 697a 6174 696f 6e20  e authorization 
+000115e0: 6865 6164 6572 2069 7320 6e6f 7420 7365  header is not se
+000115f0: 6e74 2074 6f0a 2269 6e73 6563 7572 6522  nt to."insecure"
+00011600: 2073 6572 7665 7273 2e0a 0a49 6e20 626f   servers...In bo
+00011610: 7468 2074 6865 2022 6573 6462 2220 616e  th the "esdb" an
+00011620: 6420 2265 7364 622b 6469 7363 6f76 6572  d "esdb+discover
+00011630: 2220 7363 6865 6d65 732c 2074 6865 206f  " schemes, the o
+00011640: 7074 696f 6e61 6c20 7175 6572 7920 7374  ptional query st
+00011650: 7269 6e67 206d 7573 7420 6265 206f 6e65  ring must be one
+00011660: 0a6f 7220 6d61 6e79 2066 6965 6c64 2d76  .or many field-v
+00011670: 616c 7565 2061 7267 756d 656e 7473 2c20  alue arguments, 
+00011680: 7365 7061 7261 7465 6420 6672 6f6d 2065  separated from e
+00011690: 6163 6820 6f74 6865 7220 7769 7468 2074  ach other with t
+000116a0: 6865 2022 2622 2063 6861 7261 6374 6572  he "&" character
+000116b0: 2e0a 0a20 2020 2071 7565 7279 2d73 7472  ...    query-str
+000116c0: 696e 6720 3d20 6669 656c 642d 7661 6c75  ing = field-valu
+000116d0: 652c 207b 2022 2622 2c20 6669 656c 642d  e, { "&", field-
+000116e0: 7661 6c75 6520 7d20 3b0a 0a45 6163 6820  value } ;..Each 
+000116f0: 6669 656c 642d 7661 6c75 6520 6172 6775  field-value argu
+00011700: 6d65 6e74 206d 7573 7420 6265 206f 6e65  ment must be one
+00011710: 206f 6620 7468 6520 7375 7070 6f72 7465   of the supporte
+00011720: 6420 6669 656c 6473 2c20 616e 6420 616e  d fields, and an
+00011730: 0a61 7070 726f 7072 6961 7465 2076 616c  .appropriate val
+00011740: 7565 2c20 7365 7061 7261 7465 6420 7769  ue, separated wi
+00011750: 7468 2074 6865 2022 3d22 2063 6861 7261  th the "=" chara
+00011760: 6374 6572 2e0a 0a20 2020 2066 6965 6c64  cter...    field
+00011770: 2d76 616c 7565 203d 2028 2022 546c 7322  -value = ( "Tls"
+00011780: 2c20 223d 2220 2c20 2274 7275 6522 207c  , "=" , "true" |
+00011790: 2022 6661 6c73 6522 2029 0a20 2020 2020   "false" ).     
+000117a0: 2020 2020 2020 2020 2020 207c 2028 2022             | ( "
+000117b0: 546c 7356 6572 6966 7943 6572 7422 2c20  TlsVerifyCert", 
+000117c0: 223d 2220 2c20 2274 7275 6522 207c 2022  "=" , "true" | "
+000117d0: 6661 6c73 6522 2029 0a20 2020 2020 2020  false" ).       
+000117e0: 2020 2020 2020 2020 207c 2028 2022 436f           | ( "Co
+000117f0: 6e6e 6563 7469 6f6e 4e61 6d65 222c 2022  nnectionName", "
+00011800: 3d22 202c 2073 7472 696e 6720 290a 2020  =" , string ).  
+00011810: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00011820: 2820 224e 6f64 6550 7265 6665 7265 6e63  ( "NodePreferenc
+00011830: 6522 2c20 223d 2220 2c20 226c 6561 6465  e", "=" , "leade
+00011840: 7222 207c 2022 666f 6c6c 6f77 6572 2220  r" | "follower" 
+00011850: 7c20 2272 6561 646f 6e6c 7972 6570 6c69  | "readonlyrepli
+00011860: 6361 2220 7c20 2272 616e 646f 6d22 2029  ca" | "random" )
+00011870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011880: 207c 2028 2022 4465 6661 756c 7444 6561   | ( "DefaultDea
+00011890: 646c 696e 6522 2c20 223d 2220 2c20 696e  dline", "=" , in
+000118a0: 7465 6765 7220 290a 2020 2020 2020 2020  teger ).        
+000118b0: 2020 2020 2020 2020 7c20 2820 2247 6f73          | ( "Gos
+000118c0: 7369 7054 696d 656f 7574 222c 2022 3d22  sipTimeout", "="
+000118d0: 202c 2069 6e74 6567 6572 2029 0a20 2020   , integer ).   
+000118e0: 2020 2020 2020 2020 2020 2020 207c 2028               | (
+000118f0: 2022 4d61 7844 6973 636f 7665 7241 7474   "MaxDiscoverAtt
+00011900: 656d 7074 7322 2c20 223d 2220 2c20 696e  empts", "=" , in
+00011910: 7465 6765 7220 290a 2020 2020 2020 2020  teger ).        
+00011920: 2020 2020 2020 2020 7c20 2820 2244 6973          | ( "Dis
+00011930: 636f 7665 7279 496e 7465 7276 616c 222c  coveryInterval",
+00011940: 2022 3d22 202c 2069 6e74 6567 6572 2029   "=" , integer )
+00011950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011960: 207c 2028 2022 4d61 7844 6973 636f 7665   | ( "MaxDiscove
+00011970: 7241 7474 656d 7074 7322 2c20 223d 2220  rAttempts", "=" 
+00011980: 2c20 696e 7465 6765 7220 290a 2020 2020  , integer ).    
+00011990: 2020 2020 2020 2020 2020 2020 7c20 2820              | ( 
+000119a0: 224b 6565 7041 6c69 7665 496e 7465 7276  "KeepAliveInterv
+000119b0: 616c 222c 2022 3d22 202c 2069 6e74 6567  al", "=" , integ
+000119c0: 6572 2029 0a20 2020 2020 2020 2020 2020  er ).           
+000119d0: 2020 2020 207c 2028 2022 4b65 6570 416c       | ( "KeepAl
+000119e0: 6976 6549 6e74 6572 7661 6c22 2c20 223d  iveInterval", "=
+000119f0: 2220 2c20 696e 7465 6765 7220 2920 3b0a  " , integer ) ;.
+00011a00: 0a54 6865 2074 6162 6c65 2062 656c 6f77  .The table below
+00011a10: 2064 6573 6372 6962 6573 2074 6865 2071   describes the q
+00011a20: 7565 7279 2066 6965 6c64 2d76 616c 7565  uery field-value
+00011a30: 7320 7375 7070 6f72 7465 6420 6279 2074  s supported by t
+00011a40: 6869 7320 636c 6965 6e74 2e0a 0a7c 2046  his client...| F
+00011a50: 6965 6c64 2020 2020 2020 2020 2020 2020  ield            
+00011a60: 2020 207c 2056 616c 7565 2020 2020 2020     | Value      
+00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011aa0: 2020 2020 2020 2020 2020 207c 2044 6573             | Des
+00011ab0: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
+00011ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b40: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00011b50: 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .|--------------
+00011b60: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
+00011b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00011bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011c50: 2d2d 2d7c 0a7c 2054 6c73 2020 2020 2020  ---|.| Tls      
+00011c60: 2020 2020 2020 2020 2020 207c 2022 7472             | "tr
+00011c70: 7565 222c 2022 6661 6c73 6522 2028 6465  ue", "false" (de
+00011c80: 6661 756c 743a 2022 7472 7565 2229 2020  fault: "true")  
+00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cb0: 2020 207c 2049 6620 2274 7275 6522 2074     | If "true" t
+00011cc0: 6865 2063 6c69 656e 7420 7769 6c6c 2063  he client will c
+00011cd0: 7265 6174 6520 6120 2273 6563 7572 6522  reate a "secure"
+00011ce0: 2067 5250 4320 6368 616e 6e65 6c2e 2049   gRPC channel. I
+00011cf0: 6620 2266 616c 7365 2220 7468 6520 636c  f "false" the cl
+00011d00: 6965 6e74 2077 696c 6c20 6372 6561 7465  ient will create
+00011d10: 2061 6e20 2269 6e73 6563 7572 6522 2067   an "insecure" g
+00011d20: 5250 4320 6368 616e 6e65 6c2e 2054 6869  RPC channel. Thi
+00011d30: 7320 6d75 7374 206d 6174 6368 2074 6865  s must match the
+00011d40: 2073 6572 7665 7220 636f 6e66 6967 7572   server configur
+00011d50: 6174 696f 6e2e 207c 0a7c 2054 6c73 5665  ation. |.| TlsVe
+00011d60: 7269 6679 4365 7274 2020 2020 2020 207c  rifyCert       |
+00011d70: 2022 7472 7565 222c 2022 6661 6c73 6522   "true", "false"
+00011d80: 2028 6465 6661 756c 743a 2022 7472 7565   (default: "true
+00011d90: 2229 2020 2020 2020 2020 2020 2020 2020  ")              
+00011da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011db0: 2020 2020 2020 207c 204e 4f54 2059 4554         | NOT YET
+00011dc0: 2049 4d50 4c45 4d45 4e54 4544 2020 2020   IMPLEMENTED    
+00011dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e50: 2020 2020 2020 2020 2020 207c 0a7c 2043             |.| C
+00011e60: 6f6e 6e65 6374 696f 6e4e 616d 6520 2020  onnectionName   
+00011e70: 2020 207c 2073 7472 696e 6720 2864 6566     | string (def
+00011e80: 6175 6c74 3a20 6175 746f 2d67 656e 6572  ault: auto-gener
+00011e90: 6174 6564 2076 6572 7369 6f6e 2d34 2055  ated version-4 U
+00011ea0: 5549 4429 2020 2020 2020 2020 2020 2020  UID)            
+00011eb0: 2020 2020 2020 2020 2020 207c 2053 656e             | Sen
+00011ec0: 7420 696e 2063 616c 6c20 6d65 7461 6461  t in call metada
+00011ed0: 7461 2066 6f72 2065 7665 7279 2063 616c  ta for every cal
+00011ee0: 6c2c 2074 6f20 6964 656e 7469 6679 2074  l, to identify t
+00011ef0: 6865 2063 6c69 656e 7420 746f 2074 6865  he client to the
+00011f00: 2063 6c75 7374 6572 2e20 2020 2020 2020   cluster.       
+00011f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00011f60: 0a7c 204e 6f64 6550 7265 6665 7265 6e63  .| NodePreferenc
+00011f70: 6520 2020 2020 207c 2022 6c65 6164 6572  e      | "leader
+00011f80: 222c 2022 666f 6c6c 6f77 6572 222c 2022  ", "follower", "
+00011f90: 7265 6164 6f6e 6c79 7265 706c 6963 6122  readonlyreplica"
+00011fa0: 2c20 2272 616e 646f 6d22 2028 6465 6661  , "random" (defa
+00011fb0: 756c 743a 2022 6c65 6164 6572 2229 207c  ult: "leader") |
+00011fc0: 2054 6865 206e 6f64 6520 7374 6174 6520   The node state 
+00011fd0: 7072 6566 6572 7265 6420 6279 2074 6865  preferred by the
+00011fe0: 2063 6c69 656e 742e 2054 6865 2063 6c69   client. The cli
+00011ff0: 656e 7420 7769 6c6c 2073 656c 6563 7420  ent will select 
+00012000: 6120 6e6f 6465 2066 726f 6d20 7468 6520  a node from the 
+00012010: 636c 7573 7465 7220 696e 666f 2072 6563  cluster info rec
+00012020: 6569 7665 6420 6672 6f6d 2074 6865 2047  eived from the G
+00012030: 6f73 7369 7020 4150 4920 6163 636f 7264  ossip API accord
+00012040: 696e 6720 746f 2074 6869 7320 7072 6566  ing to this pref
+00012050: 6572 656e 6365 2e20 2020 2020 2020 2020  erence.         
+00012060: 2020 207c 0a7c 2044 6566 6175 6c74 4465     |.| DefaultDe
+00012070: 6164 6c69 6e65 2020 2020 207c 2069 6e74  adline     | int
+00012080: 6567 6572 2028 6465 6661 756c 743a 2060  eger (default: `
+00012090: 4e6f 6e65 6029 2020 2020 2020 2020 2020  None`)          
+000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120c0: 2020 207c 2054 6865 2064 6566 6175 6c74     | The default
+000120d0: 2076 616c 7565 2028 696e 2073 6563 6f6e   value (in secon
+000120e0: 6473 2920 6f66 2074 6865 2060 7469 6d65  ds) of the `time
+000120f0: 6f75 7460 2061 7267 756d 656e 7420 6f66  out` argument of
+00012100: 2063 6c69 656e 7420 2277 7269 7465 2220   client "write" 
+00012110: 6d65 7468 6f64 7320 7375 6368 2061 7320  methods such as 
+00012120: 6061 7070 656e 645f 6576 656e 7473 2829  `append_events()
+00012130: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
+00012140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012160: 2020 2020 2020 207c 0a7c 2047 6f73 7369         |.| Gossi
+00012170: 7054 696d 656f 7574 2020 2020 2020 207c  pTimeout       |
+00012180: 2069 6e74 6567 6572 2028 6465 6661 756c   integer (defaul
+00012190: 743a 2035 2920 2020 2020 2020 2020 2020  t: 5)           
+000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121c0: 2020 2020 2020 207c 2054 6865 2064 6566         | The def
+000121d0: 6175 6c74 2076 616c 7565 2028 696e 2073  ault value (in s
+000121e0: 6563 6f6e 6473 2920 6f66 2074 6865 2060  econds) of the `
+000121f0: 7469 6d65 6f75 7460 2061 7267 756d 656e  timeout` argumen
+00012200: 7420 6f66 2067 6f73 7369 7020 7265 6164  t of gossip read
+00012210: 206d 6574 686f 6473 2c20 7375 6368 2061   methods, such a
+00012220: 7320 6072 6561 645f 676f 7373 6970 2829  s `read_gossip()
+00012230: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
+00012240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012260: 2020 2020 2020 2020 2020 207c 0a7c 204d             |.| M
+00012270: 6178 4469 7363 6f76 6572 4174 7465 6d70  axDiscoverAttemp
+00012280: 7473 207c 2069 6e74 6567 6572 2028 6465  ts | integer (de
+00012290: 6661 756c 743a 2031 3029 2020 2020 2020  fault: 10)      
+000122a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122c0: 2020 2020 2020 2020 2020 207c 2054 6865             | The
+000122d0: 206e 756d 6265 7220 6f66 2061 7474 656d   number of attem
+000122e0: 7074 7320 746f 2072 6561 6420 676f 7373  pts to read goss
+000122f0: 6970 2077 6865 6e20 636f 6e6e 6563 7469  ip when connecti
+00012300: 6e67 206f 7220 7265 636f 6e6e 6563 7469  ng or reconnecti
+00012310: 6e67 2074 6f20 6120 636c 7573 7465 7220  ng to a cluster 
+00012320: 6d65 6d62 6572 2e20 2020 2020 2020 2020  member.         
+00012330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012360: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00012370: 0a7c 2044 6973 636f 7665 7279 496e 7465  .| DiscoveryInte
+00012380: 7276 616c 2020 207c 2069 6e74 6567 6572  rval   | integer
+00012390: 2028 6465 6661 756c 743a 2031 3030 2920   (default: 100) 
+000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123c0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000123d0: 2048 6f77 206c 6f6e 6720 746f 2077 6169   How long to wai
+000123e0: 7420 2869 6e20 6d69 6c6c 6973 6563 6f6e  t (in millisecon
+000123f0: 6473 2920 6265 7477 6565 6e20 676f 7373  ds) between goss
+00012400: 6970 2072 6574 7269 6573 2e20 2020 2020  ip retries.     
+00012410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012470: 2020 207c 0a7c 204b 6565 7041 6c69 7665     |.| KeepAlive
+00012480: 496e 7465 7276 616c 2020 207c 2069 6e74  Interval   | int
+00012490: 6567 6572 2028 6465 6661 756c 743a 2060  eger (default: `
+000124a0: 4e6f 6e65 6029 2020 2020 2020 2020 2020  None`)          
+000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124d0: 2020 207c 2054 6865 2076 616c 7565 206f     | The value o
+000124e0: 6620 7468 6520 2267 7270 632e 6b65 6570  f the "grpc.keep
+000124f0: 616c 6976 655f 6d73 2220 6752 5043 2063  alive_ms" gRPC c
+00012500: 6861 6e6e 656c 206f 7074 696f 6e2e 2020  hannel option.  
+00012510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012570: 2020 2020 2020 207c 0a7c 204b 6565 7041         |.| KeepA
+00012580: 6c69 7665 5469 6d65 6f75 7420 2020 207c  liveTimeout    |
+00012590: 2069 6e74 6567 6572 2028 6465 6661 756c   integer (defaul
+000125a0: 743a 2060 4e6f 6e65 6029 2020 2020 2020  t: `None`)      
+000125b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125d0: 2020 2020 2020 207c 2054 6865 2076 616c         | The val
+000125e0: 7565 206f 6620 7468 6520 2267 7270 632e  ue of the "grpc.
+000125f0: 6b65 6570 616c 6976 655f 7469 6d65 6f75  keepalive_timeou
+00012600: 745f 6d73 2220 6752 5043 2063 6861 6e6e  t_ms" gRPC chann
+00012610: 656c 206f 7074 696f 6e2e 2020 2020 2020  el option.      
+00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012670: 2020 2020 2020 2020 2020 207c 0a0a 0a48             |...H
+00012680: 6572 6520 6172 6520 736f 6d65 2065 7861  ere are some exa
+00012690: 6d70 6c65 7320 6f66 2045 7665 6e74 5374  mples of EventSt
+000126a0: 6f72 6544 4220 636f 6e6e 6563 7469 6f6e  oreDB connection
+000126b0: 2073 7472 696e 6720 5552 4973 2e0a 0a20   string URIs... 
+000126c0: 2020 2023 2047 6574 2063 6c75 7374 6572     # Get cluster
+000126d0: 2069 6e66 6f20 6672 6f6d 2073 6563 7572   info from secur
+000126e0: 6520 7365 7276 6572 2073 6f63 6b65 7420  e server socket 
+000126f0: 6c6f 6361 6c68 6f73 743a 3231 3133 2c0a  localhost:2113,.
+00012700: 2020 2020 2320 616e 6420 7573 6520 2261      # and use "a
+00012710: 646d 696e 2220 616e 6420 2263 6861 6e67  dmin" and "chang
+00012720: 6569 7422 2061 7320 7573 6572 6e61 6d65  eit" as username
+00012730: 2061 6e64 2070 6173 7377 6f72 640a 2020   and password.  
+00012740: 2020 2320 7768 656e 206d 616b 696e 6720    # when making 
+00012750: 6361 6c6c 7320 746f 2045 7665 6e74 5374  calls to EventSt
+00012760: 6f72 6544 4220 4150 4920 6d65 7468 6f64  oreDB API method
+00012770: 732e 0a0a 2020 2020 6573 6462 3a2f 2f61  s...    esdb://a
+00012780: 646d 696e 3a63 6861 6e67 6569 7440 6c6f  dmin:changeit@lo
+00012790: 6361 6c68 6f73 743a 3231 3133 0a0a 0a20  calhost:2113... 
+000127a0: 2020 2023 2047 6574 2063 6c75 7374 6572     # Get cluster
+000127b0: 2069 6e66 6f20 6672 6f6d 2069 6e73 6563   info from insec
+000127c0: 7572 6520 7365 7276 6572 2073 6f63 6b65  ure server socke
+000127d0: 7420 3132 372e 302e 302e 313a 3231 3134  t 127.0.0.1:2114
+000127e0: 0a0a 2020 2020 6573 6462 3a2f 2f31 3237  ..    esdb://127
+000127f0: 2e30 2e30 2e31 3a32 3131 343f 546c 733d  .0.0.1:2114?Tls=
+00012800: 6661 6c73 650a 0a0a 2020 2020 2320 4765  false...    # Ge
+00012810: 7420 636c 7573 7465 7220 696e 666f 2066  t cluster info f
+00012820: 726f 6d20 6164 6472 6573 7365 7320 696e  rom addresses in
+00012830: 2027 4127 2072 6563 6f72 6473 2066 6f72   'A' records for
+00012840: 2063 6c75 7374 6572 312e 6578 616d 706c   cluster1.exampl
+00012850: 652e 636f 6d2c 0a20 2020 2023 2061 6e64  e.com,.    # and
+00012860: 2075 7365 2061 2064 6566 6175 6c74 2064   use a default d
+00012870: 6561 646c 696e 6520 666f 7220 6d61 6b69  eadline for maki
+00012880: 6e67 2063 616c 6c73 2074 6f20 4576 656e  ng calls to Even
+00012890: 7453 746f 7265 2041 5049 206d 6574 686f  tStore API metho
+000128a0: 642e 0a0a 2020 2020 6573 6462 2b64 6973  d...    esdb+dis
+000128b0: 636f 7665 723a 2f2f 6164 6d69 6e3a 6368  cover://admin:ch
+000128c0: 616e 6765 6974 4063 6c75 7374 6572 312e  angeit@cluster1.
+000128d0: 6578 616d 706c 652e 636f 6d3f 4465 6661  example.com?Defa
+000128e0: 756c 7444 6561 646c 696e 653d 350a 0a0a  ultDeadline=5...
+000128f0: 2020 2020 2320 4765 7420 636c 7573 7465      # Get cluste
+00012900: 7220 696e 666f 2066 726f 6d20 6569 7468  r info from eith
+00012910: 6572 206c 6f63 616c 686f 7374 3a32 3131  er localhost:211
+00012920: 3120 6f72 206c 6f63 616c 686f 7374 3a32  1 or localhost:2
+00012930: 3131 3220 6f72 0a20 2020 2023 206c 6f63  112 or.    # loc
+00012940: 616c 686f 7374 3a32 3131 332c 2061 6e64  alhost:2113, and
+00012950: 2074 6865 6e20 636f 6e6e 6563 7420 746f   then connect to
+00012960: 2061 2066 6f6c 6c6f 7765 7220 6e6f 6465   a follower node
+00012970: 2069 6e20 7468 6520 636c 7573 7465 722e   in the cluster.
+00012980: 0a0a 2020 2020 6573 6462 3a2f 2f61 646d  ..    esdb://adm
+00012990: 696e 3a63 6861 6e67 6569 7440 6c6f 6361  in:changeit@loca
+000129a0: 6c68 6f73 743a 3231 3131 2c6c 6f63 616c  lhost:2111,local
+000129b0: 686f 7374 3a32 3131 322c 6c6f 6361 6c68  host:2112,localh
+000129c0: 6f73 743a 3231 3133 3f4e 6f64 6550 7265  ost:2113?NodePre
+000129d0: 6665 7265 6e63 653d 666f 6c6c 6f77 6572  ference=follower
+000129e0: 0a0a 0a20 2020 2023 2047 6574 2063 6c75  ...    # Get clu
+000129f0: 7374 6572 2069 6e66 6f20 6672 6f6d 2061  ster info from a
+00012a00: 6464 7265 7373 6573 2069 6e20 2741 2720  ddresses in 'A' 
+00012a10: 7265 636f 7264 7320 666f 7220 636c 7573  records for clus
+00012a20: 7465 7231 2e65 7861 6d70 6c65 2e63 6f6d  ter1.example.com
+00012a30: 2c0a 2020 2020 2320 616e 6420 636f 6e66  ,.    # and conf
+00012a40: 6967 7572 6520 226b 6565 7020 616c 6976  igure "keep aliv
+00012a50: 6522 2074 696d 656f 7574 2061 6e64 2069  e" timeout and i
+00012a60: 6e74 6572 7661 6c20 696e 2074 6865 2067  nterval in the g
+00012a70: 5250 4320 6368 616e 6e65 6c2e 0a0a 2020  RPC channel...  
+00012a80: 2020 6573 6462 2b64 6973 636f 7665 723a    esdb+discover:
+00012a90: 2f2f 6164 6d69 6e3a 6368 616e 6765 6974  //admin:changeit
+00012aa0: 4063 6c75 7374 6572 312e 6578 616d 706c  @cluster1.exampl
+00012ab0: 652e 636f 6d3f 4b65 6570 416c 6976 6549  e.com?KeepAliveI
+00012ac0: 6e74 6572 7661 6c3d 3130 3030 3026 4b65  nterval=10000&Ke
+00012ad0: 6570 416c 6976 6554 696d 656f 7574 3d31  epAliveTimeout=1
+00012ae0: 3030 3030 0a0a 0a50 6c65 6173 6520 6e6f  0000...Please no
+00012af0: 7465 2c20 7468 6520 636c 6965 6e74 2069  te, the client i
+00012b00: 7320 696e 7365 6e73 6974 6976 6520 746f  s insensitive to
+00012b10: 2074 6865 2063 6173 6520 6f66 2066 6965   the case of fie
+00012b20: 6c64 7320 616e 6420 7661 6c75 6573 2e20  lds and values. 
+00012b30: 4966 2066 6965 6c64 7320 6172 650a 7265  If fields are.re
+00012b40: 7065 6174 6564 2069 6e20 7468 6520 7175  peated in the qu
+00012b50: 6572 7920 7374 7269 6e67 2c20 7468 6520  ery string, the 
+00012b60: 7175 6572 7920 7374 7269 6e67 2077 696c  query string wil
+00012b70: 6c20 6265 2070 6172 7365 6420 7769 7468  l be parsed with
+00012b80: 6f75 7420 6572 726f 722e 2048 6f77 6576  out error. Howev
+00012b90: 6572 2c0a 7468 6520 636f 6e6e 6563 7469  er,.the connecti
+00012ba0: 6f6e 206f 7074 696f 6e73 2075 7365 6420  on options used 
+00012bb0: 6279 2074 6865 2063 6c69 656e 7420 7769  by the client wi
+00012bc0: 6c6c 2075 7365 2074 6865 2076 616c 7565  ll use the value
+00012bd0: 206f 6620 7468 6520 6669 7273 7420 6669   of the first fi
+00012be0: 656c 642e 2041 6c6c 0a74 6865 206f 7468  eld. All.the oth
+00012bf0: 6572 2066 6965 6c64 2d76 616c 7565 7320  er field-values 
+00012c00: 696e 2074 6865 2071 7565 7279 2073 7472  in the query str
+00012c10: 696e 6720 7769 7468 2074 6865 2073 616d  ing with the sam
+00012c20: 6520 6669 656c 6420 6e61 6d65 2077 696c  e field name wil
+00012c30: 6c20 6265 2069 676e 6f72 6564 2e0a 4669  l be ignored..Fi
+00012c40: 656c 6473 2077 6974 686f 7574 2076 616c  elds without val
+00012c50: 7565 7320 7769 6c6c 2061 6c73 6f20 6265  ues will also be
+00012c60: 2069 676e 6f72 6564 2e0a 0a49 6620 7468   ignored...If th
+00012c70: 6520 636c 6965 6e74 2773 206e 6f64 6520  e client's node 
+00012c80: 7072 6566 6572 656e 6365 2069 7320 226c  preference is "l
+00012c90: 6561 6465 7222 2061 6e64 2074 6865 206e  eader" and the n
+00012ca0: 6f64 6520 6265 636f 6d65 7320 610a 2266  ode becomes a."f
+00012cb0: 6f6c 6c6f 7765 7222 2c20 7468 6520 636c  ollower", the cl
+00012cc0: 6965 6e74 2077 696c 6c20 6174 7465 6d70  ient will attemp
+00012cd0: 7420 746f 2072 6563 6f6e 6e65 6374 2074  t to reconnect t
+00012ce0: 6f20 7468 6520 6375 7272 656e 7420 6c65  o the current le
+00012cf0: 6164 6572 2077 6865 6e20 6120 6d65 7468  ader when a meth
+00012d00: 6f64 0a69 7320 6361 6c6c 6564 2074 6861  od.is called tha
+00012d10: 7420 6578 7065 6374 7320 746f 2063 616c  t expects to cal
+00012d20: 6c20 6120 6c65 6164 6572 2e20 4d65 7468  l a leader. Meth
+00012d30: 6f64 7320 7768 6963 6820 6d75 7461 7465  ods which mutate
+00012d40: 2074 6865 2073 7461 7465 206f 6620 7468   the state of th
+00012d50: 6520 6461 7461 6261 7365 0a65 7870 6563  e database.expec
+00012d60: 7420 746f 2063 616c 6c20 6120 6c65 6164  t to call a lead
+00012d70: 6572 2e20 466f 7220 7375 6368 206d 6574  er. For such met
+00012d80: 686f 6473 2c20 7468 6520 4854 5450 2068  hods, the HTTP h
+00012d90: 6561 6465 7222 7265 7175 6972 6573 2d6c  eader"requires-l
+00012da0: 6561 6465 7222 2069 7320 7365 7420 746f  eader" is set to
+00012db0: 0a22 7472 7565 222c 2061 6e64 2074 6869  ."true", and thi
+00012dc0: 7320 6865 6164 6572 2069 7320 6f62 7365  s header is obse
+00012dd0: 7276 6564 2062 7920 7468 6520 7365 7276  rved by the serv
+00012de0: 6572 2c20 616e 6420 736f 2061 206e 6f64  er, and so a nod
+00012df0: 6520 7768 6963 6820 6973 206e 6f74 2061  e which is not a
+00012e00: 206c 6561 6465 720a 7468 6174 2072 6563   leader.that rec
+00012e10: 6569 7665 7320 7375 6368 2061 2072 6571  eives such a req
+00012e20: 7565 7374 2077 696c 6c20 7265 7475 726e  uest will return
+00012e30: 2061 6e20 6572 726f 722e 2054 6869 7320   an error. This 
+00012e40: 6572 726f 7220 6973 2064 6574 6563 7465  error is detecte
+00012e50: 6420 6279 2074 6865 2063 6c69 656e 742c  d by the client,
+00012e60: 0a77 6869 6368 2077 696c 6c20 7468 656e  .which will then
+00012e70: 2063 6c6f 7365 2074 6865 2063 7572 7265   close the curre
+00012e80: 6e74 2067 5250 4320 636f 6e6e 6563 7469  nt gRPC connecti
+00012e90: 6f6e 2061 6e64 2063 7265 6174 6520 6120  on and create a 
+00012ea0: 6e65 7720 636f 6e6e 6563 7469 6f6e 2074  new connection t
+00012eb0: 6f20 7468 650a 6c65 6164 6572 2e20 5468  o the.leader. Th
+00012ec0: 6520 7265 7175 6573 7420 7769 6c6c 2074  e request will t
+00012ed0: 6865 6e20 6265 2072 6574 7269 6564 2077  hen be retried w
+00012ee0: 6974 6820 7468 6520 6c65 6164 6572 2e0a  ith the leader..
+00012ef0: 0a49 6620 7468 6520 636c 6965 6e74 2773  .If the client's
+00012f00: 206e 6f64 6520 7072 6566 6572 656e 6365   node preference
+00012f10: 2069 7320 2266 6f6c 6c6f 7765 7222 2061   is "follower" a
+00012f20: 6e64 2074 6865 7265 2061 7265 206e 6f20  nd there are no 
+00012f30: 666f 6c6c 6f77 6572 0a6e 6f64 6573 2069  follower.nodes i
+00012f40: 6e20 7468 6520 636c 7573 7465 722c 2074  n the cluster, t
+00012f50: 6865 6e20 7468 6520 636c 6965 6e74 2077  hen the client w
+00012f60: 696c 6c20 7261 6973 6520 616e 2065 7863  ill raise an exc
+00012f70: 6570 7469 6f6e 2e20 5369 6d69 6c61 726c  eption. Similarl
+00012f80: 792c 2069 6620 7468 650a 636c 6965 6e74  y, if the.client
+00012f90: 2773 206e 6f64 6520 7072 6566 6572 656e  's node preferen
+00012fa0: 6365 2069 7320 2272 6561 646f 6e6c 7972  ce is "readonlyr
+00012fb0: 6570 6c69 6361 2220 616e 6420 7468 6572  eplica" and ther
+00012fc0: 6520 6172 6520 6e6f 2072 6561 642d 6f6e  e are no read-on
+00012fd0: 6c79 2072 6570 6c69 6361 0a6e 6f64 6573  ly replica.nodes
+00012fe0: 2069 6e20 7468 6520 636c 7573 7465 722c   in the cluster,
+00012ff0: 2074 6865 6e20 7468 6520 636c 6965 6e74   then the client
+00013000: 2077 696c 6c20 616c 736f 2072 6169 7365   will also raise
+00013010: 2061 6e20 6578 6365 7074 696f 6e2e 0a0a   an exception...
+00013020: 5468 6520 6752 5043 2063 6861 6e6e 656c  The gRPC channel
+00013030: 206f 7074 696f 6e20 2267 7270 632e 6d61   option "grpc.ma
+00013040: 785f 7265 6365 6976 655f 6d65 7373 6167  x_receive_messag
+00013050: 655f 6c65 6e67 7468 2220 6973 2061 7574  e_length" is aut
+00013060: 6f6d 6174 6963 616c 6c79 0a63 6f6e 6669  omatically.confi
+00013070: 6775 7265 6420 746f 2074 6865 2076 616c  gured to the val
+00013080: 7565 2060 3137 202a 2031 3032 3420 2a20  ue `17 * 1024 * 
+00013090: 3130 3234 602e 2054 6869 7320 7661 6c75  1024`. This valu
+000130a0: 6520 6361 6e6e 6f74 2062 6520 6368 616e  e cannot be chan
+000130b0: 6765 642e 0a0a 0a23 2323 2052 6567 756c  ged....### Regul
+000130c0: 6172 2065 7870 7265 7373 696f 6e20 6669  ar expression fi
+000130d0: 6c74 6572 730a 0a54 6865 2066 696c 7465  lters..The filte
+000130e0: 7220 6172 6775 6d65 6e74 7320 696e 2060  r arguments in `
+000130f0: 7265 6164 5f61 6c6c 5f65 7665 6e74 7328  read_all_events(
+00013100: 2960 2c20 6073 7562 7363 7269 6265 5f61  )`, `subscribe_a
+00013110: 6c6c 5f65 7665 6e74 7328 2960 2c0a 6063  ll_events()`,.`c
+00013120: 7265 6174 655f 7375 6273 6372 6970 7469  reate_subscripti
+00013130: 6f6e 2829 6020 616e 6420 6063 6f6d 6d69  on()` and `commi
+00013140: 745f 706f 7369 7469 6f6e 2829 6020 6172  t_position()` ar
+00013150: 6520 6170 706c 6965 6420 746f 2074 6865  e applied to the
+00013160: 2060 7479 7065 600a 6174 7472 6962 7574   `type`.attribut
+00013170: 6520 6f66 2072 6563 6f72 6465 6420 6576  e of recorded ev
+00013180: 656e 7473 2e0a 0a54 6865 2064 6566 6175  ents...The defau
+00013190: 6c74 2076 616c 7565 206f 6620 7468 6520  lt value of the 
+000131a0: 6066 696c 7465 725f 6578 636c 7564 6560  `filter_exclude`
+000131b0: 2061 7267 756d 656e 7473 2069 7320 6465   arguments is de
+000131c0: 7369 676e 6564 2074 6f20 6578 636c 7564  signed to exclud
+000131d0: 650a 4576 656e 7453 746f 7265 4442 2022  e.EventStoreDB "
+000131e0: 7379 7374 656d 2220 616e 6420 2270 6572  system" and "per
+000131f0: 7369 7374 656e 6365 2073 7562 7363 7269  sistence subscri
+00013200: 7074 696f 6e20 636f 6e66 6967 2220 6576  ption config" ev
+00013210: 656e 7473 2c20 7768 6963 680a 6f74 6865  ents, which.othe
+00013220: 7277 6973 6520 776f 756c 6420 6265 2069  rwise would be i
+00013230: 6e63 6c75 6465 642e 2053 7973 7465 6d20  ncluded. System 
+00013240: 6576 656e 7473 2067 656e 6572 6174 6564  events generated
+00013250: 2062 7920 4576 656e 7453 746f 7265 4442   by EventStoreDB
+00013260: 2061 6c6c 0a68 6176 6520 6074 7970 6560   all.have `type`
+00013270: 2073 7472 696e 6773 2074 6861 7420 7374   strings that st
+00013280: 6172 7420 7769 7468 2074 6865 2060 2460  art with the `$`
+00013290: 2073 6967 6e2e 2050 6572 7369 7374 656e   sign. Persisten
+000132a0: 6365 2073 7562 7363 7269 7074 696f 6e0a  ce subscription.
+000132b0: 6576 656e 7473 2067 656e 6572 6174 6564  events generated
+000132c0: 2077 6865 6e20 6d61 6e69 7075 6c61 7469   when manipulati
+000132d0: 6e67 2070 6572 7369 7374 656e 6365 2073  ng persistence s
+000132e0: 7562 7363 7269 7074 696f 6e73 2061 6c6c  ubscriptions all
+000132f0: 2068 6176 6520 6074 7970 6560 0a73 7472   have `type`.str
+00013300: 696e 6773 2074 6861 7420 7374 6172 7420  ings that start 
+00013310: 7769 7468 2060 5065 7273 6973 7465 6e74  with `Persistent
+00013320: 436f 6e66 6967 602e 0a0a 466f 7220 6578  Config`...For ex
+00013330: 616d 706c 652c 2074 6f20 6d61 7463 6820  ample, to match 
+00013340: 7468 6520 7479 7065 206f 6620 4576 656e  the type of Even
+00013350: 7453 746f 7265 4442 2073 7973 7465 6d20  tStoreDB system 
+00013360: 6576 656e 7473 2c20 7573 6520 7468 6520  events, use the 
+00013370: 7265 6775 6c61 720a 6578 7072 6573 7369  regular.expressi
+00013380: 6f6e 2060 7227 5c24 2e2b 2760 2e20 506c  on `r'\$.+'`. Pl
+00013390: 6561 7365 206e 6f74 652c 2074 6865 2063  ease note, the c
+000133a0: 6f6e 7374 616e 7420 6045 5344 425f 5359  onstant `ESDB_SY
+000133b0: 5354 454d 5f45 5645 4e54 535f 5245 4745  STEM_EVENTS_REGE
+000133c0: 5860 2069 730a 7365 7420 746f 2060 7227  X` is.set to `r'
+000133d0: 5c24 2e2b 2760 2e20 596f 7520 6361 6e20  \$.+'`. You can 
+000133e0: 696d 706f 7274 2074 6869 7320 7661 6c75  import this valu
+000133f0: 650a 2860 6672 6f6d 2065 7364 6263 6c69  e.(`from esdbcli
+00013400: 656e 7420 696d 706f 7274 2045 5344 425f  ent import ESDB_
+00013410: 5359 5354 454d 5f45 5645 4e54 535f 5245  SYSTEM_EVENTS_RE
+00013420: 4745 5860 2920 616e 6420 7573 650a 6974  GEX`) and use.it
+00013430: 2077 6865 6e20 6275 696c 6469 6e67 206c   when building l
+00013440: 6f6e 6765 7220 7365 7175 656e 6365 7320  onger sequences 
+00013450: 6f66 2072 6567 756c 6172 2065 7870 7265  of regular expre
+00013460: 7373 696f 6e73 2e0a 0a53 696d 696c 6172  ssions...Similar
+00013470: 6c79 2c20 746f 206d 6174 6368 2074 6865  ly, to match the
+00013480: 2074 7970 6520 6f66 2045 7665 6e74 5374   type of EventSt
+00013490: 6f72 6544 4220 7065 7273 6973 7465 6e63  oreDB persistenc
+000134a0: 6520 7375 6273 6372 6970 7469 6f6e 2065  e subscription e
+000134b0: 7665 6e74 732c 2075 7365 2074 6865 0a72  vents, use the.r
+000134c0: 6567 756c 6172 2065 7870 7265 7373 696f  egular expressio
+000134d0: 6e20 6072 2750 6572 7369 7374 656e 7443  n `r'PersistentC
+000134e0: 6f6e 6669 675c 642b 2760 2e20 5468 6520  onfig\d+'`. The 
+000134f0: 636f 6e73 7461 6e74 2060 4553 4442 5f50  constant `ESDB_P
+00013500: 4552 5349 5354 454e 545f 434f 4e46 4947  ERSISTENT_CONFIG
+00013510: 5f45 5645 4e54 535f 5245 4745 5860 0a69  _EVENTS_REGEX`.i
+00013520: 7320 7365 7420 746f 2060 7227 5065 7273  s set to `r'Pers
+00013530: 6973 7465 6e74 436f 6e66 6967 5c64 2b27  istentConfig\d+'
+00013540: 602e 2059 6f75 2063 616e 2061 6c73 6f20  `. You can also 
+00013550: 696d 706f 7274 2074 6869 7320 7661 6c75  import this valu
+00013560: 650a 2860 6672 6f6d 2065 7364 6263 6c69  e.(`from esdbcli
+00013570: 656e 7420 696d 706f 7274 2045 5344 425f  ent import ESDB_
+00013580: 5045 5253 4953 5445 4e54 5f43 4f4e 4649  PERSISTENT_CONFI
+00013590: 475f 4556 454e 5453 5f52 4547 4558 6029  G_EVENTS_REGEX`)
+000135a0: 2061 6e64 2075 7365 2069 7420 7768 656e   and use it when
+000135b0: 2062 7569 6c64 696e 670a 6c6f 6e67 6572   building.longer
+000135c0: 2073 6571 7565 6e63 6573 206f 6620 7265   sequences of re
+000135d0: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
+000135e0: 732e 0a0a 5468 6520 636f 6e73 7461 6e74  s...The constant
+000135f0: 2060 4445 4641 554c 545f 4558 434c 5544   `DEFAULT_EXCLUD
+00013600: 455f 4649 4c54 4552 6020 6973 2061 2073  E_FILTER` is a s
+00013610: 6571 7565 6e63 6520 6f66 2072 6567 756c  equence of regul
+00013620: 6172 2065 7870 7265 7373 696f 6e73 2074  ar expressions t
+00013630: 6861 7420 6d61 7463 680a 7468 6520 6576  hat match.the ev
+00013640: 656e 7473 2074 6861 7420 4576 656e 7453  ents that EventS
+00013650: 746f 7265 4442 2067 656e 6572 6174 6573  toreDB generates
+00013660: 2069 6e74 6572 6e61 6c6c 792c 2065 7665   internally, eve
+00013670: 6e74 7320 7468 6174 2061 7265 2065 7874  nts that are ext
+00013680: 7261 6e65 6f75 7320 746f 2074 686f 7365  raneous to those
+00013690: 0a77 6869 6368 2079 6f75 2061 7070 656e  .which you appen
+000136a0: 6420 7573 696e 6720 7468 6520 6061 7070  d using the `app
+000136b0: 656e 645f 6576 656e 7473 2829 6020 6d65  end_events()` me
+000136c0: 7468 6f64 2e0a 0a46 6f72 2065 7861 6d70  thod...For examp
+000136d0: 6c65 2c20 746f 2065 7863 6c75 6465 2073  le, to exclude s
+000136e0: 7973 7465 6d20 6576 656e 7473 2061 6e64  ystem events and
+000136f0: 2070 6572 7369 7374 656e 6365 2073 7562   persistence sub
+00013700: 7363 7269 7074 696f 6e20 636f 6e66 6967  scription config
+00013710: 7572 6174 696f 6e20 6576 656e 7473 2c0a  uration events,.
+00013720: 616e 6420 736e 6170 7368 6f74 732c 2079  and snapshots, y
+00013730: 6f75 206d 6967 6874 2075 7365 2074 6865  ou might use the
+00013740: 2073 6571 7565 6e63 6520 6044 4546 4155   sequence `DEFAU
+00013750: 4c54 5f45 5843 4c55 4445 5f46 494c 5445  LT_EXCLUDE_FILTE
+00013760: 5220 2b20 5b27 2e2a 536e 6170 7368 6f74  R + ['.*Snapshot
+00013770: 275d 6020 6173 0a74 6865 2076 616c 7565  ']` as.the value
+00013780: 206f 6620 7468 6520 6066 696c 7465 725f   of the `filter_
+00013790: 6578 636c 7564 6560 2061 7267 756d 656e  exclude` argumen
+000137a0: 7420 7768 656e 2063 616c 6c69 6e67 2060  t when calling `
+000137b0: 7265 6164 5f61 6c6c 5f65 7665 6e74 7328  read_all_events(
+000137c0: 2960 2c0a 6073 7562 7363 7269 6265 5f61  )`,.`subscribe_a
+000137d0: 6c6c 5f65 7665 6e74 7328 2960 2c20 6063  ll_events()`, `c
+000137e0: 7265 6174 655f 7375 6273 6372 6970 7469  reate_subscripti
+000137f0: 6f6e 2829 6020 6f72 2060 6765 745f 636f  on()` or `get_co
+00013800: 6d6d 6974 5f70 6f73 6974 696f 6e28 2960  mmit_position()`
+00013810: 2e0a 0a23 2323 204e 6577 2065 7665 6e74  ...### New event
+00013820: 206f 626a 6563 7473 0a0a 5468 6520 604e   objects..The `N
+00013830: 6577 4576 656e 7460 2063 6c61 7373 2069  ewEvent` class i
+00013840: 7320 7573 6564 2077 6865 6e20 6170 7065  s used when appe
+00013850: 6e64 696e 6720 6576 656e 7473 2e0a 0a54  nding events...T
+00013860: 6865 2072 6571 7569 7265 6420 6172 6775  he required argu
+00013870: 6d65 6e74 2060 7479 7065 6020 6973 2061  ment `type` is a
+00013880: 2050 7974 686f 6e20 6073 7472 6020 6f62   Python `str` ob
+00013890: 6a65 6374 2c20 7573 6564 2074 6f20 696e  ject, used to in
+000138a0: 6469 6361 7465 2074 6865 2074 7970 6520  dicate the type 
+000138b0: 6f66 0a74 6865 2065 7665 6e74 2074 6861  of.the event tha
+000138c0: 7420 7769 6c6c 2062 6520 7265 636f 7264  t will be record
+000138d0: 6564 2e0a 0a54 6865 2072 6571 7569 7265  ed...The require
+000138e0: 6420 6172 6775 6d65 6e74 2060 6461 7461  d argument `data
+000138f0: 6020 6973 2061 2050 7974 686f 6e20 6062  ` is a Python `b
+00013900: 7974 6573 6020 6f62 6a65 6374 2c20 7573  ytes` object, us
+00013910: 6564 2074 6f20 696e 6469 6361 7465 2074  ed to indicate t
+00013920: 6865 2064 6174 6120 6f66 0a74 6865 2065  he data of.the e
+00013930: 7665 6e74 2074 6861 7420 7769 6c6c 2062  vent that will b
+00013940: 6520 7265 636f 7264 6564 2e0a 0a54 6865  e recorded...The
+00013950: 206f 7074 696f 6e61 6c20 6172 6775 6d65   optional argume
+00013960: 6e74 2060 6d65 7461 6461 7461 6020 6973  nt `metadata` is
+00013970: 2061 2050 7974 686f 6e20 6062 7974 6573   a Python `bytes
+00013980: 6020 6f62 6a65 6374 2c20 7573 6564 2074  ` object, used t
+00013990: 6f20 696e 6469 6361 7465 2061 6e79 0a6d  o indicate any.m
+000139a0: 6574 6164 6174 6120 6f66 2074 6865 2065  etadata of the e
+000139b0: 7665 6e74 2074 6861 7420 7769 6c6c 2062  vent that will b
+000139c0: 6520 7265 636f 7264 6564 2e20 5468 6520  e recorded. The 
+000139d0: 6465 6661 756c 7420 7661 6c75 6520 6973  default value is
+000139e0: 2061 6e20 656d 7074 7920 6062 7974 6573   an empty `bytes
+000139f0: 600a 6f62 6a65 6374 2e0a 0a54 6865 206f  `.object...The o
+00013a00: 7074 696f 6e61 6c20 6172 6775 6d65 6e74  ptional argument
+00013a10: 2060 636f 6e74 656e 745f 7479 7065 6020   `content_type` 
+00013a20: 6973 2061 2050 7974 686f 6e20 6073 7472  is a Python `str
+00013a30: 6020 6f62 6a65 6374 2c20 7573 6564 2074  ` object, used t
+00013a40: 6f20 696e 6469 6361 7465 2074 6865 0a74  o indicate the.t
+00013a50: 7970 6520 6f66 2074 6865 2064 6174 6120  ype of the data 
+00013a60: 7468 6174 2077 696c 6c20 6265 2072 6563  that will be rec
+00013a70: 6f72 6465 6420 666f 7220 7468 6973 2065  orded for this e
+00013a80: 7665 6e74 2e20 5468 6520 6465 6661 756c  vent. The defaul
+00013a90: 7420 7661 6c75 6520 6973 0a60 6170 706c  t value is.`appl
+00013aa0: 6963 6174 696f 6e2f 6a73 6f6e 602c 2077  ication/json`, w
+00013ab0: 6869 6368 2069 6e64 6963 6174 6573 2074  hich indicates t
+00013ac0: 6861 7420 7468 6520 6064 6174 6160 2077  hat the `data` w
+00013ad0: 6173 2073 6572 6961 6c69 7365 6420 7573  as serialised us
+00013ae0: 696e 6720 4a53 4f4e 2e0a 416e 2061 6c74  ing JSON..An alt
+00013af0: 6572 6e61 7469 7665 2076 616c 7565 2066  ernative value f
+00013b00: 6f72 2074 6869 7320 6172 6775 6d65 6e74  or this argument
+00013b10: 2069 7320 6061 7070 6c69 6361 7469 6f6e   is `application
+00013b20: 2f6f 6374 6574 2d73 7472 6561 6d60 2e0a  /octet-stream`..
+00013b30: 0a54 6865 206f 7074 696f 6e61 6c20 6172  .The optional ar
+00013b40: 6775 6d65 6e74 2060 6964 6020 6973 2061  gument `id` is a
+00013b50: 2050 7974 686f 6e20 6055 5549 4460 206f   Python `UUID` o
+00013b60: 626a 6563 742c 2075 7365 6420 746f 2073  bject, used to s
+00013b70: 7065 6369 6679 2074 6865 2075 6e69 7175  pecify the uniqu
+00013b80: 6520 4944 0a6f 6620 7468 6520 6576 656e  e ID.of the even
+00013b90: 7420 7468 6174 2077 696c 6c20 6265 2072  t that will be r
+00013ba0: 6563 6f72 6465 642e 2054 6869 7320 7661  ecorded. This va
+00013bb0: 6c75 6520 7769 6c6c 2064 6566 6175 6c74  lue will default
+00013bc0: 2074 6f20 6120 6e65 7720 7665 7273 696f   to a new versio
+00013bd0: 6e2d 3420 5555 4944 2e0a 0a60 6060 7079  n-4 UUID...```py
+00013be0: 7468 6f6e 0a6e 6577 5f65 7665 6e74 3120  thon.new_event1 
+00013bf0: 3d20 4e65 7745 7665 6e74 280a 2020 2020  = NewEvent(.    
+00013c00: 7479 7065 3d27 4f72 6465 7243 7265 6174  type='OrderCreat
+00013c10: 6564 272c 0a20 2020 2064 6174 613d 6227  ed',.    data=b'
+00013c20: 7b22 6e61 6d65 223a 2022 4772 6567 227d  {"name": "Greg"}
+00013c30: 272c 0a29 0a61 7373 6572 7420 6e65 775f  ',.).assert new_
+00013c40: 6576 656e 7431 2e74 7970 6520 3d3d 2027  event1.type == '
+00013c50: 4f72 6465 7243 7265 6174 6564 270a 6173  OrderCreated'.as
+00013c60: 7365 7274 206e 6577 5f65 7665 6e74 312e  sert new_event1.
+00013c70: 6461 7461 203d 3d20 6227 7b22 6e61 6d65  data == b'{"name
+00013c80: 223a 2022 4772 6567 227d 270a 6173 7365  ": "Greg"}'.asse
+00013c90: 7274 206e 6577 5f65 7665 6e74 312e 6d65  rt new_event1.me
+00013ca0: 7461 6461 7461 203d 3d20 6227 270a 6173  tadata == b''.as
+00013cb0: 7365 7274 206e 6577 5f65 7665 6e74 312e  sert new_event1.
+00013cc0: 636f 6e74 656e 745f 7479 7065 203d 3d20  content_type == 
+00013cd0: 2761 7070 6c69 6361 7469 6f6e 2f6a 736f  'application/jso
+00013ce0: 6e27 0a61 7373 6572 7420 6973 696e 7374  n'.assert isinst
+00013cf0: 616e 6365 286e 6577 5f65 7665 6e74 312e  ance(new_event1.
+00013d00: 6964 2c20 5555 4944 290a 0a65 7665 6e74  id, UUID)..event
+00013d10: 5f69 6420 3d20 7575 6964 3428 290a 6e65  _id = uuid4().ne
+00013d20: 775f 6576 656e 7432 203d 204e 6577 4576  w_event2 = NewEv
+00013d30: 656e 7428 0a20 2020 2074 7970 653d 2749  ent(.    type='I
+00013d40: 6d61 6765 4372 6561 7465 6427 2c0a 2020  mageCreated',.  
+00013d50: 2020 6461 7461 3d62 2730 3130 3130 3130    data=b'0101010
+00013d60: 3130 3130 3130 3127 2c0a 2020 2020 6d65  1010101',.    me
+00013d70: 7461 6461 7461 3d62 277b 2261 223a 2031  tadata=b'{"a": 1
+00013d80: 7d27 2c0a 2020 2020 636f 6e74 656e 745f  }',.    content_
+00013d90: 7479 7065 3d27 6170 706c 6963 6174 696f  type='applicatio
+00013da0: 6e2f 6f63 7465 742d 7374 7265 616d 272c  n/octet-stream',
+00013db0: 0a20 2020 2069 643d 6576 656e 745f 6964  .    id=event_id
+00013dc0: 2c0a 290a 6173 7365 7274 206e 6577 5f65  ,.).assert new_e
+00013dd0: 7665 6e74 322e 7479 7065 203d 3d20 2749  vent2.type == 'I
+00013de0: 6d61 6765 4372 6561 7465 6427 0a61 7373  mageCreated'.ass
+00013df0: 6572 7420 6e65 775f 6576 656e 7432 2e64  ert new_event2.d
+00013e00: 6174 6120 3d3d 2062 2730 3130 3130 3130  ata == b'0101010
+00013e10: 3130 3130 3130 3127 0a61 7373 6572 7420  1010101'.assert 
+00013e20: 6e65 775f 6576 656e 7432 2e6d 6574 6164  new_event2.metad
+00013e30: 6174 6120 3d3d 2062 277b 2261 223a 2031  ata == b'{"a": 1
+00013e40: 7d27 0a61 7373 6572 7420 6e65 775f 6576  }'.assert new_ev
+00013e50: 656e 7432 2e63 6f6e 7465 6e74 5f74 7970  ent2.content_typ
+00013e60: 6520 3d3d 2027 6170 706c 6963 6174 696f  e == 'applicatio
+00013e70: 6e2f 6f63 7465 742d 7374 7265 616d 270a  n/octet-stream'.
+00013e80: 6173 7365 7274 206e 6577 5f65 7665 6e74  assert new_event
+00013e90: 322e 6964 203d 3d20 6576 656e 745f 6964  2.id == event_id
+00013ea0: 0a60 6060 0a0a 2323 2320 5265 636f 7264  .```..### Record
+00013eb0: 6564 2065 7665 6e74 206f 626a 6563 7473  ed event objects
+00013ec0: 0a0a 5468 6520 6052 6563 6f72 6465 6445  ..The `RecordedE
+00013ed0: 7665 6e74 6020 636c 6173 7320 6973 2075  vent` class is u
+00013ee0: 7365 6420 7768 656e 2072 6561 6469 6e67  sed when reading
+00013ef0: 2065 7665 6e74 732e 0a0a 5468 6520 6174   events...The at
+00013f00: 7472 6962 7574 6520 6074 7970 6560 2069  tribute `type` i
+00013f10: 7320 6120 5079 7468 6f6e 2060 7374 7260  s a Python `str`
+00013f20: 206f 626a 6563 742c 2075 7365 6420 746f   object, used to
+00013f30: 2069 6e64 6963 6174 6520 7468 6520 7479   indicate the ty
+00013f40: 7065 206f 6620 6576 656e 740a 7468 6174  pe of event.that
+00013f50: 2077 6173 2072 6563 6f72 6465 642e 0a0a   was recorded...
+00013f60: 5468 6520 6174 7472 6962 7574 6520 6064  The attribute `d
+00013f70: 6174 6160 2069 7320 6120 5079 7468 6f6e  ata` is a Python
+00013f80: 2060 6279 7465 7360 206f 626a 6563 742c   `bytes` object,
+00013f90: 2075 7365 6420 746f 2069 6e64 6963 6174   used to indicat
+00013fa0: 6520 7468 6520 6461 7461 206f 6620 7468  e the data of th
+00013fb0: 650a 6576 656e 7420 7468 6174 2077 6173  e.event that was
+00013fc0: 2072 6563 6f72 6465 642e 0a0a 5468 6520   recorded...The 
+00013fd0: 6174 7472 6962 7574 6520 606d 6574 6164  attribute `metad
+00013fe0: 6174 6160 2069 7320 6120 5079 7468 6f6e  ata` is a Python
+00013ff0: 2060 6279 7465 7360 206f 626a 6563 742c   `bytes` object,
+00014000: 2075 7365 6420 746f 2069 6e64 6963 6174   used to indicat
+00014010: 6520 7468 6520 6d65 7461 6461 7461 206f  e the metadata o
+00014020: 660a 7468 6520 6576 656e 7420 7468 6174  f.the event that
+00014030: 2077 6173 2072 6563 6f72 6465 642e 0a0a   was recorded...
+00014040: 5468 6520 6174 7472 6962 7574 6520 6063  The attribute `c
+00014050: 6f6e 7465 6e74 5f74 7970 6560 2069 7320  ontent_type` is 
+00014060: 6120 5079 7468 6f6e 2060 7374 7260 206f  a Python `str` o
+00014070: 626a 6563 742c 2075 7365 6420 746f 2069  bject, used to i
+00014080: 6e64 6963 6174 6520 7468 6520 7479 7065  ndicate the type
+00014090: 206f 660a 6461 7461 2074 6861 7420 7761   of.data that wa
+000140a0: 7320 7265 636f 7264 6564 2066 6f72 2074  s recorded for t
+000140b0: 6869 7320 6576 656e 7420 2875 7375 616c  his event (usual
+000140c0: 6c79 2060 6170 706c 6963 6174 696f 6e2f  ly `application/
+000140d0: 6a73 6f6e 6020 746f 2069 6e64 6963 6174  json` to indicat
+000140e0: 6520 7468 6174 0a74 6869 7320 6461 7461  e that.this data
+000140f0: 2063 616e 2062 6520 7061 7273 6564 2061   can be parsed a
+00014100: 7320 4a53 4f4e 2c20 6275 7420 616c 7465  s JSON, but alte
+00014110: 726e 6174 6976 656c 7920 6061 7070 6c69  rnatively `appli
+00014120: 6361 7469 6f6e 2f6f 6374 6574 2d73 7472  cation/octet-str
+00014130: 6561 6d60 2074 6f0a 696e 6469 6361 7465  eam` to.indicate
+00014140: 2074 6861 7420 6974 2069 7320 736f 6d65   that it is some
+00014150: 7468 696e 6720 656c 7365 292e 0a0a 5468  thing else)...Th
+00014160: 6520 6174 7472 6962 7574 6520 6069 6460  e attribute `id`
+00014170: 2069 7320 6120 5079 7468 6f6e 2060 5555   is a Python `UU
+00014180: 4944 6020 6f62 6a65 6374 2c20 7573 6564  ID` object, used
+00014190: 2074 6f20 696e 6469 6361 7465 2074 6865   to indicate the
+000141a0: 2075 6e69 7175 6520 4944 206f 6620 7468   unique ID of th
+000141b0: 650a 6576 656e 7420 7468 6174 2077 6173  e.event that was
+000141c0: 2072 6563 6f72 6465 642e 2050 6c65 6173   recorded. Pleas
+000141d0: 6520 6e6f 7465 2c20 7768 656e 2072 6563  e note, when rec
+000141e0: 6f72 6465 6420 6576 656e 7473 2061 7265  orded events are
+000141f0: 2072 6574 7572 6e65 6420 6672 6f6d 2061   returned from a
+00014200: 2063 616c 6c0a 746f 2060 7265 6164 5f73   call.to `read_s
+00014210: 7472 6561 6d5f 6576 656e 7473 2829 6020  tream_events()` 
+00014220: 696e 2045 7665 6e74 5374 6f72 6544 4220  in EventStoreDB 
+00014230: 7632 312e 3130 2c20 7468 6520 636f 6d6d  v21.10, the comm
+00014240: 6974 2070 6f73 6974 696f 6e20 6973 206e  it position is n
+00014250: 6f74 2061 6374 7561 6c6c 790a 7365 7420  ot actually.set 
+00014260: 696e 2074 6865 2072 6573 706f 6e73 652e  in the response.
+00014270: 2054 6869 7320 6174 7472 6962 7574 6520   This attribute 
+00014280: 6973 2074 7970 6564 2061 7320 616e 206f  is typed as an o
+00014290: 7074 696f 6e61 6c20 7661 6c75 6520 2860  ptional value (`
+000142a0: 4f70 7469 6f6e 616c 5b55 5549 445d 6029  Optional[UUID]`)
+000142b0: 2c0a 616e 6420 696e 2074 6865 2063 6173  ,.and in the cas
+000142c0: 6520 6f66 2075 7369 6e67 2045 7665 6e74  e of using Event
+000142d0: 5374 6f72 6544 4220 7632 312e 3130 2074  StoreDB v21.10 t
+000142e0: 6865 2076 616c 7565 206f 6620 7468 6973  he value of this
+000142f0: 2061 7474 7269 6275 7465 2077 696c 6c20   attribute will 
+00014300: 6265 2060 4e6f 6e65 600a 7768 656e 2072  be `None`.when r
+00014310: 6561 6469 6e67 2072 6563 6f72 6465 6420  eading recorded 
+00014320: 6576 656e 7473 2066 726f 6d20 6120 7374  events from a st
+00014330: 7265 616d 2e20 5265 636f 7264 6564 2065  ream. Recorded e
+00014340: 7665 6e74 7320 7769 6c6c 2068 6f77 6576  vents will howev
+00014350: 6572 2068 6176 6520 7468 6973 0a76 616c  er have this.val
+00014360: 7565 7320 7365 7420 7768 656e 2072 6561  ues set when rea
+00014370: 6469 6e67 2072 6563 6f72 6465 6420 6576  ding recorded ev
+00014380: 656e 7473 2066 726f 6d20 6072 6561 645f  ents from `read_
+00014390: 616c 6c5f 6576 656e 7473 2829 6020 616e  all_events()` an
+000143a0: 6420 6672 6f6d 2062 6f74 680a 6361 7463  d from both.catc
+000143b0: 682d 7570 2061 6e64 2070 6572 7369 7374  h-up and persist
+000143c0: 656e 7420 7375 6273 6372 6970 7469 6f6e  ent subscription
+000143d0: 732e 0a0a 5468 6520 6174 7472 6962 7574  s...The attribut
+000143e0: 6520 6073 7472 6561 6d5f 6e61 6d65 6020  e `stream_name` 
+000143f0: 6973 2061 2050 7974 686f 6e20 6073 7472  is a Python `str
+00014400: 6020 6f62 6a65 6374 2c20 7573 6564 2074  ` object, used t
+00014410: 6f20 696e 6469 6361 7465 2074 6865 206e  o indicate the n
+00014420: 616d 6520 6f66 2074 6865 0a73 7472 6561  ame of the.strea
+00014430: 6d20 696e 2077 6869 6368 2074 6865 2065  m in which the e
+00014440: 7665 6e74 2077 6173 2072 6563 6f72 6465  vent was recorde
+00014450: 642e 0a0a 5468 6520 6174 7472 6962 7574  d...The attribut
+00014460: 6520 6073 7472 6561 6d5f 706f 7369 7469  e `stream_positi
+00014470: 6f6e 6020 6973 2061 2050 7974 686f 6e20  on` is a Python 
+00014480: 6069 6e74 602c 2075 7365 6420 746f 2069  `int`, used to i
+00014490: 6e64 6963 6174 6520 7468 6520 706f 7369  ndicate the posi
+000144a0: 7469 6f6e 2069 6e20 7468 650a 7374 7265  tion in the.stre
+000144b0: 616d 2061 7420 7768 6963 6820 7468 6520  am at which the 
+000144c0: 6576 656e 7420 7761 7320 7265 636f 7264  event was record
+000144d0: 6564 2e0a 0a54 6865 2061 7474 7269 6275  ed...The attribu
+000144e0: 7465 2060 636f 6d6d 6974 5f70 6f73 6974  te `commit_posit
+000144f0: 696f 6e60 2069 7320 6120 5079 7468 6f6e  ion` is a Python
+00014500: 2060 696e 7460 2c20 7573 6564 2074 6f20   `int`, used to 
+00014510: 696e 6469 6361 7465 2074 6865 2063 6f6d  indicate the com
+00014520: 6d69 7420 706f 7369 7469 6f6e 0a61 7420  mit position.at 
+00014530: 7768 6963 6820 7468 6520 6576 656e 7420  which the event 
+00014540: 7761 7320 7265 636f 7264 6564 2e0a 0a60  was recorded...`
+00014550: 6060 7079 7468 6f6e 0a66 726f 6d20 6573  ``python.from es
+00014560: 6462 636c 6965 6e74 2e65 7665 6e74 7320  dbclient.events 
+00014570: 696d 706f 7274 2052 6563 6f72 6465 6445  import RecordedE
+00014580: 7665 6e74 0a0a 7265 636f 7264 6564 5f65  vent..recorded_e
+00014590: 7665 6e74 203d 2052 6563 6f72 6465 6445  vent = RecordedE
+000145a0: 7665 6e74 280a 2020 2020 7479 7065 3d27  vent(.    type='
+000145b0: 4f72 6465 7243 7265 6174 6564 272c 0a20  OrderCreated',. 
+000145c0: 2020 2064 6174 613d 6227 7b7d 272c 0a20     data=b'{}',. 
+000145d0: 2020 206d 6574 6164 6174 613d 6227 272c     metadata=b'',
+000145e0: 0a20 2020 2063 6f6e 7465 6e74 5f74 7970  .    content_typ
+000145f0: 653d 2761 7070 6c69 6361 7469 6f6e 2f6a  e='application/j
+00014600: 736f 6e27 2c0a 2020 2020 6964 3d75 7569  son',.    id=uui
+00014610: 6434 2829 2c0a 2020 2020 7374 7265 616d  d4(),.    stream
+00014620: 5f6e 616d 653d 2773 7472 6561 6d31 272c  _name='stream1',
+00014630: 0a20 2020 2073 7472 6561 6d5f 706f 7369  .    stream_posi
+00014640: 7469 6f6e 3d30 2c0a 2020 2020 636f 6d6d  tion=0,.    comm
+00014650: 6974 5f70 6f73 6974 696f 6e3d 3531 322c  it_position=512,
+00014660: 0a29 0a60 6060 0a0a 2323 2043 6f6e 7472  .).```..## Contr
+00014670: 6962 7574 6f72 730a 0a23 2323 2049 6e73  ibutors..### Ins
+00014680: 7461 6c6c 2050 6f65 7472 790a 0a54 6865  tall Poetry..The
+00014690: 2066 6972 7374 2074 6869 6e67 2069 7320   first thing is 
+000146a0: 746f 2063 6865 636b 2079 6f75 2068 6176  to check you hav
+000146b0: 6520 506f 6574 7279 2069 6e73 7461 6c6c  e Poetry install
+000146c0: 6564 2e0a 0a20 2020 2024 2070 6f65 7472  ed...    $ poetr
+000146d0: 7920 2d2d 7665 7273 696f 6e0a 0a49 6620  y --version..If 
+000146e0: 796f 7520 646f 6e27 742c 2074 6865 6e20  you don't, then 
+000146f0: 706c 6561 7365 205b 696e 7374 616c 6c20  please [install 
+00014700: 506f 6574 7279 5d28 6874 7470 733a 2f2f  Poetry](https://
+00014710: 7079 7468 6f6e 2d70 6f65 7472 792e 6f72  python-poetry.or
+00014720: 672f 646f 6373 2f23 696e 7374 616c 6c69  g/docs/#installi
+00014730: 6e67 2d77 6974 682d 7468 652d 6f66 6669  ng-with-the-offi
+00014740: 6369 616c 2d69 6e73 7461 6c6c 6572 292e  cial-installer).
+00014750: 0a0a 2020 2020 2420 6375 726c 202d 7353  ..    $ curl -sS
+00014760: 4c20 6874 7470 733a 2f2f 696e 7374 616c  L https://instal
+00014770: 6c2e 7079 7468 6f6e 2d70 6f65 7472 792e  l.python-poetry.
+00014780: 6f72 6720 7c20 7079 7468 6f6e 3320 2d0a  org | python3 -.
+00014790: 0a49 7420 7769 6c6c 2068 656c 7020 746f  .It will help to
+000147a0: 206d 616b 6520 7375 7265 2050 6f65 7472   make sure Poetr
+000147b0: 7927 7320 6269 6e20 6469 7265 6374 6f72  y's bin director
+000147c0: 7920 6973 2069 6e20 796f 7572 2060 5041  y is in your `PA
+000147d0: 5448 6020 656e 7669 726f 6e6d 656e 7420  TH` environment 
+000147e0: 7661 7269 6162 6c65 2e0a 0a42 7574 2069  variable...But i
+000147f0: 6e20 616e 7920 6361 7365 2c20 6d61 6b65  n any case, make
+00014800: 2073 7572 6520 796f 7520 6b6e 6f77 2074   sure you know t
+00014810: 6865 2070 6174 6820 746f 2074 6865 2060  he path to the `
+00014820: 706f 6574 7279 6020 6578 6563 7574 6162  poetry` executab
+00014830: 6c65 2e20 5468 6520 506f 6574 7279 0a69  le. The Poetry.i
+00014840: 6e73 7461 6c6c 6572 2074 656c 6c73 2079  nstaller tells y
+00014850: 6f75 2077 6865 7265 2069 7420 6861 7320  ou where it has 
+00014860: 6265 656e 2069 6e73 7461 6c6c 6564 2c20  been installed, 
+00014870: 616e 6420 686f 7720 746f 2063 6f6e 6669  and how to confi
+00014880: 6775 7265 2079 6f75 7220 7368 656c 6c2e  gure your shell.
+00014890: 0a0a 506c 6561 7365 2072 6566 6572 2074  ..Please refer t
+000148a0: 6f20 7468 6520 5b50 6f65 7472 7920 646f  o the [Poetry do
+000148b0: 6373 5d28 6874 7470 733a 2f2f 7079 7468  cs](https://pyth
+000148c0: 6f6e 2d70 6f65 7472 792e 6f72 672f 646f  on-poetry.org/do
+000148d0: 6373 2f29 2066 6f72 2067 7569 6461 6e63  cs/) for guidanc
+000148e0: 6520 6f6e 0a75 7369 6e67 2050 6f65 7472  e on.using Poetr
+000148f0: 792e 0a0a 2323 2320 5365 7475 7020 666f  y...### Setup fo
+00014900: 7220 5079 4368 6172 6d20 7573 6572 730a  r PyCharm users.
+00014910: 0a59 6f75 2063 616e 2065 6173 696c 7920  .You can easily 
+00014920: 6f62 7461 696e 2074 6865 2070 726f 6a65  obtain the proje
+00014930: 6374 2066 696c 6573 2075 7369 6e67 2050  ct files using P
+00014940: 7943 6861 726d 2028 6d65 6e75 2022 4769  yCharm (menu "Gi
+00014950: 7420 3e20 436c 6f6e 652e 2e2e 2229 2e0a  t > Clone...")..
+00014960: 5079 4368 6172 6d20 7769 6c6c 2074 6865  PyCharm will the
+00014970: 6e20 7573 7561 6c6c 7920 7072 6f6d 7074  n usually prompt
+00014980: 2079 6f75 2074 6f20 6f70 656e 2074 6865   you to open the
+00014990: 2070 726f 6a65 6374 2e0a 0a4f 7065 6e20   project...Open 
+000149a0: 7468 6520 7072 6f6a 6563 7420 696e 2061  the project in a
+000149b0: 206e 6577 2077 696e 646f 772e 2050 7943   new window. PyC
+000149c0: 6861 726d 2077 696c 6c20 7468 656e 2075  harm will then u
+000149d0: 7375 616c 6c79 2070 726f 6d70 7420 796f  sually prompt yo
+000149e0: 7520 746f 2063 7265 6174 650a 6120 6e65  u to create.a ne
+000149f0: 7720 7669 7274 7561 6c20 656e 7669 726f  w virtual enviro
+00014a00: 6e6d 656e 742e 0a0a 4372 6561 7465 2061  nment...Create a
+00014a10: 206e 6577 2050 6f65 7472 7920 7669 7274   new Poetry virt
+00014a20: 7561 6c20 656e 7669 726f 6e6d 656e 7420  ual environment 
+00014a30: 666f 7220 7468 6520 7072 6f6a 6563 742e  for the project.
+00014a40: 2049 6620 5079 4368 6172 6d20 646f 6573   If PyCharm does
+00014a50: 6e27 7420 616c 7265 6164 790a 6b6e 6f77  n't already.know
+00014a60: 2077 6865 7265 2079 6f75 7220 6070 6f65   where your `poe
+00014a70: 7472 7960 2065 7865 6375 7461 626c 6520  try` executable 
+00014a80: 6973 2c20 7468 656e 2073 6574 2074 6865  is, then set the
+00014a90: 2070 6174 6820 746f 2079 6f75 7220 6070   path to your `p
+00014aa0: 6f65 7472 7960 2065 7865 6375 7461 626c  oetry` executabl
+00014ab0: 650a 696e 2074 6865 2022 4e65 7720 506f  e.in the "New Po
+00014ac0: 6574 7279 2045 6e76 6972 6f6e 6d65 6e74  etry Environment
+00014ad0: 2220 666f 726d 2069 6e70 7574 2066 6965  " form input fie
+00014ae0: 6c64 206c 6162 656c 6c65 6420 2250 6f65  ld labelled "Poe
+00014af0: 7472 7920 6578 6563 7574 6162 6c65 222e  try executable".
+00014b00: 2049 6e20 7468 650a 224e 6577 2050 6f65   In the."New Poe
+00014b10: 7472 7920 456e 7669 726f 6e6d 656e 7422  try Environment"
+00014b20: 2066 6f72 6d2c 2079 6f75 2077 696c 6c20   form, you will 
+00014b30: 616c 736f 2068 6176 6520 7468 6520 6f70  also have the op
+00014b40: 706f 7274 756e 6974 7920 746f 2073 656c  portunity to sel
+00014b50: 6563 7420 7768 6963 680a 5079 7468 6f6e  ect which.Python
+00014b60: 2065 7865 6375 7461 626c 6520 7769 6c6c   executable will
+00014b70: 2062 6520 7573 6564 2062 7920 7468 6520   be used by the 
+00014b80: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
+00014b90: 656e 742e 0a0a 5079 4368 6172 6d20 7769  ent...PyCharm wi
+00014ba0: 6c6c 2074 6865 6e20 6372 6561 7465 2061  ll then create a
+00014bb0: 206e 6577 2050 6f65 7472 7920 7669 7274   new Poetry virt
+00014bc0: 7561 6c20 656e 7669 726f 6e6d 656e 7420  ual environment 
+00014bd0: 666f 7220 796f 7572 2070 726f 6a65 6374  for your project
+00014be0: 2c20 7573 696e 670a 6120 7061 7274 6963  , using.a partic
+00014bf0: 756c 6172 2076 6572 7369 6f6e 206f 6620  ular version of 
+00014c00: 5079 7468 6f6e 2c20 616e 6420 616c 736f  Python, and also
+00014c10: 2069 6e73 7461 6c6c 2069 6e74 6f20 7468   install into th
+00014c20: 6973 2076 6972 7475 616c 2065 6e76 6972  is virtual envir
+00014c30: 6f6e 6d65 6e74 2074 6865 0a70 726f 6a65  onment the.proje
+00014c40: 6374 2773 2070 6163 6b61 6765 2064 6570  ct's package dep
+00014c50: 656e 6465 6e63 6965 7320 6163 636f 7264  endencies accord
+00014c60: 696e 6720 746f 2074 6865 2070 726f 6a65  ing to the proje
+00014c70: 6374 2773 2060 706f 6574 7279 2e6c 6f63  ct's `poetry.loc
+00014c80: 6b60 2066 696c 652e 0a0a 596f 7520 6361  k` file...You ca
+00014c90: 6e20 6164 6420 6469 6666 6572 656e 7420  n add different 
+00014ca0: 506f 6574 7279 2065 6e76 6972 6f6e 6d65  Poetry environme
+00014cb0: 6e74 7320 666f 7220 6469 6666 6572 656e  nts for differen
+00014cc0: 7420 5079 7468 6f6e 2076 6572 7369 6f6e  t Python version
+00014cd0: 732c 2061 6e64 2073 7769 7463 680a 6265  s, and switch.be
+00014ce0: 7477 6565 6e20 7468 656d 2075 7369 6e67  tween them using
+00014cf0: 2074 6865 2022 5079 7468 6f6e 2049 6e74   the "Python Int
+00014d00: 6572 7072 6574 6572 2220 7365 7474 696e  erpreter" settin
+00014d10: 6773 206f 6620 5079 4368 6172 6d2e 2049  gs of PyCharm. I
+00014d20: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
+00014d30: 650a 6120 7665 7273 696f 6e20 6f66 2050  e.a version of P
+00014d40: 7974 686f 6e20 7468 6174 2069 736e 2774  ython that isn't
+00014d50: 2069 6e73 7461 6c6c 6564 2c20 6569 7468   installed, eith
+00014d60: 6572 2075 7365 2079 6f75 7220 6661 766f  er use your favo
+00014d70: 7572 6974 6520 7061 636b 6167 6520 6d61  urite package ma
+00014d80: 6e61 6765 722c 0a6f 7220 696e 7374 616c  nager,.or instal
+00014d90: 6c20 5079 7468 6f6e 2062 7920 646f 776e  l Python by down
+00014da0: 6c6f 6164 696e 6720 616e 2069 6e73 7461  loading an insta
+00014db0: 6c6c 6572 2066 6f72 2072 6563 656e 7420  ller for recent 
+00014dc0: 7665 7273 696f 6e73 206f 6620 5079 7468  versions of Pyth
+00014dd0: 6f6e 2064 6972 6563 746c 790a 6672 6f6d  on directly.from
+00014de0: 2074 6865 205b 5079 7468 6f6e 2077 6562   the [Python web
+00014df0: 7369 7465 5d28 6874 7470 733a 2f2f 7777  site](https://ww
+00014e00: 772e 7079 7468 6f6e 2e6f 7267 2f64 6f77  w.python.org/dow
+00014e10: 6e6c 6f61 6473 2f29 2e0a 0a4f 6e63 6520  nloads/)...Once 
+00014e20: 7072 6f6a 6563 7420 6465 7065 6e64 656e  project dependen
+00014e30: 6369 6573 2068 6176 6520 6265 656e 2069  cies have been i
+00014e40: 6e73 7461 6c6c 6564 2c20 796f 7520 7368  nstalled, you sh
+00014e50: 6f75 6c64 2062 6520 6162 6c65 2074 6f20  ould be able to 
+00014e60: 7275 6e20 7465 7374 730a 6672 6f6d 2077  run tests.from w
+00014e70: 6974 6869 6e20 5079 4368 6172 6d20 2872  ithin PyCharm (r
+00014e80: 6967 6874 2d63 6c69 636b 206f 6e20 7468  ight-click on th
+00014e90: 6520 6074 6573 7473 6020 666f 6c64 6572  e `tests` folder
+00014ea0: 2061 6e64 2073 656c 6563 7420 7468 6520   and select the 
+00014eb0: 2752 756e 2720 6f70 7469 6f6e 292e 0a0a  'Run' option)...
+00014ec0: 4265 6361 7573 6520 6f66 2061 2063 6f6e  Because of a con
+00014ed0: 666c 6963 7420 6265 7477 6565 6e20 7079  flict between py
+00014ee0: 7465 7374 2061 6e64 2050 7943 6861 726d  test and PyCharm
+00014ef0: 2773 2064 6562 7567 6765 7220 616e 6420  's debugger and 
+00014f00: 7468 6520 636f 7665 7261 6765 2074 6f6f  the coverage too
+00014f10: 6c2c 0a79 6f75 206d 6179 206e 6565 6420  l,.you may need 
+00014f20: 746f 2061 6464 2060 602d 2d6e 6f2d 636f  to add ``--no-co
+00014f30: 7660 6020 6173 2061 6e20 6f70 7469 6f6e  v`` as an option
+00014f40: 2074 6f20 7468 6520 7465 7374 2072 756e   to the test run
+00014f50: 6e65 7220 7465 6d70 6c61 7465 2e20 416c  ner template. Al
+00014f60: 7465 726e 6174 6976 656c 792c 0a6a 7573  ternatively,.jus
+00014f70: 7420 7573 6520 7468 6520 5079 7468 6f6e  t use the Python
+00014f80: 2053 7461 6e64 6172 6420 4c69 6272 6172   Standard Librar
+00014f90: 7927 7320 6060 756e 6974 7465 7374 6060  y's ``unittest``
+00014fa0: 206d 6f64 756c 652e 0a0a 596f 7520 7368   module...You sh
+00014fb0: 6f75 6c64 2061 6c73 6f20 6265 2061 626c  ould also be abl
+00014fc0: 6520 746f 206f 7065 6e20 6120 7465 726d  e to open a term
+00014fd0: 696e 616c 2077 696e 646f 7720 696e 2050  inal window in P
+00014fe0: 7943 6861 726d 2c20 616e 6420 7275 6e20  yCharm, and run 
+00014ff0: 7468 6520 7072 6f6a 6563 7427 730a 4d61  the project's.Ma
+00015000: 6b65 6669 6c65 2063 6f6d 6d61 6e64 7320  kefile commands 
+00015010: 6672 6f6d 2074 6865 2063 6f6d 6d61 6e64  from the command
+00015020: 206c 696e 6520 2873 6565 2062 656c 6f77   line (see below
+00015030: 292e 0a0a 2323 2320 5365 7475 7020 6672  )...### Setup fr
+00015040: 6f6d 2063 6f6d 6d61 6e64 206c 696e 650a  om command line.
+00015050: 0a4f 6274 6169 6e20 7468 6520 7072 6f6a  .Obtain the proj
+00015060: 6563 7420 6669 6c65 732c 2075 7369 6e67  ect files, using
+00015070: 2047 6974 206f 7220 7375 6974 6162 6c65   Git or suitable
+00015080: 2061 6c74 6572 6e61 7469 7665 2e0a 0a49   alternative...I
+00015090: 6e20 6120 7465 726d 696e 616c 2061 7070  n a terminal app
+000150a0: 6c69 6361 7469 6f6e 2c20 6368 616e 6765  lication, change
+000150b0: 2079 6f75 7220 6375 7272 656e 7420 776f   your current wo
+000150c0: 726b 696e 6720 6469 7265 6374 6f72 790a  rking directory.
+000150d0: 746f 2074 6865 2072 6f6f 7420 666f 6c64  to the root fold
+000150e0: 6572 206f 6620 7468 6520 7072 6f6a 6563  er of the projec
+000150f0: 7420 6669 6c65 732e 2054 6865 7265 2073  t files. There s
+00015100: 686f 756c 6420 6265 2061 204d 616b 6566  hould be a Makef
+00015110: 696c 650a 696e 2074 6869 7320 666f 6c64  ile.in this fold
+00015120: 6572 2e0a 0a55 7365 2074 6865 204d 616b  er...Use the Mak
+00015130: 6566 696c 6520 746f 2063 7265 6174 6520  efile to create 
+00015140: 6120 6e65 7720 506f 6574 7279 2076 6972  a new Poetry vir
+00015150: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
+00015160: 2066 6f72 2074 6865 0a70 726f 6a65 6374   for the.project
+00015170: 2061 6e64 2069 6e73 7461 6c6c 2074 6865   and install the
+00015180: 2070 726f 6a65 6374 2773 2070 6163 6b61   project's packa
+00015190: 6765 2064 6570 656e 6465 6e63 6965 7320  ge dependencies 
+000151a0: 696e 746f 2069 742c 0a75 7369 6e67 2074  into it,.using t
+000151b0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+000151c0: 6d61 6e64 2e0a 0a20 2020 2024 206d 616b  mand...    $ mak
+000151d0: 6520 696e 7374 616c 6c2d 7061 636b 6167  e install-packag
+000151e0: 6573 0a0a 4974 2773 2061 6c73 6f20 706f  es..It's also po
+000151f0: 7373 6962 6c65 2074 6f20 616c 736f 2069  ssible to also i
+00015200: 6e73 7461 6c6c 2074 6865 2070 726f 6a65  nstall the proje
+00015210: 6374 2069 6e20 2765 6469 7461 626c 6520  ct in 'editable 
+00015220: 6d6f 6465 272e 0a0a 2020 2020 2420 6d61  mode'...    $ ma
+00015230: 6b65 2069 6e73 7461 6c6c 0a0a 506c 6561  ke install..Plea
+00015240: 7365 206e 6f74 652c 2069 6620 796f 7520  se note, if you 
+00015250: 6372 6561 7465 2074 6865 2076 6972 7475  create the virtu
+00015260: 616c 2065 6e76 6972 6f6e 6d65 6e74 2069  al environment i
+00015270: 6e20 7468 6973 2077 6179 2c20 616e 6420  n this way, and 
+00015280: 7468 656e 2074 7279 2074 6f0a 6f70 656e  then try to.open
+00015290: 2074 6865 2070 726f 6a65 6374 2069 6e20   the project in 
+000152a0: 5079 4368 6172 6d20 616e 6420 636f 6e66  PyCharm and conf
+000152b0: 6967 7572 6520 7468 6520 7072 6f6a 6563  igure the projec
+000152c0: 7420 746f 2075 7365 2074 6869 7320 7669  t to use this vi
+000152d0: 7274 7561 6c0a 656e 7669 726f 6e6d 656e  rtual.environmen
+000152e0: 7420 6173 2061 6e20 2245 7869 7374 696e  t as an "Existin
+000152f0: 6720 506f 6574 7279 2045 6e76 6972 6f6e  g Poetry Environ
+00015300: 6d65 6e74 222c 2050 7943 6861 726d 2073  ment", PyCharm s
+00015310: 6f6d 6574 696d 6573 2068 6173 2073 6f6d  ometimes has som
+00015320: 650a 6973 7375 6573 2028 646f 6e27 7420  e.issues (don't 
+00015330: 6b6e 6f77 2077 6879 2920 7768 6963 6820  know why) which 
+00015340: 6d69 6768 7420 6265 2070 726f 626c 656d  might be problem
+00015350: 6174 6963 2e20 4966 2079 6f75 2065 6e63  atic. If you enc
+00015360: 6f75 6e74 6572 2073 7563 680a 6973 7375  ounter such.issu
+00015370: 6573 2c20 796f 7520 6361 6e20 7265 736f  es, you can reso
+00015380: 6c76 6520 7468 6573 6520 6973 7375 6573  lve these issues
+00015390: 2062 7920 6465 6c65 7469 6e67 2074 6865   by deleting the
+000153a0: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
+000153b0: 6d65 6e74 0a61 6e64 2063 7265 6174 696e  ment.and creatin
+000153c0: 6720 7468 6520 506f 6574 7279 2076 6972  g the Poetry vir
+000153d0: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
+000153e0: 2075 7369 6e67 2050 7943 6861 726d 2028   using PyCharm (
+000153f0: 7365 6520 6162 6f76 6529 2e0a 0a23 2323  see above)...###
+00015400: 2050 726f 6a65 6374 204d 616b 6566 696c   Project Makefil
+00015410: 6520 636f 6d6d 616e 6473 0a0a 596f 7520  e commands..You 
+00015420: 6361 6e20 7374 6172 7420 4576 656e 7453  can start EventS
+00015430: 746f 7265 4442 2075 7369 6e67 2074 6865  toreDB using the
+00015440: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
+00015450: 6e64 2e0a 0a20 2020 2024 206d 616b 6520  nd...    $ make 
+00015460: 7374 6172 742d 6576 656e 7473 746f 7265  start-eventstore
+00015470: 6462 0a0a 596f 7520 6361 6e20 7275 6e20  db..You can run 
+00015480: 7465 7374 7320 7573 696e 6720 7468 6520  tests using the 
+00015490: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+000154a0: 6420 286e 6565 6473 2045 7665 6e74 5374  d (needs EventSt
+000154b0: 6f72 6544 4220 746f 2062 6520 7275 6e6e  oreDB to be runn
+000154c0: 696e 6729 2e0a 0a20 2020 2024 206d 616b  ing)...    $ mak
+000154d0: 6520 7465 7374 0a0a 596f 7520 6361 6e20  e test..You can 
+000154e0: 7374 6f70 2045 7665 6e74 5374 6f72 6544  stop EventStoreD
+000154f0: 4220 7573 696e 6720 7468 6520 666f 6c6c  B using the foll
+00015500: 6f77 696e 6720 636f 6d6d 616e 642e 0a0a  owing command...
+00015510: 2020 2020 2420 6d61 6b65 2073 746f 702d      $ make stop-
+00015520: 6576 656e 7473 746f 7265 6462 0a0a 596f  eventstoredb..Yo
+00015530: 7520 6361 6e20 6368 6563 6b20 7468 6520  u can check the 
+00015540: 666f 726d 6174 7469 6e67 206f 6620 7468  formatting of th
+00015550: 6520 636f 6465 2075 7369 6e67 2074 6865  e code using the
+00015560: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
+00015570: 6e64 2e0a 0a20 2020 2024 206d 616b 6520  nd...    $ make 
+00015580: 6c69 6e74 0a0a 596f 7520 6361 6e20 7265  lint..You can re
+00015590: 666f 726d 6174 2074 6865 2063 6f64 6520  format the code 
+000155a0: 7573 696e 6720 7468 6520 666f 6c6c 6f77  using the follow
+000155b0: 696e 6720 636f 6d6d 616e 642e 0a0a 2020  ing command...  
+000155c0: 2020 2420 6d61 6b65 2066 6d74 0a0a 5465    $ make fmt..Te
+000155d0: 7374 7320 6265 6c6f 6e67 2069 6e20 602e  sts belong in `.
+000155e0: 2f74 6573 7473 602e 2043 6f64 652d 756e  /tests`. Code-un
+000155f0: 6465 722d 7465 7374 2062 656c 6f6e 6773  der-test belongs
+00015600: 2069 6e20 602e 2f65 7364 6263 6c69 656e   in `./esdbclien
+00015610: 7460 2e0a 0a45 6469 7420 7061 636b 6167  t`...Edit packag
+00015620: 6520 6465 7065 6e64 656e 6369 6573 2069  e dependencies i
+00015630: 6e20 6070 7970 726f 6a65 6374 2e74 6f6d  n `pyproject.tom
+00015640: 6c60 2e20 5570 6461 7465 2069 6e73 7461  l`. Update insta
+00015650: 6c6c 6564 2070 6163 6b61 6765 7320 2861  lled packages (a
+00015660: 6e64 2074 6865 0a60 706f 6574 7279 2e6c  nd the.`poetry.l
+00015670: 6f63 6b60 2066 696c 6529 2075 7369 6e67  ock` file) using
+00015680: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00015690: 6f6d 6d61 6e64 2e0a 0a20 2020 2024 206d  ommand...    $ m
+000156a0: 616b 6520 7570 6461 7465 2d70 6163 6b61  ake update-packa
+000156b0: 6765 730a 0a                             ges..
```

