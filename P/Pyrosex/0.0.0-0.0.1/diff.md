# Comparing `tmp/Pyrosex-0.0.0.tar.gz` & `tmp/Pyrosex-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pyrosex-0.0.0.tar", last modified: Sun May  7 08:49:31 2023, max compression
+gzip compressed data, was "Pyrosex-0.0.1.tar", last modified: Sun May  7 09:08:29 2023, max compression
```

## Comparing `Pyrosex-0.0.0.tar` & `Pyrosex-0.0.1.tar`

### file list

```diff
@@ -1,484 +1,484 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.654057 Pyrosex-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-07 08:49:31.650057 Pyrosex-0.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.594057 Pyrosex-0.0.0/Pyrosex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-07 08:49:31.000000 Pyrosex-0.0.0/Pyrosex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-05-07 08:49:31.000000 Pyrosex-0.0.0/Pyrosex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 08:49:31.000000 Pyrosex-0.0.0/Pyrosex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 08:49:31.000000 Pyrosex-0.0.0/Pyrosex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 08:49:31.000000 Pyrosex-0.0.0/Pyrosex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 08:49:31.000000 Pyrosex-0.0.0/Pyrosex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.594057 Pyrosex-0.0.0/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.594057 Pyrosex-0.0.0/compiler/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20048 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/api/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.594057 Pyrosex-0.0.0/compiler/api/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/api/source/auth_key.tl
--rw-r--r--   0 runner    (1001) docker     (123)   148190 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/api/source/main_api.tl
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.594057 Pyrosex-0.0.0/compiler/api/template/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/api/template/combinator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/api/template/type.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.594057 Pyrosex-0.0.0/compiler/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/docs/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.594057 Pyrosex-0.0.0/compiler/docs/template/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/docs/template/page.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.594057 Pyrosex-0.0.0/compiler/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.598057 Pyrosex-0.0.0/compiler/errors/source/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    22041 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.598057 Pyrosex-0.0.0/compiler/errors/template/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/template/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.598057 Pyrosex-0.0.0/pyrosex/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38779 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.598057 Pyrosex-0.0.0/pyrosex/connection/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.598057 Pyrosex-0.0.0/pyrosex/connection/transport/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/connection/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.598057 Pyrosex-0.0.0/pyrosex/connection/transport/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/connection/transport/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/connection/transport/tcp/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.602057 Pyrosex-0.0.0/pyrosex/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/crypto/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/crypto/mtproto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/crypto/prime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/crypto/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)   207202 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/emoji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.602057 Pyrosex-0.0.0/pyrosex/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/auto_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/chat_event_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/chat_member_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/chat_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/message_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/message_media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/message_service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/messages_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/next_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/parse_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/sent_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/enums/user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.602057 Pyrosex-0.0.0/pyrosex/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/errors/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/file_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.606057 Pyrosex-0.0.0/pyrosex/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/callback_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/chat_join_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/chat_member_updated_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/deleted_messages_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/disconnect_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/edited_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/inline_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/poll_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/raw_update_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/handlers/user_status_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.606057 Pyrosex-0.0.0/pyrosex/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.606057 Pyrosex-0.0.0/pyrosex/methods/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/advanced/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/advanced/resolve_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/advanced/save_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.606057 Pyrosex-0.0.0/pyrosex/methods/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/check_password.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/get_password_hint.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/log_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/recover_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/resend_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/send_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/send_recovery_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/sign_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/sign_in_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/auth/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.610057 Pyrosex-0.0.0/pyrosex/methods/bots/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/answer_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/answer_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/answer_web_app_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/delete_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/get_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/get_game_high_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/request_callback_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/send_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/set_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/bots/set_game_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.614057 Pyrosex-0.0.0/pyrosex/methods/chats/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/add_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/archive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/ban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/create_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/create_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/create_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/delete_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/delete_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/delete_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/delete_user_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/get_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/get_chat_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/get_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/get_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/get_chat_members_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/get_chat_online_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/get_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/get_dialogs_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/get_nearby_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/get_send_as_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/join_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/leave_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/mark_chat_unread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/pin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/promote_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/restrict_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/set_administrator_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/set_chat_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/set_chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/set_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/set_chat_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/set_chat_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/set_send_as_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/set_slow_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/unarchive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/unban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.614057 Pyrosex-0.0.0/pyrosex/methods/contacts/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/contacts/add_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/contacts/delete_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/contacts/get_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/contacts/get_contacts_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/contacts/import_contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.618057 Pyrosex-0.0.0/pyrosex/methods/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/on_cb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/on_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/on_edited_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/on_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/on_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/on_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/on_raw_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/decorators/on_user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.618057 Pyrosex-0.0.0/pyrosex/methods/invite_links/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.626057 Pyrosex-0.0.0/pyrosex/methods/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/copy_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/copy_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/delete_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/download_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/edit_inline_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/edit_inline_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/edit_inline_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/edit_message_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/edit_message_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/edit_message_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/forward_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/get_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/get_chat_history_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/get_discussion_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/get_discussion_replies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/get_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/inline_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/read_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/retract_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/search_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/search_global_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/search_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/search_messages_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_cached_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/send_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/stop_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/stream_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/messages/vote_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.626057 Pyrosex-0.0.0/pyrosex/methods/password/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/password/change_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/password/enable_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.630057 Pyrosex-0.0.0/pyrosex/methods/users/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/users/block_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/users/delete_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/users/get_chat_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/users/get_chat_photos_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/users/get_common_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/users/get_me.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/users/set_profile_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/users/set_username.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/users/unblock_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/users/update_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.630057 Pyrosex-0.0.0/pyrosex/methods/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/utilities/add_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/utilities/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/utilities/export_session_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/utilities/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/utilities/remove_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/utilities/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/utilities/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/utilities/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/utilities/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/methods/utilities/stop_transmission.py
--rw-r--r--   0 runner    (1001) docker     (123)    60961 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/mime_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.630057 Pyrosex-0.0.0/pyrosex/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/parser/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/parser/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.630057 Pyrosex-0.0.0/pyrosex/raw/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.634057 Pyrosex-0.0.0/pyrosex/raw/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/future_salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/future_salts.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/gzip_packed.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/msg_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.634057 Pyrosex-0.0.0/pyrosex/raw/core/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/primitives/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/primitives/double.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/primitives/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/primitives/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/raw/core/tl_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.634057 Pyrosex-0.0.0/pyrosex/session/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/session/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.634057 Pyrosex-0.0.0/pyrosex/session/internals/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/session/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/session/internals/data_center.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/session/internals/msg_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/session/internals/msg_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/session/internals/seq_no.py
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.634057 Pyrosex-0.0.0/pyrosex/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/storage/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/storage/memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/storage/sqlite_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.634057 Pyrosex-0.0.0/pyrosex/types/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.634057 Pyrosex-0.0.0/pyrosex/types/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/authorization/sent_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/authorization/terms_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.638057 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.642057 Pyrosex-0.0.0/pyrosex/types/inline_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.642057 Pyrosex-0.0.0/pyrosex/types/input_media/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/input_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/input_media/input_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/input_media/input_media_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/input_media/input_media_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/input_media/input_media_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/input_media/input_media_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/input_media/input_media_video.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.646057 Pyrosex-0.0.0/pyrosex/types/input_message_content/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/input_message_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/input_message_content/input_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.646057 Pyrosex-0.0.0/pyrosex/types/messages_and_media/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/game.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/location.py
--rw-r--r--   0 runner    (1001) docker     (123)   142440 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/message_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/poll_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/web_app_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/messages_and_media/web_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/object.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.650057 Pyrosex-0.0.0/pyrosex/types/user_and_chats/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31615 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/pyrosex/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 08:49:31.654057 Pyrosex-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.650057 Pyrosex-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:49:31.650057 Pyrosex-0.0.0/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/tests/filters/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-07 08:49:20.000000 Pyrosex-0.0.0/tests/test_file_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.669459 Pyrosex-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-07 09:08:29.669459 Pyrosex-0.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.613458 Pyrosex-0.0.1/Pyrosex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-07 09:08:29.000000 Pyrosex-0.0.1/Pyrosex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-05-07 09:08:29.000000 Pyrosex-0.0.1/Pyrosex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:08:29.000000 Pyrosex-0.0.1/Pyrosex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:08:29.000000 Pyrosex-0.0.1/Pyrosex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 09:08:29.000000 Pyrosex-0.0.1/Pyrosex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 09:08:29.000000 Pyrosex-0.0.1/Pyrosex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.613458 Pyrosex-0.0.1/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.613458 Pyrosex-0.0.1/compiler/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20048 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/api/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.617457 Pyrosex-0.0.1/compiler/api/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/api/source/auth_key.tl
+-rw-r--r--   0 runner    (1001) docker     (123)   148190 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/api/source/main_api.tl
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.617457 Pyrosex-0.0.1/compiler/api/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/api/template/combinator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/api/template/type.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.617457 Pyrosex-0.0.1/compiler/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/docs/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.617457 Pyrosex-0.0.1/compiler/docs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/docs/template/page.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.617457 Pyrosex-0.0.1/compiler/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.617457 Pyrosex-0.0.1/compiler/errors/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    22041 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.617457 Pyrosex-0.0.1/compiler/errors/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/template/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.621458 Pyrosex-0.0.1/pyrosex/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38779 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.621458 Pyrosex-0.0.1/pyrosex/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.621458 Pyrosex-0.0.1/pyrosex/connection/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/connection/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.621458 Pyrosex-0.0.1/pyrosex/connection/transport/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/connection/transport/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/connection/transport/tcp/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.621458 Pyrosex-0.0.1/pyrosex/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/crypto/mtproto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/crypto/prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/crypto/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   207202 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/emoji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.625458 Pyrosex-0.0.1/pyrosex/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/enums/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.625458 Pyrosex-0.0.1/pyrosex/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.625458 Pyrosex-0.0.1/pyrosex/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/callback_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/chat_join_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/deleted_messages_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/disconnect_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/edited_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/inline_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/poll_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/raw_update_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/handlers/user_status_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.625458 Pyrosex-0.0.1/pyrosex/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.625458 Pyrosex-0.0.1/pyrosex/methods/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/advanced/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/advanced/resolve_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/advanced/save_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.629458 Pyrosex-0.0.1/pyrosex/methods/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/check_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/get_password_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/resend_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/send_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/send_recovery_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/sign_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/sign_in_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/auth/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.629458 Pyrosex-0.0.1/pyrosex/methods/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/get_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/request_callback_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/set_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/bots/set_game_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.637458 Pyrosex-0.0.1/pyrosex/methods/chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/add_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/archive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/create_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/create_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/delete_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/delete_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/delete_user_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/get_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/get_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/join_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/set_administrator_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/set_chat_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/set_slow_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/unarchive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.637458 Pyrosex-0.0.1/pyrosex/methods/contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/contacts/add_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/contacts/delete_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/contacts/get_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/contacts/import_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.637458 Pyrosex-0.0.1/pyrosex/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/on_cb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/on_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/on_edited_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/on_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/on_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/on_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/on_raw_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/decorators/on_user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.641458 Pyrosex-0.0.1/pyrosex/methods/invite_links/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.649459 Pyrosex-0.0.1/pyrosex/methods/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/copy_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/delete_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/download_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/edit_inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/edit_inline_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/forward_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/get_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/get_discussion_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/get_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/inline_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/read_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/retract_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/search_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/search_global_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/search_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/search_messages_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_cached_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/stream_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/messages/vote_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.649459 Pyrosex-0.0.1/pyrosex/methods/password/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/password/change_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/password/enable_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.649459 Pyrosex-0.0.1/pyrosex/methods/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/users/block_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/users/delete_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/users/get_chat_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/users/get_common_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/users/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/users/set_profile_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/users/set_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/users/unblock_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/users/update_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.649459 Pyrosex-0.0.1/pyrosex/methods/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/utilities/add_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/utilities/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/utilities/export_session_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/utilities/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/utilities/remove_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/utilities/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/utilities/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/utilities/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/utilities/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/methods/utilities/stop_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60961 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/mime_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.653458 Pyrosex-0.0.1/pyrosex/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/parser/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/parser/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.653458 Pyrosex-0.0.1/pyrosex/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.653458 Pyrosex-0.0.1/pyrosex/raw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/future_salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/future_salts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/gzip_packed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/msg_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.653458 Pyrosex-0.0.1/pyrosex/raw/core/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/primitives/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/primitives/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/primitives/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/primitives/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/raw/core/tl_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.653458 Pyrosex-0.0.1/pyrosex/session/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/session/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.653458 Pyrosex-0.0.1/pyrosex/session/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/session/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/session/internals/data_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/session/internals/msg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/session/internals/msg_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/session/internals/seq_no.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.653458 Pyrosex-0.0.1/pyrosex/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/storage/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/storage/sqlite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.657459 Pyrosex-0.0.1/pyrosex/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.657459 Pyrosex-0.0.1/pyrosex/types/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/authorization/sent_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/authorization/terms_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.661459 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.661459 Pyrosex-0.0.1/pyrosex/types/inline_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.661459 Pyrosex-0.0.1/pyrosex/types/input_media/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/input_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/input_media/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/input_media/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/input_media/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/input_media/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/input_media/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/input_media/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.665459 Pyrosex-0.0.1/pyrosex/types/input_message_content/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/input_message_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/input_message_content/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.665459 Pyrosex-0.0.1/pyrosex/types/messages_and_media/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142440 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/messages_and_media/web_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.669459 Pyrosex-0.0.1/pyrosex/types/user_and_chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31615 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/pyrosex/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 09:08:29.669459 Pyrosex-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.669459 Pyrosex-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:08:29.669459 Pyrosex-0.0.1/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/tests/filters/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-07 09:08:17.000000 Pyrosex-0.0.1/tests/test_file_id.py
```

### Comparing `Pyrosex-0.0.0/COPYING` & `Pyrosex-0.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/COPYING.lesser` & `Pyrosex-0.0.1/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/NOTICE` & `Pyrosex-0.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/PKG-INFO` & `Pyrosex-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyrosex
-Version: 0.0.0
+Version: 0.0.1
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/OTHFamily
 Download-URL: https://github.com/OTHFamily/pyrosex/releases/latest
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3
 Project-URL: Tracker, https://github.com/OTHFamily/pyrosex/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Pyrosex Version: 0.0.0 Summary: Elegant, modern and
