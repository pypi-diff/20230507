# Comparing `tmp/nonebot_plugin_mahjong_scoreboard-0.3.0a1.tar.gz` & `tmp/nonebot_plugin_mahjong_scoreboard-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mahjong_scoreboard-0.3.0a1.tar", max compression
+gzip compressed data, was "nonebot_plugin_mahjong_scoreboard-0.3.1.tar", max compression
```

## Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1.tar` & `nonebot_plugin_mahjong_scoreboard-0.3.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421764 nonebot_plugin_mahjong_scoreboard-0.3.0a1/LICENSE
--rw-r--r--   0        0        0      934 2023-03-16 06:42:36.537929 nonebot_plugin_mahjong_scoreboard-0.3.0a1/pyproject.toml
--rw-r--r--   0        0        0     5497 2023-03-13 11:15:04.242648 nonebot_plugin_mahjong_scoreboard-0.3.0a1/README.MD
--rw-r--r--   0        0        0     2090 2023-03-13 11:15:04.245273 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/__init__.py
--rw-r--r--   0        0        0      347 2023-03-13 11:15:04.245799 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/config.py
--rw-r--r--   0        0        0      287 2023-03-13 11:15:04.246316 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/__init__.py
--rw-r--r--   0        0        0      489 2022-10-29 10:31:10.715954 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/context.py
--rw-r--r--   0        0        0     3647 2023-03-01 06:19:33.483226 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py
--rw-r--r--   0        0        0     7291 2023-03-13 11:15:04.246837 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py
--rw-r--r--   0        0        0    14581 2023-03-13 11:15:04.247882 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py
--rw-r--r--   0        0        0     6060 2023-03-13 11:15:04.248921 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py
--rw-r--r--   0        0        0     7254 2023-03-13 11:15:04.249448 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/general_handlers.py
--rw-r--r--   0        0        0      439 2022-10-29 12:00:29.945522 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py
--rw-r--r--   0        0        0     1160 2023-03-01 06:35:10.159635 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_error_impl.py
--rw-r--r--   0        0        0      519 2022-10-25 08:26:38.853725 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_interruption_impl.py
--rw-r--r--   0        0        0     1393 2023-03-13 11:15:04.249954 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py
--rw-r--r--   0        0        0     2770 2023-03-13 11:15:04.250961 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py
--rw-r--r--   0        0        0     3722 2023-03-13 11:15:04.251961 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py
--rw-r--r--   0        0        0     2423 2023-03-13 11:15:04.252961 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_statistics_mapper.py
--rw-r--r--   0        0        0     2494 2023-03-13 11:15:04.252961 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py
--rw-r--r--   0        0        0     3086 2023-03-01 06:19:33.488463 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py
--rw-r--r--   0        0        0     3027 2023-03-13 11:15:04.253961 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py
--rw-r--r--   0        0        0    13761 2023-03-13 11:15:04.254961 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py
--rw-r--r--   0        0        0     2811 2023-03-13 11:15:04.255960 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py
--rw-r--r--   0        0        0     2807 2023-03-01 06:19:33.490557 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py
--rw-r--r--   0        0        0     5276 2023-03-13 11:15:04.256731 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py
--rw-r--r--   0        0        0     3427 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py
--rw-r--r--   0        0        0        0 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/__init__.py
--rw-r--r--   0        0        0     1022 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py
--rw-r--r--   0        0        0     2519 2023-03-13 11:15:04.258743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py
--rw-r--r--   0        0        0     1708 2023-03-13 11:15:04.258743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/send_messages.py
--rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228228 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/errors.py
--rw-r--r--   0        0        0        0 2022-10-11 14:30:16.137278 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py
--rw-r--r--   0        0        0      492 2022-10-25 11:55:32.743202 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/enums.py
--rw-r--r--   0        0        0       39 2023-03-13 11:15:04.259743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/__init__.py
--rw-r--r--   0        0        0      129 2023-03-13 11:15:04.259743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/__init__.py
--rw-r--r--   0        0        0     2014 2023-03-13 13:49:53.073496 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/metainfo.py
--rw-r--r--   0        0        0      653 2023-03-13 11:15:04.261743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/__init__.py
--rw-r--r--   0        0        0      255 2023-03-13 11:15:04.261743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/v1_to_v2.py
--rw-r--r--   0        0        0      584 2023-03-13 11:15:04.262742 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/src.py
--rw-r--r--   0        0        0     3840 2023-03-13 11:15:04.263743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/game.py
--rw-r--r--   0        0        0      876 2023-03-13 11:15:04.263743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/group.py
--rw-r--r--   0        0        0     3819 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/season.py
--rw-r--r--   0        0        0        0 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/__init__.py
--rw-r--r--   0        0        0      522 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/userdict.py
--rw-r--r--   0        0        0      461 2023-03-13 11:15:04.265743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/user.py
--rw-r--r--   0        0        0        0 2022-10-11 14:02:12.038461 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/service/__init__.py
--rw-r--r--   0        0        0    17932 2023-03-13 13:33:43.452268 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py
--rw-r--r--   0        0        0     2196 2023-03-13 11:15:04.266743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py
--rw-r--r--   0        0        0     3736 2023-03-01 06:19:33.494591 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py
--rw-r--r--   0        0        0    10068 2023-03-13 13:34:40.919314 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py
--rw-r--r--   0        0        0      582 2023-03-01 06:19:33.495592 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py
--rw-r--r--   0        0        0        0 2022-10-25 10:53:45.022120 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/__init__.py
--rw-r--r--   0        0        0      288 2022-10-25 10:55:21.893872 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/date.py
--rw-r--r--   0        0        0     1240 2022-10-25 10:57:00.084086 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py
--rw-r--r--   0        0        0      101 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/nonebot.py
--rw-r--r--   0        0        0      482 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/rank.py
--rw-r--r--   0        0        0      256 2023-02-24 10:26:11.257181 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/upload_file.py
--rw-r--r--   0        0        0      761 2023-03-13 11:15:04.268743 nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py
--rw-r--r--   0        0        0     7161 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.3.0a1/setup.py
--rw-r--r--   0        0        0     6425 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.3.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421764 nonebot_plugin_mahjong_scoreboard-0.3.1/LICENSE
+-rw-r--r--   0        0        0      932 2023-05-07 02:57:41.868310 nonebot_plugin_mahjong_scoreboard-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6759 2023-05-07 02:56:55.737523 nonebot_plugin_mahjong_scoreboard-0.3.1/README.MD
+-rw-r--r--   0        0        0     2090 2023-04-04 02:00:50.079979 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/__init__.py
+-rw-r--r--   0        0        0      347 2023-03-13 11:15:04.245799 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/config.py
+-rw-r--r--   0        0        0      287 2023-03-13 11:15:04.246316 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/__init__.py
+-rw-r--r--   0        0        0      489 2022-10-29 10:31:10.715954 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/context.py
+-rw-r--r--   0        0        0     3647 2023-03-01 06:19:33.483226 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py
+-rw-r--r--   0        0        0     7291 2023-03-13 11:15:04.246837 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py
+-rw-r--r--   0        0        0    14581 2023-03-13 11:15:04.247882 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py
+-rw-r--r--   0        0        0     5417 2023-05-07 02:50:32.445789 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py
+-rw-r--r--   0        0        0     7254 2023-03-13 11:15:04.249448 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/general_handlers.py
+-rw-r--r--   0        0        0      439 2022-10-29 12:00:29.945522 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py
+-rw-r--r--   0        0        0     1160 2023-03-01 06:35:10.159635 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_error_impl.py
+-rw-r--r--   0        0        0      519 2022-10-25 08:26:38.853725 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_interruption_impl.py
+-rw-r--r--   0        0        0     1437 2023-05-07 03:16:58.471265 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py
+-rw-r--r--   0        0        0     2770 2023-03-13 11:15:04.250961 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py
+-rw-r--r--   0        0        0     3722 2023-03-13 11:15:04.251961 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py
+-rw-r--r--   0        0        0     2645 2023-05-07 03:16:58.467263 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_statistics_mapper.py
+-rw-r--r--   0        0        0     2494 2023-03-13 11:15:04.252961 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py
+-rw-r--r--   0        0        0     3086 2023-03-01 06:19:33.488463 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py
+-rw-r--r--   0        0        0     3027 2023-03-13 11:15:04.253961 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py
+-rw-r--r--   0        0        0    13761 2023-03-13 11:15:04.254961 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py
+-rw-r--r--   0        0        0     2811 2023-03-13 11:15:04.255960 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py
+-rw-r--r--   0        0        0     2807 2023-03-01 06:19:33.490557 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py
+-rw-r--r--   0        0        0     5297 2023-05-07 02:54:53.398010 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py
+-rw-r--r--   0        0        0     3427 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/__init__.py
+-rw-r--r--   0        0        0     1022 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py
+-rw-r--r--   0        0        0     2519 2023-03-13 11:15:04.258743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py
+-rw-r--r--   0        0        0     1708 2023-03-13 11:15:04.258743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/send_messages.py
+-rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228228 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/errors.py
+-rw-r--r--   0        0        0        0 2022-10-11 14:30:16.137278 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py
+-rw-r--r--   0        0        0      492 2022-10-25 11:55:32.743202 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/enums.py
+-rw-r--r--   0        0        0      251 2023-05-07 03:08:43.903152 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/game_statistics.py
+-rw-r--r--   0        0        0       39 2023-03-13 11:15:04.259743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/__init__.py
+-rw-r--r--   0        0        0      129 2023-03-13 11:15:04.259743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/__init__.py
+-rw-r--r--   0        0        0     2014 2023-03-13 13:49:53.073496 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/metainfo.py
+-rw-r--r--   0        0        0      653 2023-03-13 11:15:04.261743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/__init__.py
+-rw-r--r--   0        0        0      255 2023-03-13 11:15:04.261743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/v1_to_v2.py
+-rw-r--r--   0        0        0      584 2023-04-04 02:00:50.080978 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/src.py
+-rw-r--r--   0        0        0     3840 2023-03-13 11:15:04.263743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/game.py
+-rw-r--r--   0        0        0      876 2023-03-13 11:15:04.263743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/group.py
+-rw-r--r--   0        0        0     3819 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/season.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/__init__.py
+-rw-r--r--   0        0        0      522 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/userdict.py
+-rw-r--r--   0        0        0      461 2023-03-13 11:15:04.265743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/user.py
+-rw-r--r--   0        0        0        0 2022-10-11 14:02:12.038461 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/__init__.py
+-rw-r--r--   0        0        0    19614 2023-05-07 03:19:06.560247 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py
+-rw-r--r--   0        0        0     2196 2023-03-13 11:15:04.266743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py
+-rw-r--r--   0        0        0     3736 2023-03-01 06:19:33.494591 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py
+-rw-r--r--   0        0        0    10068 2023-03-13 13:34:40.919314 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py
+-rw-r--r--   0        0        0      582 2023-03-01 06:19:33.495592 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py
+-rw-r--r--   0        0        0        0 2022-10-25 10:53:45.022120 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/__init__.py
+-rw-r--r--   0        0        0      288 2022-10-25 10:55:21.893872 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/date.py
+-rw-r--r--   0        0        0     1240 2022-10-25 10:57:00.084086 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py
+-rw-r--r--   0        0        0      101 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/nonebot.py
+-rw-r--r--   0        0        0      482 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/rank.py
+-rw-r--r--   0        0        0      256 2023-02-24 10:26:11.257181 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/upload_file.py
+-rw-r--r--   0        0        0      761 2023-03-13 11:15:04.268743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py
+-rw-r--r--   0        0        0     7618 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.3.1/PKG-INFO
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/LICENSE` & `nonebot_plugin_mahjong_scoreboard-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/pyproject.toml` & `nonebot_plugin_mahjong_scoreboard-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "nonebot-plugin-mahjong-scoreboard"
-version = "0.3.0a1"
+version = "0.3.1"
 description = "日麻寄分器（NoneBot插件）"
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.MD"
 license = "MIT"
 repository = "https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard"
 packages = [
     { include = "nonebot_plugin_mahjong_scoreboard", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-nonebot2 = "^2.0.0rc1"
-nonebot-adapter-onebot = "^2.1.5"
+nonebot2 = "^2.0.0rc4"
+nonebot-adapter-onebot = "^2.2.2"
 nonebot-plugin-sqlalchemy = "^0.2.0"
 aiosqlite = ">=0.17,<0.19"
 tzlocal = "^4.2"
 nonebot_plugin_apscheduler = "^0.2.0"
 cachetools = "^5.2.0"
-nonebot-plugin-gocqhttp-cross-machine-upload-file = "^0.1.3"
+nonebot-plugin-gocqhttp-cross-machine-upload-file = "^0.1.4"
 
 [tool.poetry.group.dev.dependencies]
 nonebug = "^0.2.1"
 flake8 = "^5.0.4"
 nonebot2 = {extras = ["fastapi"], version = "^2.0.0rc3"}
 
 [build-system]
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/README.MD` & `nonebot_plugin_mahjong_scoreboard-0.3.1/README.MD`

 * *Files 22% similar despite different names*

