# Comparing `tmp/syft-0.8.0b9.tar.gz` & `tmp/syft-0.8.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.0b9.tar", last modified: Sun Apr 23 13:01:36 2023, max compression
+gzip compressed data, was "syft-0.8.1b1.tar", last modified: Sun May  7 12:48:27 2023, max compression
```

## Comparing `syft-0.8.0b9.tar` & `syft-0.8.1b1.tar`

### file list

```diff
@@ -1,174 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.672410 syft-0.8.0b9/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-23 12:59:19.000000 syft-0.8.0b9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 12:59:19.000000 syft-0.8.0b9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-04-23 13:01:36.672410 syft-0.8.0b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-04-23 12:59:18.000000 syft-0.8.0b9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-23 12:59:19.000000 syft-0.8.0b9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-23 13:01:36.676410 syft-0.8.0b9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-23 12:59:19.000000 syft-0.8.0b9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.652410 syft-0.8.0b9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.656410 syft-0.8.0b9/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-23 12:59:33.000000 syft-0.8.0b9/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-23 12:59:33.000000 syft-0.8.0b9/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.660410 syft-0.8.0b9/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.660410 syft-0.8.0b9/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19073 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21112 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.660410 syft-0.8.0b9/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.660410 syft-0.8.0b9/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.660410 syft-0.8.0b9/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    26881 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.664410 syft-0.8.0b9/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.664410 syft-0.8.0b9/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.664410 syft-0.8.0b9/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    26733 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.664410 syft-0.8.0b9/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    21157 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.664410 syft-0.8.0b9/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/message/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/message/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/message/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/metadata/metadata_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/network/network_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/queue/queue_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.668410 syft-0.8.0b9/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.672410 syft-0.8.0b9/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.672410 syft-0.8.0b9/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.672410 syft-0.8.0b9/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-23 12:59:19.000000 syft-0.8.0b9/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:01:36.656410 syft-0.8.0b9/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 13:01:36.000000 syft-0.8.0b9/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.060686 syft-0.8.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-05-07 12:45:55.000000 syft-0.8.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-07 12:45:55.000000 syft-0.8.1b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-07 12:48:27.060686 syft-0.8.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-07 12:45:54.000000 syft-0.8.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-07 12:45:55.000000 syft-0.8.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-07 12:48:27.064686 syft-0.8.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-07 12:45:55.000000 syft-0.8.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.036685 syft-0.8.1b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.036685 syft-0.8.1b1/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-07 12:46:11.000000 syft-0.8.1b1/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-07 12:46:11.000000 syft-0.8.1b1/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.040685 syft-0.8.1b1/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.040685 syft-0.8.1b1/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23296 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21112 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.040685 syft-0.8.1b1/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.044685 syft-0.8.1b1/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.044685 syft-0.8.1b1/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26952 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.048685 syft-0.8.1b1/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/serde/third_party.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.048685 syft-0.8.1b1/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.048685 syft-0.8.1b1/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37961 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21160 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.048685 syft-0.8.1b1/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21157 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.052686 syft-0.8.1b1/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.052686 syft-0.8.1b1/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.052686 syft-0.8.1b1/src/syft/service/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/message/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/message/message_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/message/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.052686 syft-0.8.1b1/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/metadata/metadata_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.052686 syft-0.8.1b1/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/network/network_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.052686 syft-0.8.1b1/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.056686 syft-0.8.1b1/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.056686 syft-0.8.1b1/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/queue/queue_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.056686 syft-0.8.1b1/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16568 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.056686 syft-0.8.1b1/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.060686 syft-0.8.1b1/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.060686 syft-0.8.1b1/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.060686 syft-0.8.1b1/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-07 12:45:55.000000 syft-0.8.1b1/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:48:27.036685 syft-0.8.1b1/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-07 12:48:27.000000 syft-0.8.1b1/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-07 12:48:27.000000 syft-0.8.1b1/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:48:27.000000 syft-0.8.1b1/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-07 12:48:27.000000 syft-0.8.1b1/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:48:26.000000 syft-0.8.1b1/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-07 12:48:27.000000 syft-0.8.1b1/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 12:48:27.000000 syft-0.8.1b1/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.0b9/LICENSE` & `syft-0.8.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/PKG-INFO` & `syft-0.8.1b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,48 @@
-Metadata-Version: 2.1
-Name: syft
-Version: 0.8.0b9
-Summary: Perform numpy-like analysis on data that remains in someone elses server
-Home-page: https://openmined.github.io/PySyft/
-Author: OpenMined
-Author-email: info@openmined.org
-License: Apache-2.0
-Project-URL: Source, https://github.com/OpenMined/PySyft
-Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Provides-Extra: dev
-Provides-Extra: test_plugins
-Provides-Extra: oblv
-License-File: LICENSE
-
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://pepy.tech/badge/syft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/img/title_syft_dark.png">
   <img alt="Syft Logo" src="docs/img/title_syft_light.png" width="200px" />
 </picture>
 
 Perform `numpy`-like analysis on `data` that remains in `someone else's` server
 
-<div align="left">
-<img alt="Syft Logo" src="docs/img/header.png" alt="Syft Overview" width="100%" />
-</div>
-
 # Quickstart
 
 ✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
 
-## Install syft on Python 3.8 - 3.10
+## Install syft on Python 3.9 - 3.10
 
 ```bash
-$ pip install --pre syft -f https://whls.blob.core.windows.net/unstable/index.html
+$ pip install -U syft -f https://whls.blob.core.windows.net/unstable/index.html
 ```
 
 ## Launch a python dev Domain
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8-beta")
+sy.requires(">=0.8,<0.8.1")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Connect with our Python Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8-beta")
+sy.requires(">=0.8,<0.8.1")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## Deploy to a Container Engine or Cloud
 
 1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server a one-liner:  
    `pip install -U hagrid`
@@ -79,34 +55,36 @@
 
    `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
 
 4. During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `podman` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†
 
 ## Docs and Support
 
+- 📝 <a href="/notebooks/api">API Example Notebooks</a>
 - 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
 - HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
   †`Windows` does not support `ansible`, preventing some remote deployment targets
-- PySyft 0.8 Requires: 🐍 `python 3.8 - 3.10` - Run: `pip install -U syft`  
+- PySyft 0.8 Requires: 🐍 `python 3.9 - 3.10` - Run: `pip install -U syft`  
   \*`macOS` Apple Silicon users might need cmake: `brew install cmake`  
   ‡`Windows` users must run this first: `pip install jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html`
 - PyGrid Requires: 🐳 `docker` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
 
 # Versions
 
-`0.8.0` (Beta) - `dev` branch 👈🏽  
-`0.7.0` (Stable) - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
+`0.8.1` (Beta) - `dev` branch 👈🏽 <a href="/notebooks/api/0.8">API</a>  
+`0.8.0` (Stable) - <a href="/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
 - `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
 
 PySyft (Stable): `pip install -U syft`
```

#### html2text {}

```diff
@@ -1,81 +1,72 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.0b9 Summary: Perform numpy-like
-analysis on data that remains in someone elses server Home-page: https://
-openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
-License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
-Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
-Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
-Python Requires-Python: >=3.8 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
-Provides-Extra: oblv License-File: LICENSE
 [https://pepy.tech/badge/syft] [https://badge.fury.io/py/syft.svg] [https://
 img.shields.io/badge/docker-images-blue?logo=docker] [https://github.com/
 OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev] [https:/
 /img.shields.io/badge/chat-on%20slack-purple?logo=slack] [https://
 img.shields.io/badge/read-docs-yellow?logo=mdbook]
 
   [Syft Logo]  Perform `numpy`-like analysis on `data` that remains in `someone
-else's` server
-[Syft Logo]
-# Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ## Install syft on
-Python 3.8 - 3.10 ```bash $ pip install --pre syft -f https://
+else's` server # Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ##
+Install syft on Python 3.9 - 3.10 ```bash $ pip install -U syft -f https://
 whls.blob.core.windows.net/unstable/index.html ``` ## Launch a python dev