+Metadata-Version: 2.1 Name: Pyrosex Version: 0.0.1 Summary: Elegant, modern and
 asynchronous Telegram MTProto API framework in Python for users and bots Home-
 page: https://github.com/OTHFamily Download-URL: https://github.com/OTHFamily/
 pyrosex/releases/latest Author: OTH Author-email: oth@pyrosex.org License:
 LGPLv3 Project-URL: Tracker, https://github.com/OTHFamily/pyrosex/issues
 Project-URL: Community, https://t.me/OnTheHerd Project-URL: Source, https://
 github.com/OTHFamily/pyrosex Project-URL: Documentation, https://
 docs.pyrosex.org Keywords: telegram chat messenger mtproto api client library
```

### Comparing `Pyrosex-0.0.0/Pyrosex.egg-info/PKG-INFO` & `Pyrosex-0.0.1/Pyrosex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyrosex
-Version: 0.0.0
+Version: 0.0.1
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/OTHFamily
 Download-URL: https://github.com/OTHFamily/pyrosex/releases/latest
 Author: OTH
 Author-email: oth@pyrosex.org
 License: LGPLv3
 Project-URL: Tracker, https://github.com/OTHFamily/pyrosex/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Pyrosex Version: 0.0.0 Summary: Elegant, modern and