```diff
@@ -29,14 +29,79 @@
 
 ## 功能
 
 为群友提供日麻对局分数记录。根据马点进行PT精算，统计PT增减，支持对局与榜单查询与导出。
 
 PT精算算法为（点数-返点+马点）/1000，返点和马点在创建赛季时进行设置。
 
+## 常用Workflow
+
+### 开启赛季
+
+```
+/新建赛季
+```
+
+### 记录半庄对局
+
+```
+任何人：/新建对局
+A: /结算 25000
+B: /结算 25000
+C: /结算 25000
+D: /结算 25000
+```
+
+### 记录东场对局
+
+```
+任何人：/新建对局 四人东
+A: /结算 25000
+B: /结算 25000
+C: /结算 25000
+D: /结算 25000
+```
+
+### 记录未完成对局
+
+```
+任何人：/新建对局
+任何人：/设置对局进度 东一局0本场
+A: /结算 25000 东
+B: /结算 25000 南
+C: /结算 25000 西
+D: /结算 25000 北
+```
+
+### 将未完成对局设置为已完成
+
+```
+任何人：/设置对局进度 对局23050701 完成
+```
+
+### 删除对局
+
+用户无需手动删除错误创建的对局。当对局新建超过24h仍未成功结算时，对局会自动删除。
+
+删除已结算的对局需要管理员权限。
+
+```
+/删除对局 对局23050701
+```
+
+### 结算后为对局手动设置PT（当自动计算的PT不正确时，或者需要进行处罚时）
+
+```
+需要设置PT的人：/设置对局PT -52
+
+或
+
+任何人：/设置对局PT @需要设置PT的人 -52
+```
+
 ## 指令
 
 ### 对局
 
 - `/新建对局 [四人南|四人东]`
     - 别名：`/新对局`
 - `/结算对局 <成绩> [对局<编号>] [@<用户>] [<自风>]`
@@ -86,16 +151,18 @@
 ### 赛季查询
 
 - `/查询榜单`
     - 别名：`/榜单`
 - `/导出榜单`
 - `/查询PT [@<用户>]`
     - 别名：`/PT`
-- `/设置PT <PT> [@<用户>]`
-    - 别名：`/设置pt`
+- `/设置用户PT <PT> @<用户>`
+    - 别名：`/设置用户pt`, `/设置PT`, `/设置pt`
+- `/重置用户PT @<用户>`
+    - 别名：`/重置用户pt`, `/重置PT`, `/重置pt`
 
 ### 数据统计
 
 - `/对战数据`
 - `/赛季对战数据 [<赛季代号>]`
 - `/最近走势 [@<用户>]`
     - 别名：`/走势`
```

#### html2text {}

