# Comparing `tmp/zero_play-0.4.0.tar.gz` & `tmp/zero_play-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zero_play-0.4.0.tar", last modified: Sun Nov 15 20:09:48 2020, max compression
+gzip compressed data, was "zero_play-0.5.0.tar", last modified: Sat May  6 22:42:35 2023, max compression
```

## Comparing `zero_play-0.4.0.tar` & `zero_play-0.5.0.tar`

### file list

```diff
@@ -1,53 +1,154 @@
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 20:09:48.498360 zero_play-0.4.0/
--rw-rw-r--   0 don       (1000) don       (1000)     4356 2020-11-15 20:09:48.498360 zero_play-0.4.0/PKG-INFO
--rw-rw-r--   0 don       (1000) don       (1000)     3078 2020-09-18 18:20:00.000000 zero_play-0.4.0/README.md
--rw-rw-r--   0 don       (1000) don       (1000)       38 2020-11-15 20:09:48.498360 zero_play-0.4.0/setup.cfg
--rw-rw-r--   0 don       (1000) don       (1000)     2720 2020-11-11 21:36:04.000000 zero_play-0.4.0/setup.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 20:09:48.338362 zero_play-0.4.0/zero_play/
--rw-rw-r--   0 don       (1000) don       (1000)       22 2020-11-15 20:05:20.000000 zero_play-0.4.0/zero_play/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)     3133 2020-10-23 20:45:39.000000 zero_play-0.4.0/zero_play/about_dialog.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 20:09:48.382361 zero_play-0.4.0/zero_play/connect4/
--rw-rw-r--   0 don       (1000) don       (1000)        0 2020-07-19 17:01:24.000000 zero_play-0.4.0/zero_play/connect4/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)      770 2020-09-16 01:03:58.000000 zero_play-0.4.0/zero_play/connect4/display.py
--rw-rw-r--   0 don       (1000) don       (1000)     3018 2020-09-14 02:50:42.000000 zero_play-0.4.0/zero_play/connect4/game.py
--rw-rw-r--   0 don       (1000) don       (1000)     4877 2020-09-14 02:50:42.000000 zero_play-0.4.0/zero_play/connect4/neural_net.py
--rw-rw-r--   0 don       (1000) don       (1000)     5709 2020-10-23 21:16:35.000000 zero_play-0.4.0/zero_play/game_display.py
--rw-rw-r--   0 don       (1000) don       (1000)     8013 2020-11-14 17:25:01.000000 zero_play-0.4.0/zero_play/game_state.py
--rw-rw-r--   0 don       (1000) don       (1000)     5502 2020-10-13 18:22:24.000000 zero_play-0.4.0/zero_play/grid_controls_ui.py
--rw-rw-r--   0 don       (1000) don       (1000)    10387 2020-10-23 21:21:38.000000 zero_play-0.4.0/zero_play/grid_display.py
--rw-rw-r--   0 don       (1000) don       (1000)     1981 2020-11-15 01:45:25.000000 zero_play-0.4.0/zero_play/heuristic.py
--rw-rw-r--   0 don       (1000) don       (1000)     3476 2020-11-08 18:31:54.000000 zero_play-0.4.0/zero_play/log_display.py
--rw-rw-r--   0 don       (1000) don       (1000)    19394 2020-10-16 04:55:44.000000 zero_play-0.4.0/zero_play/main_window.py
--rw-rw-r--   0 don       (1000) don       (1000)    14358 2020-11-08 02:07:52.000000 zero_play-0.4.0/zero_play/mcts_player.py
--rw-rw-r--   0 don       (1000) don       (1000)     1543 2020-10-21 04:19:01.000000 zero_play-0.4.0/zero_play/mcts_worker.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 20:09:48.426361 zero_play-0.4.0/zero_play/othello/
--rw-rw-r--   0 don       (1000) don       (1000)        0 2020-07-19 17:01:24.000000 zero_play-0.4.0/zero_play/othello/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)     1443 2020-10-16 00:03:48.000000 zero_play-0.4.0/zero_play/othello/display.py
--rw-rw-r--   0 don       (1000) don       (1000)     5968 2020-09-15 00:21:59.000000 zero_play-0.4.0/zero_play/othello/game.py
--rw-rw-r--   0 don       (1000) don       (1000)    11718 2020-10-18 04:31:23.000000 zero_play-0.4.0/zero_play/pixmap_differ.py
--rw-rw-r--   0 don       (1000) don       (1000)     4120 2020-11-14 22:00:43.000000 zero_play-0.4.0/zero_play/play_controller.py
--rw-rw-r--   0 don       (1000) don       (1000)     1640 2020-09-14 02:50:42.000000 zero_play-0.4.0/zero_play/player.py
--rw-rw-r--   0 don       (1000) don       (1000)     1438 2020-11-15 05:43:08.000000 zero_play-0.4.0/zero_play/playout.py
--rw-rw-r--   0 don       (1000) don       (1000)      973 2020-08-27 00:02:36.000000 zero_play-0.4.0/zero_play/plot_canvas.py
--rw-rw-r--   0 don       (1000) don       (1000)      323 2020-08-27 00:11:38.000000 zero_play-0.4.0/zero_play/plot_canvas_dummy.py
--rw-rw-r--   0 don       (1000) don       (1000)     1269 2020-11-11 16:55:39.000000 zero_play-0.4.0/zero_play/plot_perf.py
--rw-rw-r--   0 don       (1000) don       (1000)      270 2020-09-15 23:42:30.000000 zero_play-0.4.0/zero_play/rules_formatter.py
--rw-rw-r--   0 don       (1000) don       (1000)     3222 2020-10-16 05:07:12.000000 zero_play-0.4.0/zero_play/scaled_label.py
--rw-rw-r--   0 don       (1000) don       (1000)     2317 2020-10-16 23:14:25.000000 zero_play-0.4.0/zero_play/scaled_radio_button.py
--rw-rw-r--   0 don       (1000) don       (1000)      704 2020-09-06 00:57:43.000000 zero_play-0.4.0/zero_play/strength_adjuster.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 20:09:48.478360 zero_play-0.4.0/zero_play/tictactoe/
--rw-rw-r--   0 don       (1000) don       (1000)        0 2020-07-19 17:01:24.000000 zero_play-0.4.0/zero_play/tictactoe/__init__.py
--rw-rw-r--   0 don       (1000) don       (1000)      475 2020-09-15 16:19:10.000000 zero_play-0.4.0/zero_play/tictactoe/display.py
--rw-rw-r--   0 don       (1000) don       (1000)     1509 2020-09-14 02:50:42.000000 zero_play-0.4.0/zero_play/tictactoe/state.py
--rw-rw-r--   0 don       (1000) don       (1000)     2781 2020-11-13 02:57:39.000000 zero_play-0.4.0/zero_play/zero_perf.py
--rw-rw-r--   0 don       (1000) don       (1000)    19384 2020-11-14 17:25:01.000000 zero_play-0.4.0/zero_play/zero_play.py
--rw-rw-r--   0 don       (1000) don       (1000)     6118 2020-09-27 00:55:29.000000 zero_play-0.4.0/zero_play/zero_play_images_rc.py
--rw-rw-r--   0 don       (1000) don       (1000)     1693 2020-09-16 23:49:36.000000 zero_play-0.4.0/zero_play/zero_play_rcc.py
--rw-rw-r--   0 don       (1000) don       (1000)     2818 2020-09-17 01:41:21.000000 zero_play-0.4.0/zero_play/zero_play_rules_rc.py
-drwxrwxr-x   0 don       (1000) don       (1000)        0 2020-11-15 20:09:48.362362 zero_play-0.4.0/zero_play.egg-info/
--rw-rw-r--   0 don       (1000) don       (1000)     4356 2020-11-15 20:09:47.000000 zero_play-0.4.0/zero_play.egg-info/PKG-INFO
--rw-rw-r--   0 don       (1000) don       (1000)     1226 2020-11-15 20:09:47.000000 zero_play-0.4.0/zero_play.egg-info/SOURCES.txt
--rw-rw-r--   0 don       (1000) don       (1000)        1 2020-11-15 20:09:47.000000 zero_play-0.4.0/zero_play.egg-info/dependency_links.txt
--rw-rw-r--   0 don       (1000) don       (1000)      554 2020-11-15 20:09:47.000000 zero_play-0.4.0/zero_play.egg-info/entry_points.txt
--rw-rw-r--   0 don       (1000) don       (1000)       83 2020-11-15 20:09:47.000000 zero_play-0.4.0/zero_play.egg-info/requires.txt
--rw-rw-r--   0 don       (1000) don       (1000)       10 2020-11-15 20:09:47.000000 zero_play-0.4.0/zero_play.egg-info/top_level.txt
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.581739 zero_play-0.5.0/
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.561739 zero_play-0.5.0/.github/
+-rw-rw-r--   0 don       (1000) don       (1000)      176 2023-04-29 01:27:40.000000 zero_play-0.5.0/.github/dependabot.yml
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.561739 zero_play-0.5.0/.github/workflows/
+-rw-rw-r--   0 don       (1000) don       (1000)     1493 2023-04-13 04:51:17.000000 zero_play-0.5.0/.github/workflows/py-build.yml
+-rw-rw-r--   0 don       (1000) don       (1000)     1283 2022-04-07 00:08:06.000000 zero_play-0.5.0/.gitignore
+-rw-rw-r--   0 don       (1000) don       (1000)     4735 2023-05-02 05:28:35.000000 zero_play-0.5.0/CONTRIBUTING.md
+-rw-rw-r--   0 don       (1000) don       (1000)     1067 2022-04-07 00:08:06.000000 zero_play-0.5.0/LICENSE
+-rw-rw-r--   0 don       (1000) don       (1000)     3817 2023-05-06 22:42:35.581739 zero_play-0.5.0/PKG-INFO
+-rw-rw-r--   0 don       (1000) don       (1000)      470 2023-04-29 01:27:40.000000 zero_play-0.5.0/Pipfile
+-rw-rw-r--   0 don       (1000) don       (1000)   123722 2023-04-29 01:27:40.000000 zero_play-0.5.0/Pipfile.lock
+-rw-rw-r--   0 don       (1000) don       (1000)     3117 2023-04-11 05:33:24.000000 zero_play-0.5.0/README.md
+-rw-rw-r--   0 don       (1000) don       (1000)     1999 2022-04-07 00:08:06.000000 zero_play-0.5.0/alembic.ini
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.561739 zero_play-0.5.0/data/
+-rw-rw-r--   0 don       (1000) don       (1000)       72 2022-04-07 00:08:06.000000 zero_play-0.5.0/data/README.md
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.561739 zero_play-0.5.0/docs/
+-rw-rw-r--   0 don       (1000) don       (1000)       86 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/Gemfile
+-rw-rw-r--   0 don       (1000) don       (1000)     7279 2023-04-13 02:57:50.000000 zero_play-0.5.0/docs/Gemfile.lock
+-rw-rw-r--   0 don       (1000) don       (1000)      236 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/_config.yml
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.561739 zero_play-0.5.0/docs/_data/
+-rw-rw-r--   0 don       (1000) don       (1000)      498 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/_data/navigation.yml
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.561739 zero_play-0.5.0/docs/_includes/
+-rw-rw-r--   0 don       (1000) don       (1000)      759 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/_includes/footer.html
+-rw-rw-r--   0 don       (1000) don       (1000)     2059 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/favicon.png
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.561739 zero_play-0.5.0/docs/images/
+-rw-rw-r--   0 don       (1000) don       (1000)    44705 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/images/index_hero.jpg
+-rw-rw-r--   0 don       (1000) don       (1000)    11901 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/images/screenshot.png
+-rw-rw-r--   0 don       (1000) don       (1000)     2595 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/index.md
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.561739 zero_play-0.5.0/docs/journal/
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.561739 zero_play-0.5.0/docs/journal/2018/
+-rw-rw-r--   0 don       (1000) don       (1000)    32682 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2018/connect-4-wins-mcts.png
+-rw-rw-r--   0 don       (1000) don       (1000)     1513 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2018.md
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.565739 zero_play-0.5.0/docs/journal/2019/
+-rw-rw-r--   0 don       (1000) don       (1000)    68906 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2019/connect4-128-win-rate.png
+-rw-rw-r--   0 don       (1000) don       (1000)    62744 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2019/connect4-512-win-rate.png
+-rw-rw-r--   0 don       (1000) don       (1000)    71336 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2019/connect4-general-nn.png
+-rw-rw-r--   0 don       (1000) don       (1000)    32538 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2019/connect4-win-rate.png
+-rw-rw-r--   0 don       (1000) don       (1000)    74867 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2019/connect4nn-win-rate.png
+-rw-rw-r--   0 don       (1000) don       (1000)    32082 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2019/spline-win-rate.png
+-rw-rw-r--   0 don       (1000) don       (1000)    32261 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2019/spline-wins.png
+-rw-rw-r--   0 don       (1000) don       (1000)    31196 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2019/tictactoe-win-rate.png
+-rw-rw-r--   0 don       (1000) don       (1000)    31010 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2019/tictactoe-wins.png
+-rw-rw-r--   0 don       (1000) don       (1000)     5706 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2019.md
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.565739 zero_play-0.5.0/docs/journal/2020/
+-rw-rw-r--   0 don       (1000) don       (1000)     8520 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2020/multiprocessing_times.csv
+-rw-rw-r--   0 don       (1000) don       (1000)    69617 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/2020/multiprocessing_times.png
+-rw-rw-r--   0 don       (1000) don       (1000)     2682 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/journal/index.md
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.569739 zero_play-0.5.0/docs/rules/
+-rw-rw-r--   0 don       (1000) don       (1000)      548 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/rules/connect4.md
+-rw-rw-r--   0 don       (1000) don       (1000)     1676 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/rules/connect4.png
+-rw-rw-r--   0 don       (1000) don       (1000)      488 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/rules/tictactoe.md
+-rw-rw-r--   0 don       (1000) don       (1000)     2178 2022-04-07 00:08:06.000000 zero_play-0.5.0/docs/rules/tictactoe.png
+-rw-rw-r--   0 don       (1000) don       (1000)      111 2022-04-07 05:18:53.000000 zero_play-0.5.0/mypy.ini
+-rw-rw-r--   0 don       (1000) don       (1000)       38 2023-05-06 22:42:35.581739 zero_play-0.5.0/setup.cfg
+-rw-rw-r--   0 don       (1000) don       (1000)     2898 2023-04-29 01:27:40.000000 zero_play-0.5.0/setup.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.569739 zero_play-0.5.0/tests/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2023-04-29 15:23:35.000000 zero_play-0.5.0/tests/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)      883 2023-04-30 14:49:04.000000 zero_play-0.5.0/tests/conftest.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.573739 zero_play-0.5.0/tests/connect4/
+-rw-rw-r--   0 don       (1000) don       (1000)     2070 2023-04-29 01:27:40.000000 zero_play-0.5.0/tests/connect4/test_connect4_display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     7388 2022-04-07 00:08:06.000000 zero_play-0.5.0/tests/connect4/test_connect4_game.py
+-rw-rw-r--   0 don       (1000) don       (1000)      863 2022-04-07 00:08:06.000000 zero_play-0.5.0/tests/connect4/test_connect4_neural_net.py
+-rw-rw-r--   0 don       (1000) don       (1000)     5708 2022-04-07 00:08:06.000000 zero_play-0.5.0/tests/connect4/training_data.json
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.573739 zero_play-0.5.0/tests/othello/
+-rw-rw-r--   0 don       (1000) don       (1000)     2549 2023-04-29 01:27:40.000000 zero_play-0.5.0/tests/othello/test_othello_display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     9124 2022-04-07 00:08:06.000000 zero_play-0.5.0/tests/othello/test_othello_game.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.573739 zero_play-0.5.0/tests/pixmap_diffs/
+-rw-rw-r--   0 don       (1000) don       (1000)       51 2022-04-07 00:08:06.000000 zero_play-0.5.0/tests/pixmap_diffs/README.md
+-rw-rw-r--   0 don       (1000) don       (1000)     4460 2022-04-07 00:08:06.000000 zero_play-0.5.0/tests/test_log_display.py
+-rw-rw-r--   0 don       (1000) don       (1000)    11031 2022-04-07 00:08:06.000000 zero_play-0.5.0/tests/test_mcts_player.py
+-rw-rw-r--   0 don       (1000) don       (1000)     2052 2023-04-29 18:20:59.000000 zero_play-0.5.0/tests/test_pixmap_differ.py
+-rw-rw-r--   0 don       (1000) don       (1000)     5181 2022-04-07 00:08:06.000000 zero_play-0.5.0/tests/test_play_controller.py
+-rw-rw-r--   0 don       (1000) don       (1000)     4125 2022-04-07 00:08:06.000000 zero_play-0.5.0/tests/test_playout.py
+-rw-rw-r--   0 don       (1000) don       (1000)      489 2022-04-07 00:08:06.000000 zero_play-0.5.0/tests/test_rules_formatter.py
+-rw-rw-r--   0 don       (1000) don       (1000)     6395 2023-04-29 01:27:40.000000 zero_play-0.5.0/tests/test_scaled_label.py
+-rw-rw-r--   0 don       (1000) don       (1000)     5334 2023-04-29 01:27:40.000000 zero_play-0.5.0/tests/test_scaled_radio_button.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1518 2022-04-07 00:08:06.000000 zero_play-0.5.0/tests/test_strength_adjuster.py
+-rw-rw-r--   0 don       (1000) don       (1000)     2468 2023-04-29 01:27:40.000000 zero_play-0.5.0/tests/test_strength_history_plot.py
+-rw-rw-r--   0 don       (1000) don       (1000)     8226 2023-04-30 15:10:26.000000 zero_play-0.5.0/tests/test_strength_plot.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.573739 zero_play-0.5.0/tests/tictactoe/
+-rw-rw-r--   0 don       (1000) don       (1000)    10276 2023-05-02 05:21:33.000000 zero_play-0.5.0/tests/tictactoe/test_tictactoe_display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     5469 2022-04-07 00:08:06.000000 zero_play-0.5.0/tests/tictactoe/test_tictactoe_game.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.577739 zero_play-0.5.0/zero_play/
+-rw-rw-r--   0 don       (1000) don       (1000)       22 2023-05-06 22:41:32.000000 zero_play-0.5.0/zero_play/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)     3313 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/about_dialog.py
+-rw-rw-r--   0 don       (1000) don       (1000)     2708 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/about_dialog.ui
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.577739 zero_play-0.5.0/zero_play/connect4/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/connect4/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)      772 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/connect4/display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     3032 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/connect4/game.py
+-rw-rw-r--   0 don       (1000) don       (1000)     4877 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/connect4/neural_net.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.577739 zero_play-0.5.0/zero_play/db/
+-rw-rw-r--   0 don       (1000) don       (1000)       38 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/db/README
+-rw-rw-r--   0 don       (1000) don       (1000)     2260 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/db/env.py
+-rw-rw-r--   0 don       (1000) don       (1000)      494 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/db/script.py.mako
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.581739 zero_play-0.5.0/zero_play/db/versions/
+-rw-rw-r--   0 don       (1000) don       (1000)     2374 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/db/versions/62b4dd973a0f_first_tables.py
+-rw-rw-r--   0 don       (1000) don       (1000)     3186 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/diagram_writer.py
+-rw-rw-r--   0 don       (1000) don       (1000)     5657 2023-05-02 05:38:32.000000 zero_play-0.5.0/zero_play/game_display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     7978 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/game_state.py
+-rw-rw-r--   0 don       (1000) don       (1000)     5628 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/grid_controls_ui.py
+-rw-rw-r--   0 don       (1000) don       (1000)     4486 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/grid_controls_ui.ui
+-rw-rw-r--   0 don       (1000) don       (1000)    10395 2023-05-02 05:38:32.000000 zero_play-0.5.0/zero_play/grid_display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1981 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/heuristic.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1539 2023-04-29 18:24:35.000000 zero_play-0.5.0/zero_play/live_qpainter.py
+-rw-rw-r--   0 don       (1000) don       (1000)     3484 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/log_display.py
+-rw-rw-r--   0 don       (1000) don       (1000)    24887 2023-04-29 13:57:22.000000 zero_play-0.5.0/zero_play/main_window.py
+-rw-rw-r--   0 don       (1000) don       (1000)    19162 2023-04-29 13:56:47.000000 zero_play-0.5.0/zero_play/main_window.ui
+-rw-rw-r--   0 don       (1000) don       (1000)    14646 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/mcts_player.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1550 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/mcts_worker.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.581739 zero_play-0.5.0/zero_play/models/
+-rw-rw-r--   0 don       (1000) don       (1000)      274 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/models/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)      900 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/models/game.py
+-rw-rw-r--   0 don       (1000) don       (1000)      925 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/models/match.py
+-rw-rw-r--   0 don       (1000) don       (1000)      701 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/models/match_note.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1005 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/models/match_player.py
+-rw-rw-r--   0 don       (1000) don       (1000)      601 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/models/player.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.581739 zero_play-0.5.0/zero_play/othello/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/othello/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1443 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/othello/display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     5982 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/othello/game.py
+-rw-rw-r--   0 don       (1000) don       (1000)     5090 2023-04-30 02:47:06.000000 zero_play-0.5.0/zero_play/pixmap_differ.py
+-rw-rw-r--   0 don       (1000) don       (1000)     4124 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/play_controller.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1647 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/player.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1438 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/playout.py
+-rw-rw-r--   0 don       (1000) don       (1000)      765 2023-04-30 15:15:29.000000 zero_play-0.5.0/zero_play/plot_canvas.py
+-rw-rw-r--   0 don       (1000) don       (1000)      432 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/plot_canvas_dummy.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1269 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/plot_perf.py
+-rw-rw-r--   0 don       (1000) don       (1000)     3520 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/plot_strengths.py
+-rw-rw-r--   0 don       (1000) don       (1000)      687 2023-05-02 05:41:20.000000 zero_play-0.5.0/zero_play/process_display.py
+-rw-rw-r--   0 don       (1000) don       (1000)      270 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/rules_formatter.py
+-rw-rw-r--   0 don       (1000) don       (1000)     3439 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/scaled_label.py
+-rw-rw-r--   0 don       (1000) don       (1000)     2534 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/scaled_radio_button.py
+-rw-rw-r--   0 don       (1000) don       (1000)      704 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/strength_adjuster.py
+-rw-rw-r--   0 don       (1000) don       (1000)     2155 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/strength_history_plot.py
+-rw-rw-r--   0 don       (1000) don       (1000)    20287 2023-04-30 15:18:22.000000 zero_play-0.5.0/zero_play/strength_plot.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.581739 zero_play-0.5.0/zero_play/tictactoe/
+-rw-rw-r--   0 don       (1000) don       (1000)        0 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/tictactoe/__init__.py
+-rw-rw-r--   0 don       (1000) don       (1000)      477 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/tictactoe/display.py
+-rw-rw-r--   0 don       (1000) don       (1000)     1523 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/tictactoe/state.py
+-rw-rw-r--   0 don       (1000) don       (1000)     2789 2023-04-29 01:27:40.000000 zero_play-0.5.0/zero_play/zero_perf.py
+-rw-rw-r--   0 don       (1000) don       (1000)    27647 2023-04-29 14:09:44.000000 zero_play-0.5.0/zero_play/zero_play.py
+-rw-rw-r--   0 don       (1000) don       (1000)     6118 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play/zero_play_images_rc.py
+-rw-rw-r--   0 don       (1000) don       (1000)     2907 2023-05-02 05:28:35.000000 zero_play-0.5.0/zero_play/zero_play_rcc.py
+-rw-rw-r--   0 don       (1000) don       (1000)    15017 2023-05-02 05:29:19.000000 zero_play-0.5.0/zero_play/zero_play_rules_rc.py
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.577739 zero_play-0.5.0/zero_play.egg-info/
+-rw-rw-r--   0 don       (1000) don       (1000)     3817 2023-05-06 22:42:35.000000 zero_play-0.5.0/zero_play.egg-info/PKG-INFO
+-rw-rw-r--   0 don       (1000) don       (1000)     3478 2023-05-06 22:42:35.000000 zero_play-0.5.0/zero_play.egg-info/SOURCES.txt
+-rw-rw-r--   0 don       (1000) don       (1000)        1 2023-05-06 22:42:35.000000 zero_play-0.5.0/zero_play.egg-info/dependency_links.txt
+-rw-rw-r--   0 don       (1000) don       (1000)      553 2023-05-06 22:42:35.000000 zero_play-0.5.0/zero_play.egg-info/entry_points.txt
+-rw-rw-r--   0 don       (1000) don       (1000)      108 2023-05-06 22:42:35.000000 zero_play-0.5.0/zero_play.egg-info/requires.txt
+-rw-rw-r--   0 don       (1000) don       (1000)       16 2023-05-06 22:42:35.000000 zero_play-0.5.0/zero_play.egg-info/top_level.txt
+drwxrwxr-x   0 don       (1000) don       (1000)        0 2023-05-06 22:42:35.581739 zero_play-0.5.0/zero_play_images/
+-rw-rw-r--   0 don       (1000) don       (1000)     1496 2022-04-07 00:08:06.000000 zero_play-0.5.0/zero_play_images/main_icon.png
```

### Comparing `zero_play-0.4.0/PKG-INFO` & `zero_play-0.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,88 @@
 Metadata-Version: 2.1
 Name: zero_play