-Domain ```python # from Jupyter / Python import syft as sy sy.requires(">=0.8-
-beta") node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True,
-reset=True) ``` ```bash # or from the command line $ syft launch --name=my-
-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:8080 ```
-## Connect with our Python Client ```python import syft as sy sy.requires
-(">=0.8-beta") domain_client = sy.login(port=8080, email="info@openmined.org",
-password="changethis") ``` ## Deploy to a Container Engine or Cloud 1. Install
-our handy ðµ cli tool which makes deploying a Domain or Gateway server a one-
-liner: `pip install -U hagrid` 2. Then run our interactive jupyter Install
-ð§ð½ââï¸ WizardBETA: `hagrid quickstart` 3. In the tutorial you will
-learn how to install and deploy: `PySyft` = our `numpy`-like ð Python
-library for computing on `private data` in someone else's `Domain` `PyGrid` =
-our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where `private data`
-lives 4. During quickstart we will deploy `PyGrid` to localhost with ð³
-`docker`, however ðµ HAGrid can deploy to `podman` or a ð§ `ubuntu` VM on
-`azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨ `ansible`â  ## Docs and
-Support - ð Docs - `#support` on Slack # Install Notes - HAGrid 0.3
-Requires: ð `python` ð `git` - Run: `pip install -U hagrid` - Interactive
-Install ð§ð½ââï¸ WizardBETA Requires ðµ `hagrid`: - Run: `hagrid
-quickstart` â `Windows` does not support `ansible`, preventing some remote
-deployment targets - PySyft 0.8 Requires: ð `python 3.8 - 3.10` - Run: `pip
-install -U syft` \*`macOS` Apple Silicon users might need cmake: `brew install
-cmake` â¡`Windows` users must run this first: `pip install jaxlib==0.3.14 -
-f https://whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires:
-ð³ `docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.0`
-(Beta) - `dev` branch ðð½ `0.7.0` (Stable) - Course_3_Updated Deprecated:
-- `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix - `0.2.0` - `0.5.0`
-PySyft and PyGrid use the same `version` and its best to match them up where
-possible. We release weekly betas which can be used in each context: PySyft
-(Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch ... tag=latest`
-PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta): `hagrid launch ...
-tag=beta` HAGrid is a cli / deployment tool so the latest version of `hagrid`
-is usually the best. # What is Syft?   [Syft]  `Syft` is OpenMined's `open
-source` stack that provides `secure` and `private` Data Science in Python. Syft
-decouples `private data` from model training, using techniques like [Federated
-Learning](https://ai.googleblog.com/2017/04/federated-learning-
-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/
-Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/
-wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and
-integration with `Deep Learning` frameworks, so that you as a `Data Scientist`
-can maintain your current workflow while using these new `privacy-enhancing
-techniques`. ### Why should I use Syft? `Syft` allows a `Data Scientist` to ask
-`questions` about a `dataset` and, within `privacy limits` set by the `data
-owner`, get `answers` to those `questions`, all without obtaining a `copy` of
-the data itself. We call this process `Remote Data Science`. It means in a wide
-variety of `domains` across society, the current `risks` of sharing information
-(`copying` data) with someone such as, privacy invasion, IP theft and blackmail
-will no longer prevent the vast `benefits` such as innovation, insights and
-scientific discovery which secure access will provide. No more cold calls to
-get `access` to a dataset. No more weeks of `wait times` to get a `result` on
-your `query`. It also means `1000x more data` in every domain. PySyft opens the
-doors to a streamlined Data Scientist `workflow`, all with the individual's
-`privacy` at its heart. # Tutorials
+Domain ```python # from Jupyter / Python import syft as sy sy.requires
+(">=0.8,<0.8.1") node = sy.orchestra.launch(name="my-domain", port=8080,
+dev_mode=True, reset=True) ``` ```bash # or from the command line $ syft launch
+--name=my-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:
+8080 ``` ## Connect with our Python Client ```python import syft as sy
+sy.requires(">=0.8,<0.8.1") domain_client = sy.login(port=8080,
+email="info@openmined.org", password="changethis") ``` ## Deploy to a Container
+Engine or Cloud 1. Install our handy ðµ cli tool which makes deploying a
+Domain or Gateway server a one-liner: `pip install -U hagrid` 2. Then run our
+interactive jupyter Install ð§ð½ââï¸ WizardBETA: `hagrid quickstart`
+3. In the tutorial you will learn how to install and deploy: `PySyft` = our
+`numpy`-like ð Python library for computing on `private data` in someone
+else's `Domain` `PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway`
+Servers where `private data` lives 4. During quickstart we will deploy `PyGrid`
+to localhost with ð³ `docker`, however ðµ HAGrid can deploy to `podman` or
+a ð§ `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨
+`ansible`â  ## Docs and Support - ð API_Example_Notebooks - ð Docs -
+`#support` on Slack # Install Notes - HAGrid 0.3 Requires: ð `python` ð
+`git` - Run: `pip install -U hagrid` - Interactive Install ð§ð½ââï¸
+WizardBETA Requires ðµ `hagrid`: - Run: `hagrid quickstart` â `Windows` does
+not support `ansible`, preventing some remote deployment targets - PySyft 0.8
+Requires: ð `python 3.9 - 3.10` - Run: `pip install -U syft` \*`macOS` Apple
+Silicon users might need cmake: `brew install cmake` â¡`Windows` users must
+run this first: `pip install jaxlib==0.3.14 -f https://
+whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires: ð³
+`docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.1`
+(Beta) - `dev` branch ðð½ API `0.8.0` (Stable) - API Deprecated: - `0.7.0`
+- Course_3_Updated - `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix -
+`0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
+match them up where possible. We release weekly betas which can be used in each
+context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
+... tag=latest` PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta):
+`hagrid launch ... tag=beta` HAGrid is a cli / deployment tool so the latest
+version of `hagrid` is usually the best. # What is Syft?   [Syft]  `Syft` is
+OpenMined's `open source` stack that provides `secure` and `private` Data
+Science in Python. Syft decouples `private data` from model training, using
+techniques like [Federated Learning](https://ai.googleblog.com/2017/04/
+federated-learning-collaborative.html), [Differential Privacy](https://
+en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https:
+//en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-
+like interface and integration with `Deep Learning` frameworks, so that you as
+a `Data Scientist` can maintain your current workflow while using these new
+`privacy-enhancing techniques`. ### Why should I use Syft? `Syft` allows a
+`Data Scientist` to ask `questions` about a `dataset` and, within `privacy
+limits` set by the `data owner`, get `answers` to those `questions`, all
+without obtaining a `copy` of the data itself. We call this process `Remote
+Data Science`. It means in a wide variety of `domains` across society, the
+current `risks` of sharing information (`copying` data) with someone such as,
+privacy invasion, IP theft and blackmail will no longer prevent the vast
+`benefits` such as innovation, insights and scientific discovery which secure
+access will provide. No more cold calls to get `access` to a dataset. No more
+weeks of `wait times` to get a `result` on your `query`. It also means `1000x
+more data` in every domain. PySyft opens the doors to a streamlined Data
+Scientist `workflow`, all with the individual's `privacy` at its heart. #
+Tutorials
  _____________________________________________________________________________
 |             [Image]     |            [Image]      |            [Image]      |
 |___________Data_Owner____|________Data_Scientist___|_________Data_Engineer___|
 |- Deploy_a_Domain_Server |- Install Syft           |- Setup Dev Mode         |
 |- Upload_Private_Data -  | - Connect to a Domain   | - Deploy to Azure -     |
 |Create_Accounts - Manage | - Search for Datasets   |Deploy to GCP - Deploy to|
 |Privacy Budget           | - Train Models -        |Kubernetes - Customize   |
```

### Comparing `syft-0.8.0b9/README.md` & `syft-0.8.1b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,68 @@
+Metadata-Version: 2.1
+Name: syft
+Version: 0.8.1b1
+Summary: Perform numpy-like analysis on data that remains in someone elses server
+Home-page: https://openmined.github.io/PySyft/
+Author: OpenMined
+Author-email: info@openmined.org
+License: Apache-2.0
+Project-URL: Source, https://github.com/OpenMined/PySyft
+Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: dev
+Provides-Extra: test_plugins
+Provides-Extra: oblv
+License-File: LICENSE
+
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://pepy.tech/badge/syft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/img/title_syft_dark.png">
   <img alt="Syft Logo" src="docs/img/title_syft_light.png" width="200px" />
 </picture>
 
 Perform `numpy`-like analysis on `data` that remains in `someone else's` server
 
-<div align="left">
-<img alt="Syft Logo" src="docs/img/header.png" alt="Syft Overview" width="100%" />
-</div>
-
 # Quickstart
 
 ✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
 
-## Install syft on Python 3.8 - 3.10
+## Install syft on Python 3.9 - 3.10
 
 ```bash
-$ pip install --pre syft -f https://whls.blob.core.windows.net/unstable/index.html
+$ pip install -U syft -f https://whls.blob.core.windows.net/unstable/index.html
 ```
 
 ## Launch a python dev Domain
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8-beta")
+sy.requires(">=0.8,<0.8.1")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Connect with our Python Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8-beta")
+sy.requires(">=0.8,<0.8.1")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## Deploy to a Container Engine or Cloud
 
 1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server a one-liner:  
    `pip install -U hagrid`
@@ -59,34 +75,36 @@
 
    `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
 
 4. During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `podman` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†
 
 ## Docs and Support
 
+- 📝 <a href="/notebooks/api">API Example Notebooks</a>
 - 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
 - HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
   †`Windows` does not support `ansible`, preventing some remote deployment targets
-- PySyft 0.8 Requires: 🐍 `python 3.8 - 3.10` - Run: `pip install -U syft`  
+- PySyft 0.8 Requires: 🐍 `python 3.9 - 3.10` - Run: `pip install -U syft`  
   \*`macOS` Apple Silicon users might need cmake: `brew install cmake`  
   ‡`Windows` users must run this first: `pip install jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html`
 - PyGrid Requires: 🐳 `docker` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
 
 # Versions
 
-`0.8.0` (Beta) - `dev` branch 👈🏽  
-`0.7.0` (Stable) - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
+`0.8.1` (Beta) - `dev` branch 👈🏽 <a href="/notebooks/api/0.8">API</a>  
+`0.8.0` (Stable) - <a href="/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
 - `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
 
 PySyft (Stable): `pip install -U syft`
```

#### html2text {}

```diff
@@ -1,72 +1,81 @@
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b1 Summary: Perform numpy-like
+analysis on data that remains in someone elses server Home-page: https://
+openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
+License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
+Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
+Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
+Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
+charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
+Provides-Extra: oblv License-File: LICENSE
 [https://pepy.tech/badge/syft] [https://badge.fury.io/py/syft.svg] [https://
 img.shields.io/badge/docker-images-blue?logo=docker] [https://github.com/
 OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev] [https:/
 /img.shields.io/badge/chat-on%20slack-purple?logo=slack] [https://
 img.shields.io/badge/read-docs-yellow?logo=mdbook]
 
   [Syft Logo]  Perform `numpy`-like analysis on `data` that remains in `someone
-else's` server
-[Syft Logo]
-# Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ## Install syft on
-Python 3.8 - 3.10 ```bash $ pip install --pre syft -f https://
+else's` server # Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ##
+Install syft on Python 3.9 - 3.10 ```bash $ pip install -U syft -f https://
 whls.blob.core.windows.net/unstable/index.html ``` ## Launch a python dev
-Domain ```python # from Jupyter / Python import syft as sy sy.requires(">=0.8-
-beta") node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True,
-reset=True) ``` ```bash # or from the command line $ syft launch --name=my-
-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:8080 ```
-## Connect with our Python Client ```python import syft as sy sy.requires
-(">=0.8-beta") domain_client = sy.login(port=8080, email="info@openmined.org",
-password="changethis") ``` ## Deploy to a Container Engine or Cloud 1. Install
-our handy ðµ cli tool which makes deploying a Domain or Gateway server a one-
-liner: `pip install -U hagrid` 2. Then run our interactive jupyter Install
-ð§ð½ââï¸ WizardBETA: `hagrid quickstart` 3. In the tutorial you will
-learn how to install and deploy: `PySyft` = our `numpy`-like ð Python
-library for computing on `private data` in someone else's `Domain` `PyGrid` =
-our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where `private data`
-lives 4. During quickstart we will deploy `PyGrid` to localhost with ð³
-`docker`, however ðµ HAGrid can deploy to `podman` or a ð§ `ubuntu` VM on
-`azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨ `ansible`â  ## Docs and
-Support - ð Docs - `#support` on Slack # Install Notes - HAGrid 0.3
-Requires: ð `python` ð `git` - Run: `pip install -U hagrid` - Interactive
-Install ð§ð½ââï¸ WizardBETA Requires ðµ `hagrid`: - Run: `hagrid
-quickstart` â `Windows` does not support `ansible`, preventing some remote
-deployment targets - PySyft 0.8 Requires: ð `python 3.8 - 3.10` - Run: `pip
-install -U syft` \*`macOS` Apple Silicon users might need cmake: `brew install
-cmake` â¡`Windows` users must run this first: `pip install jaxlib==0.3.14 -
-f https://whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires:
-ð³ `docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.0`
-(Beta) - `dev` branch ðð½ `0.7.0` (Stable) - Course_3_Updated Deprecated:
-- `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix - `0.2.0` - `0.5.0`
-PySyft and PyGrid use the same `version` and its best to match them up where
-possible. We release weekly betas which can be used in each context: PySyft
-(Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch ... tag=latest`
-PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta): `hagrid launch ...
-tag=beta` HAGrid is a cli / deployment tool so the latest version of `hagrid`
-is usually the best. # What is Syft?   [Syft]  `Syft` is OpenMined's `open
-source` stack that provides `secure` and `private` Data Science in Python. Syft
-decouples `private data` from model training, using techniques like [Federated
-Learning](https://ai.googleblog.com/2017/04/federated-learning-
-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/
-Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/
-wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and
-integration with `Deep Learning` frameworks, so that you as a `Data Scientist`
-can maintain your current workflow while using these new `privacy-enhancing
-techniques`. ### Why should I use Syft? `Syft` allows a `Data Scientist` to ask
-`questions` about a `dataset` and, within `privacy limits` set by the `data
-owner`, get `answers` to those `questions`, all without obtaining a `copy` of
-the data itself. We call this process `Remote Data Science`. It means in a wide
-variety of `domains` across society, the current `risks` of sharing information
-(`copying` data) with someone such as, privacy invasion, IP theft and blackmail
-will no longer prevent the vast `benefits` such as innovation, insights and
-scientific discovery which secure access will provide. No more cold calls to
-get `access` to a dataset. No more weeks of `wait times` to get a `result` on
-your `query`. It also means `1000x more data` in every domain. PySyft opens the
-doors to a streamlined Data Scientist `workflow`, all with the individual's
-`privacy` at its heart. # Tutorials
+Domain ```python # from Jupyter / Python import syft as sy sy.requires
+(">=0.8,<0.8.1") node = sy.orchestra.launch(name="my-domain", port=8080,
+dev_mode=True, reset=True) ``` ```bash # or from the command line $ syft launch
+--name=my-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:
+8080 ``` ## Connect with our Python Client ```python import syft as sy
+sy.requires(">=0.8,<0.8.1") domain_client = sy.login(port=8080,
+email="info@openmined.org", password="changethis") ``` ## Deploy to a Container
+Engine or Cloud 1. Install our handy ðµ cli tool which makes deploying a
+Domain or Gateway server a one-liner: `pip install -U hagrid` 2. Then run our
+interactive jupyter Install ð§ð½ââï¸ WizardBETA: `hagrid quickstart`
+3. In the tutorial you will learn how to install and deploy: `PySyft` = our
+`numpy`-like ð Python library for computing on `private data` in someone
+else's `Domain` `PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway`
+Servers where `private data` lives 4. During quickstart we will deploy `PyGrid`
+to localhost with ð³ `docker`, however ðµ HAGrid can deploy to `podman` or
+a ð§ `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨
+`ansible`â  ## Docs and Support - ð API_Example_Notebooks - ð Docs -
+`#support` on Slack # Install Notes - HAGrid 0.3 Requires: ð `python` ð
+`git` - Run: `pip install -U hagrid` - Interactive Install ð§ð½ââï¸
+WizardBETA Requires ðµ `hagrid`: - Run: `hagrid quickstart` â `Windows` does
+not support `ansible`, preventing some remote deployment targets - PySyft 0.8
+Requires: ð `python 3.9 - 3.10` - Run: `pip install -U syft` \*`macOS` Apple
+Silicon users might need cmake: `brew install cmake` â¡`Windows` users must
+run this first: `pip install jaxlib==0.3.14 -f https://
+whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires: ð³
+`docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.1`
+(Beta) - `dev` branch ðð½ API `0.8.0` (Stable) - API Deprecated: - `0.7.0`
+- Course_3_Updated - `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix -
+`0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
+match them up where possible. We release weekly betas which can be used in each
+context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
+... tag=latest` PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta):
+`hagrid launch ... tag=beta` HAGrid is a cli / deployment tool so the latest
+version of `hagrid` is usually the best. # What is Syft?   [Syft]  `Syft` is
+OpenMined's `open source` stack that provides `secure` and `private` Data
+Science in Python. Syft decouples `private data` from model training, using
+techniques like [Federated Learning](https://ai.googleblog.com/2017/04/
+federated-learning-collaborative.html), [Differential Privacy](https://
+en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https:
+//en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-
+like interface and integration with `Deep Learning` frameworks, so that you as
+a `Data Scientist` can maintain your current workflow while using these new
+`privacy-enhancing techniques`. ### Why should I use Syft? `Syft` allows a
+`Data Scientist` to ask `questions` about a `dataset` and, within `privacy
+limits` set by the `data owner`, get `answers` to those `questions`, all
+without obtaining a `copy` of the data itself. We call this process `Remote
+Data Science`. It means in a wide variety of `domains` across society, the
+current `risks` of sharing information (`copying` data) with someone such as,
+privacy invasion, IP theft and blackmail will no longer prevent the vast
+`benefits` such as innovation, insights and scientific discovery which secure
+access will provide. No more cold calls to get `access` to a dataset. No more
+weeks of `wait times` to get a `result` on your `query`. It also means `1000x
+more data` in every domain. PySyft opens the doors to a streamlined Data
+Scientist `workflow`, all with the individual's `privacy` at its heart. #
+Tutorials
  _____________________________________________________________________________
 |             [Image]     |            [Image]      |            [Image]      |
 |___________Data_Owner____|________Data_Scientist___|_________Data_Engineer___|
 |- Deploy_a_Domain_Server |- Install Syft           |- Setup Dev Mode         |
 |- Upload_Private_Data -  | - Connect to a Domain   | - Deploy to Azure -     |
 |Create_Accounts - Manage | - Search for Datasets   |Deploy to GCP - Deploy to|
 |Privacy Budget           | - Train Models -        |Kubernetes - Customize   |
```

### Comparing `syft-0.8.0b9/setup.cfg` & `syft-0.8.1b1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.0-beta.9"
+version = attr: "0.8.1-beta.1"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -57,15 +57,15 @@
 	opentelemetry-sdk==1.14.0
 	opentelemetry-exporter-jaeger==1.14.0
 	opentelemetry-instrumentation==0.35b0
 	opentelemetry-instrumentation-requests==0.35b0
 install_requires = 
 	%(syft)s
 	%(telemetry)s
-python_requires = >=3.8
+python_requires = >=3.9
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `syft-0.8.0b9/src/syft/VERSION` & `syft-0.8.1b1/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.0-beta.9"
+__version__ = "0.8.1-beta.1"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.0b9/src/syft/__init__.py` & `syft-0.8.1b1/src/syft/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0-beta.9"
+__version__ = "0.8.1-beta.1"
 
 # stdlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
 
@@ -53,15 +53,15 @@
 from .util import filterwarnings  # noqa: F401
 from .util import jax_settings  # noqa: F401
 from .util import logger  # noqa: F401
 from .util.telemetry import instrument  # noqa: F401
 from .util.util import autocache  # noqa: F401
 from .util.version_compare import make_requires
 
-LATEST_STABLE_SYFT = "0.7"
+LATEST_STABLE_SYFT = "0.8"
 requires = make_requires(LATEST_STABLE_SYFT, __version__)
 
 sys.path.append(str(Path(__file__)))
 
 logger.start()
 
 # For server-side, to enable by environment variable
```

### Comparing `syft-0.8.0b9/src/syft/abstract_node.py` & `syft-0.8.1b1/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/client/api.py` & `syft-0.8.1b1/src/syft/client/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,18 +32,20 @@
 from ..serde.signature import Signature
 from ..serde.signature import signature_remove_context
 from ..serde.signature import signature_remove_self
 from ..service.context import AuthedServiceContext
 from ..service.response import SyftAttributeError
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
+from ..service.service import UserLibConfigRegistry
 from ..service.service import UserServiceConfigRegistry
 from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftObject
+from ..types.uid import LineageID
 from ..types.uid import UID
 from ..util.telemetry import instrument
 from .connection import NodeConnection
 
 
 class APIRegistry:
     __api_registry__: Dict[str, SyftAPI] = {}
@@ -61,15 +63,29 @@
     @classmethod
     def get_all_api(cls) -> List[SyftAPI]:
         return list(cls.__api_registry__.values())
 
 
 @serializable()
 class APIEndpoint(SyftBaseObject):
-    path: str
+    service_path: str
+    module_path: str
+    name: str
+    description: str
+    doc_string: Optional[str]
+    signature: Signature
+    has_self: bool = False
+    pre_kwargs: Optional[Dict[str, Any]]
+
+
+@serializable()
+class LibEndpoint(SyftBaseObject):
+    # TODO: bad name, change
+    service_path: str
+    module_path: str
     name: str
     description: str
     doc_string: Optional[str]
     signature: Signature
     has_self: bool = False
     pre_kwargs: Optional[Dict[str, Any]]
 
@@ -167,96 +183,102 @@
 
     def wrapper(*args, **kwargs):
         blocking = True
         if "blocking" in kwargs:
             blocking = bool(kwargs["blocking"])
             del kwargs["blocking"]
 
-        _valid_kwargs = {}
-        if "kwargs" in signature.parameters:
-            _valid_kwargs = kwargs
-        else:
-            for key, value in kwargs.items():
-                if key not in signature.parameters:
-                    return SyftError(
-                        message=f"""Invalid parameter: `{key}`. Valid Parameters: {list(signature.parameters)}"""
-                    )
-                param = signature.parameters[key]
-                if isinstance(param.annotation, str):
-                    # 🟡 TODO 21: make this work for weird string type situations
-                    # happens when from __future__ import annotations in a class file
-                    t = index_syft_by_module_name(param.annotation)
-                else:
-                    t = param.annotation
-                msg = None
-                try:
-                    if t is not inspect.Parameter.empty:
-                        if isinstance(t, _GenericAlias) and type(None) in t.__args__:
-                            for v in t.__args__:
-                                if issubclass(v, EmailStr):
-                                    v = str
-                                check_type(key, value, v)  # raises Exception
-                                break  # only need one to match
-                        else:
-                            check_type(key, value, t)  # raises Exception
-                except TypeError:
-                    _type_str = getattr(t, "__name__", str(t))
-                    msg = f"`{key}` must be of type `{_type_str}` not `{type(value).__name__}`"
-
-                if msg:
-                    return SyftError(message=msg)
-
-                _valid_kwargs[key] = value
-
-        # signature.parameters is an OrderedDict, therefore,
-        # its fair to assume that order of args
-        # and the signature.parameters should always match
-        _valid_args = []
-        if "args" in signature.parameters:
-            _valid_args = args
-        else:
-            for (param_key, param), arg in zip(signature.parameters.items(), args):
-                if param_key in _valid_kwargs:
-                    continue
-                t = param.annotation
-                msg = None
-                try:
-                    if t is not inspect.Parameter.empty:
-                        if isinstance(t, _GenericAlias) and type(None) in t.__args__:
-                            for v in t.__args__:
-                                if issubclass(v, EmailStr):
-                                    v = str
-                                check_type(param_key, arg, v)  # raises Exception
-                                break  # only need one to match
-                        else:
-                            check_type(param_key, arg, t)  # raises Exception
-                except TypeError:
-                    _type_str = getattr(t, "__name__", str(t))
-                    msg = f"Arg: {arg} must be {_type_str} not {type(arg).__name__}"
-                if msg:
-                    return SyftError(message=msg)
+        res = validate_callable_args_and_kwargs(args, kwargs, signature)
 
-                _valid_args.append(arg)
+        if isinstance(res, SyftError):
+            return res
+        _valid_args, _valid_kwargs = res
 
         if pre_kwargs:
             _valid_kwargs.update(pre_kwargs)
+
         api_call = SyftAPICall(
             node_uid=node_uid,
             path=path,
             args=_valid_args,
             kwargs=_valid_kwargs,
             blocking=blocking,
         )
         result = make_call(api_call=api_call)
         return result
 
     wrapper.__ipython_inspector_signature_override__ = signature
     return wrapper
 
 
+def generate_remote_lib_function(
+    api: SyftAPI,
+    node_uid: UID,
+    signature: Signature,
+    path: str,
+    module_path: str,
+    make_call: Callable,
+    pre_kwargs: Dict[str, Any],
+):
+    if "blocking" in signature.parameters:
+        raise Exception(
+            f"Signature {signature} can't have 'blocking' kwarg because its reserved"
+        )
+
+    def wrapper(*args, **kwargs):
+        blocking = True
+        if "blocking" in kwargs:
+            blocking = bool(kwargs["blocking"])
+            del kwargs["blocking"]
+
+        res = validate_callable_args_and_kwargs(args, kwargs, signature)
+
+        if isinstance(res, SyftError):
+            return res
+        _valid_args, _valid_kwargs = res
+
+        if pre_kwargs:
+            _valid_kwargs.update(pre_kwargs)
+
+        # relative
+        from ..service.action.action_object import Action
+        from ..service.action.action_object import convert_to_pointers
+
+        action_args, action_kwargs = convert_to_pointers(
+            api, node_uid, _valid_args, _valid_kwargs
+        )
+
+        # e.g. numpy.array -> numpy, array
+        module, op = module_path.rsplit(".", 1)
+        service_args = [
+            Action(
+                path=module,
+                op=op,
+                remote_self=None,
+                args=[x.syft_lineage_id for x in action_args],
+                kwargs={k: v.syft_lineage_id for k, v in action_kwargs},
+                # TODO: fix
+                result_id=LineageID(UID(), 1),
+            )
+        ]
+
+        api_call = SyftAPICall(
+            node_uid=node_uid,
+            path=path,
+            args=service_args,
+            kwargs=dict(),
+            blocking=blocking,
+        )
+        result = make_call(api_call=api_call)
+        return result
+
+    wrapper.__ipython_inspector_signature_override__ = signature
+    return wrapper
+
+
 @serializable()
 class APIModule:
     _modules: List[APIModule]
     path: str
 
     def __init__(self, path: str) -> None:
         self._modules = []
@@ -297,15 +319,17 @@
     __version__ = SYFT_OBJECT_VERSION_1
 
     # fields
     connection: Optional[NodeConnection] = None
     node_uid: Optional[UID] = None
     node_name: Optional[str] = None
     endpoints: Dict[str, APIEndpoint]
+    lib_endpoints: Optional[Dict[str, LibEndpoint]] = None
     api_module: Optional[APIModule] = None
+    libs: Optional[APIModule] = None
     signing_key: Optional[SyftSigningKey] = None
     # serde / storage rules
     refresh_api_callback: Optional[Callable] = None
 
     # def __post_init__(self) -> None:
     #     pass
 
@@ -317,50 +341,75 @@
         # TODO: Maybe there is a possibility of merging ServiceConfig and APIEndpoint
         from ..service.code.user_code_service import UserCodeService
 
         # find user role by verify_key
         # TODO: we should probably not allow empty verify keys but instead make user always register
         role = node.get_role_for_credentials(user_verify_key)
         _user_service_config_registry = UserServiceConfigRegistry.from_role(role)
-        endpoints = {}
+        _user_lib_config_registry = UserLibConfigRegistry.from_user(user_verify_key)
+        endpoints: Dict[str, APIEndpoint] = {}
+        lib_endpoints: Dict[str, LibEndpoint] = {}
 
         for (
             path,
             service_config,
         ) in _user_service_config_registry.get_registered_configs().items():
-            endpoint = APIEndpoint(
-                path=path,
-                name=service_config.public_name,
+            if not service_config.is_from_lib:
+                endpoint = APIEndpoint(
+                    service_path=path,
+                    module_path=path,
+                    name=service_config.public_name,
+                    description="",
+                    doc_string=service_config.doc_string,
+                    signature=service_config.signature,
+                    has_self=False,
+                )
+                endpoints[path] = endpoint
+
+        for (
+            path,
+            lib_config,
+        ) in _user_lib_config_registry.get_registered_configs().items():
+            endpoint = LibEndpoint(
+                service_path="action.execute",
+                module_path=path,
+                name=lib_config.public_name,
                 description="",
-                doc_string=service_config.doc_string,
-                signature=service_config.signature,
+                doc_string=lib_config.doc_string,
+                signature=lib_config.signature,
                 has_self=False,
             )
-            endpoints[path] = endpoint
+            lib_endpoints[path] = endpoint
 
         # 🟡 TODO 35: fix root context
         context = AuthedServiceContext(credentials=user_verify_key)
         method = node.get_method_with_context(UserCodeService.get_all_for_user, context)
         code_items = method()
 
         for code_item in code_items:
-            api_path = "code.call"
+            path = "code.call"
             unique_path = f"code.call_{code_item.service_func_name}"
             endpoint = APIEndpoint(
-                path=api_path,
+                service_path=path,
+                module_path=path,
                 name=code_item.service_func_name,
                 description="",
                 doc_string=f"Users custom func {code_item.service_func_name}",
                 signature=code_item.signature,
                 has_self=False,
                 pre_kwargs={"uid": code_item.id},
             )
             endpoints[unique_path] = endpoint
 
-        return SyftAPI(node_name=node.name, node_uid=node.id, endpoints=endpoints)
+        return SyftAPI(
+            node_name=node.name,
+            node_uid=node.id,
+            endpoints=endpoints,
+            lib_endpoints=lib_endpoints,
+        )
 
     def make_call(self, api_call: SyftAPICall) -> Result:
         signed_call = api_call.sign(credentials=self.signing_key)
         signed_result = self.connection.make_call(signed_call)
 
         if not isinstance(signed_result, SignedSyftAPICall):
             return SyftError(message="The result is not signed")  # type: ignore
@@ -394,50 +443,73 @@
 
     @staticmethod
     def _add_route(
         api_module: APIModule, endpoint: APIEndpoint, endpoint_method: Callable
     ):
         """Recursively create a module path to the route endpoint."""
 
-        _modules = endpoint.path.split(".")[:-1] + [endpoint.name]
+        _modules = endpoint.module_path.split(".")[:-1] + [endpoint.name]
 
         _self = api_module
         _last_module = _modules.pop()
         while _modules:
             module = _modules.pop(0)
             if not hasattr(_self, module):
                 submodule_path = f"{_self.path}.{module}"
                 _self._add_submodule(module, APIModule(path=submodule_path))
             _self = getattr(_self, module)
         _self._add_submodule(_last_module, endpoint_method)
 
     def generate_endpoints(self) -> None:
-        api_module = APIModule(path="")
-        for _, v in self.endpoints.items():
-            signature = v.signature
-            if not v.has_self:
-                signature = signature_remove_self(signature)
-            signature = signature_remove_context(signature)
-            endpoint_function = generate_remote_function(
-                self.node_uid,
-                signature,
-                v.path,
-                self.make_call,
-                pre_kwargs=v.pre_kwargs,
-            )
-            endpoint_function.__doc__ = v.doc_string
-            self._add_route(api_module, v, endpoint_function)
-        self.api_module = api_module
+        def build_endpoint_tree(endpoints):
+            api_module = APIModule(path="")
+            for _, v in endpoints.items():
+                signature = v.signature
+                if not v.has_self:
+                    signature = signature_remove_self(signature)
+                signature = signature_remove_context(signature)
+                if isinstance(v, APIEndpoint):
+                    endpoint_function = generate_remote_function(
+                        self.node_uid,
+                        signature,
+                        v.service_path,
+                        self.make_call,
+                        pre_kwargs=v.pre_kwargs,
+                    )
+                elif isinstance(v, LibEndpoint):
+                    endpoint_function = generate_remote_lib_function(
+                        self,
+                        self.node_uid,
+                        signature,
+                        v.service_path,
+                        v.module_path,
+                        self.make_call,
+                        pre_kwargs=v.pre_kwargs,
+                    )
+
+                endpoint_function.__doc__ = v.doc_string
+                self._add_route(api_module, v, endpoint_function)
+            return api_module
+
+        if self.lib_endpoints is not None:
+            self.libs = build_endpoint_tree(self.lib_endpoints)
+        self.api_module = build_endpoint_tree(self.endpoints)
 
     @property
     def services(self) -> APIModule:
         if self.api_module is None:
             self.generate_endpoints()
         return self.api_module
 
+    @property
+    def lib(self) -> APIModule:
+        if self.libs is None:
+            self.generate_endpoints()
+        return self.libs
+
     def __repr__(self) -> str:
         modules = self.services
         _repr_str = "client.api.services\n"
         for attr_name in modules._modules:
             module_or_func = getattr(modules, attr_name)
             module_path_str = f"client.api.services.{attr_name}"
             _repr_str += f"\n{module_path_str}\n\n"
@@ -548,7 +620,77 @@
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, NodeView):
             return False
         return self.node_name == other.node_name and self.verify_key == other.verify_key
 
     def __hash__(self) -> int:
         return hash((self.node_name, self.verify_key))
+
+
+def validate_callable_args_and_kwargs(args, kwargs, signature: Signature):
+    _valid_kwargs = {}
+    if "kwargs" in signature.parameters:
+        _valid_kwargs = kwargs
+    else:
+        for key, value in kwargs.items():
+            if key not in signature.parameters:
+                return SyftError(
+                    message=f"""Invalid parameter: `{key}`. Valid Parameters: {list(signature.parameters)}"""
+                )
+            param = signature.parameters[key]
+            if isinstance(param.annotation, str):
+                # 🟡 TODO 21: make this work for weird string type situations
+                # happens when from __future__ import annotations in a class file
+                t = index_syft_by_module_name(param.annotation)
+            else:
+                t = param.annotation
+            msg = None
+            try:
+                if t is not inspect.Parameter.empty:
+                    if isinstance(t, _GenericAlias) and type(None) in t.__args__:
+                        for v in t.__args__:
+                            if issubclass(v, EmailStr):
+                                v = str
+                            check_type(key, value, v)  # raises Exception
+                            break  # only need one to match
+                    else:
+                        check_type(key, value, t)  # raises Exception
+            except TypeError:
+                _type_str = getattr(t, "__name__", str(t))
+                msg = f"`{key}` must be of type `{_type_str}` not `{type(value).__name__}`"
+
+            if msg:
+                return SyftError(message=msg)
+
+            _valid_kwargs[key] = value
+
+    # signature.parameters is an OrderedDict, therefore,
+    # its fair to assume that order of args
+    # and the signature.parameters should always match
+    _valid_args = []
+    if "args" in signature.parameters:
+        _valid_args = args
+    else:
+        for (param_key, param), arg in zip(signature.parameters.items(), args):
+            if param_key in _valid_kwargs:
+                continue
+            t = param.annotation
+            msg = None
+            try:
+                if t is not inspect.Parameter.empty:
+                    if isinstance(t, _GenericAlias) and type(None) in t.__args__:
+                        for v in t.__args__:
+                            if issubclass(v, EmailStr):
+                                v = str
+                            check_type(param_key, arg, v)  # raises Exception
+                            break  # only need one to match
+                    else:
+                        check_type(param_key, arg, t)  # raises Exception
+            except TypeError:
+                _type_str = getattr(t, "__name__", str(t))
+                msg = f"Arg: {arg} must be {_type_str} not {type(arg).__name__}"
+            if msg:
+                return SyftError(message=msg)
+
+            _valid_args.append(arg)
+
+    return _valid_args, _valid_kwargs
```

### Comparing `syft-0.8.0b9/src/syft/client/client.py` & `syft-0.8.1b1/src/syft/client/client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/client/connection.py` & `syft-0.8.1b1/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/client/deploy.py` & `syft-0.8.1b1/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/client/registry.py` & `syft-0.8.1b1/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/client/search.py` & `syft-0.8.1b1/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/client/user_settings.py` & `syft-0.8.1b1/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/external/__init__.py` & `syft-0.8.1b1/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/external/oblv/__init__.py` & `syft-0.8.1b1/src/syft/external/oblv/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # relative
-from ...core.node.new.deserialize import _deserialize
-from ...core.node.new.serializable import recursive_serde_register
-from ...core.node.new.serialize import _serialize
+from ...serde.deserialize import _deserialize
+from ...serde.serializable import recursive_serde_register
+from ...serde.serialize import _serialize
 from .auth import login  # noqa: F401
 from .deployment import create_deployment  # noqa: F401
 from .oblv_proxy import check_oblv_proxy_installation_status  # noqa: F401
 from .oblv_proxy import create_oblv_key_pair  # noqa: F401
 from .oblv_proxy import get_oblv_public_key  # noqa: F401
 from .oblv_proxy import install_oblv_proxy  # noqa: F401
```

### Comparing `syft-0.8.0b9/src/syft/external/oblv/deployment.py` & `syft-0.8.1b1/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/external/oblv/deployment_client.py` & `syft-0.8.1b1/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/external/oblv/exceptions.py` & `syft-0.8.1b1/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.1b1/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/external/oblv/oblv_service.py` & `syft-0.8.1b1/src/syft/external/oblv/oblv_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,35 +16,35 @@
 from oblv import OblvClient
 import requests
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
-from ...core.node.new.api import NodeView
-from ...core.node.new.api import SyftAPI
-from ...core.node.new.client import HTTPConnection
-from ...core.node.new.client import Routes
-from ...core.node.new.context import AuthedServiceContext
-from ...core.node.new.context import ChangeContext
-from ...core.node.new.credentials import SyftSigningKey
-from ...core.node.new.credentials import SyftVerifyKey
-from ...core.node.new.deserialize import _deserialize as deserialize
-from ...core.node.new.document_store import DocumentStore
-from ...core.node.new.response import SyftError
-from ...core.node.new.serializable import serializable
-from ...core.node.new.service import AbstractService
-from ...core.node.new.service import service_method
-from ...core.node.new.syft_object import SYFT_OBJECT_VERSION_1
-from ...core.node.new.syft_object import SyftObject
-from ...core.node.new.uid import UID
-from ...core.node.new.user_code import UserCode
-from ...core.node.new.user_code import UserCodeStatus
-from ...core.node.new.user_roles import GUEST_ROLE_LEVEL
-from ...core.node.new.util import find_available_port
+from ...client.api import NodeView
+from ...client.api import SyftAPI
+from ...client.client import HTTPConnection
+from ...client.client import Routes
+from ...node.credentials import SyftSigningKey
+from ...node.credentials import SyftVerifyKey
+from ...serde.deserialize import _deserialize as deserialize
+from ...serde.serializable import serializable
+from ...service.code.user_code import UserCode
+from ...service.code.user_code import UserCodeStatus
+from ...service.context import AuthedServiceContext
+from ...service.context import ChangeContext
+from ...service.response import SyftError
+from ...service.service import AbstractService
+from ...service.service import service_method
+from ...service.user.user_roles import GUEST_ROLE_LEVEL
+from ...store.document_store import DocumentStore
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
+from ...types.uid import UID
+from ...util.util import find_available_port
 from .constants import DOMAIN_CONNECTION_PORT
 from .constants import LOCAL_MODE
 from .deployment_client import OblvMetadata
 from .exceptions import OblvEnclaveError
 from .exceptions import OblvProxyConnectPCRError
 from .oblv_keys import OblvKeys
 from .oblv_keys_stash import OblvKeysStash
```

### Comparing `syft-0.8.0b9/src/syft/gevent_patch.py` & `syft-0.8.1b1/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/node/credentials.py` & `syft-0.8.1b1/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/node/node.py` & `syft-0.8.1b1/src/syft/node/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # stdlib
 import contextlib
 from datetime import datetime
 from functools import partial
 import hashlib
 import os
 import threading
+import traceback
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
@@ -549,16 +550,18 @@
                 else:
                     return SyftError(message=f"API call not in registered services: {api_call.path}")  # type: ignore
 
             _private_api_path = user_config_registry.private_path_for(api_call.path)
             method = self.get_service_method(_private_api_path)
             try:
                 result = method(context, *api_call.args, **api_call.kwargs)
-            except Exception as e:
-                result = SyftError(message=f"Exception calling {api_call.path}. {e}")
+            except Exception:
+                result = SyftError(
+                    message=f"Exception calling {api_call.path}. {traceback.format_exc()}"
+                )
         else:
             worker_settings = WorkerSettings(
                 id=self.id,
                 name=self.name,
                 signing_key=self.signing_key,
                 document_store_config=self.document_store_config,
                 action_store_config=self.action_store_config,
```

### Comparing `syft-0.8.0b9/src/syft/node/routes.py` & `syft-0.8.1b1/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/node/run.py` & `syft-0.8.1b1/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/node/server.py` & `syft-0.8.1b1/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/node/worker_settings.py` & `syft-0.8.1b1/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/serde/array.py` & `syft-0.8.1b1/src/syft/serde/array.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,97 +33,102 @@
     np.dtype("uint64"): np.int64,
 }
 
 recursive_serde_register(
     np.ndarray, serialize=numpy_serialize, deserialize=numpy_deserialize
 )
 
+recursive_serde_register(
+    np._globals._NoValueType,
+)
+#  serialize=numpy_serialize, deserialize=numpy_deserialize
+
 
 recursive_serde_register(
     np.bool_,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.bool_),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.bool_)[0],
 )
 
 recursive_serde_register(
     np.int8,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.int8),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.int8)[0],
 )
 
 recursive_serde_register(
     np.int16,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.int16),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.int16)[0],
 )
 
 recursive_serde_register(
     np.int32,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.int32),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.int32)[0],
 )
 
 recursive_serde_register(
     np.int64,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.int64),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.int64)[0],
 )
 
 recursive_serde_register(
     np.uint8,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.uint8),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.uint8)[0],
 )
 
 recursive_serde_register(
     np.uint16,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.uint16),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.uint16)[0],
 )
 
 recursive_serde_register(
     np.uint32,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.uint32),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.uint32)[0],
 )
 
 recursive_serde_register(
     np.uint64,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.uint64),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.uint64)[0],
 )
 
 recursive_serde_register(
     np.single,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.single),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.single)[0],
 )
 
 recursive_serde_register(
     np.double,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.double),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.double)[0],
 )
 
 recursive_serde_register(
     np.float16,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.float16),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.float16)[0],
 )
 
 recursive_serde_register(
     np.float32,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.float32),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.float32)[0],
 )
 
 recursive_serde_register(
     np.float64,
     serialize=lambda x: x.tobytes(),
-    deserialize=lambda buffer: frombuffer(buffer, dtype=np.float64),
+    deserialize=lambda buffer: frombuffer(buffer, dtype=np.float64)[0],
 )
 
 # TODO: There is an incorrect mapping in looping,which makes it not work.
 # numpy_scalar_types = [
 #     np.bool_,
 #     np.int8,
 #     np.int16,
