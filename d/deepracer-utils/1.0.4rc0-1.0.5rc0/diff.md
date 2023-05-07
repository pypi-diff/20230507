# Comparing `tmp/deepracer-utils-1.0.4rc0.tar.gz` & `tmp/deepracer-utils-1.0.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepracer-utils-1.0.4rc0.tar", last modified: Thu Mar 30 19:46:12 2023, max compression
+gzip compressed data, was "deepracer-utils-1.0.5rc0.tar", last modified: Sun May  7 10:31:35 2023, max compression
```

## Comparing `deepracer-utils-1.0.4rc0.tar` & `deepracer-utils-1.0.5rc0.tar`

### file list

```diff
@@ -1,260 +1,260 @@
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.851212 deepracer-utils-1.0.4rc0/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       35 2021-11-14 14:06:51.000000 deepracer-utils-1.0.4rc0/.gitattributes
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1845 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/.gitignore
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1002 2021-11-14 14:06:51.000000 deepracer-utils-1.0.4rc0/LICENSE
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      101 2021-11-14 14:06:51.000000 deepracer-utils-1.0.4rc0/MANIFEST.in
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     4351 2023-03-30 19:46:12.851212 deepracer-utils-1.0.4rc0/PKG-INFO
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     3413 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/README.md
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.851212 deepracer-utils-1.0.4rc0/deepracer/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      145 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/deepracer/__init__.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      342 2021-11-14 14:06:51.000000 deepracer-utils-1.0.4rc0/deepracer/__main__.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      500 2023-03-30 19:46:12.851212 deepracer-utils-1.0.4rc0/deepracer/_version.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.779212 deepracer-utils-1.0.4rc0/deepracer/boto3_enhancer/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     2303 2021-11-14 14:06:51.000000 deepracer-utils-1.0.4rc0/deepracer/boto3_enhancer/__init__.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/deepracer/boto3_enhancer/models/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/deepracer/boto3_enhancer/models/deepracer/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.779212 deepracer-utils-1.0.4rc0/deepracer/boto3_enhancer/models/deepracer/2019-04-01/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   102470 2021-11-14 14:06:51.000000 deepracer-utils-1.0.4rc0/deepracer/boto3_enhancer/models/deepracer/2019-04-01/service-2.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.779212 deepracer-utils-1.0.4rc0/deepracer/console/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       61 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/deepracer/console/__init__.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     7842 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/deepracer/console/helper.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.779212 deepracer-utils-1.0.4rc0/deepracer/logs/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      322 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/deepracer/logs/__init__.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    16030 2023-03-29 12:56:34.000000 deepracer-utils-1.0.4rc0/deepracer/logs/handler.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    16576 2023-03-29 12:56:34.000000 deepracer-utils-1.0.4rc0/deepracer/logs/log.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    39268 2023-03-29 20:28:09.000000 deepracer-utils-1.0.4rc0/deepracer/logs/log_utils.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    17340 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/deepracer/logs/metrics.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      301 2023-03-29 12:56:34.000000 deepracer-utils-1.0.4rc0/deepracer/logs/misc.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.779212 deepracer-utils-1.0.4rc0/deepracer/model/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       82 2021-11-14 14:06:51.000000 deepracer-utils-1.0.4rc0/deepracer/model/__init__.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     3934 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/deepracer/model/visualization.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.779212 deepracer-utils-1.0.4rc0/deepracer/tracks/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       69 2021-11-14 14:06:51.000000 deepracer-utils-1.0.4rc0/deepracer/tracks/__init__.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    15519 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/deepracer/tracks/track_utils.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.779212 deepracer-utils-1.0.4rc0/deepracer/update_action_speeds/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    11604 2021-11-14 14:06:51.000000 deepracer-utils-1.0.4rc0/deepracer/update_action_speeds/action_space.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     2421 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/deepracer/update_action_speeds/updateActionSpeeds.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       77 2021-11-14 14:06:51.000000 deepracer-utils-1.0.4rc0/deepracer/utils.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.779212 deepracer-utils-1.0.4rc0/deepracer_utils.egg-info/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     4351 2023-03-30 19:46:12.000000 deepracer-utils-1.0.4rc0/deepracer_utils.egg-info/PKG-INFO
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    14162 2023-03-30 19:46:12.000000 deepracer-utils-1.0.4rc0/deepracer_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)        1 2023-03-30 19:46:12.000000 deepracer-utils-1.0.4rc0/deepracer_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      248 2023-03-30 19:46:12.000000 deepracer-utils-1.0.4rc0/deepracer_utils.egg-info/requires.txt
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       10 2023-03-30 19:46:12.000000 deepracer-utils-1.0.4rc0/deepracer_utils.egg-info/top_level.txt
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.779212 deepracer-utils-1.0.4rc0/docs/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1364 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/docs/development.md
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      324 2022-02-17 18:38:25.000000 deepracer-utils-1.0.4rc0/requirements.txt
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      336 2023-03-30 19:46:12.851212 deepracer-utils-1.0.4rc0/setup.cfg
--rwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)     1873 2022-07-11 06:48:52.000000 deepracer-utils-1.0.4rc0/setup.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/tests/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.775212 deepracer-utils-1.0.4rc0/tests/deepracer/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.779212 deepracer-utils-1.0.4rc0/tests/deepracer/boto3_enhancer/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      143 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/boto3_enhancer/test_boto3_client.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.779212 deepracer-utils-1.0.4rc0/tests/deepracer/console/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     4094 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/console/test_helper.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.779212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.783212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   112947 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612082853-IBZwYd0MRMqgwKlAe7bb0A-robomaker.log
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113488 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612083839-PMfF__s5QJSQT_-E0rEYwg-robomaker.log
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.783212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   106112 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703172842-wDhqXQC-SkGOinLUdZCQZQ-robomaker.log
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   107041 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703174103-zi4mg1gOTvugQLn-3BfL4g-robomaker.log
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.783212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/training/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   137849 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230350-EHNgTNY2T9-77qXhqjBi6A-sagemaker.log
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)  5707542 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230353-EHNgTNY2T9-77qXhqjBi6A-robomaker.log
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/metrics/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.787212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612082523-IBZwYd0MRMqgwKlAe7bb0A.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612083508-PMfF__s5QJSQT_-E0rEYwg.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.787212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/metrics/training/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   153326 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/metrics/training/training-20220611205309-EHNgTNY2T9-77qXhqjBi6A.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.787212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   115644 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.791212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   116427 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.803212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    81652 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/0-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    77042 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/1-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   155513 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/10-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   233071 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/11-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   162819 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/12-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   214043 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/13-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   252793 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/14-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   261410 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/15-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   209393 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/16-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   259528 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/17-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   235348 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/18-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   279330 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/19-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    72279 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/2-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   312243 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/20-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   434094 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/21-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   480156 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/22-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   378034 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/23-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   486461 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/24-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   555753 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/25-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   585741 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/26-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   658706 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/27-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    72306 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/3-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    85863 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/4-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    87398 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/5-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    92249 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/6-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114238 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/7-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   109345 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/8-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   131791 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/9-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.803212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.803212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   100069 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.803212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    97505 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.771212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.803212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    96515 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.803212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/ip/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      345 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/ip/hyperparameters.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.807212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      799 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200242.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      799 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200509.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      799 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200711.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   129562 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/TrainingMetrics.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.807212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/model/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1347 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/model/model_metadata.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      814 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/reward_function.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.819212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    81353 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/0-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    84136 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/1-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   168052 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/10-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   178087 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/11-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   214490 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/12-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   193144 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/13-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   194615 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/14-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   251890 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/15-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   227580 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/16-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   248032 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/17-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   320022 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/18-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   313286 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/19-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    73171 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/2-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   361801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/20-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   344302 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/21-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   434929 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/22-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   454222 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/23-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   374326 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/24-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   421050 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/25-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   460575 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/26-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    90695 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/3-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    93003 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/4-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    98389 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/5-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   112093 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/6-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    98816 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/7-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   146572 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/8-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   137178 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/9-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.775212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.775212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.827212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    47172 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/0-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    50573 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/1-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    96527 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/10-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   117657 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/11-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   101889 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/12-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    89625 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/13-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   148525 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/14-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   123770 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/15-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   106181 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/16-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   126631 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/17-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   174793 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/18-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   168419 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/19-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    39878 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/2-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   179810 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/20-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   156930 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/21-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   188297 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/22-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    48537 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/3-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    55379 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/4-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    85245 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/5-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    67049 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/6-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    77951 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/7-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    78538 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/8-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   139171 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/9-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.775212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.835212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    37614 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/0-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    43030 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/1-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    93980 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/10-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113794 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/11-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   107108 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/12-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   132614 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/13-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114432 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/14-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   149434 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/15-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   102219 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/16-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113987 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/17-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   135489 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/18-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   155853 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/19-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    47261 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/2-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   191968 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/20-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   110352 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/21-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   144271 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/22-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    43714 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/3-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    55034 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/4-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    52608 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/5-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    51339 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/6-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    68982 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/7-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   106093 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/8-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    77558 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/9-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.775212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.843212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    29966 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/0-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    26515 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/1-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   117025 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/10-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    83693 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/11-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    72713 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/12-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   111947 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/13-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113485 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/14-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   104342 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/15-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   122551 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/16-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114585 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/17-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   146897 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/18-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   170834 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/19-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    32485 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/2-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   138286 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/20-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   162069 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/21-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   149478 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/22-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    32675 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/3-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    44562 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/4-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    49757 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/5-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    57740 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/6-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    65111 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/7-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    91385 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/8-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    79828 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/9-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.775212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.847212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   109654 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.775212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.847212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114575 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.775212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.847212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   110747 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.847212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/ip/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      345 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/ip/hyperparameters.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.847212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201503.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201704.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201920.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    64134 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    51847 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_1.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    51846 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_2.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.847212 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/model/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1347 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/model/model_metadata.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    20184 2023-03-30 19:19:38.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/test_logs.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1793 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/logs/test_metrics.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-03-30 19:46:12.851212 deepracer-utils-1.0.4rc0/tests/deepracer/track_utils/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     2204 2022-08-11 19:53:40.000000 deepracer-utils-1.0.4rc0/tests/deepracer/track_utils/test_track_utils.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      397 2023-03-30 19:20:38.000000 deepracer-utils-1.0.4rc0/tox.ini
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    68691 2021-11-14 14:06:51.000000 deepracer-utils-1.0.4rc0/versioneer.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       35 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/.gitattributes
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1863 2023-05-07 10:31:02.000000 deepracer-utils-1.0.5rc0/.gitignore
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1002 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/LICENSE
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      101 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/MANIFEST.in
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     4350 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/PKG-INFO
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     3413 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/README.md
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/deepracer/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      145 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/__init__.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      342 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/deepracer/__main__.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      500 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/deepracer/_version.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     2303 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/__init__.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/models/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/models/deepracer/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/models/deepracer/2019-04-01/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   112300 2023-05-07 10:31:02.000000 deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/models/deepracer/2019-04-01/service-2.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/deepracer/console/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       61 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/console/__init__.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     7842 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/console/helper.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/deepracer/logs/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      322 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/logs/__init__.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    16030 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/deepracer/logs/handler.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    16576 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/deepracer/logs/log.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    39268 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/deepracer/logs/log_utils.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    17340 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/logs/metrics.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      301 2023-03-29 12:56:34.000000 deepracer-utils-1.0.5rc0/deepracer/logs/misc.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/deepracer/model/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       82 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/deepracer/model/__init__.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     3934 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/model/visualization.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/deepracer/tracks/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       69 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/deepracer/tracks/__init__.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    15519 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/tracks/track_utils.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/deepracer/update_action_speeds/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    11604 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/deepracer/update_action_speeds/action_space.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     2421 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/update_action_speeds/updateActionSpeeds.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       77 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/deepracer/utils.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     4350 2023-05-07 10:31:35.000000 deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    14162 2023-05-07 10:31:35.000000 deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)        1 2023-05-07 10:31:35.000000 deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      253 2023-05-07 10:31:35.000000 deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/requires.txt
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       10 2023-05-07 10:31:35.000000 deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/top_level.txt
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/docs/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1364 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/docs/development.md
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      295 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/requirements.txt
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      336 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/setup.cfg
+-rwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)     1877 2023-05-07 10:31:05.000000 deepracer-utils-1.0.5rc0/setup.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/tests/deepracer/boto3_enhancer/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      143 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/boto3_enhancer/test_boto3_client.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/tests/deepracer/console/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     4094 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/console/test_helper.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   112947 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612082853-IBZwYd0MRMqgwKlAe7bb0A-robomaker.log
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113488 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612083839-PMfF__s5QJSQT_-E0rEYwg-robomaker.log
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   106112 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703172842-wDhqXQC-SkGOinLUdZCQZQ-robomaker.log
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   107041 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703174103-zi4mg1gOTvugQLn-3BfL4g-robomaker.log
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/training/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   137849 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230350-EHNgTNY2T9-77qXhqjBi6A-sagemaker.log
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)  5707542 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230353-EHNgTNY2T9-77qXhqjBi6A-robomaker.log
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.884350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612082523-IBZwYd0MRMqgwKlAe7bb0A.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612083508-PMfF__s5QJSQT_-E0rEYwg.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.884350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/training/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   153326 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/training/training-20220611205309-EHNgTNY2T9-77qXhqjBi6A.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.884350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   115644 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.884350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   116427 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    81652 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/0-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    77042 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/1-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   155513 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/10-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   233071 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/11-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   162819 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/12-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   214043 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/13-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   252793 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/14-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   261410 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/15-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   209393 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/16-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   259528 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/17-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   235348 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/18-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   279330 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/19-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    72279 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/2-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   312243 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/20-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   434094 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/21-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   480156 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/22-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   378034 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/23-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   486461 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/24-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   555753 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/25-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   585741 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/26-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   658706 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/27-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    72306 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/3-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    85863 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/4-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    87398 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/5-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    92249 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/6-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114238 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/7-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   109345 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/8-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   131791 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/9-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   100069 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    97505 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    96515 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/ip/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      345 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/ip/hyperparameters.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      799 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200242.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      799 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200509.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      799 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200711.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   129562 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/TrainingMetrics.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/model/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1347 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/model/model_metadata.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      814 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/reward_function.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.904351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    81353 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/0-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    84136 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/1-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   168052 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/10-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   178087 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/11-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   214490 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/12-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   193144 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/13-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   194615 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/14-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   251890 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/15-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   227580 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/16-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   248032 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/17-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   320022 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/18-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   313286 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/19-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    73171 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/2-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   361801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/20-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   344302 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/21-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   434929 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/22-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   454222 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/23-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   374326 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/24-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   421050 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/25-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   460575 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/26-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    90695 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/3-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    93003 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/4-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    98389 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/5-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   112093 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/6-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    98816 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/7-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   146572 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/8-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   137178 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/9-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.912351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    47172 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/0-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    50573 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/1-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    96527 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/10-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   117657 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/11-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   101889 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/12-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    89625 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/13-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   148525 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/14-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   123770 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/15-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   106181 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/16-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   126631 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/17-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   174793 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/18-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   168419 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/19-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    39878 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/2-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   179810 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/20-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   156930 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/21-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   188297 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/22-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    48537 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/3-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    55379 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/4-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    85245 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/5-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    67049 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/6-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    77951 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/7-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    78538 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/8-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   139171 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/9-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.916351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    37614 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/0-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    43030 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/1-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    93980 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/10-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113794 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/11-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   107108 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/12-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   132614 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/13-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114432 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/14-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   149434 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/15-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   102219 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/16-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113987 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/17-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   135489 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/18-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   155853 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/19-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    47261 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/2-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   191968 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/20-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   110352 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/21-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   144271 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/22-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    43714 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/3-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    55034 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/4-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    52608 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/5-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    51339 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/6-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    68982 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/7-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   106093 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/8-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    77558 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/9-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.920351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    29966 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/0-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    26515 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/1-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   117025 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/10-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    83693 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/11-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    72713 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/12-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   111947 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/13-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113485 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/14-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   104342 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/15-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   122551 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/16-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114585 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/17-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   146897 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/18-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   170834 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/19-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    32485 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/2-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   138286 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/20-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   162069 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/21-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   149478 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/22-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    32675 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/3-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    44562 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/4-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    49757 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/5-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    57740 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/6-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    65111 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/7-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    91385 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/8-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    79828 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/9-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.920351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   109654 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.920351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114575 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.920351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   110747 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.920351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/ip/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      345 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/ip/hyperparameters.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201503.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201704.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201920.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    64134 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    51847 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_1.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    51846 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_2.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/model/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1347 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/model/model_metadata.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    20184 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/test_logs.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1793 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/test_metrics.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/tests/deepracer/track_utils/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     2373 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/tests/deepracer/track_utils/test_track_utils.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      397 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/tox.ini
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    68691 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/versioneer.py
```

### Comparing `deepracer-utils-1.0.4rc0/.gitignore` & `deepracer-utils-1.0.5rc0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -126,7 +126,10 @@
 
 # Pyre type checker
 .pyre/
 
 # vscode
 .vscode/launch.json
 .vscode/settings.json
+
+# intellij
+.idea
```

### Comparing `deepracer-utils-1.0.4rc0/LICENSE` & `deepracer-utils-1.0.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/PKG-INFO` & `deepracer-utils-1.0.5rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: deepracer-utils
-Version: 1.0.4rc0
+Version: 1.0.5rc0
 Summary: A set of tools for working with DeepRacer training
 Home-page: https://github.com/aws-deepracer-community/deepracer-utils/
 Author: AWS DeepRacer Community
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/aws-deepracer-community/deepracer-utils/issues
 Project-URL: Source, https://github.com/aws-deepracer-community/deepracer-utils/
 Keywords: aws deepracer awsdeepracer
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: Log Analysis
-Requires-Python: >=3.6.*, <4
+Requires-Python: >=3.6,<4.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: visualization
 License-File: LICENSE
 
 # Deepracer Utilities - Analyzing Your DeepRacer Model