-Version: 0.4.0
+Version: 0.5.0
 Summary: Teach a computer to play any game
 Home-page: https://donkirkby.github.io/zero-play/
 Author: Don Kirkby
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/donkirkby/zero-play/issues
 Project-URL: Source, https://github.com/donkirkby/zero-play
-Description: # Zero Play [![Build Badge]][build] [![Coverage Badge]][codecov] [![PyPI Badge]][pypi]
-        ### Teach a computer to play any game
-        
-        [Build Badge]: https://travis-ci.org/donkirkby/zero-play.svg?branch=master
-        [build]: https://travis-ci.org/donkirkby/zero-play
-        [Coverage Badge]: https://codecov.io/github/donkirkby/zero-play/coverage.svg?branch=master
-        [codecov]: https://codecov.io/github/donkirkby/zero-play?branch=master
-        [PyPI Badge]: https://badge.fury.io/py/zero-play.svg
-        [pypi]: https://badge.fury.io/py/zero-play
-        [journal]: docs/journal
-        [screenshot]: https://donkirkby.github.io/zero-play/images/screenshot.png
-        
-        The zero play library is based on the ideas in the [AlphaGo Zero paper] and the
-        example Python code in the [alpha-zero-general project]. The goal of this
-        project is to make a reusable Python library that other projects can build on
-        to make powerful computer opponents for many different board games. An example
-        project that uses this library is [Shibumi Games].
-        
-        It includes a graphical display that you can use to play against the computer
-        opponent or another human.
-        
-        ![screenshot]
-        
-        [AlphaGo Zero paper]: https://deepmind.com/blog/alphago-zero-learning-scratch/
-        [alpha-zero-general project]: https://github.com/suragnair/alpha-zero-general
-        [Shibumi Games]: https://donkirkby.github.io/shibumi-games/
-        
-        ## Installing Zero Play
-        Even though Zero Play has a graphical display, it is a regular Python package,
-        so you can install it with `pip install zero-play`. If you haven't installed
-        Python packages before, read Brett Cannon's [quick-and-dirty guide].
-        
-        Then run it with the `zero_play` command.
-        
-        The default installation generates some errors about `bdist_wheel` that don't
-        seem to actually cause any problems. You can either ignore them, or install
-        `wheel` before installing Zero Play.
-        
-            pip install wheel
-            pip install zero-play
-            zero_play
-        
-        Known bug on Ubuntu 20.04:
-        
-        > qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though
-        > it was found.
-        
-        This is a [PySide2 bug] that is missing some dependencies. You can work around
-        it by installing those dependencies like this:
-        
-            sudo apt install libxcb-xinerama0
-        
-        [quick-and-dirty guide]: https://snarky.ca/a-quick-and-dirty-guide-on-how-to-install-packages-for-python/
-        [PySide2 bug]: https://bugreports.qt.io/browse/QTBUG-84749
-        
-        ## More Information
-        If you'd like to help out with the project, or add your own games, see the
-        `CONTRIBUTING.md` file in the source code. For all the details, look through the
-        design [journal] for the project.
-        
-        ## Related Projects
-        Here are some similar projects for inspiration or collaboration:
-        
-        * I already mentioned the [alpha-zero-general project]. It was a big inspiration, but I'm trying to build something
-            that's easier to add new games to, or use as a library within another project.
-        * [Galvanise] looks interesting. It's a mix of Python and C++, using Tensorflow. As of 2020, it looks like a single
-            developer, without much documentation. The games are defined with GDL, not Python code.
-        
-        [Galvanise]: https://github.com/richemslie/galvanise_zero
-        
 Keywords: boardgames alphazero machine learning mcts
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: ml
 Provides-Extra: ml-gpu