```

### Comparing `syft-0.8.0b9/src/syft/serde/arrow.py` & `syft-0.8.1b1/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/serde/deserialize.py` & `syft-0.8.1b1/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/serde/recursive.py` & `syft-0.8.1b1/src/syft/serde/recursive.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,15 @@
     is_type = False
     if isinstance(self, type):
         is_type = True
 
     msg = recursive_scheme.new_message()
     fqn = get_fully_qualified_name(self)
     if fqn not in TYPE_BANK:
+        # third party
         raise Exception(f"{fqn} not in TYPE_BANK")
 
     msg.fullyQualifiedName = fqn
     (
         nonrecursive,
         serialize,
         deserialize,
```

### Comparing `syft-0.8.0b9/src/syft/serde/recursive_primitives.py` & `syft-0.8.1b1/src/syft/serde/recursive_primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,11 +336,22 @@
 
 recursive_serde_register_type(_SpecialForm)
 recursive_serde_register_type(_GenericAlias)
 recursive_serde_register_type(Union)
 recursive_serde_register_type(TypeVar)
 
 if sys.version_info >= (3, 9):
-    recursive_serde_register_type(_UnionGenericAlias)
+    recursive_serde_register_type(
+        _UnionGenericAlias,
+        serialize_attrs=[
+            "__parameters__",
+            "__slots__",
+            "_inst",
+            "_name",
+            "__args__",
+            "__module__",
+            "__origin__",
+        ],
+    )
     recursive_serde_register_type(_SpecialGenericAlias)
 
 recursive_serde_register_type(EnumMeta)
```

### Comparing `syft-0.8.0b9/src/syft/serde/serializable.py` & `syft-0.8.1b1/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/serde/third_party.py` & `syft-0.8.1b1/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/action/action_object.py` & `syft-0.8.1b1/src/syft/service/action/action_object.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,97 @@
 # future
 from __future__ import annotations
 
 # stdlib
 import inspect
+import traceback
 import types
 from typing import Any
 from typing import Callable
 from typing import ClassVar
 from typing import Dict
 from typing import KeysView
 from typing import List
 from typing import Optional
-from typing import Set
 from typing import Tuple
 from typing import Type
 from typing import Union
 
 # third party
 import pydantic
+from result import Err
+from result import Ok
+from result import Result
 from typing_extensions import Self
 
 # relative
+from ...client.api import SyftAPI
 from ...client.client import SyftClient
 from ...serde.serializable import serializable
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftBaseObject
 from ...types.syft_object import SyftObject
 from ...types.uid import LineageID
 from ...types.uid import UID
+from ...util.logger import debug
 from ..response import SyftException
 from .action_data_empty import ActionDataEmpty
 from .action_types import action_type_for_type
 from .action_types import action_types
 
 
 @serializable()
 class Action(SyftObject):
+    """Serializable Action object.
+
+    Parameters:
+        path: str
+            The path of the Type of the remote object.
+        op: str
+            The method to be executed from the remote object.
+        remote_self: Optional[LineageID]
+            The extended UID of the SyftObject
+        args: List[LineageID]
+            `op` args
+        kwargs: Dict[str, LineageID]
+            `op` kwargs
+        result_id: Optional[LineageID]
+            Extended UID of the resulted SyftObject
+    """
+
     __canonical_name__ = "Action"
     __version__ = SYFT_OBJECT_VERSION_1
 
     __attr_searchable__: List[str] = []
 
     path: str
     op: str
     remote_self: Optional[LineageID]
     args: List[LineageID]
     kwargs: Dict[str, LineageID]
     result_id: Optional[LineageID]
 
     @pydantic.validator("id", pre=True, always=True)
     def make_id(cls, v: Optional[UID]) -> UID:
+        """Generate or reuse an UID"""
         return v if isinstance(v, UID) else UID()
 
     @pydantic.validator("result_id", pre=True, always=True)
     def make_result_id(cls, v: Optional[Union[UID, LineageID]]) -> UID:
+        """Generate or reuse a LineageID"""
         return v if isinstance(v, LineageID) else LineageID(v)
 
     @property
     def full_path(self) -> str:
+        """Action path and operation"""
         return f"{self.path}.{self.op}"
 
     @property
     def syft_history_hash(self) -> int:
+        """Create a unique hash for the operations applied on the object."""
         hashes = 0
         if self.remote_self:
             hashes += hash(self.remote_self.syft_history_hash)
         # 🔵 TODO: resolve this
         # if the object is ActionDataEmpty then the type might not be equal to the
         # real thing. This is the same issue with determining the result type from
         # a pointer operation in the past, so we should think about what we want here
@@ -79,14 +105,15 @@
         return hashes
 
 
 class ActionObjectPointer:
     pass
 
 
+# Hooks
 HOOK_ALWAYS = "ALWAYS"
 
 passthrough_attrs = [
     "__dict__",  # python
     "__class__",  # python
     "__repr_name__",  # python
     "__annotations__",  # python
@@ -131,118 +158,162 @@
     "__setitem__",
     "__len__",
     "shape",
 ]
 action_data_empty_must_run = [
     "__repr__",
 ]
-show_print = False
 
 
-def debug_original_func(name: str, func: Callable) -> None:
-    print(f"{name} func is:")
-    print("inspect.isdatadescriptor", inspect.isdatadescriptor(func))
-    print("inspect.isgetsetdescriptor", inspect.isgetsetdescriptor(func))
-    print("inspect.isfunction", inspect.isfunction(func))
-    print("inspect.isbuiltin", inspect.isbuiltin(func))
-    print("inspect.ismethod", inspect.ismethod(func))
-    print("inspect.ismethoddescriptor", inspect.ismethoddescriptor(func))
+class PreHookContext(SyftBaseObject):
+    """Hook context
+
+    Parameters:
+        obj: Any
+            The ActionObject to use for the action
+        op_name: str
+            The method name to use for the action
+        node_uid: Optional[UID]
+            Optional Syft node UID
+        result_id: Optional[Union[UID, LineageID]]
+            Optional result Syft UID
+        action: Optional[Action]
+            The action generated by the current hook
+    """
 
+    obj: Any
+    op_name: str
+    node_uid: Optional[UID]
+    result_id: Optional[Union[UID, LineageID]]
+    action: Optional[Action]
 
-def make_action_side_effect(context: PreHookContext, *args: Any, **kwargs: Any) -> Any:
+
+def make_action_side_effect(
+    context: PreHookContext, *args: List[Any, ...], **kwargs: Dict[str, Any]
+) -> Result[Ok[Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]], Err[str]]:
+    """Create a new action from context_op_name, and add it to the PreHookContext
+
+    Parameters:
+        context: PreHookContext
+            PreHookContext object
+        *args:
+            Operation *args
+        **kwargs
+            Operation *kwargs
+    Returns:
+        - Ok[[Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]] on success
+        - Err[str] on failure
+    """
     try:
         action = context.obj.syft_make_method_action(
             op=context.op_name, args=args, kwargs=kwargs
         )
         context.action = action