+Metadata-Version: 2.1 Name: Pyrosex Version: 0.0.1 Summary: Elegant, modern and
 asynchronous Telegram MTProto API framework in Python for users and bots Home-
 page: https://github.com/OTHFamily Download-URL: https://github.com/OTHFamily/
 pyrosex/releases/latest Author: OTH Author-email: oth@pyrosex.org License:
 LGPLv3 Project-URL: Tracker, https://github.com/OTHFamily/pyrosex/issues
 Project-URL: Community, https://t.me/OnTheHerd Project-URL: Source, https://
 github.com/OTHFamily/pyrosex Project-URL: Documentation, https://
 docs.pyrosex.org Keywords: telegram chat messenger mtproto api client library
```

### Comparing `Pyrosex-0.0.0/Pyrosex.egg-info/SOURCES.txt` & `Pyrosex-0.0.1/Pyrosex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/README.md` & `Pyrosex-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/api/compiler.py` & `Pyrosex-0.0.1/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/api/source/auth_key.tl` & `Pyrosex-0.0.1/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/api/source/main_api.tl` & `Pyrosex-0.0.1/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/api/source/sys_msgs.tl` & `Pyrosex-0.0.1/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/api/template/combinator.txt` & `Pyrosex-0.0.1/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/api/template/type.txt` & `Pyrosex-0.0.1/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/docs/compiler.py` & `Pyrosex-0.0.1/compiler/docs/compiler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/errors/compiler.py` & `Pyrosex-0.0.1/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/errors/source/400_BAD_REQUEST.tsv` & `Pyrosex-0.0.1/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/errors/source/401_UNAUTHORIZED.tsv` & `Pyrosex-0.0.1/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/errors/source/403_FORBIDDEN.tsv` & `Pyrosex-0.0.1/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `Pyrosex-0.0.1/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `Pyrosex-0.0.1/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/__init__.py` & `Pyrosex-0.0.1/pyrosex/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-__version__ = "0.0.0"
+__version__ = "0.0.1"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
-__copyright__ = "Copyright (C) 2017-present OTH <https://github.com/OTHFamily>"
+__copyright__ = "Copyright (C) 2023-present OTH <https://github.com/OTHFamily>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
     pass
