# Comparing `tmp/ja2mqtt-1.0.4.tar.gz` & `tmp/ja2mqtt-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ja2mqtt-1.0.4.tar", last modified: Fri May  5 20:53:35 2023, max compression
+gzip compressed data, was "dist/ja2mqtt-1.0.5.tar", last modified: Sun May  7 12:39:57 2023, max compression
```

## Comparing `ja2mqtt-1.0.4.tar` & `ja2mqtt-1.0.5.tar`

### file list

```diff
@@ -1,48 +1,34 @@
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.625080 ja2mqtt-1.0.4/
--rw-r--r--   0 tomas      (501) staff       (20)     1069 2023-05-03 21:57:45.000000 ja2mqtt-1.0.4/LICENSE
--rw-r--r--   0 tomas      (501) staff       (20)      143 2023-05-03 21:57:45.000000 ja2mqtt-1.0.4/MANIFEST.in
--rw-r--r--   0 tomas      (501) staff       (20)     2017 2023-05-05 20:53:35.624939 ja2mqtt-1.0.4/PKG-INFO
--rw-r--r--   0 tomas      (501) staff       (20)     1650 2023-05-03 21:57:45.000000 ja2mqtt-1.0.4/README-pypi.text
--rw-r--r--   0 tomas      (501) staff       (20)     4375 2023-05-05 20:48:52.000000 ja2mqtt-1.0.4/README.md
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.615368 ja2mqtt-1.0.4/bin/
--rwxr-xr-x   0 tomas      (501) staff       (20)      345 2023-05-05 18:31:56.000000 ja2mqtt-1.0.4/bin/env.sh
--rwxr-xr-x   0 tomas      (501) staff       (20)       31 2023-05-03 21:57:45.000000 ja2mqtt-1.0.4/bin/ja2mqtt
--rw-r--r--   0 tomas      (501) staff       (20)      107 2023-05-03 21:57:45.000000 ja2mqtt-1.0.4/bin/requirements-dev.txt
--rwxr-xr-x   0 tomas      (501) staff       (20)      700 2023-05-03 21:57:45.000000 ja2mqtt-1.0.4/bin/requirements-setup-py.sh
--rw-r--r--   0 tomas      (501) staff       (20)      118 2023-05-05 20:51:46.000000 ja2mqtt-1.0.4/bin/requirements.txt
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.615572 ja2mqtt-1.0.4/config/
--rw-r--r--   0 tomas      (501) staff       (20)     3956 2023-04-30 23:14:11.000000 ja2mqtt-1.0.4/config/ja2mqtt.yaml
--rw-r--r--   0 tomas      (501) staff       (20)     2024 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/config/sample-config.yaml
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.615895 ja2mqtt-1.0.4/docker/
--rw-r--r--   0 tomas      (501) staff       (20)      975 2023-04-20 19:55:01.000000 ja2mqtt-1.0.4/docker/Dockerfile
--rw-r--r--   0 tomas      (501) staff       (20)      299 2023-04-18 22:48:03.000000 ja2mqtt-1.0.4/docker/docker-compose.yaml
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.616028 ja2mqtt-1.0.4/docker/mqtt-config/
--rw-r--r--   0 tomas      (501) staff       (20)    40475 2023-04-17 22:42:29.000000 ja2mqtt-1.0.4/docker/mqtt-config/mosquitto.conf
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.616572 ja2mqtt-1.0.4/ja2mqtt/
--rwxr-xr-x   0 tomas      (501) staff       (20)      167 2023-05-05 20:49:44.000000 ja2mqtt-1.0.4/ja2mqtt/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)      251 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/__main__.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.617763 ja2mqtt-1.0.4/ja2mqtt/commands/
--rw-r--r--   0 tomas      (501) staff       (20)     2192 2023-05-04 21:44:40.000000 ja2mqtt-1.0.4/ja2mqtt/commands/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)     2301 2023-05-04 21:45:06.000000 ja2mqtt-1.0.4/ja2mqtt/commands/config.py
--rw-r--r--   0 tomas      (501) staff       (20)     1859 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/commands/ja2mqtt.py
--rw-r--r--   0 tomas      (501) staff       (20)     1208 2023-04-30 22:17:24.000000 ja2mqtt-1.0.4/ja2mqtt/commands/run.py
--rw-r--r--   0 tomas      (501) staff       (20)     2552 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/commands/test.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.624615 ja2mqtt-1.0.4/ja2mqtt/components/
--rw-r--r--   0 tomas      (501) staff       (20)      819 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/components/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)    11210 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/components/bridge.py
--rw-r--r--   0 tomas      (501) staff       (20)     5572 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/components/mqtt.py
--rw-r--r--   0 tomas      (501) staff       (20)     7854 2023-04-30 22:20:40.000000 ja2mqtt-1.0.4/ja2mqtt/components/serial.py
--rw-r--r--   0 tomas      (501) staff       (20)     6477 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/components/simulator.py
--rw-r--r--   0 tomas      (501) staff       (20)    15442 2023-05-04 21:44:24.000000 ja2mqtt-1.0.4/ja2mqtt/config.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.624745 ja2mqtt-1.0.4/ja2mqtt/schemas/
--rw-r--r--   0 tomas      (501) staff       (20)     3030 2023-04-30 22:00:50.000000 ja2mqtt-1.0.4/ja2mqtt/schemas/config-schema.yaml
--rw-r--r--   0 tomas      (501) staff       (20)     8079 2023-04-20 19:55:01.000000 ja2mqtt-1.0.4/ja2mqtt/utils.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.617251 ja2mqtt-1.0.4/ja2mqtt.egg-info/
--rw-r--r--   0 tomas      (501) staff       (20)     2017 2023-05-05 20:53:35.000000 ja2mqtt-1.0.4/ja2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 tomas      (501) staff       (20)      857 2023-05-05 20:53:35.000000 ja2mqtt-1.0.4/ja2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 tomas      (501) staff       (20)        1 2023-05-05 20:53:35.000000 ja2mqtt-1.0.4/ja2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 tomas      (501) staff       (20)       61 2023-05-05 20:53:35.000000 ja2mqtt-1.0.4/ja2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 tomas      (501) staff       (20)       89 2023-05-05 20:53:35.000000 ja2mqtt-1.0.4/ja2mqtt.egg-info/requires.txt
--rw-r--r--   0 tomas      (501) staff       (20)        8 2023-05-05 20:53:35.000000 ja2mqtt-1.0.4/ja2mqtt.egg-info/top_level.txt
--rw-r--r--   0 tomas      (501) staff       (20)       38 2023-05-05 20:53:35.625113 ja2mqtt-1.0.4/setup.cfg
--rw-r--r--   0 tomas      (501) staff       (20)     1615 2023-05-03 21:58:21.000000 ja2mqtt-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/README-pypi.text
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/commands/ja2mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/commands/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/components/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/components/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/components/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/components/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15810 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/schemas/config-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/schemas/ja2mqtt-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ja2mqtt-1.0.4/PKG-INFO` & `ja2mqtt-1.0.5/README-pypi.text`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: ja2mqtt
-Version: 1.0.4
-Summary: Jablotron MQTT bridge
-Author: Tomas Vitvar
-Author-email: tomas@vitvar.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6.0
-License-File: LICENSE
-
 ja2mqtt is a bridge that connects a Jablotron control unit, extended with the [JA-121T RS-485 bus interface](https://www.jablotron.com/en/produkt/rs-485-bus-interface-426/), to an MQTT broker.
 
 ja2mqtt enables the use of MQTT events to control Jablotron events, allowing for seamless integration with MQTT-based IoT systems and platforms. With this bridge, Jablotron alarms can be integrated into a larger IoT ecosystem, alongside other devices that use industry-standard protocols like ZigBee or MQTT. For example, by using ja2mqtt in conjunction with ZigBee2MQTT, Jablotron alarms and ZigBee devices can be connected in a single network and integrated with other systems such as Alexa, Tahoma, or Google Assistant, providing a unified and interoperable smart home or industrial automation solution.
 
 ja2mqtt reads input from the JA-121T serial interface, converts it into MQTT events, and publishes them to the MQTT broker using defined MQTT topics. It utilizes a ja2mqtt definition file that outlines the implementation of the JA-121T protocol. Additionally, ja2mqtt defines MQTT events that can be converted into input for the JA-121T serial interface, such as changing the state of a section to ARMED or READY. Each MQTT request may contain a correlation ID that is copied to the corresponding generated MQTT event.
 
 If you do not have access to a JA-121T interface for testing, ja2mqtt offers a simulator that can simulate the interaction with the JA-121T interface. This allows you to test and verify the functionality of ja2mqtt even without the physical JA-121T interface available.
```