-    except Exception:  # nosec
-        # print(
-        #     "Exception detected in make_action_side_effect", e
-        # )  # TODO: Put this Exception back
-        pass
-    return context, args, kwargs
+    except Exception:
+        return Err(f"make_action_side_effect failed with {traceback.format_exc()}")
+    return Ok((context, args, kwargs))
+
+
+def convert_to_pointers(
+    api: SyftAPI,
+    node_uid: Optional[UID] = None,
+    args: Optional[List] = None,
+    kwargs: Optional[Dict] = None,
+) -> Tuple[List, Dict]:
+    arg_list = []
+    kwarg_dict = {}
+    if args is not None:
+        for arg in args:
+            if not isinstance(arg, ActionObject):
+                arg = ActionObject.from_obj(arg)
+                arg.syft_node_uid = node_uid
+                arg = api.services.action.set(arg)
+                # arg = action_obj.send(
+                #     client
+                # )  # make sure this doesn't break things later on in send_method_action
+            arg_list.append(arg)
+
+    if kwargs is not None:
+        for k, arg in kwargs.items():
+            if not isinstance(arg, ActionObject):
+                arg = ActionObject.from_obj(arg)
+                arg.syft_node_uid = node_uid
+                arg = api.services.action.set(arg)
+                # arg = action_obj.send(client)
+
+            kwarg_dict[k] = arg
+
+    return arg_list, kwarg_dict
 
 
 def send_action_side_effect(context: PreHookContext, *args: Any, **kwargs: Any) -> Any:
     try:
         if context.op_name not in dont_make_side_effects and hasattr(
             context.obj, "syft_node_uid"
         ):
             if getattr(context.obj, "syft_node_uid", None):
                 if context.action is not None:
                     action = context.obj.syft_make_method_action(
                         op=context.op_name, args=args, kwargs=kwargs
                     )
                     context.action = action
 
-                action_result = context.obj.syft_execute_action(action, sync=True)
-                if not isinstance(action_result, ActionObject):
-                    # print("Got back unexpected response", action_result)
-                    pass
-                else:
-                    context.node_uid = action_result.syft_node_uid
-                    context.result_id = action.result_id
-                    # print("IGNORING: got action result", action_result)
-            else:
-                # 🟡 TODO
-                pass
-                # print(
-                #     "Can't Send Action without a target node. Use .point_to(node_uid: UID)"
-                # )
-    except Exception:  # nosec
-        # print(
-        #     "Exception in send_action_side_effect", e
-        # )  # TODO: Put this Exception back
-        pass
-    return context, args, kwargs
+        result = make_action_side_effect(context, *args, **kwargs)
+        if result.is_err():
+            raise RuntimeError(result.err())
 
+        context, _, _ = result.ok()
 
-def propagate_node_uid(context: PreHookContext, op: str, result: Any) -> Any:
-    try:
-        if context.op_name not in dont_make_side_effects and hasattr(
-            context.obj, "syft_node_uid"
-        ):
-            syft_node_uid = getattr(context.obj, "syft_node_uid", None)
-            if syft_node_uid:
-                if not hasattr(result, "syft_node_uid"):
-                    # print("result doesnt have a syft_node_uid attr")
-                    pass
-                if op not in context.obj._syft_dont_wrap_attrs():
-                    if hasattr(result, "syft_node_uid"):
-                        setattr(result, "syft_node_uid", syft_node_uid)
-                else:
-                    # print("dont propogate node_uid because output isnt wrapped")
-                    pass
-            else:
-                # 🟡 TODO
-                # print("Can't proagate node_uid because parent doesnt have one")
-                pass
-    except Exception:  # nosec
-        # print("Exception in propagate_node_uid", e)
-        pass
-    return result
+        action_result = context.obj.syft_execute_action(context.action, sync=True)
 
+        if not isinstance(action_result, ActionObject):
+            raise RuntimeError(f"Got back unexpected response : {action_result}")
+        else:
+            context.node_uid = action_result.syft_node_uid
+            context.result_id = context.action.result_id
+    except Exception:
+        return Err(f"send_action_side_effect failed with {traceback.format_exc()}")
+    return Ok((context, args, kwargs))
+
+
+def propagate_node_uid(
+    context: PreHookContext, op: str, result: Any
+) -> Result[Ok[Any], Err[str]]:
+    """Patch the result to include the syft_node_uid
+
+    Parameters:
+        context: PreHookContext
+            PreHookContext object
+        op: str
+            Which operation was executed
+        result: Any
+            The result to patch
+    Returns:
+        - Ok[[result] on success
+        - Err[str] on failure
+    """
+    if context.op_name in dont_make_side_effects or not hasattr(
+        context.obj, "syft_node_uid"
+    ):
+        return Ok(result)
 
-def is_action_data_empty(obj: Any) -> bool:
-    if hasattr(obj, "syft_action_data"):
-        obj = obj.syft_action_data
-    if isinstance(obj, ActionDataEmpty):
-        return True
-    return False
+    try:
+        syft_node_uid = getattr(context.obj, "syft_node_uid", None)
+        if syft_node_uid is None:
+            raise RuntimeError("Can't proagate node_uid because parent doesnt have one")
+
+        if op not in context.obj._syft_dont_wrap_attrs():
+            if hasattr(result, "syft_node_uid"):
+                setattr(result, "syft_node_uid", syft_node_uid)
+        else:
+            raise RuntimeError("dont propogate node_uid because output isnt wrapped")
+    except Exception:
+        return Err(f"propagate_node_uid failed with {traceback.format_exc()}")
 
-
-def has_action_data_empty(args: Any, kwargs: Any) -> bool:
-    for a in args:
-        if is_action_data_empty(a):
-            return True
-
-    for _, a in kwargs.items():
-        if is_action_data_empty(a):
-            return True
-    return False
+    return Ok(result)
 
 
 def debox_args_and_kwargs(args: Any, kwargs: Any) -> Tuple[Any, Any]:
     filtered_args = []
     filtered_kwargs = {}
     for a in args:
         value = a
@@ -255,23 +326,17 @@
         if hasattr(value, "syft_action_data"):
             value = value.syft_action_data
         filtered_kwargs[k] = a
 
     return tuple(filtered_args), filtered_kwargs
 
 
-class PreHookContext(SyftBaseObject):
-    obj: Any
-    op_name: str
-    node_uid: Optional[UID]
-    result_id: Optional[Union[UID, LineageID]]
-    action: Optional[Action]
-
-
 class ActionObject(SyftObject):
+    """Action object for remote execution."""
+
     __canonical_name__ = "ActionObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     __attr_searchable__: List[str] = []
     syft_action_data: Optional[Any] = None
     syft_pointer_type: ClassVar[Type[ActionObjectPointer]]
 
@@ -279,380 +344,568 @@
     syft_parent_hashes: Optional[Union[int, List[int]]]
     syft_parent_op: Optional[str]
     syft_parent_args: Optional[Any]
     syft_parent_kwargs: Optional[Any]
     syft_history_hash: Optional[int]
     syft_internal_type: ClassVar[Type[Any]]
     syft_node_uid: Optional[UID]
-    _syft_pre_hooks__: Dict[str, Set] = {}
-    _syft_post_hooks__: Dict[str, Set] = {}
+    _syft_pre_hooks__: Dict[str, List] = {}
+    _syft_post_hooks__: Dict[str, List] = {}
 
     @property
     def syft_lineage_id(self) -> LineageID:
+        """Compute the LineageID of the ActionObject, using the `id` and the `syft_history_hash` memebers"""
         return LineageID(self.id, self.syft_history_hash)
 
     @pydantic.validator("id", pre=True, always=True)
     def make_id(cls, v: Optional[UID]) -> UID:
-        return v if isinstance(v, UID) else UID()
+        """Generate or reuse an UID"""
+        return Action.make_id(v)
 
     @pydantic.validator("syft_action_data", pre=True, always=True)
     def check_action_data(
         cls, v: ActionObject.syft_pointer_type
     ) -> ActionObject.syft_pointer_type:
         if cls == AnyActionObject or isinstance(
             v, (cls.syft_internal_type, ActionDataEmpty)
         ):
             return v
         raise SyftException(
             f"Must init {cls} with {cls.syft_internal_type} not {type(v)}"
         )
 
-    def syft_point_to(self, node_uid: UID) -> None:
+    def syft_point_to(self, node_uid: UID) -> "ActionObject":
+        """Set the syft_node_uid, used in the post hooks"""
         self.syft_node_uid = node_uid
 
+        return self
+
     def syft_get_property(self, obj: Any, method: str) -> Any:
         klass_method = getattr(type(obj), method, None)
         if klass_method is None:
             raise Exception(f"{type(obj)} has no {method} attribute")
         return klass_method.__get__(obj)
 
     def syft_is_property(self, obj: Any, method: str) -> bool:
         klass_method = getattr(type(obj), method, None)
         return isinstance(klass_method, property) or inspect.isdatadescriptor(
             klass_method
         )
 
+    def syft_execute_action(
+        self, action: Action, sync: bool = True
+    ) -> ActionObjectPointer:
+        """Execute a remote action
+
+        Parameters:
+            action: Action
+                Which action to execute
+            sync: bool
+                Run sync/async
+
+        Returns:
+            ActionObjectPointer
+        """
+        if self.syft_node_uid is None:
+            raise SyftException("Pointers can't execute without a node_uid.")
+
+        # relative
+        from ...client.api import APIRegistry
+        from ...client.api import SyftAPICall
+
+        api = APIRegistry.api_for(node_uid=self.syft_node_uid)
+
+        kwargs = {"action": action}
+        api_call = SyftAPICall(
+            node_uid=self.syft_node_uid, path="action.execute", args=[], kwargs=kwargs
+        )
+        return api.make_call(api_call)
+
+    def _syft_try_to_save_to_store(self, obj) -> None:
+        if self.syft_node_uid is None:
+            return
+
+        # relative
+        from ...client.api import APIRegistry
+
+        api = APIRegistry.api_for(node_uid=self.syft_node_uid)
+        api.services.action.set(obj)
+
+    def _syft_prepare_obj_uid(self, obj) -> LineageID:
+        # We got the UID
+        if isinstance(obj, (UID, LineageID)):
+            return LineageID(obj.id)
+
+        # We got the ActionObjectPointer
+        if isinstance(obj, ActionObjectPointer):
+            return obj.syft_lineage_id
+
+        # We got the ActionObject. We need to save it in the store.
+        if isinstance(obj, ActionObject):
+            self._syft_try_to_save_to_store(obj)
+            return obj.syft_lineage_id
+
+        # We got a raw object. We need to create the ActionObject from scratch and save it in the store.
+        obj_id = Action.make_id(None)
+        lin_obj_id = Action.make_result_id(obj_id)
+        act_obj = ActionObject.from_obj(obj, id=obj_id, syft_lineage_id=lin_obj_id)
+
+        self._syft_try_to_save_to_store(act_obj)
+
+        return act_obj.syft_lineage_id
+
+    def syft_make_action(
+        self,
+        path: str,
+        op: str,
+        remote_self: Optional[Union[UID, LineageID]] = None,
+        args: Optional[
+            List[Union[UID, LineageID, ActionObjectPointer, ActionObject, Any]]
+        ] = [],
+        kwargs: Optional[
+            Dict[str, Union[UID, LineageID, ActionObjectPointer, ActionObject, Any]]
+        ] = {},
+    ) -> Action:
+        """Generate new action from the information
+
+        Parameters:
+            path: str
+                The path of the Type of the remote object.
+            op: str
+                The method to be executed from the remote object.
+            remote_self: Optional[Union[UID, LineageID]]
+                The extended UID of the SyftObject
+            args: Optional[List[Union[UID, LineageID, ActionObjectPointer, ActionObject]]]
+                `op` args
+            kwargs: Optional[Dict[str, Union[UID, LineageID, ActionObjectPointer, ActionObject]]]
+                `op` kwargs
+        Returns:
+            Action object
+
+        Raises:
+            ValueError: For invalid args or kwargs
+            PydanticValidationError: For args and kwargs
+        """
+        arg_ids = []
+        kwarg_ids = {}
+
+        for obj in args:
+            arg_ids.append(self._syft_prepare_obj_uid(obj))
+
+        for k, uid in kwargs.items():
+            kwarg_ids[k] = self._syft_prepare_obj_uid(obj)
+
+        action = Action(
+            path=path,
+            op=op,
+            remote_self=LineageID(remote_self),
+            args=arg_ids,
+            kwargs=kwarg_ids,
+        )
+        return action
+
+    def syft_make_method_action(
+        self,
+        op: str,
+        args: Optional[List[Union[UID, ActionObjectPointer]]] = None,
+        kwargs: Optional[Dict[str, Union[UID, ActionObjectPointer]]] = None,
+    ) -> Action:
+        """Generate new method action from the current object.
+
+        Parameters:
+            op: str
+                The method to be executed from the remote object.
+            args: List[LineageID]
+                `op` args
+            kwargs: Dict[str, LineageID]
+                `op` kwargs
+        Returns:
+            Action object
+
+        Raises:
+            ValueError: For invalid args or kwargs
+            PydanticValidationError: For args and kwargs
+        """
+        path = self.syft_get_path()
+        return self.syft_make_action(
+            path=path, op=op, remote_self=self.syft_lineage_id, args=args, kwargs=kwargs
+        )
+
+    def syft_get_path(self) -> str:
+        """Get the type path of the underlying object"""
+        if isinstance(self, AnyActionObject) and self.syft_internal_type:
+            return f"{type(self.syft_action_data).__name__}"  # avoids AnyActionObject errors
+        return f"{type(self).__name__}"
+
+    def syft_remote_method(
+        self,
+        op: str,
+    ) -> Callable:
+        """Generate a Callable object for remote calls.
+
+        Parameters:
+            op: str
+                he method to be executed from the remote object.
+
+        Returns:
+            A function
+        """
+
+        def wrapper(
+            *args: Optional[List[Union[UID, ActionObjectPointer]]],
+            **kwargs: Optional[Dict[str, Union[UID, ActionObjectPointer]]],
+        ) -> Action:
+            return self.syft_make_method_action(op=op, args=args, kwargs=kwargs)
+
+        return wrapper
+
     def send(self, client: SyftClient) -> Self:
+        """Send the object to a Syft Client"""
+
         return client.api.services.action.set(self)
 
     def get_from(self, client: SyftClient) -> Any:
+        """Get the object from a Syft Client"""
+
         return client.api.services.action.get(self.id).syft_action_data
 
     @staticmethod
     def from_obj(
         syft_action_data: Any,
         id: Optional[UID] = None,
         syft_lineage_id: Optional[LineageID] = None,
     ) -> ActionObject:
-        if isinstance(syft_action_data, ActionObject):
-            return syft_action_data
+        """Create an ActionObject from an existing object.
+
+        Parameters:
+            syft_action_data: Any
+                The object to be converted to a Syft ActionObject
+            id: Optional[UID]
+                Which ID to use for the ActionObject. Optional
+            syft_lineage_id: Optional[LineageID]
+                Which LineageID to use for the ActionObject. Optional
+        """
         if id and syft_lineage_id and id != syft_lineage_id.id:
-            raise Exception("UID and LineageID should match")
+            raise ValueError("UID and LineageID should match")
+
         action_type = action_type_for_type(syft_action_data)
-        if action_type is None:
-            raise Exception(f"{type(syft_action_data)} not in action_types")
         action_object = action_type(syft_action_data=syft_action_data)
+
         if id:
             action_object.id = id
+
         if syft_lineage_id:
             action_object.id = syft_lineage_id.id
             action_object.syft_history_hash = syft_lineage_id.syft_history_hash
         elif id:
             action_object.syft_history_hash = hash(id)
 
         return action_object
 
     @staticmethod
     def empty(
-        syft_internal_type: Optional[Any] = Any,
+        syft_internal_type: Any = Any,
         id: Optional[UID] = None,
         syft_lineage_id: Optional[LineageID] = None,
     ) -> ActionObject:
+        """Create an ActionObject from a type, using a ActionDataEmpty object
+
+        Parameters:
+            syft_internal_type: Type
+                The Type for which to create a ActionDataEmpty object
+            id: Optional[UID]
+                Which ID to use for the ActionObject. Optional
+            syft_lineage_id: Optional[LineageID]
+                Which LineageID to use for the ActionObject. Optional
+        """
+
         empty = ActionDataEmpty(syft_internal_type=syft_internal_type)
-        action_object = ActionObject.from_obj(
+        return ActionObject.from_obj(
             syft_action_data=empty, id=id, syft_lineage_id=syft_lineage_id
         )
-        return action_object
 
     def __post_init__(self) -> None:
+        """Add pre/post hooks."""
         if HOOK_ALWAYS not in self._syft_pre_hooks__:
-            self._syft_pre_hooks__[HOOK_ALWAYS] = set()
-        self._syft_pre_hooks__[HOOK_ALWAYS].add(make_action_side_effect)
-        self._syft_pre_hooks__[HOOK_ALWAYS].add(send_action_side_effect)
+            self._syft_pre_hooks__[HOOK_ALWAYS] = []
+
+        # this should be a list as orders matters
+        for side_effect in [make_action_side_effect, send_action_side_effect]:
+            if side_effect not in self._syft_pre_hooks__[HOOK_ALWAYS]:
+                self._syft_pre_hooks__[HOOK_ALWAYS].append(side_effect)
 
         if HOOK_ALWAYS not in self._syft_post_hooks__:
-            self._syft_post_hooks__[HOOK_ALWAYS] = set()
-        self._syft_post_hooks__[HOOK_ALWAYS].add(propagate_node_uid)
+            self._syft_post_hooks__[HOOK_ALWAYS] = []
+
+        for side_effect in [propagate_node_uid]:
+            if side_effect not in self._syft_post_hooks__[HOOK_ALWAYS]:
+                self._syft_post_hooks__[HOOK_ALWAYS].append(side_effect)
 
         if isinstance(self.syft_action_data, ActionObject):
             raise Exception("Nested ActionObjects", self.syft_action_data)
 
         self.syft_history_hash = hash(self.id)
 
     def _syft_run_pre_hooks__(
         self, context: PreHookContext, name: str, args: Any, kwargs: Any
     ) -> Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]:
-        try:
-            result_args, result_kwargs = args, kwargs
-            if name in self._syft_pre_hooks__:
-                for hook in self._syft_pre_hooks__[name]:
-                    context, result_args, result_kwargs = hook(
-                        context, *result_args, **result_kwargs
-                    )
+        """Hooks executed before the actual call"""
+        result_args, result_kwargs = args, kwargs
+        if name in self._syft_pre_hooks__:
+            for hook in self._syft_pre_hooks__[name]:
+                result = hook(context, *result_args, **result_kwargs)
+                if result.is_ok():
+                    context, result_args, result_kwargs = result.ok()
+                else:
+                    debug(f"Pre-hook failed with {result.err()}")
+
+        if name not in self._syft_dont_wrap_attrs():
+            if HOOK_ALWAYS in self._syft_pre_hooks__:
+                for hook in self._syft_pre_hooks__[HOOK_ALWAYS]:
+                    result = hook(context, *result_args, **result_kwargs)
+                    if result.is_ok():
+                        context, result_args, result_kwargs = result.ok()
+                    else:
+                        debug(f"Pre-hook failed with {result.err()}")
 
-            if name not in self._syft_dont_wrap_attrs():
-                if HOOK_ALWAYS in self._syft_pre_hooks__:
-                    for hook in self._syft_pre_hooks__[HOOK_ALWAYS]:
-                        context, result_args, result_kwargs = hook(
-                            context, *result_args, **result_kwargs
-                        )
-        except Exception as e:
-            print("Exception in pre hooks", e)
         return context, result_args, result_kwargs
 
     def _syft_run_post_hooks__(
         self, context: PreHookContext, name: str, result: Any
     ) -> Any:
+        """Hooks executed after the actual call"""
         new_result = result
         if name in self._syft_post_hooks__:
             for hook in self._syft_post_hooks__[name]:
-                new_result = hook(context, name, new_result)
+                result = hook(context, name, new_result)
+                if result.is_ok():
+                    new_result = result.ok()
+                else:
+                    debug(f"Post hook failed with {result.err()}")
 
         if name not in self._syft_dont_wrap_attrs():
             if HOOK_ALWAYS in self._syft_post_hooks__:
                 for hook in self._syft_post_hooks__[HOOK_ALWAYS]:
-                    new_result = hook(context, name, new_result)
+                    result = hook(context, name, new_result)
+                    if result.is_ok():
+                        new_result = result.ok()
+                    else:
+                        debug(f"Post hook failed with {result.err()}")
+
         return new_result
 
     def _syft_output_action_object(
         self,
         result: Any,
     ) -> Any:
-        # can check types here
-        if not issubclass(type(result), ActionObject):
-            constructor = action_type_for_type(result)
-            if not constructor:
-                raise Exception(f"output: {type(result)} no in action_types")
-            result = constructor(syft_action_data=result)
+        """Wrap the result in an ActionObject"""
+        if issubclass(type(result), ActionObject):
+            return result
+
+        constructor = action_type_for_type(result)
+        result = constructor(syft_action_data=result)
 
         return result
 
     def _syft_passthrough_attrs(self) -> List[str]:
+        """These attributes are forwarded to the `object` base class."""
         return passthrough_attrs + getattr(self, "syft_passthrough_attrs", [])
 
     def _syft_dont_wrap_attrs(self) -> List[str]:
+        """The results from these attributes are ignored from UID patching."""
         return dont_wrap_output_attrs + getattr(self, "syft_dont_wrap_attrs", [])
 
-    def __getattribute__(self, name: str) -> Any:
-        # bypass certain attrs to prevent recursion issues
-        if name.startswith("_syft") or name.startswith("syft"):
-            return object.__getattribute__(self, name)
-
-        if name in self._syft_passthrough_attrs():
-            return object.__getattribute__(self, name)
+    def _syft_get_attr_context(self, name: str) -> Any:
+        """Find which instance - Syft ActionObject or the original object - has the requested attribute."""
         defined_on_self = name in self.__dict__ or name in self.__private_attributes__
-        if show_print:
-            print(">> ", name, ", defined_on_self = ", defined_on_self)
 
-        # use the custom definied version
+        debug(">> ", name, ", defined_on_self = ", defined_on_self)
+
+        # use the custom defined version
         context_self = self
         if not defined_on_self:
             context_self = self.syft_action_data  # type: ignore
 
-        # TODO: weird edge cases here for things like tuples
-        if name == "__bool__" and not hasattr(self.syft_action_data, "__bool__"):
-            context = PreHookContext(obj=self, op_name=name)
-            context, _, _ = self._syft_run_pre_hooks__(context, name, (), {})
-            # no input needs to propagate
-            result = self._syft_run_post_hooks__(
-                context, name, bool(self.syft_action_data)
+        return context_self
+
+    def _syft_attr_propagate_ids(self, context, name: str, result: Any) -> Any:
+        """Patch the results with the syft_history_hash, node_uid, and result_id."""
+        if name in self._syft_dont_wrap_attrs():
+            return result
+
+        # Wrap as Syft Object
+        result = self._syft_output_action_object(result)
+
+        # Propagate History
+        if context.action is not None:
+            result.syft_history_hash = context.action.syft_history_hash
+
+        # Propagate Syft Node UID
+        result.syft_node_uid = context.node_uid
+
+        # Propagate Result ID
+        if context.result_id is not None:
+            result.id = context.result_id
+
+        return result
+
+    def _syft_wrap_attribute_for_bool_on_nonbools(self, name: str) -> Any:
+        """Handle `__getattribute__` for bool casting."""
+        if name != "__bool__":
+            raise RuntimeError(
+                "[_wrap_attribute_for_bool_on_nonbools] Use this only for the __bool__ operator"
             )
-            if name not in self._syft_dont_wrap_attrs():
-                result = self._syft_output_action_object(result)
-                if context.action is not None:
-                    result.syft_history_hash = context.action.syft_history_hash
 
-            def __wrapper__bool__() -> bool:
-                return result
+        if hasattr(self.syft_action_data, "__bool__"):
+            raise RuntimeError(
+                "[_wrap_attribute_for_bool_on_nonbools] self.syft_action_data already implements the bool operator"
+            )
 
-            return __wrapper__bool__
+        debug("[__getattribute__] Handling bool on nonbools")
+        context = PreHookContext(obj=self, op_name=name)
+        context, _, _ = self._syft_run_pre_hooks__(context, name, (), {})
+
+        # no input needs to propagate
+        result = self._syft_run_post_hooks__(context, name, bool(self.syft_action_data))
+        result = self._syft_attr_propagate_ids(context, name, result)
+
+        def __wrapper__bool__() -> bool:
+            return result
+
+        return __wrapper__bool__
+
+    def _syft_wrap_attribute_for_properties(self, name: str) -> Any:
+        """Handle `__getattribute__` for properties."""
+        context_self = self._syft_get_attr_context(name)
+
+        if not self.syft_is_property(context_self, name):
+            raise RuntimeError(
+                "[_wrap_attribute_for_properties] Use this only on properties"
+            )
+        debug(f"[__getattribute__] Handling property {name} ")
 
-        if self.syft_is_property(context_self, name):
-            if show_print:
-                print("Property detected: ", name)
-            if self.syft_is_property(context_self, name):
-                context = PreHookContext(obj=self, op_name=name)
-                context, _, _ = self._syft_run_pre_hooks__(context, name, (), {})
-                # no input needs to propagate
-                result = self._syft_run_post_hooks__(
-                    context, name, self.syft_get_property(context_self, name)
-                )
-                if name not in self._syft_dont_wrap_attrs():
-                    result = self._syft_output_action_object(result)
-                    if context.action is not None:
-                        result.syft_history_hash = context.action.syft_history_hash
-                return result
+        context = PreHookContext(obj=self, op_name=name)
+        context, _, _ = self._syft_run_pre_hooks__(context, name, (), {})
+        # no input needs to propagate
+        result = self._syft_run_post_hooks__(
+            context, name, self.syft_get_property(context_self, name)
+        )
+
+        return self._syft_attr_propagate_ids(context, name, result)
+
+    def _syft_wrap_attribute_for_methods(self, name: str) -> Any:
+        """Handle `__getattribute__` for methods."""
 
         # check for other types that aren't methods, functions etc
         def fake_func(*args: Any, **kwargs: Any) -> Any:
             return ActionDataEmpty(syft_internal_type=self.syft_internal_type)
 
+        debug(f"[__getattribute__] Handling method {name} ")
         if (
             isinstance(self.syft_action_data, ActionDataEmpty)
             and name not in action_data_empty_must_run
         ):
             original_func = fake_func
         else:
             original_func = getattr(self.syft_action_data, name)
 
-        if show_print:
-            debug_original_func(name, original_func)
-        if inspect.ismethod(original_func) or inspect.ismethoddescriptor(original_func):
-            if show_print:
-                print("Running method: ", name)
+        debug_original_func(name, original_func)
 
-            def wrapper(_self: Any, *args: Any, **kwargs: Any) -> Any:
-                context = PreHookContext(obj=self, op_name=name)
-                context, pre_hook_args, pre_hook_kwargs = self._syft_run_pre_hooks__(
-                    context, name, args, kwargs
+        def _base_wrapper(*args: Any, **kwargs: Any) -> Any:
+            context = PreHookContext(obj=self, op_name=name)
+            context, pre_hook_args, pre_hook_kwargs = self._syft_run_pre_hooks__(
+                context, name, args, kwargs
+            )
+
+            if has_action_data_empty(args=args, kwargs=kwargs):
+                result = fake_func(*args, **kwargs)
+            else:
+                original_args, original_kwargs = debox_args_and_kwargs(
+                    pre_hook_args, pre_hook_kwargs
                 )
+                result = original_func(*original_args, **original_kwargs)
 
-                if not has_action_data_empty(args=args, kwargs=kwargs):
-                    original_args, original_kwargs = debox_args_and_kwargs(
-                        pre_hook_args, pre_hook_kwargs
-                    )
+            post_result = self._syft_run_post_hooks__(context, name, result)
+            post_result = self._syft_attr_propagate_ids(context, name, post_result)
 
-                    result = original_func(*original_args, **original_kwargs)
-                else:
-                    result = fake_func(*args, **kwargs)
+            return post_result
 
-                post_result = self._syft_run_post_hooks__(context, name, result)
-                if name not in self._syft_dont_wrap_attrs():
-                    post_result = self._syft_output_action_object(
-                        post_result,
-                    )
-                    if context.action is not None:
-                        post_result.syft_history_hash = context.action.syft_history_hash
-                    post_result.syft_node_uid = context.node_uid
-                    if context.result_id is not None:
-                        post_result.id = context.result_id
-                return post_result
+        if inspect.ismethod(original_func) or inspect.ismethoddescriptor(original_func):
+            debug("Running method: ", name)
+
+            def wrapper(_self: Any, *args: Any, **kwargs: Any):
+                return _base_wrapper(*args, **kwargs)
 
             wrapper = types.MethodType(wrapper, type(self))
         else:
-            if show_print:
-                print("Running non-method: ", name)
-
-            def wrapper(*args: Any, **kwargs: Any) -> Any:
-                context = PreHookContext(obj=self, op_name=name)
-                context, pre_hook_args, pre_hook_kwargs = self._syft_run_pre_hooks__(
-                    context, name, args, kwargs
-                )
-
-                if not has_action_data_empty(args=args, kwargs=kwargs):
-                    original_args, original_kwargs = debox_args_and_kwargs(
-                        pre_hook_args, pre_hook_kwargs
-                    )
-
-                    result = original_func(*original_args, **original_kwargs)
-                else:
-                    result = fake_func(*args, **kwargs)
+            debug("Running non-method: ", name)
 
-                post_result = self._syft_run_post_hooks__(context, name, result)
-                if name not in self._syft_dont_wrap_attrs():
-                    post_result = self._syft_output_action_object(post_result)
-                    if context.action is not None:
-                        post_result.syft_history_hash = context.action.syft_history_hash
-                    post_result.syft_node_uid = context.node_uid
-                    if context.result_id is not None:
-                        post_result.id = context.result_id
-                return post_result
+            wrapper = _base_wrapper
 
         try:
             wrapper.__doc__ = original_func.__doc__
-            if show_print:
-                print(
-                    "Found original signature for ",
-                    name,
-                    inspect.signature(original_func),
-                )
+            debug(
+                "Found original signature for ",
+                name,
+                inspect.signature(original_func),
+            )
             wrapper.__ipython_inspector_signature_override__ = inspect.signature(
                 original_func
             )
         except Exception:
-            if show_print:
-                print("name", name, "has no signature")
+            debug("name", name, "has no signature")
 
         return wrapper
 
-    def syft_execute_action(
-        self, action: Action, sync: bool = True
-    ) -> ActionObjectPointer:
-        if self.syft_node_uid is None:
-            raise SyftException("Pointers can't execute without a node_uid.")
-        # relative
-        from ...client.api import APIRegistry
-        from ...client.api import SyftAPICall
+    def __getattribute__(self, name: str) -> Any:
+        """Called unconditionally to implement attribute accesses for instances of the class.
+        If the class also defines __getattr__(), the latter will not be called unless __getattribute__()
+        either calls it explicitly or raises an AttributeError.
+        This method should return the (computed) attribute value or raise an AttributeError exception.
+        In order to avoid infinite recursion in this method, its implementation should always:
+         * call the base class method with the same name to access any attributes it needs
+            for example : object.__getattribute__(self, name).
+         * use the syft/_syft prefix for internal methods.
+         * add the method name to the passthrough_attrs.
+
+        Parameters:
+            name: str
+                The name of the attribute to access.
+        """
+        # bypass certain attrs to prevent recursion issues
+        if name.startswith("_syft") or name.startswith("syft"):
+            return object.__getattribute__(self, name)
 
-        api = APIRegistry.api_for(node_uid=self.syft_node_uid)
+        if name in self._syft_passthrough_attrs():
+            return object.__getattribute__(self, name)
+        context_self = self._syft_get_attr_context(name)
 
-        kwargs = {"action": action}
-        api_call = SyftAPICall(
-            node_uid=self.syft_node_uid, path="action.execute", args=[], kwargs=kwargs
-        )
-        return api.make_call(api_call)
+        # Handle bool operator on nonbools
+        if name == "__bool__" and not hasattr(self.syft_action_data, "__bool__"):
+            return self._syft_wrap_attribute_for_bool_on_nonbools(name)
 
-    def syft_make_action(
-        self,
-        path: str,
-        op: str,
-        remote_self: Optional[Union[UID, LineageID]] = None,
-        args: Optional[List[Union[UID, ActionObjectPointer, LineageID]]] = None,
-        kwargs: Optional[Dict[str, Union[UID, ActionObjectPointer, LineageID]]] = None,
-    ) -> Action:
-        if args is None:
-            args = []
-        if kwargs is None:
-            kwargs = {}
-        arg_ids = [
-            LineageID(uid) if isinstance(uid, (UID, LineageID)) else uid.syft_lineage_id
-            for uid in args
-        ]
-        kwarg_ids = {
-            k: LineageID(uid)
-            if isinstance(uid, (LineageID, UID))
-            else uid.syft_lineage_id
-            for k, uid in kwargs.items()
-        }
-        action = Action(
-            path=path,
-            op=op,
-            remote_self=LineageID(remote_self),
-            args=arg_ids,
-            kwargs=kwarg_ids,
-        )
-        return action
+        # Handle Properties
+        if self.syft_is_property(context_self, name):
+            return self._syft_wrap_attribute_for_properties(name)
 
-    def syft_make_method_action(
-        self,
-        op: str,
-        args: Optional[List[Union[UID, ActionObjectPointer]]] = None,
-        kwargs: Optional[Dict[str, Union[UID, ActionObjectPointer]]] = None,
-    ) -> Action:
-        path = self.syft_get_path()
-        return self.syft_make_action(
-            path=path, op=op, remote_self=self.syft_lineage_id, args=args, kwargs=kwargs
-        )
+        # Handle anything else
+        return self._syft_wrap_attribute_for_methods(name)
 
-    def syft_get_path(self) -> str:
-        if isinstance(self, AnyActionObject) and self.syft_internal_type:
-            return f"{self.syft_internal_type.__name__}"
-        return f"{type(self).__name__}"
+    def __setattr__(self, name: str, value: Any) -> Any:
+        defined_on_self = name in self.__dict__ or name in self.__private_attributes__
 
-    def syft_remote_method(
-        self,
-        op: str,
-    ) -> Callable:
-        def wrapper(
-            *args: Optional[List[Union[UID, ActionObjectPointer]]],
-            **kwargs: Optional[Dict[str, Union[UID, ActionObjectPointer]]],
-        ) -> Action:
-            return self.syft_make_method_action(op=op, args=args, kwargs=kwargs)
+        debug(">> ", name, ", defined_on_self = ", defined_on_self)
 
-        return wrapper
+        # use the custom defined version
+        if defined_on_self:
+            self.__dict__[name] = value
+            return value
+        else:
+            context_self = self.syft_action_data  # type: ignore
+            return context_self.__setattr__(name, value)
 
     def keys(self) -> KeysView[str]:
         return self.syft_action_data.keys()  # type: ignore
 
     ###### __DUNDER_MIFFLIN__
 
     # if we do not implement these boiler plate __method__'s then special infix
@@ -709,45 +962,149 @@
 
     def __delattr__(self, key: Any) -> None:
         self.__delattr__(key)
 
     def __delitem__(self, key: Any) -> None:
         self.__delitem__(key)
 
-    def __invert__(self, other: Any) -> Any:
-        return self._syft_output_action_object(self.__invert__(other))
+    def __invert__(self) -> Any:
+        return self._syft_output_action_object(self.__invert__())
+
+    def __round__(self) -> Any:
+        return self._syft_output_action_object(self.__round__())
+
+    def __pos__(self) -> Any:
+        return self._syft_output_action_object(self.__pos__())
+
+    def __trunc__(self) -> Any:
+        return self._syft_output_action_object(self.__trunc__())
 
     def __divmod__(self, other: Any) -> Any:
         return self._syft_output_action_object(self.__divmod__(other))
 
     def __floordiv__(self, other: Any) -> Any:
         return self._syft_output_action_object(self.__floordiv__(other))
 
     def __mod__(self, other: Any) -> Any:
         return self._syft_output_action_object(self.__mod__(other))
 
+    def __abs__(self) -> Any:
+        return self._syft_output_action_object(self.__abs__())
+
+    def __neg__(self) -> Any:
+        return self._syft_output_action_object(self.__neg__())
+
+    def __or__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__or__(other))
+
+    def __and__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__and__(other))
+
+    def __xor__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__xor__(other))
+
+    def __pow__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__pow__(other))
+
+    def __truediv__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__truediv__(other))
+
+    def __lshift__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__lshift__(other))
+
+    def __rshift__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rshift__(other))
+
+    def __iter__(self):
+        return self._syft_output_action_object(self.__iter__())
+
+    def __next__(self):
+        return self._syft_output_action_object(self.__next__())
+
     # r ops
     # we want the underlying implementation so we should just call into __getattribute__
     def __radd__(self, other: Any) -> Any:
         return self.__radd__(other)
 
     def __rsub__(self, other: Any) -> Any:
         return self.__rsub__(other)
 
