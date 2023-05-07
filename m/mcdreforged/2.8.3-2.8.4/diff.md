# Comparing `tmp/mcdreforged-2.8.3.tar.gz` & `tmp/mcdreforged-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcdreforged-2.8.3.tar", last modified: Mon Apr  3 19:50:28 2023, max compression
+gzip compressed data, was "mcdreforged-2.8.4.tar", last modified: Sun May  7 13:59:31 2023, max compression
```

## Comparing `mcdreforged-2.8.3.tar` & `mcdreforged-2.8.4.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.052959 mcdreforged-2.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-03 19:50:28.052959 mcdreforged-2.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.036959 mcdreforged-2.8.3/mcdreforged/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.036959 mcdreforged-2.8.3/mcdreforged/api/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.036959 mcdreforged-2.8.3/mcdreforged/api/all/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/all/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.036959 mcdreforged-2.8.3/mcdreforged/api/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.036959 mcdreforged-2.8.3/mcdreforged/api/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/decorator/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/decorator/new_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/decorator/spam_proof.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.036959 mcdreforged-2.8.3/mcdreforged/api/event/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/event/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.040959 mcdreforged-2.8.3/mcdreforged/api/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.040959 mcdreforged-2.8.3/mcdreforged/api/rcon/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/rcon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.040959 mcdreforged-2.8.3/mcdreforged/api/rtext/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/rtext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.040959 mcdreforged-2.8.3/mcdreforged/api/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.040959 mcdreforged-2.8.3/mcdreforged/api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/api/utils/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.040959 mcdreforged-2.8.3/mcdreforged/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/cli/cli_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/cli/cmd_gendefault.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/cli/cmd_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/cli/cmd_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/cli/cmd_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.040959 mcdreforged-2.8.3/mcdreforged/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.040959 mcdreforged-2.8.3/mcdreforged/command/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/command/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/command/builder/command_builder_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/command/builder/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/command/builder/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.040959 mcdreforged-2.8.3/mcdreforged/command/builder/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/command/builder/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/command/builder/nodes/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    22553 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/command/builder/nodes/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12833 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/command/builder/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/command/command_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/command/command_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.040959 mcdreforged-2.8.3/mcdreforged/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/constants/core_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/constants/plugin_constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.040959 mcdreforged-2.8.3/mcdreforged/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/executor/console_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/executor/task_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/executor/thread_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/executor/update_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/executor/watchdog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.040959 mcdreforged-2.8.3/mcdreforged/handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8295 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/abstract_server_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.044959 mcdreforged-2.8.3/mcdreforged/handler/impl/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/impl/abstract_minecraft_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/impl/basic_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/impl/beta18_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/impl/bukkit14_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/impl/bukkit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/impl/bungeecord_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/impl/cat_server_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/impl/forge_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/impl/vanilla_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/impl/velocity_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/impl/waterfall_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/handler/server_handler_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.044959 mcdreforged-2.8.3/mcdreforged/info_reactor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/info_reactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/info_reactor/abstract_info_reactor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.044959 mcdreforged-2.8.3/mcdreforged/info_reactor/impl/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/info_reactor/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/info_reactor/impl/general_reactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/info_reactor/impl/player_reactor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2029 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/info_reactor/impl/server_reactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/info_reactor/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/info_reactor/info_reactor_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/info_reactor/server_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/mcdr_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24141 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/mcdr_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/mcdr_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.044959 mcdreforged-2.8.3/mcdreforged/minecraft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/minecraft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.044959 mcdreforged-2.8.3/mcdreforged/minecraft/rcon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/minecraft/rcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/minecraft/rcon/rcon_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/minecraft/rcon/rcon_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.044959 mcdreforged-2.8.3/mcdreforged/minecraft/rtext/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/minecraft/rtext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/minecraft/rtext/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/minecraft/rtext/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.044959 mcdreforged-2.8.3/mcdreforged/permission/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/permission/permission_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/permission/permission_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.044959 mcdreforged-2.8.3/mcdreforged/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.044959 mcdreforged-2.8.3/mcdreforged/plugin/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.048959 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.048959 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/check_update_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/debug_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/help_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/permission_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/plugin_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/preference_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/reload_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/status_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/sub_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/mcdreforged_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/builtin/python_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.048959 mcdreforged-2.8.3/mcdreforged/plugin/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/meta/dependency_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/meta/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/meta/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/operation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/plugin_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/plugin_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    24770 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/plugin_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    42338 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/server_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.048959 mcdreforged-2.8.3/mcdreforged/plugin/type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/type/directory_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/type/multi_file_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/type/packed_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/type/permanent_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/type/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/type/regular_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/plugin/type/solo_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.048959 mcdreforged-2.8.3/mcdreforged/preference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/preference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/preference/preference_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.048959 mcdreforged-2.8.3/mcdreforged/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/resources/default_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/resources/default_permission.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.048959 mcdreforged-2.8.3/mcdreforged/resources/lang/
--rw-r--r--   0 runner    (1001) docker     (123)    14289 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/resources/lang/en_us.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/resources/lang/zh_cn.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.048959 mcdreforged-2.8.3/mcdreforged/translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/translation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/translation/translation_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/translation/translation_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.052959 mcdreforged-2.8.3/mcdreforged/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/class_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/future.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/lazy_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/misc_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/resources_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/string_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/thread_local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/translation_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/tree_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/mcdreforged/utils/yaml_data_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:50:28.036959 mcdreforged-2.8.3/mcdreforged.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-03 19:50:28.000000 mcdreforged-2.8.3/mcdreforged.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-03 19:50:28.000000 mcdreforged-2.8.3/mcdreforged.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 19:50:28.000000 mcdreforged-2.8.3/mcdreforged.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-03 19:50:28.000000 mcdreforged-2.8.3/mcdreforged.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 19:50:28.000000 mcdreforged-2.8.3/mcdreforged.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 19:50:28.052959 mcdreforged-2.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-03 19:50:23.000000 mcdreforged-2.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.014186 mcdreforged-2.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-07 13:59:31.014186 mcdreforged-2.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:30.998186 mcdreforged-2.8.4/mcdreforged/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:30.998186 mcdreforged-2.8.4/mcdreforged/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/all/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/all/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/decorator/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/decorator/new_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/decorator/spam_proof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/event/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/event/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/rcon/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/rcon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/rtext/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/rtext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/api/utils/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/cli_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/cmd_gendefault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/cmd_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/cmd_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/cli/cmd_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/command/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/command_builder_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/command/builder/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/nodes/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22553 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/nodes/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12833 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/builder/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/command_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/command/command_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/constants/core_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/constants/plugin_constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.002186 mcdreforged-2.8.4/mcdreforged/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/executor/console_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/executor/task_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/executor/thread_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/executor/update_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/executor/watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8295 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/abstract_server_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/handler/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/abstract_minecraft_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/basic_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/beta18_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/bukkit14_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/bukkit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/bungeecord_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/cat_server_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/forge_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/vanilla_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/velocity_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/impl/waterfall_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/handler/server_handler_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/info_reactor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/abstract_info_reactor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/info_reactor/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/impl/general_reactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/impl/player_reactor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2029 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/impl/server_reactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/info_reactor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/info_reactor/server_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/mcdr_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24141 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/mcdr_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/mcdr_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/minecraft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/minecraft/rcon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/rcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/rcon/rcon_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/rcon/rcon_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/minecraft/rtext/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/rtext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/rtext/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/minecraft/rtext/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/permission/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/permission/permission_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/permission/permission_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.006186 mcdreforged-2.8.4/mcdreforged/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/plugin/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/check_update_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/debug_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/help_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/permission_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/plugin_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/preference_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/reload_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/status_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/sub_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/mcdreforged_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/builtin/python_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/plugin/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/meta/dependency_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/meta/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/meta/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/operation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/plugin_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/plugin_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24770 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/plugin_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42338 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/server_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/plugin/type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/directory_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/multi_file_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/packed_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/permanent_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/regular_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/plugin/type/solo_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/preference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/preference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/preference/preference_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/resources/default_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/resources/default_permission.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/resources/lang/
+-rw-r--r--   0 runner    (1001) docker     (123)    14289 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/resources/lang/en_us.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/resources/lang/zh_cn.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.010187 mcdreforged-2.8.4/mcdreforged/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/translation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/translation/translation_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/translation/translation_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:31.014186 mcdreforged-2.8.4/mcdreforged/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/class_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/lazy_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/misc_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/resources_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/thread_local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/translation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/tree_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/mcdreforged/utils/yaml_data_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:30.998186 mcdreforged-2.8.4/mcdreforged.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-07 13:59:30.000000 mcdreforged-2.8.4/mcdreforged.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-07 13:59:30.000000 mcdreforged-2.8.4/mcdreforged.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 13:59:30.000000 mcdreforged-2.8.4/mcdreforged.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-07 13:59:30.000000 mcdreforged-2.8.4/mcdreforged.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 13:59:30.000000 mcdreforged-2.8.4/mcdreforged.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 13:59:31.014186 mcdreforged-2.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-07 13:59:23.000000 mcdreforged-2.8.4/setup.py
```

### Comparing `mcdreforged-2.8.3/LICENSE` & `mcdreforged-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/PKG-INFO` & `mcdreforged-2.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcdreforged
-Version: 2.8.3
+Version: 2.8.4
 Summary: A rewritten version of MCDaemon, a python script to control your Minecraft server
 Home-page: https://github.com/Fallen-Breath/MCDReforged
 Author: Fallen_Breath
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `mcdreforged-2.8.3/README.md` & `mcdreforged-2.8.4/README.md`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/api/all/__init__.py` & `mcdreforged-2.8.4/mcdreforged/api/all/__init__.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/api/command/__init__.py` & `mcdreforged-2.8.4/mcdreforged/api/command/__init__.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/api/decorator/event_listener.py` & `mcdreforged-2.8.4/mcdreforged/api/decorator/event_listener.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/api/decorator/new_thread.py` & `mcdreforged-2.8.4/mcdreforged/api/decorator/new_thread.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/api/decorator/spam_proof.py` & `mcdreforged-2.8.4/mcdreforged/api/decorator/spam_proof.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/api/types/__init__.py` & `mcdreforged-2.8.4/mcdreforged/api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/cli/cli_entry.py` & `mcdreforged-2.8.4/mcdreforged/cli/cli_entry.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/cli/cmd_pack.py` & `mcdreforged-2.8.4/mcdreforged/cli/cmd_pack.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/cli/cmd_run.py` & `mcdreforged-2.8.4/mcdreforged/cli/cmd_run.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/command/builder/command_builder_util.py` & `mcdreforged-2.8.4/mcdreforged/command/builder/command_builder_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/command/builder/common.py` & `mcdreforged-2.8.4/mcdreforged/command/builder/common.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/command/builder/exception.py` & `mcdreforged-2.8.4/mcdreforged/command/builder/exception.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/command/builder/nodes/arguments.py` & `mcdreforged-2.8.4/mcdreforged/command/builder/nodes/arguments.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/command/builder/nodes/basic.py` & `mcdreforged-2.8.4/mcdreforged/command/builder/nodes/basic.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/command/builder/tools.py` & `mcdreforged-2.8.4/mcdreforged/command/builder/tools.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/command/command_manager.py` & `mcdreforged-2.8.4/mcdreforged/command/command_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/command/command_source.py` & `mcdreforged-2.8.4/mcdreforged/command/command_source.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/constants/core_constant.py` & `mcdreforged-2.8.4/mcdreforged/constants/core_constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 NAME_SHORT = 'MCDR'
 NAME = 'MCDReforged'
 PACKAGE_NAME = 'mcdreforged'
 
 # MCDR Version Storage
 # Related: docs/source/conf.py
