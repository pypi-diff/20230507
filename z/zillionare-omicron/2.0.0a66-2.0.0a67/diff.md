# Comparing `tmp/zillionare_omicron-2.0.0a66.tar.gz` & `tmp/zillionare_omicron-2.0.0a67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillionare_omicron-2.0.0a66.tar", max compression
+gzip compressed data, was "zillionare_omicron-2.0.0a67.tar", max compression
```

## Comparing `zillionare_omicron-2.0.0a66.tar` & `zillionare_omicron-2.0.0a67.tar`

### file list

```diff
@@ -1,116 +1,124 @@
--rw-r--r--   0        0        0      112 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a66/AUTHORS.md
--rw-r--r--   0        0        0     1561 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a66/HISTORY.md
--rw-r--r--   0        0        0     1068 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a66/LICENSE
--rw-r--r--   0        0        0     1880 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a66/README.md
--rw-r--r--   0        0        0   503846 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/_static/Omicron_Windows10.docx
--rw-r--r--   0        0        0     5620 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a66/docs/_static/jetbrains-variant-3.svg
--rw-r--r--   0        0        0       84 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/dal/flux.md
--rw-r--r--   0        0        0      110 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/dal/influxclient.md
--rw-r--r--   0        0        0      189 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/dal/serialize.md
--rw-r--r--   0        0        0     5772 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/metrics.md
--rw-r--r--   0        0        0      203 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/omicron.md
--rw-r--r--   0        0        0       73 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/plotting.md
--rw-r--r--   0        0        0       68 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/security.md
--rw-r--r--   0        0        0       65 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/stock.md
--rw-r--r--   0        0        0       58 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/talib.md
--rw-r--r--   0        0        0       57 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/api/timeframe.md
--rw-r--r--   0        0        0       66 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a66/docs/api/triggers.md
--rw-r--r--   0        0        0      907 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a66/docs/css/extra.css
--rw-r--r--   0        0        0     1778 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/developer.md
--rw-r--r--   0        0        0       43 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a66/docs/history.md
--rw-r--r--   0        0        0       42 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a66/docs/index.md
--rw-r--r--   0        0        0     1820 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/installation.md
--rw-r--r--   0        0        0     9823 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/docs/usage.md
--rw-r--r--   0        0        0      920 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/omicron/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a66/omicron/config/__init__.py
--rw-r--r--   0        0        0    56389 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/config/calendar.json
--rw-r--r--   0        0        0      441 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/config/defaults.yaml
--rw-r--r--   0        0        0      378 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/config/dev.yaml
--rw-r--r--   0        0        0     1334 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/config/schema.py
--rw-r--r--   0        0        0      816 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a66/omicron/config/sql/v0.6.sql
--rw-r--r--   0        0        0     2785 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/config/sql/v1.0.sql
--rw-r--r--   0        0        0       46 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a66/omicron/core/__init__.py
--rw-r--r--   0        0        0      140 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/core/constants.py
--rw-r--r--   0        0        0     1095 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/core/errors.py
--rw-r--r--   0        0        0       46 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/core/events.py
--rw-r--r--   0        0        0     6517 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/core/triggers.py
--rw-r--r--   0        0        0       71 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/dal/__init__.py
--rw-r--r--   0        0        0     3215 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/dal/cache.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/dal/influx/__init__.py
--rw-r--r--   0        0        0      370 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/dal/influx/errors.py
--rw-r--r--   0        0        0      996 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a66/omicron/dal/influx/escape.py
--rw-r--r--   0        0        0    19097 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/dal/influx/flux.py
--rw-r--r--   0        0        0    16805 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/dal/influx/influxclient.py
--rw-r--r--   0        0        0    27708 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/dal/influx/serialize.py
--rw-r--r--   0        0        0       78 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/extensions/__init__.py
--rw-r--r--   0        0        0      656 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/extensions/decimals.py
--rw-r--r--   0        0        0    15929 2023-05-01 02:32:25.512887 zillionare_omicron-2.0.0a66/omicron/extensions/np.py
--rw-r--r--   0        0        0      492 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/models/__init__.py
--rw-r--r--   0        0        0     7867 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a66/omicron/models/board.py
--rw-r--r--   0        0        0    26127 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/models/security.py
--rw-r--r--   0        0        0    53741 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/models/stock.py
--rw-r--r--   0        0        0    41959 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/models/timeframe.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/notify/__init__.py
--rw-r--r--   0        0        0     5472 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/notify/dingtalk.py
--rw-r--r--   0        0        0     6006 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/notify/mail.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/notify/tts.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/plotting/__init__.py
--rw-r--r--   0        0        0    14220 2023-05-03 09:06:32.908144 zillionare_omicron-2.0.0a66/omicron/plotting/candlestick.py
--rw-r--r--   0        0        0     8636 2023-05-03 08:59:53.293039 zillionare_omicron-2.0.0a66/omicron/plotting/metrics.py
--rw-r--r--   0        0        0      114 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a66/omicron/talib/__init__.py
--rw-r--r--   0        0        0     9958 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a66/omicron/talib/core.py
--rw-r--r--   0        0        0    23141 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a66/omicron/talib/morph.py
--rwxr-xr-x   0        0        0     3312 2023-05-03 10:52:55.254047 zillionare_omicron-2.0.0a66/pyproject.toml
--rw-r--r--   0        0        0     5556 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a66/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a66/tests/core/__init__.py
--rw-r--r--   0        0        0      297 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a66/tests/core/test_errors.py
--rw-r--r--   0        0        0     3615 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a66/tests/core/test_triggers.py
--rw-r--r--   0        0        0     1024 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/core/test_types.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/dal/__init__.py
--rw-r--r--   0        0        0      622 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/dal/influx/__init__.py
--rw-r--r--   0        0        0     1177 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/dal/influx/test_escape.py
--rw-r--r--   0        0        0     8531 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/dal/influx/test_flux.py
--rw-r--r--   0        0        0    14284 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/dal/influx/test_influxclient.py
--rw-r--r--   0        0        0    15710 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/dal/influx/test_serialize.py
--rw-r--r--   0        0        0     1253 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.15m.csv
--rw-r--r--   0        0        0      118 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.1M.csv
--rw-r--r--   0        0        0      188 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.1d.csv
--rw-r--r--   0        0        0    22206 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.1m.csv
--rw-r--r--   0        0        0      115 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.1w.csv
--rw-r--r--   0        0        0      654 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.30m.csv
--rw-r--r--   0        0        0     3633 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.5m.csv
--rw-r--r--   0        0        0      352 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.60m.csv
--rw-r--r--   0        0        0     8089 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.1d.csv
--rw-r--r--   0        0        0    22419 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.1m.csv
--rw-r--r--   0        0        0     7166 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.1w.csv
--rw-r--r--   0        0        0     8096 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.30m.csv
--rw-r--r--   0        0        0     7585 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.1d.csv
--rw-r--r--   0        0        0    20344 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.1m.csv
--rw-r--r--   0        0        0     6443 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.1w.csv
--rw-r--r--   0        0        0     7688 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.30m.csv
--rw-r--r--   0        0        0     1145 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/README.md
--rw-r--r--   0        0        0     2191 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a66/tests/data/bars_1d.pkl
--rw-r--r--   0        0        0   408697 2023-01-24 12:41:24.943079 zillionare_omicron-2.0.0a66/tests/data/bars_1m.pkl
--rw-r--r--   0        0        0      713 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/data/limits.csv
--rw-r--r--   0        0        0   164066 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/data/stock_bars_flux_query.txt
--rw-r--r--   0        0        0     6315 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/data/test.jpg
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/extensions/__init__.py
--rw-r--r--   0        0        0      594 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/extensions/test_decimals.py
--rw-r--r--   0        0        0     9864 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/extensions/test_np.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/models/__init__.py
--rw-r--r--   0        0        0     6802 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/models/test_board.py
--rw-r--r--   0        0        0    11161 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a66/tests/models/test_security.py
--rw-r--r--   0        0        0    68822 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/models/test_stock.py
--rw-r--r--   0        0        0    36351 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/models/test_timeframe.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/notify/__init__.py
--rw-r--r--   0        0        0      823 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/notify/test_dingtalk.py
--rw-r--r--   0        0        0     2686 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/notify/test_mail.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/performance/influx/__init__.py
--rw-r--r--   0        0        0     3317 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/performance/influx/end2end.py
--rw-r--r--   0        0        0     4197 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/performance/influx/serialize.py
--rw-r--r--   0        0        0      294 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/performance/readme.md
--rw-r--r--   0        0        0      406 2023-01-19 03:32:37.466696 zillionare_omicron-2.0.0a66/tests/pyrightconfig.json
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/talib/__init__.py
--rw-r--r--   0        0        0     2917 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/talib/test_core.py
--rw-r--r--   0        0        0    37991 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a66/tests/talib/test_morph.py
--rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 zillionare_omicron-2.0.0a66/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a67/AUTHORS.md
+-rw-r--r--   0        0        0     1561 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a67/HISTORY.md
+-rw-r--r--   0        0        0     1068 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a67/LICENSE
+-rw-r--r--   0        0        0     1331 2023-05-07 03:30:41.208098 zillionare_omicron-2.0.0a67/README.md
+-rw-r--r--   0        0        0   503846 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/_static/Omicron_Windows10.docx
+-rw-r--r--   0        0        0     5620 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a67/docs/_static/jetbrains-variant-3.svg
+-rw-r--r--   0        0        0       84 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/dal/flux.md
+-rw-r--r--   0        0        0      110 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/dal/influxclient.md
+-rw-r--r--   0        0        0      189 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/dal/serialize.md
+-rw-r--r--   0        0        0     5772 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/metrics.md
+-rw-r--r--   0        0        0      203 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/omicron.md
+-rw-r--r--   0        0        0      142 2023-05-07 03:32:06.872770 zillionare_omicron-2.0.0a67/docs/api/plotting.md
+-rw-r--r--   0        0        0       68 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/security.md
+-rw-r--r--   0        0        0       65 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/stock.md
+-rw-r--r--   0        0        0       21 2023-05-07 03:32:19.736871 zillionare_omicron-2.0.0a67/docs/api/strategy.md
+-rw-r--r--   0        0        0       58 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/talib.md
+-rw-r--r--   0        0        0       57 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/api/timeframe.md
+-rw-r--r--   0        0        0       66 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a67/docs/api/triggers.md
+-rw-r--r--   0        0        0      907 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a67/docs/css/extra.css
+-rw-r--r--   0        0        0     1778 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/developer.md
+-rw-r--r--   0        0        0       43 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a67/docs/history.md
+-rw-r--r--   0        0        0       42 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a67/docs/index.md
+-rw-r--r--   0        0        0     1820 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/installation.md
+-rw-r--r--   0        0        0     9823 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/docs/usage.md
+-rw-r--r--   0        0        0      920 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/omicron/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a67/omicron/config/__init__.py
+-rw-r--r--   0        0        0    56389 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/config/calendar.json
+-rw-r--r--   0        0        0      441 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/config/defaults.yaml
+-rw-r--r--   0        0        0      378 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/config/dev.yaml
+-rw-r--r--   0        0        0     1334 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/config/schema.py
+-rw-r--r--   0        0        0      816 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a67/omicron/config/sql/v0.6.sql
+-rw-r--r--   0        0        0     2785 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/config/sql/v1.0.sql
+-rw-r--r--   0        0        0       46 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a67/omicron/core/__init__.py
+-rw-r--r--   0        0        0      140 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/core/constants.py
+-rw-r--r--   0        0        0     1095 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/core/errors.py
+-rw-r--r--   0        0        0       46 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/core/events.py
+-rw-r--r--   0        0        0     6517 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/core/triggers.py
+-rw-r--r--   0        0        0       71 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/dal/__init__.py
+-rw-r--r--   0        0        0     3215 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/dal/cache.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/dal/influx/__init__.py
+-rw-r--r--   0        0        0      370 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/dal/influx/errors.py
+-rw-r--r--   0        0        0      996 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a67/omicron/dal/influx/escape.py
+-rw-r--r--   0        0        0    19097 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/dal/influx/flux.py
+-rw-r--r--   0        0        0    16805 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/dal/influx/influxclient.py
+-rw-r--r--   0        0        0    27708 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/dal/influx/serialize.py
+-rw-r--r--   0        0        0       78 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/extensions/__init__.py
+-rw-r--r--   0        0        0      656 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/extensions/decimals.py
+-rw-r--r--   0        0        0    15929 2023-05-01 02:32:25.512887 zillionare_omicron-2.0.0a67/omicron/extensions/np.py
+-rw-r--r--   0        0        0      492 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/models/__init__.py
+-rw-r--r--   0        0        0     7867 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a67/omicron/models/board.py
+-rw-r--r--   0        0        0    26127 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/models/security.py
+-rw-r--r--   0        0        0    53741 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/models/stock.py
+-rw-r--r--   0        0        0    41959 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/models/timeframe.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/notify/__init__.py
+-rw-r--r--   0        0        0     5472 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/notify/dingtalk.py
+-rw-r--r--   0        0        0     6006 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/notify/mail.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/notify/tts.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/plotting/__init__.py
+-rw-r--r--   0        0        0    14220 2023-05-03 09:06:32.908144 zillionare_omicron-2.0.0a67/omicron/plotting/candlestick.py
+-rw-r--r--   0        0        0     9039 2023-05-07 05:01:15.503704 zillionare_omicron-2.0.0a67/omicron/plotting/metrics.py
+-rw-r--r--   0        0        0        0 2023-05-07 01:07:54.376952 zillionare_omicron-2.0.0a67/omicron/strategy/__init__.py
+-rw-r--r--   0        0        0     8912 2023-05-07 03:40:18.247316 zillionare_omicron-2.0.0a67/omicron/strategy/base.py
+-rw-r--r--   0        0        0     1099 2023-05-07 02:09:33.855184 zillionare_omicron-2.0.0a67/omicron/strategy/sma.py
+-rw-r--r--   0        0        0      114 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a67/omicron/talib/__init__.py
+-rw-r--r--   0        0        0     9958 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a67/omicron/talib/core.py
+-rw-r--r--   0        0        0    23141 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a67/omicron/talib/morph.py
+-rwxr-xr-x   0        0        0     3391 2023-05-07 04:10:04.992167 zillionare_omicron-2.0.0a67/pyproject.toml
+-rw-r--r--   0        0        0     5556 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a67/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a67/tests/core/__init__.py
+-rw-r--r--   0        0        0      297 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a67/tests/core/test_errors.py
+-rw-r--r--   0        0        0     3615 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a67/tests/core/test_triggers.py
+-rw-r--r--   0        0        0     1024 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/core/test_types.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/dal/__init__.py
+-rw-r--r--   0        0        0      622 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/dal/influx/__init__.py
+-rw-r--r--   0        0        0     1177 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/dal/influx/test_escape.py
+-rw-r--r--   0        0        0     8531 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/dal/influx/test_flux.py
+-rw-r--r--   0        0        0    14284 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/dal/influx/test_influxclient.py
+-rw-r--r--   0        0        0    15710 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/dal/influx/test_serialize.py
+-rw-r--r--   0        0        0     1253 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.15m.csv
+-rw-r--r--   0        0        0      118 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.1M.csv
+-rw-r--r--   0        0        0      188 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.1d.csv
+-rw-r--r--   0        0        0    22206 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.1m.csv
+-rw-r--r--   0        0        0      115 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.1w.csv
+-rw-r--r--   0        0        0      654 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.30m.csv
+-rw-r--r--   0        0        0     3633 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.5m.csv
+-rw-r--r--   0        0        0      352 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.60m.csv
+-rw-r--r--   0        0        0  1059606 2023-05-07 02:32:26.029160 zillionare_omicron-2.0.0a67/tests/data/000001.XSHG.1m.csv
+-rw-r--r--   0        0        0     8089 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.1d.csv
+-rw-r--r--   0        0        0    22419 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.1m.csv
+-rw-r--r--   0        0        0     7166 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.1w.csv
+-rw-r--r--   0        0        0     8096 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.30m.csv
+-rw-r--r--   0        0        0     7585 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.1d.csv
+-rw-r--r--   0        0        0    20344 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.1m.csv
+-rw-r--r--   0        0        0     6443 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.1w.csv
+-rw-r--r--   0        0        0     7688 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.30m.csv
+-rw-r--r--   0        0        0     4206 2023-05-07 02:31:54.553073 zillionare_omicron-2.0.0a67/tests/data/600000.XSHG.1d.csv
+-rw-r--r--   0        0        0     1145 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/README.md
+-rw-r--r--   0        0        0     2191 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a67/tests/data/bars_1d.pkl
+-rw-r--r--   0        0        0   408697 2023-01-24 12:41:24.943079 zillionare_omicron-2.0.0a67/tests/data/bars_1m.pkl
+-rw-r--r--   0        0        0      713 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/data/limits.csv
+-rw-r--r--   0        0        0   164066 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/data/stock_bars_flux_query.txt
+-rw-r--r--   0        0        0     6315 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/data/test.jpg
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/extensions/__init__.py
+-rw-r--r--   0        0        0      594 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/extensions/test_decimals.py
+-rw-r--r--   0        0        0     9864 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/extensions/test_np.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/models/__init__.py
+-rw-r--r--   0        0        0     6802 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/models/test_board.py
+-rw-r--r--   0        0        0    11161 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a67/tests/models/test_security.py
+-rw-r--r--   0        0        0    68822 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/models/test_stock.py
+-rw-r--r--   0        0        0    36351 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/models/test_timeframe.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/notify/__init__.py
+-rw-r--r--   0        0        0      823 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/notify/test_dingtalk.py
+-rw-r--r--   0        0        0     2686 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/notify/test_mail.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/performance/influx/__init__.py
+-rw-r--r--   0        0        0     3317 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/performance/influx/end2end.py
+-rw-r--r--   0        0        0     4197 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/performance/influx/serialize.py
+-rw-r--r--   0        0        0      294 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/performance/readme.md
+-rw-r--r--   0        0        0      406 2023-01-19 03:32:37.466696 zillionare_omicron-2.0.0a67/tests/pyrightconfig.json
+-rw-r--r--   0        0        0        0 2023-05-07 02:10:22.915444 zillionare_omicron-2.0.0a67/tests/strategy/__init__.py
+-rw-r--r--   0        0        0     1517 2023-05-07 03:14:15.795948 zillionare_omicron-2.0.0a67/tests/strategy/test_strategy.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/talib/__init__.py
+-rw-r--r--   0        0        0     2917 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/talib/test_core.py
+-rw-r--r--   0        0        0    37991 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a67/tests/talib/test_morph.py
+-rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 zillionare_omicron-2.0.0a67/PKG-INFO
```

### Comparing `zillionare_omicron-2.0.0a66/HISTORY.md` & `zillionare_omicron-2.0.0a67/HISTORY.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/LICENSE` & `zillionare_omicron-2.0.0a67/LICENSE`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/README.md` & `zillionare_omicron-2.0.0a67/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 
 <h1 align="center">Omicron - Core Library for Zillionare</h1>
 
 
 [![Version](http://img.shields.io/pypi/v/zillionare-omicron?color=brightgreen)](https://pypi.python.org/pypi/zillionare-omicron)
 [![CI Status](https://github.com/zillionare/omicron/actions/workflows/release.yml/badge.svg)](https://github.com/zillionare/omicron)
 [![Code Coverage](https://img.shields.io/codecov/c/github/zillionare/omicron)](https://app.codecov.io/gh/zillionare/omicron)
-<<<<<<< HEAD
-=======
-[![ReadtheDos](https://readthedocs.org/projects/omicron/badge/?version=latest)](https://omicron.readthedocs.io/en/latest/?badge=latest)
->>>>>>> master
 [![Downloads](https://pepy.tech/badge/zillionare-omicron)](https://pepy.tech/project/zillionare-omicron)
 [![License](https://img.shields.io/badge/License-MIT.svg)](https://opensource.org/licenses/MIT)
 [![Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # Contents
 
 ## 简介
@@ -23,14 +19,9 @@
 
 Omicron是大富翁量化框架的一部分。您必须至少安装并运行[Omega](https://zillionare.github.io/omega)，然后才能利用omicron来访问上述数据。
 
 [使用文档](https://zillionare.github.io/omicron)
 
 ## Credits
 
-<<<<<<< HEAD
 Zillionare-Omicron采用[Python Project Wizard](https://zillionare.github.io/python-project-wizard)构建。
-=======
-* [Cookiecutter](https://github.com/audreyr/cookiecutter)
-* [Cookiecutter-pypackage](https://github.com/zillionare/cookiecutter-pypackage)
-* ![JetBrains Black Box Logo logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_square.svg) [Pycharm开源项目支持计划](https://www.jetbrains.com/?from=zillionare-omega)
->>>>>>> master
+
```