+    def __rmul__(self, other: Any) -> Any:
+        return self.__rmul__(other)
+
     def __rmatmul__(self, other: Any) -> Any:
         return self.__rmatmul__(other)
 
+    def __rmod__(self, other: Any) -> Any:
+        return self.__rmod__(other)
+
+    def __ror__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__ror__(other))
+
+    def __rand__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rand__(other))
+
+    def __rxor__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rxor__(other))
+
+    def __rpow__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rpow__(other))
+
+    def __rtruediv__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rtruediv__(other))
+
+    def __rfloordiv__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rfloordiv__(other))
+
+    def __rlshift__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rlshift__(other))
+
+    def __rrshift__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rrshift__(other))
+
 
 @serializable()
 class AnyActionObject(ActionObject):
     __canonical_name__ = "AnyActionObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     syft_internal_type: ClassVar[Type[Any]] = Any  # type: ignore
     syft_passthrough_attrs: List[str] = []
     syft_dont_wrap_attrs: List[str] = []
 
     def __float__(self) -> float:
         return float(self.syft_action_data)
 
+    def __int__(self) -> float:
+        return int(self.syft_action_data)
+
 
 action_types[Any] = AnyActionObject
+
+
+def debug_original_func(name: str, func: Callable) -> None:
+    debug(f"{name} func is:")
+    debug("inspect.isdatadescriptor", inspect.isdatadescriptor(func))
+    debug("inspect.isgetsetdescriptor", inspect.isgetsetdescriptor(func))
+    debug("inspect.isfunction", inspect.isfunction(func))
+    debug("inspect.isbuiltin", inspect.isbuiltin(func))
+    debug("inspect.ismethod", inspect.ismethod(func))
+    debug("inspect.ismethoddescriptor", inspect.ismethoddescriptor(func))
+
+
+def is_action_data_empty(obj: Any) -> bool:
+    if hasattr(obj, "syft_action_data"):
+        obj = obj.syft_action_data
+    if isinstance(obj, ActionDataEmpty):
+        return True
+    return False
+
+
+def has_action_data_empty(args: Any, kwargs: Any) -> bool:
+    for a in args:
+        if is_action_data_empty(a):
+            return True
+
+    for _, a in kwargs.items():
+        if is_action_data_empty(a):
+            return True
+    return False
```

### Comparing `syft-0.8.0b9/src/syft/service/action/action_permissions.py` & `syft-0.8.1b1/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/action/action_service.py` & `syft-0.8.1b1/src/syft/service/action/action_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # stdlib
 from enum import Enum
+import importlib
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Union
 
 # third party
 import numpy as np
@@ -19,14 +20,15 @@
 from ..code.user_code import execute_byte_code
 from ..context import AuthedServiceContext
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
+from ..service import UserLibConfigRegistry
 from ..service import service_method
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from .action_object import Action
 from .action_object import ActionObject
 from .action_object import ActionObjectPointer
 from .action_object import AnyActionObject
 from .action_store import ActionStore
@@ -97,15 +99,15 @@
 
     @service_method(path="action.get", name="get", roles=GUEST_ROLE_LEVEL)
     def get(
         self,
         context: AuthedServiceContext,
         uid: UID,
         twin_mode: TwinMode = TwinMode.PRIVATE,
-    ) -> Result[ActionObject, str]:
+    ) -> Result[Ok[ActionObject], Err[str]]:
         """Get an object from the action store"""
         # TODO 🟣 Temporarily added skip permission arguments for enclave
         # until permissions are fully integrated
         result = self.store.get(uid=uid, credentials=context.credentials)
         if result.is_ok():
             obj = result.ok()
             if isinstance(obj, TwinObject):
@@ -115,15 +117,15 @@
                 elif twin_mode == TwinMode.MOCK:
                     obj = obj.mock
                     obj.syft_point_to(context.node.id)
                 else:
                     obj.mock.syft_point_to(context.node.id)
                     obj.private.syft_point_to(context.node.id)
             return Ok(obj)
-        return Err(result.err())
+        return result
 
     @service_method(
         path="action.get_pointer", name="get_pointer", roles=GUEST_ROLE_LEVEL
     )
     def get_pointer(
         self, context: AuthedServiceContext, uid: UID
     ) -> Result[ActionObjectPointer, str]:
@@ -203,47 +205,66 @@
         return Ok(result_action_object)
 
     @service_method(path="action.execute", name="execute", roles=GUEST_ROLE_LEVEL)
     def execute(
         self, context: AuthedServiceContext, action: Action
     ) -> Result[ActionObjectPointer, Err]:
         """Execute an operation on objects in the action store"""
-        resolved_self = self.get(
-            context=context, uid=action.remote_self, twin_mode=TwinMode.NONE
-        )
-        if resolved_self.is_err():
-            return resolved_self.err()
-        resolved_self = resolved_self.ok()
-
-        if isinstance(resolved_self, TwinObject):
-            private_result = execute_object(
-                self, context, resolved_self.private, action, twin_mode=TwinMode.PRIVATE
-            )
-            if private_result.is_err():
-                return private_result.err()
-            mock_result = execute_object(
-                self, context, resolved_self.mock, action, twin_mode=TwinMode.MOCK
-            )
-            if mock_result.is_err():
-                return mock_result.err()
-
-            private_result = private_result.ok()
-            mock_result = mock_result.ok()
 