```diff
@@ -3,17 +3,32 @@
                           æ¥éº»è®°åå¨æä»¶ â¨_
                            [license] [pypi] [python]
 æ¯æééå¨ï¼[OneBot V11](https://onebot.adapters.nonebot.dev/
 ) æ¯æé©±å¨å¨ï¼[FastAPI](https://v2.nonebot.dev/docs/tutorial/choose-
 driver) ## åè½
 ä¸ºç¾¤åæä¾æ¥éº»å¯¹å±åæ°è®°å½ãæ ¹æ®é©¬ç¹è¿è¡PTç²¾ç®ï¼ç»è®¡PTå¢åï¼æ¯æå¯¹å±ä¸æ¦åæ¥è¯¢ä¸å¯¼åºã
 PTç²¾ç®ç®æ³ä¸ºï¼ç¹æ°-è¿ç¹+é©¬ç¹ï¼/
-1000ï¼è¿ç¹åé©¬ç¹å¨åå»ºèµå­£æ¶è¿è¡è®¾ç½®ã ## æä»¤ ### å¯¹å± -
-`/æ°å»ºå¯¹å± [åäººå|åäººä¸]` - å«åï¼`/æ°å¯¹å±` - `/ç»ç®å¯¹å±
-<æç»©> [å¯¹å±<ç¼å·>] [@<ç¨æ·>] [<èªé£>]` - å«åï¼`/ç»ç®` - `/
+1000ï¼è¿ç¹åé©¬ç¹å¨åå»ºèµå­£æ¶è¿è¡è®¾ç½®ã ## å¸¸ç¨Workflow ###
+å¼å¯èµå­£ ``` /æ°å»ºèµå­£ ``` ### è®°å½ååºå¯¹å± ``` ä»»ä½äººï¼/
+æ°å»ºå¯¹å± A: /ç»ç® 25000 B: /ç»ç® 25000 C: /ç»ç® 25000 D: /ç»ç®
+25000 ``` ### è®°å½ä¸åºå¯¹å± ``` ä»»ä½äººï¼/æ°å»ºå¯¹å± åäººä¸ A: /
+ç»ç® 25000 B: /ç»ç® 25000 C: /ç»ç® 25000 D: /ç»ç® 25000 ``` ###
+è®°å½æªå®æå¯¹å± ``` ä»»ä½äººï¼/æ°å»ºå¯¹å± ä»»ä½äººï¼/
+è®¾ç½®å¯¹å±è¿åº¦ ä¸ä¸å±0æ¬åº A: /ç»ç® 25000 ä¸ B: /ç»ç® 25000 å
+C: /ç»ç® 25000 è¥¿ D: /ç»ç® 25000 å ``` ###
+å°æªå®æå¯¹å±è®¾ç½®ä¸ºå·²å®æ ``` ä»»ä½äººï¼/è®¾ç½®å¯¹å±è¿åº¦
+å¯¹å±23050701 å®æ ``` ### å é¤å¯¹å±
+ç¨æ·æ éæå¨å é¤éè¯¯åå»ºçå¯¹å±ãå½å¯¹å±æ°å»ºè¶è¿24hä»æªæåç»ç®æ¶ï¼å¯¹å±ä¼èªå¨å é¤ã
+å é¤å·²ç»ç®çå¯¹å±éè¦ç®¡çåæéã ``` /å é¤å¯¹å±
+å¯¹å±23050701 ``` ###
+ç»ç®åä¸ºå¯¹å±æå¨è®¾ç½®PTï¼å½èªå¨è®¡ç®çPTä¸æ­£ç¡®æ¶ï¼æèéè¦è¿è¡å¤ç½æ¶ï¼
+``` éè¦è®¾ç½®PTçäººï¼/è®¾ç½®å¯¹å±PT -52 æ ä»»ä½äººï¼/è®¾ç½®å¯¹å±PT
+@éè¦è®¾ç½®PTçäºº -52 ``` ## æä»¤ ### å¯¹å± - `/æ°å»ºå¯¹å±
+[åäººå|åäººä¸]` - å«åï¼`/æ°å¯¹å±` - `/ç»ç®å¯¹å± <æç»©>
+[å¯¹å±<ç¼å·>] [@<ç¨æ·>] [<èªé£>]` - å«åï¼`/ç»ç®` - `/
 æ¤éç»ç®å¯¹å± [å¯¹å±<ç¼å·>] [@<ç¨æ·>]` - å«åï¼`/æ¤éç»ç®` -
 `/è®¾ç½®å¯¹å±PT  [å¯¹å±<ç¼å·>] [@<ç¨æ·>]` - å«åï¼`/å¯¹å±PT` - `/
 å é¤å¯¹å± [å¯¹å±<ç¼å·>]` - `/è®¾ç½®å¯¹å±è¿åº¦ <ä¸/åxå±yæ¬åº æ
 å®æ> [å¯¹å±<ç¼å·>]` - å«åï¼`/å¯¹å±è¿åº¦` - `/è®¾ç½®å¯¹å±å¤æ³¨
 [å¯¹å±<ç¼å·>] <å¯¹å±å¤æ³¨>` - å«åï¼`/å¯¹å±å¤æ³¨`
 ä¸å¯¹å±ç¸å³çæä»¤å¯ä»¥çç¥å¯¹å±ç¼å·ï¼çç¥æ¶é»è®¤å¯¹æè¿æ°å»ºçå¯¹å±è¿è¡æä½ãä¹å¯ä»¥éè¿åå¤Botååºçå¯¹å±æ¶æ¯æ¥ä»£æ¿æå®å¯¹å±ç¼å·ã
 å¯¹å±ç¸å³æä»¤å¨å¯¹å±å®æè¶è¿24å°æ¶åéè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ãï¼`/