```

### Comparing `Pyrosex-0.0.0/pyrosex/client.py` & `Pyrosex-0.0.1/pyrosex/client.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/connection/connection.py` & `Pyrosex-0.0.1/pyrosex/connection/connection.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/connection/transport/tcp/tcp.py` & `Pyrosex-0.0.1/pyrosex/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/connection/transport/tcp/tcp_abridged.py` & `Pyrosex-0.0.1/pyrosex/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/connection/transport/tcp/tcp_abridged_o.py` & `Pyrosex-0.0.1/pyrosex/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/connection/transport/tcp/tcp_full.py` & `Pyrosex-0.0.1/pyrosex/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/connection/transport/tcp/tcp_intermediate.py` & `Pyrosex-0.0.1/pyrosex/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/connection/transport/tcp/tcp_intermediate_o.py` & `Pyrosex-0.0.1/pyrosex/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/crypto/aes.py` & `Pyrosex-0.0.1/pyrosex/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/crypto/mtproto.py` & `Pyrosex-0.0.1/pyrosex/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/crypto/prime.py` & `Pyrosex-0.0.1/pyrosex/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/crypto/rsa.py` & `Pyrosex-0.0.1/pyrosex/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/dispatcher.py` & `Pyrosex-0.0.1/pyrosex/dispatcher.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/emoji.py` & `Pyrosex-0.0.1/pyrosex/emoji.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/enums/__init__.py` & `Pyrosex-0.0.1/pyrosex/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/enums/chat_action.py` & `Pyrosex-0.0.1/pyrosex/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/enums/chat_event_action.py` & `Pyrosex-0.0.1/pyrosex/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/enums/chat_members_filter.py` & `Pyrosex-0.0.1/pyrosex/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/enums/message_entity_type.py` & `Pyrosex-0.0.1/pyrosex/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/enums/message_media_type.py` & `Pyrosex-0.0.1/pyrosex/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/enums/message_service_type.py` & `Pyrosex-0.0.1/pyrosex/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/enums/messages_filter.py` & `Pyrosex-0.0.1/pyrosex/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/enums/next_code_type.py` & `Pyrosex-0.0.1/pyrosex/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/enums/sent_code_type.py` & `Pyrosex-0.0.1/pyrosex/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/errors/__init__.py` & `Pyrosex-0.0.1/pyrosex/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/errors/rpc_error.py` & `Pyrosex-0.0.1/pyrosex/errors/rpc_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from datetime import datetime
-from pyrosex import import_module
+from importlib import import_module
 from typing import Type, Union
 
 from pyrosex import raw
 from pyrosex.raw.core import TLObject
 from .exceptions.all import exceptions