+License-File: LICENSE
+
+# Zero Play [![Build Badge]][build] [![Coverage Badge]][codecov] [![PyPI Badge]][pypi]
+### Teach a computer to play any game
+
+[Build Badge]: https://github.com/donkirkby/zero-play/actions/workflows/py-build.yml/badge.svg?branch=master
+[build]: https://github.com/donkirkby/zero-play/actions
+[Coverage Badge]: https://codecov.io/github/donkirkby/zero-play/coverage.svg?branch=master
+[codecov]: https://codecov.io/github/donkirkby/zero-play?branch=master
+[PyPI Badge]: https://badge.fury.io/py/zero-play.svg
+[pypi]: https://badge.fury.io/py/zero-play
+[journal]: docs/journal
+[screenshot]: https://donkirkby.github.io/zero-play/images/screenshot.png
+
+The zero play library is based on the ideas in the [AlphaGo Zero paper] and the
+example Python code in the [alpha-zero-general project]. The goal of this
+project is to make a reusable Python library that other projects can build on
+to make powerful computer opponents for many different board games. An example
+project that uses this library is [Shibumi Games].
+
+It includes a graphical display that you can use to play against the computer
+opponent or another human.
+
+![screenshot]
+
+[AlphaGo Zero paper]: https://deepmind.com/blog/alphago-zero-learning-scratch/
+[alpha-zero-general project]: https://github.com/suragnair/alpha-zero-general
+[Shibumi Games]: https://donkirkby.github.io/shibumi-games/
+
+## Installing Zero Play
+Even though Zero Play has a graphical display, it is a regular Python package,
+so you can install it with `pip install zero-play`. If you haven't installed
+Python packages before, read Brett Cannon's [quick-and-dirty guide].
+
+Then run it with the `zero_play` command.
+
+The default installation generates some errors about `bdist_wheel` that don't
+seem to actually cause any problems. You can either ignore them, or install
+`wheel` before installing Zero Play.
+
+    pip install wheel
+    pip install zero-play
+    zero_play
+
+Known bug on Ubuntu 20.04:
+
+> qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though
+> it was found.
+
+This is a [PySide2 bug] that is missing some dependencies. You can work around
+it by installing those dependencies like this:
+
+    sudo apt install libxcb-xinerama0
+
+[quick-and-dirty guide]: https://snarky.ca/a-quick-and-dirty-guide-on-how-to-install-packages-for-python/
+[PySide2 bug]: https://bugreports.qt.io/browse/QTBUG-84749
+
+## More Information
+If you'd like to help out with the project, or add your own games, see the
+`CONTRIBUTING.md` file in the source code. For all the details, look through the
+design [journal] for the project.
+
+## Related Projects
+Here are some similar projects for inspiration or collaboration:
+
+* I already mentioned the [alpha-zero-general project]. It was a big inspiration, but I'm trying to build something
+    that's easier to add new games to, or use as a library within another project.
+* [Galvanise] looks interesting. It's a mix of Python and C++, using Tensorflow. As of 2020, it looks like a single
+    developer, without much documentation. The games are defined with GDL, not Python code.
+
+[Galvanise]: https://github.com/richemslie/galvanise_zero
```

### Comparing `zero_play-0.4.0/README.md` & `zero_play-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Zero Play [![Build Badge]][build] [![Coverage Badge]][codecov] [![PyPI Badge]][pypi]
 ### Teach a computer to play any game
 
-[Build Badge]: https://travis-ci.org/donkirkby/zero-play.svg?branch=master
-[build]: https://travis-ci.org/donkirkby/zero-play
+[Build Badge]: https://github.com/donkirkby/zero-play/actions/workflows/py-build.yml/badge.svg?branch=master
+[build]: https://github.com/donkirkby/zero-play/actions
 [Coverage Badge]: https://codecov.io/github/donkirkby/zero-play/coverage.svg?branch=master
 [codecov]: https://codecov.io/github/donkirkby/zero-play?branch=master
 [PyPI Badge]: https://badge.fury.io/py/zero-play.svg
 [pypi]: https://badge.fury.io/py/zero-play
 [journal]: docs/journal
 [screenshot]: https://donkirkby.github.io/zero-play/images/screenshot.png
```

### Comparing `zero_play-0.4.0/setup.py` & `zero_play-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,21 @@
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Developers',
           'Topic :: Games/Entertainment :: Board Games',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3.8'],
       keywords='boardgames alphazero machine learning mcts',
       packages=setuptools.find_packages(),
-      install_requires=['numpy<1.19.0', 'matplotlib', 'PySide2', 'markdown'],
+      install_requires=['numpy',
+                        'matplotlib',
+                        'PySide6',
+                        'markdown',
+                        'space-tracer',
+                        'sqlalchemy',
+                        'alembic'],
       extras_require={'ml': ['tensorflow'],
                       'ml-gpu': ['tensorflow-gpu']},
       entry_points={
           'gui_scripts': ['zero_play=zero_play.zero_play:main'],
           'console_scripts': ['zero_play_rcc=zero_play.zero_play_rcc:main',
                               'zero_perf=zero_play.zero_perf:main'],
           # The game_display entry point lets you add screens for new games.
```

### Comparing `zero_play-0.4.0/zero_play/about_dialog.py` & `zero_play-0.5.0/zero_play/about_dialog.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'about_dialog.ui'
 ##
-## Created by: Qt User Interface Compiler version 5.15.0
+## Created by: Qt User Interface Compiler version 6.2.1
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
-from PySide2.QtCore import (QCoreApplication, QDate, QDateTime, QMetaObject,
-    QObject, QPoint, QRect, QSize, QTime, QUrl, Qt)
-from PySide2.QtGui import (QBrush, QColor, QConicalGradient, QCursor, QFont,
-    QFontDatabase, QIcon, QKeySequence, QLinearGradient, QPalette, QPainter,
-    QPixmap, QRadialGradient)
-from PySide2.QtWidgets import *
-
+from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
+    QMetaObject, QObject, QPoint, QRect,
+    QSize, QTime, QUrl, Qt)
+from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
+    QFont, QFontDatabase, QGradient, QIcon,
+    QImage, QKeySequence, QLinearGradient, QPainter,
+    QPalette, QPixmap, QRadialGradient, QTransform)
+from PySide6.QtWidgets import (QAbstractButton, QApplication, QDialog, QDialogButtonBox,
+    QGridLayout, QLabel, QScrollArea, QSizePolicy,
+    QVBoxLayout, QWidget)
 
 class Ui_Dialog(object):
     def setupUi(self, Dialog):
         if not Dialog.objectName():
             Dialog.setObjectName(u"Dialog")
         Dialog.resize(500, 400)
         Dialog.setSizeGripEnabled(False)
```

### Comparing `zero_play-0.4.0/zero_play/connect4/display.py` & `zero_play-0.5.0/zero_play/connect4/display.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 
 from zero_play.connect4.game import Connect4State
 from zero_play.grid_display import GridDisplay, GraphicsPieceItem
 
 
 class Connect4Display(GridDisplay):
-    rules_path = ':/zero_play_rules/connect4.md'
+    rules_path = ':/zero_play_rules/connect4.html'
 
     def __init__(self):
         super().__init__(Connect4State())
 
     def calculate_move(self, row, column):
         return column
```

### Comparing `zero_play-0.4.0/zero_play/connect4/game.py` & `zero_play-0.5.0/zero_play/connect4/game.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from zero_play.game_state import GridGameState
 
 
 class Connect4State(GridGameState):
     game_name = 'Connect 4'
 
     def __init__(self,
-                 text: str = None,
+                 text: str | None = None,
                  board_height: int = 6,
                  board_width: int = 7,
-                 spaces: np.ndarray = None):
+                 spaces: np.ndarray | None = None):
         if text is None:
             lines = None
         else:
             lines = text.splitlines()
             if len(lines) == board_height+1:
                 # Trim off coordinates.
                 lines = lines[1:]
```

### Comparing `zero_play-0.4.0/zero_play/connect4/neural_net.py` & `zero_play-0.5.0/zero_play/connect4/neural_net.py`

 * *Files identical despite different names*

### Comparing `zero_play-0.4.0/zero_play/game_display.py` & `zero_play-0.5.0/zero_play/game_display.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 from abc import abstractmethod
 import typing
 
 import numpy as np
-from PySide2.QtCore import Signal, QThread, QSize, Slot
-from PySide2.QtGui import QResizeEvent
-from PySide2.QtWidgets import QGraphicsSimpleTextItem, QSizePolicy, QWidget
+from PySide6.QtCore import Signal, QThread, QSize, Slot
+from PySide6.QtGui import QResizeEvent
+from PySide6.QtWidgets import QGraphicsSimpleTextItem
 
 from zero_play.game_state import GameState
 from zero_play.log_display import LogDisplay
 from zero_play.mcts_player import MctsPlayer
 from zero_play.mcts_worker import MctsWorker
+from zero_play.process_display import ProcessDisplay
 
 
-class GameDisplay(QWidget):
-    default_font = 'Sans Serif,9,-1,5,50,0,0,0,0,0'
+class GameDisplay(ProcessDisplay):
     rules_path: typing.Optional[str] = None
 
     move_needed = Signal(int, np.ndarray)  # active_player, board
     move_made = Signal(np.ndarray)  # board
     game_ended = Signal(np.ndarray)  # final_board
 
     def __init__(self, start_state: GameState):
         super().__init__()
         self.start_state = start_state
         self.mcts_workers: typing.Dict[int, MctsWorker] = {}
-        self.worker_thread: typing.Optional[QThread] = None
         self.current_state = self.start_state
         self.valid_moves = self.start_state.get_valid_moves()
         self._show_coordinates = False
         self.log_display = LogDisplay()
-        self.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         self.is_reviewing = False
 
     @property
     def show_coordinates(self):
         return self._show_coordinates
 
     @show_coordinates.setter
     def show_coordinates(self, value):
         self._show_coordinates = value
+        # noinspection PyUnresolvedReferences
         scene = self.scene()
         size = QSize(scene.width(), scene.height())
         self.resizeEvent(QResizeEvent(size, size))
 
     @property
     def mcts_players(self):
         return [worker.player for worker in self.mcts_workers.values()]
@@ -54,24 +53,30 @@
         self.log_display = LogDisplay()
         self.mcts_workers = {player.player_number: MctsWorker(player)
                              for player in players}
         if not self.mcts_workers:
             self.worker_thread = None
         else:
             self.worker_thread = QThread()
+            self.worker_thread.finished.connect(  # type: ignore
+                self.worker_thread.deleteLater)
             for worker in self.mcts_workers.values():
                 worker.move_chosen.connect(self.make_move)  # type: ignore
                 worker.move_analysed.connect(self.analyse_move)  # type: ignore
-                # noinspection PyUnresolvedReferences
                 self.move_needed.connect(worker.choose_move)  # type: ignore
-                # noinspection PyUnresolvedReferences
                 self.move_made.connect(worker.analyse_move)  # type: ignore
                 worker.moveToThread(self.worker_thread)
             self.worker_thread.start()
 
+    def get_player(self, player_number: int) -> typing.Optional[MctsPlayer]:
+        worker = self.mcts_workers.get(player_number)
+        if worker:
+            return worker.player
+        return None
+
     @abstractmethod
     def update_board(self, board: GameState):
         """ Update self.scene, based on the state in board.
 
         It's probably also helpful to override resizeEvent().
 
         :param board: the state of the game to display.
@@ -135,21 +140,14 @@
     def request_move(self):
         if self.current_state.is_ended():
             return
         player = self.current_state.get_active_player()
         # noinspection PyUnresolvedReferences
         self.move_needed.emit(player, self.current_state)
 
-    def close(self):
-        self.stop_workers()
-
-    def stop_workers(self):
-        if self.worker_thread is not None:
-            self.worker_thread.quit()
-
     def can_move(self):
         if self.is_reviewing:
             return False
         return not self.current_state.get_active_player() in self.mcts_workers
 
 
 def center_text_item(item: QGraphicsSimpleTextItem, x: float, y: float):
```

### Comparing `zero_play-0.4.0/zero_play/game_state.py` & `zero_play-0.5.0/zero_play/game_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,14 +55,17 @@
         """ Create human-readable display text for the given move.
 
         :param move: the move to describe.
         :return: display text. Typically, this should be valid text for passing
             to parse_move().
         """
 
+    def get_players(self) -> typing.Iterable[int]:
+        return self.X_PLAYER, self.O_PLAYER
+
     @abstractmethod
     def get_move_count(self) -> int:
         """ The number of moves that have already been made in the game. """
 
     @abstractmethod
     def get_spaces(self) -> np.ndarray:
         """ Extract the board spaces from the complete game state.