@@ -24,17 +39,19 @@
 - `/ä¸ªäººæªå®æå¯¹å± [@<ç¨æ·>]` - å«åï¼`/æªå®æå¯¹å±` - `/
 ç¾¤æªå®æå¯¹å±` - `/å¯¼åºèµå­£å¯¹å± [<ä»£å·>]` - å«åï¼`/
 å¯¼åºå¯¹å±` - `/å¯¼åºææå¯¹å±` ### èµå­£ - `/æ¥è¯¢èµå­£ [<ä»£å·>]` -
 å«åï¼`/èµå­£`ï¼`/å½åèµå­£` - `/æ¥è¯¢ææèµå­£` - å«åï¼`/
 ææèµå­£` - `/æ°å»ºèµå­£` - å«åï¼`/æ°èµå­£` - `/å¼å¯èµå­£
 [<ä»£å·>]` - `/ç»æèµå­£` - `/å é¤èµå­£ [<ä»£å·>]` ### èµå­£æ¥è¯¢ -
 `/æ¥è¯¢æ¦å` - å«åï¼`/æ¦å` - `/å¯¼åºæ¦å` - `/æ¥è¯¢PT
-[@<ç¨æ·>]` - å«åï¼`/PT` - `/è®¾ç½®PT  [@<ç¨æ·>]` - å«åï¼`/è®¾ç½®pt`
-### æ°æ®ç»è®¡ - `/å¯¹ææ°æ®` - `/èµå­£å¯¹ææ°æ® [<èµå­£ä»£å·>]` -
-`/æè¿èµ°å¿ [@<ç¨æ·>]` - å«åï¼`/èµ°å¿` ä¸èµå­£/
+[@<ç¨æ·>]` - å«åï¼`/PT` - `/è®¾ç½®ç¨æ·PT  @<ç¨æ·>` - å«åï¼`/
+è®¾ç½®ç¨æ·pt`, `/è®¾ç½®PT`, `/è®¾ç½®pt` - `/éç½®ç¨æ·PT @<ç¨æ·>` -
+å«åï¼`/éç½®ç¨æ·pt`, `/éç½®PT`, `/éç½®pt` ### æ°æ®ç»è®¡ - `/
+å¯¹ææ°æ®` - `/èµå­£å¯¹ææ°æ® [<èµå­£ä»£å·>]` - `/æè¿èµ°å¿
+[@<ç¨æ·>]` - å«åï¼`/èµ°å¿` ä¸èµå­£/
 èµå­£PTç¸å³çæä»¤åå¯éè¿ç§è/
 ç¾¤èä¸¤ç§æ¹å¼ä½¿ç¨ãå½æªæå®åæ°æ¶è¿å¥é®ç­æ¨¡å¼ï¼åå¤`/
 q`å¯éåºé®ç­æ¨¡å¼ã ä¸èµå­£/
 èµå­£PTç¸å³çæä»¤ï¼æ¥è¯¢ãå¯¼åºé¤å¤ï¼éè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ã
 ## éç½® ### mahjong_scoreboard_database_conn_url
 æ°æ®åºè¿æ¥URLï¼å¿é¡»ä½¿ç¨å¼æ­¥SQLAlchemyé©±å¨å¨ã
 é»è®¤å¼ï¼sqlite+aiosqlite:///mahjong_scoreboard.db ### callback_host
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from nonebot.adapters.onebot.v11 import Message
 from nonebot.internal.matcher import Matcher
 
 from nonebot_plugin_mahjong_scoreboard.controller.general_handlers import require_parse_unary_at_arg, \
     require_group_binding_qq, require_user_binding_qq, require_running_season
 from nonebot_plugin_mahjong_scoreboard.controller.interceptor import general_interceptor
 from nonebot_plugin_mahjong_scoreboard.controller.mapper.game_statistics_mapper import map_season_user_trend, \
-    map_user_statistics, map_season_user_statistics
+    map_game_statistics
 from nonebot_plugin_mahjong_scoreboard.controller.utils.message import SplitCommandArgs
 from nonebot_plugin_mahjong_scoreboard.errors import BadRequestError
 from nonebot_plugin_mahjong_scoreboard.service import season_user_point_service
-from nonebot_plugin_mahjong_scoreboard.service.game_service import get_games
+from nonebot_plugin_mahjong_scoreboard.service.game_service import get_game_statistics
 from nonebot_plugin_mahjong_scoreboard.service.group_service import get_group_by_binding_qq
 from nonebot_plugin_mahjong_scoreboard.service.season_service import get_season_by_id, get_season_by_code
 from nonebot_plugin_mahjong_scoreboard.service.user_service import get_user_by_binding_qq
 
 # ============ 查询最近走势 ============
 query_season_user_trend_matcher = on_command("查询最近走势", aliases={"最近走势", "走势"}, priority=5)
 
@@ -58,29 +58,16 @@
 async def query_user_statistics(matcher: Matcher):
     group_binding_qq = matcher.state["binding_qq"]
     user_binding_qq = matcher.state["user_binding_qq"]
 
     group = await get_group_by_binding_qq(group_binding_qq)
     user = await get_user_by_binding_qq(user_binding_qq)
 
-    games = await get_games(group, user, completed_only=True)
-
-    if len(games) == 0:
-        await matcher.send("你还没有进行对局")
-        return
-
-    cnt = [0, 0, 0, 0]
-
-    for g in games:
-        for r in g.records:
-            if r.user_id == user.id:
-                cnt[r.rank - 1] += 1
-
-    rates = list(map(lambda x: x / len(games), cnt))
-    msg = await map_user_statistics(group, user, len(games), rates)
+    game_statistics = await get_game_statistics(group, user)
+    msg = await map_game_statistics(group, user, None, game_statistics)
     await matcher.send(msg)
 
 
 # ============ 赛季对战数据 ============
 query_season_user_statistics_matcher = on_command("赛季对战数据", priority=5)
 
 
@@ -124,23 +111,10 @@
             raise BadRequestError("找不到指定赛季")
     else:
         if group.running_season_id:
             season = await get_season_by_id(group.running_season_id)
         else:
             raise BadRequestError("当前没有运行中的赛季")
 
-    games = await get_games(group, user, season, completed_only=True)
-
-    if len(games) == 0:
-        await matcher.send("你还没有进行对局")
-        return
-
-    cnt = [0, 0, 0, 0]
-
-    for g in games:
-        for r in g.records:
-            if r.user_id == user.id:
-                cnt[r.rank - 1] += 1
-
-    rates = list(map(lambda x: x / len(games), cnt))
-    msg = await map_season_user_statistics(group, user, season, len(games), rates)
+    game_statistics = await get_game_statistics(group, user, season)
+    msg = await map_game_statistics(group, user, season, game_statistics)
     await matcher.send(msg)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/general_handlers.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/general_handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_error_impl.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_error_impl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_interruption_impl.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_interruption_impl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+from typing import Union
 
 import pytz
 import tzlocal
 
 from nonebot_plugin_mahjong_scoreboard.model.enums import PlayerAndWind, GameState, SeasonState, Wind
 
 player_and_wind_mapping = {
@@ -45,14 +46,14 @@
     return dt.astimezone(tzlocal.get_localzone()).strftime(datetime_format)
 
 
 def percentile_str(x: float, ndigits: int = 2) -> str:
     return f'{round(x * 100, ndigits)}%'
 
 
-def map_point(raw_point: int, scale: int) -> str:
+def map_point(raw_point: Union[int, float], scale: int = 0) -> str:
     point_text = f"%.{-scale}f" % (raw_point * 10 ** scale)
     if raw_point > 0:
         point_text = f'+{point_text}'
     elif raw_point == 0:
         point_text = f'±{point_text}'
     return point_text
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_statistics_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_statistics_mapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from io import StringIO
-from typing import List, Tuple
+from typing import List, Tuple, Optional
 
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 
 from nonebot_plugin_mahjong_scoreboard.controller.mapper import digit_mapping, percentile_str
 from nonebot_plugin_mahjong_scoreboard.controller.mapper.season_user_point_mapper import map_point
+from nonebot_plugin_mahjong_scoreboard.model.game_statistics import GameStatistics
 from nonebot_plugin_mahjong_scoreboard.model.orm.game import GameRecordOrm, GameOrm
 from nonebot_plugin_mahjong_scoreboard.model.orm.group import GroupOrm
 from nonebot_plugin_mahjong_scoreboard.model.orm.season import SeasonOrm, \
     SeasonUserPointChangeLogOrm
 from nonebot_plugin_mahjong_scoreboard.model.orm.user import UserOrm
 from nonebot_plugin_mahjong_scoreboard.service.group_service import get_user_nickname
 
@@ -22,27 +23,24 @@
             sio.write(f"  {record.rank}位    {record.score}点  "
                       f"({map_point(record.raw_point, record.point_scale)})  "
                       f"对局{game.code}\n")
 
         return Message(MessageSegment.text(sio.getvalue().strip()))
 
 
-async def map_user_statistics(group: GroupOrm, user: UserOrm, total: int, rates: List[int]) -> Message:
+async def map_game_statistics(group: GroupOrm, user: UserOrm, season: Optional[SeasonOrm],
+                              game_statistics: GameStatistics) -> Message:
     with StringIO() as sio:
-        sio.write(f"用户[{await get_user_nickname(user, group)}]的对战数据如下：\n")
+        if season is not None:
+            sio.write(f"用户[{await get_user_nickname(user, group)}]在赛季[{season.name}]的对战数据如下：\n")
+        else:
+            sio.write(f"用户[{await get_user_nickname(user, group)}]的对战数据如下：\n")
 
-        sio.write(f"  对局数：{total}\n")
-        for i, rate in enumerate(rates):
-            sio.write(f"  {digit_mapping[i + 1]}位率：{percentile_str(rate)}\n")
-
-        return Message(MessageSegment.text(sio.getvalue().strip()))
-
-
-async def map_season_user_statistics(group: GroupOrm, user: UserOrm, season: SeasonOrm, total: int, rates: List[int]) -> Message:
-    with StringIO() as sio:
-        sio.write(f"用户[{await get_user_nickname(user, group)}]在赛季[{season.name}]的对战数据如下：\n")
-
-        sio.write(f"  对局数：{total}\n")
-        for i, rate in enumerate(rates):
+        sio.write(f"  对局数：{game_statistics.total} （半庄：{game_statistics.total_south}、东风：{game_statistics.total_east}）\n")
+        for i, rate in enumerate(game_statistics.rates):
             sio.write(f"  {digit_mapping[i + 1]}位率：{percentile_str(rate)}\n")
+        sio.write(f"  平均顺位：{round(game_statistics.avg_rank, 2)}\n")
+        if game_statistics.pt_expectation is not None:
+            sio.write(f"  PT期望：{map_point(game_statistics.pt_expectation)}\n")
+        sio.write(f"  被飞率：{percentile_str(game_statistics.flying_rate)}")
 
         return Message(MessageSegment.text(sio.getvalue().strip()))
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         msg.append(MessageSegment.text("\n\n设置用户PT成功"))
         await matcher.send(msg)
     else:
         await matcher.finish("取消设置用户PT")
 
 
 # ========== 重置用户PT ==========
-reset_season_user_point_matcher = on_command("重置用户PT", aliases={"初始化用户pt"}, priority=5)
+reset_season_user_point_matcher = on_command("重置用户PT", aliases={"重置用户pt", "重置PT", "重置pt"}, priority=5)
 
 require_parse_unary_at_arg(reset_season_user_point_matcher, "user_binding_qq")
 require_group_binding_qq(reset_season_user_point_matcher)
 require_user_binding_qq(reset_season_user_point_matcher, sender_as_default_on_group_msg=False)
 require_running_season(reset_season_user_point_matcher)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/send_messages.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/send_messages.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/metainfo.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/metainfo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/src.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/src.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/game.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/group.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/season.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/season.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/userdict.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/userdict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from sqlalchemy import select, update, delete
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import selectinload
 from sqlalchemy.sql import Select
 
 from nonebot_plugin_mahjong_scoreboard.errors import BadRequestError
 from nonebot_plugin_mahjong_scoreboard.model.enums import GameState, PlayerAndWind, Wind, SeasonState
+from nonebot_plugin_mahjong_scoreboard.model.game_statistics import GameStatistics
 from nonebot_plugin_mahjong_scoreboard.model.orm import data_source
 from nonebot_plugin_mahjong_scoreboard.model.orm.game import GameOrm, GameRecordOrm, GameProgressOrm
 from nonebot_plugin_mahjong_scoreboard.model.orm.group import GroupOrm
 from nonebot_plugin_mahjong_scoreboard.model.orm.season import SeasonOrm
 from nonebot_plugin_mahjong_scoreboard.model.orm.user import UserOrm
 from nonebot_plugin_mahjong_scoreboard.service.group_service import is_group_admin
 from nonebot_plugin_mahjong_scoreboard.service.season_user_point_service import revert_season_user_point_by_game, \
@@ -480,11 +481,68 @@
     game.comment = comment
 
     game.update_time = datetime.utcnow()
     await session.commit()
     return game
 
 
+async def get_game_statistics(group: GroupOrm, user: UserOrm, season: Optional[SeasonOrm] = None):
+    games = await get_games(group, user, season, completed_only=True)
+
+    if len(games) == 0:
+        raise BadRequestError("你还没有进行对局")
+
+    total = len(games)
+
+    total_east = 0
+    total_south = 0
+
+    for g in games:
+        if g.player_and_wind == PlayerAndWind.four_men_south:
+            total_south += 1
+        elif g.player_and_wind == PlayerAndWind.four_men_east:
+            total_east += 1
+
+    cnt = [0, 0, 0, 0]
+
+    pt_south = 0.0
+    pt_east = 0.0
+
+    flying = 0
+
+    for g in games:
+        for r in g.records:
+            if r.user_id == user.id:
+                cnt[r.rank - 1] += 1
+
+                if r.score < 0:
+                    flying += 1
+
+                if g.player_and_wind == PlayerAndWind.four_men_south:
+                    pt_south += r.point
+                elif g.player_and_wind == PlayerAndWind.four_men_east:
+                    pt_east += r.point
+
+                break
+
+    rates = list(map(lambda x: x / total, cnt))
+
+    avg_rank = (cnt[0] * 1 + cnt[1] * 2 + cnt[2] * 3 + cnt[3] * 4) / total
+
+    if season is not None:
+        pt_expectation = 0
+        if total_south:
+            pt_expectation += pt_south / total_south
+        if total_east:
+            pt_expectation += pt_east / total_east
+    else:
+        pt_expectation = None
+
+    flying_rate = flying / total
+
+    return GameStatistics(total, total_east, total_south, rates, avg_rank, pt_expectation, flying_rate)
+
+
 __all__ = ("get_game_by_code", "get_games",
            "new_game", "delete_game", "record_game", "revert_record", "set_record_point",
            "make_game_progress", "remove_game_progress",
            "delete_uncompleted_season_games")
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.0a1/setup.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,251 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-mahjong-scoreboard
+Version: 0.3.1
+Summary: 日麻寄分器（NoneBot插件）
+Home-page: https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard
+License: MIT
+Author: ssttkkl
+Author-email: huang.wen.long@hotmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiosqlite (>=0.17,<0.19)
+Requires-Dist: cachetools (>=5.2.0,<6.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
+Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-file (>=0.1.4,<0.2.0)
+Requires-Dist: nonebot-plugin-sqlalchemy (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
+Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: tzlocal (>=4.2,<5.0)
+Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard
+Description-Content-Type: text/plain
 
-package_dir = \
-{'': 'src'}
+<!-- markdownlint-disable MD033 MD036 MD041 -->
 
-packages = \
-['nonebot_plugin_mahjong_scoreboard',
- 'nonebot_plugin_mahjong_scoreboard.controller',
- 'nonebot_plugin_mahjong_scoreboard.controller.interceptor',
- 'nonebot_plugin_mahjong_scoreboard.controller.mapper',
- 'nonebot_plugin_mahjong_scoreboard.controller.utils',
- 'nonebot_plugin_mahjong_scoreboard.model',
- 'nonebot_plugin_mahjong_scoreboard.model.orm',
- 'nonebot_plugin_mahjong_scoreboard.model.orm._data_source',
- 'nonebot_plugin_mahjong_scoreboard.model.orm._data_source.migrations',
- 'nonebot_plugin_mahjong_scoreboard.model.orm.types',
- 'nonebot_plugin_mahjong_scoreboard.service',
- 'nonebot_plugin_mahjong_scoreboard.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiosqlite>=0.17,<0.19',
- 'cachetools>=5.2.0,<6.0.0',
- 'nonebot-adapter-onebot>=2.1.5,<3.0.0',
- 'nonebot-plugin-gocqhttp-cross-machine-upload-file>=0.1.3,<0.2.0',
- 'nonebot-plugin-sqlalchemy>=0.2.0,<0.3.0',
- 'nonebot2>=2.0.0rc1,<3.0.0',
- 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
- 'tzlocal>=4.2,<5.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-mahjong-scoreboard',
-    'version': '0.3.0a1',
-    'description': '日麻寄分器（NoneBot插件）',
-    'long_description': '<!-- markdownlint-disable MD033 MD036 MD041 -->\n\n<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\nnonebot-plugin-mahjong-scoreboard\n============\n\n_✨ NoneBot 日麻记分器插件 ✨_\n\n</div>\n\n<p align="center">\n  <a href="https://raw.githubusercontent.com/ssttkkl/nonebot-plugin-mahjong-scoreboard/master/LICENSE">\n    <img src="https://img.shields.io/github/license/ssttkkl/nonebot-plugin-mahjong-scoreboard.svg" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/nonebot-plugin-mahjong-scoreboard">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-mahjong-scoreboard.svg" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n</p>\n\n支持适配器：[OneBot V11](https://onebot.adapters.nonebot.dev/)\n\n支持驱动器：[FastAPI](https://v2.nonebot.dev/docs/tutorial/choose-driver)\n\n## 功能\n\n为群友提供日麻对局分数记录。根据马点进行PT精算，统计PT增减，支持对局与榜单查询与导出。\n\nPT精算算法为（点数-返点+马点）/1000，返点和马点在创建赛季时进行设置。\n\n## 指令\n\n### 对局\n\n- `/新建对局 [四人南|四人东]`\n    - 别名：`/新对局`\n- `/结算对局 <成绩> [对局<编号>] [@<用户>] [<自风>]`\n    - 别名：`/结算`\n- `/撤销结算对局 [对局<编号>] [@<用户>]`\n    - 别名：`/撤销结算`\n- `/设置对局PT <PT> [对局<编号>] [@<用户>]`\n    - 别名：`/对局PT`\n- `/删除对局 [对局<编号>]`\n- `/设置对局进度 <东/南x局y本场 或 完成> [对局<编号>]`\n    - 别名：`/对局进度`\n- `/设置对局备注 [对局<编号>] <对局备注>`\n    - 别名：`/对局备注`\n\n与对局相关的指令可以省略对局编号，省略时默认对最近新建的对局进行操作。也可以通过回复Bot发出的对局消息来代替指定对局编号。\n\n对局相关指令在对局完成超过24小时后需要拥有群主或管理员身份才能使用。（`/删除对局`除外，该指令需要拥有群主或管理员身份才能使用）\n\n未完成且未设置进度的对局会在创建24小时后自动删除。赛季结束后，未完成对局会自动删除，所有已完成对局均无法再进行修改。\n\n### 对局查询\n\n- `/查询对局 [<编号>]`\n    - 别名：`/对局`\n- `/个人最近对局 [@<用户>]`\n    - 别名：`/最近对局`\n- `/群最近对局`\n- `/个人未完成对局 [@<用户>]`\n    - 别名：`/未完成对局`\n- `/群未完成对局`\n- `/导出赛季对局 [<代号>]`\n    - 别名：`/导出对局`\n- `/导出所有对局`\n\n### 赛季\n\n- `/查询赛季 [<代号>]`\n    - 别名：`/赛季`，`/当前赛季`\n- `/查询所有赛季`\n    - 别名：`/所有赛季`\n- `/新建赛季`\n    - 别名：`/新赛季`\n- `/开启赛季 [<代号>]`\n- `/结束赛季`\n- `/删除赛季 [<代号>]`\n\n### 赛季查询\n\n- `/查询榜单`\n    - 别名：`/榜单`\n- `/导出榜单`\n- `/查询PT [@<用户>]`\n    - 别名：`/PT`\n- `/设置PT <PT> [@<用户>]`\n    - 别名：`/设置pt`\n\n### 数据统计\n\n- `/对战数据`\n- `/赛季对战数据 [<赛季代号>]`\n- `/最近走势 [@<用户>]`\n    - 别名：`/走势`\n\n与赛季/赛季PT相关的指令均可通过私聊/群聊两种方式使用。当未指定参数时进入问答模式，回复`/q`可退出问答模式。\n\n与赛季/赛季PT相关的指令（查询、导出除外）需要拥有群主或管理员身份才能使用。\n\n## 配置\n\n### mahjong_scoreboard_database_conn_url\n\n数据库连接URL，必须使用异步SQLAlchemy驱动器。\n\n默认值：sqlite+aiosqlite:///mahjong_scoreboard.db\n\n### callback_host\n\n回调HOST，若为非容器环境部署（go-cqhttp与nonebot均运行在同一环境）则保持默认值。若为Docker环境部署则设置为Docker容器名。用于上传文件时让go-cqhttp下载本机文件。\n\n默认值：127.0.0.1\n\n### callback_port\n\n回调端口，保持默认值即可。\n\n默认值：与PORT保持一致即可\n\n## 在线乞讨\n\n<details><summary>点击请我打两把maimai</summary>\n\n![](https://github.com/ssttkkl/ssttkkl/blob/main/afdian-ssttkkl.jfif)\n\n</details>\n\n## LICENSE\n\n> MIT License\n>\n> Copyright (c) 2022 ssttkkl\n>\n> Permission is hereby granted, free of charge, to any person obtaining a copy\n> of this software and associated documentation files (the "Software"), to deal\n> in the Software without restriction, including without limitation the rights\n> to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n> copies of the Software, and to permit persons to whom the Software is\n> furnished to do so, subject to the following conditions:\n>\n> The above copyright notice and this permission notice shall be included in all\n> copies or substantial portions of the Software.\n>\n> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\n> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\n> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\n> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\n> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\n> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\n> SOFTWARE.\n> \n',
-    'author': 'ssttkkl',
-    'author_email': 'huang.wen.long@hotmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+<p align="center">
+  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+</p>
 
+<div align="center">
+
+nonebot-plugin-mahjong-scoreboard
+============
+
+_✨ NoneBot 日麻记分器插件 ✨_
+
+</div>
+
+<p align="center">
+  <a href="https://raw.githubusercontent.com/ssttkkl/nonebot-plugin-mahjong-scoreboard/master/LICENSE">
+    <img src="https://img.shields.io/github/license/ssttkkl/nonebot-plugin-mahjong-scoreboard.svg" alt="license">
+  </a>
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-mahjong-scoreboard">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-mahjong-scoreboard.svg" alt="pypi">
+  </a>
+  <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+</p>
+
+支持适配器：[OneBot V11](https://onebot.adapters.nonebot.dev/)
+
+支持驱动器：[FastAPI](https://v2.nonebot.dev/docs/tutorial/choose-driver)
+
+## 功能
+
+为群友提供日麻对局分数记录。根据马点进行PT精算，统计PT增减，支持对局与榜单查询与导出。
+
+PT精算算法为（点数-返点+马点）/1000，返点和马点在创建赛季时进行设置。
+
+## 常用Workflow
+
+### 开启赛季
+
+```
+/新建赛季
+```
+
+### 记录半庄对局
+
+```
+任何人：/新建对局
+A: /结算 25000
+B: /结算 25000
+C: /结算 25000
+D: /结算 25000
+```
+
+### 记录东场对局
+
+```
+任何人：/新建对局 四人东
+A: /结算 25000
+B: /结算 25000
+C: /结算 25000
+D: /结算 25000
+```
+
+### 记录未完成对局
+
+```
+任何人：/新建对局
+任何人：/设置对局进度 东一局0本场
+A: /结算 25000 东
+B: /结算 25000 南
+C: /结算 25000 西
+D: /结算 25000 北
+```
+
+### 将未完成对局设置为已完成
+
+```
+任何人：/设置对局进度 对局23050701 完成
+```
+
+### 删除对局
+
+用户无需手动删除错误创建的对局。当对局新建超过24h仍未成功结算时，对局会自动删除。
+
+删除已结算的对局需要管理员权限。
+
+```
+/删除对局 对局23050701
+```
+
+### 结算后为对局手动设置PT（当自动计算的PT不正确时，或者需要进行处罚时）
+
+```
+需要设置PT的人：/设置对局PT -52
+
+或
+
+任何人：/设置对局PT @需要设置PT的人 -52
+```
+
+## 指令
+
+### 对局
+
+- `/新建对局 [四人南|四人东]`
+    - 别名：`/新对局`
+- `/结算对局 <成绩> [对局<编号>] [@<用户>] [<自风>]`
+    - 别名：`/结算`
+- `/撤销结算对局 [对局<编号>] [@<用户>]`
+    - 别名：`/撤销结算`
+- `/设置对局PT <PT> [对局<编号>] [@<用户>]`
+    - 别名：`/对局PT`
+- `/删除对局 [对局<编号>]`
+- `/设置对局进度 <东/南x局y本场 或 完成> [对局<编号>]`
+    - 别名：`/对局进度`
+- `/设置对局备注 [对局<编号>] <对局备注>`
+    - 别名：`/对局备注`
+
+与对局相关的指令可以省略对局编号，省略时默认对最近新建的对局进行操作。也可以通过回复Bot发出的对局消息来代替指定对局编号。
+
+对局相关指令在对局完成超过24小时后需要拥有群主或管理员身份才能使用。（`/删除对局`除外，该指令需要拥有群主或管理员身份才能使用）
+
+未完成且未设置进度的对局会在创建24小时后自动删除。赛季结束后，未完成对局会自动删除，所有已完成对局均无法再进行修改。
+
+### 对局查询
+
+- `/查询对局 [<编号>]`
+    - 别名：`/对局`
+- `/个人最近对局 [@<用户>]`
+    - 别名：`/最近对局`
+- `/群最近对局`
+- `/个人未完成对局 [@<用户>]`
+    - 别名：`/未完成对局`
+- `/群未完成对局`
+- `/导出赛季对局 [<代号>]`
+    - 别名：`/导出对局`
+- `/导出所有对局`
+
+### 赛季
+
+- `/查询赛季 [<代号>]`
+    - 别名：`/赛季`，`/当前赛季`
+- `/查询所有赛季`
+    - 别名：`/所有赛季`
+- `/新建赛季`
+    - 别名：`/新赛季`
+- `/开启赛季 [<代号>]`
+- `/结束赛季`
+- `/删除赛季 [<代号>]`
+
+### 赛季查询
+
+- `/查询榜单`
+    - 别名：`/榜单`
+- `/导出榜单`
+- `/查询PT [@<用户>]`
+    - 别名：`/PT`
+- `/设置用户PT <PT> @<用户>`
+    - 别名：`/设置用户pt`, `/设置PT`, `/设置pt`
+- `/重置用户PT @<用户>`
+    - 别名：`/重置用户pt`, `/重置PT`, `/重置pt`
+
+### 数据统计
+
+- `/对战数据`
+- `/赛季对战数据 [<赛季代号>]`
+- `/最近走势 [@<用户>]`
+    - 别名：`/走势`
+
+与赛季/赛季PT相关的指令均可通过私聊/群聊两种方式使用。当未指定参数时进入问答模式，回复`/q`可退出问答模式。
+
+与赛季/赛季PT相关的指令（查询、导出除外）需要拥有群主或管理员身份才能使用。
+
+## 配置
+
+### mahjong_scoreboard_database_conn_url
+
+数据库连接URL，必须使用异步SQLAlchemy驱动器。
+
+默认值：sqlite+aiosqlite:///mahjong_scoreboard.db
+
+### callback_host
+
+回调HOST，若为非容器环境部署（go-cqhttp与nonebot均运行在同一环境）则保持默认值。若为Docker环境部署则设置为Docker容器名。用于上传文件时让go-cqhttp下载本机文件。
+
+默认值：127.0.0.1
+
+### callback_port
+
+回调端口，保持默认值即可。
+
+默认值：与PORT保持一致即可
+
+## 在线乞讨
+
+<details><summary>点击请我打两把maimai</summary>
+
+![](https://github.com/ssttkkl/ssttkkl/blob/main/afdian-ssttkkl.jfif)
+
+</details>
+
+## LICENSE
+
+> MIT License
+>
+> Copyright (c) 2022 ssttkkl
+>
+> Permission is hereby granted, free of charge, to any person obtaining a copy
+> of this software and associated documentation files (the "Software"), to deal
+> in the Software without restriction, including without limitation the rights
+> to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+> copies of the Software, and to permit persons to whom the Software is
+> furnished to do so, subject to the following conditions:
+>
+> The above copyright notice and this permission notice shall be included in all
+> copies or substantial portions of the Software.
+>
+> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+> SOFTWARE.
+> 
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,87 +1,93 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['nonebot_plugin_mahjong_scoreboard',
-'nonebot_plugin_mahjong_scoreboard.controller',
-'nonebot_plugin_mahjong_scoreboard.controller.interceptor',
-'nonebot_plugin_mahjong_scoreboard.controller.mapper',
-'nonebot_plugin_mahjong_scoreboard.controller.utils',
-'nonebot_plugin_mahjong_scoreboard.model',
-'nonebot_plugin_mahjong_scoreboard.model.orm',
-'nonebot_plugin_mahjong_scoreboard.model.orm._data_source',
-'nonebot_plugin_mahjong_scoreboard.model.orm._data_source.migrations',
-'nonebot_plugin_mahjong_scoreboard.model.orm.types',
-'nonebot_plugin_mahjong_scoreboard.service',
-'nonebot_plugin_mahjong_scoreboard.utils'] package_data = \ {'': ['*']}
-install_requires = \ ['aiosqlite>=0.17,<0.19', 'cachetools>=5.2.0,<6.0.0',
-'nonebot-adapter-onebot>=2.1.5,<3.0.0', 'nonebot-plugin-gocqhttp-cross-machine-
-upload-file>=0.1.3,<0.2.0', 'nonebot-plugin-sqlalchemy>=0.2.0,<0.3.0',
-'nonebot2>=2.0.0rc1,<3.0.0', 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
-'tzlocal>=4.2,<5.0'] setup_kwargs = { 'name': 'nonebot-plugin-mahjong-
-scoreboard', 'version': '0.3.0a1', 'description':
-'æ¥éº»å¯åå¨ï¼NoneBotæä»¶ï¼', 'long_description': '\n\n
-                                \n [nonebot]\n
-\n\n
-      \n\nnonebot-plugin-mahjong-scoreboard\n============\n\n_â¨ NoneBot
-                        æ¥éº»è®°åå¨æä»¶ â¨_\n\n
-\n\n
-                 \n \n_[license]\n\n \n_[pypi]\n\n [python]\n
-\n\næ¯æééå¨ï¼[OneBot V11](https://onebot.adapters.nonebot.dev/
-)\n\næ¯æé©±å¨å¨ï¼[FastAPI](https://v2.nonebot.dev/docs/tutorial/choose-
-driver)\n\n##
-åè½\n\nä¸ºç¾¤åæä¾æ¥éº»å¯¹å±åæ°è®°å½ãæ ¹æ®é©¬ç¹è¿è¡PTç²¾ç®ï¼ç»è®¡PTå¢åï¼æ¯æå¯¹å±ä¸æ¦åæ¥è¯¢ä¸å¯¼åºã\n\nPTç²¾ç®ç®æ³ä¸ºï¼ç¹æ°-
-è¿ç¹+é©¬ç¹ï¼/1000ï¼è¿ç¹åé©¬ç¹å¨åå»ºèµå­£æ¶è¿è¡è®¾ç½®ã\n\n##
-æä»¤\n\n### å¯¹å±\n\n- `/æ°å»ºå¯¹å± [åäººå|åäººä¸]`\n - å«åï¼`/
-æ°å¯¹å±`\n- `/ç»ç®å¯¹å± <æç»©> [å¯¹å±<ç¼å·>] [@<ç¨æ·>]
-[<èªé£>]`\n - å«åï¼`/ç»ç®`\n- `/æ¤éç»ç®å¯¹å± [å¯¹å±<ç¼å·>]
-[@<ç¨æ·>]`\n - å«åï¼`/æ¤éç»ç®`\n- `/è®¾ç½®å¯¹å±PT  [å¯¹å±<ç¼å·>]
-[@<ç¨æ·>]`\n - å«åï¼`/å¯¹å±PT`\n- `/å é¤å¯¹å± [å¯¹å±<ç¼å·>]`\n- `/
-è®¾ç½®å¯¹å±è¿åº¦ <ä¸/åxå±yæ¬åº æ å®æ> [å¯¹å±<ç¼å·>]`\n -
-å«åï¼`/å¯¹å±è¿åº¦`\n- `/è®¾ç½®å¯¹å±å¤æ³¨ [å¯¹å±<ç¼å·>]
-<å¯¹å±å¤æ³¨>`\n - å«åï¼`/
-å¯¹å±å¤æ³¨`\n\nä¸å¯¹å±ç¸å³çæä»¤å¯ä»¥çç¥å¯¹å±ç¼å·ï¼çç¥æ¶é»è®¤å¯¹æè¿æ°å»ºçå¯¹å±è¿è¡æä½ãä¹å¯ä»¥éè¿åå¤Botååºçå¯¹å±æ¶æ¯æ¥ä»£æ¿æå®å¯¹å±ç¼å·ã\n\nå¯¹å±ç¸å³æä»¤å¨å¯¹å±å®æè¶è¿24å°æ¶åéè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ãï¼`/
-å é¤å¯¹å±`é¤å¤ï¼è¯¥æä»¤éè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ï¼\n\næªå®æä¸æªè®¾ç½®è¿åº¦çå¯¹å±ä¼å¨åå»º24å°æ¶åèªå¨å é¤ãèµå­£ç»æåï¼æªå®æå¯¹å±ä¼èªå¨å é¤ï¼ææå·²å®æå¯¹å±åæ æ³åè¿è¡ä¿®æ¹ã\n\n###
-å¯¹å±æ¥è¯¢\n\n- `/æ¥è¯¢å¯¹å± [<ç¼å·>]`\n - å«åï¼`/å¯¹å±`\n- `/
-ä¸ªäººæè¿å¯¹å± [@<ç¨æ·>]`\n - å«åï¼`/æè¿å¯¹å±`\n- `/
-ç¾¤æè¿å¯¹å±`\n- `/ä¸ªäººæªå®æå¯¹å± [@<ç¨æ·>]`\n - å«åï¼`/
-æªå®æå¯¹å±`\n- `/ç¾¤æªå®æå¯¹å±`\n- `/å¯¼åºèµå­£å¯¹å± [<ä»£å·>]`\n
-- å«åï¼`/å¯¼åºå¯¹å±`\n- `/å¯¼åºææå¯¹å±`\n\n### èµå­£\n\n- `/
-æ¥è¯¢èµå­£ [<ä»£å·>]`\n - å«åï¼`/èµå­£`ï¼`/å½åèµå­£`\n- `/
-æ¥è¯¢ææèµå­£`\n - å«åï¼`/ææèµå­£`\n- `/æ°å»ºèµå­£`\n -
-å«åï¼`/æ°èµå­£`\n- `/å¼å¯èµå­£ [<ä»£å·>]`\n- `/ç»æèµå­£`\n- `/
-å é¤èµå­£ [<ä»£å·>]`\n\n### èµå­£æ¥è¯¢\n\n- `/æ¥è¯¢æ¦å`\n -
-å«åï¼`/æ¦å`\n- `/å¯¼åºæ¦å`\n- `/æ¥è¯¢PT [@<ç¨æ·>]`\n -
-å«åï¼`/PT`\n- `/è®¾ç½®PT  [@<ç¨æ·>]`\n - å«åï¼`/è®¾ç½®pt`\n\n###
-æ°æ®ç»è®¡\n\n- `/å¯¹ææ°æ®`\n- `/èµå­£å¯¹ææ°æ® [<èµå­£ä»£å·>]`\n-
-`/æè¿èµ°å¿ [@<ç¨æ·>]`\n - å«åï¼`/èµ°å¿`\n\nä¸èµå­£/
+Metadata-Version: 2.1 Name: nonebot-plugin-mahjong-scoreboard Version: 0.3.1
+Summary: æ¥éº»å¯åå¨ï¼NoneBotæä»¶ï¼ Home-page: https://github.com/
+ssttkkl/nonebot-plugin-mahjong-scoreboard License: MIT Author: ssttkkl Author-
+email: huang.wen.long@hotmail.com Requires-Python: >=3.9,<4.0 Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: aiosqlite (>=0.17,<0.19) Requires-Dist:
+cachetools (>=5.2.0,<6.0.0) Requires-Dist: nonebot-adapter-onebot
+(>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-
+file (>=0.1.4,<0.2.0) Requires-Dist: nonebot-plugin-sqlalchemy (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Requires-Dist:
+nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist: tzlocal (>=4.2,<5.0)
+Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-mahjong-
+scoreboard Description-Content-Type: text/plain
+                                   [nonebot]
+          nonebot-plugin-mahjong-scoreboard ============ _â¨ NoneBot
+                          æ¥éº»è®°åå¨æä»¶ â¨_
+                           [license] [pypi] [python]
+æ¯æééå¨ï¼[OneBot V11](https://onebot.adapters.nonebot.dev/
+) æ¯æé©±å¨å¨ï¼[FastAPI](https://v2.nonebot.dev/docs/tutorial/choose-
+driver) ## åè½
+ä¸ºç¾¤åæä¾æ¥éº»å¯¹å±åæ°è®°å½ãæ ¹æ®é©¬ç¹è¿è¡PTç²¾ç®ï¼ç»è®¡PTå¢åï¼æ¯æå¯¹å±ä¸æ¦åæ¥è¯¢ä¸å¯¼åºã
+PTç²¾ç®ç®æ³ä¸ºï¼ç¹æ°-è¿ç¹+é©¬ç¹ï¼/
+1000ï¼è¿ç¹åé©¬ç¹å¨åå»ºèµå­£æ¶è¿è¡è®¾ç½®ã ## å¸¸ç¨Workflow ###
+å¼å¯èµå­£ ``` /æ°å»ºèµå­£ ``` ### è®°å½ååºå¯¹å± ``` ä»»ä½äººï¼/
+æ°å»ºå¯¹å± A: /ç»ç® 25000 B: /ç»ç® 25000 C: /ç»ç® 25000 D: /ç»ç®
+25000 ``` ### è®°å½ä¸åºå¯¹å± ``` ä»»ä½äººï¼/æ°å»ºå¯¹å± åäººä¸ A: /
+ç»ç® 25000 B: /ç»ç® 25000 C: /ç»ç® 25000 D: /ç»ç® 25000 ``` ###
+è®°å½æªå®æå¯¹å± ``` ä»»ä½äººï¼/æ°å»ºå¯¹å± ä»»ä½äººï¼/
+è®¾ç½®å¯¹å±è¿åº¦ ä¸ä¸å±0æ¬åº A: /ç»ç® 25000 ä¸ B: /ç»ç® 25000 å
+C: /ç»ç® 25000 è¥¿ D: /ç»ç® 25000 å ``` ###
+å°æªå®æå¯¹å±è®¾ç½®ä¸ºå·²å®æ ``` ä»»ä½äººï¼/è®¾ç½®å¯¹å±è¿åº¦
+å¯¹å±23050701 å®æ ``` ### å é¤å¯¹å±
+ç¨æ·æ éæå¨å é¤éè¯¯åå»ºçå¯¹å±ãå½å¯¹å±æ°å»ºè¶è¿24hä»æªæåç»ç®æ¶ï¼å¯¹å±ä¼èªå¨å é¤ã
+å é¤å·²ç»ç®çå¯¹å±éè¦ç®¡çåæéã ``` /å é¤å¯¹å±
+å¯¹å±23050701 ``` ###
+ç»ç®åä¸ºå¯¹å±æå¨è®¾ç½®PTï¼å½èªå¨è®¡ç®çPTä¸æ­£ç¡®æ¶ï¼æèéè¦è¿è¡å¤ç½æ¶ï¼
+``` éè¦è®¾ç½®PTçäººï¼/è®¾ç½®å¯¹å±PT -52 æ ä»»ä½äººï¼/è®¾ç½®å¯¹å±PT
+@éè¦è®¾ç½®PTçäºº -52 ``` ## æä»¤ ### å¯¹å± - `/æ°å»ºå¯¹å±
+[åäººå|åäººä¸]` - å«åï¼`/æ°å¯¹å±` - `/ç»ç®å¯¹å± <æç»©>
+[å¯¹å±<ç¼å·>] [@<ç¨æ·>] [<èªé£>]` - å«åï¼`/ç»ç®` - `/
+æ¤éç»ç®å¯¹å± [å¯¹å±<ç¼å·>] [@<ç¨æ·>]` - å«åï¼`/æ¤éç»ç®` -
+`/è®¾ç½®å¯¹å±PT  [å¯¹å±<ç¼å·>] [@<ç¨æ·>]` - å«åï¼`/å¯¹å±PT` - `/
+å é¤å¯¹å± [å¯¹å±<ç¼å·>]` - `/è®¾ç½®å¯¹å±è¿åº¦ <ä¸/åxå±yæ¬åº æ
+å®æ> [å¯¹å±<ç¼å·>]` - å«åï¼`/å¯¹å±è¿åº¦` - `/è®¾ç½®å¯¹å±å¤æ³¨
+[å¯¹å±<ç¼å·>] <å¯¹å±å¤æ³¨>` - å«åï¼`/å¯¹å±å¤æ³¨`
+ä¸å¯¹å±ç¸å³çæä»¤å¯ä»¥çç¥å¯¹å±ç¼å·ï¼çç¥æ¶é»è®¤å¯¹æè¿æ°å»ºçå¯¹å±è¿è¡æä½ãä¹å¯ä»¥éè¿åå¤Botååºçå¯¹å±æ¶æ¯æ¥ä»£æ¿æå®å¯¹å±ç¼å·ã
+å¯¹å±ç¸å³æä»¤å¨å¯¹å±å®æè¶è¿24å°æ¶åéè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ãï¼`/
+å é¤å¯¹å±`é¤å¤ï¼è¯¥æä»¤éè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ï¼
+æªå®æä¸æªè®¾ç½®è¿åº¦çå¯¹å±ä¼å¨åå»º24å°æ¶åèªå¨å é¤ãèµå­£ç»æåï¼æªå®æå¯¹å±ä¼èªå¨å é¤ï¼ææå·²å®æå¯¹å±åæ æ³åè¿è¡ä¿®æ¹ã
+### å¯¹å±æ¥è¯¢ - `/æ¥è¯¢å¯¹å± [<ç¼å·>]` - å«åï¼`/å¯¹å±` - `/
+ä¸ªäººæè¿å¯¹å± [@<ç¨æ·>]` - å«åï¼`/æè¿å¯¹å±` - `/ç¾¤æè¿å¯¹å±`
+- `/ä¸ªäººæªå®æå¯¹å± [@<ç¨æ·>]` - å«åï¼`/æªå®æå¯¹å±` - `/
+ç¾¤æªå®æå¯¹å±` - `/å¯¼åºèµå­£å¯¹å± [<ä»£å·>]` - å«åï¼`/
+å¯¼åºå¯¹å±` - `/å¯¼åºææå¯¹å±` ### èµå­£ - `/æ¥è¯¢èµå­£ [<ä»£å·>]` -
+å«åï¼`/èµå­£`ï¼`/å½åèµå­£` - `/æ¥è¯¢ææèµå­£` - å«åï¼`/
+ææèµå­£` - `/æ°å»ºèµå­£` - å«åï¼`/æ°èµå­£` - `/å¼å¯èµå­£
+[<ä»£å·>]` - `/ç»æèµå­£` - `/å é¤èµå­£ [<ä»£å·>]` ### èµå­£æ¥è¯¢ -
+`/æ¥è¯¢æ¦å` - å«åï¼`/æ¦å` - `/å¯¼åºæ¦å` - `/æ¥è¯¢PT
+[@<ç¨æ·>]` - å«åï¼`/PT` - `/è®¾ç½®ç¨æ·PT  @<ç¨æ·>` - å«åï¼`/
+è®¾ç½®ç¨æ·pt`, `/è®¾ç½®PT`, `/è®¾ç½®pt` - `/éç½®ç¨æ·PT @<ç¨æ·>` -
+å«åï¼`/éç½®ç¨æ·pt`, `/éç½®PT`, `/éç½®pt` ### æ°æ®ç»è®¡ - `/
+å¯¹ææ°æ®` - `/èµå­£å¯¹ææ°æ® [<èµå­£ä»£å·>]` - `/æè¿èµ°å¿
+[@<ç¨æ·>]` - å«åï¼`/èµ°å¿` ä¸èµå­£/
 èµå­£PTç¸å³çæä»¤åå¯éè¿ç§è/
 ç¾¤èä¸¤ç§æ¹å¼ä½¿ç¨ãå½æªæå®åæ°æ¶è¿å¥é®ç­æ¨¡å¼ï¼åå¤`/
