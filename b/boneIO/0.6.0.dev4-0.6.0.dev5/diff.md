# Comparing `tmp/boneIO-0.6.0.dev4.tar.gz` & `tmp/boneIO-0.6.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boneIO-0.6.0.dev4.tar", last modified: Mon Apr 10 19:09:14 2023, max compression
+gzip compressed data, was "boneIO-0.6.0.dev5.tar", last modified: Sun May  7 10:27:55 2023, max compression
```

## Comparing `boneIO-0.6.0.dev4.tar` & `boneIO-0.6.0.dev5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    35149 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/LICENSE
--rw-r--r--   0        0        0      474 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/README.md
--rw-r--r--   0        0        0      147 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/__init__.py
--rw-r--r--   0        0        0     3155 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/bonecli.py
--rw-r--r--   0        0        0     2924 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/const.py
--rw-r--r--   0        0        0     8454 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/cover.py
--rw-r--r--   0        0        0        0 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/__init__.py
--rw-r--r--   0        0        0      168 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/adc.yaml
--rw-r--r--   0        0        0      326 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/config.yaml
--rw-r--r--   0        0        0      150 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/cover.yaml
--rw-r--r--   0        0        0     2883 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/input.yaml
--rw-r--r--   0        0        0     3392 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/led32x4A.yaml
--rw-r--r--   0        0        0     1691 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/output24x16A.yaml
--rw-r--r--   0        0        0     2403 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/example_config/output32x5A.yaml
--rw-r--r--   0        0        0    19372 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/fonts/danube__.ttf
--rw-r--r--   0        0        0     2039 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/__init__.py
--rw-r--r--   0        0        0      985 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/async_updater.py
--rw-r--r--   0        0        0     1169 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/click_timer.py
--rw-r--r--   0        0        0     1311 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/config.py
--rw-r--r--   0        0        0     7494 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/events.py
--rw-r--r--   0        0        0      637 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/exceptions.py
--rw-r--r--   0        0        0      885 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/filter.py
--rw-r--r--   0        0        0     2718 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/gpio.py
--rw-r--r--   0        0        0     6129 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/ha_discovery.py
--rw-r--r--   0        0        0    13488 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/loader.py
--rw-r--r--   0        0        0     1801 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/logger.py
--rw-r--r--   0        0        0      759 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/mqtt.py
--rw-r--r--   0        0        0      351 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/oled.py
--rw-r--r--   0        0        0     2430 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/onewire/W1ThermSensor.py
--rw-r--r--   0        0        0      448 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/onewire/__init__.py
--rw-r--r--   0        0        0     5169 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/onewire/ds2482.py
--rw-r--r--   0        0        0     2497 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/onewire/onewire.py
--rw-r--r--   0        0        0     1066 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/queue.py
--rw-r--r--   0        0        0     1994 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/state_manager.py
--rw-r--r--   0        0        0     5693 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/stats.py
--rw-r--r--   0        0        0     5806 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/timeperiod.py
--rw-r--r--   0        0        0      508 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/util.py
--rw-r--r--   0        0        0    11304 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/helper/yaml_util.py
--rw-r--r--   0        0        0       99 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/input/__init__.py
--rw-r--r--   0        0        0     2583 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/input/gpio.py
--rw-r--r--   0        0        0    20273 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/manager.py
--rw-r--r--   0        0        0     4176 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/modbus.py
--rw-r--r--   0        0        0     6983 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/mqtt_client.py
--rw-r--r--   0        0        0     5244 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/oled.py
--rw-r--r--   0        0        0      181 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/relay/__init__.py
--rw-r--r--   0        0        0     2629 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/relay/basic.py
--rw-r--r--   0        0        0     1163 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/relay/gpio.py
--rw-r--r--   0        0        0     2669 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/relay/mcp.py
--rw-r--r--   0        0        0     4873 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/relay/pca.py
--rw-r--r--   0        0        0     2287 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/runner.py
--rw-r--r--   0        0        0     1030 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/actions.yaml
--rw-r--r--   0        0        0      129 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/actions_sensor.yaml
--rw-r--r--   0        0        0      124 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/actions_switch.yaml
--rw-r--r--   0        0        0      286 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/filters.yaml
--rw-r--r--   0        0        0      304 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/filters_adc.yaml
--rw-r--r--   0        0        0       75 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/id.yaml
--rw-r--r--   0        0        0    12551 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/schema.yaml
--rw-r--r--   0        0        0       65 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/temp_unit.yaml
--rw-r--r--   0        0        0      133 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/schema/update_interval.yaml
--rw-r--r--   0        0        0      431 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/__init__.py
--rw-r--r--   0        0        0     1281 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/adc.py
--rw-r--r--   0        0        0     1289 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/gpio.py
--rw-r--r--   0        0        0     8500 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/__init__.py
--rw-r--r--   0        0        0     8810 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/dts1964_3f.json
--rw-r--r--   0        0        0      526 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/pt100.json
--rw-r--r--   0        0        0     2735 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/r4dcb08.json
--rw-r--r--   0        0        0     4145 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/sdm120.json
--rw-r--r--   0        0        0    10969 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/sdm630.json
--rw-r--r--   0        0        0     5592 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/modbus/sofar.json
--rw-r--r--   0        0        0     1659 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/temp/__init__.py
--rw-r--r--   0        0        0     2485 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/temp/dallas.py
--rw-r--r--   0        0        0      243 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/temp/lm75.py
--rw-r--r--   0        0        0      271 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/sensor/temp/mcp9808.py
--rw-r--r--   0        0        0       41 2023-04-10 19:08:41.962688 boneIO-0.6.0.dev4/boneio/version.py
--rw-r--r--   0        0        0     1871 2023-04-10 19:08:41.966688 boneIO-0.6.0.dev4/pyproject.toml
--rw-r--r--   0        0        0      166 2023-04-10 19:08:41.966688 boneIO-0.6.0.dev4/tests/32_5_config.yaml
--rw-r--r--   0        0        0      224 2023-04-10 19:08:41.966688 boneIO-0.6.0.dev4/tests/bandit.yaml
--rw-r--r--   0        0        0     1070 2023-04-10 19:08:41.966688 boneIO-0.6.0.dev4/tests/relay_32_5.py
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 boneIO-0.6.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/LICENSE
+-rw-r--r--   0        0        0      474 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/README.md
+-rw-r--r--   0        0        0      147 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/__init__.py
+-rw-r--r--   0        0        0     3341 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/bonecli.py
+-rw-r--r--   0        0        0     2924 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/const.py
+-rw-r--r--   0        0        0     8454 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/cover.py
+-rw-r--r--   0        0        0        0 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/adc.yaml
+-rw-r--r--   0        0        0      326 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/config.yaml
+-rw-r--r--   0        0        0      150 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/cover.yaml
+-rw-r--r--   0        0        0     2883 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/input.yaml
+-rw-r--r--   0        0        0     3392 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/led32x4A.yaml
+-rw-r--r--   0        0        0     1691 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/output24x16A.yaml
+-rw-r--r--   0        0        0     2403 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/output32x5A.yaml
+-rw-r--r--   0        0        0    19372 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/fonts/danube__.ttf
+-rw-r--r--   0        0        0     2039 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/__init__.py
+-rw-r--r--   0        0        0      985 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/async_updater.py
+-rw-r--r--   0        0        0     1169 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/click_timer.py
+-rw-r--r--   0        0        0     2233 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/config.py
+-rw-r--r--   0        0        0     7494 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/events.py
+-rw-r--r--   0        0        0      717 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/exceptions.py
+-rw-r--r--   0        0        0      885 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/filter.py
+-rw-r--r--   0        0        0     2718 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/gpio.py
+-rw-r--r--   0        0        0     6278 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/ha_discovery.py
+-rw-r--r--   0        0        0    13547 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/loader.py
+-rw-r--r--   0        0        0     1801 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/logger.py
+-rw-r--r--   0        0        0      765 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/mqtt.py
+-rw-r--r--   0        0        0      351 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/oled.py
+-rw-r--r--   0        0        0     2430 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/onewire/W1ThermSensor.py
+-rw-r--r--   0        0        0      448 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/onewire/__init__.py
+-rw-r--r--   0        0        0     5169 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/onewire/ds2482.py
+-rw-r--r--   0        0        0     2497 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/onewire/onewire.py
+-rw-r--r--   0        0        0     1066 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/queue.py
+-rw-r--r--   0        0        0     1994 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/state_manager.py
+-rw-r--r--   0        0        0     5693 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/stats.py
+-rw-r--r--   0        0        0     5806 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/timeperiod.py
+-rw-r--r--   0        0        0      508 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/util.py
+-rw-r--r--   0        0        0    11304 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/yaml_util.py
+-rw-r--r--   0        0        0       99 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/input/__init__.py
+-rw-r--r--   0        0        0     2597 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/input/gpio.py
+-rw-r--r--   0        0        0    21023 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/manager.py
+-rw-r--r--   0        0        0     4176 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/modbus.py
+-rw-r--r--   0        0        0     8331 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/mqtt_client.py
+-rw-r--r--   0        0        0     5244 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/oled.py
+-rw-r--r--   0        0        0      181 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/relay/__init__.py
+-rw-r--r--   0        0        0     2623 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/relay/basic.py
+-rw-r--r--   0        0        0     1163 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/relay/gpio.py
+-rw-r--r--   0        0        0     2669 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/relay/mcp.py
+-rw-r--r--   0        0        0     4873 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/relay/pca.py
+-rw-r--r--   0        0        0     2569 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/runner.py
+-rw-r--r--   0        0        0     1030 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/actions.yaml
+-rw-r--r--   0        0        0      124 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/actions_sensor.yaml
+-rw-r--r--   0        0        0      129 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/actions_switch.yaml
+-rw-r--r--   0        0        0      286 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/filters.yaml
+-rw-r--r--   0        0        0      304 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/filters_adc.yaml
+-rw-r--r--   0        0        0       75 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/id.yaml
+-rw-r--r--   0        0        0    12988 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/schema.yaml
+-rw-r--r--   0        0        0       65 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/temp_unit.yaml
+-rw-r--r--   0        0        0      133 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/update_interval.yaml
+-rw-r--r--   0        0        0      431 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/__init__.py
+-rw-r--r--   0        0        0     1281 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/adc.py
+-rw-r--r--   0        0        0     1303 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/gpio.py
+-rw-r--r--   0        0        0     8500 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/__init__.py
+-rw-r--r--   0        0        0     8810 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/dts1964_3f.json
+-rw-r--r--   0        0        0      526 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/pt100.json
+-rw-r--r--   0        0        0     2735 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/r4dcb08.json
+-rw-r--r--   0        0        0     4145 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/sdm120.json
+-rw-r--r--   0        0        0    10969 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/sdm630.json
+-rw-r--r--   0        0        0     5592 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/sofar.json
+-rw-r--r--   0        0        0     1659 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/temp/__init__.py
+-rw-r--r--   0        0        0     2485 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/temp/dallas.py
+-rw-r--r--   0        0        0      243 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/temp/lm75.py
+-rw-r--r--   0        0        0      271 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/temp/mcp9808.py
+-rw-r--r--   0        0        0       41 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/version.py
+-rw-r--r--   0        0        0     1873 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/tests/32_5_config.yaml
+-rw-r--r--   0        0        0      224 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/tests/bandit.yaml
+-rw-r--r--   0        0        0     1070 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/tests/relay_32_5.py
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 boneIO-0.6.0.dev5/PKG-INFO
```

### Comparing `boneIO-0.6.0.dev4/LICENSE` & `boneIO-0.6.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/bonecli.py` & `boneIO-0.6.0.dev5/boneio/bonecli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Bonecli script."""
+from __future__ import annotations
 import argparse
 import asyncio
 import logging
 import sys
 import os
+from typing import Any
 
 os.environ["W1THERMSENSOR_NO_KERNEL_MODULE"] = "1"
 
 from colorlog import ColoredFormatter
 from yaml import MarkedYAMLError
 
 from boneio.const import ACTION
 from boneio.helper import load_config_from_file
-from boneio.helper.exceptions import ConfigurationException
+from boneio.helper.exceptions import ConfigurationException, RestartRequestException
 from boneio.helper.logger import configure_logger
 from boneio.runner import async_run
 from boneio.version import __version__
 
 TASK_CANCELATION_TIMEOUT = 1
 
 _LOGGER = logging.getLogger(__name__)
@@ -65,31 +67,35 @@
         "--mqttpassword", help="Mqtt password to use if you don't want provide in file."
     )
     arguments = parser.parse_args()
 
     return arguments
 
 
-def run(config: str, debug: int, mqttusername: str = "", mqttpassword: str = ""):
+def run(config: str, debug: int, mqttusername: str = "", mqttpassword: str = "") -> int:
     """Run BoneIO."""
     _LOGGER.info("BoneIO %s starting.", __version__)
     try:
         _config = load_config_from_file(config_file=config)
         if not _config:
             _LOGGER.error("Config not loaded. Exiting.")
             return 1
         configure_logger(log_config=_config.get("logger"), debug=debug)
-        return asyncio.run(
+        asyncio.run(
             async_run(
                 config=_config,
                 config_file=config,
                 mqttusername=mqttusername,
                 mqttpassword=mqttpassword,
             ),
         )
+        return 0
+    except RestartRequestException as err:
+        _LOGGER.info(err)
+        return 0
     except (ConfigurationException, MarkedYAMLError) as err:
         _LOGGER.error("Failed to load config. %s Exiting.", err)
         return 1
 
 
 def main() -> int:
     """Start boneIO."""
```

### Comparing `boneIO-0.6.0.dev4/boneio/const.py` & `boneIO-0.6.0.dev5/boneio/const.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/cover.py` & `boneIO-0.6.0.dev5/boneio/cover.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/example_config/input.yaml` & `boneIO-0.6.0.dev5/boneio/example_config/input.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/example_config/led32x4A.yaml` & `boneIO-0.6.0.dev5/boneio/example_config/led32x4A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/example_config/output24x16A.yaml` & `boneIO-0.6.0.dev5/boneio/example_config/output24x16A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/example_config/output32x5A.yaml` & `boneIO-0.6.0.dev5/boneio/example_config/output32x5A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/fonts/danube__.ttf` & `boneIO-0.6.0.dev5/boneio/fonts/danube__.ttf`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/__init__.py` & `boneIO-0.6.0.dev5/boneio/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/async_updater.py` & `boneIO-0.6.0.dev5/boneio/helper/async_updater.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/click_timer.py` & `boneIO-0.6.0.dev5/boneio/helper/click_timer.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/events.py` & `boneIO-0.6.0.dev5/boneio/helper/events.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/exceptions.py` & `boneIO-0.6.0.dev5/boneio/helper/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 class BoneIOException(Exception):
     """BoneIO standard exception."""
 
 
 class GPIOInputException(BoneIOException):
     """GPIOInput Exception."""
 
+
 class GPIOOutputException(BoneIOException):
     """GPIOInput Exception."""
 
 
 class I2CError(BoneIOException):
     """I2C Exception."""
 
@@ -26,7 +27,11 @@
 
 class CoverRelayException(BoneIOException):
     """Cover configuration exception."""
 
 
 class ModbusUartException(BoneIOException):
     """Cover configuration exception."""
+
+
+class RestartRequestException(BoneIOException):
+    """Restart exception."""
```

### Comparing `boneIO-0.6.0.dev4/boneio/helper/filter.py` & `boneIO-0.6.0.dev5/boneio/helper/filter.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/gpio.py` & `boneIO-0.6.0.dev5/boneio/helper/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/ha_discovery.py` & `boneIO-0.6.0.dev5/boneio/helper/ha_discovery.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,32 +47,36 @@
     msg = ha_availabilty_message(device_type=RELAY, topic=topic, id=id, **kwargs)
     msg["command_topic"] = f"{topic}/cmd/{RELAY}/{id}/set"
     msg["payload_off"] = OFF
     msg["payload_on"] = ON
     msg["state_value_template"] = "{{ value_json.state }}"
     return msg
 
+
 def ha_led_availabilty_message(id: str, topic: str = "boneIO", **kwargs):
     """Create LED availability topic for HA."""
     msg = ha_availabilty_message(device_type=RELAY, topic=topic, id=id, **kwargs)
     msg["command_topic"] = f"{topic}/cmd/{RELAY}/{id}/set"
     msg["brightness_state_topic"] = f"{topic}/{RELAY}/{id}"
     msg["brightness_command_topic"] = f"{topic}/cmd/{RELAY}/{id}/set_brightness"
     msg["brightness_scale"] = 65535
     msg["payload_off"] = OFF
     msg["payload_on"] = ON
     msg["state_value_template"] = "{{ value_json.state }}"
     msg["brightness_value_template"] = "{{ value_json.brightness }}"
     return msg
 
-def ha_button_availabilty_message(id: str, topic: str = "boneIO", **kwargs):
+
+def ha_button_availabilty_message(
+    id: str, topic: str = "boneIO", payload_press: str = "reload", **kwargs
+):
     """Create BUTTON availability topic for HA."""
     msg = ha_availabilty_message(device_type="button", topic=topic, id=id, **kwargs)
     msg["command_topic"] = f"{topic}/cmd/button/{id}/set"
-    msg["payload_press"] = "reload"
+    msg["payload_press"] = payload_press
     return msg
 
 
 def ha_switch_availabilty_message(id: str, topic: str = "boneIO", **kwargs):
     """Create SWITCH availability topic for HA."""
     msg = ha_availabilty_message(device_type=RELAY, topic=topic, id=id, **kwargs)
     msg["command_topic"] = f"{topic}/cmd/relay/{id}/set"
@@ -98,17 +102,19 @@
 
 def ha_sensor_availabilty_message(unit_of_measurement: str = None, **kwargs):
     msg = ha_availabilty_message(device_type=SENSOR, **kwargs)
     if not unit_of_measurement:
         return msg
 
 
-def ha_binary_sensor_availabilty_message(id: str, name: str, topic: str = "boneIO"):
+def ha_binary_sensor_availabilty_message(id: str, name: str, device_class: str, topic: str = "boneIO"):
     """Create availability topic for HA."""
+    kwargs = {"device_class": device_class} if device_class else {}
     return {
+        **kwargs,
         "availability": [{"topic": f"{topic}/{STATE}"}],
         "device": {
             "identifiers": [topic],
             "manufacturer": "boneIO",
             "model": "boneIO Relay Board",
             "name": f"boneIO {topic}",
             "sw_version": __version__,
```

### Comparing `boneIO-0.6.0.dev4/boneio/helper/loader.py` & `boneIO-0.6.0.dev5/boneio/helper/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,14 +350,15 @@
             **gpio,
         )
         if gpio.get(SHOW_HA, True):
             send_ha_autodiscovery(
                 id=pin,
                 name=gpio.get(ID, pin),
                 ha_type=getattr(input, "ha_type"),
+                device_class=gpio.get(DEVICE_CLASS, None),
                 availability_msg_func=getattr(input, "availability_msg_f"),
             )
         return pin
     except GPIOInputException as err:
         _LOGGER.error("This PIN %s can't be configured. %s", pin, err)
         pass
```

### Comparing `boneIO-0.6.0.dev4/boneio/helper/logger.py` & `boneIO-0.6.0.dev5/boneio/helper/logger.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/mqtt.py` & `boneIO-0.6.0.dev5/boneio/helper/mqtt.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         """Initialize module."""
         self._id = id.replace(" ", "")
         self._name = name
         self._send_message = send_message
         self._send_topic = f"{topic_prefix}/{topic_type}/{self.id}"
 
     @property
-    def id(self) -> bool:
+    def id(self) -> str:
         """Id of the module."""
         return self._id
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Return name of the sensor."""
         return self._name