@@ -128,17 +131,17 @@
 
 
 # noinspection PyAbstractClass
 class GridGameState(GameState):
     def __init__(self,
                  board_height: int,
                  board_width: int,
-                 text: str = None,
-                 lines: typing.Sequence[str] = None,
-                 spaces: np.ndarray = None,
+                 text: str | None = None,
+                 lines: typing.Sequence[str] | None = None,
+                 spaces: np.ndarray | None = None,
                  extra_count: int = 0):
         self.board_height = board_height
         self.board_width = board_width
         if spaces is None:
             self.board = np.zeros(self.board_height*self.board_width + extra_count,
                                   dtype=int)
         else:
@@ -163,26 +166,23 @@
 
     def __eq__(self, other):
         if not isinstance(other, GridGameState):
             return False
         return np.array_equal(self.board, other.board)
 
     def get_move_count(self) -> int:
-        return (self.get_spaces() != GameState.NO_PLAYER).sum()
+        return int((self.get_spaces() != GameState.NO_PLAYER).sum())
 
     def get_spaces(self) -> np.ndarray:
         return self.board[:self.board_height*self.board_width].reshape(
             self.board_height,
             self.board_width)
 
     def get_valid_moves(self) -> np.ndarray:
         spaces = self.get_spaces()
-        if (self.is_win(self.X_PLAYER) or
-                self.is_win(self.O_PLAYER)):
-            return np.zeros(self.board_height*self.board_width, bool)
         return spaces.reshape(self.board_height *
                               self.board_width) == GameState.NO_PLAYER
 
     def display(self, show_coordinates: bool = False) -> str:
         result = StringIO()
         if show_coordinates:
             result.write('  ')
```

### Comparing `zero_play-0.4.0/zero_play/grid_controls_ui.py` & `zero_play-0.5.0/zero_play/grid_controls_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'grid_controls_ui.ui'
 ##
-## Created by: Qt User Interface Compiler version 5.15.0
+## Created by: Qt User Interface Compiler version 6.2.1
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
-from PySide2.QtCore import (QCoreApplication, QDate, QDateTime, QMetaObject,
-    QObject, QPoint, QRect, QSize, QTime, QUrl, Qt)
-from PySide2.QtGui import (QBrush, QColor, QConicalGradient, QCursor, QFont,
-    QFontDatabase, QIcon, QKeySequence, QLinearGradient, QPalette, QPainter,
-    QPixmap, QRadialGradient)
-from PySide2.QtWidgets import *
+from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
+    QMetaObject, QObject, QPoint, QRect,
+    QSize, QTime, QUrl, Qt)
+from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
+    QFont, QFontDatabase, QGradient, QIcon,
+    QImage, QKeySequence, QLinearGradient, QPainter,
+    QPalette, QPixmap, QRadialGradient, QTransform)
+from PySide6.QtWidgets import (QApplication, QGraphicsView, QGridLayout, QSizePolicy,
+    QSpacerItem, QWidget)
 
 from zero_play.scaled_label import ScaledLabel
 
-
 class Ui_GridControls(object):
     def setupUi(self, GridControls):
         if not GridControls.objectName():
             GridControls.setObjectName(u"GridControls")
         GridControls.resize(400, 300)
         self.grid_layout = QGridLayout(GridControls)
         self.grid_layout.setObjectName(u"grid_layout")
```

### Comparing `zero_play-0.4.0/zero_play/grid_display.py` & `zero_play-0.5.0/zero_play/grid_display.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
 import typing
 
-from PySide2.QtGui import QColor, QBrush, QFont, QResizeEvent, QPixmap, Qt, QPainter, QPen
-from PySide2.QtWidgets import QGraphicsItem, QGraphicsEllipseItem, \
+from PySide6.QtGui import QColor, QBrush, QFont, QResizeEvent, QPixmap, Qt, QPainter, QPen
+from PySide6.QtWidgets import QGraphicsEllipseItem, \
     QGraphicsSceneHoverEvent, QGraphicsSceneMouseEvent, QGraphicsScene
 
 from zero_play.game_state import GridGameState, GameState
 from zero_play.game_display import GameDisplay, center_text_item
 from zero_play.grid_controls_ui import Ui_GridControls
 
 
@@ -69,15 +69,15 @@
         for j in range(start_state.board_width):
             self.column_labels.append(scene.addSimpleText(chr(65+j)))
         self.to_move = scene.addEllipse(
             0, 0, 1, 1, brush=self.get_player_brush(self.start_state.X_PLAYER))
         self.to_move.setVisible(False)
         self.move_text = ui.move_text
         for i in range(self.start_state.board_height):
-            row: typing.List[QGraphicsItem] = []
+            row: typing.List[GraphicsPieceItem] = []
             self.spaces.append(row)
             for j in range(self.start_state.board_width):
                 piece = GraphicsPieceItem(i, j, self)
                 scene.addItem(piece)
                 piece.setBrush(self.background_colour)
                 piece.setPen(self.background_colour)
                 row.append(piece)
@@ -134,15 +134,15 @@
     def scene(self) -> QGraphicsScene:
         return self.ui.game_display.scene()
 
     @staticmethod
     def create_icon(player_colour: QColor) -> QPixmap:
         size = 200
         icon = QPixmap(size, size)
-        icon.fill(Qt.transparent)
+        icon.fill(Qt.GlobalColor.transparent)
         painter = QPainter(icon)
         try:
             painter.setBrush(player_colour)
             pen = QPen()
             pen.setWidth(3)
             painter.setPen(pen)
             painter.drawEllipse(1, 1, size-2, size-2)
@@ -196,15 +196,15 @@
                       else self.player2_colour)
 
     def get_player_icon(self, player: int) -> QPixmap:
         return (self.player1_icon
                 if player == self.start_state.X_PLAYER
                 else self.player2_icon)
 
-    def update_move_text(self, text: str = None):
+    def update_move_text(self, text: str | None = None):
         if self.debug_message:
             self.move_text.setText(self.debug_message)
         elif text is not None:
             self.move_text.setText(text)
 
     def on_hover_enter(self, piece_item: GraphicsPieceItem):
         if self.is_piece_played(piece_item):
```

### Comparing `zero_play-0.4.0/zero_play/heuristic.py` & `zero_play-0.5.0/zero_play/heuristic.py`

 * *Files identical despite different names*

### Comparing `zero_play-0.4.0/zero_play/log_display.py` & `zero_play-0.5.0/zero_play/log_display.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 self.move_text == other.move_text and
                 self.game_state == other.game_state and
                 self.comment == other.comment and
                 self.choices == other.choices)
 
 
 class LogDisplay:
-    def __init__(self):
+    def __init__(self) -> None:
         self.step = 0
         self.items: typing.List[LogItem] = []
         self.offsets: typing.List[int] = []
 
     def record_move(self, game_state: GameState, move: int):
         self.step += 1
         player = game_state.display_player(game_state.get_active_player())
```

### Comparing `zero_play-0.4.0/zero_play/main_window.py` & `zero_play-0.5.0/zero_play/main_window.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'main_window.ui'
 ##
-## Created by: Qt User Interface Compiler version 5.15.0
+## Created by: Qt User Interface Compiler version 6.4.3
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
-from PySide2.QtCore import (QCoreApplication, QDate, QDateTime, QMetaObject,
-    QObject, QPoint, QRect, QSize, QTime, QUrl, Qt)
-from PySide2.QtGui import (QBrush, QColor, QConicalGradient, QCursor, QFont,
-    QFontDatabase, QIcon, QKeySequence, QLinearGradient, QPalette, QPainter,
-    QPixmap, QRadialGradient)
-from PySide2.QtWidgets import *
-
+from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
+    QMetaObject, QObject, QPoint, QRect,
+    QSize, QTime, QUrl, Qt)
+from PySide6.QtGui import (QAction, QBrush, QColor, QConicalGradient,
+    QCursor, QFont, QFontDatabase, QGradient,
+    QIcon, QImage, QKeySequence, QLinearGradient,
+    QPainter, QPalette, QPixmap, QRadialGradient,
+    QTransform)
+from PySide6.QtWidgets import (QApplication, QCheckBox, QComboBox, QGridLayout,
+    QHeaderView, QLabel, QLineEdit, QMainWindow,
+    QMenu, QMenuBar, QPushButton, QSizePolicy,
+    QSpacerItem, QSpinBox, QStackedWidget, QStatusBar,
+    QTableWidget, QTableWidgetItem, QTextBrowser, QVBoxLayout,
+    QWidget)
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         if not MainWindow.objectName():
             MainWindow.setObjectName(u"MainWindow")
         MainWindow.resize(911, 607)
         self.action_open = QAction(MainWindow)
@@ -45,14 +52,16 @@
         self.action_coordinates.setCheckable(True)
         self.action_about = QAction(MainWindow)
         self.action_about.setObjectName(u"action_about")
         self.action_new_db = QAction(MainWindow)
         self.action_new_db.setObjectName(u"action_new_db")
         self.action_open_db = QAction(MainWindow)
         self.action_open_db.setObjectName(u"action_open_db")
+        self.action_strength_test = QAction(MainWindow)
+        self.action_strength_test.setObjectName(u"action_strength_test")
         self.centralwidget = QWidget(MainWindow)
         self.centralwidget.setObjectName(u"centralwidget")
         self.verticalLayout_2 = QVBoxLayout(self.centralwidget)
         self.verticalLayout_2.setObjectName(u"verticalLayout_2")
         self.stacked_widget = QStackedWidget(self.centralwidget)
         self.stacked_widget.setObjectName(u"stacked_widget")
         self.game_page = QWidget()
@@ -198,47 +207,47 @@
 
         self.player_layout.setColumnStretch(1, 10)
         self.player_layout.setColumnStretch(2, 1)
 
         self.verticalLayout.addLayout(self.player_layout)
 
         self.stacked_widget.addWidget(self.players_page)
-        self.history_page = QWidget()
-        self.history_page.setObjectName(u"history_page")
-        self.gridLayout = QGridLayout(self.history_page)
+        self.humans_page = QWidget()
+        self.humans_page.setObjectName(u"humans_page")
+        self.gridLayout = QGridLayout(self.humans_page)
         self.gridLayout.setObjectName(u"gridLayout")
-        self.close_humans = QPushButton(self.history_page)
+        self.close_humans = QPushButton(self.humans_page)
         self.close_humans.setObjectName(u"close_humans")
         sizePolicy4.setHeightForWidth(self.close_humans.sizePolicy().hasHeightForWidth())
         self.close_humans.setSizePolicy(sizePolicy4)
 
         self.gridLayout.addWidget(self.close_humans, 1, 1, 1, 1)
 
-        self.players_label = QLabel(self.history_page)
+        self.players_label = QLabel(self.humans_page)
         self.players_label.setObjectName(u"players_label")
 
         self.gridLayout.addWidget(self.players_label, 0, 0, 1, 1)
 
-        self.new_human = QPushButton(self.history_page)
+        self.new_human = QPushButton(self.humans_page)
         self.new_human.setObjectName(u"new_human")
         sizePolicy4.setHeightForWidth(self.new_human.sizePolicy().hasHeightForWidth())
         self.new_human.setSizePolicy(sizePolicy4)
 
         self.gridLayout.addWidget(self.new_human, 1, 3, 1, 1)
 
-        self.tableWidget = QTableWidget(self.history_page)
-        self.tableWidget.setObjectName(u"tableWidget")
+        self.players_table = QTableWidget(self.humans_page)
+        self.players_table.setObjectName(u"players_table")
 
-        self.gridLayout.addWidget(self.tableWidget, 0, 1, 1, 3)
+        self.gridLayout.addWidget(self.players_table, 0, 1, 1, 3)
 
-        self.horizontalSpacer = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.spacer = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
-        self.gridLayout.addItem(self.horizontalSpacer, 1, 2, 1, 1)
+        self.gridLayout.addItem(self.spacer, 1, 2, 1, 1)
 
-        self.stacked_widget.addWidget(self.history_page)
+        self.stacked_widget.addWidget(self.humans_page)
         self.rules_page = QWidget()
         self.rules_page.setObjectName(u"rules_page")
         self.gridLayout_4 = QGridLayout(self.rules_page)
         self.gridLayout_4.setObjectName(u"gridLayout_4")
         self.rules_text = QTextBrowser(self.rules_page)
         self.rules_text.setObjectName(u"rules_text")
 
@@ -292,19 +301,101 @@
 
         self.game_display = QLabel(self.display_page)
         self.game_display.setObjectName(u"game_display")
 
         self.gridLayout_2.addWidget(self.game_display, 0, 0, 1, 3)
 
         self.stacked_widget.addWidget(self.display_page)