### Comparing `zillionare_omicron-2.0.0a66/docs/_static/Omicron_Windows10.docx` & `zillionare_omicron-2.0.0a67/docs/_static/Omicron_Windows10.docx`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/docs/_static/jetbrains-variant-3.svg` & `zillionare_omicron-2.0.0a67/docs/_static/jetbrains-variant-3.svg`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/docs/api/metrics.md` & `zillionare_omicron-2.0.0a67/docs/api/metrics.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/docs/css/extra.css` & `zillionare_omicron-2.0.0a67/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/docs/developer.md` & `zillionare_omicron-2.0.0a67/docs/developer.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/docs/installation.md` & `zillionare_omicron-2.0.0a67/docs/installation.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/docs/usage.md` & `zillionare_omicron-2.0.0a67/docs/usage.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/__init__.py` & `zillionare_omicron-2.0.0a67/omicron/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/config/calendar.json` & `zillionare_omicron-2.0.0a67/omicron/config/calendar.json`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/config/schema.py` & `zillionare_omicron-2.0.0a67/omicron/config/schema.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/config/sql/v0.6.sql` & `zillionare_omicron-2.0.0a67/omicron/config/sql/v0.6.sql`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/config/sql/v1.0.sql` & `zillionare_omicron-2.0.0a67/omicron/config/sql/v1.0.sql`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/core/errors.py` & `zillionare_omicron-2.0.0a67/omicron/core/errors.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/core/triggers.py` & `zillionare_omicron-2.0.0a67/omicron/core/triggers.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/dal/cache.py` & `zillionare_omicron-2.0.0a67/omicron/dal/cache.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/dal/influx/escape.py` & `zillionare_omicron-2.0.0a67/omicron/dal/influx/escape.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/dal/influx/flux.py` & `zillionare_omicron-2.0.0a67/omicron/dal/influx/flux.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/dal/influx/influxclient.py` & `zillionare_omicron-2.0.0a67/omicron/dal/influx/influxclient.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/dal/influx/serialize.py` & `zillionare_omicron-2.0.0a67/omicron/dal/influx/serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/extensions/decimals.py` & `zillionare_omicron-2.0.0a67/omicron/extensions/decimals.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/extensions/np.py` & `zillionare_omicron-2.0.0a67/omicron/extensions/np.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/models/board.py` & `zillionare_omicron-2.0.0a67/omicron/models/board.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/models/security.py` & `zillionare_omicron-2.0.0a67/omicron/models/security.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/models/stock.py` & `zillionare_omicron-2.0.0a67/omicron/models/stock.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/models/timeframe.py` & `zillionare_omicron-2.0.0a67/omicron/models/timeframe.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/notify/dingtalk.py` & `zillionare_omicron-2.0.0a67/omicron/notify/dingtalk.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/notify/mail.py` & `zillionare_omicron-2.0.0a67/omicron/notify/mail.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/plotting/candlestick.py` & `zillionare_omicron-2.0.0a67/omicron/plotting/candlestick.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/plotting/metrics.py` & `zillionare_omicron-2.0.0a67/omicron/plotting/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,23 @@
+"""绘制回测资产曲线和指标图。
+
+示例:
+```python
+from omicron.plotting import MetricsGraph
+
+# calling some strategy's backtest and get bills/metrics
+mg = MetricsGraph(bills, metrics)
+
+await mg.plot()
+```
+注意此方法需要在notebook中调用。
+
+"""
 import datetime
