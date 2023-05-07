# Comparing `tmp/nonebot_plugin_mahjong_scoreboard-0.3.1.tar.gz` & `tmp/nonebot_plugin_mahjong_scoreboard-0.3.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mahjong_scoreboard-0.3.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_mahjong_scoreboard-0.3.1.post1.tar", max compression
```

## Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1.tar` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421764 nonebot_plugin_mahjong_scoreboard-0.3.1/LICENSE
--rw-r--r--   0        0        0      932 2023-05-07 02:57:41.868310 nonebot_plugin_mahjong_scoreboard-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6759 2023-05-07 02:56:55.737523 nonebot_plugin_mahjong_scoreboard-0.3.1/README.MD
--rw-r--r--   0        0        0     2090 2023-04-04 02:00:50.079979 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/__init__.py
--rw-r--r--   0        0        0      347 2023-03-13 11:15:04.245799 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/config.py
--rw-r--r--   0        0        0      287 2023-03-13 11:15:04.246316 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/__init__.py
--rw-r--r--   0        0        0      489 2022-10-29 10:31:10.715954 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/context.py
--rw-r--r--   0        0        0     3647 2023-03-01 06:19:33.483226 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py
--rw-r--r--   0        0        0     7291 2023-03-13 11:15:04.246837 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py
--rw-r--r--   0        0        0    14581 2023-03-13 11:15:04.247882 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py
--rw-r--r--   0        0        0     5417 2023-05-07 02:50:32.445789 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py
--rw-r--r--   0        0        0     7254 2023-03-13 11:15:04.249448 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/general_handlers.py
--rw-r--r--   0        0        0      439 2022-10-29 12:00:29.945522 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py
--rw-r--r--   0        0        0     1160 2023-03-01 06:35:10.159635 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_error_impl.py
--rw-r--r--   0        0        0      519 2022-10-25 08:26:38.853725 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_interruption_impl.py
--rw-r--r--   0        0        0     1437 2023-05-07 03:16:58.471265 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py
--rw-r--r--   0        0        0     2770 2023-03-13 11:15:04.250961 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py
--rw-r--r--   0        0        0     3722 2023-03-13 11:15:04.251961 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py
--rw-r--r--   0        0        0     2645 2023-05-07 03:16:58.467263 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_statistics_mapper.py
--rw-r--r--   0        0        0     2494 2023-03-13 11:15:04.252961 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py
--rw-r--r--   0        0        0     3086 2023-03-01 06:19:33.488463 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py
--rw-r--r--   0        0        0     3027 2023-03-13 11:15:04.253961 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py
--rw-r--r--   0        0        0    13761 2023-03-13 11:15:04.254961 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py
--rw-r--r--   0        0        0     2811 2023-03-13 11:15:04.255960 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py
--rw-r--r--   0        0        0     2807 2023-03-01 06:19:33.490557 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py
--rw-r--r--   0        0        0     5297 2023-05-07 02:54:53.398010 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py
--rw-r--r--   0        0        0     3427 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py
--rw-r--r--   0        0        0        0 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/__init__.py
--rw-r--r--   0        0        0     1022 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py
--rw-r--r--   0        0        0     2519 2023-03-13 11:15:04.258743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py
--rw-r--r--   0        0        0     1708 2023-03-13 11:15:04.258743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/send_messages.py
--rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228228 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/errors.py
--rw-r--r--   0        0        0        0 2022-10-11 14:30:16.137278 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py
--rw-r--r--   0        0        0      492 2022-10-25 11:55:32.743202 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/enums.py
--rw-r--r--   0        0        0      251 2023-05-07 03:08:43.903152 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/game_statistics.py
--rw-r--r--   0        0        0       39 2023-03-13 11:15:04.259743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/__init__.py
--rw-r--r--   0        0        0      129 2023-03-13 11:15:04.259743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/__init__.py
--rw-r--r--   0        0        0     2014 2023-03-13 13:49:53.073496 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/metainfo.py
--rw-r--r--   0        0        0      653 2023-03-13 11:15:04.261743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/__init__.py
--rw-r--r--   0        0        0      255 2023-03-13 11:15:04.261743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/v1_to_v2.py
--rw-r--r--   0        0        0      584 2023-04-04 02:00:50.080978 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/src.py
--rw-r--r--   0        0        0     3840 2023-03-13 11:15:04.263743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/game.py
--rw-r--r--   0        0        0      876 2023-03-13 11:15:04.263743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/group.py
--rw-r--r--   0        0        0     3819 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/season.py
--rw-r--r--   0        0        0        0 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/__init__.py
--rw-r--r--   0        0        0      522 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/userdict.py
--rw-r--r--   0        0        0      461 2023-03-13 11:15:04.265743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/user.py
--rw-r--r--   0        0        0        0 2022-10-11 14:02:12.038461 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/__init__.py
--rw-r--r--   0        0        0    19614 2023-05-07 03:19:06.560247 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py
--rw-r--r--   0        0        0     2196 2023-03-13 11:15:04.266743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py
--rw-r--r--   0        0        0     3736 2023-03-01 06:19:33.494591 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py
--rw-r--r--   0        0        0    10068 2023-03-13 13:34:40.919314 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py
--rw-r--r--   0        0        0      582 2023-03-01 06:19:33.495592 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py
--rw-r--r--   0        0        0        0 2022-10-25 10:53:45.022120 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/__init__.py
--rw-r--r--   0        0        0      288 2022-10-25 10:55:21.893872 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/date.py
--rw-r--r--   0        0        0     1240 2022-10-25 10:57:00.084086 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py
--rw-r--r--   0        0        0      101 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/nonebot.py
--rw-r--r--   0        0        0      482 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/rank.py
--rw-r--r--   0        0        0      256 2023-02-24 10:26:11.257181 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/upload_file.py
--rw-r--r--   0        0        0      761 2023-03-13 11:15:04.268743 nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py
--rw-r--r--   0        0        0     7618 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421764 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/LICENSE
+-rw-r--r--   0        0        0      938 2023-05-07 03:46:59.348863 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     6759 2023-05-07 03:20:47.530795 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/README.MD
+-rw-r--r--   0        0        0     2090 2023-04-04 02:00:50.079979 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/__init__.py
+-rw-r--r--   0        0        0      347 2023-03-13 11:15:04.245799 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/config.py
+-rw-r--r--   0        0        0      287 2023-03-13 11:15:04.246316 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/__init__.py
+-rw-r--r--   0        0        0      489 2022-10-29 10:31:10.715954 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/context.py
+-rw-r--r--   0        0        0     3647 2023-03-01 06:19:33.483226 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py
+-rw-r--r--   0        0        0     7291 2023-03-13 11:15:04.246837 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py
+-rw-r--r--   0        0        0    14581 2023-03-13 11:15:04.247882 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py
+-rw-r--r--   0        0        0     5417 2023-05-07 03:20:47.531830 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py
+-rw-r--r--   0        0        0     7254 2023-03-13 11:15:04.249448 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/general_handlers.py
+-rw-r--r--   0        0        0      439 2022-10-29 12:00:29.945522 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py
+-rw-r--r--   0        0        0     1160 2023-03-01 06:35:10.159635 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_error_impl.py
+-rw-r--r--   0        0        0      519 2022-10-25 08:26:38.853725 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_interruption_impl.py
+-rw-r--r--   0        0        0     1549 2023-05-07 03:44:28.905567 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py
+-rw-r--r--   0        0        0     2770 2023-03-13 11:15:04.250961 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py
+-rw-r--r--   0        0        0     3722 2023-03-13 11:15:04.251961 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py
+-rw-r--r--   0        0        0     2669 2023-05-07 03:45:01.376945 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_statistics_mapper.py
+-rw-r--r--   0        0        0     2494 2023-03-13 11:15:04.252961 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py
+-rw-r--r--   0        0        0     3086 2023-03-01 06:19:33.488463 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py
+-rw-r--r--   0        0        0     3027 2023-03-13 11:15:04.253961 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py
+-rw-r--r--   0        0        0    13761 2023-03-13 11:15:04.254961 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py
+-rw-r--r--   0        0        0     2811 2023-03-13 11:15:04.255960 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py
+-rw-r--r--   0        0        0     2807 2023-03-01 06:19:33.490557 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py
+-rw-r--r--   0        0        0     5297 2023-05-07 03:20:47.532347 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py
+-rw-r--r--   0        0        0     3427 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/__init__.py
+-rw-r--r--   0        0        0     1022 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py
+-rw-r--r--   0        0        0     2519 2023-03-13 11:15:04.258743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py
+-rw-r--r--   0        0        0     1708 2023-03-13 11:15:04.258743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/send_messages.py
+-rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228228 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/errors.py
+-rw-r--r--   0        0        0        0 2022-10-11 14:30:16.137278 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py
+-rw-r--r--   0        0        0      492 2022-10-25 11:55:32.743202 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/enums.py
+-rw-r--r--   0        0        0      251 2023-05-07 03:20:47.949666 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/game_statistics.py
+-rw-r--r--   0        0        0       39 2023-03-13 11:15:04.259743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/__init__.py
+-rw-r--r--   0        0        0      129 2023-03-13 11:15:04.259743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/__init__.py
+-rw-r--r--   0        0        0     2014 2023-03-13 13:49:53.073496 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/metainfo.py
+-rw-r--r--   0        0        0      653 2023-03-13 11:15:04.261743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/__init__.py
+-rw-r--r--   0        0        0      255 2023-03-13 11:15:04.261743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/v1_to_v2.py
+-rw-r--r--   0        0        0      584 2023-04-04 02:00:50.080978 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/src.py
+-rw-r--r--   0        0        0     3842 2023-05-07 03:44:12.878318 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/game.py
+-rw-r--r--   0        0        0      876 2023-03-13 11:15:04.263743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/group.py
+-rw-r--r--   0        0        0     3819 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/season.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/__init__.py
+-rw-r--r--   0        0        0      522 2023-03-13 11:15:04.264743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/userdict.py
+-rw-r--r--   0        0        0      461 2023-03-13 11:15:04.265743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/user.py
+-rw-r--r--   0        0        0        0 2022-10-11 14:02:12.038461 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/__init__.py
+-rw-r--r--   0        0        0    19271 2023-05-07 03:44:45.192491 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py
+-rw-r--r--   0        0        0     2196 2023-03-13 11:15:04.266743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py
+-rw-r--r--   0        0        0     3736 2023-03-01 06:19:33.494591 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py
+-rw-r--r--   0        0        0    10068 2023-03-13 13:34:40.919314 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py
+-rw-r--r--   0        0        0      582 2023-03-01 06:19:33.495592 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py
+-rw-r--r--   0        0        0        0 2022-10-25 10:53:45.022120 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/__init__.py
+-rw-r--r--   0        0        0      288 2022-10-25 10:55:21.893872 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/date.py
+-rw-r--r--   0        0        0     1240 2022-10-25 10:57:00.084086 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py
+-rw-r--r--   0        0        0      101 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/nonebot.py
+-rw-r--r--   0        0        0      482 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/rank.py
+-rw-r--r--   0        0        0      256 2023-02-24 10:26:11.257181 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/upload_file.py
+-rw-r--r--   0        0        0      761 2023-03-13 11:15:04.268743 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py
+-rw-r--r--   0        0        0     7624 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.3.1.post1/PKG-INFO
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/LICENSE` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/pyproject.toml` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mahjong-scoreboard"
-version = "0.3.1"
+version = "0.3.1.post1"
 description = "日麻寄分器（NoneBot插件）"
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.MD"
 license = "MIT"
 repository = "https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard"
 packages = [
     { include = "nonebot_plugin_mahjong_scoreboard", from = "src" },
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/README.MD` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/README.MD`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/general_handlers.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/general_handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_error_impl.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_error_impl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_interruption_impl.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/handle_interruption_impl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,13 +47,17 @@
 
 
 def percentile_str(x: float, ndigits: int = 2) -> str:
     return f'{round(x * 100, ndigits)}%'
 
 
 def map_point(raw_point: Union[int, float], scale: int = 0) -> str:
-    point_text = f"%.{-scale}f" % (raw_point * 10 ** scale)
-    if raw_point > 0:
+    return map_real_point(raw_point * 10 ** scale, scale)
+
+
+def map_real_point(point: Union[int, float], precision: int = 0) -> str:
+    point_text = f"%.{precision}f" % point
+    if point > 0:
         point_text = f'+{point_text}'
-    elif raw_point == 0:
+    elif point == 0:
         point_text = f'±{point_text}'
     return point_text
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_statistics_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_statistics_mapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import StringIO
 from typing import List, Tuple, Optional
 
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 
-from nonebot_plugin_mahjong_scoreboard.controller.mapper import digit_mapping, percentile_str
+from nonebot_plugin_mahjong_scoreboard.controller.mapper import digit_mapping, percentile_str, map_real_point
 from nonebot_plugin_mahjong_scoreboard.controller.mapper.season_user_point_mapper import map_point
 from nonebot_plugin_mahjong_scoreboard.model.game_statistics import GameStatistics
 from nonebot_plugin_mahjong_scoreboard.model.orm.game import GameRecordOrm, GameOrm
 from nonebot_plugin_mahjong_scoreboard.model.orm.group import GroupOrm
 from nonebot_plugin_mahjong_scoreboard.model.orm.season import SeasonOrm, \
     SeasonUserPointChangeLogOrm
 from nonebot_plugin_mahjong_scoreboard.model.orm.user import UserOrm
@@ -36,11 +36,11 @@
             sio.write(f"用户[{await get_user_nickname(user, group)}]的对战数据如下：\n")
 
         sio.write(f"  对局数：{game_statistics.total} （半庄：{game_statistics.total_south}、东风：{game_statistics.total_east}）\n")
         for i, rate in enumerate(game_statistics.rates):
             sio.write(f"  {digit_mapping[i + 1]}位率：{percentile_str(rate)}\n")
         sio.write(f"  平均顺位：{round(game_statistics.avg_rank, 2)}\n")
         if game_statistics.pt_expectation is not None:
-            sio.write(f"  PT期望：{map_point(game_statistics.pt_expectation)}\n")
+            sio.write(f"  PT期望：{map_real_point(game_statistics.pt_expectation, 2)}\n")
         sio.write(f"  被飞率：{percentile_str(game_statistics.flying_rate)}")
 
         return Message(MessageSegment.text(sio.getvalue().strip()))
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/send_messages.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/send_messages.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/metainfo.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/metainfo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/src.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/_data_source/src.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/game.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     # 真正PT=raw_point*10^point_scale，例如point_scale=0时缩放1x，point_scale=-1时缩放0.1x
     raw_point: Mapped[int] = mapped_column('point', default=0)  # pt
     point_scale: Mapped[int] = mapped_column(default=0)  # pt缩放比例
 
     @property
     def point(self) -> float:
-        return self.raw_point * 10 ** self.point_scale
+        return self.raw_point * (10 ** self.point_scale)
 
     rank: Mapped[Optional[int]] = mapped_column("rnk")  # 排名
 
 
 @data_source.registry.mapped
 class GameProgressOrm:
     __tablename__ = 'game_progresses'
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/group.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/season.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/season.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/userdict.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/model/orm/types/userdict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -500,44 +500,36 @@
         if g.player_and_wind == PlayerAndWind.four_men_south:
             total_south += 1
         elif g.player_and_wind == PlayerAndWind.four_men_east:
             total_east += 1
 
     cnt = [0, 0, 0, 0]
 
-    pt_south = 0.0
-    pt_east = 0.0
+    sum_point = 0.0
 
     flying = 0
 
     for g in games:
         for r in g.records:
             if r.user_id == user.id:
                 cnt[r.rank - 1] += 1
 
                 if r.score < 0:
                     flying += 1
 
-                if g.player_and_wind == PlayerAndWind.four_men_south:
-                    pt_south += r.point
-                elif g.player_and_wind == PlayerAndWind.four_men_east:
-                    pt_east += r.point
+                sum_point += r.point
 
                 break
 
     rates = list(map(lambda x: x / total, cnt))
 
     avg_rank = (cnt[0] * 1 + cnt[1] * 2 + cnt[2] * 3 + cnt[3] * 4) / total
 
     if season is not None:
-        pt_expectation = 0
-        if total_south:
-            pt_expectation += pt_south / total_south
-        if total_east:
-            pt_expectation += pt_east / total_east
+        pt_expectation = sum_point / total
     else:
         pt_expectation = None
 
     flying_rate = flying / total
 
     return GameStatistics(total, total_east, total_south, rates, avg_rank, pt_expectation, flying_rate)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.3.1/PKG-INFO` & `nonebot_plugin_mahjong_scoreboard-0.3.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mahjong-scoreboard
-Version: 0.3.1
+Version: 0.3.1.post1
 Summary: 日麻寄分器（NoneBot插件）
 Home-page: https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mahjong-scoreboard Version: 0.3.1
-Summary: æ¥éº»å¯åå¨ï¼NoneBotæä»¶ï¼ Home-page: https://github.com/
-ssttkkl/nonebot-plugin-mahjong-scoreboard License: MIT Author: ssttkkl Author-
-email: huang.wen.long@hotmail.com Requires-Python: >=3.9,<4.0 Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: aiosqlite (>=0.17,<0.19) Requires-Dist:
-cachetools (>=5.2.0,<6.0.0) Requires-Dist: nonebot-adapter-onebot
+Metadata-Version: 2.1 Name: nonebot-plugin-mahjong-scoreboard Version:
+0.3.1.post1 Summary: æ¥éº»å¯åå¨ï¼NoneBotæä»¶ï¼ Home-page: https://
+github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard License: MIT Author:
+ssttkkl Author-email: huang.wen.long@hotmail.com Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: aiosqlite (>=0.17,<0.19) Requires-
+Dist: cachetools (>=5.2.0,<6.0.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-
 file (>=0.1.4,<0.2.0) Requires-Dist: nonebot-plugin-sqlalchemy (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Requires-Dist:
 nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist: tzlocal (>=4.2,<5.0)
 Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-mahjong-
 scoreboard Description-Content-Type: text/plain
                                    [nonebot]
```