-        self.plot_page = QWidget()
-        self.plot_page.setObjectName(u"plot_page")
-        self.plot_layout = QVBoxLayout(self.plot_page)
-        self.plot_layout.setObjectName(u"plot_layout")
-        self.stacked_widget.addWidget(self.plot_page)
+        self.plot_strength_page = QWidget()
+        self.plot_strength_page.setObjectName(u"plot_strength_page")
+        self.gridLayout_5 = QGridLayout(self.plot_strength_page)
+        self.gridLayout_5.setObjectName(u"gridLayout_5")
+        self.strength_count_label = QLabel(self.plot_strength_page)
+        self.strength_count_label.setObjectName(u"strength_count_label")
+
+        self.gridLayout_5.addWidget(self.strength_count_label, 6, 0, 1, 1)
+
+        self.label_2 = QLabel(self.plot_strength_page)
+        self.label_2.setObjectName(u"label_2")
+
+        self.gridLayout_5.addWidget(self.label_2, 3, 0, 1, 1)
+
+        self.strength_test_game = QComboBox(self.plot_strength_page)
+        self.strength_test_game.setObjectName(u"strength_test_game")
+
+        self.gridLayout_5.addWidget(self.strength_test_game, 0, 1, 1, 2)
+
+        self.reset_strength_test = QPushButton(self.plot_strength_page)
+        self.reset_strength_test.setObjectName(u"reset_strength_test")
+
+        self.gridLayout_5.addWidget(self.reset_strength_test, 6, 2, 1, 1)
+
+        self.label = QLabel(self.plot_strength_page)
+        self.label.setObjectName(u"label")
+
+        self.gridLayout_5.addWidget(self.label, 0, 0, 1, 1)
+
+        self.strength_test_min = QSpinBox(self.plot_strength_page)
+        self.strength_test_min.setObjectName(u"strength_test_min")
+        self.strength_test_min.setMinimum(1)
+        self.strength_test_min.setMaximum(1000000)
+
+        self.gridLayout_5.addWidget(self.strength_test_min, 3, 1, 1, 2)
+
+        self.start_strength_test = QPushButton(self.plot_strength_page)
+        self.start_strength_test.setObjectName(u"start_strength_test")
+
+        self.gridLayout_5.addWidget(self.start_strength_test, 6, 1, 1, 1)
+
+        self.strengths_label = QLabel(self.plot_strength_page)
+        self.strengths_label.setObjectName(u"strengths_label")
+
+        self.gridLayout_5.addWidget(self.strengths_label, 2, 0, 1, 1)
+
+        self.label_3 = QLabel(self.plot_strength_page)
+        self.label_3.setObjectName(u"label_3")
+
+        self.gridLayout_5.addWidget(self.label_3, 4, 0, 1, 1)
+
+        self.strength_test_strengths = QLineEdit(self.plot_strength_page)
+        self.strength_test_strengths.setObjectName(u"strength_test_strengths")
+
+        self.gridLayout_5.addWidget(self.strength_test_strengths, 2, 1, 1, 2)
+
+        self.strength_test_max = QSpinBox(self.plot_strength_page)
+        self.strength_test_max.setObjectName(u"strength_test_max")
+        self.strength_test_max.setMinimum(1)
+        self.strength_test_max.setMaximum(1000000)
+        self.strength_test_max.setValue(512)
+
+        self.gridLayout_5.addWidget(self.strength_test_max, 4, 1, 1, 2)
+
+        self.stacked_widget.addWidget(self.plot_strength_page)
+        self.plot_strength_display_page = QWidget()
+        self.plot_strength_display_page.setObjectName(u"plot_strength_display_page")
+        self.gridLayout_7 = QGridLayout(self.plot_strength_display_page)
+        self.gridLayout_7.setObjectName(u"gridLayout_7")
+        self.stacked_widget.addWidget(self.plot_strength_display_page)
+        self.plot_history_page = QWidget()
+        self.plot_history_page.setObjectName(u"plot_history_page")
+        self.gridLayout_6 = QGridLayout(self.plot_history_page)
+        self.gridLayout_6.setObjectName(u"gridLayout_6")
+        self.label_4 = QLabel(self.plot_history_page)
+        self.label_4.setObjectName(u"label_4")
+
+        self.gridLayout_6.addWidget(self.label_4, 0, 0, 1, 1)
+
+        self.history_game = QComboBox(self.plot_history_page)
+        self.history_game.setObjectName(u"history_game")
+
+        self.gridLayout_6.addWidget(self.history_game, 0, 1, 1, 1)
+
+        self.gridLayout_6.setColumnStretch(0, 1)
+        self.gridLayout_6.setColumnStretch(1, 8)
+        self.stacked_widget.addWidget(self.plot_history_page)
 
         self.verticalLayout_2.addWidget(self.stacked_widget)
 
         MainWindow.setCentralWidget(self.centralwidget)
         self.menubar = QMenuBar(MainWindow)
         self.menubar.setObjectName(u"menubar")
         self.menubar.setGeometry(QRect(0, 0, 911, 22))
@@ -332,21 +423,22 @@
         self.menu_file.addAction(self.action_save_log)
         self.menu_file.addAction(self.action_new_db)
         self.menu_file.addAction(self.action_open_db)
         self.menu_new.addAction(self.action_game)
         self.menu_new.addAction(self.action_comparison)
         self.menu_new.addAction(self.action_plot)
         self.menu_new.addAction(self.action_training_session)
+        self.menu_new.addAction(self.action_strength_test)
         self.menu_view.addAction(self.action_coordinates)
         self.menu_help.addAction(self.action_about)
         self.menu_help.addAction(self.menu_rules.menuAction())
 
         self.retranslateUi(MainWindow)
 
-        self.stacked_widget.setCurrentIndex(1)
+        self.stacked_widget.setCurrentIndex(5)
 
 
         QMetaObject.connectSlotsByName(MainWindow)
     # setupUi
 
     def retranslateUi(self, MainWindow):
         MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"MainWindow", None))
@@ -357,14 +449,15 @@
         self.action_game.setText(QCoreApplication.translate("MainWindow", u"&Game", None))
         self.action_save.setText(QCoreApplication.translate("MainWindow", u"&Save...", None))
         self.action_save_log.setText(QCoreApplication.translate("MainWindow", u"Save &Log...", None))
         self.action_coordinates.setText(QCoreApplication.translate("MainWindow", u"Coordinates", None))
         self.action_about.setText(QCoreApplication.translate("MainWindow", u"&About...", None))
         self.action_new_db.setText(QCoreApplication.translate("MainWindow", u"New Player &Database...", None))
         self.action_open_db.setText(QCoreApplication.translate("MainWindow", u"&Open Player Database...", None))
+        self.action_strength_test.setText(QCoreApplication.translate("MainWindow", u"&Strength Test", None))
         self.connect4.setText(QCoreApplication.translate("MainWindow", u"Connect 4", None))
         self.tic_tac_toe.setText(QCoreApplication.translate("MainWindow", u"Tic Tac Toe", None))
         self.othello.setText(QCoreApplication.translate("MainWindow", u"Othello", None))
         self.searches_lock2.setText(QCoreApplication.translate("MainWindow", u"Lock", None))
         self.cancel.setText(QCoreApplication.translate("MainWindow", u"Cancel", None))
         self.searches_label1.setText(QCoreApplication.translate("MainWindow", u"searches", None))
         self.searches_lock1.setText(QCoreApplication.translate("MainWindow", u"Lock", None))
@@ -378,14 +471,31 @@
         self.close_humans.setText(QCoreApplication.translate("MainWindow", u"OK", None))
         self.players_label.setText(QCoreApplication.translate("MainWindow", u"Players", None))
         self.new_human.setText(QCoreApplication.translate("MainWindow", u"New", None))
         self.rules_close.setText(QCoreApplication.translate("MainWindow", u"Close", None))
         self.toggle_review.setText(QCoreApplication.translate("MainWindow", u"Review / Resume", None))
         self.resume_here.setText(QCoreApplication.translate("MainWindow", u"Resume Here", None))
         self.game_display.setText(QCoreApplication.translate("MainWindow", u"Game Display", None))
+        self.strength_count_label.setText(QCoreApplication.translate("MainWindow", u"0 games recorded", None))
+        self.label_2.setText(QCoreApplication.translate("MainWindow", u"Opponent min:", None))
+        self.reset_strength_test.setText(QCoreApplication.translate("MainWindow", u"Reset", None))
+        self.label.setText(QCoreApplication.translate("MainWindow", u"Game:", None))
+        self.strength_test_min.setSuffix(QCoreApplication.translate("MainWindow", u" iteration(s)", None))
+        self.start_strength_test.setText(QCoreApplication.translate("MainWindow", u"Start", None))
+        self.strengths_label.setText(QCoreApplication.translate("MainWindow", u"Player strengths:", None))
+        self.label_3.setText(QCoreApplication.translate("MainWindow", u"Opponent max:", None))
+#if QT_CONFIG(tooltip)
+        self.strength_test_strengths.setToolTip("")
+#endif // QT_CONFIG(tooltip)
+#if QT_CONFIG(whatsthis)
+        self.strength_test_strengths.setWhatsThis("")
+#endif // QT_CONFIG(whatsthis)
+        self.strength_test_strengths.setText(QCoreApplication.translate("MainWindow", u"1 8 64", None))
+        self.strength_test_max.setSuffix(QCoreApplication.translate("MainWindow", u" iteration(s)", None))
+        self.label_4.setText(QCoreApplication.translate("MainWindow", u"Game:", None))
         self.menu_file.setTitle(QCoreApplication.translate("MainWindow", u"&File", None))
         self.menu_new.setTitle(QCoreApplication.translate("MainWindow", u"&New", None))
         self.menu_view.setTitle(QCoreApplication.translate("MainWindow", u"&View", None))
         self.menu_help.setTitle(QCoreApplication.translate("MainWindow", u"&Help", None))
         self.menu_rules.setTitle(QCoreApplication.translate("MainWindow", u"&Rules", None))
     # retranslateUi
```

### Comparing `zero_play-0.4.0/zero_play/mcts_player.py` & `zero_play-0.5.0/zero_play/mcts_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 class SearchNode:
     # Controls exploration of new nodes vs. exploitation of good nodes.
     exploration_weight = 1.0
 
     def __init__(self,
                  game_state: GameState,
-                 parent: 'SearchNode' = None,
-                 move: int = None):
+                 parent: typing.Optional['SearchNode'] = None,
+                 move: int | None = None):
         """ Initialize an instance.
 
         :param game_state: the board state that this node represents
         :param parent: the board state that this node came from
         :param move: the move to get from parent to this node
         """
         self.game_state = game_state
@@ -66,23 +66,27 @@
                 best_score = score
                 best_child = child
         return best_child.select_leaf()
 
     def find_all_children(self) -> typing.List['SearchNode']:
         if self.children is not None:
             return self.children
-        children = []
+        children: typing.List['SearchNode'] = []
+        if self.game_state.is_ended():
+            return children
         for move, is_valid in enumerate(self.game_state.get_valid_moves()):
             if is_valid:
                 child_state = self.game_state.make_move(move)
                 children.append(SearchNode(child_state, self, move))
         self.children = children
         return children
 