```

### Comparing `boneIO-0.6.0.dev4/boneio/helper/onewire/W1ThermSensor.py` & `boneIO-0.6.0.dev5/boneio/helper/onewire/W1ThermSensor.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/onewire/ds2482.py` & `boneIO-0.6.0.dev5/boneio/helper/onewire/ds2482.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/onewire/onewire.py` & `boneIO-0.6.0.dev5/boneio/helper/onewire/onewire.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/queue.py` & `boneIO-0.6.0.dev5/boneio/helper/queue.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/state_manager.py` & `boneIO-0.6.0.dev5/boneio/helper/state_manager.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/stats.py` & `boneIO-0.6.0.dev5/boneio/helper/stats.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/timeperiod.py` & `boneIO-0.6.0.dev5/boneio/helper/timeperiod.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/helper/yaml_util.py` & `boneIO-0.6.0.dev5/boneio/helper/yaml_util.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/input/gpio.py` & `boneIO-0.6.0.dev5/boneio/input/gpio.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             self.press_callback(click_type=SINGLE)
 
     async def _run(self) -> None:
         while True:
             self.check_state(state=self.is_pressed)
             await asyncio.sleep(self._bounce_time.total_in_seconds)
 
-    def check_state(self, state):
+    def check_state(self, state: bool) -> None:
         if state == self._state:
             return
         self._state = state
         if state:
             self._timer_long.start_timer()
             if self._timer_double.is_waiting():
                 self._timer_double.reset()