```

### Comparing `deepracer-utils-1.0.4rc0/README.md` & `deepracer-utils-1.0.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/deepracer/boto3_enhancer/__init__.py` & `deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/__init__.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/deepracer/boto3_enhancer/models/deepracer/2019-04-01/service-2.json` & `deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/models/deepracer/2019-04-01/service-2.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8947107225650477%*

 * *Differences: {"'metadata'": "{'serviceId': 'DeepRacer'}",*

 * * "'operations'": "{'AddLeaderboardAccessPermission': {delete: ['errors']}, "*

 * *                 "'CloneReinforcementLearningModel': {delete: ['errors']}, 'CreateCar': {delete: "*

 * *                 "['errors']}, 'CreateLeaderboardAccessToken': {delete: ['errors']}, "*

 * *                 "'CreateLeaderboardSubmission': {delete: ['errors']}, "*

 * *                 "'CreateReinforcementLearningModel': {delete: ['errors']}, 'DeleteModel': "*

 * *                 "{delete: ['errors']} […]*

```diff
@@ -2,1565 +2,863 @@
     "documentation": "<p>AWS DeepRacer is the easiest way to get started with learning reinforcement learning. Visit <a href=\"https://aws.amazon.com/deepracer/\">https://aws.amazon.com/deepracer/</a> to learn more.</p>\n<p>While it is strongly recommended that you start interacting with DeepRacer through the AWS Console, all operations available on the website are also available programatically and through aws cli.</p>",
     "metadata": {
         "apiVersion": "2019-04-01",
         "endpointPrefix": "deepracer-prod",
         "jsonVersion": "1.1",
         "protocol": "json",
         "serviceFullName": "AWS DeepRacer",
-        "serviceId": "ID",
+        "serviceId": "DeepRacer",
         "signatureVersion": "v4",
         "signingName": "deepracer",
         "targetPrefix": "AwsSilverstoneCloudService",
         "uid": "deepracer-2019-04-01"
     },
     "operations": {
         "AddLeaderboardAccessPermission": {
             "documentation": "<p>Join a community race.</p><p>Using this method you can join the race without having to open the AWS DeepRacer Console.</p><p>When successful, the leaderboard for a given race will be available to you in the leaderboards list</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "TooManyRequestsException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "AddLeaderboardAccessPermissionRequest"
             },
             "name": "AddLeaderboardAccessPermission",
             "output": {
                 "shape": "AddLeaderboardAccessPermissionResponse"
             }
         },
-        "CloneReinforcementLearningModel": {
-            "documentation": "<p>Clones an existing model and continues training with new instructions</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceAlreadyExistsException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "TooManyRequestsException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "AdminGetAccountConfig": {
+            "documentation": "<p>TODO</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "CloneReinforcementLearningModelRequest"
+                "shape": "AdminGetAccountConfigRequest"
             },
-            "name": "CloneReinforcementLearningModel",
+            "name": "AdminGetAccountConfig",
             "output": {
-                "shape": "CloneReinforcementLearningModelResponse"
+                "shape": "AdminGetAccountConfigResponse"
             }
         },
-        "CreateAccountResources": {
-            "documentation": "<p>This method is no longer supported and should not be used.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceAlreadyExistsException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "AdminListAssociatedResources": {
+            "documentation": "<p>TODO</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "CreateAccountResourcesRequest"
+                "shape": "AdminListAssociatedResourcesRequest"
             },
-            "name": "CreateAccountResources",
+            "name": "AdminListAssociatedResources",
             "output": {
-                "shape": "CreateAccountResourcesResponse"
+                "shape": "AdminListAssociatedResourcesResponse"
             }
         },
-        "CreateCar": {
-            "documentation": "<p>Create a new car to train your model with.</p><p>You can choose various settings for your car including the action space, name or look.</p><p>There is a limit of 20 cars that you can create. If you reach this limit, update an existing car instead using update-car</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceLimitExceededException"
-                },
-                {
-                    "shape": "ResourceAlreadyExistsException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "AdminListAssociatedUsers": {
+            "documentation": "<p>TODO</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "CreateCarRequest"
+                "shape": "AdminListAssociatedUsersRequest"
             },
-            "name": "CreateCar",
+            "name": "AdminListAssociatedUsers",
             "output": {
-                "shape": "CreateCarResponse"
+                "shape": "AdminListAssociatedUsersResponse"
             }
         },
-        "CreateLeaderboardAccessToken": {
-            "documentation": "<p>Create a new invitation token for the community race. It is useful if your existing invitation link has been shared outside of your desired users.</p><p>To use the new token simply put it in place of [token] in url https://console.aws.amazon.com/deepracer/home#raceToken/[token]</p><p>Creation of a new access token makes the old token invalid.</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "TooManyRequestsException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "AdminManageUser": {
+            "documentation": "<p>TODO</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "CreateLeaderboardAccessTokenRequest"
+                "shape": "AdminManageUserRequest"
             },
-            "name": "CreateLeaderboardAccessToken",
+            "name": "AdminManageUser",
             "output": {
-                "shape": "CreateLeaderboardAccessTokenResponse"
+                "shape": "AdminManageUserResponse"
             }
         },
-        "CreateLeaderboardSubmission": {
-            "documentation": "<p>Submit a model to a race.</p><p>Simply choose the model and a race and your submission will be created</p><p>When creating your first submission you need to confirm that you accept the terms and conditions of it. If you don't, you will not be allowed to submit your entry.</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "TooManyRequestsException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "AdminSetAccountConfig": {
+            "documentation": "<p>TODO</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "CreateLeaderboardSubmissionRequest"
+                "shape": "AdminSetAccountConfigRequest"
             },
-            "name": "CreateLeaderboardSubmission",
+            "name": "AdminSetAccountConfig",
             "output": {
-                "shape": "CreateLeaderboardSubmissionResponse"
+                "shape": "AdminSetAccountConfigResponse"
             }
         },
-        "CreatePrivateLeaderboard": {
-            "documentation": "<p>Creates a community race</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ResourceAlreadyExistsException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "ResourceLimitExceededException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "CloneReinforcementLearningModel": {
+            "documentation": "<p>Clones an existing model and continues training with new instructions</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "CreatePrivateLeaderboardRequest"
+                "shape": "CloneReinforcementLearningModelRequest"
             },
-            "name": "CreatePrivateLeaderboard",
+            "name": "CloneReinforcementLearningModel",
             "output": {
-                "shape": "CreatePrivateLeaderboardResponse"
+                "shape": "CloneReinforcementLearningModelResponse"
             }
         },
-        "CreateReinforcementLearningModel": {
-            "documentation": "<p>Starts a new training with instructions provided.</p><p>A new model is created and used in the training session to gather experiences, then it is updated in the learning session based on the reward gathered.</p><p>While you can start training through the cli/boto3, it is recommended that you use the Deepracer Console instead for a richer experience.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceAlreadyExistsException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "TooManyRequestsException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "CreateCar": {
+            "documentation": "<p>Create a new car to train your model with.</p><p>You can choose various settings for your car including the action space, name or look.</p><p>There is a limit of 20 cars that you can create. If you reach this limit, update an existing car instead using update-car</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "CreateReinforcementLearningModelRequest"
+                "shape": "CreateCarRequest"
             },
-            "name": "CreateReinforcementLearningModel",
+            "name": "CreateCar",
             "output": {
-                "shape": "CreateReinforcementLearningModelResponse"
+                "shape": "CreateCarResponse"
             }
         },
-        "DeleteAccountResources": {
-            "documentation": "<p>This method is no longer supported and should not be used.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "CreateLeaderboard": {
+            "documentation": "<p>Creates a race</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "DeleteAccountResourcesRequest"
+                "shape": "CreateLeaderboardRequest"
             },
-            "name": "DeleteAccountResources",
+            "name": "CreateLeaderboard",
             "output": {
-                "shape": "DeleteAccountResourcesResponse"
+                "shape": "CreateLeaderboardResponse"
             }
         },
-        "DeleteCar": {
-            "documentation": "<p>This method is for internal use only and should not be used.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
+        "CreateLeaderboardAccessToken": {
+            "documentation": "<p>Create a new invitation token for the community race. It is useful if your existing invitation link has been shared outside of your desired users.</p><p>To use the new token simply put it in place of [token] in url https://console.aws.amazon.com/deepracer/home#raceToken/[token]</p><p>Creation of a new access token makes the old token invalid.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "DeleteCarRequest"
+                "shape": "CreateLeaderboardAccessTokenRequest"
             },
-            "internalonly": true,
-            "name": "DeleteCar",
+            "name": "CreateLeaderboardAccessToken",
             "output": {
-                "shape": "DeleteCarResponse"
+                "shape": "CreateLeaderboardAccessTokenResponse"
             }
         },
-        "DeleteCars": {
-            "documentation": "<p>This method is for internal use only and should not be used.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
+        "CreateLeaderboardSubmission": {
+            "documentation": "<p>Submit a model to a race.</p><p>Simply choose the model and a race and your submission will be created</p><p>When creating your first submission you need to confirm that you accept the terms and conditions of it. If you don't, you will not be allowed to submit your entry.</p>",
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "CreateLeaderboardSubmissionRequest"
+            },
+            "name": "CreateLeaderboardSubmission",
+            "output": {
+                "shape": "CreateLeaderboardSubmissionResponse"
+            }
+        },
+        "CreateReinforcementLearningModel": {
+            "documentation": "<p>Starts a new training with instructions provided.</p><p>A new model is created and used in the training session to gather experiences, then it is updated in the learning session based on the reward gathered.</p><p>While you can start training through the cli/boto3, it is recommended that you use the Deepracer Console instead for a richer experience.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "DeleteCarsRequest"
+                "shape": "CreateReinforcementLearningModelRequest"
             },
-            "internalonly": true,
-            "name": "DeleteCars",
+            "name": "CreateReinforcementLearningModel",
             "output": {
-                "shape": "DeleteCarsResponse"
+                "shape": "CreateReinforcementLearningModelResponse"
             }
         },
-        "DeleteModel": {
-            "documentation": "<p>Delete existing model.</p><p>This method lets you limit your AWS DeepRacer model storage costs ",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
+        "DeleteLeaderboard": {
+            "documentation": "<p>Deletes a race</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "DeleteModelRequest"
+                "shape": "DeleteLeaderboardRequest"
             },
-            "name": "DeleteModel",
+            "name": "DeleteLeaderboard",
             "output": {
-                "shape": "DeleteModelResponse"
+                "shape": "DeleteLeaderboardResponse"
             }
         },
-        "DeletePrivateLeaderboard": {
-            "documentation": "<p>Deletes a community race</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "TooManyRequestsException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "DeleteModel": {
+            "documentation": "<p>Delete existing model.</p><p>This method lets you limit your AWS DeepRacer model storage costs ",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "DeletePrivateLeaderboardRequest"
+                "shape": "DeleteModelRequest"
             },
-            "name": "DeletePrivateLeaderboard",
+            "name": "DeleteModel",
             "output": {
-                "shape": "DeletePrivateLeaderboardResponse"
+                "shape": "DeleteModelResponse"
             }
         },
-        "EditPrivateLeaderboard": {
-            "documentation": "<p>Updates a community race</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "TooManyRequestsException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "EditLeaderboard": {
+            "documentation": "<p>Updates a race</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "EditPrivateLeaderboardRequest"
+                "shape": "EditLeaderboardRequest"
             },
-            "name": "EditPrivateLeaderboard",
+            "name": "EditLeaderboard",
             "output": {
-                "shape": "EditPrivateLeaderboardResponse"
+                "shape": "EditLeaderboardResponse"
             }
         },
-        "GetAccountResources": {
-            "documentation": "<p>This method is no longer supported and should not be used.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "GetAccountConfig": {
+            "documentation": "<p>TODO</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "GetAccountResourcesRequest"
+                "shape": "GetAccountConfigRequest"
             },
-            "name": "GetAccountResources",
+            "name": "GetAccountConfig",
             "output": {
-                "shape": "GetAccountResourcesResponse"
+                "shape": "GetAccountConfigResponse"
             }
         },
         "GetAlias": {
             "documentation": "<p>Displays the racer alias assigned to given account</p>",
-            "errors": [
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "name": "GetAlias",
             "output": {
                 "shape": "GetAliasResponse"
             }
         },
         "GetAssetUrl": {
-            "documentation": "<p>Used to fetch various assets related to a model, training or race submission</p><p>Returns a Url that you can use to fetch things like logs, models etc.</p><p>Asset types prefixed with \"S3_\" are for copying assets to S3 (operations available in a model view under Actions->Copy to S3).",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
+            "documentation": "<p>Used to fetch various assets related to a model, training or race submission</p><p>Returns a Url that you can use to fetch things like logs, models etc.</p><p>Asset types prefixed with S3 are for copying assets to S3 (operations available in a model view under Actions->Copy to S3 ).",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetAssetUrlRequest"
             },
             "name": "GetAssetUrl",
             "output": {
                 "shape": "GetAssetUrlResponse"
             }
         },
+        "GetBYOAJob": {
+            "documentation": "<p>TODO</p>",
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "GetBYOAJobRequest"
+            },
+            "name": "GetBYOAJob",
+            "output": {
+                "shape": "GetBYOAJobResponse"
+            }
+        },
         "GetCar": {
             "documentation": "<p>Returns current car settings.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetCarRequest"
             },
             "name": "GetCar",
             "output": {
                 "shape": "GetCarResponse"
             }
         },
         "GetCars": {
             "documentation": "<p>Returns a list of configured cars</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetCarsRequest"
             },
             "name": "GetCars",
             "output": {
                 "shape": "GetCarsResponse"
             }
         },
         "GetEvaluation": {
             "documentation": "<p>Get evaluation details.</p><p>Returns information about a given evaluation</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetEvaluationRequest"
             },
             "name": "GetEvaluation",
             "output": {
                 "shape": "GetEvaluationResponse"
             }
         },
         "GetLatestUserSubmission": {
             "documentation": "<p>Returns information about the most recent model submission status</p><p>This is the information that you will see next to your name on the race page.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetLatestUserSubmissionRequest"
             },
             "name": "GetLatestUserSubmission",
             "output": {
                 "shape": "GetLatestUserSubmissionResponse"
             }
         },
         "GetLeaderboard": {
             "documentation": "<p>Returns a details for a race</p><p>Does not return the entrants ranking - that is available through ListLeaderboardSubmissions (list-leaderboard-submissions for AWS CLI).</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetLeaderboardRequest"
             },
             "name": "GetLeaderboard",
             "output": {
                 "shape": "GetLeaderboardResponse"
             }
         },
         "GetModel": {
             "documentation": "<p>Fetch information about the model</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetModelRequest"
             },
             "name": "GetModel",
             "output": {
                 "shape": "GetModelResponse"
             }
         },
-        "GetPrivateLeaderboard": {
-            "documentation": "<p>Returns a details for a race</p><p>Don't quote me on that but it does look like an aliast for GetLeaderboard (get-leaderboard) which returns both community and public leaderboards</p><p>Does not return the entrants ranking - that is available through ListLeaderboardSubmissions (list-leaderboard-submissions for AWS CLI).</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "GetRankedUserSubmission": {
+            "documentation": "<p>Returns current user's best submission for a given race.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "GetPrivateLeaderboardRequest"
+                "shape": "GetRankedUserSubmissionRequest"
             },
-            "name": "GetPrivateLeaderboard",
+            "name": "GetRankedUserSubmission",
             "output": {
-                "shape": "GetPrivateLeaderboardResponse"
+                "shape": "GetRankedUserSubmissionResponse"
             }
         },
-        "GetRankedUserSubmission": {
-            "documentation": "<p>Returns current user's best submission for a given race.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "GetRecords": {
+            "documentation": "<p>TODO</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
-            "input": {
-                "shape": "GetRankedUserSubmissionRequest"
-            },
-            "name": "GetRankedUserSubmission",
+            "name": "GetRecords",
             "output": {
-                "shape": "GetRankedUserSubmissionResponse"
+                "shape": "GetRecordsResponse"
             }
         },
         "GetTournament": {
             "documentation": "<p>TODO</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetTournamentRequest"
             },
             "name": "GetTournament",
             "output": {
                 "shape": "GetTournamentResponse"
             }
         },
         "GetTrack": {
             "documentation": "<p>Provides information about a given track.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetTrackRequest"
             },
             "name": "GetTrack",
             "output": {
                 "shape": "GetTrackResponse"
             }
         },
         "GetTrainingJob": {
             "documentation": "<p>Get information about how a model is being trained</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetTrainingJobRequest"
             },
             "name": "GetTrainingJob",
             "output": {
                 "shape": "GetTrainingJobResponse"
             }
         },
         "ImportModel": {
             "documentation": "<p>Import a model from S3 into console</p><p>Allows to import a model from backup or alternative training solution and clone for more training or submit to a race.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceAlreadyExistsException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ImportModelRequest"
             },
             "name": "ImportModel",
             "output": {
                 "shape": "ImportModelResponse"
             }
         },
+        "ListBYOAJobs": {
+            "documentation": "<p>TODO</p>",
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "ListBYOAJobsRequest"
+            },
+            "name": "ListBYOAJobs",
+            "output": {
+                "shape": "ListBYOAJobsResponse"
+            }
+        },
         "ListEvaluations": {
             "documentation": "<p>Returns a list of evaluations performed on a given model.</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListEvaluationsRequest"
             },
             "name": "ListEvaluations",
             "output": {
                 "shape": "ListEvaluationsResponse"
             }
         },
         "ListLeaderboardSubmissions": {
             "documentation": "<p>Returns an ordered list of a given race entries.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListLeaderboardSubmissionsRequest"
             },
             "name": "ListLeaderboardSubmissions",
             "output": {
                 "shape": "ListLeaderboardSubmissionsResponse"
             }
         },
         "ListLeaderboardWinners": {
             "documentation": "<p>TODO</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListLeaderboardWinnersRequest"
             },
             "name": "ListLeaderboardWinners",
             "output": {
                 "shape": "ListLeaderboardWinnersResponse"
             }
         },
         "ListLeaderboards": {
             "documentation": "<p>List races that current user has access to</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListLeaderboardsRequest"
             },
             "name": "ListLeaderboards",
             "output": {
                 "shape": "ListLeaderboardsResponse"
             }
         },
         "ListModels": {
             "documentation": "<p>List current user's models</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListModelsRequest"
             },
             "name": "ListModels",
             "output": {
                 "shape": "ListModelsResponse"
             }
         },
         "ListPrivateLeaderboardParticipants": {
             "documentation": "<p>Lists users which have joined a private race.</p><p>For public race Arn an empty list is returned</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListPrivateLeaderboardParticipantsRequest"
             },
             "name": "ListPrivateLeaderboardParticipants",
             "output": {
                 "shape": "ListPrivateLeaderboardParticipantsResponse"
             }
         },
-        "ListPrivateLeaderboards": {
-            "documentation": "<p>Lists community races that current user has created.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "ListPrivateLeaderboardsRequest"
-            },
-            "name": "ListPrivateLeaderboards",
-            "output": {
-                "shape": "ListPrivateLeaderboardsResponse"
-            }
-        },
-        "ListSubscribedPrivateLeaderboards": {
-            "documentation": "<p>Lists community races that current user has joined.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "ListTagsForResource": {
+            "documentation": "<p>TODO</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "ListSubscribedPrivateLeaderboardsRequest"
+                "shape": "ListTagsForResourceRequest"
             },
-            "name": "ListSubscribedPrivateLeaderboards",
+            "name": "ListTagsForResource",
             "output": {
-                "shape": "ListSubscribedPrivateLeaderboardsResponse"
+                "shape": "ListTagsForResourceResponse"
             }
         },
         "ListTracks": {
             "documentation": "<p>List available tracks</p>",
-            "errors": [
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListTracksRequest"
             },
             "name": "ListTracks",
             "output": {
                 "shape": "ListTracksResponse"
             }
         },
         "ListTrainingJobs": {
             "documentation": "<p>List current user's training jobs</p><p>Training jobs are associated with models that user has.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListTrainingJobsRequest"
             },
             "name": "ListTrainingJobs",
             "output": {
                 "shape": "ListTrainingJobsResponse"
             }
         },
-        "MigrateModels": {
-            "documentation": "<p>This method is no longer be relevant and you should not use it</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+        "PerformLeaderboardOperation": {
+            "documentation": "<p>TODO</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "MigrateModelsRequest"
+                "shape": "PerformLeaderboardOperationRequest"
             },
-            "name": "MigrateModels",
+            "name": "PerformLeaderboardOperation",
             "output": {
-                "shape": "MigrateModelsResponse"
+                "shape": "PerformLeaderboardOperationResponse"
             }
         },
         "RemoveLeaderboardAccessPermission": {
             "documentation": "<p>Removes a racer from a community race administrated by the current user.</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "TooManyRequestsException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "RemoveLeaderboardAccessPermissionRequest"
             },
             "name": "RemoveLeaderboardAccessPermission",
             "output": {
                 "shape": "RemoveLeaderboardAccessPermissionResponse"
             }
         },
         "RunTournament": {
             "documentation": "<p>TODO</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "RunTournamentRequest"
             },
             "name": "RunTournament",
             "output": {
                 "shape": "RunTournamentResponse"
             }
         },
         "SetAlias": {
-            "documentation": "<p>Set your racer name. You can only set your racer name once so choose wisely!</p>\n<p>The names are checked in terms approprietness. You may have your name rejected if a disallowed word is a substring of it.</p>",
-            "errors": [
-                {
-                    "shape": "ResourceAlreadyExistsException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
+            "documentation": "<p>Set your racer name.</p>\n<p>The names are checked in terms approprietness. You may have your name rejected if a disallowed word is a substring of it.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "SetAliasRequest"
             },
             "name": "SetAlias"
         },
+        "StartBYOAJob": {
+            "documentation": "<p>TODO</p>",
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "StartBYOAJobRequest"
+            },
+            "name": "StartBYOAJob",
+            "output": {
+                "shape": "StartBYOAJobResponse"
+            }
+        },
         "StartEvaluation": {
             "documentation": "<p>Evaluate your model in conditions of your choice.</p><p>This is a great opportunity to check how your model is doing without the entropy altering it actions which happens during the training. But there's more: you can try a different track, different racing format or even race your model against a car with another model that you have trained.</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceInUseException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "TooManyRequestsException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "StartEvaluationRequest"
             },
             "name": "StartEvaluation",
             "output": {
                 "shape": "StartEvaluationResponse"
             }
         },
+        "StopBYOAJob": {
+            "documentation": "<p>TODO</p>",
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "StopBYOAJobRequest"
+            },
+            "name": "StopBYOAJob",
+            "output": {
+                "shape": "StopBYOAJobResponse"
+            }
+        },
         "StopEvaluation": {
             "documentation": "<p>Stop performing evaluation</p><p>The system will still take some time to shut everything down, but the evaluation will have been stopped at the time of request</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "JobNotActiveException"
-                },
-                {
-                    "shape": "TooManyRequestsException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "StopEvaluationRequest"
             },
             "name": "StopEvaluation",
             "output": {
                 "shape": "StopEvaluationResponse"
             }
         },
         "StopTrainingReinforcementLearningModel": {
             "documentation": "<p>Stop the training job.</p><p>The training will be immediately interrupted and will perform a shutdown of the environment which can take a few minutes. Once done, you will be able to evaluate, clone or submit your model to a race. The interrupted iteration is discarded and only the last and the best complete iterations are being stored.</p>",
-            "errors": [
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "JobNotActiveException"
-                },
-                {
-                    "shape": "ServiceException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "StopTrainingReinforcementLearningModelRequest"
             },
             "name": "StopTrainingReinforcementLearningModel",
             "output": {
                 "shape": "StopTrainingReinforcementLearningModelResponse"
             }
         },
+        "TagResource": {
+            "documentation": "<p>TODO</p>",
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "TagResourceRequest"
+            },
+            "name": "TagResource",
+            "output": {
+                "shape": "TagResourceResponse"
+            }
+        },
         "TestRewardFunction": {
             "documentation": "<p>Test reward function. Submit your function to perform a number of tests against it.</p><p>Not all problems are clearly communicated even if caught, for instance whitespace issues. If you don't get the details that could help you, do revert to a code editor of your choice.</p>",
-            "errors": [
-                {
-                    "shape": "TooManyRequestsException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "TestRewardFunctionRequest"
             },
             "name": "TestRewardFunction",
             "output": {
                 "shape": "TestRewardFunctionResponse"
             }
         },
+        "UntagResource": {
+            "documentation": "<p>TODO</p>",
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "UntagResourceRequest"
+            },
+            "name": "UntagResource",
+            "output": {
+                "shape": "UntagResourceResponse"
+            }
+        },
         "UpdateCar": {
             "documentation": "<p>Change settings of your car</p><p>You can choose various settings for your car including the action space, name or look.</p><p>Changing the settings for a car only affects new models being created from scratch. Old models and their clones will continue to use the old settings which are stored with the model at the start of a new training and then passed on during cloning.</p>",
-            "errors": [
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "CustomerAuthorizationFailedException"
-                },
-                {
-                    "shape": "ResourceDoesNotExistException"
-                },
-                {
-                    "shape": "ResourceAlreadyExistsException"
-                },
-                {
-                    "shape": "ServiceException"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "UpdateCarRequest"
             },
             "name": "UpdateCar",
             "output": {
                 "shape": "UpdateCarResponse"
             }
+        },
+        "VerifyResourcesExistForTagris": {
+            "documentation": "<p>TODO</p>",
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "VerifyResourcesExistForTagrisRequest"
+            },
+            "name": "VerifyResourcesExistForTagris",
+            "output": {
+                "shape": "VerifyResourcesExistForTagrisResponse"
+            }
         }
     },
     "shapes": {
         "AccessToken": {
-            "max": 32,
-            "min": 1,
-            "pattern": "^[a-zA-Z0-9\\-_]+$",
+            "sensitive": true,
+            "type": "string"
+        },
+        "Accessories": {
+            "enum": [
+                "Blank",
+                "Prescription02",
+                "Round",
+                "Prescription01",
+                "Sunglasses",
+                "Wayfarers",
+                "Kurt"
+            ],
             "type": "string"
         },
         "AccountId": {
             "max": 12,
             "min": 12,
             "pattern": "[0-9]{12}",
             "type": "string"
         },
-        "AccountResources": {
+        "ActionSpace": {
             "members": {
-                "AccountRoles": {
-                    "shape": "AccountRoles"
+                "ActionSpaceType": {
+                    "shape": "ActionSpaceType"
                 },
-                "RoboMakerSimulationApplication": {
-                    "shape": "RoboMakerSimulationApplication"
+                "ContinuousActionSpace": {
+                    "shape": "ContinuousActionSpace"
                 },
-                "S3Bucket": {
-                    "shape": "S3Bucket"
-                },
-                "Status": {
-                    "shape": "AccountResourcesStatus"
-                },
-                "VersioningStatus": {
-                    "shape": "VersioningStatus"
-                },
-                "VpcStack": {
-                    "shape": "VpcStack"
+                "DiscreteActionSpace": {
+                    "shape": "DiscreteActionSpaceList"
                 }
             },
             "required": [
-                "AccountRoles"
+                "ActionSpaceType"
             ],
             "type": "structure"
         },
-        "AccountResourcesStatus": {
-            "enum": [
-                "CREATED",
-                "CREATING",
-                "DELETING",
-                "ERROR",
-                "MIGRATING"
-            ],
+        "ActionSpaceType": {
             "type": "string"
         },
-        "AccountRoles": {
-            "members": {
-                "CloudFormationRoleArn": {
-                    "shape": "RoleArn"
-                },
-                "DeepRacerRoleArn": {
-                    "shape": "RoleArn"
-                },
-                "LambdaRoleArn": {
-                    "shape": "RoleArn"
-                },
-                "RoboMakerRoleArn": {
-                    "shape": "RoleArn"
-                },
-                "SageMakerRoleArn": {
-                    "shape": "RoleArn"
-                }
-            },
-            "required": [
-                "DeepRacerRoleArn",
-                "SageMakerRoleArn",
-                "RoboMakerRoleArn",
-                "LambdaRoleArn",
-                "CloudFormationRoleArn"
-            ],
-            "type": "structure"
-        },
-        "ActionSpace": {
-            "members": {
-                "MaximumSpeed": {
-                    "shape": "MaximumSpeed"
-                },
-                "MaximumSteeringAngle": {
-                    "shape": "MaximumSteeringAngle"
-                },
-                "SpeedGranularity": {
-                    "shape": "SpeedGranularity"
-                },
-                "SteeringGranularity": {
-                    "shape": "SteeringGranularity"
-                }
-            },
-            "required": [
-                "MaximumSteeringAngle",
-                "SteeringGranularity",
-                "MaximumSpeed",
-                "SpeedGranularity"
-            ],
-            "type": "structure"
-        },
         "ActivityJob": {
             "members": {
                 "CreationTime": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
                 },
                 "EndTime": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
                 },
                 "FailureReason": {
                     "shape": "Description"
                 },
                 "LogDownloadComplete": {
-                    "shape": "Boolean"
+                    "shape": "boolean"
                 },
                 "MetricsPreSignedUrl": {
                     "shape": "Url"
                 },
                 "MetricsS3Path": {
                     "shape": "StandardLengthString"
                 },
                 "ModelArn": {
                     "shape": "ModelArn"
                 },
                 "StartTime": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
                 },
                 "Status": {
                     "shape": "ActivityStatus"
                 },
+                "VideoPreSignedUrl": {
+                    "shape": "Url"
+                },
                 "Videos": {
                     "shape": "ActivityVideos"
                 }
             },
             "required": [
-                "ModelArn",
                 "CreationTime",
                 "StartTime",
                 "Status"
             ],
             "type": "structure"
         },
         "ActivityJobStatus": {
@@ -1628,14 +926,17 @@
                 "shape": "ActivityVideo"
             }
         },
         "AddLeaderboardAccessPermissionRequest": {
             "members": {
                 "AccessToken": {
                     "shape": "AccessToken"
+                },
+                "UserIds": {
+                    "shape": "UserIds"
                 }
             },
             "required": [
                 "AccessToken"
             ],
             "type": "structure"
         },
@@ -1646,17 +947,126 @@
                 }
             },
             "required": [
                 "LeaderboardArn"
             ],
             "type": "structure"
         },
+        "AdminGetAccountConfigRequest": {
+            "members": {},
+            "type": "structure"
+        },
+        "AdminGetAccountConfigResponse": {
+            "members": {
+                "MultiracerConfig": {
+                    "shape": "MultiracerConfig"
+                }
+            },
+            "required": [
+                "MultiracerConfig"
+            ],
+            "type": "structure"
+        },
+        "AdminListAssociatedResourcesRequest": {
+            "members": {
+                "MaxResults": {
+                    "shape": "integer"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                },
+                "UserId": {
+                    "shape": "StandardLengthString"
+                }
+            },
+            "type": "structure"
+        },
+        "AdminListAssociatedResourcesResponse": {
+            "members": {
+                "AssociatedResources": {
+                    "shape": "AssociatedResources"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                }
+            },
+            "required": [
+                "AssociatedResources"
+            ],
+            "type": "structure"
+        },
+        "AdminListAssociatedUsersRequest": {
+            "members": {
+                "MaxResults": {
+                    "shape": "integer"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                },
+                "UserState": {
+                    "shape": "UserState"
+                }
+            },
+            "type": "structure"
+        },
+        "AdminListAssociatedUsersResponse": {
+            "members": {
+                "AssociatedUsers": {
+                    "shape": "AssociatedUsers"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                }
+            },
+            "required": [
+                "AssociatedUsers"
+            ],
+            "type": "structure"
+        },
+        "AdminManageUserRequest": {
+            "members": {
+                "Action": {
+                    "shape": "UserAction"
+                },
+                "Limits": {
+                    "shape": "UserLimits"
+                },
+                "UserIds": {
+                    "shape": "UserIds"
+                }
+            },
+            "required": [
+                "UserIds",
+                "Action"
+            ],
+            "type": "structure"
+        },
+        "AdminManageUserResponse": {
+            "members": {},
+            "type": "structure"
+        },
+        "AdminSetAccountConfigRequest": {
+            "members": {
+                "MultiracerConfig": {
+                    "shape": "MultiracerConfig"
+                }
+            },
+            "required": [
+                "MultiracerConfig"
+            ],
+            "type": "structure"
+        },
+        "AdminSetAccountConfigResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "AgentAlgorithm": {
             "enum": [
-                "PPO"
+                "PPO",
+                "SAC"
             ],
             "type": "string"
         },
         "AgentNetwork": {
             "enum": [
                 "SIX_LAYER_DOUBLE_HEAD_OUTPUT"
             ],
@@ -1687,21 +1097,100 @@
                 "S3_PKG_MODEL_LOGS",
                 "S3_PKG_MODEL",
                 "VIDEOS",
                 "ROBOMAKER_METRICS"
             ],
             "type": "string"
         },
+        "AssociatedResource": {
+            "members": {
+                "Models": {
+                    "shape": "ModelList"
+                },
+                "UserId": {
+                    "shape": "StandardLengthString"
+                }
+            },
+            "required": [
+                "UserId",
+                "Models"
+            ],
+            "type": "structure"
+        },
+        "AssociatedResources": {
+            "member": {
+                "shape": "AssociatedResource"
+            },
+            "type": "list"
+        },
+        "AssociatedUser": {
+            "members": {
+                "Alias": {
+                    "shape": "Alias"
+                },
+                "AssociatedOn": {
+                    "shape": "long"
+                },
+                "ComputeMinutesQueued": {
+                    "shape": "integer"
+                },
+                "ComputeMinutesUsed": {
+                    "shape": "integer"
+                },
+                "MaxModels": {
+                    "shape": "integer"
+                },
+                "MaxTotalComputeMinutes": {
+                    "shape": "integer"
+                },
+                "StorageBytesUsed": {
+                    "shape": "long"
+                },
+                "UserId": {
+                    "shape": "StandardLengthString"
+                },
+                "UserState": {
+                    "shape": "UserState"
+                }
+            },
+            "required": [
+                "Alias",
+                "UserId",
+                "AssociatedOn",
+                "ComputeMinutesUsed",
+                "ComputeMinutesQueued",
+                "MaxTotalComputeMinutes",
+                "MaxModels",
+                "StorageBytesUsed",
+                "UserState"
+            ],
+            "type": "structure"
+        },
+        "AssociatedUsers": {
+            "member": {
+                "shape": "AssociatedUser"
+            },
+            "type": "list"
+        },
+        "AttachedRewards": {
+            "member": {
+                "shape": "StandardLengthString"
+            },
+            "type": "list"
+        },
         "AutoSubmission": {
             "members": {
                 "AutoSubmissionStatus": {
                     "shape": "AutoSubmissionStatus"
                 },
                 "LeaderboardArn": {
                     "shape": "LeaderboardArn"
+                },
+                "TermsAccepted": {
+                    "shape": "boolean"
                 }
             },
             "required": [
                 "LeaderboardArn"
             ],
             "type": "structure"
         },
@@ -1711,21 +1200,115 @@
                 "SUBMITTED",
                 "TRAINING_FAILED",
                 "SUBMISSION_SQS_FAILED",
                 "SUBMISSION_REQUEST_FAILED"
             ],
             "type": "string"
         },
-        "Boolean": {
-            "type": "boolean"
+        "AvailableTrackFeatures": {
+            "members": {
+                "DefaultDirection": {
+                    "shape": "Direction"
+                },
+                "EnabledDirections": {
+                    "shape": "Directions"
+                }
+            },
+            "type": "structure"
         },
-        "BotCarSpeed": {
-            "max": 12,
-            "min": 0.2,
-            "type": "double"
+        "AvatarConfig": {
+            "members": {
+                "Accessories": {
+                    "shape": "Accessories"
+                },
+                "Clothing": {
+                    "shape": "Clothing"
+                },
+                "ClothingColor": {
+                    "shape": "ClothingColor"
+                },
+                "CountryCode": {
+                    "shape": "CountryCode"
+                },
+                "Eyebrows": {
+                    "shape": "Eyebrows"
+                },
+                "Eyes": {
+                    "shape": "Eyes"
+                },
+                "FacialHair": {
+                    "shape": "FacialHair"
+                },
+                "FacialHairColor": {
+                    "shape": "FacialHairColor"
+                },
+                "HairColor": {
+                    "shape": "HairColor"
+                },
+                "HatColor": {
+                    "shape": "HatColor"
+                },
+                "Mouth": {
+                    "shape": "Mouth"
+                },
+                "SkinColor": {
+                    "shape": "SkinColor"
+                },
+                "Top": {
+                    "shape": "Top"
+                },
+                "TshirtGraphic": {
+                    "shape": "TshirtGraphic"
+                }
+            },
+            "type": "structure"
+        },
+        "BYOAJob": {
+            "members": {
+                "ActivityJob": {
+                    "shape": "ActivityJob"
+                },
+                "Config": {
+                    "shape": "BYOAJobConfig"
+                },
+                "EventResourceConfig": {
+                    "shape": "ResourceConfig"
+                },
+                "EventResourcesConfigs": {
+                    "shape": "EventResourcesConfigs"
+                },
+                "JobArn": {
+                    "shape": "Arn"
+                },
+                "Name": {
+                    "shape": "StandardLengthString"
+                }
+            },
+            "required": [
+                "JobArn",
+                "ActivityJob"
+            ],
+            "type": "structure"
+        },
+        "BYOAJobConfig": {
+            "members": {
+                "TerminationConditions": {
+                    "shape": "TerminationConditions"
+                }
+            },
+            "required": [
+                "TerminationConditions"
+            ],
+            "type": "structure"
+        },
+        "BYOAJobs": {
+            "member": {
+                "shape": "BYOAJob"
+            },
+            "type": "list"
         },
         "Car": {
             "members": {
                 "Arn": {
                     "shape": "CarArn"
                 },
                 "Configuration": {
@@ -1752,25 +1335,25 @@
             "min": 1,
             "pattern": "^[a-zA-Z0-9\\-_]+$",
             "type": "string"
         },
         "CarConfiguration": {
             "members": {
                 "ActionSpace": {
+                    "description": "<p>This is not needed anymore, cars no longer have the action space associated with them</p>",
                     "shape": "ActionSpace"
                 },
                 "NeuralNetwork": {
                     "shape": "NeuralNetwork"
                 },
                 "Sensors": {
                     "shape": "SensorsList"
                 }
             },
             "required": [
-                "ActionSpace",
                 "NeuralNetwork",
                 "Sensors"
             ],
             "type": "structure"
         },
         "CarControlConfig": {
             "members": {
@@ -1837,14 +1420,20 @@
         },
         "CloneReinforcementLearningModelRequest": {
             "members": {
                 "AutoSubmission": {
                     "documentation": "<p>Decide whether after training completion you wish to submit the model to a race</p>",
                     "shape": "AutoSubmission"
                 },
+                "CarArn": {
+                    "shape": "CarArn"
+                },
+                "CustomActionSpace": {
+                    "shape": "ActionSpace"
+                },
                 "ModelArnToClone": {
                     "documentation": "<p>Identifies the base model that you wish to clone</p>",
                     "shape": "ModelArn"
                 },
                 "ModelDescription": {
                     "documentation": "<p>Descirption that you want to give to your new model</p>",
                     "shape": "Description"
@@ -1853,14 +1442,17 @@
                     "documentation": "<p>The name that you want to give to your new model</p>",
                     "shape": "ModelName"
                 },
                 "RoleArn": {
                     "documentation": "<p>Arn Role of the user that allows to perform this operation</p>",
                     "shape": "RoleArn"
                 },
+                "Tags": {
+                    "shape": "Tags"
+                },
                 "TrainingConfig": {
                     "documentation": "<p>Configuration of the training to be started after cloning</p>",
                     "shape": "TrainingConfig"
                 }
             },
             "required": [
                 "ModelName",
@@ -1876,76 +1468,154 @@
                 }
             },
             "required": [
                 "ModelArn"
             ],
             "type": "structure"
         },
+        "Clothing": {
+            "enum": [
+                "CollarSweater",
+                "Hoodie",
+                "Overall",
+                "BlazerSweater",
+                "BlazerShirt",
+                "ShirtCrewNeck",
+                "GraphicShirt",
+                "ShirtScoopNeck",
+                "ShirtVNeck"
+            ],
+            "type": "string"
+        },
+        "ClothingColor": {
+            "enum": [
+                "Blue01",
+                "Blue02",
+                "Blue03",
+                "Pink",
+                "Red",
+                "PastelBlue",
+                "PastelGreen",
+                "PastelOrange",
+                "PastelRed",
+                "PastelYellow",
+                "Gray01",
+                "Gray02",
+                "Heather",
+                "Black",
+                "White"
+            ],
+            "type": "string"
+        },
         "CodeBlock": {
             "max": 100000,
             "min": 1,
             "type": "string"
         },
-        "CreateAccountResourcesRequest": {
+        "ContinuousActionSpace": {
             "members": {
-                "AccountRoles": {
-                    "shape": "AccountRoles"
+                "Speed": {
+                    "shape": "SpeedRange"
+                },
+                "SteeringAngle": {
+                    "shape": "SteeringAngleRange"
                 }
             },
             "required": [
-                "AccountRoles"
+                "Speed",
+                "SteeringAngle"
             ],
             "type": "structure"
         },
-        "CreateAccountResourcesResponse": {
-            "members": {},
-            "type": "structure"
+        "CountryCode": {
+            "max": 3,
+            "min": 1,
+            "pattern": "^[A-Z]+$",
+            "type": "string"
         },
         "CreateCarRequest": {
             "members": {
                 "Car": {
                     "shape": "Car"
+                },
+                "Tags": {
+                    "shape": "Tags"
                 }
             },
+            "required": [
+                "Car"
+            ],
             "type": "structure"
         },
         "CreateCarResponse": {
             "members": {
                 "Car": {
                     "shape": "Car"
                 }
             },
             "type": "structure"
         },
         "CreateLeaderboardAccessTokenRequest": {
             "members": {
                 "ExpirationTime": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
                 },
                 "LeaderboardArn": {
                     "shape": "LeaderboardArn"
                 }
             },
             "required": [
-                "LeaderboardArn",
-                "ExpirationTime"
+                "LeaderboardArn"
             ],
             "type": "structure"
         },
         "CreateLeaderboardAccessTokenResponse": {
             "members": {
                 "AccessToken": {
                     "shape": "AccessToken"
                 }
             },
             "required": [
                 "AccessToken"
             ],
             "type": "structure"
         },
+        "CreateLeaderboardRequest": {
+            "members": {
+                "Definition": {
+                    "shape": "LeaderboardDefinition"
+                },
+                "Features": {
+                    "shape": "Features"
+                },
+                "RaceConfig": {
+                    "shape": "RaceConfig"
+                },
+                "Tags": {
+                    "shape": "Tags"
+                }
+            },
+            "required": [
+                "Definition",
+                "RaceConfig",
+                "Features"
+            ],
+            "type": "structure"
+        },
+        "CreateLeaderboardResponse": {
+            "members": {
+                "LeaderboardArn": {
+                    "shape": "Arn"
+                }
+            },
+            "required": [
+                "LeaderboardArn"
+            ],
+            "type": "structure"
+        },
         "CreateLeaderboardSubmissionRequest": {
             "members": {
                 "AutoSubmission": {
                     "shape": "AutoSubmission"
                 },
                 "LeaderboardArn": {
                     "shape": "LeaderboardArn"
@@ -1955,104 +1625,66 @@
                 },
                 "RoleArn": {
                     "shape": "RoleArn"
                 },
                 "SubmissionDescription": {
                     "shape": "Description"
                 },
+                "SubmissionOverrides": {
+                    "shape": "SubmissionOverrides"
+                },
                 "TermsAccepted": {
-                    "shape": "Boolean"
+                    "shape": "boolean"
+                },
+                "UserId": {
+                    "shape": "StandardLengthString"
                 }
             },
             "required": [
                 "ModelArn",
                 "LeaderboardArn"
             ],
             "type": "structure"
         },
         "CreateLeaderboardSubmissionResponse": {
             "members": {},
             "type": "structure"
         },
-        "CreatePrivateLeaderboardRequest": {
-            "members": {
-                "EndTime": {
-                    "shape": "epochTimeMillis"
-                },
-                "LeaderboardDescription": {
-                    "shape": "Description"
-                },
-                "LeaderboardImage": {
-                    "shape": "LeaderboardImage"
-                },
-                "LeaderboardName": {
-                    "shape": "LeaderboardName"
-                },
-                "MinimumLaps": {
-                    "shape": "PositiveInteger"
-                },
-                "StartTime": {
-                    "shape": "epochTimeMillis"
-                },
-                "TotalLaps": {
-                    "shape": "PositiveInteger"
-                },
-                "TrackArn": {
-                    "shape": "TrackArn"
-                }
-            },
-            "required": [
-                "LeaderboardName",
-                "LeaderboardDescription",
-                "MinimumLaps",
-                "TotalLaps",
-                "StartTime",
-                "EndTime",
-                "TrackArn",
-                "LeaderboardImage"
-            ],
-            "type": "structure"
-        },
-        "CreatePrivateLeaderboardResponse": {
-            "members": {
-                "LeaderboardArn": {
-                    "shape": "LeaderboardArn"
-                }
-            },
-            "required": [
-                "LeaderboardArn"
-            ],
-            "type": "structure"
-        },
         "CreateReinforcementLearningModelRequest": {
             "members": {
                 "AgentAlgorithm": {
                     "shape": "AgentAlgorithm"
                 },
                 "AgentNetwork": {
                     "shape": "AgentNetwork"
                 },
                 "AutoSubmission": {
                     "shape": "AutoSubmission"
                 },
                 "CarArn": {
                     "shape": "CarArn"
                 },
+                "CustomActionSpace": {
+                    "shape": "ActionSpace"
+                },
                 "ModelDescription": {
                     "shape": "Description"
                 },
                 "ModelFramework": {
                     "shape": "ModelFramework"
                 },
                 "ModelName": {
                     "shape": "ModelName"
                 },
                 "RoleArn": {
                     "shape": "RoleArn"
                 },
+                "Tags": {
+                    "shape": "Tags"
+                },
                 "TrainingConfig": {
                     "shape": "TrainingConfig"
                 }
             },
             "required": [
                 "ModelName",
                 "ModelFramework",
@@ -2069,47 +1701,26 @@
                 }
             },
             "required": [
                 "ModelArn"
             ],
             "type": "structure"
         },
-        "CustomerAuthorizationFailedException": {
-            "exception": true,
-            "members": {},
-            "type": "structure"
-        },
-        "DeleteAccountResourcesRequest": {
-            "members": {},
-            "type": "structure"
-        },
-        "DeleteAccountResourcesResponse": {
-            "members": {},
-            "type": "structure"
-        },
-        "DeleteCarRequest": {
+        "DeleteLeaderboardRequest": {
             "members": {
-                "Arn": {
-                    "shape": "CarArn"
+                "LeaderboardArn": {
+                    "shape": "LeaderboardArn"
                 }
             },
             "required": [
-                "Arn"
+                "LeaderboardArn"
             ],
             "type": "structure"
         },
-        "DeleteCarResponse": {
-            "members": {},
-            "type": "structure"
-        },
-        "DeleteCarsRequest": {
-            "members": {},
-            "type": "structure"
-        },
-        "DeleteCarsResponse": {
+        "DeleteLeaderboardResponse": {
             "members": {},
             "type": "structure"
         },
         "DeleteModelRequest": {
             "members": {
                 "ModelArn": {
                     "shape": "ModelArn"
@@ -2120,29 +1731,14 @@
             ],
             "type": "structure"
         },
         "DeleteModelResponse": {
             "members": {},
             "type": "structure"
         },
-        "DeletePrivateLeaderboardRequest": {
-            "members": {
-                "LeaderboardArn": {
-                    "shape": "LeaderboardArn"
-                }
-            },
-            "required": [
-                "LeaderboardArn"
-            ],
-            "type": "structure"
-        },
-        "DeletePrivateLeaderboardResponse": {
-            "members": {},
-            "type": "structure"
-        },
         "Description": {
             "max": 255,
             "min": 1,
             "pattern": "^.+$",
             "type": "string"
         },
         "Details": {
@@ -2162,62 +1758,93 @@
         },
         "DimensionList": {
             "member": {
                 "shape": "Dimension"
             },
             "type": "list"
         },
+        "Direction": {
+            "enum": [
+                "CLOCKWISE",
+                "COUNTER_CLOCKWISE"
+            ],
+            "type": "string"
+        },
+        "Directions": {
+            "member": {
+                "shape": "Direction"
+            },
+            "type": "list"
+        },
+        "DiscreteActionSpace": {
+            "members": {
+                "Speed": {
+                    "shape": "double"
+                },
+                "SteeringAngle": {
+                    "shape": "double"
+                }
+            },
+            "required": [
+                "Speed",
+                "SteeringAngle"
+            ],
+            "type": "structure"
+        },
+        "DiscreteActionSpaceList": {
+            "member": {
+                "shape": "DiscreteActionSpace"
+            },
+            "type": "list"
+        },
         "Division": {
             "max": 64,
             "min": 1,
             "type": "string"
         },
-        "EditPrivateLeaderboardRequest": {
+        "EditLeaderboardRequest": {
             "members": {
-                "EndTime": {
-                    "shape": "epochTimeMillis"
-                },
-                "LeaderboardArn": {
+                "Arn": {
                     "shape": "LeaderboardArn"
                 },
-                "LeaderboardDescription": {
-                    "shape": "Description"
+                "Definition": {
+                    "shape": "LeaderboardDefinition"
                 },
-                "LeaderboardImage": {
-                    "shape": "LeaderboardImage"
+                "Features": {
+                    "shape": "Features"
                 },
-                "MinimumLaps": {
-                    "shape": "PositiveInteger"
-                },
-                "StartTime": {
-                    "shape": "epochTimeMillis"
-                },
-                "TotalLaps": {
-                    "shape": "PositiveInteger"
-                },
-                "TrackArn": {
-                    "shape": "TrackArn"
+                "RaceConfig": {
+                    "shape": "RaceConfig"
                 }
             },
             "required": [
-                "LeaderboardArn",
-                "LeaderboardDescription",
-                "MinimumLaps",
-                "TotalLaps",
-                "StartTime",
-                "EndTime",
-                "TrackArn",
-                "LeaderboardImage"
+                "Arn",
+                "Definition",
+                "RaceConfig",
+                "Features"
             ],
             "type": "structure"
         },
-        "EditPrivateLeaderboardResponse": {
+        "EditLeaderboardResponse": {
             "members": {},
             "type": "structure"
         },
+        "EnabledConsoles": {
+            "member": {
+                "shape": "StandardLengthString"
+            },
+            "type": "list"
+        },
+        "EntryMode": {
+            "enum": [
+                "OPEN_DOOR",
+                "CLOSED_DOOR"
+            ],
+            "type": "string"
+        },
         "EntryTypeConfig": {
             "members": {
                 "InvitationEntryType": {
                     "shape": "StandardLengthString"
                 },
                 "RacingDivisionEntryType": {
                     "shape": "StandardLengthString"
@@ -2262,31 +1889,37 @@
             "member": {
                 "shape": "ErrorDetails"
             },
             "type": "list"
         },
         "EvaluationConfig": {
             "members": {
+                "EvaluationName": {
+                    "shape": "StandardLengthString"
+                },
                 "HeadToHeadConfig": {
                     "shape": "HeadToHeadConfig"
                 },
                 "ObjectAvoidanceConfig": {
                     "shape": "ObjectAvoidanceConfig"
                 },
                 "RaceType": {
                     "shape": "RaceType"
                 },
                 "ResettingBehaviorConfig": {
-                    "shape": "ResettingBehaviorConfig"
+                    "shape": "ResettingBehaviourConfig"
                 },
                 "TerminationConditions": {
                     "shape": "EvaluationTerminationConditions"
                 },
                 "TrackArn": {
-                    "shape": "StandardLengthString"
+                    "shape": "TrackArn"
+                },
+                "TrackFeatures": {
+                    "shape": "TrackFeatures"
                 }
             },
             "required": [
                 "TrackArn",
                 "TerminationConditions"
             ],
             "type": "structure"
@@ -2298,14 +1931,17 @@
                 },
                 "Config": {
                     "shape": "EvaluationConfig"
                 },
                 "JobArn": {
                     "shape": "EvaluationJobArn"
                 },
+                "LeaderboardArn": {
+                    "shape": "LeaderboardArn"
+                },
                 "Metrics": {
                     "shape": "EvaluationMetrics"
                 },
                 "RoboMakerJobArn": {
                     "shape": "Arn"
                 }
             },
@@ -2328,79 +1964,261 @@
                 "shape": "EvaluationJob"
             },
             "type": "list"
         },
         "EvaluationMetric": {
             "members": {
                 "CompletionPercentage": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
+                },
+                "CrashCount": {
+                    "shape": "integer"
                 },
                 "ElapsedTimeInMilliseconds": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
                 },
                 "EpisodeStatus": {
                     "shape": "EpisodeStatus"
                 },
+                "OffTrackCount": {
+                    "shape": "integer"
+                },
+                "ResetCount": {
+                    "shape": "integer"
+                },
                 "Trial": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
                 }
             },
             "type": "structure"
         },
         "EvaluationMetrics": {
             "member": {
                 "shape": "EvaluationMetric"
             },
             "type": "list"
         },
         "EvaluationTerminationConditions": {
             "members": {
                 "MaxLaps": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
                 },
                 "MaxTimeInMinutes": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
+                }
+            },
+            "type": "structure"
+        },
+        "EventResourceConfig": {
+            "members": {
+                "Metadata": {
+                    "shape": "StandardLengthString"
+                },
+                "ResourceArn": {
+                    "shape": "Arn"
+                },
+                "Type": {
+                    "shape": "StandardLengthString"
+                },
+                "Urls": {
+                    "shape": "ResourceUrls"
                 }
             },
+            "required": [
+                "Type",
+                "Urls"
+            ],
             "type": "structure"
         },
-        "GetAccountResourcesRequest": {
+        "EventResourcesConfigs": {
+            "member": {
+                "shape": "EventResourceConfig"
+            },
+            "type": "list"
+        },
+        "EventSchedule": {
+            "members": {
+                "EndTime": {
+                    "shape": "long"
+                },
+                "LeaderboardArn": {
+                    "shape": "Arn"
+                },
+                "StartTime": {
+                    "shape": "long"
+                }
+            },
+            "required": [
+                "StartTime",
+                "EndTime"
+            ],
+            "type": "structure"
+        },
+        "EventScheduleList": {
+            "member": {
+                "shape": "EventSchedule"
+            },
+            "type": "list"
+        },
+        "Eyebrows": {
+            "enum": [
+                "Angry",
+                "AngryNatural",
+                "SadConcerned",
+                "SadConcernedNatural",
+                "RaisedExcited",
+                "RaisedExcitedNatural",
+                "DefaultNatural",
+                "Default",
+                "FlatNatural",
+                "UpDown",
+                "UpDownNatural",
+                "UnibrowNatural"
+            ],
+            "type": "string"
+        },
+        "Eyes": {
+            "enum": [
+                "Close",
+                "Cry",
+                "Default",
+                "EyeRoll",
+                "Happy",
+                "Hearts",
+                "Side",
+                "Squint",
+                "Surprised",
+                "Wink",
+                "WinkWacky"
+            ],
+            "type": "string"
+        },
+        "FacialHair": {
+            "enum": [
+                "Blank",
+                "BeardMajestic",
+                "BeardMedium",
+                "MoustacheFancy",
+                "BeardLight",
+                "MoustacheMagnum"
+            ],
+            "type": "string"
+        },
+        "FacialHairColor": {
+            "enum": [
+                "Red",
+                "Black",
+                "BlondeGolden",
+                "Blonde",
+                "Platinum",
+                "Auburn",
+                "Brown",
+                "BrownDark"
+            ],
+            "type": "string"
+        },
+        "Features": {
+            "members": {
+                "AttachedRewards": {
+                    "shape": "AttachedRewards"
+                },
+                "CountryStatsEnabled": {
+                    "shape": "boolean"
+                },
+                "Playoff": {
+                    "shape": "PlayoffFeature"
+                },
+                "RacingDivisionEnabled": {
+                    "shape": "boolean"
+                },
+                "Theme": {
+                    "shape": "ThemeConfig"
+                }
+            },
+            "type": "structure"
+        },
+        "GetAccountConfigRequest": {
             "members": {},
             "type": "structure"
         },
-        "GetAccountResourcesResponse": {
+        "GetAccountConfigResponse": {
             "members": {
-                "AccountResources": {
-                    "shape": "AccountResources"
+                "MultiRacer": {
+                    "shape": "boolean"
                 }
             },
             "required": [
-                "AccountResources"
+                "MultiRacer"
             ],
             "type": "structure"
         },
         "GetAliasResponse": {
             "members": {
                 "Alias": {
                     "shape": "Alias"
+                },
+                "AlternativeEmail": {
+                    "shape": "StandardLengthString"
+                },
+                "CompetitionCountryCode": {
+                    "shape": "CountryCode"
+                },
+                "FirstName": {
+                    "shape": "StandardLengthString"
+                },
+                "FirstRaceTime": {
+                    "shape": "long"
+                },
+                "LastName": {
+                    "shape": "StandardLengthString"
+                },
+                "MiddleName": {
+                    "shape": "StandardLengthString"
+                },
+                "MultiUserEnabled": {
+                    "shape": "boolean"
+                },
+                "MultiUserProfile": {
+                    "shape": "MultiUserProfile"
+                },
+                "ProfileId": {
+                    "shape": "StandardLengthString"
+                },
+                "RacingDivisionConfig": {
+                    "shape": "RacingDivisionConfig"
+                },
+                "RacingDivisionsByRaceType": {
+                    "shape": "RacingDivisionsByRaceType"
+                },
+                "Rewards": {
+                    "shape": "Rewards"
+                },
+                "TeamName": {
+                    "shape": "StandardLengthString"
+                },
+                "UserAvatarConfig": {
+                    "shape": "AvatarConfig"
+                },
+                "UserId": {
+                    "shape": "StandardLengthString"
                 }
             },
-            "required": [
-                "Alias"
-            ],
             "type": "structure"
         },
         "GetAssetUrlRequest": {
             "members": {
                 "Arn": {
                     "shape": "Arn"
                 },
                 "AssetType": {
                     "shape": "AssetType"
                 },
+                "FirstCopy": {
+                    "shape": "boolean"
+                },
                 "ModelArtifactsS3Bucket": {
                     "shape": "S3Bucket"
                 },
                 "ModelArtifactsS3Prefix": {
                     "shape": "S3ObjectKey"
                 },
                 "RoleArn": {
@@ -2412,20 +2230,45 @@
                 "Arn",
                 "AssetType"
             ],
             "type": "structure"
         },
         "GetAssetUrlResponse": {
             "members": {
+                "ProcessedFileCount": {
+                    "shape": "integer"
+                },
                 "Url": {
                     "shape": "Url"
                 }
             },
             "type": "structure"
         },
+        "GetBYOAJobRequest": {
+            "members": {
+                "BYOAJobArn": {
+                    "shape": "Arn"
+                }
+            },
+            "required": [
+                "BYOAJobArn"
+            ],
+            "type": "structure"
+        },
+        "GetBYOAJobResponse": {
+            "members": {
+                "BYOAJob": {
+                    "shape": "BYOAJob"
+                }
+            },
+            "required": [
+                "BYOAJob"
+            ],
+            "type": "structure"
+        },
         "GetCarRequest": {
             "members": {
                 "Arn": {
                     "shape": "CarArn"
                 }
             },
             "required": [
@@ -2438,21 +2281,50 @@
                 "Car": {
                     "shape": "Car"
                 }
             },
             "type": "structure"
         },
         "GetCarsRequest": {
-            "members": {},
+            "members": {
+                "MaxResults": {
+                    "shape": "integer"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                }
+            },
             "type": "structure"
         },
         "GetCarsResponse": {
             "members": {
                 "Cars": {
                     "shape": "CarsList"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                }
+            },
+            "type": "structure"
+        },
+        "GetConflictingEventSchedulesRequest": {
+            "members": {
+                "EndTime": {
+                    "shape": "long"
+                },
+                "StartTime": {
+                    "shape": "long"
+                }
+            },
+            "type": "structure"
+        },
+        "GetConflictingEventSchedulesResponse": {
+            "members": {
+                "EventScheduleList": {
+                    "shape": "EventScheduleList"
                 }
             },
             "type": "structure"
         },
         "GetEvaluationRequest": {
             "members": {
                 "EvaluationJobArn": {
@@ -2534,33 +2406,14 @@
                 }
             },
             "required": [
                 "Model"
             ],
             "type": "structure"
         },
-        "GetPrivateLeaderboardRequest": {
-            "members": {
-                "LeaderboardArn": {
-                    "shape": "LeaderboardArn"
-                }
-            },
-            "required": [
-                "LeaderboardArn"
-            ],
-            "type": "structure"
-        },
-        "GetPrivateLeaderboardResponse": {
-            "members": {
-                "PrivateLeaderboard": {
-                    "shape": "PrivateLeaderboard"
-                }
-            },
-            "type": "structure"
-        },
         "GetRankedUserSubmissionRequest": {
             "members": {
                 "LeaderboardArn": {
                     "shape": "LeaderboardArn"
                 }
             },
             "required": [
@@ -2575,14 +2428,22 @@
                 }
             },
             "required": [
                 "LeaderboardSubmission"
             ],
             "type": "structure"
         },
+        "GetRecordsResponse": {
+            "members": {
+                "TrackRecords": {
+                    "shape": "TrackRecordList"
+                }
+            },
+            "type": "structure"
+        },
         "GetTournamentRequest": {
             "members": {
                 "LeaderboardArn": {
                     "shape": "LeaderboardArn"
                 }
             },
             "required": [
@@ -2590,14 +2451,17 @@
             ],
             "type": "structure"
         },
         "GetTournamentResponse": {
             "members": {
                 "Tournament": {
                     "shape": "TournamentResults"
+                },
+                "TournamentStatus": {
+                    "shape": "TournamentStatus"
                 }
             },
             "required": [
                 "Tournament"
             ],
             "type": "structure"
         },
@@ -2641,36 +2505,101 @@
                 }
             },
             "required": [
                 "TrainingJob"
             ],
             "type": "structure"
         },
+        "GrandPrix": {
+            "members": {
+                "RaceArn": {
+                    "shape": "Arn"
+                },
+                "ResultReleaseTime": {
+                    "shape": "long"
+                }
+            },
+            "required": [
+                "RaceArn",
+                "ResultReleaseTime"
+            ],
+            "type": "structure"
+        },
+        "HairColor": {
+            "enum": [
+                "Red",
+                "PastelPink",
+                "SilverGray",
+                "Black",
+                "BlondeGolden",
+                "Blonde",
+                "Platinum",
+                "Auburn",
+                "Brown",
+                "BrownDark"
+            ],
+            "type": "string"
+        },
+        "HatColor": {
+            "enum": [
+                "Blue01",
+                "Blue02",
+                "Blue03",
+                "Pink",
+                "Red",
+                "PastelBlue",
+                "PastelGreen",
+                "PastelOrange",
+                "PastelRed",
+                "PastelYellow",
+                "Gray01",
+                "Gray02",
+                "Heather",
+                "Black",
+                "White"
+            ],
+            "type": "string"
+        },
         "HeadToHeadConfig": {
             "members": {
                 "BotCarSpeed": {
-                    "shape": "BotCarSpeed"
+                    "shape": "double"
                 },
                 "EnableLaneChange": {
                     "shape": "boolean"
                 },
                 "HeadToHeadType": {
                     "shape": "HeadToHeadType"
                 },
                 "LowerLaneChangeTime": {
-                    "shape": "LaneChangeTime"
+                    "shape": "double"
                 },
                 "NumBotCars": {
-                    "shape": "NumBotCars"
+                    "shape": "integer"
+                },
+                "NumObstacles": {
+                    "shape": "integer"
+                },
+                "ObstaclePositions": {
+                    "shape": "ObstaclePositionList"
+                },
+                "ObstacleType": {
+                    "shape": "ObstacleType"
                 },
                 "PolicyModelArn": {
                     "shape": "ModelArn"
                 },
+                "PolicyModelName": {
+                    "shape": "StandardLengthString"
+                },
+                "RandomizeLocation": {
+                    "shape": "boolean"
+                },
                 "UpperLaneChangeTime": {
-                    "shape": "LaneChangeTime"
+                    "shape": "double"
                 }
             },
             "required": [
                 "HeadToHeadType"
             ],
             "type": "structure"
         },
@@ -2698,102 +2627,102 @@
                     "documentation": "<p>A name to be given to imported model</p>",
                     "shape": "ModelName"
                 },
                 "RoleArn": {
                     "documentation": "<p>An Arn of a role that current user has assigned, which allows to fetch files from that bucket</p>",
                     "shape": "RoleArn"
                 },
+                "TargetUserId": {
+                    "shape": "StandardLengthString"
+                },
                 "Type": {
                     "documentation": "<p>Type of model to import</p>",
                     "shape": "ModelType"
                 }
             },
             "required": [
+                "Type",
                 "Name",
                 "ModelArtifactsS3Path",
-                "RoleArn",
-                "Type"
+                "RoleArn"
             ],
             "type": "structure"
         },
         "ImportModelResponse": {
             "members": {
                 "ModelArn": {
                     "shape": "ModelArn"
                 }
             },
             "required": [
                 "ModelArn"
             ],
             "type": "structure"
         },
-        "InvalidRequestException": {
-            "exception": true,
-            "members": {},
-            "type": "structure"
-        },
-        "JobNotActiveException": {
-            "exception": true,
-            "members": {},
-            "type": "structure"
-        },
-        "LaneChangeTime": {
-            "max": 8.0,
-            "min": 1.0,
-            "type": "double"
-        },
         "Leaderboard": {
             "members": {
+                "AccessToken": {
+                    "shape": "AccessToken"
+                },
                 "Arn": {
                     "shape": "LeaderboardArn"
                 },
+                "AttachedRewards": {
+                    "shape": "AttachedRewards"
+                },
                 "CarControlConfig": {
                     "shape": "CarControlConfig"
                 },
                 "CloseTime": {
                     "shape": "epochTimeMillis"
                 },
+                "CountryStatsEnabled": {
+                    "shape": "boolean"
+                },
                 "Description": {
                     "shape": "Description"
                 },
                 "EndTime": {
                     "shape": "epochTimeMillis"
                 },
+                "EventResourceConfig": {
+                    "shape": "ResourceConfig"
+                },
                 "HeadToHeadConfig": {
                     "shape": "HeadToHeadConfig"
                 },
-                "ImageUrl": {
-                    "shape": "StandardLengthString"
-                },
                 "LaunchTime": {
                     "shape": "epochTimeMillis"
                 },
-                "LeaderboardImage": {
-                    "shape": "StandardLengthString"
+                "LeaderboardAccessRoles": {
+                    "shape": "LeaderboardAccessRoles"
                 },
                 "LeagueType": {
                     "shape": "StandardLengthString"
                 },
                 "MinimumLaps": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
+                },
+                "ModerateConfig": {
+                    "shape": "ModerateConfig"
                 },
                 "Moderated": {
                     "shape": "boolean"
                 },
                 "Name": {
                     "shape": "LeaderboardName"
                 },
                 "NumOfTeamSubmissionsRequired": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
                 },
                 "ObjectAvoidanceConfig": {
                     "shape": "ObjectAvoidanceConfig"
                 },
                 "ParticipantCount": {
-                    "shape": "NonNegativeInteger"
+                    "shape": "integer"
                 },
                 "ParticipationConfig": {
                     "shape": "ParticipationConfig"
                 },
                 "PlayoffRaceTypeConfig": {
                     "shape": "PlayoffRaceTypeConfig"
                 },
@@ -2803,51 +2732,54 @@
                 "RacingDivision": {
                     "shape": "Division"
                 },
                 "RacingDivisionEnabled": {
                     "shape": "boolean"
                 },
                 "ResettingBehaviorConfig": {
-                    "shape": "ResettingBehaviorConfig"
+                    "shape": "ResettingBehaviourConfig"
                 },
                 "StartTime": {
                     "shape": "epochTimeMillis"
                 },
                 "Status": {
                     "shape": "LeaderboardStatus"
                 },
+                "SubmissionsPerUser": {
+                    "shape": "integer"
+                },
                 "Tags": {
                     "shape": "StandardLengthString"
                 },
                 "TerminationConditions": {
-                    "shape": "TerminationConditions"
+                    "shape": "EvaluationTerminationConditions"
                 },
                 "TermsAccepted": {
-                    "shape": "Boolean"
+                    "shape": "boolean"
                 },
                 "TermsConditionId": {
                     "shape": "TermsConditionId"
                 },
                 "ThemeConfig": {
                     "shape": "ThemeConfig"
                 },
                 "TimingMethod": {
                     "shape": "TimingMethod"
                 },
                 "TotalLaps": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
                 },
                 "Tournament": {
                     "shape": "Tournament"
                 },
                 "TrackArn": {
                     "shape": "TrackArn"
                 },
-                "TrackImageUrl": {
-                    "shape": "StandardLengthString"
+                "TrackFeatures": {
+                    "shape": "TrackFeatures"
                 },
                 "Visibility": {
                     "shape": "StandardLengthString"
                 },
                 "WinnerAlias": {
                     "shape": "Alias"
                 },
@@ -2859,36 +2791,78 @@
                 "Arn",
                 "Name",
                 "Description",
                 "LaunchTime",
                 "CloseTime",
                 "Status",
                 "MinimumLaps",
-                "ParticipantCount",
-                "ImageUrl",
-                "TrackImageUrl"
+                "ParticipantCount"
             ],
             "type": "structure"
         },
+        "LeaderboardAccessRole": {
+            "type": "string"
+        },
+        "LeaderboardAccessRoles": {
+            "member": {
+                "shape": "LeaderboardAccessRole"
+            },
+            "type": "list"
+        },
         "LeaderboardArn": {
             "max": 1600,
             "min": 1,
             "pattern": "arn:.*",
             "type": "string"
         },
-        "LeaderboardImage": {
-            "enum": [
-                "LeaderboardImage1",
-                "LeaderboardImage2",
-                "LeaderboardImage3",
-                "LeaderboardImage4",
-                "LeaderboardImage5",
-                "LeaderboardImage6"
+        "LeaderboardDefinition": {
+            "members": {
+                "CloseTime": {
+                    "shape": "long"
+                },
+                "Description": {
+                    "shape": "Description"
+                },
+                "Division": {
+                    "shape": "Division"
+                },
+                "LaunchTime": {
+                    "shape": "long"
+                },
+                "LeagueType": {
+                    "shape": "StandardLengthString"
+                },
+                "Name": {
+                    "shape": "LeaderboardName"
+                },
+                "Tags": {
+                    "shape": "StandardLengthString"
+                },
+                "TermsConditionId": {
+                    "shape": "TermsConditionId"
+                },
+                "TrackArn": {
+                    "shape": "Arn"
+                },
+                "TrackFeatures": {
+                    "shape": "TrackFeatures"
+                },
+                "Visibility": {
+                    "shape": "StandardLengthString"
+                }
+            },
+            "required": [
+                "Name",
+                "Visibility",
+                "LaunchTime",
+                "CloseTime",
+                "TrackArn",
+                "LeagueType"
             ],
-            "type": "string"
+            "type": "structure"
         },
         "LeaderboardList": {
             "member": {
                 "shape": "Leaderboard"
             },
             "type": "list"
         },
@@ -2911,84 +2885,89 @@
                 "ActivityArn": {
                     "shape": "Arn"
                 },
                 "Alias": {
                     "shape": "Alias"
                 },
                 "AvgLapTime": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
                 },
                 "AvgResets": {
                     "shape": "double"
                 },
                 "BestLapTime": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
+                },
+                "ClearedJob": {
+                    "shape": "boolean"
                 },
                 "CollisionCount": {
-                    "shape": "NonNegativeInteger"
+                    "shape": "integer"
                 },
-                "JobName": {
-                    "shape": "Name"
+                "CountryCode": {
+                    "shape": "CountryCode"
+                },
+                "EventResourcesConfigs": {
+                    "shape": "EventResourcesConfigs"
                 },
                 "LapCount": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
                 },
                 "LeaderboardSubmissionStatusType": {
                     "shape": "LeaderboardSubmissionStatusType"
                 },
+                "LeagueRanks": {
+                    "shape": "LeagueRanks"
+                },
                 "LogDownloadComplete": {
-                    "shape": "Boolean"
+                    "shape": "boolean"
                 },
                 "ModelArn": {
                     "shape": "ModelArn"
                 },
-                "ModelCreatedInDataAccount": {
-                    "shape": "Boolean"
+                "ModelName": {
+                    "shape": "StandardLengthString"
                 },
                 "OffTrackCount": {
-                    "shape": "NonNegativeInteger"
+                    "shape": "integer"
                 },
                 "RacingDivision": {
                     "shape": "StandardLengthString"
                 },
                 "Rank": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
                 },
                 "RankingScore": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
                 },
                 "ResetCount": {
-                    "shape": "NonNegativeInteger"
+                    "shape": "integer"
                 },
                 "SubmissionCount": {
-                    "shape": "NonNegativeInteger"
+                    "shape": "integer"
                 },
                 "SubmissionTime": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
                 },
                 "SubmissionVideoS3path": {
                     "shape": "Url"
                 },
                 "TeamName": {
                     "shape": "StandardLengthString"
                 },
                 "TotalLapTime": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
+                },
+                "UserAvatarConfig": {
+                    "shape": "AvatarConfig"
                 },
                 "UserId": {
                     "shape": "StandardLengthString"
                 }
             },
-            "required": [
-                "Alias",
-                "SubmissionTime",
-                "LapCount",
-                "AvgLapTime",
-                "LeaderboardSubmissionStatusType"
-            ],
             "type": "structure"
         },
         "LeaderboardSubmissionList": {
             "member": {
                 "shape": "LeaderboardSubmission"
             },
             "type": "list"
@@ -2999,18 +2978,71 @@
                 "QUEUED",
                 "RUNNING",
                 "FAILED",
                 "ERROR"
             ],
             "type": "string"
         },
+        "LeagueRanks": {
+            "members": {
+                "Country": {
+                    "shape": "integer"
+                },
+                "Global": {
+                    "shape": "integer"
+                },
+                "Region": {
+                    "shape": "integer"
+                }
+            },
+            "type": "structure"
+        },
+        "LeagueTopRacers": {
+            "members": {
+                "Country": {
+                    "shape": "RacerSubmission"
+                },
+                "Global": {
+                    "shape": "RacerSubmission"
+                },
+                "Region": {
+                    "shape": "RacerSubmission"
+                }
+            },
+            "type": "structure"
+        },
+        "ListBYOAJobsRequest": {
+            "members": {
+                "MaxResults": {
+                    "shape": "integer"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                },
+                "StatusEquals": {
+                    "shape": "ActivityJobStatus"
+                }
+            },
+            "type": "structure"
+        },
+        "ListBYOAJobsResponse": {
+            "members": {
+                "BYOAJobs": {
+                    "shape": "BYOAJobs"
+                },
+                "NextToken": {
+                    "shape": "NextToken"
+                }
+            },
+            "type": "structure"
+        },
         "ListEvaluationsRequest": {
             "members": {
                 "MaxResults": {
-                    "shape": "MaxResults"
+                    "shape": "integer"
                 },
                 "ModelArn": {
                     "shape": "ModelArn"
                 },
                 "NextToken": {
                     "shape": "NextToken"
                 },
@@ -3038,19 +3070,22 @@
                     "shape": "NextToken"
                 }
             },
             "type": "structure"
         },
         "ListLeaderboardSubmissionsRequest": {
             "members": {
+                "GetTopRacer": {
+                    "shape": "boolean"
+                },
                 "LeaderboardArn": {
                     "shape": "LeaderboardArn"
                 },
                 "MaxResults": {
-                    "shape": "MaxResults"
+                    "shape": "integer"
                 },
                 "NextToken": {
                     "shape": "NextToken"
                 }
             },
             "required": [
                 "LeaderboardArn"
@@ -3058,24 +3093,27 @@
             "type": "structure"
         },
         "ListLeaderboardSubmissionsResponse": {
             "members": {
                 "LeaderboardSubmissions": {
                     "shape": "LeaderboardSubmissionList"
                 },
+                "LeagueTopRacers": {
+                    "shape": "LeagueTopRacers"
+                },
                 "NextToken": {
                     "shape": "NextToken"
                 }
             },
             "type": "structure"
         },
         "ListLeaderboardWinnersRequest": {
             "members": {
                 "MaxResults": {
-                    "shape": "MaxResults"
+                    "shape": "integer"
                 },
                 "NextToken": {
                     "shape": "NextToken"
                 },
                 "WinnerCutoffTime": {
                     "shape": "epochTimeMillis"
                 }
@@ -3090,23 +3128,29 @@
                 "NextToken": {
                     "shape": "NextToken"
                 },
                 "WinnerList": {
                     "shape": "WinnerList"
                 }
             },
-            "required": [
-                "WinnerList"
-            ],
             "type": "structure"
         },
         "ListLeaderboardsRequest": {
             "members": {
+                "CutoffTime": {
+                    "shape": "long"
+                },
+                "LeaderboardAccessRoles": {
+                    "shape": "LeaderboardAccessRoles"
+                },
+                "LeagueType": {
+                    "shape": "StandardLengthString"
+                },
                 "MaxResults": {
-                    "shape": "MaxResults"
+                    "shape": "integer"
                 },
                 "NextToken": {
                     "shape": "NextToken"
                 }
             },
             "type": "structure"
         },
@@ -3123,15 +3167,15 @@
                 "Leaderboards"
             ],
             "type": "structure"
         },
         "ListModelsRequest": {
             "members": {
                 "MaxResults": {
-                    "shape": "MaxResults"
+                    "shape": "integer"
                 },
                 "ModelType": {
                     "shape": "ModelType"
                 },
                 "NextToken": {
                     "shape": "NextToken"
                 },
@@ -3156,19 +3200,25 @@
                     "shape": "NextToken"
                 }
             },
             "type": "structure"
         },
         "ListPrivateLeaderboardParticipantsRequest": {
             "members": {
+                "IncludeExtendedUserData": {
+                    "shape": "boolean"
+                },
+                "LeaderboardAccessRoles": {
+                    "shape": "LeaderboardAccessRoles"
+                },
                 "LeaderboardArn": {
                     "shape": "LeaderboardArn"
                 },
                 "MaxResults": {
-                    "shape": "MaxResults"
+                    "shape": "integer"
                 },
                 "NextToken": {
                     "shape": "NextToken"
                 }
             },
             "required": [
                 "LeaderboardArn"
@@ -3185,75 +3235,44 @@
                 }
             },
             "required": [
                 "PrivateLeaderboardParticipants"
             ],
             "type": "structure"
         },
-        "ListPrivateLeaderboardsRequest": {
-            "members": {
-                "MaxResults": {
-                    "shape": "MaxResults"
-                },
-                "NextToken": {
-                    "shape": "NextToken"
-                }
-            },
-            "type": "structure"
-        },
-        "ListPrivateLeaderboardsResponse": {
-            "members": {
-                "NextToken": {
-                    "shape": "NextToken"
-                },
-                "PrivateLeaderboards": {
-                    "shape": "PrivateLeaderboardList"
-                }
-            },
-            "required": [
-                "PrivateLeaderboards"
-            ],
-            "type": "structure"
-        },
         "ListSortOrder": {
             "enum": [
                 "ASCENDING",
                 "DESCENDING"
             ],
             "type": "string"
         },
-        "ListSubscribedPrivateLeaderboardsRequest": {
+        "ListTagsForResourceRequest": {
             "members": {
-                "MaxResults": {
-                    "shape": "MaxResults"
-                },
-                "NextToken": {
-                    "shape": "NextToken"
+                "ResourceArn": {
+                    "shape": "Arn"
                 }
             },
+            "required": [
+                "ResourceArn"
+            ],
             "type": "structure"
         },
-        "ListSubscribedPrivateLeaderboardsResponse": {
+        "ListTagsForResourceResponse": {
             "members": {
-                "NextToken": {
-                    "shape": "NextToken"
-                },
-                "PrivateLeaderboards": {
-                    "shape": "PrivateLeaderboardList"
+                "Tags": {
+                    "shape": "Tags"
                 }
             },
-            "required": [
-                "PrivateLeaderboards"
-            ],
             "type": "structure"
         },
         "ListTracksRequest": {
             "members": {
                 "MaxResults": {
-                    "shape": "MaxResults"
+                    "shape": "integer"
                 },
                 "NextToken": {
                     "shape": "NextToken"
                 }
             },
             "type": "structure"
         },
@@ -3267,15 +3286,15 @@
                 }
             },
             "type": "structure"
         },
         "ListTrainingJobsRequest": {
             "members": {
                 "MaxResults": {
-                    "shape": "MaxResults"
+                    "shape": "integer"
                 },
                 "ModelArn": {
                     "shape": "ModelArn"
                 },
                 "NextToken": {
                     "shape": "NextToken"
                 }
@@ -3292,77 +3311,64 @@
                 },
                 "TrainingJobs": {
                     "shape": "TrainingJobList"
                 }
             },
             "type": "structure"
         },
-        "MaxResults": {
-            "max": 100,
-            "min": 1,
-            "type": "integer"
-        },
-        "MaximumSpeed": {
-            "max": 12.0,
-            "min": 0.1,
-            "type": "double"
-        },
-        "MaximumSteeringAngle": {
-            "max": 30.0,
-            "min": 1.0,
-            "type": "double"
+        "Live": {
+            "members": {
+                "RaceArn": {
+                    "shape": "Arn"
+                }
+            },
+            "required": [
+                "RaceArn"
+            ],
+            "type": "structure"
         },
         "Message": {
             "max": 2000,
             "min": 1,
             "type": "string"
         },
         "MetaData": {
             "max": 100000,
             "min": 1,
             "type": "string"
         },
-        "MigrateModelsRequest": {
-            "members": {
-                "ModelArnList": {
-                    "shape": "ModelArnList"
-                },
-                "RoleArn": {
-                    "shape": "RoleArn"
-                }
-            },
-            "type": "structure"
-        },
-        "MigrateModelsResponse": {
-            "members": {},
-            "type": "structure"
-        },
         "Model": {
             "members": {
                 "AgentAlgorithm": {
                     "shape": "AgentAlgorithm"
                 },
                 "AgentNetwork": {
                     "shape": "AgentNetwork"
                 },
                 "CarArn": {
                     "shape": "CarArn"
                 },
                 "CarConfiguration": {
                     "shape": "CarConfiguration"
                 },
+                "CreatedByAlias": {
+                    "shape": "Alias"
+                },
                 "CreatedInDataAccount": {
                     "shape": "boolean"
                 },
                 "CreationTime": {
                     "shape": "epochTimeMillis"
                 },
                 "Error": {
                     "shape": "ModelError"
                 },
+                "ImportModelS3SrcLocation": {
+                    "shape": "StandardLengthString"
+                },
                 "ModelArn": {
                     "shape": "ModelArn"
                 },
                 "ModelArtifactS3Location": {
                     "shape": "S3Bucket"
                 },
                 "ModelDescription": {
@@ -3371,15 +3377,18 @@
                 "ModelFramework": {
                     "shape": "ModelFramework"
                 },
                 "ModelName": {
                     "shape": "ModelName"
                 },
                 "ModelPackagingComplete": {
-                    "shape": "Boolean"
+                    "shape": "boolean"
+                },
+                "ModelSizeInGb": {
+                    "shape": "double"
                 },
                 "ModelType": {
                     "shape": "ModelType"
                 },
                 "Status": {
                     "shape": "ModelStatus"
                 },
@@ -3462,14 +3471,133 @@
         },
         "ModelType": {
             "enum": [
                 "REINFORCEMENT_LEARNING"
             ],
             "type": "string"
         },
+        "ModerateConfig": {
+            "members": {
+                "EntryMode": {
+                    "shape": "StandardLengthString"
+                },
+                "RacersSubmissions": {
+                    "shape": "ModerateConfigRacersSubmissions"
+                }
+            },
+            "required": [
+                "RacersSubmissions"
+            ],
+            "type": "structure"
+        },
+        "ModerateConfigRacersSubmission": {
+            "members": {
+                "Alias": {
+                    "shape": "Alias"
+                },
+                "ClearedJob": {
+                    "shape": "boolean"
+                },
+                "EvaluationCompletedTime": {
+                    "shape": "long"
+                },
+                "EvaluationStartTime": {
+                    "shape": "long"
+                },
+                "ModelArn": {
+                    "shape": "Arn"
+                },
+                "SubmissionStatus": {
+                    "shape": "StandardLengthString"
+                },
+                "SubmissionTime": {
+                    "shape": "long"
+                },
+                "UserId": {
+                    "shape": "StandardLengthString"
+                },
+                "UserIndex": {
+                    "shape": "long"
+                }
+            },
+            "required": [
+                "UserId",
+                "Alias",
+                "SubmissionStatus"
+            ],
+            "type": "structure"
+        },
+        "ModerateConfigRacersSubmissions": {
+            "member": {
+                "shape": "ModerateConfigRacersSubmission"
+            },
+            "type": "list"
+        },
+        "Mouth": {
+            "enum": [
+                "Concerned",
+                "Default",
+                "Disbelief",
+                "Eating",
+                "Grimace",
+                "Sad",
+                "ScreamOpen",
+                "Serious",
+                "Smile",
+                "Tongue",
+                "Twinkle"
+            ],
+            "type": "string"
+        },
+        "MultiUserProfile": {
+            "members": {
+                "AssociatedOn": {
+                    "shape": "long"
+                },
+                "ComputeMinutesQueued": {
+                    "shape": "integer"
+                },
+                "ComputeMinutesUsed": {
+                    "shape": "integer"
+                },
+                "MaxModels": {
+                    "shape": "integer"
+                },
+                "MaxTotalComputeMinutes": {
+                    "shape": "integer"
+                },
+                "StorageBytesUsed": {
+                    "shape": "long"
+                },
+                "UserState": {
+                    "shape": "UserState"
+                }
+            },
+            "required": [
+                "AssociatedOn",
+                "ComputeMinutesUsed",
+                "ComputeMinutesQueued",
+                "MaxTotalComputeMinutes",
+                "MaxModels",
+                "StorageBytesUsed",
+                "UserState"
+            ],
+            "type": "structure"
+        },
+        "MultiracerConfig": {
+            "members": {
+                "MultiracerModeEnabled": {
+                    "shape": "boolean"
+                }
+            },
+            "required": [
+                "MultiracerModeEnabled"
+            ],
+            "type": "structure"
+        },
         "Name": {
             "max": 255,
             "min": 1,
             "pattern": "^[a-zA-Z0-9\\-]+$",
             "type": "string"
         },
         "NeuralNetwork": {
@@ -3489,52 +3617,36 @@
             "min": 0,
             "type": "double"
         },
         "NonNegativeInteger": {
             "min": 0,
             "type": "integer"
         },
-        "NumBotCars": {
-            "max": 6,
-            "min": 1,
-            "type": "integer"
-        },
-        "NumObstacles": {
-            "max": 10,
-            "min": 1,
-            "type": "integer"
-        },
         "ObjectAvoidanceConfig": {
             "members": {
                 "NumObstacles": {
-                    "shape": "NumObstacles"
+                    "shape": "integer"
                 },
                 "ObstaclePositions": {
-                    "shape": "ObstablePositionList"
+                    "shape": "ObstaclePositionList"
                 },
                 "ObstacleType": {
                     "shape": "ObstacleType"
                 },
                 "RandomizeLocation": {
                     "shape": "boolean"
                 }
             },
             "required": [
-                "RandomizeLocation",
                 "NumObstacles",
-                "ObstacleType"
+                "ObstacleType",
+                "RandomizeLocation"
             ],
             "type": "structure"
         },
-        "ObstablePositionList": {
-            "member": {
-                "shape": "ObstaclePosition"
-            },
-            "type": "list"
-        },
         "ObstaclePosition": {
             "members": {
                 "LaneNumber": {
                     "shape": "NonNegativeInteger"
                 },
                 "TrackPercentage": {
                     "shape": "NonNegativeDouble"
@@ -3542,14 +3654,20 @@
             },
             "required": [
                 "LaneNumber",
                 "TrackPercentage"
             ],
             "type": "structure"
         },
+        "ObstaclePositionList": {
+            "member": {
+                "shape": "ObstaclePosition"
+            },
+            "type": "list"
+        },
         "ObstacleType": {
             "enum": [
                 "BOX"
             ],
             "type": "string"
         },
         "ParticipationConfig": {
@@ -3563,150 +3681,125 @@
             },
             "required": [
                 "EntryTypeConfig",
                 "ViewType"
             ],
             "type": "structure"
         },
+        "PerformLeaderboardOperationRequest": {
+            "members": {
+                "EntryMode": {
+                    "shape": "EntryMode"
+                },
+                "GetConflictingEventSchedulesRequest": {
+                    "shape": "GetConflictingEventSchedulesRequest"
+                },
+                "LeaderboardArn": {
+                    "shape": "Arn"
+                },
+                "NumberOfBackupResources": {
+                    "shape": "integer"
+                },
+                "Operation": {
+                    "shape": "StandardLengthString"
+                },
+                "ReLaunch": {
+                    "shape": "boolean"
+                },
+                "ResourceIds": {
+                    "shape": "ResourceIds"
+                },
+                "UserIds": {
+                    "shape": "UserIds"
+                }
+            },
+            "required": [
+                "Operation"
+            ],
+            "type": "structure"
+        },
+        "PerformLeaderboardOperationResponse": {
+            "members": {
+                "GetConflictingEventSchedulesResponse": {
+                    "shape": "GetConflictingEventSchedulesResponse"
+                }
+            },
+            "type": "structure"
+        },
         "PerspectiveCustomization": {
             "members": {
                 "Decal": {
                     "shape": "CarDecal"
                 }
             },
             "type": "structure"
         },
+        "PlayoffFeature": {
+            "members": {
+                "GrandPrix": {
+                    "shape": "GrandPrix"
+                },
+                "LaunchTime": {
+                    "shape": "long"
+                },
+                "Live": {
+                    "shape": "Live"
+                },
+                "PlayoffType": {
+                    "shape": "StandardLengthString"
+                },
+                "Tournament": {
+                    "shape": "Tournament"
+                }
+            },
+            "required": [
+                "PlayoffType"
+            ],
+            "type": "structure"
+        },
         "PlayoffRaceTypeConfig": {
             "members": {
                 "PlayoffRaceArn": {
-                    "shape": "LeaderboardArn"
+                    "shape": "Arn"
                 },
                 "PlayoffRaceTypeID": {
-                    "shape": "PlayoffRaceTypeID"
+                    "shape": "StandardLengthString"
                 },
                 "PlayoffReleaseTime": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
                 },
                 "PlayoffResultReleaseTime": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
                 }
             },
             "type": "structure"
         },
-        "PlayoffRaceTypeID": {
-            "enum": [
-                "TOURNAMENT",
-                "GRANDPRIX"
-            ],
-            "type": "string"
-        },
         "PositiveInteger": {
             "min": 1,
             "type": "integer"
         },
-        "PrivateLeaderboard": {
-            "members": {
-                "AccessToken": {
-                    "shape": "AccessToken"
-                },
-                "Alias": {
-                    "shape": "Alias"
-                },
-                "Arn": {
-                    "shape": "LeaderboardArn"
-                },
-                "Description": {
-                    "shape": "Description"
-                },
-                "Division": {
-                    "shape": "Division"
-                },
-                "EndTime": {
-                    "shape": "epochTimeMillis"
-                },
-                "HeadToHeadConfig": {
-                    "shape": "HeadToHeadConfig"
-                },
-                "LeaderboardImage": {
-                    "shape": "LeaderboardImage"
-                },
-                "MinimumLaps": {
-                    "shape": "PositiveInteger"
-                },
-                "Name": {
-                    "shape": "LeaderboardName"
-                },
-                "ObjectAvoidanceConfig": {
-                    "shape": "ObjectAvoidanceConfig"
-                },
-                "ParticipantCount": {
-                    "shape": "NonNegativeInteger"
-                },
-                "PlayoffRaceTypeConfig": {
-                    "shape": "PlayoffRaceTypeConfig"
-                },
-                "RaceType": {
-                    "shape": "RaceType"
-                },
-                "ResettingBehaviorConfig": {
-                    "shape": "ResettingBehaviorConfig"
-                },
-                "StartTime": {
-                    "shape": "epochTimeMillis"
-                },
-                "Status": {
-                    "shape": "LeaderboardStatus"
-                },
-                "ThemeConfig": {
-                    "shape": "ThemeConfig"
-                },
-                "TimingMethod": {
-                    "shape": "TimingMethod"
-                },
-                "TotalLaps": {
-                    "shape": "PositiveInteger"
-                },
-                "TrackArn": {
-                    "shape": "TrackArn"
-                },
-                "TrackImageUrl": {
-                    "shape": "StandardLengthString"
-                }
-            },
-            "required": [
-                "Arn",
-                "Name",
-                "Description",
-                "StartTime",
-                "EndTime",
-                "TrackArn",
-                "MinimumLaps",
-                "TotalLaps",
-                "ParticipantCount",
-                "LeaderboardImage",
-                "Status"
-            ],
-            "type": "structure"
-        },
-        "PrivateLeaderboardList": {
-            "member": {
-                "shape": "PrivateLeaderboard"
-            },
-            "type": "list"
+        "PreprocessType": {
+            "type": "string"
         },
         "PrivateLeaderboardParticipant": {
             "members": {
                 "AccountId": {
                     "shape": "AccountId"
                 },
                 "Alias": {
                     "shape": "Alias"
                 },
                 "JoinTime": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
+                },
+                "UserAvatarConfig": {
+                    "shape": "AvatarConfig"
+                },
+                "UserId": {
+                    "shape": "StandardLengthString"
                 }
             },
             "type": "structure"
         },
         "PrivateLeaderboardParticipantList": {
             "member": {
                 "shape": "PrivateLeaderboardParticipant"
@@ -3732,152 +3825,334 @@
                 },
                 "Winner": {
                     "shape": "Alias"
                 }
             },
             "type": "structure"
         },
+        "RaceConfig": {
+            "members": {
+                "CarControlConfig": {
+                    "shape": "CarControlConfig"
+                },
+                "MinimumLaps": {
+                    "shape": "integer"
+                },
+                "Moderated": {
+                    "shape": "boolean"
+                },
+                "ParticipationConfig": {
+                    "shape": "ParticipationConfig"
+                },
+                "RaceTypeConfig": {
+                    "shape": "RaceTypeConfig"
+                },
+                "ResettingBehavior": {
+                    "shape": "ResettingBehaviourConfig"
+                },
+                "SubmissionsPerUser": {
+                    "shape": "integer"
+                },
+                "TerminationConditions": {
+                    "shape": "EvaluationTerminationConditions"
+                },
+                "TimingMethod": {
+                    "shape": "TimingMethod"
+                }
+            },
+            "required": [
+                "MinimumLaps",
+                "RaceTypeConfig",
+                "ResettingBehavior",
+                "TerminationConditions",
+                "TimingMethod"
+            ],
+            "type": "structure"
+        },
         "RaceList": {
             "member": {
                 "shape": "Race"
             },
             "type": "list"
         },
         "RaceType": {
             "enum": [
                 "TIME_TRIAL",
                 "OBJECT_AVOIDANCE",
                 "HEAD_TO_HEAD_RACING"
             ],
             "type": "string"
         },
+        "RaceTypeConfig": {
+            "members": {
+                "HeadToHead": {
+                    "shape": "HeadToHeadConfig"
+                },
+                "ObjectAvoidance": {
+                    "shape": "ObjectAvoidanceConfig"
+                },
+                "RaceType": {
+                    "shape": "RaceType"
+                },
+                "TimeTrial": {
+                    "shape": "TimeTrial"
+                }
+            },
+            "required": [
+                "RaceType"
+            ],
+            "type": "structure"
+        },
         "RacerStatistics": {
             "members": {
                 "Alias": {
                     "shape": "Alias"
                 },
                 "CrashCount": {
-                    "shape": "NonNegativeInteger"
+                    "shape": "integer"
                 },
                 "OffTrackCount": {
-                    "shape": "NonNegativeInteger"
+                    "shape": "integer"
                 },
                 "SeedNumber": {
-                    "shape": "NonNegativeInteger"
+                    "shape": "integer"
                 },
                 "TimeTakenMillis": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
                 },
                 "VideoUrl": {
                     "shape": "Url"
                 }
             },
             "type": "structure"
         },
+        "RacerSubmission": {
+            "members": {
+                "TopRacer": {
+                    "shape": "LeaderboardSubmission"
+                },
+                "TotalParticipants": {
+                    "shape": "integer"
+                }
+            },
+            "type": "structure"
+        },
+        "RacingDivisionConfig": {
+            "members": {
+                "EndTime": {
+                    "shape": "long"
+                },
+                "RacingDivision": {
+                    "shape": "Division"
+                },
+                "StartTime": {
+                    "shape": "long"
+                }
+            },
+            "type": "structure"
+        },
+        "RacingDivisionsByRaceType": {
+            "members": {
+                "H2hRacingDivision": {
+                    "shape": "Division"
+                },
+                "ObjectAvoidanceRacingDivision": {
+                    "shape": "Division"
+                },
+                "TimeTrialRacingDivision": {
+                    "shape": "Division"
+                }
+            },
+            "type": "structure"
+        },
+        "Ranking": {
+            "members": {
+                "ItemName": {
+                    "shape": "StandardLengthString"
+                },
+                "MediaLink": {
+                    "shape": "StandardLengthString"
+                },
+                "RankingValue": {
+                    "shape": "long"
+                },
+                "UserAvatarConfig": {
+                    "shape": "AvatarConfig"
+                }
+            },
+            "type": "structure"
+        },
+        "RankingList": {
+            "member": {
+                "shape": "Ranking"
+            },
+            "type": "list"
+        },
         "RemoveLeaderboardAccessPermissionRequest": {
             "members": {
                 "AccountId": {
                     "shape": "AccountId"
                 },
                 "LeaderboardArn": {
                     "shape": "LeaderboardArn"
+                },
+                "UserId": {
+                    "shape": "StandardLengthString"
                 }
             },
             "required": [
-                "LeaderboardArn",
-                "AccountId"
+                "LeaderboardArn"
             ],
             "type": "structure"
         },
         "RemoveLeaderboardAccessPermissionResponse": {
             "members": {},
             "type": "structure"
         },
-        "ResettingBehaviorConfig": {
+        "ResettingBehaviourConfig": {
             "members": {
                 "AllowReset": {
                     "shape": "boolean"
                 },
                 "CollisionPenaltySeconds": {
-                    "shape": "NonNegativeDouble"
+                    "shape": "double"
                 },
                 "CutOffSeconds": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
                 },
                 "IsContinuousLap": {
                     "shape": "boolean"
                 },
                 "MaxResetTimes": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
                 },
                 "OffTrackPenaltySeconds": {
-                    "shape": "NonNegativeDouble"
+                    "shape": "double"
                 },
                 "PenaltySeconds": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
                 }
             },
             "type": "structure"
         },
-        "ResourceAlreadyExistsException": {
-            "exception": true,
-            "members": {},
+        "ResourceConfig": {
+            "members": {
+                "ResourceCreationTime": {
+                    "shape": "long"
+                },
+                "ResourceFailoverTime": {
+                    "shape": "long"
+                },
+                "ResourceId": {
+                    "shape": "StandardLengthString"
+                },
+                "ResourceStatus": {
+                    "shape": "StandardLengthString"
+                }
+            },
+            "required": [
+                "ResourceId",
+                "ResourceStatus"
+            ],
             "type": "structure"
         },
-        "ResourceDoesNotExistException": {
-            "exception": true,
-            "members": {},
-            "type": "structure"
+        "ResourceIds": {
+            "member": {
+                "shape": "StandardLengthString"
+            },
+            "type": "list"
         },
-        "ResourceInUseException": {
-            "exception": true,
-            "members": {},
+        "ResourceUrl": {
+            "members": {
+                "Endpoint": {
+                    "shape": "StandardLengthString"
+                },
+                "Expiry": {
+                    "shape": "integer"
+                },
+                "Protocol": {
+                    "shape": "StandardLengthString"
+                }
+            },
             "type": "structure"
         },
-        "ResourceLimitExceededException": {
-            "exception": true,
-            "members": {},
-            "type": "structure"
+        "ResourceUrls": {
+            "member": {
+                "shape": "ResourceUrl"
+            },
+            "type": "list"
         },
         "ResultsReleaseTimes": {
             "member": {
                 "shape": "epochTimeMillis"
             },
             "type": "list"
         },
-        "RewardFunctionCode": {
-            "max": 140000,
-            "min": 1,
-            "pattern": "[\\s\\S]+",
-            "type": "string"
-        },
-        "RoboMakerSimulationApplication": {
+        "Reward": {
             "members": {
-                "Name": {
+                "AwardedTime": {
+                    "shape": "long"
+                },
+                "Context": {
+                    "shape": "RewardContext"
+                },
+                "RewardDescription": {
+                    "shape": "StandardLengthString"
+                },
+                "RewardId": {
+                    "shape": "StandardLengthString"
+                },
+                "RewardName": {
                     "shape": "StandardLengthString"
                 },
-                "Version": {
+                "Type": {
                     "shape": "StandardLengthString"
                 }
             },
-            "required": [
-                "Name"
-            ],
             "type": "structure"
         },
+        "RewardContext": {
+            "members": {
+                "CountryCode": {
+                    "shape": "CountryCode"
+                },
+                "Leaderboard": {
+                    "shape": "Leaderboard"
+                }
+            },
+            "type": "structure"
+        },
+        "RewardFunctionCode": {
+            "max": 140000,
+            "min": 1,
+            "pattern": "[\\s\\S]+",
+            "type": "string"
+        },
+        "Rewards": {
+            "member": {
+                "shape": "Reward"
+            },
+            "type": "list"
+        },
         "RoleArn": {
             "max": 1600,
             "min": 1,
             "pattern": "arn:aws(-iso)?:iam::[0-9]{12}:role/(service-role/)?[a-zA-Z0-9_\\+=,\\.\\-@]{1,64}",
             "type": "string"
         },
         "RunTournamentRequest": {
             "members": {
                 "LeaderboardArn": {
                     "shape": "LeaderboardArn"
+                },
+                "TournamentConfig": {
+                    "shape": "TournamentConfig"
+                },
+                "TournamentRacersOverride": {
+                    "shape": "TournamentRacersOverride"
                 }
             },
             "required": [
                 "LeaderboardArn"
             ],
             "type": "structure"
         },
@@ -3905,33 +4180,50 @@
         },
         "SensorsList": {
             "member": {
                 "shape": "SensorType"
             },
             "type": "list"
         },
-        "ServiceException": {
-            "exception": true,
-            "members": {},
-            "type": "structure"
-        },
         "SetAliasRequest": {
             "members": {
-                "AccountId": {
-                    "shape": "AccountId"
-                },
                 "Alias": {
                     "shape": "Alias"
+                },
+                "AlternativeEmail": {
+                    "shape": "StandardLengthString"
+                },
+                "CompetitionCountryCode": {
+                    "shape": "StandardLengthString"
+                },
+                "FirstName": {
+                    "shape": "StandardLengthString"
+                },
+                "LastName": {
+                    "shape": "StandardLengthString"
+                },
+                "MiddleName": {
+                    "shape": "StandardLengthString"
+                },
+                "UserAvatarConfig": {
+                    "shape": "AvatarConfig"
                 }
             },
-            "required": [
-                "Alias"
-            ],
             "type": "structure"
         },
+        "SkinColor": {
+            "enum": [
+                "Pale",
+                "Light",
+                "Brown",
+                "DarkBrown",
+                "Black"
+            ],
+            "type": "string"
+        },
         "SortEvaluationsBy": {
             "enum": [
                 "CREATION_TIME"
             ],
             "type": "string"
         },
         "SortModelsBy": {
@@ -3941,30 +4233,70 @@
             "type": "string"
         },
         "SpeedGranularity": {
             "max": 3,
             "min": 1,
             "type": "integer"
         },
+        "SpeedRange": {
+            "members": {
+                "High": {
+                    "shape": "double"
+                },
+                "Low": {
+                    "shape": "double"
+                }
+            },
+            "required": [
+                "Low",
+                "High"
+            ],
+            "type": "structure"
+        },
         "StandardLengthString": {
             "max": 255,
             "min": 1,
             "pattern": "^.+$",
             "type": "string"
         },
+        "StartBYOAJobRequest": {
+            "members": {
+                "Name": {
+                    "shape": "StandardLengthString"
+                },
+                "TerminationConditions": {
+                    "shape": "TerminationConditions"
+                }
+            },
+            "required": [
+                "TerminationConditions"
+            ],
+            "type": "structure"
+        },
+        "StartBYOAJobResponse": {
+            "members": {
+                "BYOAJobArn": {
+                    "shape": "Arn"
+                }
+            },
+            "required": [
+                "BYOAJobArn"
+            ],
+            "type": "structure"
+        },
         "StartEvaluationRequest": {
             "members": {
                 "EvaluationConfig": {
                     "shape": "EvaluationConfig"
                 },
                 "ModelArn": {
                     "shape": "ModelArn"
                 },
                 "RoleArn": {
-                    "shape": "RoleArn"
+                    "shape": "Arn"
                 }
             },
             "required": [
                 "ModelArn",
                 "EvaluationConfig"
             ],
             "type": "structure"
@@ -3976,19 +4308,49 @@
                 }
             },
             "required": [
                 "EvaluationJobArn"
             ],
             "type": "structure"
         },
+        "SteeringAngleRange": {
+            "members": {
+                "High": {
+                    "shape": "double"
+                },
+                "Low": {
+                    "shape": "double"
+                }
+            },
+            "required": [
+                "Low",
+                "High"
+            ],
+            "type": "structure"
+        },
         "SteeringGranularity": {
             "max": 7,
             "min": 1,
             "type": "integer"
         },
+        "StopBYOAJobRequest": {
+            "members": {
+                "BYOAJobArn": {
+                    "shape": "Arn"
+                }
+            },
+            "required": [
+                "BYOAJobArn"
+            ],
+            "type": "structure"
+        },
+        "StopBYOAJobResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "StopEvaluationRequest": {
             "members": {
                 "EvaluationJobArn": {
                     "shape": "EvaluationJobArn"
                 }
             },
             "required": [
@@ -4011,24 +4373,105 @@
             ],
             "type": "structure"
         },
         "StopTrainingReinforcementLearningModelResponse": {
             "members": {},
             "type": "structure"
         },
-        "TerminationConditions": {
+        "SubmissionOverrides": {
             "members": {
-                "MaxEpisodes": {
-                    "shape": "NonNegativeInteger"
+                "AliasOverride": {
+                    "shape": "StandardLengthString"
                 },
-                "MaxTimeInMinutes": {
-                    "shape": "NonNegativeInteger"
+                "CarCustomizationOverride": {
+                    "shape": "CarCustomization"
                 },
-                "RewardScore": {
-                    "shape": "double"
+                "Email": {
+                    "shape": "StandardLengthString"
+                }
+            },
+            "required": [
+                "AliasOverride",
+                "CarCustomizationOverride"
+            ],
+            "type": "structure"
+        },
+        "Tag": {
+            "members": {
+                "Key": {
+                    "shape": "StandardLengthString"
+                },
+                "Value": {
+                    "shape": "StandardLengthString"
+                }
+            },
+            "required": [
+                "Key",
+                "Value"
+            ],
+            "type": "structure"
+        },
+        "TagKeys": {
+            "member": {
+                "shape": "StandardLengthString"
+            },
+            "type": "list"
+        },
+        "TagResourceRequest": {
+            "members": {
+                "ResourceArn": {
+                    "shape": "Arn"
+                },
+                "Tags": {
+                    "shape": "Tags"
+                }
+            },
+            "required": [
+                "ResourceArn",
+                "Tags"
+            ],
+            "type": "structure"
+        },
+        "TagResourceResponse": {
+            "members": {},
+            "type": "structure"
+        },
+        "TagrisSweep": {
+            "members": {
+                "TagrisAccountId": {
+                    "shape": "StandardLengthString"
+                },
+                "TagrisAmazonResourceName": {
+                    "shape": "StandardLengthString"
+                },
+                "TagrisInternalId": {
+                    "shape": "StandardLengthString"
+                },
+                "TagrisVersion": {
+                    "shape": "long"
+                }
+            },
+            "type": "structure"
+        },
+        "TagrisSweepList": {
+            "member": {
+                "shape": "TagrisSweep"
+            },
+            "type": "list"
+        },
+        "Tags": {
+            "member": {
+                "shape": "Tag"
+            },
+            "type": "list"
+        },
+        "TerminationConditions": {
+            "members": {
+                "MaxTimeInMinutes": {
+                    "shape": "integer"
                 }
             },
             "required": [
                 "MaxTimeInMinutes"
             ],
             "type": "structure"
         },
@@ -4074,26 +4517,63 @@
             "type": "structure"
         },
         "ThemeID": {
             "max": 64,
             "min": 1,
             "type": "string"
         },
+        "TimeTrial": {
+            "members": {},
+            "type": "structure"
+        },
         "TimingMethod": {
             "enum": [
                 "BEST_LAP_TIME",
                 "AVG_LAP_TIME",
                 "TOTAL_TIME"
             ],
             "type": "string"
         },
-        "TooManyRequestsException": {
-            "exception": true,
-            "members": {},
-            "type": "structure"
+        "Top": {
+            "enum": [
+                "Helmet",
+                "Hijab",
+                "Turban",
+                "WinterHat1",
+                "WinterHat2",
+                "WinterHat3",
+                "WinterHat4",
+                "LongHairFrida",
+                "LongHairFro",
+                "LongHairFroBand",
+                "NoHair",
+                "ShortHairSides",
+                "LongHairBigHair",
+                "LongHairBob",
+                "LongHairBun",
+                "LongHairCurly",
+                "LongHairCurvy",
+                "LongHairDreads",
+                "LongHairNotTooLong",
+                "LongHairMiaWallace",
+                "LongHairStraight",
+                "LongHairStraight2",
+                "LongHairStraightStrand",
+                "ShortHairDreads01",
+                "ShortHairDreads02",
+                "ShortHairFrizzle",
+                "ShortHairShaggyMullet",
+                "ShortHairShortCurly",
+                "ShortHairShortFlat",
+                "ShortHairShortRound",
+                "ShortHairShortWaved",
+                "ShortHairTheCaesar",
+                "ShortHairTheCaesarSidePart"
+            ],
+            "type": "string"
         },
         "Tournament": {
             "members": {
                 "ResultsReleaseTimes": {
                     "shape": "ResultsReleaseTimes"
                 },
                 "Size": {
@@ -4102,50 +4582,73 @@
             },
             "required": [
                 "Size",
                 "ResultsReleaseTimes"
             ],
             "type": "structure"
         },
+        "TournamentConfig": {
+            "members": {
+                "MaxLaps": {
+                    "shape": "integer"
+                },
+                "ResettingBehavior": {
+                    "shape": "ResettingBehaviourConfig"
+                }
+            },
+            "type": "structure"
+        },
+        "TournamentRacersOverride": {
+            "member": {
+                "shape": "StandardLengthString"
+            },
+            "type": "list"
+        },
         "TournamentResults": {
             "members": {
                 "Races": {
                     "shape": "RaceList"
                 }
             },
             "type": "structure"
         },
+        "TournamentStatus": {
+            "type": "string"
+        },
         "Track": {
             "members": {
+                "AvailableTrackFeatures": {
+                    "shape": "AvailableTrackFeatures"
+                },
+                "EnabledConsoles": {
+                    "shape": "EnabledConsoles"
+                },
                 "TrackArn": {
                     "shape": "TrackArn"
                 },
                 "TrackDescription": {
                     "shape": "Description"
                 },
                 "TrackDifficulty": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
                 },
                 "TrackLength": {
                     "shape": "double"
                 },
                 "TrackName": {
                     "shape": "Name"
                 },
-                "TrackPicture": {
-                    "shape": "StandardLengthString"
-                },
-                "TrackRaceTypePictureMap": {
-                    "shape": "TrackRaceTypePictureMap"
-                },
                 "TrackReleaseTime": {
-                    "shape": "epochTimeMillis"
+                    "shape": "long"
+                },
+                "TrackTags": {
+                    "shape": "Tags"
                 },
                 "TrackUsageCount": {
-                    "shape": "PositiveInteger"
+                    "shape": "integer"
                 },
                 "TrackWidth": {
                     "shape": "double"
                 }
             },
             "type": "structure"
         },
@@ -4162,43 +4665,48 @@
                 }
             },
             "required": [
                 "TrackArn"
             ],
             "type": "structure"
         },
+        "TrackFeatures": {
+            "members": {
+                "Direction": {
+                    "shape": "Direction"
+                }
+            },
+            "required": [
+                "Direction"
+            ],
+            "type": "structure"
+        },
         "TrackList": {
             "member": {
                 "shape": "Track"
             },
             "type": "list"
         },
-        "TrackRaceTypePictureMap": {
+        "TrackRecord": {
             "members": {
-                "HeadToHeadRacing": {
-                    "shape": "StandardLengthString"
-                },
-                "HeadToHeadRacingGray": {
-                    "shape": "StandardLengthString"
-                },
-                "ObjectAvoidance": {
-                    "shape": "StandardLengthString"
+                "Rankings": {
+                    "shape": "RankingList"
                 },
-                "ObjectAvoidanceGray": {
-                    "shape": "StandardLengthString"
-                },
-                "TimeTrial": {
-                    "shape": "StandardLengthString"
-                },
-                "TimeTrialGray": {
+                "RecordItemKey": {
                     "shape": "StandardLengthString"
                 }
             },
             "type": "structure"
         },
+        "TrackRecordList": {
+            "member": {
+                "shape": "TrackRecord"
+            },
+            "type": "list"
+        },
         "TrainingConfig": {
             "members": {
                 "HeadToHeadConfig": {
                     "shape": "HeadToHeadConfig"
                 },
                 "Hyperparameters": {
                     "shape": "map"
@@ -4208,14 +4716,20 @@
                 },
                 "ModelMetadataS3Source": {
                     "shape": "S3Bucket"
                 },
                 "ObjectAvoidanceConfig": {
                     "shape": "ObjectAvoidanceConfig"
                 },
+                "PreprocessParameters": {
+                    "shape": "map"
+                },
+                "PreprocessType": {
+                    "shape": "PreprocessType"
+                },
                 "RaceType": {
                     "shape": "RaceType"
                 },
                 "ResourceConfig": {
                     "shape": "TrainingResourceConfig"
                 },
                 "RewardFunction": {
@@ -4321,84 +4835,139 @@
                 },
                 "RewardScore": {
                     "shape": "double"
                 }
             },
             "type": "structure"
         },
+        "TshirtGraphic": {
+            "enum": [
+                "Diamond",
+                "Hola",
+                "Pizza"
+            ],
+            "type": "string"
+        },
+        "UntagResourceRequest": {
+            "members": {
+                "ResourceArn": {
+                    "shape": "Arn"
+                },
+                "TagKeys": {
+                    "shape": "TagKeys"
+                }
+            },
+            "required": [
+                "ResourceArn",
+                "TagKeys"
+            ],
+            "type": "structure"
+        },
+        "UntagResourceResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "UpdateCarRequest": {
             "members": {
                 "Car": {
                     "shape": "Car"
                 }
             },
+            "required": [
+                "Car"
+            ],
             "type": "structure"
         },
         "UpdateCarResponse": {
             "members": {
                 "Car": {
                     "shape": "Car"
                 }
             },
             "type": "structure"
         },
         "Url": {
             "pattern": "^https:\\/\\/.*",
             "type": "string"
         },
-        "VersioningStatus": {
+        "UserAction": {
             "enum": [
-                "OUTDATED",
-                "LATEST"
+                "ENABLE",
+                "DISABLE",
+                "RESTRICT",
+                "DELETE_RESOURCES",
+                "SET_LIMITS"
             ],
             "type": "string"
         },
-        "VpcStack": {
+        "UserIds": {
+            "member": {
+                "shape": "StandardLengthString"
+            },
+            "type": "list"
+        },
+        "UserLimits": {
             "members": {
-                "Status": {
-                    "shape": "VpcStackStatus"
+                "MaxComputeMinutes": {
+                    "shape": "integer"
+                },
+                "MaxModels": {
+                    "shape": "integer"
                 }
             },
-            "required": [
-                "Status"
-            ],
             "type": "structure"
         },
-        "VpcStackStatus": {
+        "UserState": {
             "enum": [
-                "CREATED",
-                "FAILED"
+                "ACTIVE",
+                "DISABLED",
+                "RESTRICTED"
             ],
             "type": "string"
         },
+        "VerifyResourcesExistForTagrisRequest": {
+            "members": {
+                "TagrisSweepList": {
+                    "shape": "TagrisSweepList"
+                }
+            },
+            "required": [
+                "TagrisSweepList"
+            ],
+            "type": "structure"
+        },
+        "VerifyResourcesExistForTagrisResponse": {
+            "members": {
+                "TagrisSweepListResult": {
+                    "shape": "map"
+                }
+            },
+            "required": [
+                "TagrisSweepListResult"
+            ],
+            "type": "structure"
+        },
         "Winner": {
             "members": {
-                "CloseTime": {
-                    "shape": "epochTimeMillis"
+                "Id": {
+                    "shape": "StandardLengthString"
                 },
-                "LeaderboardArn": {
-                    "shape": "LeaderboardArn"
+                "Name": {
+                    "shape": "StandardLengthString"
                 },
-                "LeaderboardName": {
-                    "shape": "LeaderboardName"
+                "Rewards": {
+                    "shape": "Rewards"
                 },
-                "RaceType": {
+                "Type": {
                     "shape": "RaceType"
                 },
-                "WinnerAlias": {
-                    "shape": "Alias"
+                "UserAvatarConfig": {
+                    "shape": "AvatarConfig"
                 }
             },
-            "required": [
-                "LeaderboardArn",
-                "LeaderboardName",
-                "WinnerAlias",
-                "CloseTime",
-                "RaceType"
-            ],
             "type": "structure"
         },
         "WinnerList": {
             "member": {
                 "shape": "Winner"
             },
             "type": "list"
@@ -4411,14 +4980,17 @@
         },
         "epochTimeMillis": {
             "type": "long"
         },
         "integer": {
             "type": "integer"
         },
+        "long": {
+            "type": "long"
+        },
         "map": {
             "key": {
                 "shape": "StandardLengthString"
             },
             "type": "map",
             "value": {
                 "shape": "StandardLengthString"
```

### Comparing `deepracer-utils-1.0.4rc0/deepracer/console/helper.py` & `deepracer-utils-1.0.5rc0/deepracer/console/helper.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/deepracer/logs/handler.py` & `deepracer-utils-1.0.5rc0/deepracer/logs/handler.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/deepracer/logs/log.py` & `deepracer-utils-1.0.5rc0/deepracer/logs/log.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/deepracer/logs/log_utils.py` & `deepracer-utils-1.0.5rc0/deepracer/logs/log_utils.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/deepracer/logs/metrics.py` & `deepracer-utils-1.0.5rc0/deepracer/logs/metrics.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/deepracer/model/visualization.py` & `deepracer-utils-1.0.5rc0/deepracer/model/visualization.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/deepracer/tracks/track_utils.py` & `deepracer-utils-1.0.5rc0/deepracer/tracks/track_utils.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/deepracer/update_action_speeds/action_space.json` & `deepracer-utils-1.0.5rc0/deepracer/update_action_speeds/action_space.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/deepracer/update_action_speeds/updateActionSpeeds.py` & `deepracer-utils-1.0.5rc0/deepracer/update_action_speeds/updateActionSpeeds.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/deepracer_utils.egg-info/PKG-INFO` & `deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: deepracer-utils
-Version: 1.0.4rc0
+Version: 1.0.5rc0
 Summary: A set of tools for working with DeepRacer training
 Home-page: https://github.com/aws-deepracer-community/deepracer-utils/
 Author: AWS DeepRacer Community
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/aws-deepracer-community/deepracer-utils/issues
 Project-URL: Source, https://github.com/aws-deepracer-community/deepracer-utils/
 Keywords: aws deepracer awsdeepracer
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: Log Analysis
-Requires-Python: >=3.6.*, <4
+Requires-Python: >=3.6,<4.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: visualization
 License-File: LICENSE
 
 # Deepracer Utilities - Analyzing Your DeepRacer Model
```

### Comparing `deepracer-utils-1.0.4rc0/deepracer_utils.egg-info/SOURCES.txt` & `deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/docs/development.md` & `deepracer-utils-1.0.5rc0/docs/development.md`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/setup.py` & `deepracer-utils-1.0.5rc0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,20 +29,20 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
 
         'Topic :: Internet :: Log Analysis'
     ],
     keywords='aws deepracer awsdeepracer',
-    python_requires='>=3.6.*, <4',
+    python_requires='>=3.6,<4.0',
     install_requires=[
         'boto3>=1.12.0',
         'python-dateutil<3.0.0,>=2.1',
         'numpy>=1.18.0',
-        'shapely>=1.7.0',
+        'shapely>=1.7.0,<2.0',
         'matplotlib>=3.1.0',
         'pandas>=1.0.0',
         'scikit-learn>=0.22.0',
         'joblib>=0.17.0'
     ],
     extras_require={
         'visualization': ['tensorflow==1.15.4', 'opencv-python', 'python-resize-image'],
```

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/console/test_helper.py` & `deepracer-utils-1.0.5rc0/tests/deepracer/console/test_helper.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612082853-IBZwYd0MRMqgwKlAe7bb0A-robomaker.log` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612082853-IBZwYd0MRMqgwKlAe7bb0A-robomaker.log`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612083839-PMfF__s5QJSQT_-E0rEYwg-robomaker.log` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612083839-PMfF__s5QJSQT_-E0rEYwg-robomaker.log`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703172842-wDhqXQC-SkGOinLUdZCQZQ-robomaker.log` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703172842-wDhqXQC-SkGOinLUdZCQZQ-robomaker.log`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703174103-zi4mg1gOTvugQLn-3BfL4g-robomaker.log` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703174103-zi4mg1gOTvugQLn-3BfL4g-robomaker.log`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230350-EHNgTNY2T9-77qXhqjBi6A-sagemaker.log` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230350-EHNgTNY2T9-77qXhqjBi6A-sagemaker.log`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230353-EHNgTNY2T9-77qXhqjBi6A-robomaker.log` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230353-EHNgTNY2T9-77qXhqjBi6A-robomaker.log`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612082523-IBZwYd0MRMqgwKlAe7bb0A.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612082523-IBZwYd0MRMqgwKlAe7bb0A.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612083508-PMfF__s5QJSQT_-E0rEYwg.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612083508-PMfF__s5QJSQT_-E0rEYwg.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/metrics/training/training-20220611205309-EHNgTNY2T9-77qXhqjBi6A.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/training/training-20220611205309-EHNgTNY2T9-77qXhqjBi6A.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/1-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/1-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/10-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/10-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/11-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/11-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/12-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/12-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/13-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/13-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/14-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/14-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/15-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/15-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/16-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/16-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/17-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/17-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/18-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/18-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/19-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/19-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/2-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/2-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/20-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/20-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/21-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/21-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/22-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/22-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/23-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/23-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/24-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/24-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/25-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/25-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/26-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/26-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/27-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/27-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/3-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/3-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/4-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/4-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/5-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/5-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/6-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/6-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/7-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/7-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/8-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/8-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/9-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/9-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200242.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200242.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200509.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200509.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200711.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200711.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/TrainingMetrics.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/TrainingMetrics.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/model/model_metadata.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/model/model_metadata.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/reward_function.py` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/reward_function.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/1-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/1-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/10-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/10-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/11-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/11-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/12-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/12-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/13-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/13-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/14-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/14-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/15-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/15-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/16-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/16-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/17-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/17-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/18-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/18-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/19-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/19-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/2-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/2-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/20-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/20-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/21-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/21-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/22-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/22-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/23-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/23-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/24-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/24-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/25-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/25-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/26-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/26-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/3-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/3-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/4-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/4-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/5-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/5-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/6-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/6-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/7-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/7-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/8-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/8-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/9-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/9-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/1-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/1-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/10-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/10-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/11-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/11-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/12-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/12-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/13-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/13-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/14-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/14-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/15-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/15-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/16-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/16-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/17-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/17-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/18-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/18-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/19-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/19-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/2-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/2-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/20-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/20-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/21-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/21-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/22-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/22-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/3-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/3-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/4-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/4-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/5-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/5-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/6-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/6-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/7-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/7-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/8-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/8-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/9-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/9-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/1-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/1-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/10-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/10-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/11-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/11-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/12-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/12-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/13-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/13-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/14-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/14-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/15-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/15-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/16-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/16-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/17-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/17-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/18-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/18-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/19-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/19-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/2-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/2-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/20-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/20-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/21-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/21-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/22-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/22-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/3-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/3-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/4-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/4-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/5-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/5-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/6-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/6-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/7-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/7-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/8-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/8-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/9-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/9-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/1-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/1-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/10-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/10-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/11-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/11-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/12-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/12-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/13-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/13-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/14-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/14-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/15-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/15-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/16-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/16-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/17-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/17-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/18-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/18-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/19-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/19-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/2-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/2-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/20-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/20-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/21-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/21-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/22-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/22-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/3-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/3-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/4-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/4-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/5-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/5-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/6-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/6-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/7-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/7-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/8-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/8-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/9-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/9-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201503.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201503.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201704.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201704.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201920.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201920.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_1.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_1.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_2.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_2.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/sample-drfc-3-logs/model/model_metadata.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/model/model_metadata.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/test_logs.py` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/test_logs.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/logs/test_metrics.py` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/test_metrics.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.4rc0/tests/deepracer/track_utils/test_track_utils.py` & `deepracer-utils-1.0.5rc0/tests/deepracer/track_utils/test_track_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from deepracer.tracks import GeometryUtils
+from deepracer.tracks import GeometryUtils, TrackIO
 
 
 class TestGeometryUtils:
     def test_vector(self):
         assert np.all([23, 67] == GeometryUtils.vector([50, 100], [27, 33]))
 
     def test_angle_zero(self):
@@ -63,7 +63,14 @@
     def test_get_a_point_on_a_line_closest_to_point_2(self):
         assert np.all(
             [2.0, -1.0] ==
             GeometryUtils.get_a_point_on_a_line_closest_to_point(
                 [0.0, 0.0], [2.0, -1.0], [4.0, 3.0]
             )
         )
+
+
+class TestLoadTrack:
+
+    def test_load_a_track(self):
+        tu = TrackIO(base_path='./deepracer/track_utils/tracks')
+        tu.load_track('reinvent_base')
```

### Comparing `deepracer-utils-1.0.4rc0/versioneer.py` & `deepracer-utils-1.0.5rc0/versioneer.py`

 * *Files identical despite different names*