-            result_action_object = Ok(
-                TwinObject(
-                    id=action.result_id,
-                    private_obj=private_result,
-                    private_obj_id=action.result_id,
-                    mock_obj=mock_result,
-                    mock_obj_id=action.result_id,
-                )
+        if action.remote_self is None:
+            _user_lib_config_registry = UserLibConfigRegistry.from_user(
+                context.credentials
             )
+            absolute_path = f"{action.path}.{action.op}"
+            if absolute_path in _user_lib_config_registry:
+                # TODO: implement properly
+                # Now we are assuming its a function/class
+                result_action_object = execute_callable(self, context, action)
+            else:
+                return Err(f"You have no permission for {absolute_path}")
         else:
-            result_action_object = execute_object(self, context, resolved_self, action)
+            resolved_self = self.get(
+                context=context, uid=action.remote_self, twin_mode=TwinMode.NONE
+            )
+            if resolved_self.is_err():
+                return resolved_self.err()
+            resolved_self = resolved_self.ok()
+
+            if isinstance(resolved_self, TwinObject):
+                private_result = execute_object(
+                    self,
+                    context,
+                    resolved_self.private,
+                    action,
+                    twin_mode=TwinMode.PRIVATE,
+                )
+                if private_result.is_err():
+                    return private_result.err()
+                mock_result = execute_object(
+                    self, context, resolved_self.mock, action, twin_mode=TwinMode.MOCK
+                )
+                if mock_result.is_err():
+                    return mock_result.err()
+
+                private_result = private_result.ok()
+                mock_result = mock_result.ok()
+
+                result_action_object = Ok(
+                    TwinObject(
+                        id=action.result_id,
+                        private_obj=private_result,
+                        private_obj_id=action.result_id,
+                        mock_obj=mock_result,
+                        mock_obj_id=action.result_id,
+                    )
+                )
+            else:
+                result_action_object = execute_object(
+                    self, context, resolved_self, action
+                )
 
         if result_action_object.is_err():
             return result_action_object.err()
         else:
             result_action_object = result_action_object.ok()
 
         set_result = self.store.set(
@@ -267,43 +288,147 @@
         """Checks if the given object id exists in the Action Store"""
         if self.store.exists(obj_id):
             return SyftSuccess(message=f"Object: {obj_id} exists")
         else:
             return SyftError(message=f"Object: {obj_id} does not exist")
 
 
+def execute_callable(
+    service: ActionService,
+    context: AuthedServiceContext,
+    action: Action,
+) -> Result[ActionObject, str]:
+    args = []
+
+    if action.args:
+        for arg_id in action.args:
+            arg_value = service.get(
+                context=context, uid=arg_id, twin_mode=TwinMode.NONE
+            )
+            if arg_value.is_err():
+                return arg_value.err()
+            if isinstance(arg_value.ok(), TwinObject):
+                pass
+            args.append(arg_value.ok())
+
+    kwargs = {}
+    if action.kwargs:
+        for key, arg_id in action.kwargs.items():
+            kwarg_value = service.get(
+                context=context, uid=arg_id, twin_mode=TwinMode.NONE
+            )
+            if kwarg_value.is_err():
+                return kwarg_value.err()
+            if isinstance(kwarg_value.ok(), TwinObject):
+                pass
+            kwargs[key] = kwarg_value.ok()
+
+    # 🔵 TODO 10: Get proper code From old RunClassMethodAction to ensure the function
+    # is not bound to the original object or mutated
+    # stdlib
+
+    # TODO: get from CMPTree is probably safer
+    def _get_target_callable(path: str, op: str):
+        path_elements = path.split(".")
+        res = importlib.import_module(path_elements[0])
+        for p in path_elements[1:]:
+            res = getattr(res, p)
+        res = getattr(res, op)
+        return res
+
+    target_callable = _get_target_callable(action.path, action.op)
+
+    result = None
+    try:
+        if target_callable:
+            # if twin_mode == TwinMode.NONE and not has_twin_inputs:
+            twin_mode = TwinMode.NONE
+            # no twins
+            filtered_args = filter_twin_args(args, twin_mode=twin_mode)
+            filtered_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
+            result = target_callable(*filtered_args, **filtered_kwargs)
+            result_action_object = wrap_result(action.id, action.result_id, result)
+            # elif twin_mode == TwinMode.NONE and has_twin_inputs:
+            #     # self isn't a twin but one of the inputs is
+            #     private_args = filter_twin_args(args, twin_mode=twin_mode)
+            #     private_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
+            #     private_result = target_method(*private_args, **private_kwargs)
+            #     result_action_object_private = wrap_result(
+            #         action.parent_id, action.result_id, private_result
+            #     )
+
+            #     mock_args = filter_twin_args(args, twin_mode=twin_mode)
+            #     mock_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
+            #     mock_result = target_method(*mock_args, **mock_kwargs)
+            #     result_action_object_mock = wrap_result(
+            #         action.parent_id, action.result_id, mock_result
+            #     )
+
+            #     result_action_object = TwinObject(
+            #         id=action.result_id,
+            #         private_obj=result_action_object_private,
+            #         mock_obj=result_action_object_mock,
+            #     )
+            # elif twin_mode == twin_mode.PRIVATE:  # type: ignore
+            #     # twin private path
+            #     private_args = filter_twin_args(args, twin_mode=twin_mode)
+            #     private_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
+            #     result = target_method(*private_args, **private_kwargs)
+            #     result_action_object = wrap_result(
+            #         action.parent_id, action.result_id, result
+            #     )
+            # elif twin_mode == twin_mode.MOCK:  # type: ignore
+            #     # twin mock path
+            #     mock_args = filter_twin_args(args, twin_mode=twin_mode)
+            #     mock_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
+            #     target_method = getattr(unboxed_resolved_self, action.op, None)
+            #     result = target_method(*mock_args, **mock_kwargs)
+            #     result_action_object = wrap_result(
+            #         action.parent_id, action.result_id, result
+            #     )
+            # else:
+            #     raise Exception(
+            #         f"Bad combination of: twin_mode: {twin_mode} and has_twin_inputs: {has_twin_inputs}"
+            #     )
+
+    except Exception as e:
+        print("what is this exception", e)
+        return Err(e)
+    return Ok(result_action_object)
+
+
 def execute_object(
     service: ActionService,
     context: AuthedServiceContext,
     resolved_self: ActionObject,
     action: Action,
     twin_mode: TwinMode = TwinMode.NONE,
-) -> Result[Union[TwinObject, ActionObject], str]:
+) -> Result[Ok[Union[TwinObject, ActionObject]], Err[str]]:
     unboxed_resolved_self = resolved_self.syft_action_data
     args = []
     has_twin_inputs = False
     if action.args:
         for arg_id in action.args:
             arg_value = service.get(
                 context=context, uid=arg_id, twin_mode=TwinMode.NONE
             )
             if arg_value.is_err():
-                return arg_value.err()
+                return arg_value
             if isinstance(arg_value.ok(), TwinObject):
                 has_twin_inputs = True
             args.append(arg_value.ok())
 
     kwargs = {}
     if action.kwargs:
         for key, arg_id in action.kwargs.items():
             kwarg_value = service.get(
                 context=context, uid=arg_id, twin_mode=TwinMode.NONE
             )
             if kwarg_value.is_err():
-                return kwarg_value.err()
+                return kwarg_value
             if isinstance(kwarg_value.ok(), TwinObject):
                 has_twin_inputs = True
             kwargs[key] = kwarg_value.ok()
 
     # 🔵 TODO 10: Get proper code From old RunClassMethodAction to ensure the function
     # is not bound to the original object or mutated
     target_method = getattr(unboxed_resolved_self, action.op, None)
@@ -311,17 +436,15 @@
     try:
         if target_method:
             if twin_mode == TwinMode.NONE and not has_twin_inputs:
                 # no twins
                 filtered_args = filter_twin_args(args, twin_mode=twin_mode)
                 filtered_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
                 result = target_method(*filtered_args, **filtered_kwargs)
-                result_action_object = wrap_result(
-                    action.parent_id, action.result_id, result
-                )
+                result_action_object = wrap_result(action.id, action.result_id, result)
             elif twin_mode == TwinMode.NONE and has_twin_inputs:
                 # self isn't a twin but one of the inputs is
                 private_args = filter_twin_args(args, twin_mode=twin_mode)
                 private_kwargs = filter_twin_kwargs(kwargs, twin_mode=twin_mode)
                 private_result = target_method(*private_args, **private_kwargs)
                 result_action_object_private = wrap_result(
                     action.parent_id, action.result_id, private_result
@@ -356,18 +479,20 @@
                 result_action_object = wrap_result(
                     action.parent_id, action.result_id, result
                 )
             else:
                 raise Exception(
                     f"Bad combination of: twin_mode: {twin_mode} and has_twin_inputs: {has_twin_inputs}"
                 )
+        else:
+            return Err("Missing target method")
 
     except Exception as e:
-        print("what is this exception", e)
         return Err(e)
+
     return Ok(result_action_object)
 
 
 def wrap_result(parent_id: UID, result_id: UID, result: Any) -> ActionObject:
     # 🟡 TODO 11: Figure out how we want to store action object results
     action_type = action_type_for_type(result)
     result_action_object = action_type(
```

### Comparing `syft-0.8.0b9/src/syft/service/action/action_store.py` & `syft-0.8.1b1/src/syft/service/action/action_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...store.dict_document_store import DictStoreConfig
 from ...store.document_store import BasePartitionSettings
 from ...store.document_store import StoreConfig
 from ...types.syft_object import SyftObject
 from ...types.twin_object import TwinObject
+from ...types.uid import LineageID
 from ...types.uid import UID
 from ..response import SyftSuccess
 from .action_permissions import ActionObjectEXECUTE
 from .action_permissions import ActionObjectOWNER
 from .action_permissions import ActionObjectPermission
 from .action_permissions import ActionObjectREAD
 from .action_permissions import ActionObjectWRITE
@@ -56,45 +57,57 @@
             "permissions", self.settings, self.store_config, ddtype=set
         )
         if root_verify_key is None:
             root_verify_key = SyftSigningKey.generate().verify_key
         self.root_verify_key = root_verify_key
 
     def get(self, uid: UID, credentials: SyftVerifyKey) -> Result[SyftObject, str]:
+        uid = uid.id  # We only need the UID from LineageID or UID
+
         # TODO 🟣 Temporarily added skip permission argument for enclave
         # until permissions are fully integrated
         # if you get something you need READ permission
         read_permission = ActionObjectREAD(uid=uid, credentials=credentials)
-        # if True:
         if self.has_permission(read_permission):
-            syft_object = self.data[uid]
+            if isinstance(uid, LineageID):
+                syft_object = self.data[uid.id]
+            elif isinstance(uid, UID):
+                syft_object = self.data[uid]
+            else:
+                raise Exception(f"Unrecognized UID type: {type(uid)}")
             return Ok(syft_object)
         return Err(f"Permission: {read_permission} denied")
 
     def get_pointer(
         self, uid: UID, credentials: SyftVerifyKey, node_uid: UID
     ) -> Result[SyftObject, str]:
+        uid = uid.id  # We only need the UID from LineageID or UID
+
         try:
             # 🟡 TODO 34: do we want pointer read permissions?
             if uid in self.data:
                 obj = self.data[uid]
                 if isinstance(obj, TwinObject):
                     obj = obj.mock
                 obj.syft_point_to(node_uid)
                 return Ok(obj)
             return Err("Permission denied")
         except Exception as e:
             return Err(str(e))
 
     def exists(self, uid: UID) -> bool:
+        uid = uid.id  # We only need the UID from LineageID or UID
+
         return uid in self.data
 
     def set(
         self, uid: UID, credentials: SyftVerifyKey, syft_object: SyftObject
     ) -> Result[SyftSuccess, Err]:
+        uid = uid.id  # We only need the UID from LineageID or UID
+
         # if you set something you need WRITE permission
         write_permission = ActionObjectWRITE(uid=uid, credentials=credentials)
         can_write = self.has_permission(write_permission)
 
         if not self.exists(uid=uid):
             # attempt to claim it for writing
             ownership_result = self.take_ownership(uid=uid, credentials=credentials)
@@ -111,28 +124,32 @@
             self.permissions[uid] = permissions
             return Ok(SyftSuccess(message=f"Set for ID: {uid}"))
         return Err(f"Permission: {write_permission} denied")
 
     def take_ownership(
         self, uid: UID, credentials: SyftVerifyKey
     ) -> Result[SyftSuccess, str]:
+        uid = uid.id  # We only need the UID from LineageID or UID
+
         # first person using this UID can claim ownership
         if uid not in self.permissions and uid not in self.data:
             self.add_permissions(
                 [
                     ActionObjectOWNER(uid=uid, credentials=credentials),
                     ActionObjectWRITE(uid=uid, credentials=credentials),
                     ActionObjectREAD(uid=uid, credentials=credentials),
                     ActionObjectEXECUTE(uid=uid, credentials=credentials),
                 ]
             )
             return Ok(SyftSuccess(message=f"Ownership of ID: {uid} taken."))
         return Err(f"UID: {uid} already owned.")
 
     def delete(self, uid: UID, credentials: SyftVerifyKey) -> Result[SyftSuccess, str]:
+        uid = uid.id  # We only need the UID from LineageID or UID
+
         # if you delete something you need OWNER permission
         # is it bad to evict a key and have someone else reuse it?
         # perhaps we should keep permissions but no data?
         owner_permission = ActionObjectOWNER(uid=uid, credentials=credentials)
         if self.has_permission(owner_permission):
             if uid in self.data:
                 del self.data[uid]
```

### Comparing `syft-0.8.0b9/src/syft/service/action/action_types.py` & `syft-0.8.1b1/src/syft/service/action/action_types.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 # stdlib
 from typing import Any
-from typing import Union
+from typing import Type
 
 # relative
+from ...util.logger import debug
 from .action_data_empty import ActionDataEmpty
 
 action_types = {}
 
 
-def action_type_for_type(obj_or_type: Union[object, type]) -> type:
+def action_type_for_type(obj_or_type: Any) -> Type:
+    """Convert standard type to Syft types
+
+    Parameters:
+        obj_or_type: Union[object, type]
+            Can be an object or a class
+    """
     if type(obj_or_type) != type:
         if isinstance(obj_or_type, ActionDataEmpty):
             obj_or_type = obj_or_type.syft_internal_type
         else:
             obj_or_type = type(obj_or_type)
 
     if obj_or_type not in action_types:
-        # 🟡 TODO: print(f"WARNING: No Type for {obj_or_type}, returning {action_types[Any]}")
+        debug(f"WARNING: No Type for {obj_or_type}, returning {action_types[Any]}")
         return action_types[Any]
+
     return action_types[obj_or_type]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `syft-0.8.0b9/src/syft/service/action/numpy.py` & `syft-0.8.1b1/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/action/pandas.py` & `syft-0.8.1b1/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/action/verification.py` & `syft-0.8.1b1/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/code/unparse.py` & `syft-0.8.1b1/src/syft/service/code/unparse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/code/user_code.py` & `syft-0.8.1b1/src/syft/service/code/user_code.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/code/user_code_parse.py` & `syft-0.8.1b1/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/code/user_code_service.py` & `syft-0.8.1b1/src/syft/service/code/user_code_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/code/user_code_stash.py` & `syft-0.8.1b1/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/context.py` & `syft-0.8.1b1/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/data_subject/data_subject.py` & `syft-0.8.1b1/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.1b1/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.1b1/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.1b1/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/dataset/dataset.py` & `syft-0.8.1b1/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/dataset/dataset_service.py` & `syft-0.8.1b1/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.1b1/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/message/message_service.py` & `syft-0.8.1b1/src/syft/service/message/message_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/message/message_stash.py` & `syft-0.8.1b1/src/syft/service/message/message_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/message/messages.py` & `syft-0.8.1b1/src/syft/service/message/messages.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/metadata/metadata_service.py` & `syft-0.8.1b1/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/metadata/metadata_stash.py` & `syft-0.8.1b1/src/syft/service/metadata/metadata_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/metadata/node_metadata.py` & `syft-0.8.1b1/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/network/network_service.py` & `syft-0.8.1b1/src/syft/service/network/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/policy/policy.py` & `syft-0.8.1b1/src/syft/service/policy/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/policy/policy_service.py` & `syft-0.8.1b1/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.1b1/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/project/project.py` & `syft-0.8.1b1/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/project/project_service.py` & `syft-0.8.1b1/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/project/project_stash.py` & `syft-0.8.1b1/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/queue/queue_stash.py` & `syft-0.8.1b1/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/request/request.py` & `syft-0.8.1b1/src/syft/service/request/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
             )
 
         api = APIRegistry.api_for(self.node_uid)
         if not api:
             raise Exception(f"Login to {self.node_uid} first.")
 
         action_object = ActionObject.from_obj(result)
+
         result = api.services.action.save(action_object)
         if not result:
             return result
 
         permission_request = self.approve()
         if not permission_request:
             return permission_request
```

### Comparing `syft-0.8.0b9/src/syft/service/request/request_service.py` & `syft-0.8.1b1/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/request/request_stash.py` & `syft-0.8.1b1/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/response.py` & `syft-0.8.1b1/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/service.py` & `syft-0.8.1b1/src/syft/service/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,32 @@
 import inspect
 from inspect import Parameter
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Set
 from typing import Tuple
 from typing import Type
 from typing import Union
 
 # third party
 from result import Ok
 from result import OkErr
 
 # relative
 from ..abstract_node import AbstractNode
+from ..node.credentials import SyftVerifyKey
+from ..serde.lib_permissions import CMPCRUDPermission
+from ..serde.lib_permissions import CMPPermission
+from ..serde.lib_service_registry import CMPBase
+from ..serde.lib_service_registry import CMPClass
+from ..serde.lib_service_registry import CMPFunction
+from ..serde.lib_service_registry import action_execute_registry_libs
 from ..serde.serializable import serializable
 from ..serde.signature import Signature
 from ..serde.signature import signature_remove_context
 from ..serde.signature import signature_remove_self
 from ..store.linked_obj import LinkedObject
 from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftObject
@@ -57,28 +65,107 @@
             obj.node_uid = context.node.id
         if not isinstance(obj, OkErr):
             obj = Ok(obj)
         return obj
 
 
 @serializable()
-class ServiceConfig(SyftBaseObject):
+class BaseConfig(SyftBaseObject):
     public_path: str
     private_path: str
     public_name: str
     method_name: str
     doc_string: Optional[str]
-    signature: Signature
+    signature: Optional[Signature]
+    is_from_lib: bool = False
+
+
+@serializable()
+class ServiceConfig(BaseConfig):
     permissions: List
     roles: List[ServiceRole]
 
     def has_permission(self, user_service_role: ServiceRole):
         return user_service_role in self.roles
 
 
+@serializable()
+class LibConfig(BaseConfig):
+    permissions: Set[CMPPermission]
+
+    def has_permission(self, credentials: SyftVerifyKey):
+        # TODO: implement user level permissions
+        for p in self.permissions:
+            if p.permission_string == CMPCRUDPermission.ALL_EXECUTE.name:
+                return True
+            if p.permission_string == CMPCRUDPermission.NONE_EXECUTE.name:
+                return False
+        return False
+
+
+class ServiceConfigRegistry:
+    __service_config_registry__: Dict[str, ServiceConfig] = {}
+    # __public_to_private_path_map__: Dict[str, str] = {}
+
+    @classmethod
+    def register(cls, config: ServiceConfig) -> None:
+        if not cls.path_exists(config.public_path):
+            cls.__service_config_registry__[config.public_path] = config
+            # cls.__public_to_private_path_map__[config.public_path] = config.private_path
+
+    @classmethod
+    def get_registered_configs(cls) -> Dict[str, ServiceConfig]:
+        return cls.__service_config_registry__
+
+    @classmethod
+    def path_exists(cls, path: str):
+        return path in cls.__service_config_registry__
+
+
+class LibConfigRegistry:
+    __service_config_registry__: Dict[str, ServiceConfig] = {}
+
+    @classmethod
+    def register(cls, config: ServiceConfig) -> None:
+        if not cls.path_exists(config.public_path):
+            cls.__service_config_registry__[config.public_path] = config
+
+    @classmethod
+    def get_registered_configs(cls) -> Dict[str, ServiceConfig]:
+        return cls.__service_config_registry__
+
+    @classmethod
+    def path_exists(cls, path: str):
+        return path in cls.__service_config_registry__
+
+
+class UserLibConfigRegistry:
+    def __init__(self, service_config_registry: Dict[str, LibConfig]):
+        self.__service_config_registry__: Dict[str, LibConfig] = service_config_registry
+
+    @classmethod
+    def from_user(cls, credentials: SyftVerifyKey):
+        return cls(
+            {
+                k: lib_config
+                for k, lib_config in LibConfigRegistry.get_registered_configs().items()
+                if lib_config.has_permission(credentials)
+            }
+        )
+
+    def __contains__(self, path: str):
+        return path in self.__service_config_registry__
+
+    def private_path_for(self, public_path: str) -> str:
+        return self.__service_config_registry__[public_path].private_path
+
+    def get_registered_configs(self) -> Dict[str, LibConfig]:
+        return self.__service_config_registry__
+
+
 class UserServiceConfigRegistry:
     def __init__(self, service_config_registry: Dict[str, ServiceConfig]):
         self.__service_config_registry__: Dict[
             str, ServiceConfig
         ] = service_config_registry
 
     @classmethod
@@ -97,31 +184,43 @@
     def private_path_for(self, public_path: str) -> str:
         return self.__service_config_registry__[public_path].private_path
 
     def get_registered_configs(self) -> Dict[str, ServiceConfig]:
         return self.__service_config_registry__
 
 
-class ServiceConfigRegistry:
-    __service_config_registry__: Dict[str, ServiceConfig] = {}
-    # __public_to_private_path_map__: Dict[str, str] = {}
-
-    @classmethod
-    def register(cls, config: ServiceConfig) -> None:
-        if not cls.path_exists(config.public_path):
-            cls.__service_config_registry__[config.public_path] = config
-            # cls.__public_to_private_path_map__[config.public_path] = config.private_path
-
-    @classmethod
-    def get_registered_configs(cls) -> Dict[str, ServiceConfig]:
-        return cls.__service_config_registry__
-
-    @classmethod
-    def path_exists(cls, path: str):
-        return path in cls.__service_config_registry__
+def register_lib_obj(lib_obj: CMPBase):
+    signature = lib_obj.signature
+    path = lib_obj.absolute_path
+    func_name = lib_obj.name
+
+    if signature is not None:
+        if path != "numpy.source":
+            lib_config = LibConfig(
+                public_path=str(path),
+                private_path=str(path),
+                public_name=str(func_name),
+                method_name=str(func_name),
+                doc_string=str(lib_obj.__doc__),
+                signature=signature,
+                permissions=set([lib_obj.permissions]),
+                is_from_lib=True,
+            )
+
+            LibConfigRegistry.register(lib_config)
+
+
+# hacky, prevent circular imports
+for lib_obj in action_execute_registry_libs.flatten():
+    # # for functions
+    # func_name = func.__name__
+    # # for classes
+    # func_name = path.split(".")[-1]
+    if isinstance(lib_obj, CMPFunction) or isinstance(lib_obj, CMPClass):
+        register_lib_obj(lib_obj)
 
 
 def deconstruct_param(param: inspect.Parameter) -> Dict[str, Any]:
     # Gets the init signature form pydantic object
     param_type = param.annotation
     if not hasattr(param_type, "__signature__"):
         raise Exception(
```

### Comparing `syft-0.8.0b9/src/syft/service/user/user.py` & `syft-0.8.1b1/src/syft/service/user/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,17 @@
 @serializable()
 class UserView(SyftObject):
     __canonical_name__ = "UserView"
     __version__ = SYFT_OBJECT_VERSION_1
 
     email: EmailStr
     name: str
+    role: ServiceRole  # make sure role cant be set without uid
+    institution: Optional[str]
+    website: Optional[str]
 
     __attr_repr_cols__ = ["name", "email"]
 
 
 @transform(UserUpdate, User)
 def user_update_to_user() -> List[Callable]:
     return [
```

### Comparing `syft-0.8.0b9/src/syft/service/user/user_roles.py` & `syft-0.8.1b1/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/user/user_service.py` & `syft-0.8.1b1/src/syft/service/user/user_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/service/user/user_stash.py` & `syft-0.8.1b1/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/store/dict_document_store.py` & `syft-0.8.1b1/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/store/document_store.py` & `syft-0.8.1b1/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/store/kv_document_store.py` & `syft-0.8.1b1/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/store/linked_obj.py` & `syft-0.8.1b1/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/store/locks.py` & `syft-0.8.1b1/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/store/mongo_client.py` & `syft-0.8.1b1/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/store/mongo_codecs.py` & `syft-0.8.1b1/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/store/mongo_document_store.py` & `syft-0.8.1b1/src/syft/store/mongo_document_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 from pymongo import ASCENDING
 from pymongo import WriteConcern
 from pymongo.collection import Collection as MongoCollection
 from pymongo.errors import DuplicateKeyError
 from result import Err
 from result import Ok
 from result import Result
+from typing_extensions import Self
 
 # relative
 from ..node.credentials import SyftVerifyKey
 from ..serde.serializable import serializable
 from ..service.action.action_permissions import ActionObjectPermission
 from ..service.action.action_permissions import ActionObjectREAD
 from ..service.action.action_permissions import ActionObjectWRITE
 from ..service.response import SyftSuccess
 from ..types.syft_object import StorableObjectType
+from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftObject
 from ..types.syft_object import SyftObjectRegistry
 from ..types.transforms import TransformContext
 from ..types.transforms import transform
 from ..types.transforms import transform_method
 from .document_store import DocumentStore
 from .document_store import QueryKey
@@ -34,14 +36,31 @@
 from .document_store import StorePartition
 from .locks import LockingConfig
 from .locks import NoLockingConfig
 from .mongo_client import MongoClient
 from .mongo_client import MongoStoreClientConfig
 
 
+@serializable()
+class MongoDict(SyftBaseObject):
+    keys: List[Any]
+    values: List[Any]
+
+    @property
+    def dict(self) -> Dict[Any, Any]:
+        return dict(zip(self.keys, self.values))
+
+    @staticmethod
+    def from_dict(input: Dict[Any, Any]) -> Self:
+        return MongoDict(keys=list(input.keys()), values=list(input.values()))
+
+    def __repr__(self):
+        return self.dict.__repr__()
+
+
 class MongoBsonObject(StorableObjectType, dict):
     pass
 
 
 def _repr_debug_(value: Any) -> str:
     if hasattr(value, "_repr_debug_"):
         return value._repr_debug_()
@@ -62,15 +81,16 @@
         else:
             output[k] = value
 
     if "id" in context.output:
         output["_id"] = context.output["id"]
     output["__canonical_name__"] = context.obj.__canonical_name__
     output["__version__"] = context.obj.__version__
-    output["__obj__"] = context.obj.to_dict()
+    mongo_dict = MongoDict.from_dict(context.obj.to_dict())
+    output["__obj__"] = mongo_dict
     output["__arepr__"] = _repr_debug_(context.obj)  # a comes first in alphabet
     context.output = output
     return context
 
 
 @transform(SyftObject, MongoBsonObject)
 def syft_obj_to_mongo():
@@ -84,15 +104,16 @@
     constructor = SyftObjectRegistry.versioned_class(
         name=storage_obj["__canonical_name__"], version=storage_obj["__version__"]
     )
     if constructor is None:
         raise ValueError(
             "Versioned class should not be None for initialization of SyftObject."
         )
-    output = storage_obj["__obj__"]
+    mongo_dict = storage_obj["__obj__"]
+    output = mongo_dict.dict
     for attr, funcs in constructor.__serde_overrides__.items():
         if attr in output:
             output[attr] = funcs[1](output[attr])
     return constructor(**output)
 
 
 @serializable(attrs=["storage_type"])
```

### Comparing `syft-0.8.0b9/src/syft/store/sqlite_document_store.py` & `syft-0.8.1b1/src/syft/store/sqlite_document_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 
 # third party
+from result import Err
+from result import Ok
+from result import Result
 from typing_extensions import Self
 
 # relative
 from ..serde.deserialize import _deserialize
 from ..serde.serializable import serializable
 from ..serde.serialize import _serialize
 from ..types.uid import UID
@@ -30,15 +33,15 @@
 from .kv_document_store import KeyValueStorePartition
 from .locks import FileLockingConfig
 from .locks import LockingConfig
 
 
 def _repr_debug_(value: Any) -> str:
     if hasattr(value, "_repr_debug_"):
-        return value._repr_debug_()
+        return str(value._repr_debug_())
     return repr(value)
 
 
 def thread_ident() -> int:
     return threading.current_thread().ident
 
 
@@ -122,109 +125,128 @@
         self.db.close()
 
     def _commit(self) -> None:
         self.db.commit()
 
     def _execute(
         self, sql: str, *args: Optional[List[Any]]
-    ) -> Optional[sqlite3.Cursor]:
+    ) -> Result[Ok[sqlite3.Cursor], Err[str]]:
         cursor: Optional[sqlite3.Cursor] = None
-
+        err = None
         try:
             cursor = self.cur.execute(sql, *args)
-        except BaseException:
+        except BaseException as e:
             self.db.rollback()  # Roll back all changes if an exception occurs.
+            err = Err(str(e))
         else:
             self.db.commit()  # Commit if everything went ok
 
-        return cursor
+        if err is not None:
+            return err
+
+        return Ok(cursor)
 
     def _set(self, key: UID, value: Any) -> None:
         if self._exists(key):
             self._update(key, value)
         else:
             insert_sql = f"insert into {self.table_name} (uid, repr, value) VALUES (?, ?, ?)"  # nosec
             data = _serialize(value, to_bytes=True)
-            self._execute(insert_sql, [str(key), _repr_debug_(value), data])
+            res = self._execute(insert_sql, [str(key), _repr_debug_(value), data])
+            if res.is_err():
+                raise ValueError(res.err())
 
     def _update(self, key: UID, value: Any) -> None:
         insert_sql = f"update {self.table_name} set uid = ?, repr = ?, value = ? where uid = ?"  # nosec
         data = _serialize(value, to_bytes=True)
-        self._execute(insert_sql, [str(key), _repr_debug_(value), data, str(key)])
+        res = self._execute(insert_sql, [str(key), _repr_debug_(value), data, str(key)])
+        if res.is_err():
+            raise ValueError(res.err())
 
     def _get(self, key: UID) -> Any:
         select_sql = f"select * from {self.table_name} where uid = ?"  # nosec
-        cursor = self._execute(select_sql, [str(key)])
-        if cursor is None:
+        res = self._execute(select_sql, [str(key)])
+        if res.is_err():
             raise KeyError(f"Query {select_sql} failed")
+        cursor = res.ok()
 
         row = cursor.fetchone()
         if row is None or len(row) == 0:
             raise KeyError(f"{key} not in {type(self)}")
         data = row[2]
         return _deserialize(data, from_bytes=True)
 
     def _exists(self, key: UID) -> bool:
         select_sql = f"select uid from {self.table_name} where uid = ?"  # nosec
 
-        cursor = self._execute(select_sql, [str(key)])
-        if cursor is None:
+        res = self._execute(select_sql, [str(key)])
+        if res.is_err():
             return False
+        cursor = res.ok()
 
         row = cursor.fetchone()
         if row is None:
             return False
 
         return bool(row)
 
     def _get_all(self) -> Any:
         select_sql = f"select * from {self.table_name}"  # nosec
         keys = []
         data = []
 
-        cursor = self._execute(select_sql)
-        if cursor is None:
+        res = self._execute(select_sql)
+        if res.is_err():
             return {}
+        cursor = res.ok()
 
         rows = cursor.fetchall()
         if rows is None:
             return {}
 
         for row in rows:
             keys.append(UID(row[0]))
             data.append(_deserialize(row[2], from_bytes=True))
         return dict(zip(keys, data))
 
     def _get_all_keys(self) -> Any:
         select_sql = f"select uid from {self.table_name}"  # nosec
         keys = []
 
-        cursor = self._execute(select_sql)
-        if cursor is None:
+        res = self._execute(select_sql)
+        if res.is_err():
             return []
+        cursor = res.ok()
 
         rows = cursor.fetchall()
         if rows is None:
             return []
 
         for row in rows:
             keys.append(UID(row[0]))
         return keys
 
     def _delete(self, key: UID) -> None:
         select_sql = f"delete from {self.table_name} where uid = ?"  # nosec
-        self._execute(select_sql, [str(key)])
+        res = self._execute(select_sql, [str(key)])
+        if res.is_err():
+            raise ValueError(res.err())
 
     def _delete_all(self) -> None:
         select_sql = f"delete from {self.table_name}"  # nosec
-        self._execute(select_sql)
+        res = self._execute(select_sql)
+        if res.is_err():
+            raise ValueError(res.err())
 
     def _len(self) -> int:
         select_sql = f"select count(uid) from {self.table_name}"  # nosec
-        cursor = self._execute(select_sql)
+        res = self._execute(select_sql)
+        if res.is_err():
+            raise ValueError(res.err())
+        cursor = res.ok()
         cnt = cursor.fetchone()[0]
         return cnt
 
     def __setitem__(self, key: Any, value: Any) -> None:
         self._set(key, value)
 
     def __getitem__(self, key: Any) -> Self:
```

### Comparing `syft-0.8.0b9/src/syft/types/datetime.py` & `syft-0.8.1b1/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/types/grid_url.py` & `syft-0.8.1b1/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/types/syft_metaclass.py` & `syft-0.8.1b1/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/types/syft_object.py` & `syft-0.8.1b1/src/syft/types/syft_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/types/transforms.py` & `syft-0.8.1b1/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/types/twin_object.py` & `syft-0.8.1b1/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/types/uid.py` & `syft-0.8.1b1/src/syft/types/uid.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,19 +61,17 @@
         """
         # checks to make sure you've set a proto_type
         super().__init__()
 
         # if value is not set - create a novel and unique ID.
         if isinstance(value, str):
             value = uuid.UUID(value)
-
-        if isinstance(value, bytes):
+        elif isinstance(value, bytes):
             value = uuid.UUID(bytes=value)
-
-        if isinstance(value, UID):
+        elif isinstance(value, UID):
             value = value.value
 
         self.value = uuid.uuid4() if value is None else value
 
     @staticmethod
     def from_string(value: str) -> "UID":
         try:
@@ -180,14 +178,18 @@
 
         Return a SHORT human-readable version of the ID which
         makes it print nicer when embedded (often alongside other
         UID objects) within other object __repr__ methods."""
 
         return f"..{str(self.value)[-5:]}"
 
+    @property
+    def id(self) -> "UID":
+        return self
+
     @staticmethod
     def _check_or_convert(value: Union[str, "UID", uuid.UUID]) -> "UID":
         if isinstance(value, uuid.UUID):
             return UID(value)
         elif isinstance(value, str):
             return UID.from_string(value)
         elif isinstance(value, UID):
@@ -197,41 +199,46 @@
             return ValueError(  # type: ignore
                 f"Incorrect value,type:{value,type(value)} for conversion to UID, expected Union[str,UID,UUID]"
             )
 
 
 @serializable(attrs=["syft_history_hash"])
 class LineageID(UID):
+    """Extended UID containing a history hash as well, which is used for comparisons."""
+
     syft_history_hash: int
 
     def __init__(
         self,
         value: Optional[Union[uuid_type, str, bytes]] = None,
         syft_history_hash: Optional[int] = None,
     ):
         if isinstance(value, LineageID):
             syft_history_hash = value.syft_history_hash
             value = value.value
 
-        if isinstance(value, UID):
-            self.value = value.value
-        else:
-            super().__init__(value)
+        super().__init__(value)
 
         if syft_history_hash is None:
             syft_history_hash = hash(self.value)
         self.syft_history_hash = syft_history_hash
 
     @property
     def id(self) -> UID:
         return UID(self.value)
 
+    def __hash__(self):
+        return hash((self.syft_history_hash, self.value))
+
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, LineageID):
             return (
                 self.id == other.id
                 and self.syft_history_hash == other.syft_history_hash
             )
-        return self == other
+        elif isinstance(other, UID):
+            return hash(self) == hash(other)
+        else:
+            raise ValueError(f"Unsupported comparison: LineageID with {type(other)}")
 
     def __repr__(self) -> str:
         return f"<{type(self).__name__}: {self.no_dash} - {self.syft_history_hash}>"
```

### Comparing `syft-0.8.0b9/src/syft/util/decorators.py` & `syft-0.8.1b1/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/util/experimental_flags.py` & `syft-0.8.1b1/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/util/filterwarnings.py` & `syft-0.8.1b1/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/util/logger.py` & `syft-0.8.1b1/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/util/telemetry.py` & `syft-0.8.1b1/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/util/trace_decorator.py` & `syft-0.8.1b1/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/util/util.py` & `syft-0.8.1b1/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b9/src/syft/util/version_compare.py` & `syft-0.8.1b1/src/syft/util/version_compare.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,43 +29,70 @@
         elif one_char in operators.keys():
             op_char = one_char
             version_string = version_string[1:]
     op = operators[op_char]
     return version_string, op, op_char
 
 
+def check_rule(version_string: str, LATEST_STABLE_SYFT: str, __version__: str) -> bool:
+    version_string, op, op_char = get_operator(version_string)
+    syft_version = version.parse(__version__)
+    stable_version = version.parse(LATEST_STABLE_SYFT)
+    required = version.parse(version_string)
+    result = op(syft_version, required)
+
+    requirements = []
+    messages = []
+
+    if result:
+        requirements.append(f"the requirement {op_char}{required}")
+    else:
+        requirements.append(f"the requirement {op_char}{required}")
+        pre = ""
+        if required.minor > stable_version.minor:
+            pre = " --pre"
+        msg = f"Alternatively you could try to match {op_char}{required} with:\n"
+        if required > syft_version:
+            upgrade = f"pip install -U{pre} syft or "
+        else:
+            upgrade = ""
+        msg += f"{upgrade}pip install syft=={required}"
+        messages.append(msg)
+    return result, requirements, messages
+
+
 def make_requires(LATEST_STABLE_SYFT: str, __version__: str) -> Callable:
     def requires(version_string: str, silent: bool = False) -> Optional[bool]:
-        version_string, op, op_char = get_operator(version_string)
         syft_version = version.parse(__version__)
-        stable_version = version.parse(LATEST_STABLE_SYFT)
-        required = version.parse(version_string)
-        result = op(syft_version, required)
+        parts = version_string.split(",")
+        result = True
+        all_requirements = []
+        all_messages = []
+        for part in parts:
+            part_result, requirements, messages = check_rule(
+                version_string=part,
+                LATEST_STABLE_SYFT=LATEST_STABLE_SYFT,
+                __version__=__version__,
+            )
+            all_requirements += requirements
+            all_messages += messages
+            if not part_result:
+                result = False
+
         if silent:
             return result
 
+        msg_requirements = " and ".join(all_requirements)
         if result:
             print(
-                f"✅ The installed version of syft=={syft_version} matches "
-                f"the requirement {op_char}{required}"
+                f"✅ The installed version of syft=={syft_version} matches {msg_requirements}"
             )
         else:
             print(
-                f"❌ The installed version of syft=={syft_version} doesn't match "
-                f"the requirement {op_char}{required}."
-            )
-            pre = ""
-            if required.minor > stable_version.minor:
-                pre = " --pre"
-            print(
-                f"This code or notebook may have issues if APIs have changed.\n"
-                f"Alternatively you could try to match {op_char}{required} it with:\n"
+                f"❌ The installed version of syft=={syft_version} doesn't match {msg_requirements}"
             )
-            if required > syft_version:
-                upgrade = f"pip install -U{pre} syft or "
-            else:
-                upgrade = ""
-            msg = f"{upgrade}pip install syft=={required}"
-            print(msg)
+        if len(all_messages):
+            print("This code or notebook may have issues if APIs have changed\n")
+            print("\n\n".join(all_messages))
         return None
 
     return requires
```

### Comparing `syft-0.8.0b9/src/syft.egg-info/PKG-INFO` & `syft-0.8.1b1/src/syft.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.0b9
+Version: 0.8.1b1
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: dev
 Provides-Extra: test_plugins
 Provides-Extra: oblv
 License-File: LICENSE
 
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://pepy.tech/badge/syft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
@@ -24,49 +24,45 @@
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/img/title_syft_dark.png">
   <img alt="Syft Logo" src="docs/img/title_syft_light.png" width="200px" />
 </picture>
 
 Perform `numpy`-like analysis on `data` that remains in `someone else's` server
 
-<div align="left">
-<img alt="Syft Logo" src="docs/img/header.png" alt="Syft Overview" width="100%" />
-</div>
-
 # Quickstart
 
 ✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
 
-## Install syft on Python 3.8 - 3.10
+## Install syft on Python 3.9 - 3.10
 
 ```bash
-$ pip install --pre syft -f https://whls.blob.core.windows.net/unstable/index.html
+$ pip install -U syft -f https://whls.blob.core.windows.net/unstable/index.html
 ```
 
 ## Launch a python dev Domain
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8-beta")
+sy.requires(">=0.8,<0.8.1")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Connect with our Python Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8-beta")
+sy.requires(">=0.8,<0.8.1")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## Deploy to a Container Engine or Cloud
 
 1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server a one-liner:  
    `pip install -U hagrid`
@@ -79,34 +75,36 @@
 
    `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
 
 4. During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `podman` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†
 
 ## Docs and Support
 
+- 📝 <a href="/notebooks/api">API Example Notebooks</a>
 - 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
 - HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
   †`Windows` does not support `ansible`, preventing some remote deployment targets
-- PySyft 0.8 Requires: 🐍 `python 3.8 - 3.10` - Run: `pip install -U syft`  
+- PySyft 0.8 Requires: 🐍 `python 3.9 - 3.10` - Run: `pip install -U syft`  
   \*`macOS` Apple Silicon users might need cmake: `brew install cmake`  
   ‡`Windows` users must run this first: `pip install jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html`
 - PyGrid Requires: 🐳 `docker` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
 
 # Versions
 
-`0.8.0` (Beta) - `dev` branch 👈🏽  
-`0.7.0` (Stable) - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
+`0.8.1` (Beta) - `dev` branch 👈🏽 <a href="/notebooks/api/0.8">API</a>  
+`0.8.0` (Stable) - <a href="/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
 - `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
 
 PySyft (Stable): `pip install -U syft`
```

#### html2text {}

```diff
@@ -1,81 +1,81 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.0b9 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b1 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
-Python Requires-Python: >=3.8 Description-Content-Type: text/markdown;
+Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
 Provides-Extra: oblv License-File: LICENSE
 [https://pepy.tech/badge/syft] [https://badge.fury.io/py/syft.svg] [https://
 img.shields.io/badge/docker-images-blue?logo=docker] [https://github.com/
 OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev] [https:/
 /img.shields.io/badge/chat-on%20slack-purple?logo=slack] [https://
 img.shields.io/badge/read-docs-yellow?logo=mdbook]
 
   [Syft Logo]  Perform `numpy`-like analysis on `data` that remains in `someone
-else's` server
-[Syft Logo]
-# Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ## Install syft on
-Python 3.8 - 3.10 ```bash $ pip install --pre syft -f https://
+else's` server # Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ##
+Install syft on Python 3.9 - 3.10 ```bash $ pip install -U syft -f https://
 whls.blob.core.windows.net/unstable/index.html ``` ## Launch a python dev
-Domain ```python # from Jupyter / Python import syft as sy sy.requires(">=0.8-
-beta") node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True,
-reset=True) ``` ```bash # or from the command line $ syft launch --name=my-
-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:8080 ```
-## Connect with our Python Client ```python import syft as sy sy.requires
-(">=0.8-beta") domain_client = sy.login(port=8080, email="info@openmined.org",
-password="changethis") ``` ## Deploy to a Container Engine or Cloud 1. Install
-our handy ðµ cli tool which makes deploying a Domain or Gateway server a one-
-liner: `pip install -U hagrid` 2. Then run our interactive jupyter Install
-ð§ð½ââï¸ WizardBETA: `hagrid quickstart` 3. In the tutorial you will
-learn how to install and deploy: `PySyft` = our `numpy`-like ð Python
-library for computing on `private data` in someone else's `Domain` `PyGrid` =
-our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where `private data`
-lives 4. During quickstart we will deploy `PyGrid` to localhost with ð³
-`docker`, however ðµ HAGrid can deploy to `podman` or a ð§ `ubuntu` VM on
-`azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨ `ansible`â  ## Docs and
-Support - ð Docs - `#support` on Slack # Install Notes - HAGrid 0.3
-Requires: ð `python` ð `git` - Run: `pip install -U hagrid` - Interactive
-Install ð§ð½ââï¸ WizardBETA Requires ðµ `hagrid`: - Run: `hagrid
-quickstart` â `Windows` does not support `ansible`, preventing some remote
-deployment targets - PySyft 0.8 Requires: ð `python 3.8 - 3.10` - Run: `pip
-install -U syft` \*`macOS` Apple Silicon users might need cmake: `brew install
-cmake` â¡`Windows` users must run this first: `pip install jaxlib==0.3.14 -
-f https://whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires:
-ð³ `docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.0`
-(Beta) - `dev` branch ðð½ `0.7.0` (Stable) - Course_3_Updated Deprecated:
-- `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix - `0.2.0` - `0.5.0`
-PySyft and PyGrid use the same `version` and its best to match them up where
-possible. We release weekly betas which can be used in each context: PySyft
-(Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch ... tag=latest`
-PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta): `hagrid launch ...
-tag=beta` HAGrid is a cli / deployment tool so the latest version of `hagrid`
-is usually the best. # What is Syft?   [Syft]  `Syft` is OpenMined's `open
-source` stack that provides `secure` and `private` Data Science in Python. Syft
-decouples `private data` from model training, using techniques like [Federated
-Learning](https://ai.googleblog.com/2017/04/federated-learning-
-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/
-Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/
-wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and
-integration with `Deep Learning` frameworks, so that you as a `Data Scientist`
-can maintain your current workflow while using these new `privacy-enhancing
-techniques`. ### Why should I use Syft? `Syft` allows a `Data Scientist` to ask
-`questions` about a `dataset` and, within `privacy limits` set by the `data
-owner`, get `answers` to those `questions`, all without obtaining a `copy` of
-the data itself. We call this process `Remote Data Science`. It means in a wide
-variety of `domains` across society, the current `risks` of sharing information
-(`copying` data) with someone such as, privacy invasion, IP theft and blackmail
-will no longer prevent the vast `benefits` such as innovation, insights and
-scientific discovery which secure access will provide. No more cold calls to
-get `access` to a dataset. No more weeks of `wait times` to get a `result` on
-your `query`. It also means `1000x more data` in every domain. PySyft opens the
-doors to a streamlined Data Scientist `workflow`, all with the individual's
-`privacy` at its heart. # Tutorials
+Domain ```python # from Jupyter / Python import syft as sy sy.requires
+(">=0.8,<0.8.1") node = sy.orchestra.launch(name="my-domain", port=8080,
+dev_mode=True, reset=True) ``` ```bash # or from the command line $ syft launch
+--name=my-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:
+8080 ``` ## Connect with our Python Client ```python import syft as sy
+sy.requires(">=0.8,<0.8.1") domain_client = sy.login(port=8080,
+email="info@openmined.org", password="changethis") ``` ## Deploy to a Container
+Engine or Cloud 1. Install our handy ðµ cli tool which makes deploying a
+Domain or Gateway server a one-liner: `pip install -U hagrid` 2. Then run our
+interactive jupyter Install ð§ð½ââï¸ WizardBETA: `hagrid quickstart`
+3. In the tutorial you will learn how to install and deploy: `PySyft` = our
+`numpy`-like ð Python library for computing on `private data` in someone
+else's `Domain` `PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway`
+Servers where `private data` lives 4. During quickstart we will deploy `PyGrid`
+to localhost with ð³ `docker`, however ðµ HAGrid can deploy to `podman` or
+a ð§ `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨
+`ansible`â  ## Docs and Support - ð API_Example_Notebooks - ð Docs -
+`#support` on Slack # Install Notes - HAGrid 0.3 Requires: ð `python` ð
+`git` - Run: `pip install -U hagrid` - Interactive Install ð§ð½ââï¸
+WizardBETA Requires ðµ `hagrid`: - Run: `hagrid quickstart` â `Windows` does
+not support `ansible`, preventing some remote deployment targets - PySyft 0.8
+Requires: ð `python 3.9 - 3.10` - Run: `pip install -U syft` \*`macOS` Apple
+Silicon users might need cmake: `brew install cmake` â¡`Windows` users must
+run this first: `pip install jaxlib==0.3.14 -f https://
+whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires: ð³
+`docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.1`
+(Beta) - `dev` branch ðð½ API `0.8.0` (Stable) - API Deprecated: - `0.7.0`
+- Course_3_Updated - `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix -
+`0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
+match them up where possible. We release weekly betas which can be used in each
+context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
+... tag=latest` PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta):
+`hagrid launch ... tag=beta` HAGrid is a cli / deployment tool so the latest
+version of `hagrid` is usually the best. # What is Syft?   [Syft]  `Syft` is
+OpenMined's `open source` stack that provides `secure` and `private` Data
+Science in Python. Syft decouples `private data` from model training, using
+techniques like [Federated Learning](https://ai.googleblog.com/2017/04/
+federated-learning-collaborative.html), [Differential Privacy](https://
+en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https:
+//en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-
+like interface and integration with `Deep Learning` frameworks, so that you as
+a `Data Scientist` can maintain your current workflow while using these new
+`privacy-enhancing techniques`. ### Why should I use Syft? `Syft` allows a
+`Data Scientist` to ask `questions` about a `dataset` and, within `privacy
+limits` set by the `data owner`, get `answers` to those `questions`, all
+without obtaining a `copy` of the data itself. We call this process `Remote
+Data Science`. It means in a wide variety of `domains` across society, the
+current `risks` of sharing information (`copying` data) with someone such as,
+privacy invasion, IP theft and blackmail will no longer prevent the vast
+`benefits` such as innovation, insights and scientific discovery which secure
+access will provide. No more cold calls to get `access` to a dataset. No more
+weeks of `wait times` to get a `result` on your `query`. It also means `1000x
+more data` in every domain. PySyft opens the doors to a streamlined Data
+Scientist `workflow`, all with the individual's `privacy` at its heart. #
+Tutorials
  _____________________________________________________________________________
 |             [Image]     |            [Image]      |            [Image]      |
 |___________Data_Owner____|________Data_Scientist___|_________Data_Engineer___|
 |- Deploy_a_Domain_Server |- Install Syft           |- Setup Dev Mode         |
 |- Upload_Private_Data -  | - Connect to a Domain   | - Deploy to Azure -     |
 |Create_Accounts - Manage | - Search for Datasets   |Deploy to GCP - Deploy to|
 |Privacy Budget           | - Train Models -        |Kubernetes - Customize   |
```

### Comparing `syft-0.8.0b9/src/syft.egg-info/SOURCES.txt` & `syft-0.8.1b1/src/syft.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 src/syft/node/worker.py
 src/syft/node/worker_settings.py
 src/syft/serde/__init__.py
 src/syft/serde/array.py
 src/syft/serde/arrow.py
 src/syft/serde/capnp.py
 src/syft/serde/deserialize.py
+src/syft/serde/lib_permissions.py
+src/syft/serde/lib_service_registry.py
 src/syft/serde/recursive.py
 src/syft/serde/recursive_primitives.py
 src/syft/serde/serializable.py
 src/syft/serde/serialize.py
 src/syft/serde/signature.py
 src/syft/serde/third_party.py
 src/syft/service/__init__.py
```

### Comparing `syft-0.8.0b9/src/syft.egg-info/requires.txt` & `syft-0.8.1b1/src/syft.egg-info/requires.txt`

 * *Files identical despite different names*