### Comparing `ja2mqtt-1.0.4/README-pypi.text` & `ja2mqtt-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,25 @@
-ja2mqtt is a bridge that connects a Jablotron control unit, extended with the [JA-121T RS-485 bus interface](https://www.jablotron.com/en/produkt/rs-485-bus-interface-426/), to an MQTT broker.
-
-ja2mqtt enables the use of MQTT events to control Jablotron events, allowing for seamless integration with MQTT-based IoT systems and platforms. With this bridge, Jablotron alarms can be integrated into a larger IoT ecosystem, alongside other devices that use industry-standard protocols like ZigBee or MQTT. For example, by using ja2mqtt in conjunction with ZigBee2MQTT, Jablotron alarms and ZigBee devices can be connected in a single network and integrated with other systems such as Alexa, Tahoma, or Google Assistant, providing a unified and interoperable smart home or industrial automation solution.
-
-ja2mqtt reads input from the JA-121T serial interface, converts it into MQTT events, and publishes them to the MQTT broker using defined MQTT topics. It utilizes a ja2mqtt definition file that outlines the implementation of the JA-121T protocol. Additionally, ja2mqtt defines MQTT events that can be converted into input for the JA-121T serial interface, such as changing the state of a section to ARMED or READY. Each MQTT request may contain a correlation ID that is copied to the corresponding generated MQTT event.
-
-If you do not have access to a JA-121T interface for testing, ja2mqtt offers a simulator that can simulate the interaction with the JA-121T interface. This allows you to test and verify the functionality of ja2mqtt even without the physical JA-121T interface available.
-
-See https://github.com/tomvit/ja2mqtt for more details.
-
+Metadata-Version: 1.2
+Name: ja2mqtt
+Version: 1.0.5
+Summary: Jablotron MQTT bridge
+Home-page: UNKNOWN
+Author: Tomas Vitvar
+Author-email: tomas@vitvar.com
+License: UNKNOWN
+Description: ja2mqtt is a bridge that connects a Jablotron control unit, extended with the [JA-121T RS-485 bus interface](https://www.jablotron.com/en/produkt/rs-485-bus-interface-426/), to an MQTT broker.
+        
+        ja2mqtt enables the use of MQTT events to control Jablotron events, allowing for seamless integration with MQTT-based IoT systems and platforms. With this bridge, Jablotron alarms can be integrated into a larger IoT ecosystem, alongside other devices that use industry-standard protocols like ZigBee or MQTT. For example, by using ja2mqtt in conjunction with ZigBee2MQTT, Jablotron alarms and ZigBee devices can be connected in a single network and integrated with other systems such as Alexa, Tahoma, or Google Assistant, providing a unified and interoperable smart home or industrial automation solution.
+        
+        ja2mqtt reads input from the JA-121T serial interface, converts it into MQTT events, and publishes them to the MQTT broker using defined MQTT topics. It utilizes a ja2mqtt definition file that outlines the implementation of the JA-121T protocol. Additionally, ja2mqtt defines MQTT events that can be converted into input for the JA-121T serial interface, such as changing the state of a section to ARMED or READY. Each MQTT request may contain a correlation ID that is copied to the corresponding generated MQTT event.
+        
+        If you do not have access to a JA-121T interface for testing, ja2mqtt offers a simulator that can simulate the interaction with the JA-121T interface. This allows you to test and verify the functionality of ja2mqtt even without the physical JA-121T interface available.
+        
+        See https://github.com/tomvit/ja2mqtt for more details.
+        
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.6.0
```

### Comparing `ja2mqtt-1.0.4/README.md` & `ja2mqtt-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # $ ja2mqtt
 
-[![](https://img.shields.io/pypi/v/ja2mqtt.svg)](https://pypi.org/project/ja2mqtt/)
+[![PyPI](https://img.shields.io/pypi/v/ja2mqtt?label=PyPI)](https://pypi.org/project/ja2mqtt/)
+[![Docker Image Version (tag latest semver)](https://img.shields.io/docker/v/tomvit/ja2mqtt/latest?label=Docker)](https://hub.docker.com/r/tomvit/ja2mqtt/tags)
 
 <!-- start elevator-pitch -->
 
 ja2mqtt is a bridge that connects a Jablotron control unit, extended with the [JA-121T RS-485 bus interface](https://www.jablotron.com/en/produkt/rs-485-bus-interface-426/), to an MQTT broker.
 
 <p align="center">
   <img src="https://docs.google.com/drawings/export/svg?id=1GINAM_3vBMGUWAl9Av3RNUfqQ2NBDTurdChcjQiTuOw" />
@@ -12,36 +13,34 @@
 
 ja2mqtt reads input from the JA-121T serial interface, converts it into MQTT events, and publishes them to the MQTT broker using defined MQTT topics. It utilizes a ja2mqtt definition file that outlines the implementation of the JA-121T protocol. Additionally, ja2mqtt defines MQTT events that can be converted into input for the JA-121T serial interface, such as changing the state of a section to ARMED or READY.
 
 <!-- end elevator-pitch -->
 
 If you do not have access to a JA-121T interface for testing, ja2mqtt offers a simulator that can simulate the interaction with the JA-121T interface. This allows you to test and verify the functionality of ja2mqtt even without the physical JA-121T interface available.
 
-Read the [ja2mqtt documentation](https://ja2mqtt.vitvar.com) for details on how to configure, run and use ja2mqtt.  
+Read the [ja2mqtt documentation](https://ja2mqtt.vitvar.com) for details on how to [configure](https://ja2mqtt.vitvar.com/configuration/), [install](https://ja2mqtt.vitvar.com/installation.html) and [use](https://ja2mqtt.vitvar.com/usage.html) ja2mqtt.  
 
 ## Features
 
 <!-- start features -->
 
 * **Jablotron topology** definition in the YAML configuration file, including sections and their codes, names, and peripherals' positions, types, and names.
-* **Declarative rules** that define how JA-121T serial bus protocol is implemented.
-* Reading events from Jablotron, such as section arming and disarming, peripheral state changes, and converting them to **MQTT events**.
+* **Jablotron events published as MQTT events**, such as section arming and disarming or peripheral state changes.
 * MQTT topics that clients can use to **control sections** and **retrieve section and peripheral states**.
+* **Declarative rules** that define how JA-121T serial bus protocol is implemented.
 * **Automated recovery** of serial interface and MQTT broker connection failures.
 * **JA-121T simulator** to simulate section state changes, peripheral state changes, and heartbeat messages.
 
 <!-- end features -->
 
 ## Quickstart
 
 <!-- start quickstart -->
 
-ja2mqtt requires JA-121T bus interface, however, you can test it using the simulator if you do not have one. The Docker image comes with a sample configuration that uses the simulator. The simulator provides a straightforward Jablotron topology with two sections: `House` with code `1` and an initial state of `ARMED`, and `Garage` with code `2` and an initial state of `READY`. This topology can be used to simulate changing the state or retrieving the status of the sections. The simulator also mimics peripheral state changes and Jablotron heartbeat messages by generating "OK" messages every 10 seconds.
-
-In addition, ja2mqtt requires a running instance of [MQTT broker](https://mqtt.org/). The below steps use the [Eclipse Mosquitto MQTT broker](https://mosquitto.org/) with a sample configuration. To test ja2mqtt, follow the steps below.
+ja2mqtt requires JA-121T bus interface, however, you can test it using the simulator if you do not have one. The Docker image comes with a sample configuration that uses the simulator. ja2mqtt also requires a running instance of [MQTT broker](https://mqtt.org/). The below steps use the [Eclipse Mosquitto MQTT broker](https://mosquitto.org/) with a sample configuration. For complete installation instructions, please refer to the [installation guide](https://ja2mqtt.vitvar.com/installation.html).
 
 1. In your working directory, create a sub-directory `mqtt-config` and add the [`mosquitto.conf`](https://github.com/tomvit/ja2mqtt/tree/master/docker/mqtt-config/mosquitto.conf) into it.
 
 1. Add a [`docker-compose.yaml`](https://github.com/tomvit/ja2mqtt/tree/master/docker/docker-compose.yaml) with the following content.
 
    ```yaml
    version: '3.0'
@@ -66,19 +65,24 @@
 
 2. Inspect the logs of ja2mqtt by running the following command:
 
    ```
    $ docker logs ja2mqtt
    ```
 
-3. Publish the MQTT event to retrieve the state of sections as follows:
+3. The simulator provides a straightforward Jablotron topology with two sections: `House` with code `1` and an initial state of `ARMED`, and `Garage` with code `2` and an initial state of `READY`. This topology can be used to simulate changing the state or retrieving the status of the sections. The simulator also mimics peripheral state changes and Jablotron heartbeat messages by generating "OK" messages every 10 seconds.
+
+   You can use the below example to publish the MQTT event to retrieve the state of sections:
 
    ```
    $ docker exec -it ja2mqtt pub -t ja2mqtt/section/get -d pin=1234
    <-- send: ja2mqtt/section/get: {"pin": "1234", "corrid": "ca8438b82f16"}
    --> recv: ja2mqtt/section/house: {"corrid": "ca8438b82f16", "section_code": 1, "section_name": "house", "state": "ARMED"}
    --> recv: ja2mqtt/section/garage: {"corrid": "ca8438b82f16", "section_code": 2, "section_name": "garage", "state": "READY"}   
    ```
 
-4. Check the log entries in the ja2mqtt log again to see if the events were generated.
+   Please refer to the [usage guide](https://ja2mqtt.vitvar.com/usage.html) for more details on how to use ja2mqtt to query and control Jablotron sections and perihperals.
+
+
+4. Check the log entries in the ja2mqtt log to see the events were generated.
 
 <!-- end quickstart -->
```

### Comparing `ja2mqtt-1.0.4/ja2mqtt/commands/__init__.py` & `ja2mqtt-1.0.5/ja2mqtt/commands/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,10 +67,11 @@
         init_logging(
             config.get_dir_path(config.root("logs")),
             "run",
             log_level="DEBUG" if ja2mqtt_config.DEBUG else "INFO",
             handlers=["file"],
         )
 
+
 class BaseCommandLogOnlyNoValidate(BaseCommandLogOnly):
     def validate_config(self, config):
         pass
```

### Comparing `ja2mqtt-1.0.4/ja2mqtt/commands/config.py` & `ja2mqtt-1.0.5/ja2mqtt/commands/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,18 @@
 
 @click.command(
     "ja2mqtt", help="Show the ja2mqtt definition configuration.", cls=BaseCommandLogOnly
 )
 def config_ja2mqtt(config, log):
     ja2mqtt_file = config.get_dir_path(config.root("ja2mqtt"))
     scope = Map(topology=config.root("topology"))
-    ja2mqtt = Config(ja2mqtt_file, scope=scope, use_template=True)
+    ja2mqtt = Config(
+        ja2mqtt_file, scope=scope, use_template=True, schema="ja2mqtt-schema.yaml"
+    )
+    ja2mqtt.validate(throw_ex=True)
     print(json.dumps(ja2mqtt.root._config, indent=4, default=str))
 
 
 @click.command("env", help="Show environment varialbes.")
 def config_env():
     print("List of environment variables used by ja2mqtt:")
     print("")
@@ -52,22 +55,42 @@
     print("Publishing:")
     for t in ja2mqtt("serial2mqtt"):
         print(f"- {t['name']}")
     print("Subscribing:")
     for t in ja2mqtt("mqtt2serial"):
         print(f"- {t['name']}")
 
-@click.command("validate", help="Validate configuration.", cls=BaseCommandLogOnlyNoValidate)
+
+@click.command(
+    "validate", help="Validate configuration.", cls=BaseCommandLogOnlyNoValidate
+)
 def config_validate(config, log):
+    def _display_validation(res, errors, file):
+        if not res:
+            if errors is not None:
+                click.echo(f"Validation of {file} failed with the following errors:")
+                for e in errors:
+                    print(f"- {e.message}, in {e.json_path[2:]}")
+            else:
+                click.echo(f"Validation of {file} failed.")
+        else:
+            click.echo(f"The configuration file {file} is valid.")
+
     res, errors = config.validate(throw_ex=False)
-    if not res:
-        click.echo("Validation failed with the following errors:")
-        for e in errors:
-            print(f"- {e.message}, in {e.json_path[2:]}")
-    else:
-        print("The configuration is valid.")
+    _display_validation(res, errors, config.config_file)
+    try:
+        ja2mqtt_file = config.get_dir_path(config.root("ja2mqtt"))
+        scope = Map(topology=config.root("topology"))
+        ja2mqtt = Config(
+            ja2mqtt_file, scope=scope, use_template=True, schema="ja2mqtt-schema.yaml"
+        )
+        res, errors = ja2mqtt.validate(throw_ex=False)
+        _display_validation(res, errors, ja2mqtt_file)
+    except:
+        _display_validation(False, None, None)
+
 
 command_config.add_command(config_main)
 command_config.add_command(config_ja2mqtt)
 command_config.add_command(config_env)
 command_config.add_command(config_topics)
 command_config.add_command(config_validate)
```

### Comparing `ja2mqtt-1.0.4/ja2mqtt/commands/ja2mqtt.py` & `ja2mqtt-1.0.5/ja2mqtt/commands/ja2mqtt.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.4/ja2mqtt/commands/run.py` & `ja2mqtt-1.0.5/ja2mqtt/commands/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 def command_run(config, log):
     bridge = SerialMQTTBridge(config)
 
     simulator = None
     if config("simulator") is not None:
         simulator = Simulator(config.get_part("simulator"), bridge.prfstate_bits)
     elif config("serial.use_simulator", False):
-        log.error("The serial interface is be simulated but the simulator configuration does not exist!")
+        log.error(
+            "The serial interface is be simulated but the simulator configuration does not exist!"
+        )
 
     serial = Serial(config.get_part("serial"), simulator)
     mqtt = MQTT(f"ja2mqtt-client+{randomString(10)}", config.get_part("mqtt-broker"))
 
     bridge.set_mqtt(mqtt)
     bridge.set_serial(serial)
```

### Comparing `ja2mqtt-1.0.4/ja2mqtt/commands/test.py` & `ja2mqtt-1.0.5/ja2mqtt/commands/test.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.4/ja2mqtt/components/__init__.py` & `ja2mqtt-1.0.5/ja2mqtt/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.4/ja2mqtt/components/bridge.py` & `ja2mqtt-1.0.5/ja2mqtt/components/bridge.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.4/ja2mqtt/components/mqtt.py` & `ja2mqtt-1.0.5/ja2mqtt/components/mqtt.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,14 +29,24 @@
         super().__init__(config, "mqtt")
         self.client_name = name
         self.address = self.config.value_str("address")
         self.port = self.config.value_int("port", default=1883)
         self.keepalive = self.config.value_int("keepalive", default=60)
         self.reconnect_after = self.config.value_int("reconnect_after", default=30)
         self.loop_timeout = self.config.value_int("loop_timeout", default=1)
+        self.username = self.config.value_str("username", default=None)
+        self.password = self.config.value_str("password", default=None)
+        self.protocol = {
+            "MQTTv311": mqtt.MQTTv311,
+            "MQTTv31": mqtt.MQTTv31,
+            "MQTTv5": mqtt.MQTTv5,
+            "default": None,
+        }[self.config.value_str("protocol", default="MQTTv311")]
+        self.transport = self.config.value_str("transport", default="tcp")
+        self.clean_session = self.config.value_str("clean_session", default=None)
         self.client = None
         self.connected = False
         self.on_connect_ext = None
         self.on_message_ext = None
         self.on_error_ext = None
         self.log.info(f"The MQTT client configured for {self.address}.")
         self.log.debug(f"The MQTT object is {self}.")
@@ -78,15 +88,27 @@
             self.connected = False
             if rc != 0:
                 raise Exception("The client was disconnected unexpectedly.")
         except Exception as e:
             self.on_error(e)
 
     def init_client(self):
-        self.client = mqtt.Client(self.client_name)
+        self.client = mqtt.Client(
+            self.client_name,
+            clean_session=self.clean_session,
+            protocol=self.protocol,
+            transport=self.transport,
+        )
+        if self.username is not None:
+            self.log.debug(
+                f"Using '{self.username}/*******' to authenticate with the MQTT broker."
+            )
+            if self.password is None:
+                self.log.warning("The password was not specified!")
+            self.client.username_pw_set(username=self.username, password=self.password)
         self.client.on_connect = self.on_connect
         self.client.on_disconnect = self.on_disconnect
 
     def subscribe(self, topic):
         self.log.info(f"Subscribing to {topic}")
         self.client.subscribe(topic)
```

### Comparing `ja2mqtt-1.0.4/ja2mqtt/components/serial.py` & `ja2mqtt-1.0.5/ja2mqtt/components/serial.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
             self.log.info(f"The serial connection configured, the port is {self.port}")
         else:
             self.port = "<simulator>"
             self.ser = simulator
             self.log.info("The serial interface events will be simulated.")
             self.log.debug(f"The simulator object is {self.ser}")
 
-
     def create_serial(self):
         """
         Create serial object and initialize the parameters from the configuration.
         """
         self.ser = py_serial.serial_for_url(self.port, do_not_open=True)
         self.ser.baudrate = self.config.value_int("baudrate", min=0, default=9600)
         self.ser.bytesize = self.config.value_int("bytesize", min=7, max=8, default=8)
```

### Comparing `ja2mqtt-1.0.4/ja2mqtt/components/simulator.py` & `ja2mqtt-1.0.5/ja2mqtt/components/simulator.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.4/ja2mqtt/config.py` & `ja2mqtt-1.0.5/ja2mqtt/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -210,14 +210,15 @@
         return PythonExpression(replace_env_variable(node.value))
     except Exception as e:
         raise Exception(
             'Cannot create python expression from string "%s". %s'
             % (node.value, str(e))
         )
 
+
 class Config:
     """
     The main confuguration.
     """
 
     def __init__(
         self,
@@ -241,52 +242,61 @@
         self.root = self.get_part(None)
         if schema:
             self.schema = read_config(
                 get_schema_file(schema), None, use_template=False
             )[0]
 
     def check_dupplicates(self, path):
-        _path = path.split('.')
+        _path = path.split(".")
         _prop = _path[-1]
-        values = [x[_prop] for x in self('.'.join(_path[:-1]),[],required=False)]
+        values = [x[_prop] for x in self(".".join(_path[:-1]), [], required=False)]
         dupplicates = list(set([x for x in values if values.count(x) > 1]))
         if len(dupplicates) > 0:
             raise Exception(f"There are dupplicate values in '{path}': {dupplicates}")
 
     def validate(self, throw_ex=True):
         def __version(c, i):
             return i in SCHEMA_VERSIONS
 
-        def __time_condition(c, i):
+        def __python_expr_or_int(c, i):
             return isinstance(i, PythonExpression) or isinstance(i, int)
 
-        def __write_expr(c, i):
+        def __python_expr_or_str(c, i):
             return isinstance(i, PythonExpression) or isinstance(i, str)
 
+        def __python_expr_or_str_or_number(c, i):
+            return (
+                isinstance(i, PythonExpression)
+                or isinstance(i, str)
+                or isinstance(i, int)
+                or isinstance(i, float)
+            )
+
         type_checker = Draft7Validator.TYPE_CHECKER.redefine_many(
             Map(
                 __version=__version,
-                __time_condition=__time_condition,
-                __write_expr=__write_expr,
+                __python_expr_or_int=__python_expr_or_int,
+                __python_expr_or_str=__python_expr_or_str,
+                __python_expr_or_str_or_number=__python_expr_or_str_or_number,
             )
         )
         ConfigValidator = extend(Draft7Validator, type_checker=type_checker)
         validator = ConfigValidator(self.schema)
         errors = list(validator.iter_errors(self.raw_config))
 
         if errors:
             if throw_ex:
                 raise Exception(
                     f"The configuration file '{self.config_file}' is not valid!"
                 )
             return False, errors
         else:
-            self.check_dupplicates('topology.section.code')
-            self.check_dupplicates('topology.peripheral.pos')
-            self.check_dupplicates('simulator.sections.code')
+            self.check_dupplicates("topology.section.code")
+            self.check_dupplicates("topology.peripheral.pos")
+            self.check_dupplicates("simulator.sections.code")
             return True, None
 
     def get_dir_path(self, path, base_dir=None, check=False):
         """
         Return the full directory of the path with `config_dir` as the base directory.
         """
         return get_dir_path(self.config_dir, path, base_dir, check)
```

### Comparing `ja2mqtt-1.0.4/ja2mqtt/schemas/config-schema.yaml` & `ja2mqtt-1.0.5/ja2mqtt/schemas/config-schema.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 $schmea: "http://json-schema.org/draft-04/schema#"
-id: "ja2mqtt-config"
+id: "main-config"
 
 # root properties
 type: "object"
 required:
   - "version"
   - "ja2mqtt"
   - "mqtt-broker"
@@ -21,14 +21,31 @@
       - "address"
     additionalProperties: False
     properties:
       address:
         type: "string"
       port:
         type: "integer"
+      username:
+        type: "string"
+      password:
+        type: "string"
+      clean_session:
+        type: "boolean"
+      transport:
+        type: "string"
+        enum:
+          - "tcp"
+          - "websockets"
+      protocol:
+        type: "string"
+        enum:
+          - "MQTTv311"
+          - "MQTTv31"
+
   logs:
     type: "string"
 
   # serial interface properties
   serial:
     type: "object"
     required:
@@ -144,11 +161,10 @@
           type: "object"
           required:
             - "time_next"
             - "write"
           additionalProperties: False
           properties:
             time_next:
-              type: "__time_condition"
+              type: "__python_expr_or_int"
             write:
-              type: "__write_expr"
-            
+              type: "__python_expr_or_str"
```

### Comparing `ja2mqtt-1.0.4/ja2mqtt/utils.py` & `ja2mqtt-1.0.5/ja2mqtt/utils.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.4/ja2mqtt.egg-info/PKG-INFO` & `ja2mqtt-1.0.5/ja2mqtt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: ja2mqtt
-Version: 1.0.4
+Version: 1.0.5
 Summary: Jablotron MQTT bridge
+Home-page: UNKNOWN
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
+License: UNKNOWN
+Description: ja2mqtt is a bridge that connects a Jablotron control unit, extended with the [JA-121T RS-485 bus interface](https://www.jablotron.com/en/produkt/rs-485-bus-interface-426/), to an MQTT broker.
+        
+        ja2mqtt enables the use of MQTT events to control Jablotron events, allowing for seamless integration with MQTT-based IoT systems and platforms. With this bridge, Jablotron alarms can be integrated into a larger IoT ecosystem, alongside other devices that use industry-standard protocols like ZigBee or MQTT. For example, by using ja2mqtt in conjunction with ZigBee2MQTT, Jablotron alarms and ZigBee devices can be connected in a single network and integrated with other systems such as Alexa, Tahoma, or Google Assistant, providing a unified and interoperable smart home or industrial automation solution.
+        
+        ja2mqtt reads input from the JA-121T serial interface, converts it into MQTT events, and publishes them to the MQTT broker using defined MQTT topics. It utilizes a ja2mqtt definition file that outlines the implementation of the JA-121T protocol. Additionally, ja2mqtt defines MQTT events that can be converted into input for the JA-121T serial interface, such as changing the state of a section to ARMED or READY. Each MQTT request may contain a correlation ID that is copied to the corresponding generated MQTT event.
+        
+        If you do not have access to a JA-121T interface for testing, ja2mqtt offers a simulator that can simulate the interaction with the JA-121T interface. This allows you to test and verify the functionality of ja2mqtt even without the physical JA-121T interface available.
+        
+        See https://github.com/tomvit/ja2mqtt for more details.
+        
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6.0
-License-File: LICENSE
-
-ja2mqtt is a bridge that connects a Jablotron control unit, extended with the [JA-121T RS-485 bus interface](https://www.jablotron.com/en/produkt/rs-485-bus-interface-426/), to an MQTT broker.
-
-ja2mqtt enables the use of MQTT events to control Jablotron events, allowing for seamless integration with MQTT-based IoT systems and platforms. With this bridge, Jablotron alarms can be integrated into a larger IoT ecosystem, alongside other devices that use industry-standard protocols like ZigBee or MQTT. For example, by using ja2mqtt in conjunction with ZigBee2MQTT, Jablotron alarms and ZigBee devices can be connected in a single network and integrated with other systems such as Alexa, Tahoma, or Google Assistant, providing a unified and interoperable smart home or industrial automation solution.
-
-ja2mqtt reads input from the JA-121T serial interface, converts it into MQTT events, and publishes them to the MQTT broker using defined MQTT topics. It utilizes a ja2mqtt definition file that outlines the implementation of the JA-121T protocol. Additionally, ja2mqtt defines MQTT events that can be converted into input for the JA-121T serial interface, such as changing the state of a section to ARMED or READY. Each MQTT request may contain a correlation ID that is copied to the corresponding generated MQTT event.
-
-If you do not have access to a JA-121T interface for testing, ja2mqtt offers a simulator that can simulate the interaction with the JA-121T interface. This allows you to test and verify the functionality of ja2mqtt even without the physical JA-121T interface available.
-
-See https://github.com/tomvit/ja2mqtt for more details.
-
```

### Comparing `ja2mqtt-1.0.4/setup.py` & `ja2mqtt-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # required modules
 install_requires = [
     'click>=8.0.4',
     'Jinja2>=3.0.3',
     'paho-mqtt>=1.6.1',
     'pyserial>=3.5',
     'PyYAML>=6.0',
-    'jsonschema>=4.17.3'
+    'jsonschema>=4.0.0'
 ]
 
 setup(
     name='ja2mqtt',
     version=__version__,
     description='Jablotron MQTT bridge',
     long_description=read('README-pypi.text'),
```