-q`å¯éåºé®ç­æ¨¡å¼ã\n\nä¸èµå­£/
-èµå­£PTç¸å³çæä»¤ï¼æ¥è¯¢ãå¯¼åºé¤å¤ï¼éè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ã\n\n##
-éç½®\n\n###
-mahjong_scoreboard_database_conn_url\n\næ°æ®åºè¿æ¥URLï¼å¿é¡»ä½¿ç¨å¼æ­¥SQLAlchemyé©±å¨å¨ã\n\né»è®¤å¼ï¼sqlite+aiosqlite:
-///mahjong_scoreboard.db\n\n###
-callback_host\n\nåè°HOSTï¼è¥ä¸ºéå®¹å¨ç¯å¢é¨ç½²ï¼go-
+q`å¯éåºé®ç­æ¨¡å¼ã ä¸èµå­£/
+èµå­£PTç¸å³çæä»¤ï¼æ¥è¯¢ãå¯¼åºé¤å¤ï¼éè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ã
+## éç½® ### mahjong_scoreboard_database_conn_url
+æ°æ®åºè¿æ¥URLï¼å¿é¡»ä½¿ç¨å¼æ­¥SQLAlchemyé©±å¨å¨ã
+é»è®¤å¼ï¼sqlite+aiosqlite:///mahjong_scoreboard.db ### callback_host
+åè°HOSTï¼è¥ä¸ºéå®¹å¨ç¯å¢é¨ç½²ï¼go-
 cqhttpä¸nonebotåè¿è¡å¨åä¸ç¯å¢ï¼åä¿æé»è®¤å¼ãè¥ä¸ºDockerç¯å¢é¨ç½²åè®¾ç½®ä¸ºDockerå®¹å¨åãç¨äºä¸ä¼ æä»¶æ¶è®©go-