+import logging
 from collections import defaultdict
 from copy import deepcopy
 from typing import List, Union
 
 import arrow
 import numpy as np
 import pandas as pd
@@ -12,14 +27,16 @@
 from plotly.subplots import make_subplots
 
 from omicron import tf
 from omicron.extensions import fill_nan
 from omicron.models.security import Security
 from omicron.models.stock import Stock
 
+logger = logging.getLogger(__name__)
+
 
 class MetricsGraph:
     def __init__(self, bills: dict, metrics: dict):
         self.metrics = metrics
         self.trades = bills["trades"]
         self.positions = bills["positions"]
         self.start = arrow.get(bills["assets"][0][0]).date()
@@ -66,19 +83,19 @@
     def _format_tick(self, frames: Union[Frame, List[Frame]]) -> Union[str, NDArray]:
         if type(frames) == datetime.date:
             x = frames
             return f"{x.year:02}-{x.month:02}-{x.day:02}"
         elif type(frames) == datetime.datetime:
             x = frames
             return f"{x.month:02}-{x.day:02} {x.hour:02}:{x.minute:02}"
-        elif type(frames[0]) == datetime.date:
+        elif type(frames[0]) == datetime.date:  # type: ignore
             return np.array([f"{x.year:02}-{x.month:02}-{x.day:02}" for x in frames])
         else:
             return np.array(
-                [f"{x.month:02}-{x.day:02} {x.hour:02}:{x.minute:02}" for x in frames]
+                [f"{x.month:02}-{x.day:02} {x.hour:02}:{x.minute:02}" for x in frames]  # type: ignore
             )
 
     async def _metrics_traces(self):
         metric_names = {
             "start": "起始日",
             "end": "结束日",
             "window": "资产暴露窗口",
@@ -197,14 +214,15 @@
             hover = f"资产:{asset/10000:.1f}万<br>{'<br>'.join(text)}"
             data.append(hover)
 
         trace = go.Scatter(x=X, y=Y, mode="markers", text=data, name="交易详情")
         return trace
 
     async def plot(self, baseline_code: str = "399300.XSHE"):
+        """绘制资产曲线及回测指标图"""
         n = len(self.assets)
         bars = await Stock.get_bars(baseline_code, n, FrameType.DAY, self.end)
 
         baseline_prices = self._fill_missing_prices(bars, self.frames)
         baseline_prices /= baseline_prices[0]
 
         fig = make_subplots(
```

### Comparing `zillionare_omicron-2.0.0a66/omicron/talib/core.py` & `zillionare_omicron-2.0.0a67/omicron/talib/core.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/omicron/talib/morph.py` & `zillionare_omicron-2.0.0a67/omicron/talib/morph.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/pyproject.toml` & `zillionare_omicron-2.0.0a67/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [[tool.poetry.source]]
-name = "ali"
-url = "https://mirrors.aliyun.com/pypi/simple/"
+name = "tsinghua"
+url = "https://pypi.tuna.tsinghua.edu.cn/simple"
 default = true
 secondary=false
 
 
 [tool.poetry.dev-dependencies]
 [tool.poetry]
 name = "zillionare-omicron"
 packages = [
     {include = "omicron"}
 ]
-version = "2.0.0.a66"
+version = "2.0.0a67"
 description = "Core Library for Zillionare"
 authors = ["jieyu <code@jieyu.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zillionare-omicron.readthedocs.io"
 repository = "https://github.com/zillionare/omicron"
 documentation = "https://zillionare-omicron.readthedocs.io"
@@ -80,14 +80,15 @@
 pyreadline = {version = "^2.1", optional = true}
 mike = { version="^1.1.2", optional=true}
 freezegun = {version = "^1.2.1", optional = true}
 
 plotly = "^5.10.0"
 TA-Lib = {version = "^0.4.25", platform = "linux"}
 retry = {version = "^0.9.2"}
+zillionare-trader-client = {version = "^0.4.1", allow-prereleases = true}
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
     "flake8",
```

### Comparing `zillionare_omicron-2.0.0a66/tests/__init__.py` & `zillionare_omicron-2.0.0a67/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/core/test_triggers.py` & `zillionare_omicron-2.0.0a67/tests/core/test_triggers.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/core/test_types.py` & `zillionare_omicron-2.0.0a67/tests/core/test_types.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/dal/influx/__init__.py` & `zillionare_omicron-2.0.0a67/tests/dal/influx/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/dal/influx/test_escape.py` & `zillionare_omicron-2.0.0a67/tests/dal/influx/test_escape.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/dal/influx/test_flux.py` & `zillionare_omicron-2.0.0a67/tests/dal/influx/test_flux.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/dal/influx/test_influxclient.py` & `zillionare_omicron-2.0.0a67/tests/dal/influx/test_influxclient.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/dal/influx/test_serialize.py` & `zillionare_omicron-2.0.0a67/tests/dal/influx/test_serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.15m.csv` & `zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.15m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.1m.csv` & `zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.30m.csv` & `zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/000001.XSHE.5m.csv` & `zillionare_omicron-2.0.0a67/tests/data/000001.XSHE.5m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.1d.csv` & `zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.1m.csv` & `zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.1w.csv` & `zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.1w.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/000002.XSHE.30m.csv` & `zillionare_omicron-2.0.0a67/tests/data/000002.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.1d.csv` & `zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.1m.csv` & `zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.1w.csv` & `zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.1w.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/000004.XSHE.30m.csv` & `zillionare_omicron-2.0.0a67/tests/data/000004.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/README.md` & `zillionare_omicron-2.0.0a67/tests/data/README.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/bars_1d.pkl` & `zillionare_omicron-2.0.0a67/tests/data/bars_1d.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/bars_1m.pkl` & `zillionare_omicron-2.0.0a67/tests/data/bars_1m.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/limits.csv` & `zillionare_omicron-2.0.0a67/tests/data/limits.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/stock_bars_flux_query.txt` & `zillionare_omicron-2.0.0a67/tests/data/stock_bars_flux_query.txt`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/data/test.jpg` & `zillionare_omicron-2.0.0a67/tests/data/test.jpg`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/extensions/test_decimals.py` & `zillionare_omicron-2.0.0a67/tests/extensions/test_decimals.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/extensions/test_np.py` & `zillionare_omicron-2.0.0a67/tests/extensions/test_np.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/models/test_board.py` & `zillionare_omicron-2.0.0a67/tests/models/test_board.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/models/test_security.py` & `zillionare_omicron-2.0.0a67/tests/models/test_security.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/models/test_stock.py` & `zillionare_omicron-2.0.0a67/tests/models/test_stock.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/models/test_timeframe.py` & `zillionare_omicron-2.0.0a67/tests/models/test_timeframe.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/notify/test_dingtalk.py` & `zillionare_omicron-2.0.0a67/tests/notify/test_dingtalk.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/notify/test_mail.py` & `zillionare_omicron-2.0.0a67/tests/notify/test_mail.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/performance/influx/end2end.py` & `zillionare_omicron-2.0.0a67/tests/performance/influx/end2end.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/performance/influx/serialize.py` & `zillionare_omicron-2.0.0a67/tests/performance/influx/serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/talib/test_core.py` & `zillionare_omicron-2.0.0a67/tests/talib/test_core.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/tests/talib/test_morph.py` & `zillionare_omicron-2.0.0a67/tests/talib/test_morph.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a66/PKG-INFO` & `zillionare_omicron-2.0.0a67/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillionare-omicron
-Version: 2.0.0a66
+Version: 2.0.0a67
 Summary: Core Library for Zillionare
 Home-page: https://zillionare-omicron.readthedocs.io
 License: MIT
 Keywords: AI,quant,trade,stock
 Author: jieyu
 Author-email: code@jieyu.ai
 Requires-Python: >=3.8,<3.9
@@ -56,31 +56,28 @@
 Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
 Requires-Dist: sh (==1.14.1)
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
 Requires-Dist: tox (>=3.24.5,<4.0.0) ; extra == "dev"
 Requires-Dist: twine (>=3.8.0,<4.0.0) ; extra == "dev"
 Requires-Dist: zigzag (>=0.3,<0.4)
 Requires-Dist: zillionare-core-types (>=0.5.2,<0.6.0)
+Requires-Dist: zillionare-trader-client (>=0.4.1,<0.5.0)
 Project-URL: Documentation, https://zillionare-omicron.readthedocs.io
 Project-URL: Repository, https://github.com/zillionare/omicron
 Description-Content-Type: text/markdown
 
 
 ![](http://images.jieyu.ai/images/hot/zillionbanner.jpg)
 
 <h1 align="center">Omicron - Core Library for Zillionare</h1>
 
 
 [![Version](http://img.shields.io/pypi/v/zillionare-omicron?color=brightgreen)](https://pypi.python.org/pypi/zillionare-omicron)
 [![CI Status](https://github.com/zillionare/omicron/actions/workflows/release.yml/badge.svg)](https://github.com/zillionare/omicron)
 [![Code Coverage](https://img.shields.io/codecov/c/github/zillionare/omicron)](https://app.codecov.io/gh/zillionare/omicron)
-<<<<<<< HEAD
-=======
-[![ReadtheDos](https://readthedocs.org/projects/omicron/badge/?version=latest)](https://omicron.readthedocs.io/en/latest/?badge=latest)
->>>>>>> master
 [![Downloads](https://pepy.tech/badge/zillionare-omicron)](https://pepy.tech/project/zillionare-omicron)
 [![License](https://img.shields.io/badge/License-MIT.svg)](https://opensource.org/licenses/MIT)
 [![Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # Contents
 
 ## 简介
@@ -89,15 +86,10 @@
 
 Omicron是大富翁量化框架的一部分。您必须至少安装并运行[Omega](https://zillionare.github.io/omega)，然后才能利用omicron来访问上述数据。
 
 [使用文档](https://zillionare.github.io/omicron)
 
 ## Credits
 
-<<<<<<< HEAD
 Zillionare-Omicron采用[Python Project Wizard](https://zillionare.github.io/python-project-wizard)构建。
-=======
-* [Cookiecutter](https://github.com/audreyr/cookiecutter)
-* [Cookiecutter-pypackage](https://github.com/zillionare/cookiecutter-pypackage)
-* ![JetBrains Black Box Logo logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_square.svg) [Pycharm开源项目支持计划](https://www.jetbrains.com/?from=zillionare-omega)
->>>>>>> master
+
```