-VERSION = '2.8.3'       # semver (1.2.3-alpha.4)
-VERSION_PYPI = '2.8.3'  # pythonic ver (1.2.3a4)
+VERSION = '2.8.4'       # semver (1.2.3-alpha.4)
+VERSION_PYPI = '2.8.4'  # pythonic ver (1.2.3a4)
 
 GITHUB_URL = 'https://github.com/Fallen-Breath/MCDReforged'
 GITHUB_API_LATEST = 'https://api.github.com/repos/Fallen-Breath/MCDReforged/releases/latest'
 DOCUMENTATION_URL = 'https://mcdreforged.readthedocs.io/'
 
 PACKAGE_PATH = os.path.realpath(os.path.join(os.path.dirname(__file__), '..'))
 LOGGING_FILE = os.path.join('logs', '{}.log'.format(NAME_SHORT))
```

### Comparing `mcdreforged-2.8.3/mcdreforged/constants/plugin_constant.py` & `mcdreforged-2.8.4/mcdreforged/constants/plugin_constant.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/executor/console_handler.py` & `mcdreforged-2.8.4/mcdreforged/executor/console_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/executor/task_executor.py` & `mcdreforged-2.8.4/mcdreforged/executor/task_executor.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/executor/thread_executor.py` & `mcdreforged-2.8.4/mcdreforged/executor/thread_executor.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/executor/update_helper.py` & `mcdreforged-2.8.4/mcdreforged/executor/update_helper.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/executor/watchdog.py` & `mcdreforged-2.8.4/mcdreforged/executor/watchdog.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/abstract_server_handler.py` & `mcdreforged-2.8.4/mcdreforged/handler/abstract_server_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/impl/__init__.py` & `mcdreforged-2.8.4/mcdreforged/handler/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/impl/abstract_minecraft_handler.py` & `mcdreforged-2.8.4/mcdreforged/handler/impl/abstract_minecraft_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/impl/basic_handler.py` & `mcdreforged-2.8.4/mcdreforged/handler/impl/basic_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/impl/beta18_handler.py` & `mcdreforged-2.8.4/mcdreforged/handler/impl/beta18_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/impl/bukkit14_handler.py` & `mcdreforged-2.8.4/mcdreforged/handler/impl/bukkit14_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/impl/bukkit_handler.py` & `mcdreforged-2.8.4/mcdreforged/handler/impl/bukkit_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/impl/bungeecord_handler.py` & `mcdreforged-2.8.4/mcdreforged/handler/impl/bungeecord_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/impl/cat_server_handler.py` & `mcdreforged-2.8.4/mcdreforged/handler/impl/cat_server_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/impl/forge_handler.py` & `mcdreforged-2.8.4/mcdreforged/handler/impl/forge_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/impl/velocity_handler.py` & `mcdreforged-2.8.4/mcdreforged/handler/impl/velocity_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/impl/waterfall_handler.py` & `mcdreforged-2.8.4/mcdreforged/handler/impl/waterfall_handler.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/handler/server_handler_manager.py` & `mcdreforged-2.8.4/mcdreforged/handler/server_handler_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/info_reactor/abstract_info_reactor.py` & `mcdreforged-2.8.4/mcdreforged/info_reactor/abstract_info_reactor.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/info_reactor/impl/general_reactor.py` & `mcdreforged-2.8.4/mcdreforged/info_reactor/impl/general_reactor.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/info_reactor/impl/player_reactor.py` & `mcdreforged-2.8.4/mcdreforged/info_reactor/impl/player_reactor.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/info_reactor/impl/server_reactor.py` & `mcdreforged-2.8.4/mcdreforged/info_reactor/impl/server_reactor.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/info_reactor/info.py` & `mcdreforged-2.8.4/mcdreforged/info_reactor/info.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/info_reactor/info_reactor_manager.py` & `mcdreforged-2.8.4/mcdreforged/info_reactor/info_reactor_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/info_reactor/server_information.py` & `mcdreforged-2.8.4/mcdreforged/info_reactor/server_information.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/mcdr_config.py` & `mcdreforged-2.8.4/mcdreforged/mcdr_config.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/mcdr_server.py` & `mcdreforged-2.8.4/mcdreforged/mcdr_server.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/mcdr_state.py` & `mcdreforged-2.8.4/mcdreforged/mcdr_state.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/minecraft/rcon/rcon_connection.py` & `mcdreforged-2.8.4/mcdreforged/minecraft/rcon/rcon_connection.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/minecraft/rcon/rcon_manager.py` & `mcdreforged-2.8.4/mcdreforged/minecraft/rcon/rcon_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/minecraft/rtext/style.py` & `mcdreforged-2.8.4/mcdreforged/minecraft/rtext/style.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/minecraft/rtext/text.py` & `mcdreforged-2.8.4/mcdreforged/minecraft/rtext/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 			text.set_styles(styles)
 			if 'color' in data:
 				try:
 					text.set_color(RColor.from_mc_value(data['color']))
 				except ValueError:
 					pass
 			try:
-				click_event = ['clickEvent']
+				click_event = data['clickEvent']
 				if isinstance(click_event, dict):
 					text.set_click_event(RAction[click_event['action']], click_event['value'])
 			except KeyError:
 				pass
 			try:
 				hover_event = data['hoverEvent']
 				if isinstance(hover_event, dict) and hover_event['action'] == 'show_text':
```

### Comparing `mcdreforged-2.8.3/mcdreforged/permission/permission_level.py` & `mcdreforged-2.8.4/mcdreforged/permission/permission_level.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/permission/permission_manager.py` & `mcdreforged-2.8.4/mcdreforged/permission/permission_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/debug_command.py` & `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/debug_command.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/help_command.py` & `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/permission_command.py` & `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/permission_command.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/plugin_command.py` & `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/plugin_command.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/preference_command.py` & `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/preference_command.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/reload_command.py` & `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/reload_command.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/status_command.py` & `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/status_command.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/sub_command.py` & `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/commands/sub_command.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/builtin/mcdreforged_plugin/mcdreforged_plugin.py` & `mcdreforged-2.8.4/mcdreforged/plugin/builtin/mcdreforged_plugin/mcdreforged_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/builtin/python_plugin.py` & `mcdreforged-2.8.4/mcdreforged/plugin/builtin/python_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/meta/dependency_walker.py` & `mcdreforged-2.8.4/mcdreforged/plugin/meta/dependency_walker.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/meta/metadata.py` & `mcdreforged-2.8.4/mcdreforged/plugin/meta/metadata.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/meta/version.py` & `mcdreforged-2.8.4/mcdreforged/plugin/meta/version.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/operation_result.py` & `mcdreforged-2.8.4/mcdreforged/plugin/operation_result.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/plugin_event.py` & `mcdreforged-2.8.4/mcdreforged/plugin/plugin_event.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/plugin_factory.py` & `mcdreforged-2.8.4/mcdreforged/plugin/plugin_factory.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/plugin_manager.py` & `mcdreforged-2.8.4/mcdreforged/plugin/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/plugin_registry.py` & `mcdreforged-2.8.4/mcdreforged/plugin/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/plugin_thread.py` & `mcdreforged-2.8.4/mcdreforged/plugin/plugin_thread.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/server_interface.py` & `mcdreforged-2.8.4/mcdreforged/plugin/server_interface.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/type/directory_plugin.py` & `mcdreforged-2.8.4/mcdreforged/plugin/type/directory_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/type/multi_file_plugin.py` & `mcdreforged-2.8.4/mcdreforged/plugin/type/multi_file_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/type/packed_plugin.py` & `mcdreforged-2.8.4/mcdreforged/plugin/type/packed_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/type/permanent_plugin.py` & `mcdreforged-2.8.4/mcdreforged/plugin/type/permanent_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/type/plugin.py` & `mcdreforged-2.8.4/mcdreforged/plugin/type/plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/type/regular_plugin.py` & `mcdreforged-2.8.4/mcdreforged/plugin/type/regular_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/plugin/type/solo_plugin.py` & `mcdreforged-2.8.4/mcdreforged/plugin/type/solo_plugin.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/preference/preference_manager.py` & `mcdreforged-2.8.4/mcdreforged/preference/preference_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/resources/default_config.yml` & `mcdreforged-2.8.4/mcdreforged/resources/default_config.yml`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/resources/lang/en_us.yml` & `mcdreforged-2.8.4/mcdreforged/resources/lang/en_us.yml`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/resources/lang/zh_cn.yml` & `mcdreforged-2.8.4/mcdreforged/resources/lang/zh_cn.yml`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/translation/translation_manager.py` & `mcdreforged-2.8.4/mcdreforged/translation/translation_manager.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/translation/translation_text.py` & `mcdreforged-2.8.4/mcdreforged/translation/translation_text.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/utils/class_util.py` & `mcdreforged-2.8.4/mcdreforged/utils/class_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/utils/file_util.py` & `mcdreforged-2.8.4/mcdreforged/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/utils/future.py` & `mcdreforged-2.8.4/mcdreforged/utils/future.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/utils/logger.py` & `mcdreforged-2.8.4/mcdreforged/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/utils/misc_util.py` & `mcdreforged-2.8.4/mcdreforged/utils/misc_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/utils/resources_util.py` & `mcdreforged-2.8.4/mcdreforged/utils/resources_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/utils/serializer.py` & `mcdreforged-2.8.4/mcdreforged/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/utils/string_util.py` & `mcdreforged-2.8.4/mcdreforged/utils/string_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/utils/thread_local_storage.py` & `mcdreforged-2.8.4/mcdreforged/utils/thread_local_storage.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/utils/translation_util.py` & `mcdreforged-2.8.4/mcdreforged/utils/translation_util.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/utils/tree_printer.py` & `mcdreforged-2.8.4/mcdreforged/utils/tree_printer.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged/utils/yaml_data_storage.py` & `mcdreforged-2.8.4/mcdreforged/utils/yaml_data_storage.py`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/mcdreforged.egg-info/PKG-INFO` & `mcdreforged-2.8.4/mcdreforged.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcdreforged
-Version: 2.8.3
+Version: 2.8.4
 Summary: A rewritten version of MCDaemon, a python script to control your Minecraft server
 Home-page: https://github.com/Fallen-Breath/MCDReforged
 Author: Fallen_Breath
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `mcdreforged-2.8.3/mcdreforged.egg-info/SOURCES.txt` & `mcdreforged-2.8.4/mcdreforged.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcdreforged-2.8.3/setup.py` & `mcdreforged-2.8.4/setup.py`

 * *Files identical despite different names*