-    def record_value(self, value: float, child_predictions: np.ndarray = None):
+    def record_value(self,
+                     value: float,
+                     child_predictions: np.ndarray | None = None):
         if child_predictions is not None:
             self.child_predictions = child_predictions
         if (not self.parent or
                 self.parent.game_state.get_active_player() !=
                 self.game_state.get_active_player()):
             value *= -1
         self.average_value = ((self.average_value * self.value_count + value) /
@@ -100,16 +104,17 @@
 
         :param temperature: positive value that controls how deterministic the
         choice is. The closer to zero, the more likely it is to choose the
         child with maximum count.
         """
         children = self.find_all_children()
         probabilities = self.rank_children(children, temperature)
-        child = np.random.choice(children, p=probabilities)
-        return child
+        child_count = len(children)
+        child_index = np.random.choice(child_count, p=probabilities)
+        return children[child_index]
 
     @staticmethod
     def rank_children(children, temperature):
         values = np.array([temperature * child.value_count for child in children])
 
         # Avoid overflow by keeping the weights between 0 and 1.
         values -= values.max(initial=0)
@@ -193,21 +198,21 @@
         for done_future in done:
             done_leaf = self.tasks.pop(done_future)
             value, child_predictions = done_future.result()
             done_leaf.record_value(value, child_predictions)
 
     def get_best_move(self) -> int:
         best_children = self.current_node.find_best_children()
-        self.current_node = np.random.choice(best_children)
-        assert self.current_node.move is not None
-        return self.current_node.move
+        self.current_node = child = np.random.choice(best_children)
+        assert child.move is not None
+        return child.move
 
     def choose_weighted_move(self) -> int:
         temperature = 1.0
-        child = self.current_node.choose_child(temperature)
+        self.current_node = child = self.current_node.choose_child(temperature)
         assert child.move is not None
         return child.move
 
     def get_move_probabilities(
             self,
             game_state: GameState,
             limit: int = 10) -> typing.List[typing.Tuple[str,
@@ -237,15 +242,15 @@
                       value_count,
                       child_node.average_value)
                      for value_count, probability, child_node in top_children
                      if child_node.move is not None]
         return top_moves
 
     def create_training_data(self, iterations: int, data_size: int):
-        game_states = []
+        game_states: typing.List[typing.Tuple[GameState, np.ndarray]] = []
         self.search(self.current_node.game_state, iterations=1)  # One extra to start.
         report_size = 0
         board_shape = self.current_node.game_state.get_spaces().shape
         boards = np.zeros((data_size,) + board_shape, int)
         move_count = self.current_node.game_state.get_valid_moves().size
         outputs = np.zeros((data_size, move_count + 1))
         data_count = 0
@@ -256,15 +261,15 @@
             move_weights = np.zeros(self.current_node.child_predictions.size)
             for child in self.current_node.children:
                 move = child.move
                 move_weights[move] = child.value_count
             total_weight = move_weights.sum()
             if total_weight:
                 move_weights /= total_weight
-            game_states.append([self.current_node.game_state, move_weights])
+            game_states.append((self.current_node.game_state, move_weights))
             move = np.random.choice(move_weights.size, p=move_weights)
             for child in self.current_node.children:
                 if child.move == move:
                     self.current_node = child
                     break
             if self.current_node.game_state.is_ended():
                 final_value, _ = self.heuristic.analyse(self.current_node.game_state)
@@ -299,15 +304,15 @@
     """
     DEFAULT_ITERATIONS = 80
 
     def __init__(self,
                  start_state: GameState,
                  player_number: int = GameState.X_PLAYER,
                  iteration_count: int = DEFAULT_ITERATIONS,
-                 heuristic: Heuristic = None,
+                 heuristic: Heuristic | None = None,
                  process_count: int = 1):
         super().__init__(player_number, heuristic)
         self.iteration_count = iteration_count
         self.search_manager = SearchManager(start_state,
                                             self.heuristic,
                                             process_count)
 
@@ -318,15 +323,15 @@
     @heuristic.setter
     def heuristic(self, value: Heuristic):
         self._heuristic = value
         search_manager = getattr(self, 'search_manager', None)
         if search_manager is not None:
             search_manager.heuristic = value
 
-    def end_game(self, game_state: np.ndarray, opponent: Player):
+    def end_game(self, game_state: GameState, opponent: Player):
         self.search_manager.reset()
 
     def choose_move(self, game_state: GameState) -> int:
         """ Choose a move for the given board.
 
         :param game_state: the current state of the game.
         :return: the chosen move's index in the list of valid moves.
```

### Comparing `zero_play-0.4.0/zero_play/mcts_worker.py` & `zero_play-0.5.0/zero_play/mcts_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from traceback import print_exc
 
-from PySide2.QtCore import QObject, Signal, Slot
-from PySide2.QtWidgets import QMessageBox
+from PySide6.QtCore import QObject, Signal, Slot
+from PySide6.QtWidgets import QMessageBox
 
 from zero_play.game_state import GameState
 from zero_play.mcts_player import MctsPlayer
 
 
 class MctsWorker(QObject):
     move_chosen = Signal(int)
     # board, analysing_player, [(move_text, probability, count)] for top 10 choices
     move_analysed = Signal(GameState, int, list)
 
-    def __init__(self, player: MctsPlayer, parent: QObject = None):
+    def __init__(self, player: MctsPlayer, parent: QObject | None = None):
         super().__init__(parent)
         self.player = player
 
     @Slot(int, GameState)  # type: ignore
     def choose_move(self, active_player: int, game_state: GameState):
         # noinspection PyBroadException
         try:
```

### Comparing `zero_play-0.4.0/zero_play/othello/display.py` & `zero_play-0.5.0/zero_play/othello/display.py`

 * *Files identical despite different names*

### Comparing `zero_play-0.4.0/zero_play/othello/game.py` & `zero_play-0.5.0/zero_play/othello/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from zero_play.game_state import GridGameState
 
 
 class OthelloState(GridGameState):
     game_name = 'Othello'
 
     def __init__(self,
-                 text: str = None,
+                 text: str | None = None,
                  board_height: int = 6,
                  board_width: int = 6,
-                 spaces: np.ndarray = None):
+                 spaces: np.ndarray | None = None):
         if spaces is not None:
             size = spaces.size
             board_width = board_height = int(math.sqrt(size-1))
             assert text is None
         if text is None:
             lines = None
             next_player_line = None
```

### Comparing `zero_play-0.4.0/zero_play/play_controller.py` & `zero_play-0.5.0/zero_play/play_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             move_time = self.total_time / self.move_count
         else:
             move_time = 0.0
         return f'{self.summary} - {self.win_count} wins, {move_time:0.3}s/move'
 
 
 class PlayController:
-    def __init__(self, start_state: GameState, players: typing.List[Player]):
+    def __init__(self, start_state: GameState, players: typing.Sequence[Player]):
         self.board = self.start_state = start_state
         x_player: Player
         o_player: Player
         x_player, o_player = players
         x_player.player_number = start_state.players[0]
         o_player.player_number = start_state.players[1]
         self.players = {x_player.player_number: x_player,
```

### Comparing `zero_play-0.4.0/zero_play/player.py` & `zero_play-0.5.0/zero_play/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         i = -1
     return values[i]
 
 
 class Player(metaclass=ABCMeta):
     def __init__(self,
                  player_number: int = GameState.X_PLAYER,
-                 heuristic: Heuristic = None):
+                 heuristic: Heuristic | None = None):
         if heuristic is None:
             heuristic = Playout()
         self.player_number = player_number
         self.heuristic = heuristic
 
     @property
     def heuristic(self):
```

### Comparing `zero_play-0.4.0/zero_play/playout.py` & `zero_play-0.5.0/zero_play/playout.py`

 * *Files identical despite different names*

### Comparing `zero_play-0.4.0/zero_play/plot_perf.py` & `zero_play-0.5.0/zero_play/plot_perf.py`

 * *Files identical despite different names*

### Comparing `zero_play-0.4.0/zero_play/scaled_label.py` & `zero_play-0.5.0/zero_play/scaled_label.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PySide2.QtCore import QMargins
-from PySide2.QtGui import QResizeEvent, QFontMetrics, Qt
-from PySide2.QtWidgets import QLabel
+from PySide6.QtCore import QMargins
+from PySide6.QtGui import QResizeEvent, QFontMetrics, Qt
+from PySide6.QtWidgets import QLabel
 
 
 class ScaledLabel(QLabel):
     def resizeEvent(self, event: QResizeEvent):
         # This flag is used for pixmaps, but I thought it might be useful to
         # be able to disable font scaling.
         if not self.hasScaledContents():
@@ -20,15 +20,19 @@
         font = self.font()
         while min_size < max_size:
             new_size = (min_size + max_size) // 2
             font.setPointSize(new_size)
             metrics = QFontMetrics(font)
 
             # Be careful which overload of boundingRect() you call.
-            rect = metrics.boundingRect(target_rect, Qt.AlignLeft, text)
+            rect = metrics.boundingRect(target_rect,
+                                        Qt.AlignmentFlag.AlignLeft,
+                                        text,
+                                        tabstops=0,
+                                        tabarray=None)  # type: ignore
             if (target_rect.width() < rect.width() or
                     target_rect.height() < rect.height()):
                 max_size = new_size - 1
             elif (rect.width() == target_rect.width() or
                   rect.height() == target_rect.height()):
                 min_size = max_size = new_size
             else:
```

### Comparing `zero_play-0.4.0/zero_play/scaled_radio_button.py` & `zero_play-0.5.0/zero_play/scaled_radio_button.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PySide2.QtCore import QSize
-from PySide2.QtGui import QResizeEvent, QFontMetrics, Qt
-from PySide2.QtWidgets import QRadioButton
+from PySide6.QtCore import QSize
+from PySide6.QtGui import QResizeEvent, QFontMetrics, Qt
+from PySide6.QtWidgets import QRadioButton
 
 
 class ScaledRadioButton(QRadioButton):
     def resizeEvent(self, event: QResizeEvent):
         target_rect = self.contentsRect()
         text = self.text()
         icon = self.icon()
@@ -20,15 +20,19 @@
             new_size = (min_size + max_size) // 2
             indicator_width = new_size
             indicator_spacing = new_size // 2
             font.setPointSize(new_size)
             metrics = QFontMetrics(font)
 
             # Be careful which overload of boundingRect() you call.
-            rect = metrics.boundingRect(target_rect, Qt.AlignLeft, text)
+            rect = metrics.boundingRect(target_rect,
+                                        Qt.AlignmentFlag.AlignLeft,
+                                        text,
+                                        tabstops=0,
+                                        tabarray=None)  # type: ignore
             full_width = indicator_width + indicator_spacing + rect.width()
             height = rect.height()
             if icon:
                 icon_size = new_size * 3 // 2
                 full_width += icon_size
                 if text:
                     full_width += icon_spacing
```

### Comparing `zero_play-0.4.0/zero_play/strength_adjuster.py` & `zero_play-0.5.0/zero_play/strength_adjuster.py`

 * *Files identical despite different names*

### Comparing `zero_play-0.4.0/zero_play/tictactoe/state.py` & `zero_play-0.5.0/zero_play/tictactoe/state.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from zero_play.game_state import GridGameState
 
 
 class TicTacToeState(GridGameState):
     game_name = 'Tic Tac Toe'
 
     def __init__(self,
-                 text: str = None,
-                 spaces: np.ndarray = None,
+                 text: str | None = None,
+                 spaces: np.ndarray | None = None,
                  board_height: int = 3,
                  board_width: int = 3):
         super().__init__(board_height=board_height,
                          board_width=board_width,
                          text=text,
                          spaces=spaces)
```

### Comparing `zero_play-0.4.0/zero_play/zero_perf.py` & `zero_play-0.5.0/zero_play/zero_perf.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                         help='Number of parallel search processes for player 2.')
     parser.add_argument('--display',
                         action='store_true',
                         help='Display moves in the games.')
     return parser.parse_args()
 
 
-def main():
+def main() -> None:
     args = parse_args()
     class_path = args.game
     class_parts = class_path.split('.')
     class_name = class_parts.pop()
     module_name = '.'.join(class_parts)
     module = import_module(module_name)
     game_state_class = getattr(module, class_name)
```

### Comparing `zero_play-0.4.0/zero_play/zero_play.py` & `zero_play-0.5.0/zero_play/zero_play.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,132 +1,199 @@
 import math
+import os
 import sys
 import typing
+from datetime import datetime
 from functools import partial
 from itertools import chain
 from operator import attrgetter
 from os import cpu_count
+from pathlib import Path
 from random import shuffle
 
 import numpy as np
-from PySide2.QtCore import QSettings, QFile, QTextStream
+from PySide6.QtCore import QSettings
 
-from PySide2.QtGui import Qt, QIcon, QPixmap
-from PySide2.QtWidgets import (QApplication, QMainWindow, QFileDialog,
+from PySide6.QtGui import Qt, QIcon, QPixmap
+from PySide6.QtWidgets import (QApplication, QMainWindow, QFileDialog,
                                QTableWidgetItem, QGridLayout, QPushButton,
                                QSizePolicy, QDialog, QWidget, QLabel, QComboBox)
+from alembic import command
+from alembic.config import Config
 from pkg_resources import iter_entry_points, EntryPoint
+from sqlalchemy import create_engine
+from sqlalchemy.orm import Session as BaseSession
+from sqlalchemy.util import immutabledict
 
 import zero_play
 from zero_play.about_dialog import Ui_Dialog
 from zero_play.game_state import GameState
 from zero_play.game_display import GameDisplay
 from zero_play.main_window import Ui_MainWindow
 from zero_play.mcts_player import MctsPlayer
+from zero_play.models import Session
+from zero_play.models.game import GameRecord
+from zero_play.models.match import MatchRecord
+from zero_play.models.match_player import MatchPlayerRecord
+from zero_play.models.player import PlayerRecord
+from zero_play.play_controller import PlayController
 from zero_play.playout import Playout
-from zero_play.rules_formatter import convert_markdown
+from zero_play.process_display import ProcessDisplay
 from zero_play.strength_adjuster import StrengthAdjuster
 from zero_play import zero_play_rules_rc
 from zero_play import zero_play_images_rc
+from zero_play.strength_history_plot import StrengthHistoryPlot
+from zero_play.strength_plot import StrengthPlot
 
 assert zero_play_rules_rc  # Need to import this module to load resources.
 assert zero_play_images_rc  # Need to import this module to load resources.
 
 try:
     from zero_play.plot_canvas import PlotCanvas
 except ImportError:
     from zero_play.plot_canvas_dummy import PlotCanvasDummy as PlotCanvas  # type: ignore
 
+DEFAULT_SEARCHES = 600
+
 
 class AboutDialog(QDialog):
     def __init__(self,
                  credit_pairs: typing.Iterable[typing.Tuple[str, str]],
-                 parent: QWidget = None):
+                 parent: QWidget | None = None) -> None:
         super().__init__(parent)
         self.ui = Ui_Dialog()
         self.ui.setupUi(self)
         self.ui.version.setText(zero_play.__version__)
         credits_layout = self.ui.credits_layout
         row = 0
         for row, (title, text) in enumerate(credit_pairs):
-            credits_layout.addWidget(QLabel(title), row, 0, Qt.AlignRight)
+            credits_layout.addWidget(QLabel(title),
+                                     row,
+                                     0,
+                                     Qt.AlignmentFlag.AlignRight)
             credits_layout.addWidget(QLabel(text), row, 1)
         row += 1
         credits_layout.addWidget(self.ui.version_label, row, 0)
         credits_layout.addWidget(self.ui.version, row, 1)
 
 
-def get_settings(game_state: GameState = None):
+def get_settings(game_state: GameState | None = None):
     settings = QSettings("Don Kirkby", "Zero Play")
     if game_state is not None:
         settings.beginGroup('games')
         settings.beginGroup(game_state.game_name.replace(' ', '_'))
 
     return settings
 
 
+def get_database_url(database_path: Path | None = None) -> typing.Optional[str]:
+    if database_path is None:
+        settings = get_settings()
+        database_path = settings.value('db_path')
+        if database_path is None or not os.path.exists(str(database_path)):
+            return None
+    database_url = f'sqlite:///{database_path}'
+    return database_url
+
+
 class ZeroPlayWindow(QMainWindow):
     """ Main window for a collection of board games.
 
     To create your own collection, declare a sub class, and override these
     methods: get_collection_name(), filter_games().
     """
     icon_path = ":/zero_play_images/main_icon.png"
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
-        self.setAttribute(Qt.WA_DeleteOnClose, True)
+        self.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose, True)
         ui = self.ui = Ui_MainWindow()
         ui.setupUi(self)
-        self.plot_canvas = PlotCanvas(ui.centralwidget)
-        ui.plot_page.layout().addWidget(self.plot_canvas)
+        self.plot_canvas = StrengthHistoryPlot(ui.centralwidget)
+        ui.plot_history_page.layout().addWidget(self.plot_canvas, 1, 0, 1, 2)
+        self.strength_canvas = StrengthPlot(ui.centralwidget)
+        ui.plot_strength_display_page.layout().addWidget(self.strength_canvas)
         ui.cancel.clicked.connect(self.on_cancel)
         ui.start.clicked.connect(self.on_start)
         ui.action_game.triggered.connect(self.on_new_game)
+        ui.action_new_db.triggered.connect(self.on_new_db)
+        ui.action_open_db.triggered.connect(self.on_open_db)
         ui.action_plot.triggered.connect(self.on_plot)
         ui.action_coordinates.triggered.connect(self.on_view_coordinates)
         ui.action_about.triggered.connect(self.on_about)
+        ui.action_strength_test.triggered.connect(self.on_new_strength_test)
+        ui.start_strength_test.clicked.connect(self.on_start_strength_test)
         ui.toggle_review.clicked.connect(self.on_toggle_review)
         ui.resume_here.clicked.connect(self.on_resume_here)
         ui.rules_close.clicked.connect(self.on_close_rules)
         ui.move_history.currentIndexChanged.connect(self.on_move_history)
         ui.player1.currentIndexChanged.connect(
             lambda new_index: self.on_player_changed(ui.player1, new_index))
         ui.player2.currentIndexChanged.connect(
             lambda new_index: self.on_player_changed(ui.player2, new_index))
         ui.searches1.valueChanged.connect(self.on_searches_changed)
         ui.searches_lock1.stateChanged.connect(self.on_lock_changed)
         ui.searches_lock2.stateChanged.connect(self.on_lock_changed)
-        self.cpu_count = cpu_count()
+        self.cpu_count = cpu_count() or 1
         self.is_history_dirty = False  # Has current game been rewound?
-        self.all_displays = []
+        self.all_displays: typing.List[GameDisplay] = []
         self.load_game_list(ui.game_page.layout())
         icon_pixmap = QPixmap(self.icon_path)  # After displays load resources!
         icon = QIcon(icon_pixmap)
         self.setWindowIcon(icon)
         self.start_state: typing.Optional[GameState] = None
-        self.display: typing.Optional[GameDisplay] = None
+        self.display: ProcessDisplay | StrengthPlot | None = None
+        self.game_display: typing.Optional[GameDisplay] = None
         self.on_new_game()
         self.board_to_resume: typing.Optional[np.ndarray] = None
         self.review_names = [name.strip()
                              for name in ui.toggle_review.text().split('/')]
         self.are_coordinates_always_visible = False
+        self.game_start_time = datetime.now()
+        ui.history_game.currentIndexChanged.connect(self.requery_plot)
+        self._db_session = None
+        settings = get_settings()
+        ui.strength_test_game.setCurrentText(settings.value(
+            'strength_test_game',
+            ui.strength_test_game.currentText()))
+        ui.strength_test_strengths.setText(settings.value(
+            'strength_test_strengths',
+            ui.strength_test_strengths.text()))
+        ui.strength_test_min.setValue(settings.value(
+            'strength_test_min',
+            ui.strength_test_min.value(),
+            type=int))
+        ui.strength_test_max.setValue(settings.value(
+            'strength_test_max',
+            ui.strength_test_max.value(),
+            type=int))
         self.on_toggle_review()
 
     @staticmethod
     def get_collection_name() -> str:
         return 'Zero Play'
 
     @staticmethod
     def filter_games(
             entries: typing.Iterable[EntryPoint]) -> typing.Generator[EntryPoint,
                                                                       None,
                                                                       None]:
         yield from entries
 
+    @property
+    def db_session(self) -> typing.Optional[BaseSession]:
+        if self._db_session is None:
+            db_url = get_database_url()
+            if db_url is None:
+                return None
+            engine = create_engine(db_url)
+            Session.configure(bind=engine)
+            self._db_session = Session()
+        return self._db_session
+
     def on_about(self):
         credit_pairs = chain(*(display.credit_pairs
                                for display in self.all_displays))
         dialog = AboutDialog(credit_pairs, self)
         dialog.setWindowTitle(f'About {self.get_collection_name()}')
         dialog.exec_()
 
@@ -137,87 +204,91 @@
                 child.widget().deleteLater()
         games = self.all_displays
         all_entries = iter_entry_points('zero_play.game_display')
         filtered_entries = self.filter_games(all_entries)
         for game_entry in filtered_entries:
             display_class = game_entry.load()
             display: GameDisplay = display_class()
-            self.destroyed.connect(display.close)
+            self.destroyed.connect(display.close)  # type: ignore
             display.game_ended.connect(self.on_game_ended)  # type: ignore
             games.append(display)
         games.sort(key=attrgetter('start_state.game_name'))
         column_count = math.ceil(math.sqrt(len(games)))
         for i, display in enumerate(games):
             row = i // column_count
             column = i % column_count
             game_name = display.start_state.game_name
             game_button = QPushButton(game_name)
-            game_button.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
+            game_button.setSizePolicy(QSizePolicy.Policy.Minimum,
+                                      QSizePolicy.Policy.Minimum)
 
-            # noinspection PyUnresolvedReferences
-            game_button.clicked.connect(partial(self.show_game, display))
+            game_button.clicked.connect(partial(self.show_game,  # type: ignore
+                                                display))
             game_layout.addWidget(game_button, row, column)
 
+            self.ui.history_game.addItem(game_name, userData=display)
+            self.ui.strength_test_game.addItem(game_name, userData=display)
+
             if display.rules_path is not None:
                 game_rules_action = self.ui.menu_rules.addAction(game_name)
                 game_rules_action.triggered.connect(partial(self.on_rules,
                                                             display))
 
     def on_toggle_review(self):
         choices = self.ui.choices
         current_page = self.ui.stacked_widget.currentWidget()
         is_game_displayed = current_page is self.ui.display_page
         is_named_review = self.ui.toggle_review.text() == self.review_names[0]
         is_review_visible = is_game_displayed and is_named_review
         if not is_review_visible:
-            if self.display is not None and self.board_to_resume is not None:
-                self.display.update_board(self.board_to_resume)
+            if self.game_display is not None and self.board_to_resume is not None:
+                self.game_display.update_board(self.board_to_resume)
             self.board_to_resume = None
             self.ui.action_coordinates.setChecked(
                 self.are_coordinates_always_visible)
             self.on_view_coordinates(self.are_coordinates_always_visible)
         else:
-            self.board_to_resume = self.display.current_state
+            self.board_to_resume = self.game_display.current_state
             self.are_coordinates_always_visible = (
                 self.ui.action_coordinates.isChecked())
             self.ui.action_coordinates.setChecked(True)
             self.on_view_coordinates(True)
             choices.clear()
             choices.setRowCount(3)
             choices.setColumnCount(10)
             choices.resizeColumnsToContents()
             choices.resizeRowsToContents()
             choices.setMaximumHeight(choices.horizontalHeader().height() +
                                      choices.verticalHeader().length() +
                                      choices.horizontalScrollBar().height())
             self.ui.move_history.clear()
             self.ui.move_history.addItems(
-                [str(item) for item in self.display.log_display.items])
+                [str(item) for item in self.game_display.log_display.items])
             self.ui.move_history.setCurrentIndex(self.ui.move_history.count()-1)
 
         self.ui.resume_here.setVisible(is_review_visible)
         self.ui.move_history.setVisible(is_review_visible)
         self.ui.choices.setVisible(is_review_visible)
         self.ui.toggle_review.setText(self.review_names[is_review_visible])
-        if self.display is not None:
-            self.display.is_reviewing = is_review_visible
+        if self.game_display is not None:
+            self.game_display.is_reviewing = is_review_visible
         choices.setVisible(is_review_visible)
 
     def on_resume_here(self):
-        self.board_to_resume = self.display.current_state
+        self.board_to_resume = self.game_display.current_state
         self.is_history_dirty = True
         history_index = self.ui.move_history.currentIndex()
-        self.display.log_display.rewind_to(history_index)
+        self.game_display.log_display.rewind_to(history_index)
         self.on_toggle_review()
-        self.display.request_move()
+        self.game_display.request_move()
 
     def on_move_history(self, item_index: int):
-        assert self.display is not None
-        history_item = self.display.log_display.items[item_index]
-        self.display.update_board(history_item.game_state)
+        assert self.game_display is not None
+        history_item = self.game_display.log_display.items[item_index]
+        self.game_display.update_board(history_item.game_state)
         choices = self.ui.choices
         choices.clear()
         choices.setColumnCount(len(history_item.choices))
         choices.setVerticalHeaderLabels(['count', 'probability', 'value'])
         choices.setHorizontalHeaderLabels([choice[0]
                                            for choice in history_item.choices])
         for i, (choice,
@@ -226,33 +297,36 @@
                 value) in enumerate(history_item.choices):
             choices.setItem(0, i, QTableWidgetItem(f'{count}'))
             choices.setItem(1, i, QTableWidgetItem(f'{probability}'))
             choices.setItem(2, i, QTableWidgetItem(f'{value}'))
         choices.resizeColumnsToContents()
 
     def on_new_game(self):
-        if self.display is not None:
-            self.display.stop_workers()
-            self.display = None
+        self.stop_workers()
         self.ui.stacked_widget.setCurrentWidget(self.ui.game_page)
         self.setWindowTitle(self.get_collection_name())
 
+    def stop_workers(self):
+        if self.display is not None:
+            self.display.stop_workers()
+            self.display = self.game_display = None
+
     def show_game(self, display: GameDisplay):
-        QApplication.setOverrideCursor(Qt.WaitCursor)
-        self.display = display
+        QApplication.setOverrideCursor(Qt.CursorShape.WaitCursor)
+        self.display = self.game_display = display
         start_state = display.start_state
         self.start_state = start_state
         collection_name = self.get_collection_name()
         self.setWindowTitle(f'{collection_name} - {start_state.game_name}')
         self.ui.game_name.setText(start_state.game_name)
         settings = get_settings(start_state)
         is_locked = settings.value('searches_locked', False, bool)
         self.ui.searches_lock1.setChecked(is_locked)
         self.ui.searches_lock2.setChecked(is_locked)
-        search_count = settings.value('searches', 600, int)
+        search_count = settings.value('searches', DEFAULT_SEARCHES, int)
         self.ui.searches1.setValue(search_count)
         self.ui.searches2.setValue(search_count)
         self.ui.shuffle_players.setChecked(settings.value('shuffle_players',
                                                           False,
                                                           bool))
         heuristics = self.load_heuristics()
         player1_index = settings.value('player_1', 0, int)
@@ -272,14 +346,15 @@
         self.on_toggle_review()
         QApplication.restoreOverrideCursor()
 
     def on_player_changed(self, player: QComboBox, new_index: int):
         if new_index < 0:
             # Combo box was cleared.
             return
+        assert self.start_state is not None
         settings = get_settings(self.start_state)
         if player is self.ui.player1:
             searches = self.ui.searches1
             searches_label = self.ui.searches_label1
             searches_lock = self.ui.searches_lock1
             setting_name = 'player_1'
             row = 1
@@ -324,79 +399,161 @@
     def on_network1(self):
         file_name, _ = QFileDialog.getOpenFileName(
             self.ui.players_page,
             "Open a file for player 1's neural network.",
             filter='Checkpoint (*.h5)',
             options=QFileDialog.DontUseNativeDialog)
 
-    def on_start(self):
-        self.display.update_board(self.display.start_state)
+    def on_start(self) -> None:
+        self.game_start_time = datetime.now()
+        assert self.game_display is not None
+        assert self.start_state is not None
+        self.game_display.update_board(self.game_display.start_state)
         self.is_history_dirty = False
         ui = self.ui
         player_fields = [(ui.player1.currentData(), ui.searches1.value()),
                          (ui.player2.currentData(), ui.searches2.value())]
         is_shuffled = ui.shuffle_players.isChecked()
         settings = get_settings(self.start_state)
         settings.setValue('shuffle_players', is_shuffled)
         if is_shuffled:
             shuffle(player_fields)
         mcts_choices = {self.start_state.players[0]: player_fields[0],
                         self.start_state.players[1]: player_fields[1]}
-        self.display.mcts_players = [
+        self.game_display.mcts_players = [
             MctsPlayer(self.start_state,
                        player_number,
                        iteration_count=searches,
                        process_count=self.cpu_count)
             for player_number, (heuristic, searches) in mcts_choices.items()
             if heuristic is not None]
         layout: QGridLayout = ui.display_page.layout()
-        layout.replaceWidget(ui.game_display, self.display)
+        layout.replaceWidget(ui.game_display, self.game_display)
         ui.game_display.setVisible(False)
-        ui.game_display = self.display
-        self.display.setVisible(True)
-        self.display.show_coordinates = ui.action_coordinates.isChecked()
+        ui.game_display = self.game_display
+        self.game_display.setVisible(True)
+        self.game_display.show_coordinates = ui.action_coordinates.isChecked()
 
         self.on_view_game()
 
     def on_view_game(self):
-        if self.display is None:
+        if self.game_display is None:
             self.on_new_game()
         else:
             self.ui.stacked_widget.setCurrentWidget(self.ui.display_page)
-            self.display.update_board(self.display.current_state)
-            self.display.request_move()
+            self.game_display.update_board(self.game_display.current_state)
+            self.game_display.request_move()
 
     def on_view_coordinates(self, is_checked: bool):
-        if self.display is not None:
-            self.display.show_coordinates = is_checked
+        if self.game_display is not None:
+            self.game_display.show_coordinates = is_checked
+
+    def on_new_strength_test(self):
+        self.stop_workers()
+        self.ui.stacked_widget.setCurrentWidget(
+            self.ui.plot_strength_page)
+
+    def on_start_strength_test(self) -> None:
+        settings = get_settings()
+        ui = self.ui
+        settings.setValue('strength_test_game',
+                          ui.strength_test_game.currentText())
+        settings.setValue('strength_test_strengths',
+                          ui.strength_test_strengths.text())
+        settings.setValue('strength_test_min', ui.strength_test_min.value())
+        settings.setValue('strength_test_max', ui.strength_test_max.value())
+        game_display: GameDisplay = ui.strength_test_game.currentData()
+        start_state = game_display.start_state
+        players = [MctsPlayer(start_state, GameState.X_PLAYER),
+                   MctsPlayer(start_state, GameState.O_PLAYER)]
+        controller = PlayController(start_state, players)
+        player_definitions = ui.strength_test_strengths.text().split()
+        self.display = self.strength_canvas
+        assert self.db_session is not None
+        self.strength_canvas.start(self.db_session,
+                                   controller,
+                                   player_definitions,
+                                   ui.strength_test_min.value(),
+                                   ui.strength_test_max.value())
+        ui.stacked_widget.setCurrentWidget(
+            ui.plot_strength_display_page)
 
     def on_plot(self):
-        self.ui.stacked_widget.setCurrentWidget(self.ui.plot_page)
+        self.ui.stacked_widget.setCurrentWidget(self.ui.plot_history_page)
+        self.requery_plot()
+
+    def requery_plot(self) -> None:
+        display: GameDisplay = self.ui.history_game.currentData()
+        self.plot_canvas.game = display.start_state
+        settings = get_settings(display.start_state)
+        future_strength = settings.value('searches', DEFAULT_SEARCHES, int)
+        self.plot_canvas.requery(self.db_session, future_strength)
 
     def on_searches_changed(self, search_count: int):
         if self.ui.stacked_widget.currentWidget() is not self.ui.players_page:
             return
         if self.start_state is not None:
             settings = get_settings(self.start_state)
             settings.setValue('searches', search_count)
             settings.remove('game_count')
             settings.remove('last_score')
             settings.remove('streak_length')
 
     def on_game_ended(self, game_state: GameState):
         if (self.is_history_dirty or
-                self.display is None or
+                self.game_display is None or
                 self.ui.searches_lock1.isChecked()):
             return
+        db_session = self.db_session
+        if db_session is None:
+            return
+        game_record = GameRecord.find_or_create(db_session, game_state)
+        game_end_time = datetime.now()
+        game_duration = game_end_time - self.game_start_time
+        match_record = MatchRecord(game=game_record,
+                                   start_time=self.game_start_time,
+                                   total_seconds=round(game_duration.total_seconds()),
+                                   move_count=game_state.get_move_count())
+        db_session.add(match_record)
+        winner = game_state.get_winner()
+        mcts_player: typing.Optional[MctsPlayer]
+        for player_number in game_state.get_players():
+            mcts_player = self.game_display.get_player(player_number)
+            if mcts_player is None:
+                player_record = db_session.query(PlayerRecord).filter_by(
+                    type=PlayerRecord.HUMAN_TYPE).one_or_none()
+                if player_record is None:
+                    player_record = PlayerRecord(type=PlayerRecord.HUMAN_TYPE)
+                    db_session.add(player_record)
+            else:
+                player_record = db_session.query(PlayerRecord).filter_by(
+                    type=PlayerRecord.PLAYOUT_TYPE,
+                    iterations=mcts_player.iteration_count).one_or_none()
+                if player_record is None:
+                    player_record = PlayerRecord(type=PlayerRecord.PLAYOUT_TYPE,
+                                                 iterations=mcts_player.iteration_count)
+                    db_session.add(player_record)
+            if player_number == winner:
+                result = 1
+            elif winner == game_state.NO_PLAYER:
+                result = 0
+            else:
+                result = -1
+            match_player = MatchPlayerRecord(match=match_record,
+                                             player=player_record,
+                                             player_number=player_number,
+                                             result=result)
+            db_session.add(match_player)
+        db_session.commit()
         try:
-            mcts_player: MctsPlayer
-            mcts_player, = self.display.mcts_players
+            mcts_player, = self.game_display.mcts_players
         except ValueError:
             # Didn't have exactly one MCTS player
             return
+        assert mcts_player is not None
         winning_player = game_state.get_winner()
         if winning_player == mcts_player.player_number:
             score = -1
         elif winning_player == GameState.NO_PLAYER:
             score = 0
         else:
             score = 1
@@ -420,34 +577,53 @@
 
     def on_rules(self, display: GameDisplay):
         self.ui.stacked_widget.setCurrentWidget(self.ui.rules_page)
         rules_path = display.rules_path
         if rules_path is None:
             game_name = display.start_state.game_name
             rules_html = f'No rules found for {game_name}.'
+            self.ui.rules_text.setHtml(rules_html)
         else:
-            rules_file = QFile(rules_path)
-            rules_file.open(QFile.ReadOnly | QFile.Text)
-            rules_markdown = QTextStream(rules_file).readAll()
-            rules_html = convert_markdown(rules_markdown)
-
-        self.ui.rules_text.setHtml(rules_html)
+            self.ui.rules_text.setSource('qrc' + rules_path)
 
     def on_close_rules(self):
-        if self.display is None:
+        if self.game_display is None:
             page = self.ui.game_page
-        elif self.display.current_state == self.display.start_state:
+        elif self.game_display.current_state == self.game_display.start_state:
             page = self.ui.players_page
         else:
             page = self.ui.display_page
         self.ui.stacked_widget.setCurrentWidget(page)
 
+    def on_new_db(self):
+        settings = get_settings()
+        db_path = settings.value('db_path')
+        file_name, _ = QFileDialog.getSaveFileName(
+            self,
+            "Create a new database",
+            dir=db_path,
+            filter='Player databases (*.zpl)',
+            options=QFileDialog.DontUseNativeDialog)
+        if not file_name:
+            return
+        script_path = str(Path(__file__).parent / 'db')
+        database_path = Path(file_name).absolute()
+        settings.setValue('db_path', str(database_path))
+        database_url = get_database_url(database_path)
+        alembic_config = Config(config_args=immutabledict({
+            'script_location': script_path,
+            'sqlalchemy.url': database_url}))
+        command.upgrade(alembic_config, 'head')
+
+    def on_open_db(self):
+        pass
+
 
 def main():
     app = QApplication(sys.argv)
     window = ZeroPlayWindow()
     window.show()
-    return app.exec_()
+    return app.exec()
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `zero_play-0.4.0/zero_play/zero_play_images_rc.py` & `zero_play-0.5.0/zero_play/zero_play_images_rc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Resource object code (Python 3)
 # Created by: object code
 # Created by: The Resource Compiler for Qt version 5.15.1
 # WARNING! All changes made in this file will be lost!
 
-from PySide2 import QtCore
+from PySide6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x05\xd8\
 \x89\
 PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
 \x00\x00\x80\x00\x00\x00\x80\x08\x06\x00\x00\x00\xc3>a\xcb\
 \x00\x00\x00\x09pHYs\x00\x00\x0e\xc4\x00\x00\x0e\xc4\
```

### Comparing `zero_play-0.4.0/zero_play.egg-info/PKG-INFO` & `zero_play-0.5.0/zero_play.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,88 @@
 Metadata-Version: 2.1
 Name: zero-play
-Version: 0.4.0
+Version: 0.5.0
 Summary: Teach a computer to play any game
 Home-page: https://donkirkby.github.io/zero-play/
 Author: Don Kirkby
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/donkirkby/zero-play/issues
 Project-URL: Source, https://github.com/donkirkby/zero-play
-Description: # Zero Play [![Build Badge]][build] [![Coverage Badge]][codecov] [![PyPI Badge]][pypi]
-        ### Teach a computer to play any game
-        
-        [Build Badge]: https://travis-ci.org/donkirkby/zero-play.svg?branch=master
-        [build]: https://travis-ci.org/donkirkby/zero-play
-        [Coverage Badge]: https://codecov.io/github/donkirkby/zero-play/coverage.svg?branch=master
-        [codecov]: https://codecov.io/github/donkirkby/zero-play?branch=master
-        [PyPI Badge]: https://badge.fury.io/py/zero-play.svg
-        [pypi]: https://badge.fury.io/py/zero-play
-        [journal]: docs/journal
-        [screenshot]: https://donkirkby.github.io/zero-play/images/screenshot.png
-        
-        The zero play library is based on the ideas in the [AlphaGo Zero paper] and the
-        example Python code in the [alpha-zero-general project]. The goal of this
-        project is to make a reusable Python library that other projects can build on
-        to make powerful computer opponents for many different board games. An example
-        project that uses this library is [Shibumi Games].
-        
-        It includes a graphical display that you can use to play against the computer
-        opponent or another human.
-        
-        ![screenshot]
-        
-        [AlphaGo Zero paper]: https://deepmind.com/blog/alphago-zero-learning-scratch/
-        [alpha-zero-general project]: https://github.com/suragnair/alpha-zero-general
-        [Shibumi Games]: https://donkirkby.github.io/shibumi-games/
-        
-        ## Installing Zero Play
-        Even though Zero Play has a graphical display, it is a regular Python package,
-        so you can install it with `pip install zero-play`. If you haven't installed
-        Python packages before, read Brett Cannon's [quick-and-dirty guide].
-        
-        Then run it with the `zero_play` command.
-        
-        The default installation generates some errors about `bdist_wheel` that don't
-        seem to actually cause any problems. You can either ignore them, or install
-        `wheel` before installing Zero Play.
-        
-            pip install wheel
-            pip install zero-play
-            zero_play
-        
-        Known bug on Ubuntu 20.04:
-        
-        > qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though
-        > it was found.
-        
-        This is a [PySide2 bug] that is missing some dependencies. You can work around
-        it by installing those dependencies like this:
-        
-            sudo apt install libxcb-xinerama0
-        
-        [quick-and-dirty guide]: https://snarky.ca/a-quick-and-dirty-guide-on-how-to-install-packages-for-python/
-        [PySide2 bug]: https://bugreports.qt.io/browse/QTBUG-84749
-        
-        ## More Information
-        If you'd like to help out with the project, or add your own games, see the
-        `CONTRIBUTING.md` file in the source code. For all the details, look through the
-        design [journal] for the project.
-        
-        ## Related Projects
-        Here are some similar projects for inspiration or collaboration:
-        
-        * I already mentioned the [alpha-zero-general project]. It was a big inspiration, but I'm trying to build something
-            that's easier to add new games to, or use as a library within another project.
-        * [Galvanise] looks interesting. It's a mix of Python and C++, using Tensorflow. As of 2020, it looks like a single
-            developer, without much documentation. The games are defined with GDL, not Python code.
-        
-        [Galvanise]: https://github.com/richemslie/galvanise_zero
-        
 Keywords: boardgames alphazero machine learning mcts
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: ml
 Provides-Extra: ml-gpu
+License-File: LICENSE
+
+# Zero Play [![Build Badge]][build] [![Coverage Badge]][codecov] [![PyPI Badge]][pypi]
+### Teach a computer to play any game
+
+[Build Badge]: https://github.com/donkirkby/zero-play/actions/workflows/py-build.yml/badge.svg?branch=master
+[build]: https://github.com/donkirkby/zero-play/actions
+[Coverage Badge]: https://codecov.io/github/donkirkby/zero-play/coverage.svg?branch=master
+[codecov]: https://codecov.io/github/donkirkby/zero-play?branch=master
+[PyPI Badge]: https://badge.fury.io/py/zero-play.svg
+[pypi]: https://badge.fury.io/py/zero-play
+[journal]: docs/journal
+[screenshot]: https://donkirkby.github.io/zero-play/images/screenshot.png
+
+The zero play library is based on the ideas in the [AlphaGo Zero paper] and the
+example Python code in the [alpha-zero-general project]. The goal of this
+project is to make a reusable Python library that other projects can build on
+to make powerful computer opponents for many different board games. An example
+project that uses this library is [Shibumi Games].
+
+It includes a graphical display that you can use to play against the computer
+opponent or another human.
+
+![screenshot]
+
+[AlphaGo Zero paper]: https://deepmind.com/blog/alphago-zero-learning-scratch/
+[alpha-zero-general project]: https://github.com/suragnair/alpha-zero-general
+[Shibumi Games]: https://donkirkby.github.io/shibumi-games/
+
+## Installing Zero Play
+Even though Zero Play has a graphical display, it is a regular Python package,
+so you can install it with `pip install zero-play`. If you haven't installed
+Python packages before, read Brett Cannon's [quick-and-dirty guide].
+
+Then run it with the `zero_play` command.
+
+The default installation generates some errors about `bdist_wheel` that don't
+seem to actually cause any problems. You can either ignore them, or install
+`wheel` before installing Zero Play.
+
+    pip install wheel
+    pip install zero-play
+    zero_play
+
+Known bug on Ubuntu 20.04:
+
+> qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though
+> it was found.
+
+This is a [PySide2 bug] that is missing some dependencies. You can work around
+it by installing those dependencies like this:
+
+    sudo apt install libxcb-xinerama0
+
+[quick-and-dirty guide]: https://snarky.ca/a-quick-and-dirty-guide-on-how-to-install-packages-for-python/
+[PySide2 bug]: https://bugreports.qt.io/browse/QTBUG-84749
+
+## More Information
+If you'd like to help out with the project, or add your own games, see the
+`CONTRIBUTING.md` file in the source code. For all the details, look through the
+design [journal] for the project.
+
+## Related Projects
+Here are some similar projects for inspiration or collaboration:
+
+* I already mentioned the [alpha-zero-general project]. It was a big inspiration, but I'm trying to build something
+    that's easier to add new games to, or use as a library within another project.
+* [Galvanise] looks interesting. It's a mix of Python and C++, using Tensorflow. As of 2020, it looks like a single
+    developer, without much documentation. The games are defined with GDL, not Python code.
+
+[Galvanise]: https://github.com/richemslie/galvanise_zero
```

### Comparing `zero_play-0.4.0/zero_play.egg-info/entry_points.txt` & `zero_play-0.5.0/zero_play.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,7 @@
 [zero_play.heuristic]
 connect4 = zero_play.connect4.neural_net:NeuralNet
 playout = zero_play.playout:Playout
 
 [zero_play.player]
 human = zero_play.human_player:HumanPlayer
 mcts = zero_play.mcts_player:MctsPlayer
-
```