```

### Comparing `boneIO-0.6.0.dev4/boneio/manager.py` & `boneIO-0.6.0.dev5/boneio/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import logging
 from collections import deque
-from typing import Callable, Coroutine, List, Optional, Set, Union
+from typing import Callable, Coroutine, List, Optional, Set, Union, Awaitable
 from board import SCL, SDA
 from busio import I2C
 
 from boneio.const import (
     ACTION,
     ADDRESS,
     BUTTON,
@@ -76,42 +76,43 @@
 
 class Manager:
     """Manager to communicate MQTT with GPIO inputs and outputs."""
 
     def __init__(
         self,
         send_message: Callable[[str, Union[str, dict], bool], None],
+        stop_client: Callable[[], Awaitable[None]],
         state_manager: StateManager,
         config_helper: ConfigHelper,
         config_file_path: str,
         relay_pins: List = [],
         input_pins: List = [],
         sensors: dict = {},
-        modbus: dict = None,
-        pca9685: Optional[List] = None,
-        mcp23017: Optional[List] = None,
+        modbus: dict = {},
+        pca9685: list = [],
+        mcp23017: list = [],
         ds2482: Optional[List] = [],
         dallas: Optional[dict] = None,
         oled: dict = {},
-        adc_list: Optional[List] = None,
-        covers: Optional[List] = [],
+        adc: Optional[List] = None,
+        cover: list = [],
     ) -> None:
         """Initialize the manager."""
         _LOGGER.info("Initializing manager module.")
 
         self._loop = asyncio.get_event_loop()
-        used_pins = set()
+
         self._config_helper = config_helper
         self._host_data = None
         self._config_file_path = config_file_path
         self._state_manager = state_manager
         self._event_bus = EventBus(self._loop)
-        self._autodiscovery_messages = []
 
         self.send_message = send_message
+        self.stop_client = stop_client
         self._input_pins = input_pins
         self._i2cbusio = I2C(SCL, SDA)
         self._mcp = {}
         self._pca = {}
         self._output = {}
         self._oled = None
         self._tasks: List[asyncio.Task] = []
@@ -131,15 +132,15 @@
         self.grouped_outputs = create_mcp23017(
             manager=self, mcp23017=mcp23017, i2cbusio=self._i2cbusio
         )
         self.grouped_outputs.update(
             create_pca9685(manager=self, pca9685=pca9685, i2cbusio=self._i2cbusio)
         )
 
-        self._configure_adc(adc_list=adc_list)
+        self._configure_adc(adc_list=adc)
 
         for _config in relay_pins:
             _id = _config[ID].replace(" ", "")
             out = configure_relay(
                 manager=self,
                 state_manager=self._state_manager,
                 topic_prefix=self._config_helper.topic_prefix,
@@ -162,15 +163,15 @@
                     )
             self._loop.call_soon_threadsafe(
                 self._loop.call_later,
                 0.5,
                 out.send_state,
             )
 
-        for _config in covers:
+        for _config in cover:
             _id = _config[ID].replace(" ", "")
             open_relay = self._output.get(_config.get("open_relay"))
             close_relay = self._output.get(_config.get("close_relay"))
             if not open_relay:
                 _LOGGER.error(
                     "Can't configure cover %s. This relay doesn't exist.",
                     _config.get("open_relay"),
@@ -200,32 +201,20 @@
                 close_time=_config.get("close_time"),
                 event_bus=self._event_bus,
                 send_ha_autodiscovery=self.send_ha_autodiscovery,
                 topic_prefix=self._config_helper.topic_prefix,
             )
 
         _LOGGER.info("Initializing inputs. This will take a while.")
-        for gpio in self._input_pins:
-            pin = gpio.pop(PIN)
-            if pin in used_pins:
-                _LOGGER.warn("This PIN %s is already configured. Omitting it.", pin)
-                continue
-            used_pins.add(
-                configure_input(
-                    gpio=gpio,
-                    pin=pin,
-                    press_callback=self.press_callback,
-                    send_ha_autodiscovery=self.send_ha_autodiscovery,
-                )
-            )
+        self.configure_inputs(reload_config=False)
 
         if oled.get("enabled", False):
             from boneio.oled import Oled
 
-            screens = oled.get("screens")
+            screens = oled.get("screens", [])
 
             self._host_data = HostData(
                 manager=self,
                 enabled_screens=screens,
                 output=self.grouped_outputs,
                 temp_sensor=self._temp_sensors[0] if self._temp_sensors else None,
                 callback=self._host_data_callback,
@@ -236,17 +225,34 @@
                     screen_order=screens,
                     output_groups=list(self.grouped_outputs),
                     sleep_timeout=oled.get("screensaver_timeout", 60),
                 )
             except (GPIOInputException, I2CError) as err:
                 _LOGGER.error("Can't configure OLED display. %s", err)
         self.prepare_ha_buttons()
-
         _LOGGER.info("BoneIO manager is ready.")
 
+    def configure_inputs(self, reload_config: bool = False):
+        used_pins = set()
+        if reload_config:
+            load_config_from_file(self._config_file_path)
+        for gpio in self._input_pins:
+            pin = gpio.pop(PIN)
+            if pin in used_pins:
+                _LOGGER.warn("This PIN %s is already configured. Omitting it.", pin)
+                continue
+            used_pins.add(
+                configure_input(
+                    gpio=gpio,
+                    pin=pin,
+                    press_callback=self.press_callback,
+                    send_ha_autodiscovery=self.send_ha_autodiscovery,
+                )
+            )
+
     def append_task(self, coro: Coroutine, name: str = "Unknown") -> asyncio.Future:
         """Add task to run with asyncio loop."""
         _LOGGER.debug("Appending update task for %s", name)
         task: asyncio.Future = asyncio.create_task(coro())
         self._tasks.append(task)
         return task
 
@@ -333,28 +339,30 @@
             create_adc(
                 manager=self,
                 topic_prefix=self._config_helper.topic_prefix,
                 adc_list=adc_list,
             )
 
     def _configure_modbus(self, modbus: dict) -> None:
-        if modbus and modbus.get(UART) in UARTS:
+        uart = modbus.get(UART)
+        if uart and uart in UARTS:
             try:
-                self._modbus = Modbus(UARTS[modbus.get(UART)])
+                self._modbus = Modbus(UARTS[uart])
             except ModbusUartException:
                 _LOGGER.error(
                     "This UART %s can't be used for modbus communication.",
-                    modbus.get(UART),
+                    uart,
                 )
                 self._modbus = None
 
     def _configure_temp_sensors(self, sensors: dict) -> None:
         for sensor_type in (LM75, MCP_TEMP_9808):
-            if sensors.get(sensor_type):
-                for temp_def in sensors.get(sensor_type):
+            sensor = sensors.get(sensor_type)
+            if sensor:
+                for temp_def in sensor:
                     temp_sensor = create_temp_sensor(
                         manager=self,
                         topic_prefix=self._config_helper.topic_prefix,
                         sensor_type=sensor_type,
                         config=temp_def,
                         i2cbusio=self._i2cbusio,
                     )
@@ -405,18 +413,27 @@
     def get_tasks(self) -> Set[asyncio.Task]:
         """Retrieve asyncio tasks to run."""
         return self._tasks
 
     def prepare_ha_buttons(self) -> None:
         """Prepare HA buttons for reload."""
         self.send_ha_autodiscovery(
-            id="Logger",
+            id="logger",
             name="Logger reload",
             ha_type=BUTTON,
             availability_msg_func=ha_button_availabilty_message,
+            entity_category="config",
+        )
+        self.send_ha_autodiscovery(
+            id="restart",
+            name="Restart boneIO",
+            ha_type=BUTTON,
+            payload_press="restart",
+            availability_msg_func=ha_button_availabilty_message,
+            entity_category="config",
         )
 
     @property
     def mcp(self):
         """Get MCP by it's id."""
         return self._mcp
 
@@ -427,15 +444,15 @@
 
     def press_callback(
         self, x: ClickTypes, inpin: str, actions: List, input_type: InputTypes = INPUT
     ) -> None:
         """Press callback to use in input gpio.
         If relay input map is provided also toggle action on relay or cover or mqtt."""
         topic = f"{self._config_helper.topic_prefix}/{input_type}/{inpin}"
-        self.send_message(topic=topic, payload=x)
+        self.send_message(topic=topic, payload=x, retain=False)
         for action_definition in actions:
             _LOGGER.debug("Executing action %s", action_definition)
             if action_definition[ACTION] == OUTPUT:
                 device = action_definition.get(PIN)
                 if not device:
                     continue
                 relay = self._output.get(device.replace(" ", ""))
@@ -476,21 +493,22 @@
         """Send HA autodiscovery information for each relay."""
         if not self._config_helper.ha_discovery:
             return
         topic_prefix = topic_prefix or self._config_helper.topic_prefix
         payload = availability_msg_func(topic=topic_prefix, id=id, name=name, **kwargs)
         topic = f"{self._config_helper.ha_discovery_prefix}/{ha_type}/{topic_prefix}/{id}/config"
         _LOGGER.debug("Sending HA discovery for %s, %s.", ha_type, name)
-        self._config_helper.add_autodiscovery_msg(topic=topic, payload=payload)
+        self._config_helper.add_autodiscovery_msg(topic=topic, ha_type=ha_type, payload=payload)
         self.send_message(topic=topic, payload=payload, retain=True)
 
     def resend_autodiscovery(self) -> None:
         for msg in self._config_helper.autodiscovery_msgs:
             self.send_message(**msg, retain=True)
 
+
     async def receive_message(self, topic: str, message: str) -> None:
         """Callback for receiving action from Mqtt."""
         _LOGGER.debug("Processing topic %s with message %s.", topic, message)
         if topic.startswith(f"{self._config_helper.ha_discovery_prefix}/status"):
             if message == ONLINE:
                 self.resend_autodiscovery()
                 self._event_bus.signal_ha_online()
@@ -554,12 +572,15 @@
                     _LOGGER.warn(
                         "Positon cannot be set. Not number between 0-100. %s", message
                     )
         elif msg_type == BUTTON and command == "set":
             if device_id == "logger" and message == "reload":
                 _LOGGER.info("Reloading logger configuration.")
                 self._logger_reload()
+            elif device_id == "restart" and message == "restart":
+                _LOGGER.info("Exiting process. Systemd should restart it soon.")
+                await self.stop_client()
 
     @property
     def output(self) -> dict:
         """Get list of output."""
         return self._output
```

### Comparing `boneIO-0.6.0.dev4/boneio/modbus.py` & `boneIO-0.6.0.dev5/boneio/modbus.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/mqtt_client.py` & `boneIO-0.6.0.dev5/boneio/mqtt_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """
 Provide an MQTT client for providing BoneIO MQTT broker.
 Code based on cgarwood/python-openzwave-mqtt.
 """
+from __future__ import annotations
 import asyncio
 import json
 import logging
 import uuid
 from contextlib import AsyncExitStack
-from typing import Any, Callable, Optional, Set, Tuple, Union
+from typing import Any, Callable, Optional, Set, Union, Awaitable
 
 import paho.mqtt.client as mqtt
 from asyncio_mqtt import Client as AsyncioClient
 from asyncio_mqtt import MqttError, Will
 from paho.mqtt.properties import Properties
 from paho.mqtt.subscribeoptions import SubscribeOptions
 
 from boneio.const import ONLINE, PAHO, STATE
 from boneio.helper import UniqueQueue
 from boneio.helper.config import ConfigHelper
+from boneio.manager import Manager
+from boneio.helper.exceptions import RestartRequestException
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class MQTTClient:
     """Represent an MQTT client."""
 
@@ -41,14 +44,16 @@
         client_options["clean_session"] = True
         self.client_options = client_options
         self.asyncio_client: AsyncioClient = None
         self.create_client()
         self.reconnect_interval = 1
         self._connection_established = False
         self.publish_queue: UniqueQueue = UniqueQueue()
+        self._discovery_topics = [f"{self._config_helper.ha_discovery_prefix}/{ha_type}/{self._config_helper.topic_prefix}/#" for ha_type in self._config_helper.ha_types] if self._config_helper.ha_discovery else []
+        self._topics = [self._config_helper.subscribe_topic, "homeassistant/status"]
 
     def create_client(self) -> None:
         """Create the asyncio client."""
         _LOGGER.debug("Creating client %s:%s", self.host, self.port)
         self.asyncio_client = AsyncioClient(
             self.host,
             self.port,
@@ -81,15 +86,15 @@
             params["properties"] = properties
 
         _LOGGER.debug("Sending message topic: %s, payload: %s", topic, payload)
         await self.asyncio_client.publish(topic, **params)
 
     async def subscribe(  # pylint:disable=too-many-arguments
         self,
-        topics: Tuple[str, str],
+        topics: list[str],
         qos: int = 0,
         options: Optional[SubscribeOptions] = None,
         properties: Optional[Properties] = None,
         timeout: float = 10.0,
     ) -> None:
         """Subscribe to topic.
 
@@ -104,28 +109,31 @@
         if properties:
             params["properties"] = properties
 
         # e.g. subscribe([("my/topic", SubscribeOptions(qos=0), ("another/topic", SubscribeOptions(qos=2)])
         await self.asyncio_client.subscribe(topic=args, **params, timeout=timeout)
 
     async def unsubscribe(
-        self, topic: str, properties: Optional[Properties] = None, timeout: float = 10.0
+        self,
+        topics: list[str],
+        properties: Optional[Properties] = None,
+        timeout: float = 10.0,
     ) -> None:
         """Unsubscribe from topic.
 
         Can raise asyncio_mqtt.MqttError.
         """
         params: dict = {"timeout": timeout}
         if properties:
             params["properties"] = properties
 
-        await self.asyncio_client.unsubscribe(topic, **params)
+        await self.asyncio_client.unsubscribe(topic=topics, **params)
 
     def send_message(
-        self, topic: str, payload: Union[str, dict], retain: bool = False
+        self, topic: str, payload: Union[str, dict, None], retain: bool = False
     ) -> None:
         """Send a message from the manager options."""
         to_publish = (
             topic,
             json.dumps(payload) if type(payload) == dict else payload,
             retain,
         )
@@ -134,15 +142,15 @@
     async def _handle_publish(self) -> None:
         """Publish messages as they are put on the queue."""
         while True:
             to_publish: tuple = await self.publish_queue.get()
             await self.publish(*to_publish)
             self.publish_queue.task_done()
 
-    async def start_client(self, manager: any) -> None:
+    async def start_client(self, manager: Manager) -> None:
         """Start the client with the manager."""
         # Reconnect automatically until the client is stopped.
         while True:
             try:
                 await self._subscribe_manager(manager)
             except MqttError as err:
                 self.reconnect_interval = min(self.reconnect_interval * 2, 900)
@@ -151,48 +159,66 @@
                     err,
                     self.reconnect_interval,
                 )
                 self._connection_established = False
                 await asyncio.sleep(self.reconnect_interval)
                 self.create_client()  # reset connect/reconnect futures
 
-    async def _subscribe_manager(self, manager: any) -> None:
+    async def stop_client(self) -> None:
+        await self.unsubscribe(
+            topics=self._topics
+        )
+        raise RestartRequestException("Restart requested.")
+
+    async def _subscribe_manager(self, manager: Manager) -> None:
         """Connect and subscribe to manager topics + host stats."""
         async with AsyncExitStack() as stack:
             tasks: Set[asyncio.Task] = set()
 
             # Connect to the MQTT broker.
             await stack.enter_async_context(self.asyncio_client)
             # Reset the reconnect interval after successful connection.
             self.reconnect_interval = 1
 
             publish_task = asyncio.create_task(self._handle_publish())
             tasks.add(publish_task)
 
             # Messages that doesn't match a filter will get logged and handled here.
             messages = await stack.enter_async_context(
-                self.asyncio_client.unfiltered_messages()
+                self.asyncio_client.messages()
             )
 
             messages_task = asyncio.create_task(
-                handle_messages(messages, manager.receive_message)
+                self.handle_messages(messages, manager.receive_message)
             )
             if not self._connection_established:
                 self._connection_established = True
                 reconnect_task = asyncio.create_task(manager.reconnect_callback())
                 tasks.add(reconnect_task)
             tasks.add(messages_task)
 
             await self.subscribe(
-                topics=(self._config_helper.subscribe_topic, "homeassistant/status")
+                topics=self._topics
+            )
+            await self.subscribe(
+                topics=self._discovery_topics
             )
 
             # Wait for everything to complete (or fail due to, e.g., network errors).
             await asyncio.gather(*tasks)
 
-
-async def handle_messages(messages: Any, callback: Callable[[str, str], None]) -> None:
-    """Handle messages with callback."""
-    async for message in messages:
-        payload = message.payload.decode()
-        _LOGGER.debug("Received message topic: %s, payload: %s", message.topic, payload)
-        await callback(message.topic, payload)
+    async def handle_messages(self, messages: Any, callback: Callable[[str, str], Awaitable[None]]):
+        """Handle messages with callback or remove osbolete HA discovery messages."""
+        async for message in messages:
+            payload = message.payload.decode()
+            callback_start = True
+            for discovery_topic in self._discovery_topics:
+                if message.topic.matches(discovery_topic):
+                    callback_start = False
+                    topic = str(message.topic)
+                    if message.payload and not self._config_helper.is_topic_in_autodiscovery(topic):
+                        _LOGGER.info("Removing unused discovery entity %s", topic)
+                        self.send_message(topic=topic, payload=None, retain=True)
+                    break
+            if callback_start:
+                _LOGGER.debug("Received message topic: %s, payload: %s", message.topic, payload)
+                await callback(str(message.topic), payload)
```

### Comparing `boneIO-0.6.0.dev4/boneio/oled.py` & `boneIO-0.6.0.dev5/boneio/oled.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/relay/basic.py` & `boneIO-0.6.0.dev5/boneio/relay/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,37 +45,36 @@
 
     @property
     def is_light(self) -> bool:
         """Check if HA type is light"""
         return self._output_type == LIGHT
 
     @property
-    def id(self) -> bool:
+    def id(self) -> str:
         """Id of the relay.
         Has to be trimmed out of spaces because of MQTT handling in HA."""
         return self._id or self._pin
 
     @property
-    def name(self) -> bool:
+    def name(self) -> str:
         """Not trimmed id."""
         return self._name or self._pin
 
     @property
     def state(self) -> bool:
         """Is relay active."""
         return self._state
 
     def send_state(self) -> None:
         """Send state to Mqtt on action."""
         state = ON if self.is_active else OFF
         self._state = state
         if self.output_type != NONE:
             self._send_message(
-                topic=self._send_topic,
-                payload={STATE: state},
+                topic=self._send_topic, payload={STATE: state}, retain=True
             )
         self._loop.call_soon_threadsafe(self._callback)
 
     def toggle(self) -> None:
         """Toggle relay."""
         _LOGGER.debug("Toggle relay.")
         if self.is_active:
```

### Comparing `boneIO-0.6.0.dev4/boneio/relay/gpio.py` & `boneIO-0.6.0.dev5/boneio/relay/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/relay/mcp.py` & `boneIO-0.6.0.dev5/boneio/relay/mcp.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/relay/pca.py` & `boneIO-0.6.0.dev5/boneio/relay/pca.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/runner.py` & `boneIO-0.6.0.dev5/boneio/runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Runner code for boneIO. Based on HA runner."""
+from __future__ import annotations
 import asyncio
 import logging
 import os
+from typing import Any
 
 from boneio.const import (
     ADC,
     COVER,
     DALLAS,
     DS2482,
     ENABLED,
@@ -30,21 +32,32 @@
 from boneio.helper import StateManager
 from boneio.helper.config import ConfigHelper
 from boneio.manager import Manager
 from boneio.mqtt_client import MQTTClient
 
 _LOGGER = logging.getLogger(__name__)
 
+config_modules = [
+    {"name": MCP23017, "default": []},
+    {"name": PCA9685, "default": []},
+    {"name": DS2482, "default": []},
+    {"name": ADC, "default": []},
+    {"name": COVER, "default": []},
+    {"name": MODBUS, "default": {}},
+    {"name": OLED, "default": {}},
+    {"name": DALLAS, "default": None},
+]
+
 
 async def async_run(
     config: dict,
     config_file: str,
     mqttusername: str = "",
     mqttpassword: str = "",
-):
+) -> list[Any]:
     """Run BoneIO."""
 
     _config_helper = ConfigHelper(
         topic_prefix=config[MQTT].pop(TOPIC_PREFIX),
         ha_discovery=config[MQTT][HA_DISCOVERY].pop(ENABLED),
         ha_discovery_prefix=config[MQTT][HA_DISCOVERY].pop(TOPIC_PREFIX),
     )
@@ -52,37 +65,35 @@
     client = MQTTClient(
         host=config[MQTT][HOST],
         username=config[MQTT].get(USERNAME, mqttusername),
         password=config[MQTT].get(PASSWORD, mqttpassword),
         port=config[MQTT].get(PORT, 1883),
         config_helper=_config_helper,
     )
+    manager_kwargs = {
+        item["name"]: config.get(item["name"], item["default"])
+        for item in config_modules
+    }
 
     manager = Manager(
         send_message=client.send_message,
+        stop_client=client.stop_client,
         relay_pins=config.get(OUTPUT, []),
         input_pins=config.get(INPUT, []),
         config_file_path=config_file,
         state_manager=StateManager(
             state_file=f"{os.path.split(config_file)[0]}state.json"
         ),
         config_helper=_config_helper,
         sensors={
             LM75: config.get(LM75, []),
             MCP_TEMP_9808: config.get(MCP_TEMP_9808, []),
             MODBUS: config.get("modbus_sensors"),
             ONEWIRE: config.get(SENSOR, []),
         },
-        mcp23017=config.get(MCP23017, []),
-        pca9685=config.get(PCA9685, []),
-        ds2482=config.get(DS2482, []),
-        dallas=config.get(DALLAS),
-        modbus=config.get(MODBUS),
-        oled=config.get(OLED),
-        adc_list=config.get(ADC, []),
-        covers=config.get(COVER, []),
+        **manager_kwargs,
     )
     tasks = set()
     tasks.update(manager.get_tasks())
     _LOGGER.info("Connecting to MQTT.")
     tasks.add(client.start_client(manager))
     return await asyncio.gather(*tasks)
```

### Comparing `boneIO-0.6.0.dev4/boneio/schema/actions.yaml` & `boneIO-0.6.0.dev5/boneio/schema/actions.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/schema/schema.yaml` & `boneIO-0.6.0.dev5/boneio/schema/schema.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -372,14 +372,20 @@
           label: Either switch or sensor. If sensor then no clicks are detected, just simple on/off on gpio.
       inverted:
         type: boolean
         default: False
         required: True
         meta:
           label: Check if sensor type is inverted. Only aplicable for sensor kind.
+      device_class:
+        type: string
+        required: False
+        allowed: ["battery", "battery_charging", "carbon_monoxide", "cold", "connectivity", "door", "garage_door", "gas", "heat", "light", "lock", "moisture", "motion", "moving", "occupancy", "opening", "plug", "power", "presence", "problem", "running", "safety", "smoke", "sound", "tamper", "vibration", "window"]
+        meta:
+          label: Device class to use in HA
       actions:
         required: False
         type: dict
         coerce: check_actions
         schema:
           single: !include actions_switch.yaml
           double: !include actions_switch.yaml
```

### Comparing `boneIO-0.6.0.dev4/boneio/sensor/adc.py` & `boneIO-0.6.0.dev5/boneio/sensor/adc.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/sensor/modbus/__init__.py` & `boneIO-0.6.0.dev5/boneio/sensor/modbus/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/sensor/modbus/dts1964_3f.json` & `boneIO-0.6.0.dev5/boneio/sensor/modbus/dts1964_3f.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/sensor/modbus/pt100.json` & `boneIO-0.6.0.dev5/boneio/sensor/modbus/pt100.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/sensor/modbus/r4dcb08.json` & `boneIO-0.6.0.dev5/boneio/sensor/modbus/r4dcb08.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/sensor/modbus/sdm120.json` & `boneIO-0.6.0.dev5/boneio/sensor/modbus/sdm120.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/sensor/modbus/sdm630.json` & `boneIO-0.6.0.dev5/boneio/sensor/modbus/sdm630.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/sensor/modbus/sofar.json` & `boneIO-0.6.0.dev5/boneio/sensor/modbus/sofar.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/sensor/temp/__init__.py` & `boneIO-0.6.0.dev5/boneio/sensor/temp/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/boneio/sensor/temp/dallas.py` & `boneIO-0.6.0.dev5/boneio/sensor/temp/dallas.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/pyproject.toml` & `boneIO-0.6.0.dev5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 description = "Python App for BoneIO"
 readme = "README.md"
 dynamic = []
 authors = [
     { name = "Paweł Szafer", email = "pszafer@gmail.com" },
 ]
 dependencies = [
-    "Adafruit-Blinka>=8.0.2",
-    "adafruit-circuitpython-ds18x20>=1.3.12",
-    "adafruit-circuitpython-mcp230xx>=2.5.5",
-    "adafruit-circuitpython-mcp9808>=3.3.14",
-    "adafruit-circuitpython-pct2075>=1.1.14",
-    "asyncio-mqtt>=0.12.1",
+    "Adafruit-Blinka>=8.19.0",
+    "adafruit-circuitpython-ds18x20>=1.3.16",
+    "adafruit-circuitpython-mcp230xx>=2.5.9",
+    "adafruit-circuitpython-mcp9808>=3.3.19",
+    "adafruit-circuitpython-pct2075>=1.1.18",
+    "asyncio-mqtt>=0.16.1",
     "Cerberus>=1.3.4",
-    "colorlog>=6.6.0",
-    "gpio>=0.3.0",
-    "luma.core>=2.3.1",
-    "luma.oled>=3.8.1",
+    "colorlog>=6.7.0",
+    "gpio>=1.0.0",
+    "luma-core>=2.4.0",
+    "luma-oled>=3.12.0",
     "pymodbus>=2.5.3",
     "pyserial-asyncio>=0.6",
     "PyYAML>=6.0",
     "Adafruit-BBIO>=1.2.0",
-    "psutil>=5.9.1",
+    "psutil>=5.9.5",
     "adafruit-circuitpython-onewire>=2.0.4",
     "w1thermsensor[async]>=2.0.0",
-    "adafruit-circuitpython-pca9685>=3.4.6",
+    "adafruit-circuitpython-pca9685>=3.4.8",
 ]
 requires-python = ">=3.7"
-version = "0.6.0.dev4"
+version = "0.6.0.dev5"
 
 [project.license]
 text = "GNU General Public License v3.0"
 
 [project.urls]
 Homepage = "https://boneio.eu"
 Repository = "https://github.com/boneIO-eu/app_bbb"
@@ -45,20 +45,20 @@
 [project.optional-dependencies]
 
 [tool.pdm.version]
 from = "boneio/version.py"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "black>=22.6.0",
-    "isort>=5.10.1",
-    "pre-commit>=2.19.0",
-    "flake8>=4.0.1",
-    "bandit>=1.7.4",
-    "setuptools>=67.6.1",
+    "black>=23.3.0",
+    "isort>=5.11.5",
+    "pre-commit>=2.21.0",
+    "flake8>=5.0.4",
+    "bandit>=1.7.5",
+    "setuptools>=67.7.2",
 ]
 
 [tool.pdm.scripts]
 lint = "pre-commit run --all-files"
 
 [tool.black]
 line-length = 88
```

### Comparing `boneIO-0.6.0.dev4/tests/relay_32_5.py` & `boneIO-0.6.0.dev5/tests/relay_32_5.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev4/PKG-INFO` & `boneIO-0.6.0.dev5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boneIO
-Version: 0.6.0.dev4
+Version: 0.6.0.dev5
 Summary: Python App for BoneIO
 License: GNU General Public License v3.0
 Author-email: Paweł Szafer <pszafer@gmail.com>
 Requires-Python: >=3.7
 Project-URL: Changelog, https://github.com/boneIO-eu/app_bbb/releases
 Project-URL: Documentation, https://boneio.eu/docs/intro/
 Project-URL: Homepage, https://boneio.eu
```