```

### Comparing `Pyrosex-0.0.0/pyrosex/file_id.py` & `Pyrosex-0.0.1/pyrosex/file_id.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/filters.py` & `Pyrosex-0.0.1/pyrosex/filters.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/__init__.py` & `Pyrosex-0.0.1/pyrosex/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/callback_query_handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/chat_join_request_handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/chat_member_updated_handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/chosen_inline_result_handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/deleted_messages_handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/disconnect_handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/edited_message_handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/inline_query_handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/message_handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/poll_handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/raw_update_handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/handlers/user_status_handler.py` & `Pyrosex-0.0.1/pyrosex/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/advanced/invoke.py` & `Pyrosex-0.0.1/pyrosex/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/advanced/resolve_peer.py` & `Pyrosex-0.0.1/pyrosex/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/advanced/save_file.py` & `Pyrosex-0.0.1/pyrosex/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/__init__.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/accept_terms_of_service.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/check_password.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/connect.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/disconnect.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/initialize.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/log_out.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/recover_password.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/resend_code.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/send_code.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/send_recovery_code.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/sign_in.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/sign_in_bot.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/sign_up.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/auth/terminate.py` & `Pyrosex-0.0.1/pyrosex/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/__init__.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/answer_callback_query.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/answer_inline_query.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/answer_web_app_query.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/delete_bot_commands.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/get_bot_commands.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/get_bot_default_privileges.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/get_chat_menu_button.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/get_game_high_scores.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/get_inline_bot_results.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/request_callback_answer.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/send_game.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/send_inline_bot_result.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/set_bot_commands.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/set_bot_default_privileges.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/set_chat_menu_button.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/bots/set_game_score.py` & `Pyrosex-0.0.1/pyrosex/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/__init__.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/add_chat_members.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/archive_chats.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/ban_chat_member.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/create_channel.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/create_group.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/create_supergroup.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/delete_channel.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/delete_chat_photo.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/delete_supergroup.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/delete_user_history.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/get_chat.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/get_chat_event_log.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/get_chat_member.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/get_chat_members.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/get_chat_members_count.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/get_chat_online_count.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/get_dialogs.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/get_dialogs_count.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/get_nearby_chats.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/get_send_as_chats.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/join_chat.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/leave_chat.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/mark_chat_unread.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/pin_chat_message.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/promote_chat_member.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/restrict_chat_member.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/set_administrator_title.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/set_chat_description.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/set_chat_permissions.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/set_chat_photo.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/set_chat_protected_content.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/set_chat_title.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/set_chat_username.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/set_send_as_chat.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/set_slow_mode.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/unarchive_chats.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/unban_chat_member.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/unpin_all_chat_messages.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/chats/unpin_chat_message.py` & `Pyrosex-0.0.1/pyrosex/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/contacts/add_contact.py` & `Pyrosex-0.0.1/pyrosex/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/contacts/delete_contacts.py` & `Pyrosex-0.0.1/pyrosex/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/contacts/get_contacts.py` & `Pyrosex-0.0.1/pyrosex/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/contacts/get_contacts_count.py` & `Pyrosex-0.0.1/pyrosex/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/contacts/import_contacts.py` & `Pyrosex-0.0.1/pyrosex/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/__init__.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/on_cb.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/on_cb.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/on_chat_join_request.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/on_chat_member_updated.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/on_chosen_inline_result.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/on_deleted_messages.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/on_disconnect.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/on_edited_message.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/on_inline_query.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/on_msg.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/on_msg.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/on_poll.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/on_raw_update.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/decorators/on_user_status.py` & `Pyrosex-0.0.1/pyrosex/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/__init__.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/approve_all_chat_join_requests.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/approve_chat_join_request.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/create_chat_invite_link.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/decline_all_chat_join_requests.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/decline_chat_join_request.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/delete_chat_admin_invite_links.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/delete_chat_invite_link.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/edit_chat_invite_link.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/export_chat_invite_link.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_admin_invite_links.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_admin_invite_links_count.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_admins_with_invite_links.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_invite_link.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_invite_link_joiners.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_invite_link_joiners_count.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/get_chat_join_requests.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/invite_links/revoke_chat_invite_link.py` & `Pyrosex-0.0.1/pyrosex/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/__init__.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/copy_media_group.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/copy_message.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/delete_messages.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/download_media.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/edit_inline_caption.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/edit_inline_media.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/edit_inline_reply_markup.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/edit_inline_text.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/edit_message_caption.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/edit_message_media.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/edit_message_reply_markup.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/edit_message_text.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/forward_messages.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/get_chat_history.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/get_chat_history_count.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/get_discussion_message.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/get_discussion_replies.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/get_discussion_replies_count.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/get_media_group.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/get_messages.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/inline_session.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/read_chat_history.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/retract_vote.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/search_global.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/search_global_count.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/search_messages.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/search_messages_count.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_animation.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_audio.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_cached_media.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_chat_action.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_contact.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_dice.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_document.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_location.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_media_group.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_message.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_photo.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_poll.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_reaction.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_sticker.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_venue.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_video.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_video_note.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/send_voice.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/stop_poll.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/stream_media.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/messages/vote_poll.py` & `Pyrosex-0.0.1/pyrosex/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/password/change_cloud_password.py` & `Pyrosex-0.0.1/pyrosex/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/password/enable_cloud_password.py` & `Pyrosex-0.0.1/pyrosex/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/password/remove_cloud_password.py` & `Pyrosex-0.0.1/pyrosex/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/users/__init__.py` & `Pyrosex-0.0.1/pyrosex/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/users/block_user.py` & `Pyrosex-0.0.1/pyrosex/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/users/delete_profile_photos.py` & `Pyrosex-0.0.1/pyrosex/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/users/get_chat_photos.py` & `Pyrosex-0.0.1/pyrosex/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/users/get_chat_photos_count.py` & `Pyrosex-0.0.1/pyrosex/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/users/get_common_chats.py` & `Pyrosex-0.0.1/pyrosex/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/users/get_me.py` & `Pyrosex-0.0.1/pyrosex/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/users/get_users.py` & `Pyrosex-0.0.1/pyrosex/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/users/set_profile_photo.py` & `Pyrosex-0.0.1/pyrosex/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/users/set_username.py` & `Pyrosex-0.0.1/pyrosex/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/users/unblock_user.py` & `Pyrosex-0.0.1/pyrosex/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/users/update_profile.py` & `Pyrosex-0.0.1/pyrosex/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/utilities/add_handler.py` & `Pyrosex-0.0.1/pyrosex/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/utilities/compose.py` & `Pyrosex-0.0.1/pyrosex/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/utilities/export_session_string.py` & `Pyrosex-0.0.1/pyrosex/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/utilities/idle.py` & `Pyrosex-0.0.1/pyrosex/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/utilities/remove_handler.py` & `Pyrosex-0.0.1/pyrosex/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/utilities/restart.py` & `Pyrosex-0.0.1/pyrosex/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/utilities/run.py` & `Pyrosex-0.0.1/pyrosex/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/utilities/start.py` & `Pyrosex-0.0.1/pyrosex/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/utilities/stop.py` & `Pyrosex-0.0.1/pyrosex/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/methods/utilities/stop_transmission.py` & `Pyrosex-0.0.1/pyrosex/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/mime_types.py` & `Pyrosex-0.0.1/pyrosex/mime_types.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/parser/html.py` & `Pyrosex-0.0.1/pyrosex/parser/html.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/parser/markdown.py` & `Pyrosex-0.0.1/pyrosex/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/parser/parser.py` & `Pyrosex-0.0.1/pyrosex/parser/parser.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/parser/utils.py` & `Pyrosex-0.0.1/pyrosex/parser/utils.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/raw/core/future_salt.py` & `Pyrosex-0.0.1/pyrosex/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/raw/core/future_salts.py` & `Pyrosex-0.0.1/pyrosex/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/raw/core/gzip_packed.py` & `Pyrosex-0.0.1/pyrosex/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/raw/core/message.py` & `Pyrosex-0.0.1/pyrosex/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/raw/core/msg_container.py` & `Pyrosex-0.0.1/pyrosex/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/raw/core/primitives/bool.py` & `Pyrosex-0.0.1/pyrosex/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/raw/core/primitives/bytes.py` & `Pyrosex-0.0.1/pyrosex/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/raw/core/primitives/int.py` & `Pyrosex-0.0.1/pyrosex/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/raw/core/primitives/vector.py` & `Pyrosex-0.0.1/pyrosex/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/raw/core/tl_object.py` & `Pyrosex-0.0.1/pyrosex/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/session/auth.py` & `Pyrosex-0.0.1/pyrosex/session/auth.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/session/internals/data_center.py` & `Pyrosex-0.0.1/pyrosex/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/session/internals/msg_factory.py` & `Pyrosex-0.0.1/pyrosex/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/session/internals/msg_id.py` & `Pyrosex-0.0.1/pyrosex/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/session/session.py` & `Pyrosex-0.0.1/pyrosex/session/session.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/storage/file_storage.py` & `Pyrosex-0.0.1/pyrosex/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/storage/memory_storage.py` & `Pyrosex-0.0.1/pyrosex/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/storage/sqlite_storage.py` & `Pyrosex-0.0.1/pyrosex/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/storage/storage.py` & `Pyrosex-0.0.1/pyrosex/storage/storage.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/sync.py` & `Pyrosex-0.0.1/pyrosex/sync.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/authorization/sent_code.py` & `Pyrosex-0.0.1/pyrosex/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/authorization/terms_of_service.py` & `Pyrosex-0.0.1/pyrosex/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/__init__.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command_scope.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command_scope_chat.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/callback_query.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/force_reply.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/game_high_score.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/inline_keyboard_button.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/inline_keyboard_markup.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/keyboard_button.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/login_url.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/menu_button.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/menu_button_web_app.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/reply_keyboard_markup.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/reply_keyboard_remove.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/bots_and_keyboards/sent_web_app_message.py` & `Pyrosex-0.0.1/pyrosex/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/__init__.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/chosen_inline_result.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_animation.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_article.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_audio.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_animation.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_audio.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_document.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_photo.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_sticker.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_video.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_cached_voice.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_contact.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_document.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_location.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_photo.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_venue.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_video.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/inline_mode/inline_query_result_voice.py` & `Pyrosex-0.0.1/pyrosex/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/input_media/input_media.py` & `Pyrosex-0.0.1/pyrosex/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/input_media/input_media_animation.py` & `Pyrosex-0.0.1/pyrosex/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/input_media/input_media_audio.py` & `Pyrosex-0.0.1/pyrosex/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/input_media/input_media_document.py` & `Pyrosex-0.0.1/pyrosex/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/input_media/input_media_photo.py` & `Pyrosex-0.0.1/pyrosex/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/input_media/input_media_video.py` & `Pyrosex-0.0.1/pyrosex/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/input_media/input_phone_contact.py` & `Pyrosex-0.0.1/pyrosex/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/input_message_content/input_message_content.py` & `Pyrosex-0.0.1/pyrosex/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/input_message_content/input_text_message_content.py` & `Pyrosex-0.0.1/pyrosex/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/__init__.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/animation.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/audio.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/contact.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/dice.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/document.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/game.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/location.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/message.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/message_entity.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/photo.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/poll.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/poll_option.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/reaction.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/sticker.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/stripped_thumbnail.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/thumbnail.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/venue.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/video.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/video_note.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/voice.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/web_app_data.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/messages_and_media/web_page.py` & `Pyrosex-0.0.1/pyrosex/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/object.py` & `Pyrosex-0.0.1/pyrosex/types/object.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/__init__.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_admin_with_invite_links.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_event.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_event_filter.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_invite_link.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_join_request.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_joiner.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_member.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_member_updated.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_permissions.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_photo.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_preview.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/chat_privileges.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/dialog.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/invite_link_importer.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/restriction.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/user.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/video_chat_ended.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/video_chat_members_invited.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/types/user_and_chats/video_chat_scheduled.py` & `Pyrosex-0.0.1/pyrosex/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/pyrosex/utils.py` & `Pyrosex-0.0.1/pyrosex/utils.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/setup.py` & `Pyrosex-0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/tests/filters/test_command.py` & `Pyrosex-0.0.1/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `Pyrosex-0.0.0/tests/test_file_id.py` & `Pyrosex-0.0.1/tests/test_file_id.py`

 * *Files identical despite different names*