-cqhttpä¸è½½æ¬æºæä»¶ã\n\né»è®¤å¼ï¼127.0.0.1\n\n###
-callback_port\n\nåè°ç«¯å£ï¼ä¿æé»è®¤å¼å³å¯ã\n\né»è®¤å¼ï¼ä¸PORTä¿æä¸è´å³å¯\n\n##
-å¨çº¿ä¹è®¨\n\nç¹å»è¯·ææä¸¤æmaimai\n\n![](https://github.com/ssttkkl/
-ssttkkl/blob/main/afdian-ssttkkl.jfif)\n\n\n\n## LICENSE\n\n> MIT License\n>\n>
-Copyright (c) 2022 ssttkkl\n>\n> Permission is hereby granted, free of charge,
-to any person obtaining a copy\n> of this software and associated documentation
-files (the "Software"), to deal\n> in the Software without restriction,
-including without limitation the rights\n> to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell\n> copies of the Software, and to
-permit persons to whom the Software is\n> furnished to do so, subject to the
-following conditions:\n>\n> The above copyright notice and this permission
-notice shall be included in all\n> copies or substantial portions of the
-Software.\n>\n> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR\n> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY,\n> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
-EVENT SHALL THE\n> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
-DAMAGES OR OTHER\n> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
-OTHERWISE, ARISING FROM,\n> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE
-USE OR OTHER DEALINGS IN THE\n> SOFTWARE.\n> \n', 'author': 'ssttkkl',
-'author_email': 'huang.wen.long@hotmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/ssttkkl/nonebot-plugin-
-mahjong-scoreboard', 'package_dir': package_dir, 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
+cqhttpä¸è½½æ¬æºæä»¶ã é»è®¤å¼ï¼127.0.0.1 ### callback_port
+åè°ç«¯å£ï¼ä¿æé»è®¤å¼å³å¯ã é»è®¤å¼ï¼ä¸PORTä¿æä¸è´å³å¯
+## å¨çº¿ä¹è®¨ ç¹å»è¯·ææä¸¤æmaimai ![](https://github.com/ssttkkl/
+ssttkkl/blob/main/afdian-ssttkkl.jfif)  ## LICENSE > MIT License > > Copyright
+(c) 2022 ssttkkl > > Permission is hereby granted, free of charge, to any
+person obtaining a copy > of this software and associated documentation files
+(the "Software"), to deal > in the Software without restriction, including
+without limitation the rights > to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell > copies of the Software, and to permit
+persons to whom the Software is > furnished to do so, subject to the following
+conditions: > > The above copyright notice and this permission notice shall be
+included in all > copies or substantial portions of the Software. > > THE
+SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR >
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, >
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE >
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER >
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, >
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE >
+SOFTWARE. >
```

